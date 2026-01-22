# DOWNLOAD DATI FORM



Il metodo in questione consente di automatizzare il download di
eventuali file xml o csv in cui vengono salvati i dati inseriti dagli
utenti del sito compilando determinati Form presenti sul sito stesso.

Il Webservice consente anche di effettuare il download di eventuali
allegati al form

**Metodo da richiamare:** DownloadForm

**Url del Webservice:** \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo DownloadForm richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **idForm**: identificativo del form (reperibile dal Wizard alla voce
  di menù Utenti-\>Gestione Forms)

La procedura può generare i seguenti errori:

- Funzionalità non disponibile: se il contratto non prevede chiamate al
  webservice

- Chiave ripetuta: se il webservice è stato richiamato più volte con la
  stessa chiave

- Chiave errata: se i dati contenuti nella chiave non sono del numero
  voluto o se le credenziali contenute sono errate

- L\'identificativo del form non è corretto o per il form non viene
  gestito nessun file: se l'identificativo passato non è valido o è
  relativo ad un form che non viene gestito tramite file

Il metodo restituisce l'array di byte del file zip. Se non ci sono
iscritti al form, viene restituito null.

Di seguito un esempio del codice scritto in C# per ottenere lo zip di un
form.

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

int idForm = 15;

using(SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\"))

{

try

{

proxySiteMethod.DownloadForm(chiaveCriptata, idForm);

}

catch (Exception exc)

{

string errore = exc.Message;

}

}

