# LETTURA SALDO PUNTI UTENTE



Il metodo in questione consente di automatizzare, in relazione ad un
determinato sistema di raccolta punti, le operazioni di lettura del
saldo punti dei vari utenti del sito

**Metodo da richiamare**: GetPuntiCliente

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo GetPuntiCliente richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **idRaccoltaPunti**: identificativo della raccolta punti, prelevabile
  dal Wizard

- **cliente**: codice del cliente di cui leggere il saldo

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

- **Il codice cliente indicato non è presente sul sito**: se per il
  campo \<cliente\> è stato indicato un codice non presente sul sito

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

decimal saldo = proxySiteMethod.GetPuntiCliente(chiaveCriptata, 1,
\"501.00001\");

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
consentire la lettura del saldo punti anche in relazione ad utenti che
non sono ancora clienti e che non hanno quindi un loro codice
gestionale)

**Metodo da richiamare**: GetPuntiUtente

**Url del Webservice**: \<url-sito\>/SiteMethod/SiteMethod.asmx

Il metodo GetPuntiUtente richiede i seguenti parametri:

- **chiave**: chiave criptata contenente la login di un utente del
  Wizard (sia di tipologia Amministratore che di tipologia Utente)

> **ATTENZIONE!** per maggiori informazioni sull'utilizzo di questo
> parametro si veda anche quanto indicato all'interno del precedente
> capitolo "*Chiave WebService*"

- **idRaccoltaPunti**: identificativo della raccolta punti, prelevabile
  dal Wizard

- **idUtente**: identificativo dell\'utente di cui leggere il saldo

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

- **L'identificativo utente indicato non è presente sul sito**: se per
  il campo \<idUtente\> è stato indicato un identificativo non presente
  sul sito

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

decimal saldo = proxySiteMethod.GetPuntiUtente(chiaveCriptata, 1, 28);

}

catch (Exception exc)

{

string errore = exc.Message;

}

finally

{

proxySiteMethod.Dispose();

}

