# TRACCIAMENTO ECOMMERCE CON GTM SERVER SIDE



Arrivati a questo punto avremo a disposizione tutta la struttura
necessaria per attivare il tracciamento server-side (tracciamento GA4
implementato mediante GTM Web o direttamente dal sito Passweb e
Contenitore GTM di tipo Server collegato ad un server creato sulla
piattaforma Stape) per cui dovremo solo collegare i vari pezzi in
maniera tale che il tracciamento GA4 implementato sul nostro sito mandi
i dati al contenitore server di GTM, e facendo in modo poi che da qui
questi stessi dati (o una loro versione opportunamente rielaborata per
soddisfare le normative GDPR) vengano effettivamente inviati ad
Analytics.

In un tracciamento "client" tradizionale infatti i dati raccolti sul
nostro sito sono inviati direttamente ai server di Analytics e questo
indipendentemente dal fatto di aver utilizzato GTM o l'integrazione
nativa presente sui siti Passweb.

In un tracciamento "server-side" invece, i dati raccolti sul sito
dovranno essere inviati per prima cosa al server su cui abbiamo
installato il contenitore GTM di tipo server e da qui poi dovranno
essere prelevati, eventualmente elaborati secondo le proprie esigenze, e
quindi inoltrati ai server di Analytics.

**ATTENZIONE!** **Si ricorda che in un tracciamento server-side la parte
"tradizionale" di raccolta dei dati relativi agli eventi che si
verificano sul sito è comunque indispensabile e può tranquillamente
continuare ad essere implementata sia mediante integrazione nativa del
sito Passweb, sia mediante il classico contenitore web di GTM.** La
parte server side introduce "solo" un livello intermedio di transito dei
dati, dati che non dovranno più arrivare direttamente ai server di
Analytics ma che dovranno passare prima attraverso il contenitore server
di GTM (che funzionerà quindi come un vero e proprio proxy)

Il primo passo da fare sarà quindi quello di andare ad impostare
correttamente il tracciamento GA4 in uso al nostro sito in maniera tale
che i dati non vengano più inviati direttamente ad Analytics ma passino
prima attraverso il contenitore server di GTM installato sui server di
Stape.

##### INVIO DEI DATI DI TRACCIAMENTO AL CONTENITORE GTM SERVER SIDE

Le operazioni da fare per fare in modo di inviare i dati di tracciamento
al contenitore server side di GTM anziché direttamente ai server di
Analytics saranno diverse a seconda del fatto di aver implementato il
tracciamento GA4 sfruttando l'integrazione nativa presente sui siti
Passweb, oppure mediante l'utilizzo del classico contenitore web di GTM.

Vediamo quindi come poter operare in entrambi i casi:

**[TRACCIAMENTO GA4 MEDIANTE INTEGRAZIONE NATIVA PASSWEB]{.underline}**

In questo caso per impostare l'invio dei dati raccolti sul sito al
contenitore server di GTM sarà sufficiente valorizzare in maniera
corretta il campo "**Transport URL (Server Side)**" presente alla pagina
"**Sito -- Preferenze**" del Wizard (tab "**Tracciamento Dati**" sezione
"**Google Analytics**")

![](./assets/media/image180.png)

**Transport URL (Server Side):** consente di impostare l' url del server
su cui è installato il contenitore server di GTM e verso cui dovranno
quindi essere inoltrati i dati di tracciamento raccolti sul sito

**ATTENZIONE!** l' url inserito all'interno di questo campo deve essere
in forma completa, comprensivo quindi del protocollo utilizzato (https)

Considerando che stiamo analizzando la procedura da seguire per attivare
correttamente un tracciamento server side mediante i servizi offerti
dalla piattaforma stape.io, all'interno di questo campo andrà inserito
esattamente l' url associato al server creato su stape e visualizzato
all'interno del campo **Tagging Server URL**

![Videate\\stape_6.bmp](./assets/media/image173.png)

Si ricorda inoltre che, come evidenziato nei precedenti capitoli di
questo manuale, tale url può essere sia quello associato automaticamente
da stape stessa al nostro server una volta creato (opzione NON
consigliata), sia un eventuale sottodominio del dominio principale in
uso al nostro sito ecommerce (**opzione questa assolutamente
consigliata**)

**ATTENZIONE!** Nel momento in cui il campo in esame dovesse essere
lasciato vuoto l'inoltro dei dati di tracciamento avverrà direttamente
verso i server di Analytics configurando di fatto l'utilizzo di un
tracciamento "client-side" tradizionale

**[TRACCIAMENTO GA4 MEDIANTE GTM (CONTENITORE WEB)]{.underline}**

Considerando che, in questo, caso l'intera configurazione del
tracciamento di GA4 è gestita interamente dal contenitore web di GTM
anche l'inoltro dei dati di tracciamento raccolti sul sito verso il
contenitore server side di GTM dovrà essere configurata direttamente su
Google Tag Manager

Nello specifico dunque, sarà necessario accedere al pannello di gestione
del contenitore web di GTM utilizzato per implementare il tracciamento,
individuare e aprire il tag di configurazione di GA4

![](./assets/media/image181.png)

Nella maschera di configurazione del Tag dovremo poi selezionare
l'opzione "**Invia al contenitore del server**" e inserire quindi l' url
associato al nostro server stape all'interno del campo "**URL del
contenitore del server**" come evidenziato nella figura di seguito
riportata

![](./assets/media/image182.png)

**ATTENZIONE!** lavorando sul Tag di configurazione di GA4 tutti gli
eventi registrati sul sito verranno inoltrati al contenitore server-side
di GTM creato su Stape.

Nel momento in cui l'esigenza dovesse essere quella di inviare solamente
alcuni eventi al contenitore server side di GTM mantenendo, invece
l'invio di tutti gli altri eventi direttamente verso i server di
Analytics, sarà necessario agire nella configurazione del singolo Tag
GA4 del relativo evento aggiungendo per esso il parametro
"**transport_url**" valorizzato anche questa volta con l' url associato
al nostro server stape

![](./assets/media/image183.png)

##### DEBUG E VERIFICA DELL'INVIO DEI DATI AL CONTENITORE SERVER SIDE DI GTM

Arrivati a questo punto dovremmo aver configurato tutto il sistema in
modo tale che i dati raccolti all'interno del sito vengano inviati al
contenitore server side di GTM.

Per verificare che tutto funzioni effettivamente come previsto possiamo
utilizzare come al solito **la modalità Debug di Google Tag Manager,
modalità che, in queste condizioni però, dovrà essere attivata
contemporaneamente sia sul contenitore web di GTM (dove vengono attivati
i tag di raccolta dati) sia sul contenitore server side (dove dovranno
invece arrivare i dati inviati dal contenitore web)**

Accedere quindi al contenitore web di GTM utilizzato per implementare il
tracciamento GA4 e avviare la modalità di debug cliccando sul pulsante
di "**Anteprima**"

![](./assets/media/image184.png)

Una volta avviata la modalità di debug di questo contenitore potremo
verificare come al solito che tutti i tag di tracciamento impostati per
il sito vengano attivati in maniera corretta

![](./assets/media/image185.png)

Ora restando sempre nella stessa finestra del browser torniamo sul tab
in cui è presente l'interfaccia di gestione di GTM e andiamo ad aprire
il contenitore Server Side

![](./assets/media/image186.png)

Lanciamo quindi anche per esso la modalità di Debug cliccando sul
relativo pulsante di "**Anteprima**"

![](./assets/media/image187.png)

A questo punto dovremmo quindi avere aperti contemporaneamente in due
tab distinti della stessa finestra del browser il debug del contenitore
web e quello del contenitore server side

![](./assets/media/image188.png)

Andiamo quindi nel tab in cui è stato aperto il front end del sito e
navighiamolo in maniera tale da far scattare alcuni tag di tracciamento.

Se tutto funziona in maniera corretta dovremo ora veder arrivare i dati
anche nella finestra di debug del contenitore server side.

Nello specifico dovremo trovarci in una situazione del tipo di quella
rappresentata in figura

![Videate\\gtm_ss_10.bmp](./assets/media/image189.png)

Selezionando uno degli eventi in arrivo sul contenitore server side (es.
page_view nella colonna di sinistra), nel tab "**Request**" della
maschera di debug dovremmo vedere, all'interno della sezione "**Incoming
http Request**" la richiesta effettivamente inviata al contenitore
server da parte del contenitore web di GTM richiesta questa che conterrà
tutti i dati di tracciamento che, normalmente, venivano inviati
direttamente ai server di Analytics (cliccandoci sopra possiamo anche
vedere il dettaglio di tutti questi dati)

**ATTENZIONE!** Come evidenziato all'interno del capitolo "*Tracciamento
Server Side*" tutto questo è reso possibile grazie al fatto che il
contenitore server side di GTM dispone nativamente di un client GA4 in
grado di acquisire e interpretare le richieste in arrivo dai tradizioni
sistemi di tracciamento client GA4

![](./assets/media/image190.png)

Al momento invece la sezione "**Outgoing HTTP Request from Server**" non
conterrà invece nessun dato.

All' interno di questa sezione dovremo infatti trovare la richiesta che
il contenitore server side invia ai server di Analytics

**ATTENZIONE!** nelle condizioni attuali non abbiamo ancora configurato
l'inoltro dei dati in arrivo al contenitore server side di GTM verso i
server di Analytics per cui se anche esaminassimo la Debug View di
Google Analytics non vedremmo ovviamente nessun tipo di dato

##### INVIO DEI DATI DAL CONTENITORE SERVER SIDE DI GTM AI SERVER DI ANALYTICS

Verificato il corretto inoltro dei dati di tracciamento dal sito al
contenitore server side di GTM non ci resta ora che aggiungere l'ultimo
mattoncino che consiste nel passaggio dei dati dal contenitore Server
Side di GTM ai server di Analytics per registrare effettivamente
l'evento

Per fare questo è possibile utilizzare, anche in questo caso, uno dei
Tag messi a disposizione nativamente da GTM esattamente come avviene per
i normali contenitori web.

Portiamoci dunque **nell'interfaccia di gestione del contenitore GTM
Server Side**, spostiamoci all'interno della sezione Tag e clicchiamo
sul pulsante "**Nuovo**" per avviare la creazione di un nuovo tag (il
procedimento è esattamente lo stesso di quello più volte utilizzato per
creare tag sul tradizionale contenitore web)

![](./assets/media/image191.png)

**ATTENZIONE!** I Tag disponibili per un contenitore server side sono
diversi (e ancora in numero molto minore) rispetto a quelli presenti per
un normale contenitore web.

Selezionare quindi tra le tipologie di tag disponibili quello relativo
ovviamente a GA4 e completare la configurazione del Tag lasciando i
valori di default

![](./assets/media/image192.png)

**ATTENZIONE!** lasciare vuoto il campo "**ID misurazione**".

In questo modo infatti sarà GTM stesso a prelevare, dai dati in ingresso
al contenitore server side, l'id di misurazione dello stream di
Analytics a cui inviare le informazioni di tracciamento, dato questo
configurato direttamente sui tag del contenitore web di GTM

**ATTENZIONE!** la configurazione di un Tag GA4 Server Side è ovviamente
diversa da quella di un tradizione Tag GA4 "client side".

Volendo sarebbe possibile, tra le altre cose ad esempio, decidere
esattamente quali dei parametri in ingresso al contenitore server side
inoltrare o meno ad Analytics (sezione "Parametri da escludere") oppure
integrare i dati in ingresso al contenitore server side con altre
informazioni (sezione "Parametri da aggiungere / modificare") prima di
passarli effettivamente ad Analytics

![](./assets/media/image193.png)

**ATTENZIONE!** Come più volte indicato lo scopo di questo manuale non è
quello di fornire una guida all'utilizzo di GTM ma semplicemente quella
di illustrare i passaggi fondamentali per arrivare ad implementare un
tracciamento ecommerce server side di base. Per maggiori informazioni
relativamente all'effettivo utilizzo e alle diverse possibilità offerte
da questo strumento è quindi necessario fare riferimento alla
documentazione ufficiale messa a disposizione da Google o ad una delle
numerose guide presenti in rete

Completata la configurazione del Tag dovremo ora impostare il relativo
attivatore. Anche in questo caso il procedimento è esattamente lo stesso
di quello più volte utilizzato per impostare un qualsiasi attivatore di
un tradizionale contenitore web.

Clicchiamo dunque sul pulsante di creazione di un nuovo attivatore e
selezioniamo, tra le opzioni disponibili, quella relativa ad un nuovo
Attivatore "**Personalizzato**"

![](./assets/media/image194.png)

Così come per i Tag anche per gli Attivatori quelli disponibili in un
contenitore server side sono sostanzialmente diversi rispetto a quelli
presenti in un tradizionale contenitore web e diverso è, ovviamente,
anche il modo in cui alcuni di essi operano e conseguentemente il modo
in cui dovranno essere configurati.

Nello specifico, quello che dovremo fare ora sarà riconoscere che le
chiamate in ingresso al nostro contenitore server side sono generate da
un "tradizionale" sistema di tracciamento GA4 e solo a questo punto
attivare il Tag GA4 server side per inoltrare i dati ad Analytics.

Questo lo possiamo fare basandoci sul nome del client che genera le
chiamate in ingresso. Come evidenziato nei precedenti capitoli di questo
manuale infatti il nostro contenitore Serve Side dispone nativamente di
due client in grado di riconoscere ed interpretare le chiamate in
ingresso provenienti rispettivamente da un sistema di tracciamento
Universal Analytics o Google Analytics 4

![](./assets/media/image157.png)

In considerazione di quanto detto il nostro attivatore personalizzato
dovrà essere configurato come nella figura di seguito riportata

![](./assets/media/image195.png)

Il campo "**Questo attivatore si attiva su**" dovrà essere impostato
sull'opzione "**Alcuni eventi**"

Il filtro di attivazione del tag (**Attiva questo attivatore quando si
verifica un evento e tutte queste condizioni sono vere)** dovrà invece
essere costruito impostando i vari campi in questo modo:

- Nel primo campo cliccare sull'opzione "**Scegli una variabile
  integrata**" e selezionare poi, tra quelle proposte, la variabile
  "**Client Name**"

- Nel secondo campo impostare l'operatore "**contiene**"

- Nel terzo campo impostare come valore della condizione la stringa
  "**GA4**"

Completiamo quindi la creazione del Tag assegnandogli un nome (es. "GA4
SS") e cliccando sul pulsante "**Salva**"

##### DEBUG E VERIFICA DEL SISTEMA DI TRACCIAMENTO ECOMMERCE SERVER SIDE

Arrivati a questo punto dobbiamo solamente verificare che tutto il
sistema funzioni in maniera corretta e quindi che gli eventi registrati
sul nostro sito ecommerce vengano correttamente inviati al contenitore
GTM Server Side (cosa questa che avevamo già verificato nei precedenti
capitoli), che l'acquisizione di questi eventi attivi il Tag GA4 server
side appena configurato e, infine, che l'attivazione di questo Tag
comporti effettivamente l'inoltro dei dati a Google Analytics con la
conseguente registrazione dell'evento all'interno del sistema di
gestione delle statistiche.

Per fare questo utilizzeremo ancora una volta la modalità di Debug di
GTM e, ora, anche la Debug View di GA4.

Seguendo dunque gli stessi passaggi descritti all'interno del capitolo
"*Debug e verifica dell'invio di dati al contenitore Server Side di
GTM*" andiamo ad attivare la modalità di Anteprima sia sul contenitore
Web che sul contenitore Server e andiamo poi a navigare il sito in
maniera tale da far scattare alcuni tag di tracciamento.

A questo punto se tutto funziona in maniera corretta andando ad
analizzare la finestra di debug del contenitore server side dovremmo
trovarci in una situazione del tipo di quella rappresentata in figura

![](./assets/media/image196.png)

In colonna sinistra dovremmo trovare l'elenco degli eventi e delle
relative chiamate provenienti dal nostro sito ecommerce e in ingresso al
contenitore GTM Server Side.

Selezionando uno di questi eventi (es. view_item_list) nel Tab
"**Tags**" dovremmo trovare, tra l'elenco dei Tag attivati (**Tags
Fired**), il tag GA4 Server Side a testimonianza del fatto che il nostro
attivatore ha funzionato in maniera corretta riconoscendo che le
chiamate in ingresso sono arrivate effettivamente da un client di tipo
GA4 e attivando quindi il tag GA4 SS precedentemente configurato.

L'attivazione di questo tag dovrebbe quindi aver provocato l'inoltro dei
dati ad Analytics. Spostandoci infatti nel Tab "**Request**" dovremmo
ora veder popolata non solo la sezione "Incoming HTTP Requests", che
come precedentemente evidenziato ci mostra le richieste in ingresso al
contenitore server side, ma anche quella relativa alle "**Outgoing HTTP
Requests form Server**" ossia le richieste effettivamente in uscita da
questo stesso contenitore server side

![](./assets/media/image197.png)

L'ultima cosa da verificare è ora che le richieste in uscita dal
contenitore server side siano state correttamente inviate ai server di
Google. Spostandoci dunque nella Debug View dell'account GA4 collegato
dovremmo trovare una situazione del tipo di quella rappresentata in
figura

![](./assets/media/image198.png)

a testimonianza del fatto che gli eventi originariamente generati sul
nostro sito ecommerce sono stati correttamente registrati da Google
Analytics e che quindi tutto il nostro sistema di tracciamento server
side funziona correttamente.

**ATTENZIONE!** si consiglia di simulare tutti gli eventi ecommerce
gestiti sul proprio sito web e verificare che per ciascuno di essi i
relativi dati vengano correttamente registrati da Google Analytics

