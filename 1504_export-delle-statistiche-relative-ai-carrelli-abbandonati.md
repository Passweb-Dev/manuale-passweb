# EXPORT DELLE STATISTICHE RELATIVE AI CARRELLI ABBANDONATI



Il metodo in questione consente di automatizzare la procedura di export
delle Statistiche Passweb relative ai carrelli abbandonati, evitando
quindi all'utente di dover effettuare questo tipo di operazione agendo
manualmente all'interno del Wizard.

**Metodo da richiamare: ExportCarrelliAbbandonati**

**Url del Webservice: \<url-sito\>/SiteMethod/SiteMethod.asmx**

Il metodo ExportCarrelliAbbandonati richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **dataInizio**: data di inizio delle statistiche

- **dataFine**: data di fine delle statistiche

- **tipologia**: tipologia. I valori ammessi sono:

  - 0 = Elenco Carrelli

  - 1 = Elenco Righe

  - 2 = Elenco Articoli e Quantità

  - 3 = Elenco Articoli e Utenti

  - 4 = File Import Carrello

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta**: se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **La tipologia indicata non è valida**: se il campo \<tipologia\> non
  ha un valore ammesso

**La procedura restituisce l\'array di byte del file csv.**

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

byte\[\] csv = proxySiteMethod.ExportCarrelliAbbandonati(chiaveCriptata,
new DateTime(2021, 1, 1), new DateTime(2021, 5, 1), 0);

}

catch (Exception exc)

{

string errore = exc.Message;

}

}

