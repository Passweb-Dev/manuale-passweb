# PUBBLICAZIONE DOCUMENTI IN AREA RISERVATA



Il metodo in questione consente di automatizzare la procedura di
caricamento file in apposite cartelle dell'area riservata del proprio
sito Passweb (sezione Documenti)

**Metodo da richiamare:** PubblicazioneFileInFolder

**Url del Webservice:** \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo **PubblicazioneFileInFolder** richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **cartelle**: array di cartelle che definiscono il percorso della
  cartella di destinazione a partire dalla radice (la cartella deve
  essere già presente, non viene creata)

- **file**: array di byte del file

- **nomeFile**: nome del file, compresa l'estensione

La procedura può generare i seguenti errori:

- Funzionalità non disponibile: se il contratto non prevede chiamate al
  webservice

- Chiave ripetuta: se il webservice è stato richiamato più volte con la
  stessa chiave

- Chiave errata: se i dati contenuti nella chiave non sono del numero
  voluto o se le credenziali contenute sono errate

- Il file è vuoto: se l'array di byte del campo \<file\> è vuoto

- Tipologia di file non ammessa: se il file ha estensione .exe

- Spazio su disco esaurito: se lo spazio su disco previsto da contratto
  è stato esaurito

- Indicare almeno una cartella: se l'array di stringhe del campo
  \<cartelle\> è vuoto

- La cartella \<cartella\> non esiste: se una cartella indicata
  nell'array non esiste sul sito

- Indicare il nome del file: se il campo \<nomeFile\> è vuoto

- Il nome del file deve includere l'estensione: se il campo \<nomeFile\>
  non comprende l'estensione del file

**ATTENZIONE!** Le cartelle indicate nel parametro \<cartelle\> devono
essere già presenti nella sezione Documenti dell'Area Riservata del
sito.

Se nella cartella è già presente un file con il nome indicato nel
parametro \<nomeFile\>, il file viene sovrascritto.

Il file viene inserito nella cartella come se fosse lo stesso creatore
della cartella ad effettuare il suo upload in Area Riservata.

Se per la cartella è stato impostato un Amministratore, diverso dal
creatore della cartella, gli viene inviata la notifica di inserimento di
un nuovo file.

Di seguito un esempio del codice scritto in C# per pubblicare il file
"demo.pdf" nella cartella "cartella\\sottocartella".

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

string\[\] folder = new string\[\] { \"CARTELLA\", \"SOTTOCARTELLA\" };

byte\[\] file = File.ReadAllBytes(@\"C:\\demo.pdf\");

string nomeFile = \"demo.pdf\";

try

{

proxySiteMethod.PubblicazioneFileInFolder(chiaveCriptata, folder, file,
nomeFile);

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

