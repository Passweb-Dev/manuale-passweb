# UPLOAD DELLE RISORSE ARTICOLO



Il metodo in questione consente di automatizzare l'upload delle risorse
articolo.

**Metodo da richiamare**: UploadRisorseArticoli

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo UploadRisorseArticoli richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **separatore**: intero indicante il separatore. I valori ammessi sono:

  - 1: punto e virgola

  - 2: virgola

  - 3: tabulazione

- **file**: array di byte del file .zip

**ATTENZIONE!** Il file .zip dovrà essere generato secondo le stesse
regole utilizzate per la creazione dell'analogo file utilizzato per
uplodare le risorse articolo direttamente dal Back End di Passweb

**ATTENZIONE!** saranno accettate solo ed esclusivamente immagini di
peso inferiore a 1 MB

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al Webservices

- **Chiave ripetuta**: se il Webservices è stato richiamato più volte
  con la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il separatore indicato non è valido**: se il separatore non è uno
  dei valori ammessi

- **Il file .zip non è corretto**: se il file .zip non può essere
  decompresso

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito-\>Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

byte\[\] file = File.ReadAllBytes(@\"C:\\articoli.zip\");

> try
>
> {
>
> proxySiteMethod.UploadRisorseArticoli(chiaveCriptata, 1, file);
>
> }
>
> catch (Exception exc)
>
> {
>
> string errore = exc.Message;
>
> }
>
> finally
>
> {
>
> proxySiteMethod.Dispose();
>
> }

