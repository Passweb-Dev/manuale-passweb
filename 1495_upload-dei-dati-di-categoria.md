# UPLOAD DEI DATI DI CATEGORIA



Il metodo in questione consente di automatizzare l\'upload dei dati
relativi alle categorie merceologiche gestite all'interno del sito.

**Metodo da richiamare**:UploadDatiCategorie

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo UploadDatiCategorie richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **separatore**: intero indicante il separatore. I valori ammessi sono:

  - 1: punto e virgola

  - 2: virgola

  - 3: tabulazione

- lingua: codice iso della lingua che dovrà essere utilizzata per il
  salvataggio dei dati di categoria

- **file**: stringa rappresentante il contenuto del file

**ATTENZIONE!** I campi gestibili nel file csv sono gli stessi
utilizzati per l\'upload dei dati di categoria da Wizard (per maggiori
informazioni in merito si veda quanto indicato all'interno del capitolo
"*Catalogo -- Gestione Articoli -- Articoli -- Categoria Merceologiche
-- Importazione / Esportazione massiva dei dati*")

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta**: se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il separatore indicato non è valido**: se il separatore non è uno
  dei valori ammessi

- **Indicare il testo del file**: se il campo \<file\> è vuoto

- **Indicare il codice ISO della lingua**: se il campo \<lingua\> è
  vuoto

- **Altri errori relativi alla non correttezza del campo \<file\>**

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

string file = File.ReadAllText(@\"C:\\demo.csv\", Encoding.UTF8);

try

{

proxySiteMethod.UploadDatiCategorie(chiaveCriptata, 1, \"it\", file);

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

