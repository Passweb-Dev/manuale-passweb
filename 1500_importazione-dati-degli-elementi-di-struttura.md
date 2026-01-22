# IMPORTAZIONE DATI DEGLI ELEMENTI DI STRUTTURA



Il metodo in questione consente di automatizzare il processo di
importazione dei dati degli elementi dei campi di struttura, evitando
dunque di dover effettuare lo stesso tipo di operazione in maniera
manuale all'interno del Wizard (mediante importazione di apposito file
csv).

**Metodo da richiamare**: UploadDatiElementiCampoStruttura

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo UploadDatiElementiCampoStruttura richiede i seguenti
parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **codiceStruttura**: codice della struttura, visibile nella griglia
  del Wizard in "**Catalogo -- Strutture**" in relazione al campo
  "Codice"

- **codiceCampoStruttura**: codice del campo della struttura, visibile
  nella griglia del Wizard in "**Catalogo -- Strutture -- Modifica
  Elementi Struttura**" in relazione al campo "Codice"

- **separatore**: intero indicante il separatore. I valori ammessi sono:

  - 1: punto e virgola

  - 2: virgola

  - 3: tabulazione

- **lingua**: codice iso della lingua che dovrà essere utilizzata per il
  salvataggio dei dati degli elementi del campo struttura

- **file**: stringa rappresentante il contenuto del file

- **raggruppatoCodice** (booleano): consente di indicare se all'interno
  del file da uplodare gli elementi di personalizzazione sono
  raggruppati per codice o distinti per singolo articolo padre

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al Webservice

- **Chiave ripetuta**: se il Webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **Il codice struttura indicato non è valido**: se il campo
  \<codiceStruttura\> non è valido

- **Il codice del campo struttura indicato non è valido**: se il campo
  \<codiceCampoStruttura\> non è valido

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

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

using (SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\"))

{

try

{ string file = File.ReadAllText(@\"C:\\demo.csv\", Encoding.UTF8);
siteMethod.UploadDatiElementiCampoStruttura(chiaveCriptata, 8, 3, 1,
\"it\", file, true); }

catch (Exception exc)

{ string errore = exc.Message; }

}

