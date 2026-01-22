# TAG DI TRACCIAMENTO DI GA4 / ADS CON USER PROVIDED DATA



Una volata creata la variabile di tipo User Provided Data che, come
visto nel precedente capitolo di questo manuale, di fatto, raggruppa in
sé tutti i dati di prima parte forniti dagli utenti che hanno prestato i
relativi consensi e che sono stati inseriti nel dataLayer gestito da
Passweb, questa stessa variabile potrà ora essere utilizzata in fase di
configurazione dei vari Tag di tracciamento Google e / o AdWords per
fare in modo di inoltrare anche a queste piattaforme i dati utente
necessari per gestire le conversioni avanzate.

In questo senso infatti, tanto nella maschera di configurazione dei Tag
di tipo **Google Ads Conversion Tracking** quanto in quella dei Tag di
tipo **Google Analytics: GA4 Events** troveremo un parametro "**Include
user-provided data from your website**"

![](./assets/media/image204.png)

![](./assets/media/image205.png)

che sarà esattamente quello da dover selezionare per fare in modo di
inviare i dati utente necessari per le conversioni avanzate alla
relativa piattaforma.

Selezionando tale parametro verrà visualizzato un ulteriore campo dove
dovremo inserire, selezionandola dall'apposito menu a tendina, la
variabile di tipo User Provided Data utilizzata per raccogliere tutti i
dati utente

![](./assets/media/image206.png)

**ATTENZIONE!** Il campo in oggetto accetta solo ed esclusivamente
variabili di tipo "User Provided data" (ecco perché si è reso necessario
creare in precedenza una variabile di questo tipo)

Nel momento in cui la variabile di tipo User Provided Data non fosse
ancora stata creata, sarebbe comunque possibile crearla direttamente in
questa fase, cliccando per questo sull'opzione "New Variable" e seguendo
la procedura descritta nei precedenti capitoli di questo manuale.

Un'ultima cosa di fondamentale importanza da tenere sempre in
considerazione è che il fatto di aver configurato tutto in maniera
corretta, prelevando i dati utente dal dataLayer di Passweb con le
apposite variabili di livello dati, creando l'apposita variabile di tipo
User Provided Data e configurando correttamente i vari Tag di
tracciamento per fare in modo che questi tengano conto anche dei dati
presenti all'interno di questa variabile, di per sé potrebbe non bastare
per gestire tanto su GA4 quanto su Google Ads le conversioni avanzate.

**Oltre a configurare in maniera corretta gli strumenti di tracciamento,
per poter gestire le conversioni avanzate su Google Ads piuttosto che su
Google Analytics sarà infatti indispensabile attivare le funzionalità di
raccolta dati utente e delle conversioni avanzate anche sulla relativa
piattaforma di tracciamento.**

In sostanza dunque se anche avessimo configurato tutto correttamente e
il nostro sistema di tracciamento dovesse effettivamente inviare i dati
utente ad esempio a Google Ads, ma Goole Ads stesso non fosse
configurato per gestire le conversioni avanzate e per ricevere quindi
questo tipo di datti di fatto questi finirebbero nel nulla e sarebbe
come non averli inviati affatto.

Per maggiori informazioni relativamente all'attivazione in Google
Analytics della raccolta dei dati utente e della gestione delle
conversioni avanzate si veda anche quanto indicato all'interno del
capitolo "*Google Analytics -- Google Analytics 4 -- GA4 User Provided
Data e Conversioni Avanzate*" di questo manuale.

Per quanto riguarda invece l'attivazione delle conversioni avanzate in
Google Ads si veda quanto indicato all'interno del capitolo "*Google Ads
User Provided Data e Conversioni Avanzate*" di questo manuale

**ATTENZIONE!** si ricorda che, in ogni caso, lo scopo del presente
manuale non è ovviamente quello di fornire una documentazione esaustiva
e dettagliata relativamente all'utilizzo di piattaforme quali Google
Analytics o Google Ads per cui il consiglio è sempre quello di fare
riferimento, per l'attivazione e la gestione di determinate funzionalità
di queste piattaforme, alla documentazione ufficiale presente in rete e
fornita direttamente da Google

