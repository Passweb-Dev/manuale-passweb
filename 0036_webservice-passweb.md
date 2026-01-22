# WEBSERVICE PASSWEB



La sezione WebService Passweb consente di configurare le chiavi di
attivazione da utilizzare per poter effettuare delle chiamate ai
Webservices messi a disposizione dall'applicativo.

![](./assets/media/image64.png)

Nello specifico, il campo:

**Chiave WebService:** consente di impostare la chiave da utilizzare
nelle chiamate ai Webservice di Passweb.

**ATTENZIONE!** La chiave deve essere lunga 32 caratteri. In caso di
lunghezza inferiore i restanti caratteri saranno degli spazi vuoti

Per maggiori informazioni relativamente a quelle che sono poi le
procedure che si possono automatizzare mediante i Webservices di Passweb
si rimanda a quanto indicato all'interno del capitolo "*Developer*" di
questo manuale.

**Chiave Gestionale WebService**: consente di impostare la chiave che
dovrà essere utilizzata per validare le chiamate che le varie App
Gestionali (Mexal e Retail) possono effettuare verso il relativo sito
Passweb. Tale chiave può anche essere generata in maniera automatica
cliccando sul corrispondente pulsante "**Genera Chiave**"

**Ovviamente la chiave inserita all'interno del campo "Chiave Gestionale
WebService" dovrà essere poi riportata anche all'interno dell'apposito
campo presente nei parametri di configurazione delle relative App
Gestionali**

In merito alle App Gestionali che possono interagire, mediante la chiave
in questione, con il corrispondente sito Passweb si rimanda alla
relativa documentazione di prodotto.

Per quel che riguarda Mexal l'App interessata è "**Sync articoli
Passweb**" disponibile all'interno di Passstore
(<https://passstore.passepartout.net/Apps/Detail/sync-articoli-passweb/583>)

![](./assets/media/image65.png)

Per quel che riguarda Retail invece la funzionalità interessata è
relativa alla possibilità di creare un'apposita Operazione Pianificata
che ha come destinatario il sito Ecommerce collegato al gestionale.

In entrambi i casi l'obbiettivo è quello di comunicare a Passweb
l'elenco di articoli che sono stati movimentati a seguito della
creazione di specifici documenti direttamente all'interno del gestionale
per fare in modo che Passweb possa poi andare a rileggere dalle basi
dati del gestionale le nuove disponibilità senza dover attendere la
prossima sincronizzazione schedulata.

**ATTENZIONE!** Per installazioni Passweb in hosting condiviso il numero
di chiamate orarie accettate è limitato a 30. Raggiunto tale limite
occorrerà attendere l'intervallo successivo prima di poter nuovamente
aggiornare la disponibilità di determinati articoli a seguito di ordini
effettuati all'interno del gestionale.

