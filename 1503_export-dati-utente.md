# EXPORT DATI UTENTE



Il metodo in questione consente di automatizzare la procedura di export
dei "Dati Utente".

**Metodo da richiamare: DownloadDatiUtenti**

**Url del Webservice: \<url-sito\>/SiteMethod/SiteMethod.asmx**

Il metodo DownloadDatiUtenti richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **separatore**: intero indicante il separatore. I valori ammessi sono:

  - 1: punto e virgola

  - 2: virgola

  - 3: tabulazione

- **campi (opzionale)**: array di campi che dovranno essere presenti nel
  csv. Se NULL, nel csv saranno presenti tutti i campi gestibili.

> I campi gestibili nel file csv sono gli stessi utilizzati per la
> procedura di export dei dati utente disponibile tramite Wizard di
> Passweb

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta:** se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata:** se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il separatore indicato non è valido:** se il separatore non è uno
  dei valori ammessi

- **Il campo \<campo\> non è gestito:** se uno dei campi presenti
  nell'array \<campi\> non è gestito

**La procedura restituisce l\'array di byte del file csv.**

**Se nell\'elenco dei campi indicati sono presenti anche campi di tipo
\"File\", l\'array di byte sarà relativo ad uno zip.**

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

string\[\] campi = new string\[\] { \"codiceIntegrazione\",
\"codiceFiscale\" };

using (SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\"))

{

try

{

byte\[\] csv = proxySiteMethod.DownloadDatiUtenti(chiaveCriptata, 1,
campi);

}

catch (Exception exc)

{

string errore = exc.Message;

}

}

