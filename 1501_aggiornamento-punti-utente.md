# AGGIORNAMENTO PUNTI UTENTE



Il metodo in questione consente di automatizzare, in relazione ad un
determinato sistema di raccolta punti, l'aggiornamento del saldo punti
utente, evitando così di dover effettuare la stessa operazione in
maniera manuale dal Wizard di Passweb.

**Metodo da richiamare**: TransazionePuntiCliente

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo TransazionePuntiCliente richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **idRaccoltaPunti**: identificativo della raccolta punti, prelevabile
  dal Wizard

- **punti**: numero dei punti. Il numero può essere sia positivo che
  negativo

- **cliente**: codice del cliente a cui assegnare i punti

- **scadenza**: data di scadenza dei punti. NULL se i punti non scadono

- **nota**: nota

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta**: se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **L'identificativo della raccolta punti indicato non è presente sul
  sito**: se per il campo \<idRaccoltaPunti\> è stato indicato un
  identificativo non presente

- **Specificare il numero dei punti**: se il campo \<punti\> è impostato
  a zero

- **Specificare il codice del cliente a cui associare i punti**: se il
  campo \<cliente\> è vuoto o NULL

- **Il codice cliente indicato non è presente sul sito**: se per il
  campo \<cliente\> è stato indicato un codice non presente sul sito

- **Saldo punti negativo - Transazione punti non ammessa**: se
  conteggiando i punti indicati per la transazione il saldo del cliente
  risulterebbe negativo

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito→Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

try

{

proxySiteMethod.TransazionePuntiCliente(chiaveCriptata, 1, 2,
\"501.00001\", null, \"Bonus\");

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

E' disponibile inoltre un metodo del tutto speculare a quello appena
analizzato che utilizza però come parametro di ingresso non più il
codice cliente ma bensì l'identificativo Passweb dell'utente (questo per
consentire di assegnare punti anche ad utenti che non sono ancora
clienti e che non hanno quindi un loro codice gestionale)

**Metodo da richiamare**: TransazionePuntiUtente

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo TransazionePuntiUtente richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **idRaccoltaPunti**: identificativo della raccolta punti, prelevabile
  dal Wizard

- **punti**: numero dei punti. Il numero può essere sia positivo che
  negativo

- **idUtente**: identificativo dell\'utente a cui assegnare i punti

- **scadenza**: data di scadenza dei punti. NULL se i punti non scadono

- **nota**: nota

La procedura può generare i seguenti errori:

- **Funzionalità non disponibile**: se il contratto non prevede chiamate
  al webservice

- **Chiave ripetuta**: se il webservice è stato richiamato più volte con
  la stessa chiave

- **Chiave errata**: se i dati contenuti nella chiave non sono del
  numero voluto o se le credenziali contenute sono errate

- **L'identificativo della raccolta punti indicato non è presente sul
  sito**: se per il campo \<idRaccoltaPunti\> è stato indicato un
  identificativo non presente

- **Specificare il numero dei punti**: se il campo \<punti\> è impostato
  a zero

- **L'identificativo utente indicato non è presente sul sito**: se per
  il campo \<idUtente\> è stato indicato un identificativo non presente
  sul sito

- **Saldo punti negativo - Transazione punti non ammessa**: se
  conteggiando i punti indicati per la transazione il saldo del cliente
  risulterebbe negativo

**[CHIAMATA AL WEBSERVICE]{.underline}**

string separatore = \"#!\$\";

**//Chiave indicata sul Wizard di Passweb in \"Sito→Preferenze\"**

string chiaveWebService = \"k!3d4tsjk!3d4tsjk!3d4tsjk!3d4tsj\";

SiteMethod proxySiteMethod = new
SiteMethod(\"http://www.sitodemo.passweb.it/SiteMethod/SiteMethod.asmx\");

Crypt crypto = new Crypt(chiaveWebService);

string chiaveCriptata = crypto.Encrypt(\"login\" + separatore +
DateTime.Now.Ticks.ToString());

try

{

proxySiteMethod.TransazionePuntiUtente(chiaveCriptata, 1, 2, 28, null,
\"Bonus\");

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

