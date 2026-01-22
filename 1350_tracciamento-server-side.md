# TRACCIAMENTO SERVER SIDE



Come ormai dovrebbe essere noto a tutti, i sistemi di tracciamento
"tradizionali" (client-side) basano il loro funzionamento principalmente
sull'utilizzo dei cookie che vengono rilasciati ed installati nel
browser degli utenti.

Da questo punto di vista però, nel corso degli ultimi anni, le cose
stanno cambiando notevolmente rendendo sempre più difficile tracciare
quello che gli utenti fanno all'interno del nostro sito. I cookie di
terza parte (rilasciati cioè su di un dominio diverso da quello in uso
al sito che si intende tracciare), infatti, hanno già issato bandiera
bianca mentre quelli di prima parte hanno ridotto la loro vita a soli 7
giorni.

A dare una bella scossa a tutto il sistema (soprattutto a Facebook), ci
ha pensato poi iOS14. L'App Tracking Transparency ha praticamente più
che dimezzato la quantità e l'accuratezza di dati provenienti dalle
strategie di digital marketing, favorendo una maggiore tutela della
privacy dei suoi utenti.

Anche Google da parte sua ha annunciato che entro il 2023 (spostando
quindi di circa un anno la deadline inizialmente stabilita) lo stesso
Chrome inizierà a bloccare i cookie di terze parti aggiungendosi così
alla lista di browser che già lo fanno dopo Safari e Firefox.

In questo clima di rinnovamento, e con la prospettiva di non poter più
utilizzare i cookie (per lo meno non come eravamo abituati a fare) uno
strumento che giocherà un ruolo sempre più importante è, sicuramente,
quello del tracciamento server-side. Questo perché, a differenza del
tracciamento classico lato client, il Server-Side tracking agisce al di
fuori del browser operando direttamente da un server dedicato bypassando
quindi molte delle problematiche causate dal blocco dei cookie e
dall'avvento di iOS14.

Ora però prima di passare ad esaminare un po' più nel dettaglio in che
cosa consiste e come funziona a grandi linee il tracciamento server side
è di fondamentale importanza avere ben chiari, innanzitutto, quelli che
sono i concetti che stanno alla base del tracciamento "tradizionale"
client-side e questo anche in considerazione del fatto che**, in ogni
caso, il tracciamento server-side non andrà a sostituire in pianta
stabile il tracciamento lato client che siamo abituati ad utilizzare ma
si affiancherà ad esso andando ad introdurre un ulteriore livello (anche
di complessità) al nostro sistema di monitoraggio.**

Per comprendere meglio i concetti che stanno alla base del tracciamento
lato client tradizionale è possibile fare riferimento alla
documentazione ufficiale messa a disposizione da Google al seguente
indirizzo:

https://developers.google.com/tag-platform/tag-manager/server-side/intro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_23.bmp](./assets/media/image155.png)

In sostanza come evidenziato dalla figura sopra riportata, in un
tracciamento lato client "tradizionale" implementato, ad esempio,
mediante Google Tag Manager ci troveremo ad avere a che fare con un
Contenitore GTM di tipo Web installato in tutte le pagine del nostro
sito con all'interno tutta una serie di Tag variabili in base ai vari
tracciamenti che avremo deciso di implementare (Analytics, Facebook,
Hotjar, Googla Ads ...)

Ciascuno di questi Tag una volta attivato (al caricamento di una nuova
pagina o al verificarsi di un determinato evento) effettuerà delle
chiamate a servizi (endpoint) specifici che risiedono su server esterni
(i server di Google Analytics, quelli di Facebook ...). Tutte queste
chiamate saranno create e gestite interamente dal browser dell'utente
che visita il sito (per questo si parla di tracciamento lato client) e
per far si che tutto possa funzionare in maniera corretta ogni singolo
Tag di tracciamento che abbiamo implementato andrà ad installare sul
nostro sito una ben precisa libreria javascript indispensabile per
gestire le chiamate al relativo endpoint e per inviargli, nella maniera
in cui l'endpoint stesso richiede, tutti i dati di tracciamento

Riassumendo dunque:

- Ogni singolo Tag di tracciamento implementato all'interno di un
  Contenitore GTM di tipo Web installa sul nostro sito uno script che
  invia delle richieste ai server dell'azienda che fornisce il tag
  (Google, Facebook, Hotjar ...) e su cui risiedono i relativi endpoint

- L'azienda fornitrice del Tag (Google, Facebook, Hotjar ...) risponderà
  alle richieste provenienti dal nostro sito installando dei cookie (di
  prima/terza parte) sul dispositivo (Pc o Smartphone) dell'utente che
  naviga il sito. Questi cookie serviranno per acquisire determinate
  informazioni sull'utente (quali siti naviga, che interessi ha ...)
  informazioni queste che verranno poi trasmesse al sistema di
  tracciamento

- Tutte queste operazioni si svolgono interamente tramite il browser
  dell'utente quindi effettivamente lato client

Chiarito tutto ciò è ora semplice comprendere come, in questo contesto,
possano esserci effettivamente tutta una serie di problemi (alterazione
degli script da parte dei browser, blocco delle richieste in uscita dal
browser mediante appositi plugin adBlocker, consensi negati da parte
dell'utente all'installazione dei cookie, problemi di privacy
relativamente alle informazioni memorizzate nei cookie ...) che di fatto
sono quelli con cui abbiamo normalmente a che fare e che limitano i dati
e le informazioni di cui possiamo poi disporre all'interno del nostro
sistema di monitoraggio.

**ATTENZIONE!** abbiamo considerato come esempio un sistema di
tracciamento client-side implementato mediante GTM ma sarebbe
esattamente la stessa cosa se il sistema di tracciamento fosse
implementato direttamente e nativamente all'interno del sito

Anche nel momento in cui i vari script, come ad esempio Google
Analytics, fossero infatti inseriti direttamente sul sito senza
l'utilizzo di GTM il funzionamento di base sarebbe esattamente lo
stesso. Avremo sempre chiamate in uscita dal nostro sito (implementate
mediante l'utilizzo di apposite librerie javascript installate sul sito
stesso) verso specifici endpoint di tracciamento con la conseguente
installazione sul browser dell'utente di cookie di prima/terza parte

Avendo ben chiaro il meccanismo che sta alla base di un tracciamento
lato client "tradizionale" possiamo passare ora a vedere cosa cambia e
come effettivamente si modifica tutto il sistema con l'introduzione del
tracciamento server-side e, per questo, facciamo riferimento ancora una
volta alla documentazione ufficiale messa a disposizione da Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_24.bmp](./assets/media/image156.png)

Come si può osservare nella figura sopra riportata il tracciamento
server side introduce, rispetto al tracciamento lato client appena
analizzato, un ulteriore strato che si va a posizionare esattamente nel
mezzo tra il nostro sito web e gli endpoint verso cui devono essere
inviati i dati di tracciamento.

Questo ulteriore strato è costituito da un nuovo tipo di contenitore
GTM, un contenitore di tipo Server, che non è installato sul nostro sito
web ma che gira su di un server dedicato, diverso quindi da quello su
cui è hostato il sito ecommerce, e che può essere collocato su Google
Cloud Platform o in un qualsiasi altro ambiente (AWS, Azure, Stape.io
...) appositamente configurato per ospitare questa nuova tipologia di
contenitore GTM.

In ogni caso indipendentemente da dove decideremo di creare il server
dedicato ad ospitare il nuovo contenitore GTM, dalla figura sopra
riportata si comprende già, in maniera abbastanza chiara, come questo
nuovo elemento funzioni esattamente come una sorta di proxy che riceve
in ingresso i dati di tracciamento inviati dal nostro sito ecommerce e
manda poi dei dati in uscita verso gli endpoint dei diversi sistemi di
tracciamento.

Entrando un po' più nel tecnico possiamo dire che il nuove server che
abbiamo introdotto si troverà a ricevere in ingresso delle richieste web
provenienti dai device degli utenti, trasformerà queste richieste in
eventi che verranno poi processati ed esaminati dai Tag, dagli
Attivatori e dalle Variabili presenti all'interno del contenitore Server
Side di GTM. Tag, Attivatori e Variabili di un contenitore GTM di tipo
server sono elementi che funzionano esattamente allo stesso modo di come
funzionano in un normale contenitore GTM di tipo web: gli Attivatori
esaminano ogni evento in ingresso per verificare se sono soddisfatte o
meno determinate condizioni e nel momento in cui lo sono accendono il
relativo tag provocando quindi l'invio delle informazioni di
tracciamento all'endpoint collegato.

Questo nuovo modello introduce quindi due domande di fondamentale
importanza:

- In che modo i dati di misurazione vengono trasferiti dal dispositivo
  dell'utente e recepiti in maniera corretta dal contenitore di tipo
  server

- In che modo i dati di misurazioni inviati ad un contenitore di tipo
  server vengono trasformati in eventi in grado di attivare quelli che
  alla fine sono poi dei normali Tag GTM

Entrambe queste domande trovano risposta nella nuova entità presente
esclusivamente nei contenitori GTM di tipo server, i cosiddetti
**Client**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_16.bmp](./assets/media/image157.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_25.bmp](./assets/media/image158.png)

Questi client sono una sorta di adattatori che si interpongono tra il
software in esecuzione sul dispositivo dell'utente e i Tag presenti nel
Contenitore Server Side di GTM. Essendo quindi in grado di interpretare
il linguaggio di entrambi questi elementi possono acquisire le
informazioni in ingresso provenienti dai dispositivi dell'utente e
rielaborarle in maniera tale da trasformarle in eventi comprensibili e
gestibili dai vari Tag. Cerchiamo di chiarire un po' meglio i diversi
passaggi:

**[I CLIENT RICEVONO I DATI DI MISURAZIONE DA UN
DISPOSITIVO]{.underline}**

Supponiamo di voler monitorare l'attività di un utente che opera su tre
dispositivi differenti: un sito web, un' app mobile e un ipotetico
dispositivo smart come potrebbe essere, ad esempio, un tostapane
intelligente. Il sito web implementa GA4, l'app mobile Firebase
Analytics e il tostapane intelligente utilizza un protocollo di
misurazione proprietario chiamato "ToastMeasure"

Ora, tracciare il comportamento dell'utente su questi tre dispositivi
utilizzando GTM richiederebbe, di norma, la presenza di un contenitore
"tradizionale" su ciascuno di essi.

Considerando invece che un contenitore GTM di tipo server viene
installato su di un server esterno, indipendente dal tipo di dispositivo
su cui si vuole implementare il sistema di tracciamento, si potrebbe
pensare di utilizzare questo stesso contenitore di tipo server come
collettore per tutte e tre le piattaforme (sito, app e tostapane).

Nel far questo però sorge immediatamente un problema rappresentato dal
fatto che i tre dispositivi considerati non "parlano tutti lo stesso
linguaggio". Il sito web e l'app potrebbero anche utilizzare entrambi
GA4 ma il protocollo di comunicazione di Analytics non è ovviamente lo
stesso di quello utilizzato per gestire il tracciamento sul tostapane
intelligente ed è proprio qui che entrano in gioco i Client.

In pratica il contenitore server side di GTM dovrà avere al suo interno
3 distinti Client: uno in grado di comprendere il linguaggio utilizzato
dal sistema di tracciamento implementato sul sito (Client GA4), un altro
in grado di comprendere il linguaggio utilizzato dal sistema di
tracciamento implementato sull' app mobile (Client Firebase Analytics) e
un altro ancora in grado di comprendere invece il protocollo di
comunicazione utilizzato dal sistema di tracciamento implementato sul
tostapane intelligente (Client ToastMeasure").

Ogni richiesta in ingresso al Contenitore GTM di tipo server verrà
quindi elaborata da uno di questi tre Client secondo un certo ordine di
priorità. Il primo ad elaborare la richiesta in ingresso sarà il Client
cui è stata assegnata la priorità più elevata, e la prima cosa che
questo Client farà sarà esattamente quella di decidere se è in grado o
meno di comprendere questa richiesta e quindi di prendersela in carico.

Nel momento in cui la richiesta in ingresso dovesse quindi essere in un
"linguaggio" comprensibile al Client che la esamina (1) questo se la
prenderà in carico e passerà alla fase successiva, in caso contrario
passerà la richiesta ad un altro Client che farà esattamente la stessa
cosa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_26.bmp](./assets/media/image159.png)

In questo modo le richieste in arrivo dal sistema di tracciamento
implementato sul sito verranno prese in carico dal Client GA4, quelle
provenienti dall'App mobile verranno prese in carico dal Client Firebase
Analytics e quelle in arrivo dal tostapane verranno invece gestite dal
Client ToastMeasure

**[I CLIENT TRASFORMANO I DATI DELLA RICHIESTA IN UNO O PIU'
EVENTI]{.underline}**

Una volta presa in carico una richiesta il Client che la gestisce e che
è quindi in grado di interpretare il linguaggio con cui è stata composta
avrà il compito di passarla agli altri elementi del contenitore server
side di GTM (2) trasformandola in qualche cosa che anche questi elementi
siano effettivamente in grado di comprendere e questo qualcosa sono,
ovviamente, **eventi** che possano poi essere gestiti (come avviene
normalmente) da Attivatori, Tag e Variabili.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_27.bmp](./assets/media/image160.png)

**[I CLIENT ATTIVANO I TAG PRESENTI NEL CONTENITORE SERVER SIDE DI
GTM]{.underline}**

Una volta che un Client ha preso in carico una richiesta e l'ha
trasformata in eventi comprensibili al resto del contenitore server side
entrano poi in gioco gli Attivatori che valutano se sono o meno
verificate determinate condizioni in relazione all'evento generato dal
Client e in caso positivo attivano i Tag corrispondenti dando seguito
quindi alla richiesta originale in ingresso al server su cui è
installato tutto il sistema. Il fatto di dare seguito a questa richiesta
potrebbe voler dire inoltrare la richiesta stessa ad un ulteriore
endpoint destinato a raccogliere i dati di tracciamento (3) come
potrebbe essere Google Analytics, Google Ads, Facebook ...

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_ss_28.bmp](./assets/media/image161.png)

ma, più in generale, potrebbe anche voler dire rispondere al dispositivo
che ha originato la richiesta dicendo semplicemente "Ok fatto" oppure
mandando indietro un comando che, ad esempio, potrebbe accendere le luci
del tostapane.

Arrivati a questo punto dovrebbe essere chiaro il ruolo fondamentale che
svolgono in tutto il processo i Client disponibili all'interno del
nostro contenitore GTM di tipo server e come il processo possa
facilmente interrompersi nel momento in cui non dovessimo disporre di un
Client adeguato.

Fortunatamente per quelli che sono i nostri scopi il contenitore di tipo
Server di GTM dispone esattamente di tutto quello che ci serve avendo
già in pancia, nativamente, la possibilità di utilizzare un Client GA4
(oltre ad uno per Universal Analytics e ad uno per il Measurement
Protocol) in grado di gestire le richieste in ingresso provenienti da un
sistema di monitoraggio, anch'esso GA4, che, a questo punto, può
tranquillamente essere implementato tanto in maniera nativa sul sito
quanto utilizzando un normale contenitore GTM di tipo web.

In definitiva dunque, un possibile esempio di tracciamento server side
per GA4 si snoderà attraverso i seguenti passaggi:

1.  Sul sito viene generato un evento di page view che viene raccolto
    come normalmente avviene dal sistema di tracciamento GA4 (lato
    client) su di esso implementato

2.  L'evento raccolto sul sito non viene inviato direttamente
    all'endpoint e quindi al server di Google Analytics (come avverrebbe
    invece in un normale tracciamento lato client) ma viene inviato
    invece ad un server di nostra proprietà su cui è installato un
    contenitore GTM di tipo server utilizzando una normale richiesta
    HTTP (per far questo ovviamente il sistema di monitoraggio
    implementato sul sito dovrà essere opportunamente configurato)

3.  Il Client GA4 presente nel contenitore GTM di tipo server sarà in
    grado di prendersi in carico la richiesta HTTP in arrivo dal nostro
    tipo, di interpretarla e rielaborala trasformandola effettivamente
    in un evento di tipo page view "tradizionale" che verrà poi data in
    pasto ai Tag implementati sul contenitore GTM di tipo server

4.  Sul contenitore GTM di tipo server dovrà esserci un Tag di gestione
    degli eventi GA4 analogo (ma, ovviamente, non uguale dal punto di
    vista dei parametri di configurazione) a Tag dello stesso tipo
    presenti in un normale contenitore web, in grado di accendersi
    (mediante un apposito attivatore) ogni qual volta gli venga passato
    dal Client GA4 corrispondente un evento e deputato a trasferire i
    dati di quello stesso evento all'endpoint e quindi ai server di
    Google Analytics che lo registreranno inserendolo e rendendolo
    visibile nel nostro sistema di statistiche.

Ora prima di andare ad esaminare un po' più nel dettaglio i vari step
necessari per mettere in piedi un sistema di tracciamento server side è
bene riassumere rapidamente quelli che possono essere i vantaggi
principali e i limiti più evidenti di questo tipo di sistema

