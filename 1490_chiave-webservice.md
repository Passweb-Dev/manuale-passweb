# CHIAVE WEBSERVICE



I metodi pubblici messi a disposizione dai Webservices di Passweb ed
elencati nei successivi capitoli di questo manuale, richiedono
l'utilizzo di un parametro "**chiave**" indispensabile per poterne
consentire l'utilizzo.

La chiave da utilizzare in questi metodi è formata da:

**login + separatore + datetime.ticks**

dove:

- **Login** deve essere lo username di un utente del Wizard di tipo
  Amministratore o Utente

- **separatore** dovrà essere la stringa "#!\$"

- **DateTime.ticks** rappresentano i segni di graduazione della data e
  dell'ora attuali. Un singolo segno di graduazione rappresenta cento
  nanosecondi. Questo numero serve per evitare che il metodo del
  WebService venga richiamato più volte con la stessa chiave.

**ATTENZIONE!** La chiave deve essere criptata con l'algoritmo **AES**.

Questo algoritmo dovrà utilizzare come chiave quella indicata sul Wizard
alla voce di menu "**Sito -- Preferenze**" nel campo "**Chiave
WebService**" (chiave lunga 32 caratteri: se la lunghezza è inferiore
verranno aggiunti degli spazi vuoti) , e come vettore la stringa
"**Versione PSW 001**".

Di seguito un esempio di chiamata a questi WebService e la classe da
utilizzare per criptare e decriptare i dati:

**[ESEMPIO CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

try

{

proxySiteMethod.\<NOME_METODO\>(chiaveCriptata, ...);

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

**[CLASSE CRYPT PER CRIPTARE E DECRIPTARE]{.underline}**

public class Crypt

{

private const string vettore = \"Versione PSW 001\";

private SymmetricAlgorithm algoritmoCriptazione;

/// \<summary\>

/// Costruttore

/// \</summary\>

/// \<param name=\"\_chiave\"\>chiave webservice\</param\>

public Crypt(string \_chiave)

{

algoritmoCriptazione = Aes.Create();

algoritmoCriptazione.Key =
ASCIIEncoding.ASCII.GetBytes(\_chiave.PadRight(32, \' \'));

algoritmoCriptazione.IV =
ASCIIEncoding.ASCII.GetBytes(vettore.PadRight(16, \' \'));

}

/// \<summary\>

/// Metodo che cripta il testo con l\'algoritmo AES

/// \</summary\>

/// \<param name=\"\_testo\"\>testo da criptare\</param\>

/// \<returns\>testo criptato\</returns\>

public string Encrypt(string \_testo)

{

if (\_testo == null \|\| \_testo.Length == 0)

return \"\";

//Conversione stringa in vettore di byte

byte\[\] bytIn = System.Text.ASCIIEncoding.ASCII.GetBytes(\_testo);

//Creazione di uno stream in memoria

System.IO.MemoryStream ms = new System.IO.MemoryStream();

//Creazione stream per la criptazione

CryptoStream cs = new CryptoStream(ms,
algoritmoCriptazione.CreateEncryptor(),CryptoStreamMode.Write);

//Scrittura nello stream in memoria del testo criptato

cs.Write(bytIn, 0, bytIn.Length);

cs.FlushFinalBlock();

//Conversione in base 64 in modo da poter usare la stringa criptata
ovunque

return System.Convert.ToBase64String(ms.GetBuffer(), 0, (int)ms.Length);

}

/// \<summary\>

/// Metodo che decripta il testo con l\'algoritmo AES

/// \</summary\>

/// \<param name=\"\_testo\"\>testo da decriptare\</param\>

/// \<returns\>testo decriptato\</returns\>

public string Decrypt(string \_testo)

{

if (\_testo == null \|\| \_testo.Length == 0)

return \"\";

//Conversione della stringa in vettore di byte

byte\[\] bytIn = System.Convert.FromBase64String(\_testo);

//Creazione di uno stream in memoria

System.IO.MemoryStream ms = new System.IO.MemoryStream(bytIn, 0,
bytIn.Length);

//Creazione stream per la decriptazione

CryptoStream cs = new CryptoStream(ms,
algoritmoCriptazione.CreateDecryptor(), CryptoStreamMode.Read);

StreamReader sr = new StreamReader(cs);

string ret = sr.ReadToEnd();

sr.Close();

cs.Close();

ms.Close();

return ret;

}

}

