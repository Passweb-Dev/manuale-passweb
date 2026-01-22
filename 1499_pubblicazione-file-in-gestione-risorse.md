# PUBBLICAZIONE FILE IN GESTIONE RISORSE



Il metodo in questione consente di automatizzare il processo di
pubblicazione file in "Gestione Risorse" del sito, evitando dunque di
dover effettuare lo stesso tipo di operazione in maniera manuale
all'interno del Wizard.

**Metodo da richiamare**: PubblicazioneFileInGestioneRisorse

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo PubblicazioneFileInGestioneRisorse richiede i seguenti
parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **cartelle**: array di cartelle che definiscono il percorso della
  cartella di destinazione. Se il percorso non esiste viene creato.

- **file**: array di byte del file

- **nomeFile**: nome del file, compresa l'estensione

- **archivio** (booleano): true se il file è uno zip da decomprimere,
  false altrimenti

**ATTENZIONE!** Il file .zip dovrà essere generato secondo le stesse
regole utilizzate per la creazione dell'analogo file utilizzato per
uplodare risorse manualmente dal Back End di Passweb

**ATTENZIONE!** in relazione a risorse di tipo immagine (bmp, jpeg, png
...) verranno accettati solo ed esclusivamente file di peso inferiore a
1 MB

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al Webservices

- **Chiave ripetuta**: se il Webservices è stato richiamato più volte
  con la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il file è vuoto**: se l'array di byte del campo \<file\> è vuoto

- **Indicare il nome del file**: se il campo \<nomeFile\> è vuoto

- **Il nome del file deve includere l'estensione**: se il campo
  \<nomeFile\> non comprende l'estensione del file

- **Tipologia di file non ammessa**: se il file ha estensione .exe

- **Spazio su disco esaurito**: se lo spazio su disco previsto da
  contratto è stato esaurito

- **Indicare almeno una cartella**: se l'array di stringhe del campo
  \<cartelle\> è vuoto

- **I file di tipo Archivio consentiti sono solo quelli con estensione
  .zip**: se "archivio" è impostato a "true" ed in "nomeFile" non è
  stato indicato un file .zip.

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

using (SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\"))

{

try

{

string\[\] folder = new string\[\]

{ \"CARTELLA\", \"SOTTOCARTELLA\" }

;

byte\[\] file = File.ReadAllBytes(@\"C:\\demo.pdf\");

string nomeFile = \"demo.pdf\";

proxySiteMethod.PubblicazioneFileInGestioneRisorse(chiaveCriptata,
folder, file, nomeFile, false);

}

catch (Exception exc)

{ string errore = exc.Message; }

}

