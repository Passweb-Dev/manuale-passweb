# DOWNLOAD DEI DATI DI CATEGORIA



Il metodo in questione consente di automatizzare il download dei dati
relativi alle categorie merceologiche gestite all'interno del sito.

**Metodo da richiamare**:DownloadDatiCategorie

**Url del Webservice:** \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo DownloadDatiCategorie richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **separatore**: intero indicante il separatore. I valori ammessi sono:

  - 1: punto e virgola

  - 2: virgola

  - 3: tabulazione

- **lingua**: codice iso della lingua che dovrà essere utilizzata per il
  reperimento dei dati di categoria

Il metodo restituisce una stringa contenente i dati delle categorie.

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta**: se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il separatore indicato non è valido**: se il separatore non è uno
  dei valori ammessi

- **Indicare il codice ISO della lingua**: se il campo \<lingua\> è
  vuoto

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

try

{

string file = proxySiteMethod.DownloadDatiCategorie(chiaveCriptata, 1,
\"it\");

}

catch (Exception exc)

{

string errore = exc.Message;

}

