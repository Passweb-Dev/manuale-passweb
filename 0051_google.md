# GOOGLE



La sezione "**Google**" del tab "**Tracciamento Dati**" consente di
impostare tutti i parametri di configurazione necessari per attivare il
tracciamento diretto Sito -- Google Analytics / Google Ads.

In questo senso sarà possibile utilizzare l'integrazione nativa tra
Passweb e Google Analytics / Google Ads oppure, volendo, si potrà anche
decidere di implementare questo ed altri tipi di tracciamento
utilizzando Google Tag Manager.

##### GOOGLE ANALYTICS

All'interno di questa sezione è possibile attivare ed impostare il
collegamento diretto tra il proprio sito Passweb e il sistema di
statistiche messo a disposizione da Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_ganalytics.bmp](./assets/media/image177.png)

**ATTENZIONE!** Google Analytics è uno strumento di web analytics molto
potente che può essere integrato nativamente con i siti Passweb
attraverso l'impostazione di semplici parametri ma rimane comunque un
software di terze parti indipendente da Passweb che richiede, al fine di
poter essere utilizzato al meglio in tutte le sue funzionalità,
specifiche conoscenze tecniche.

All'interno di questo manuale è presente un'apposita sezione (*Google
Analytics*) per approfondire un po\' le conoscenze e l'utilizzo di
questo strumento avendo comunque sempre ben chiaro che lo scopo del
presente manuale **non è** **quello di offrire una guida completa
all'utilizzo e alla configurazione di strumenti quali Google Analytics o
Google Tag Manager**.

Nel momento in cui l'esigenza dovesse essere quella di approfondire
ulteriormente questo tipo di argomenti si consiglia quindi di fare
sempre riferimento alla documentazione ufficiale messa a disposizione
direttamente da Google o alle numerose guide dedicate presenti in rete.

Fatta questa doverosa considerazione passiamo ora ad analizzare nel
dettaglio i diversi parametri che consentono di attivare e configurare,
secondo le proprie esigenze, il collegamento diretto tra il proprio sito
Passweb e Google Analytics.

**Versione Google Analytics:** consente di definire la versione di
Google Analytics con cui dovrà essere integrato il proprio sito Passweb

E' possibile selezionare una delle seguenti opzioni:

- **Disabilitato:** in queste condizioni il tracciamento diretto Sito --
  Analytics è disabilitato

- **Google Analytics 4 (GTAG):** selezionando questa opzione il sito
  verrà predisposto per inviare direttamente i dati di tracciamento a
  Google Analytics utilizzando sempre la libreria **gtag.js (GA4)**

**Measurement ID Client:** consente di impostare l' **ID Misurazione**
dello Stream di Dati verso cui inviare i dati del tracciamento client
(effettuato cioè mediante esecuzione di apposite chiamate javascript)

Questo parametro può essere facilmente trovato nella maschera di
configurazione dello Stream stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_20.bmp](./assets/media/image178.png)

**ATTENZIONE!** Tutti gli ID Misurazione di GA4 sono del tipo
**G-XXXXXXXXXX**

**Transport URL (Server Side):** consente di attivare un sistema di
monitoraggio Server Side impostando l'url della macchina su cui si è
deciso di installare il contenitore GTM di tipo server verso cui
dovranno essere inoltrati i dati di tracciamento raccolti sul sito. L'
url inserito all'interno di questo campo deve essere in forma completa,
comprensivo quindi del protocollo utilizzato (https)

**ATTENZIONE!** **il campo in esame dovrà essere valorizzato solo ed
esclusivamente nel momento in cui si sia effettivamente deciso di
implementare un sistema di tracciamento Server Side**.

Nel momento in cui l'esigenza dovesse essere quella di continuare ad
utilizzare un sistema di tracciamento "tradizionale" (lato client) il
campo in esame dovrà quindi essere lasciato vuoto.

Per maggiori informazioni relativamente ai sistemi di tracciamento
Server Side e a come poterli implementare si rimanda anche a quanto
indicato all'interno dei relativi capitoli di questo manuale ("*Google
Tag Manager -- Implementare Google Analytics con GTM -- Tracciamento
Server Side*")

**Tracciamento Server:** consente di decidere se attivare o meno il
tracciamento lato server di Google Analytics **in relazione all'evento
di purchase**

Nel momento in cui il parametro in questione dovesse essere:

- **Deselezionato:** l'evento di purchase potrà essere tracciato solo ed
  esclusivamente lato client

> In queste condizioni, dunque, l'acquisizione di un nuovo ordine potrà
> essere tracciata correttamente solo se l'utente dovesse effettivamente
> approdare nella pagina di "Conferma Ordine", pagina questa che avrà un
> indirizzo del tipo
>
> www.url_sito.it/store/cart/checkout/success?id=xxxx
>
> Nel momento in cui l'utente non dovesse, per una qualsiasi ragione,
> approdare su questa pagina (ad esempio perché ha scelto di effettuare
> un pagamento online e, una volta completata la transazione, decide poi
> di non ritornare sul sito del venditore) l'evento javascript
> necessario per comunicare ad Analytics i dati dell'ordine non potrà
> essere eseguito e, conseguentemente, non sarà possibile tracciare il
> relativo acquisto.

- **Selezionato:** l'evento di purchase verrà tracciato **sempre e
  comunque** lato server (posto ovviamente di aver impostato in maniera
  corretta anche i successivi parametri "**Measurement Id Server**" e
  "**API Key Google Analytics Eventi Server**").

> In queste condizioni dunque sarà direttamente il server su cui risiede
> il sito Passweb ad inviare ad Analytics i dati relativi
> all'acquisizione del nuovo ordine. Nel caso in cui l'utente, una volta
> chiuso un ordine, non dovesse approdare sulla relativa pagina di
> conferma (ad esempio perché ha scelto di effettuare un pagamento
> online e, una volta completata la transazione, decide poi di non
> ritornare sul sito del venditore), Passweb potrebbe inviare ugualmente
> ad Analytics tutti i dati necessari al tracciamento dell'ordine
> stesso, operando direttamente a livello server.
>
> **Affinché ciò possa avvenire in maniera corretta è però
> indispensabile che il pagamento utilizzato implementi la modalità
> Server to Server**. Sarà infatti la risposta ricevuta dal gateway di
> pagamento (oltre al fatto che l'utente abbia effettivamente prestato
> tutti i relativi consensi) a determinare o meno l'invio ad Analytics
> dei dati relativi all'ordine acquisito.
>
> Nello specifico, una volta ricevuta risposta positiva dal gateway di
> pagamento, Passweb avrà la certezza che l'ordine in questione è stato
> correttamente pagato e quindi, oltre ad inserire il documento
> all'interno del gestionale, provvederà anche ad inviare ad Analytics
> tutti i dati necessari al tracciamento dell'ordine.
>
> Se, al contrario, dal gateway di pagamento non dovesse arrivare
> nessuna risposta o dovesse comunque arrivare una risposta negativa,
> Passweb non avrà la certezza che l'ordine sia stato correttamente
> pagato; lascerà quindi il documento in stato di "Pagamento non
> confermato" e non invierà ad Analytics nessun dato.
>
> **ATTENZIONE!** abilitando il tracciamento lato server della purchase
> potrebbero verificarsi, in fase di tracciamento, problemi dovuti al
> fatto che l'evento server non viene correttamente legato da Google al
> flusso dei precedenti eventi client e questo potrebbe portare ad avere
> delle transazioni "Unassigned" (per le quali non è cioè possibile
> risalire alla sorgente e/o al mezzo che ha prodotto la visita da cui è
> stato generato l'ordine).
>
> Nel momento in cui l'esigenza dovesse quindi essere quella di ridurre
> al minimo il valore delle transazioni "Unassigned" su Google
> Analytics, il consiglio e quello di non attivare questo parametro e di
> continuare quindi a tracciare anche l'evento di purchase lato client
>
> Un'ultima cosa di fondamentale importanza da sottolineare, inoltre,
> **è che l'eventuale invio della purchase lato server avviene solo
> verso Google Analytics e non verso Google Ads**, per cui se l'utente
> non dovesse tornare nella pagina di conferma odine, una volta concluso
> il pagamento, non potrà comunque scattare l'evento client per l'invio
> dei dati a Google Ads e di conseguenza la conversione su Google Ads
> non potrà essere registrata.
>
> In queste condizioni Passweb offre comunque la possibilità di
> recuperare la conversione mettendo a disposizione dell'utente i dati
> di quello specifico ordine, dati questi che potranno poi essere
> importati in Google Ads attraverso la gestione delle "Conversioni
> avanzate per i leads" e l'import delle conversioni offline (per
> maggiori informazioni in merito si rimanda a quanto indicato
> all'interno del capitolo "*Google Ads User Provided Data e Conversioni
> Avanzate -- Import delle conversioni offline*" di questo manuale)

**Measurament Id Server:** visibile solo nel caso in cui il precedente
parametro "**Tracciamento Server**" sia stato correttamente selezionato

Consente di impostare l' **ID Monitoraggio** della proprietà di
Analytics cui dovranno essere inviati i dati del tracciamento effettuato
lato server (tipicamente è lo stesso valore inserito all'interno del
precedente campo "Chiave Google analytics")

**ATTENZIONE!** Nel caso in cui il parametro "**Tracciamento Server**"
dovesse essere selezionato ma non venga poi inserito un ID di
monitoraggio, il tracciamento lato server di Google Analytics non potrà
funzionare in maniera corretta

**API Key** **Google Analytics Eventi Server:** visibile solo nel caso
in cui il precedente parametro "**Abilita Tracciamento Server**" sia
stato correttamente selezionato

Consente di impostare l'API Key necessaria per gestire il tracciamento
lato server dei nuovi ordini

**ATTENZIONE!** Nel caso in cui il parametro "**Tracciamento Server**"
dovesse essere selezionato ma non venga poi inserita la relativa API
Key, il tracciamento lato server di non potrà funzionare in maniera
corretta

**Modalità Debug:** consente, se selezionato, di inviare i dati a GA4 in
modalità Debug. In queste condizioni sarà quindi possibile testare il
corretto funzionamento dell'integrazione visualizzando in tempo reale
eventi e relativi parametri passati a GA4 all'interno della sua Debug
View.

Per maggiori informazioni relativamente alla Debug View di GA4 è
possibile consultare il relativo capitolo di questo manuale *("Google
Analytics -- Google Analytics 4 -- Universal Analytics e GA4 Principali
differenze -- Debug View"*). Per approfondire l'argomento si consiglia
comunque di fare sempre riferimento alla documentazione ufficiale messa
a disposizione da Google o alle numerose guide dedicate presenti in
rete.

**Indirizzi IP Debug**: consente di indicare l'indirizzo o gli indirizzi
IP **pubblici** (separati da ,) per i quali dovrà essere abilitato il
tracciamento di GA4 in modalità di Debug.

**ATTENZIONE!** nel momento in cui il campo in esame dovesse essere
lasciato vuoto la modalità di Debug sarà attiva per tutti gli indirizzi
IP che visitano il sito

In sostanza, dunque, lasciando vuoto il campo in esame nella Debug View
di GA4 verranno tracciate tutte le visite al sito, indipendentemente dal
loro indirizzo IP di provenienza. Questo potrebbe rendere difficile il
debug di determinate chiamate soprattutto nel momento in cui il sito
dovesse essere in produzione (e visitato quindi da tantissimi utenti).

Nel momento in cui il campo in esame dovesse invece essere valorizzato
con un determinato indirizzo IP, la modalità di debug verrà attivata
solo per quello stesso IP e nella Debug View di GA4 verranno quindi
tracciate e visualizzate solo le visite provenienti da quello stesso IP
(rendendo quindi il processo di debug molto più semplice)

**Utilizza UserID**: consente, se selezionato, di inviare alla proprietà
GA4 collegata anche lo User Id (codice identificativo dell'utente) posto
ovviamente che l'utente che sta navigando il sito abbia effettuato
correttamente il login (per utenti non autenticati lo User Id avrà
ovviamente valore null)

**ATTENZIONE!** come richiesto da Google, una volta attivato il
parametro in questione:

- lo User Id inviato ad Analytics coinciderà esattamente con l'Id utente
  in uso al sito Passweb e sarà quindi un semplice codice numerico che
  non consente, a strumenti di terze parti, di risalire all'effettiva
  identità dell'utente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_59.bmp](./assets/media/image179.png)

- lo User Id verrà impostato a livello di tag di configurazione e verrà
  quindi inviato assieme a tutti gli eventi gestiti dal proprio sito
  Passweb

**ATTENZIONE!** prima di attivare, lato Passweb, il tracciamento
mediante User Id è necessario accertarsi bene di gestire in maniera
corretta la richiesta agli utenti di tutti i consensi necessari, di aver
sistemato in maniera adeguata l'informativa in uso sul sito e, in
generale, di soddisfare tutto quanto richiesto dal GDPR in merito di
trattamento dei dati

Per maggiori informazioni relativamente all'identificazione degli utenti
in GA4 mediante User id è possibile consultare il relativo capitolo di
questo manuale *("Google Analytics -- Google Analytics 4 -- Universal
Analytics e GA4 Principali differenze -- Privacy e Raccolta dei dati --
User ID"*). Per approfondire l'argomento si consiglia comunque di fare
sempre riferimento alla documentazione ufficiale messa a disposizione da
Google o alle numerose guide dedicate presenti in rete.

**Raccolta Dati Utente GA**: consente, se selezionato, di inviare a GA4
i dati utente necessari per la gestione, direttamente in Analytics,
delle conversioni avanzate (**enhanced conversion**).

**ATTENZIONE!** l'attivazione di questo parametro comporta l'inserimento
dei dati utente anche in eventuali chiamate server verso Analytics
effettuate mediante Measurement Protocol (MP), il tutto ovviamente nel
momento in cui si dovesse decidere di abilitare anche questo tipo di
tracciamento (parametro "**Google Analytics -- Abilita tracciamento
server**")

Per maggiori informazioni in merito a questo tipo di operazione, e a
cosa comporta anche da un punto di vista tecnico, si veda quanto
indicato nel relativo capitolo di questo manuale ("*Google Analytics --
Google Analytics 4 -- GA4 User Provided Data e Conversioni Avanzate*")

In ogni caso occorre tenere bene in considerazione che:

- come per il tracciamento dello User-id anche in questo caso è
  necessario accertarsi di gestire in maniera corretta la richiesta agli
  utenti di tutti i consensi necessari, di aver sistemato in maniera
  adeguata l'informativa in uso sul sito e, in generale, di soddisfare
  tutto quanto richiesto dal GDPR in merito di trattamento dei dati

- **al momento in cui è stato scritto questo manuale, la gestione degli
  user-provided data e le conversioni avanzate in GA4 sono ancora una
  funzionalità in Beta (come indicato da Google stesso) per cui
  andrebbero attivate in maniera più che consapevole tenendo bene in
  considerazione anche i possibili problemi che l'attivazione di questa
  stessa funzionalità potrebbe causare**

##### GOOGLE TAG MANAGER

Google Tag Manager è un sistema di gestione dei tag che consente di
gestire e aggiornare rapidamente, senza il bisogno di modificare il
codice sorgente delle pagine, i codici di monitoraggio e i relativi
snippet presenti sul sito.

La sezione **Google Tag Manager** consente di impostare e personalizzare
lo snippet di codice necessario per inserire il relativo contenitore
nelle pagine del sito e per poter garantire quindi il corretto
funzionamento di tutto il sistema.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_gtagmanager.bmp](./assets/media/image180.png)

Ovviamente nel caso in cui si sia deciso di utilizzare l'integrazione
diretta per implementare il tracciamento del proprio sito con Google
Analytics, sarà necessario accertarsi di non avere implementato lo
stesso tipo di tracciamento anche all'interno di GTM. In caso contrario
infatti tutte le statistiche presenti su Analytics potrebbero avere
valori doppi o comunque non coerenti con quello che effettivamente
succede nella realtà.

**ATTENZIONE! in ogni caso è assolutamente sconsigliato il fatto di
gestire un sistema di tracciamento in modalità mista** dove alcuni
eventi sono tracciati direttamente dal sito e altri mediante Tag
Manager. In questi casi infatti si perderebbe facilmente il controllo di
cosa viene eseguito prima e dopo (soprattutto nell'ottica di gestione
della Consent Mode) e si potrebbe quini incorrere, molto facilmente, in
errori di tracciamento

Inoltre è bene sottolineare anche che i tracciamenti "nativi" di Google
Tag Manager potrebbero non essere completamente supportati da Passweb,
che ha una sua struttura del dataLayer, e potrebbero quindi portare ad
un monitoraggio non corretto dei vari eventi. **Per la creazione dei
tag, degli attivatori e delle relative variabili in Google Tag Manager
si consiglia di seguire le indicazioni contenute all'interno del
capitolo "Google Tag Manager -- Implementare Google Analytics con Google
Tag Manager -- GTM e GA4" di questo manuale"**

Fatte queste considerazioni di fondamentale importanza, vediamo ora un
po\' più nel dettaglio i singoli parametri presenti all'interno di
questa sezione.

**Versione Data Layer**: consente di indicare la versione del dataLayer
da utilizzare all'interno del sito e che Passweb dovrà quindi generare
al verificarsi di determinati eventi

E' possibile selezionare una delle seguenti opzioni:

- **Disabilitato:** in queste condizioni non verrà creato nessun
  dataLayer da poter utilizzare per implementare un sistema di
  tracciamento del proprio sito mediante Google Tag Manager

- **Google Analytics 4**: selezionando questa opzione il dataLayer
  generato da Passweb sarà esattamente quello richiesto da Google
  Analytics 4 in relazione ai diversi eventi gestiti.

> Per maggiori informazioni relativamente a questo tipo di dataLayer e a
> come poter implementare grazie ad esso e a GTM un monitoraggio
> ecommerce su proprietà Google Analytics 4 si rimanda a quanto indicato
> nel corrispondente capitolo di questo manuale ("*Google Tag Manager --
> Implementare Google Analytics con GTM -- GTM e GA4*")

**ATTENZIONE!** **Il dataLayer è lo strumento utilizzato per trasmettere
le informazioni dalle pagine web del nostro sito a GTM e a tutti i Tag
del Contenitore (e tramite essi ai relativi strumenti di analisi di
terze parti).**

Nel momento in cui la versione del dataLayer impostata non dovesse
quindi coincidere con il sistema di tracciamento effettivamente
implementato i dati inviati dal sito potrebbero non essere corretti e il
tracciamento potrebbe, di conseguenza, non funzionare in maniera
adeguata.

**Utilizza user_id nel Data Layer**: consente, se selezionato, di
inserire nel relativo dataLayer anche il parametro "**User_id**"
valorizzato con l'identificativo assegnato da Passweb agli utenti che
effettuano il login al sito.

In relazione all'utilizzo dello User id è bene ricordare che:

- lo User ID inserito nei vari Data Layer coinciderà esattamente con
  l'Id utente in uso al sito Passweb e sarà quindi un semplice codice
  numerico che non consente, a strumenti di terze parti, di risalire
  all'effettiva identità dell'utente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_59.bmp](./assets/media/image179.png)

- lo User ID verrà inserito nel Data Layer di tutti gli eventi ecommerce
  e, ovviamente, sarà valorizzato solo nel caso in cui l'utente che
  naviga il sito abbia effettuato correttamente il login (in caso
  contrario il suo valore sarà "null")

**ATTENZIONE!** l'attivazione di questo parametro non comporta
necessariamente il passaggio di questa informazione a Google Analytics o
ad un qualsiasi altro sistema di terze parti. Affinché il dato possa
essere trasmesso dovranno infatti essere configurati opportunamente
anche i relativi tag di tracciamento creati su GTM.

In ogni caso prima di attivare, lato Passweb, il tracciamento mediante
User ID è necessario accertarsi bene di gestire in maniera corretta la
richiesta agli utenti di tutti i consensi necessari, di aver sistemato
in maniera adeguata l'informativa in uso sul sito e, in generale, di
soddisfare tutto quanto richiesto dal GDPR in merito di trattamento dei
dati

Per maggiori informazioni relativamente all'identificazione degli utenti
in GA4 mediante User id è possibile fare riferimento a quanto indicato
nel capitolo *"Google Analytics -- Privacy e Raccolta dei dati -- User
ID"* di questo manuale (per approfondire l'argomento si consiglia
comunque di fare sempre riferimento alla documentazione ufficiale messa
a disposizione da Google o alle numerose guide dedicate presenti in
rete).

Per maggiori informazioni relativamente invece a come poter implementare
il tracciamento dello User id mediante GTM si rimanda a quanto indicato
nel capitolo *"Google Tag Manager -- Implementare Google Analytics con
GTM -- GTM e GA4 -- Tracciamento dello User id"* di questo manuale.

**Raccolta Dati Utente nel Data Layer****:** consente, se selezionato,
di inserire nel dataLayer gestito da Passweb una sezione user_data del
tipo di quella di seguito indicata

*user_data: {*

*sha256_email_address: valore hashato della mail utente ,*

*sha256_phone_number: valore hashato del telefono utente,*

*address: {*

*sha256_first_name: valore hashato del nome utente,*

*sha256_last_name: valore hashato del cognome / ragione sociale utente,*

*street: indirizzo utente (via),*

*city: indirizzo utente (città),*

*postal_code: indirizzo utente (CAP),*

*country: indirizzo utente (Nazione)*

*}*

*}*

e contenente quindi i dati utente necessari per la gestione, in
Analytics o in AdWords delle conversioni avanzate (**enhanced
conversion**).

**ATTENZIONE!** **l'attivazione di questo parametro comporta solamente
l'inserimento dei dati utente nel dataLayer di Passweb secondo quanto
richiesto da Google.**

L' effettivo invio di questi dati a Google Analytics piuttosto che a
Google Ads e la conseguente attivazione e gestione sulle due piattaforme
delle conversioni avanzate, dipenderà poi dal fatto di aver implementato
correttamente all'interno di Google Tag Manager i relativi Tag di
tracciamento, Tag questi che dovranno preoccuparsi di prelevare i dati
utente dal dataLayer messo a disposizione da Passweb per poi inviarli
alla relativa piattaforma (Google Analytics / Google Ads) dove dovrà
essere stata attivata, ovviamente, la gestione delle conversioni
avanzate.

**ATTENZIONE!** Come per lo User Id anche in questo caso è necessario
accertarsi bene di gestire in maniera corretta la richiesta agli utenti
di tutti i consensi necessari, di aver sistemato in maniera adeguata
l'informativa in uso sul sito e, in generale, di soddisfare tutto quanto
richiesto dal GDPR in merito di trattamento dei dati

Per maggior informazioni relativamente a quella che sarà la struttura
del dataLayer gestito da Passweb nel momento in cui si dovesse decidere
di attivare il parametro in questione si rimanda a quanto indicato
all'interno del capitolo "*Google Tag Manager -- User Provided Data e
Conversioni Avanzate*" di questo manuale

**Monitoraggio Google Tag Manager HEAD / BODY:** consente di impostare
lo snippet di codice relativo al contenitore dei Tag che dovrà essere
inserito nelle varie pagine del sito rispettivamente all'interno del tag
\< head \> e immediatamente dopo il tag di apertura \< body \>

**Attiva Remarketing Dinamico**: consente, se abilitato, di inserire nel
datalyer gestito da Passweb in relazione agli eventi di:

- **view_item_list**

- **view_item**

- **add_to_cart**

- **purchase**

una struttura dati utile per poter gestire più facilmente in Google Tag
Manager i tag di Remarketing Dinamico (per maggiori informazioni in
merito si veda anche quanto indicato all'interno del capitolo "*Google
Tag Manager -- Remarketing Dinamico*" di questo manuale)

Per maggiori informazioni relativamente alla configurazione e
all'utilizzo di Google Tag manager si rimanda a quanto indicato nella
relativa sezione di questo manuale ("*Google Tag Manager*") e
soprattutto alla relativa documentazione ufficiale e alle numerose guide
presente in rete. **Si ricorda infatti che lo scopo del presente
manuale** **non è** **quello di offrire una guida completa all'utilizzo
e alla configurazione di Google Tag Manager** che rimane uno strumento
esterno a Passweb e che richiede anche, tra l'altro, specifiche
conoscenze tecniche per poter essere configurato ed utilizzato al
meglio.

##### GOOGLE ADS

La sezione Google Ads consente di gestire tutti i parametri di
configurazione necessari per integrare il proprio sito Passweb con
Google Ads in maniera tale da implementare un sistema di tracciamento
delle conversioni che non richiede necessariamente l'utilizzo di Google
Tag Manager.

Nello specifico occorre però considerare che **Passweb gestisce il
tracciamento diretto Sito -- Google Ads solo ed esclusivamente in
relazione a conversioni legate ad eventi di Purchase**

**Nel momento in cui l'esigenza dovesse essere quella di gestire
conversioni legate anche ad altri eventi (es. add_to_cart,
begin_checkout ...) sarà quindi necessario implementare il proprio
sistema di tracciamento utilizzando, per forza di cose, Google Tag
Manager** (in questo senso si rimanda a quanto indicato all'interno del
capitolo "*Google Tag Manager*" di questo manuale)

Si ricorda inoltre che all'interno di questo manuale è presente
un'apposita sezione (*Google Ads User Provided Data e Conversioni
Avanzate*) che consente di approfondire un po' di più le conoscenze
relative al tracciamento delle conversioni in Google Ads. In ogni caso
lo scopo del presente manuale **non è** **quello di offrire una guida
completa all'utilizzo e alla configurazione di strumenti quali Google
Ads**.

Nel momento in cui l'esigenza dovesse essere quella di approfondire
ulteriormente questo tipo di argomenti si consiglia quindi di fare
sempre riferimento alla documentazione ufficiale messa a disposizione
direttamente da Google o alle numerose guide dedicate presenti in rete.

Fatta questa doverosa considerazione passiamo ora ad analizzare nel
dettaglio i diversi parametri che consentono di attivare e configurare
il tracciamento diretto, verso Google Ads, delle conversioni che possono
verificarsi all'interno del sito Passweb in relazione all'evento di
Purchase.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_gads.bmp](./assets/media/image181.png)

**[ID CONVERSIONI GOOGLE ADS]{.underline}:**

Consente di impostare l'identificatore univoco delle conversioni
associate al proprio account Google Ads.

E' una stringa del tipo A**W-XXXXXX** che, come detto, consente a Google
Ads di sapere esattamente a quale account dovranno essere associate le
conversioni registrate all'interno del sito.

Deve essere utilizzato sia nello snippet di codice presente sul sito e
che consente di tracciare la conversione (nel caso di tracciamento
diretto Sito -- Google Ads) sia nella configurazione di un eventuale Tag
di tracciamento implementato all'interno di GTM (nel caso di
tracciamento della conversione mediante Google Tag Manager)

Lo si ricava direttamente da Google Ads in fase di configurazione di un
obiettivo di conversione andando ad esaminare le istruzioni che vengono
fornite da Google Ads stesso in merito all'installazione del codice di
monitoraggio necessario per tracciare la conversione.

Nello specifico sarà quindi necessario:

- Accedere al proprio account Google Ads e portarsi nella sezione
  "**Obiettivi -- Conversioni -- Riepilogo**" dove troveremo un elenco
  di tutti gli obiettivi attualmente codificati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_1.bmp](./assets/media/image182.png)

- Cliccare sul nome dell'obiettivo **relativo alla conversione di
  Purchase** portandosi così nella sua maschera di dettaglio (si ricorda
  che Passweb gestisce il tracciamento diretto Sito -- Google Ads solo
  ed esclusivamente in relazione a conversioni legate ad eventi di
  Purchase)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_2.bmp](./assets/media/image183.png)

- Espandere la sezione "**Impostazione del tag**" in maniera tale da
  poter accedere alle istruzioni di installazione del codice di
  tracciamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_3.bmp](./assets/media/image184.png)

> **ATTENZIONE!** la stessa sezione è presente ovviamente anche al
> termine della codifica di un nuovo obiettivo

- L' Id Conversioni Google Ads può essere a questo punto visualizzato
  sia cliccando sull'opzione "**Installa il tag autonomamente**" sia
  cliccando sull'opzione "**Utilizza Google Tag Manager**"

> Nel primo caso potremo trovarlo direttamente all'interno della sezione
> "**Snippet evento**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_4.bmp](./assets/media/image185.png)

> Nel secondo caso lo troveremo invece (anche se privo del prefisso AW-)
> in corrispondenza del campo "ID conversione"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_5.bmp](./assets/media/image186.png)

> **ATTENZIONE! all'interno del campo Passweb dovrà essere inserito
> necessariamente l'Id Conversione comprensivo del prefisso AW-**

**[LABEL DELLA CONVERSIONE DI ACQUISTO]{.underline}:**

Consente di inserire l'etichetta identificativa della singola
conversione che si desidera tracciare.

In questo senso occorre infatti sottolineare che per identificare un
determinato obiettivo codificato all'interno del proprio account Google
Ads non è sufficiente utilizzare il solo Id delle conversioni indicato
in corrispondenza del precedente parametro.

Tale Id è infatti univoco per ogni singolo account (come precedentemente
sottolineato) ma, all'interno di quello stesso account, possono essere
codificati anche più obiettivi di conversione. Per identificare il
singolo obiettivo di conversione all'interno di quell'account sarà
quindi necessario anche un altro parametro, questa volta univoco per
singola conversione, e questo è proprio la "Label di conversione"

Come per l' "Id delle conversioni", anche la "Label della conversione"
si ricava direttamente da Google Ads in fase di configurazione dello
specifico obiettivo andando ad esaminare le istruzioni di installazione.

Seguendo quindi la stessa procedura indicata per ottenere l' Id delle
conversioni, dovremo portarci nella maschera di dettaglio dell'obiettivo
**relativo alla conversione di Purchase** ed espandere la sezione
relativa alle Impostazioni del Tag

![Videate\\configurazione_gads_3.bmp](./assets/media/image184.png)

La Label della conversione potrà essere quindi visualizzata sia
cliccando sull'opzione "**Installa il tag autonomamente**" sia cliccando
sull'opzione "**Utilizza Google Tag Manager**"

Nel primo caso potremo trovarla direttamente all'interno della sezione
"**Snippet evento**" evidenziata in figura (è la parte dopo lo / )

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_6.bmp](./assets/media/image187.png)

Nel secondo caso la troveremo invece in corrispondenza del campo
"Etichetta conversione"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_7.bmp](./assets/media/image188.png)

**[DISABILITA LA PERSONALIZZAZIONE DEGLI ANNUNCI]{.underline}:**

Consente di gestire il parametro **allow_ad_personalization_signals**
che può essere inserito nelle chiamate effettuate verso Google Ads per
tracciare la conversione

Il parametro in questione controlla se Google potrà poi utilizzare o
meno i dati che gli sono stati inviati per annunci personalizzati.

Nel momento in cui il campo in questione non dovesse essere selezionato
il parametro allow_ad_personalization_signals sarà impostato a true e
questo equivale a dire a Google che gli eventi inviati dal tag diventano
idonei per la personalizzazione degli annunci.

Se invece il campo in questione dovesse essere attivato il parametro
allow_ad_personalization_signals sarà impostato a false, e questo
equivale a dire a Google che gli eventi inviati dal tag non dovranno
essere utilizzati per la personalizzazione degli annunci, mentre
potrebbero comunque essere utilizzati per i report analitici.

**[INSERISCI SNIPPET DI CONVERSIONE ALLA PAGINA DI CONFERMA
ORDINE:]{.underline}**

Se attivato, Passweb inserirà automaticamente, nella pagina di conferma
ordine, lo snippet di codice necessario per trasmettere a Google Ads i
dati dell'ordine effettuato e, di fatto dunque, per tracciare la
relativa conversione.

**ATTENZIONE! a meno di esigenze particolari che potrebbero richiedere
la personalizzazione del codice di tracciamento della conversione, e
posto ovviamente di voler gestire direttamente da Passweb il
tracciamento delle conversioni di Purchase, il parametro in questione
dovrebbe essere sempre selezionato**

Per comprendere meglio l'importanza di questo parametro occorre
considerare che l'implementazione del tracciamento diretto Sito --
Google Ads per le conversioni legate ad eventi di purchase si compone,
sostanzialmente, di due parti.

La prima parte è relativa all'attivazione e alla configurazione del
Google Tag che, come noto, è la colonna portante di tutto il sistema di
tracciamento gestito da Google, non solo in relazione a Google Ads ma
anche a Google Analytics e, in generale, a tutto l'ecosistema di Google.

In questo senso, per quel che riguarda Passweb e Google Ads questa prima
parte è legata all'inserimento dell' "**Id Conversioni Google Ads**" in
corrispondenza del parametro precedentemente analizzato.

Dal punto di vista tecnico infatti, l'impostazione dell' "Id Conversioni
Google Ads" farà si che venga poi inserito, in tutte le pagine del sito,
il codice di attivazione e di gestione del Google Tag in maniera tale da
preparare il sistema all'invio dei dati verso Google Ads.

Se poi il Google Tag dovesse essere già presente nelle varie pagine,
perché è stato attivato anche il tracciamento diretto verso Google
Analytics, l'impostazione dell'Id delle Conversioni andrà solamente ad
inserire all'interno del relativo snippet di codice l'istruzione
necessaria per fare in modo che i dati di tracciamento possano essere
inviati, non solo a Google Analytics, ma anche a Google Ads.

In ogni caso, l'impostazione del Google Tag, di per sé, consente
solamente di configurare e preparare il sito per l'invio dei dati
all'ecosistema Google. L'effettivo invio dei dati di tracciamento
avverrà invece nel momento in cui sul sito dovessero verificarsi
determinati eventi e sarà gestito da altri, specifici, snippet di
codice.

La seconda parte dell'implementazione del sistema di tracciamento si
occupa proprio di questo e, nello specifico quindi, di gestire gli
snippet di codice necessari per inviare a Google Analytics piuttosto che
a Google Ads, al verificarsi di determinati eventi, tutti i dati
necessari per la registrazione di quello stesso evento.

In sostanza dunque, attivando il parametro "**Inserisci snippet di
conversione alla pagina di conferma ordine**" verrà automaticamente
inserito, nella pagina di conferma dell'ordine, uno snippet di codice
del tipo di quello di seguito indicato

*\<script\>*

*gtag(\'event\', \'conversion\', {\'send_to\': \'ID Conversioni Google
Ads/Label della conversione di Acquisto\',*

*\'value\': totale_ordine,*

*\'currency\': \'valuta\',*

*\'transaction_id\': \'id_transazione\',*

*});*

*\</script\>*

**Sulla base di quanto detto è abbastanza semplice comprendere che, se
per qualche ragione, tale snippet di codice non dovesse essere presente
nella pagina di conferma ordine, il sistema non potrà inviare i dati
dell'evento di purchase a Google Ads e, di conseguenza, la conversione
non potrà essere tracciata.**

**ATTENZIONE**! abilitando il parametro "**Inserisci snippet di
conversione alla pagina di conferma ordine**" lo snippet di codice
necessario per il tracciamento della conversione verrà gestito
automaticamente da Passweb e l'utente non dovrà preoccuparsi di nulla

Potrebbero però esserci anche delle situazioni particolari in cui lo
snippet di codice sopra indicato, gestito automaticamente da Passweb,
potrebbe non essere sufficiente per coprire le esigenze del caso dovendo
essere ulteriormente personalizzato.

**In queste situazioni, e solo in queste situazioni**, sarà quindi
necessario non selezionare il parametro in esame e gestire manualmente
l'inserimento dello snippet di codice necessario per il tracciamento,
con le relative personalizzazioni, nella pagina di conferma ordine,
utilizzando per questo il campo "**Codice completamento**" presente alla
pagina "**Configurazione parametri dell'ordine**" del Wizard (tab
"Documento")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_gads_8.bmp](./assets/media/image189.png)

**ATTENZIONE!** nel momento in cui si dovesse decidere di gestire
manualmente lo snippet di codice per l'invio dei dati della transazione
a Google Ads occorre verificare di non aver selezionato il parametro
"**Inserisci snippet di conversione alla pagina di conferma ordine**".
In caso contrario infatti il codice di tracciamento sarebbe di fatto
inserito due volte e, di conseguenza anche la conversione verrebbe
registrata due volte.

Tra i segnaposto presenti all'interno della sezione sopra evidenziata
troveremo, oltre a quelli relativi ai dati dell'ordine, anche i due
segnaposto "**Id Conversioni Google Ads"** e **"Label della conversione
di acquisto Google Ads"** dati questi indispensabili, come visto, per
poter legare l'ordine effettuato sul sito ad un determinato account di
Google Ads e, al suo interno, ad un determinato obiettivo di
conversione.

Per maggiori informazioni relativamente al campo "Codice completamento"
e ai possibili segnaposto utilizzabili al suo interno si veda anche
quanto indicato nel corrispondente capitolo di questo manuale ( "*Ordini
-- Ordini -- Configurazione Ordini -- Documento -- Impostazione di un
codice di tracciamento*" )

Un'ultima cosa di fondamentale importanza da tenere sempre in
considerazione è quella relativa a ciò che può succedere nel momento in
cui l'utente dovesse decidere di pagare l'ordine online.

In queste condizioni, infatti, una volta confermato l'ordine l'utente
uscirà dal sito e verrà ricondotto sul gateway della banca dove potrà
completare il pagamento. Fatto questo, dipendentemente dal metodo di
pagamento utilizzato, l'utente potrebbe anche decidere di non tornare al
sito chiudendo semplicemente il browser.

**In queste condizioni quindi non essendo caricata la pagina di conferma
ordine del sito Passweb, non potrà essere eseguito lo snippet di codice
necessario per inviare a Google Ads i dati della transazione e, di
conseguenza, non potrà essere registrata la conversione.**

Per gestire queste casistiche Google Analytics offre la possibilità di
utilizzare delle chiamate lato server, mediante Measurement Protocol,
che consentono a Passweb, una volta ricevuta la chiamata server 2 server
dal gateway di pagamento (che conferma che tutto è andato a buon fine)
di inviare comunque i dati della transazione a Google Analytics.

A differenza di Analytics, purtroppo, Google Ads non mette a
disposizione un sistema simile per poter consentire a Passweb di inviare
i dati di conversione ad Ads anche nel momento in cui l'utente dovesse
decidere di chiudere il browser sul gateway di pagamento senza poi
tornare al sito, per cui la conversione andrebbe, ovviamente, persa.

In queste condizioni Passweb offre comunque la possibilità di recuperare
la conversione mettendo a disposizione dell'utente i dati di quello
specifico ordine, dati questi che potranno poi essere importati in
Google Ads attraverso la gestione delle "Conversioni avanzate per i
leads" e l'import delle conversioni offline (per maggiori informazioni
in merito si rimanda a quanto indicato all'interno del capitolo "*Google
Ads User Provided Data e Conversioni Avanzate -- Import delle
conversioni offline*" di questo manuale)

**[RACCOLTA DATI UTENTE GOOGLE ADS]{.underline}:**

Se attivato consente di inserire automaticamente nella pagina di
conferma dell'ordine lo snippet di codice necessario per inviare ad Ads,
assieme ai dati della transazione, anche i dati dell'utente che ha
effettuato l'ordine, potendo così gestire in maniera corretta le
Conversioni Avanzate per i web

**ATTENZIONE**! selezionando il parametro in esame lo snippet di codice
necessario per inviare ad Ads i dati dell'utente sarà gestito in
automatico da Passweb e non potrà quindi essere personalizzato in alcun
modo

Nel momento in cui l'esigenza dovesse essere quella di personalizzare
questo snippet di codice o se, per qualsiasi altra ragione, si dovesse
rendere necessario personalizzare l'intero codice di tracciamento della
conversione da inviare a Google Ads, i due parametri "**Inserisci
snippet di conversione alla pagina di conferma ordine**" e "**Raccolta
dati Utente Google Ads**" dovranno essere entrambi deselezionati e, come
già indicato all'interno di questo capitolo, tutto il codice di
tracciamento dovrà essere gestito in maniera manuale utilizzando per
questo il campo "**Codice completamento**" presente alla pagina
"**Configurazione parametri dell'ordine**" del Wizard (tab "Documento")

Dal punto di vista tecnico l'attivazione del parametro in esame
comporta, da una parte la modifica al comando di configurazione di
Google Ads all'interno dello snippet di codice del Google Tag, comando
questo che comprenderà ora anche l'attivazione delle conversioni
avanzate e che sarà quindi del tipo di quello di seguito indicato

*gtag(\'config\', \'AW-XXXXXX\', { \' allow_enhanced_conversions\':true
} ) ;*

Dall'altra parte l'attivazione del parametro in questione comporterà
anche l'inserimento, nella pagina di conferma ordine, del seguente
snippet di codice

*gtag(\'set\', \'user_data\', {*

*\"**sha256_email_address\":* *valore hashato della mail utente*

*\"**sha256_phone_number\":* *valore hashato del telefono utente,*

*\"address\": {*

*\"**sha256_first_name\":* *valore hashato del nome utente,*

*\"**sha256_last_name\":* *valore hashato del cognome / ragione sociale
utente,*

*\"street\":* *indirizzo utente (via),*

*\"city\":* *indirizzo utente (città),*

*\"postal_code\":* *indirizzo utente (CAP),*

*\"country\":* *indirizzo utente (Nazione)*

*}*

*});*

Come si può facilmente osservare, questo snippet di codice è in tutto e
per tutto analogo a quello che sarebbe già presente in tutte le pagine
del sito nel momento in cui avessimo deciso di le conversioni avanzate
anche su Google Analytics (sempre nell'ambito di un tracciamento diretto
Sito -- Google) abilitando il corrispondente parametro presente
all'interno della sezione "Google Analytics"

I due parametri "Raccolta Dati Utente Google Ads" e "Raccolta Dati
Utente GA" sono quindi strettamente collegati tra loro.

Nello specifico l'attivazione del parametro "**Raccolta Dati Utente GA"
comporta poi l'attivazione automatica anche del corrispondente parametro
presente nella sezione Google Ads.**

Di contro invece l'attivazione del parametro "**Raccolta Dati Utente
Google Ads" non comporta l'attivazione automatica del corrispondente
parametro di Google Analytics** e questo perché, da una parte, potremmo
anche decidere di gestire il tracciamento su Google Analytics mediante
Tag Manager e di gestire invece direttamente da Passweb il tracciamento
delle conversioni di purchase e dall'altra parte perché l'attivazione
del parametro "Raccolta Dati Utente Google Ads" comporta l'inserimento
dello snippet di codice richiesto solo nella pagina di conferma ordine a
differenza del corrispondente parametro di Google Analytics che prevede
invece l'inserimento delle stesso snippet di codice ma in tutte le
pagine del sito

**[NOME AZIONE CONVERSIONE]{.underline}**

Consente di impostare il nome assegnato su Google Ads all'azione di
conversione (tipicamente quella legata agli acquisti effettuati sul
sito) in relazione alla quale dovrà poi essere effettuato l'import dei
dati di conversione offline

Il nome in esame è quello indicato su Ads nella maschera di riepilogo
degli obiettivi in corrispondenza della colonna "**Azione di
conversione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_3.bmp](./assets/media/image190.png)

oppure nel dettaglio dello specifico obiettivo in corrispondenza del
campo "**Nome Conversione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_4.bmp](./assets/media/image191.png)

**ATTENZIONE!** è di fondamentale importanza che il nome inserito
all'interno di questo campo coincida esattamente, anche a livello di
spazi, lettere maiuscole e minuscole, con quello assegnato su Ads alla
relativa azione di conversione.

Il valore di questo campo verrà infatti inserito anche in corrispondenza
della colonna "**Conversion Name**" nei vari file di esportazione
prodotti da Passweb e che dovranno poi essere uplodati su Google Ads
nell'ambito del processo import delle conversioni offline e nel caso in
cui i due valori non dovessero coincidere l'assegnazione delle
conversioni offline potrebbe anche non essere effettuata in maniera
corretta.

Per maggiori informazioni in merito all'import delle conversioni offline
si veda anche quanto indicato all'interno del relativo capitolo di
questo manuale ("*Google Ads User Provided Data e Conversioni Avanzate
-- Import delle conversioni offline*")

**[INSERISCI GCLID IN EXPORT CSV:]{.underline}**

Consente, se attivato, di inserire nel tracciato record reso disponibile
da Passweb in merto agli ordini soggetti all' "Import delle conversioni
offline", anche il valore del parametro **GCLID**, valore questo che
verrà prelevato, se presente, direttamente dai cookie di Google e che
potrebbe essere utile per consentire a Google Ads, in fase di import
della conversione offline, di assegnare la conversione stessa alla
corretta campagna (tipicamente il consiglio è quindi quello di attivare
sempre questo parametro)

Per maggiori informazioni in merito all'import delle conversioni offline
si veda anche quanto indicato all'interno del relativo capitolo di
questo manuale ( "*Google Ads User Provided Data e Conversioni Avanzate
-- Import delle conversioni offline*")

**[ATTIVA REMARKETING DINAMICO:]{.underline}**

Consente, se attivato, di abilitare l'invio diretto a Google ADS dei
dati necessari alla gestione del Remarketing Dinamico.

Dal punto di vista tecnico l'attivazione di questo parametro comporterà,
in corrispondenza degli eventi di:

- **view_item_list**

- **view_item**

- **add_to_cart**

- **purchase**

l'esecuzione di un comando del tipo di quello qui di seguito riportato

*\<script\>*

*gtag('event', 'nome_evento', {'send_to': 'ID Conversioni Google Ads',*

*'value':2450,*

*'items': \[*

*{*

*'id': '1234',*

*'google_business_vertical': 'retail'*

*},*

*\...*

*{*

*'id': '45678',*

*'google_business_vertical': 'retail'*

*}*

*\]*

*});*

*\</script\>*

dove i parametri correlati al comando in questione verranno valorizzati
come di seguito indicato:

- **ID Conversioni Google Ads**: Identificatore univoco delle
  conversioni associate al proprio account Google Ads.

> **ATTENZIONE!** verrà utilizzato il valore inserito all'interno del
> corrispondente campo della sezione Google Ads
>
> E' semplice comprendere dunque che, per poter gestire in maniera
> corretta il Remarketing Dinamico non sarà sufficiente abilitare il
> parametro "**Attiva Remarketing Dinamico**" ma sarà necessario aver
> valorizzato in maniera corretta anche il parametro '**ID Conversioni
> Google Ads**' evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_configurazione_remarketing_dinamico.bmp](./assets/media/image192.png)

- **nome_evento**: nome dell'evento (view_item_list / view_item /
  add_to_cart / purchase) che ha fatto scattare l'esecuzione del comando
  di Remarketing

<!-- -->

- **value:** somma dei prezzi ivati dei prodotti coinvolti nell'evento

- **items:** array dei prodotti coinvolti nell'evento (ovviamente per
  gli eventi di add_to_cart e view_item si avrà un array di un solo
  elemento)

- **id:** codice del prodotto coinvolto nell'evento

- **google_buinsess_vertical**: parametro necessario per indicare la
  tipologia di Feed in cui Google andrà poi a cercare, per fare il
  match, il prodotto con il codice indicato in corrispondenza del
  precedente parametro id.

> Valorizzato sempre con la stringa '**retail**' come da documentazione
> Google (https://support.google.com/google-ads/answer/7305793)

**ATTENZIONE!** i dati passati ad con il comando sopra evidenziato
potranno essere utilizzati solo in combinazione con un Feed Prodotti di
Merchant Center.

Ciò significa, dunque, che per poter gestire in maniera corretta il
Remarketing Dinamico non sarà sufficiente inviare ad Ads, in
corrispondenza degli eventi indicati, i dati dei prodotti coinvolti in
questi stessi eventi nel formato richiesto da Google, ma sarà necessario
gestire in maniera corretta i corrispondenti prodotti anche all'interno
del proprio Merchant Center. E' proprio dal Merchant Center infatti che
Google andrà a reperire in maniera automatica (utilizzando come chiave
l'id prodotto passato ad Ads) tutte le informazioni necessarie per
gestire poi le varie campagne dei prodotti coinvolti nel Remarketing
Dinamico

##### EVENTI ECOMMERCE PER GOOGLE ANALYTICS E GOOGLE TAG MANAGER

Come già indicato nei precedenti capitoli di questo manuale, nel momento
in cui l'esigenza dovesse essere quella di attivare per il proprio sito
anche un monitoraggio Ecommerce, in maniera tale da poter poi disporre
su Analytics di dati quali, ad esempio, gli articoli aggiunti / rimossi
dal carrello, gli articoli visualizzati, gli ordini effettuati ... sarà
necessario configurare in maniera adeguata anche i parametri presenti
all'interno di questa sezione, e questo indipendentemente dal fatto di
utilizzare l'integrazione diretta Passweb -- Google Analytics oppure di
passare attraverso Google Tag Manager.

Nel primo caso (integrazione diretta Passweb -- Google Analytics)
infatti, l'attivazione dei parametri presenti all'interno di questa
sezione consentirà all'applicativo di inviare direttamente ad Analytics
i relativi dati Ecommerce, nel secondo caso (utilizzo di Google tag
Manager) invece, l'abilitazione di questi parametri consentirà
all'applicativo di attivare i diversi eventi ecommerce e di inserire nei
relativi dataLayer tutte le informazioni necessarie per configurare in
maniera corretta, su GTM, i corrispondenti Tag di tracciamento.

**ATTENZIONE! nel momento in cui alcuni di questi parametri dovessero
non essere configurati in maniera corretta non sarà possibile attivare i
corrispondenti eventi ecommerce e, conseguentemente, non verranno
inserite nel dataLayer le informazioni necessarie rendendo di fatto
impossibile effettuare un corretto monitoraggio di questi stessi
eventi**

Fatte queste considerazioni di fondamentale importanza, esaminiamo ora
più nel dettaglio ciascuno dei parametri presenti all'interno di questa
sezione, distinguendo quello che la loro attivazione effettivamente
comporta nel caso in cui si sia deciso di utilizzare UA oppure GA4

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_eventi_ecommerce.bmp](./assets/media/image193.png)

**Google Analytics -- Ricerca sul Sito:** consente di decidere se
attivare o meno il tracciamento degli eventi di ricerca interni al sito
( posto ovviamente che per effettuare queste ricerche siano stati
utilizzati i componenti nativi di Passweb ).

E' possibile selezionare uno dei seguenti valori:

- **Disabilitato**: in queste condizioni il tracciamento degli eventi di
  ricerca interni al sito verrà disabilitato e i relativi dati non
  verranno quindi inviati ad Analytics in nessun modo

- **Abilitato**: selezionando questa opzione verrà abilitata la gestione
  degli eventi di ricerca interni al sito per cui nel caso in cui si sia
  deciso di utilizzare:

<!-- -->

- **Il tracciamento diretto Sito -- GA4:** l'attivazione di questo
  parametro comporterà l'invio alla proprietà GA4 collegata dell'evento
  *search* (Ricerca) secondo quanto indicato all'interno dei
  corrispondenti capitoli della sezione "*Google Analytics -- Google
  Analytics 4 -- Monitoraggio Ecommerce*" di questo manuale

- **Il tracciamento mediante GTM**: l'attivazione di questo parametro
  comporterà l'attivazione dell'evento *search* e contestualmente la
  creazione del dataLayer secondo quanto indicato all'interno dei
  corrispondenti capitoli della sezione "*Google Tag Manager -- GTM e
  GA4 -- Tracciamento degli eventi Ecommerce*" di questo manuale

**Google Analytics -- Eventi Articolo:** consente di decidere se
attivare o meno il tracciamento dei seguenti eventi ecommerce:

- view_item_list (Impressione Prodotti)

- select_item (Click Prodotto)

- view_item (Impressione Dettaglio Prodotto)

E' possibile selezionare uno dei seguenti valori:

- **Disabilitato**: in queste condizioni il tracciamento degli eventi
  indicati verrà disabilitato e i relativi dati non verranno quindi
  inviati ad Analytics in nessun modo

- **Abilitato**: selezionando questa opzione verrà abilitata la gestione
  degli eventi sopra indicati per cui nel caso in cui si sia deciso di
  utilizzare:

<!-- -->

- **Il tracciamento diretto Sito -- GA4**: l'attivazione di questo
  parametro comporterà l'invio alla proprietà GA4 collegata degli eventi
  indicati secondo quanto descritto all'interno dei corrispondenti
  capitoli della sezione "*Google Analytics -- Google Analytics 4 --
  Monitoraggio Ecommerce*" di questo manuale

- **Il tracciamento mediante GTM:** l'attivazione di questo parametro
  comporterà l'attivazione degli eventi indicati e contestualmente la
  creazione del dataLayer secondo quanto indicato all'interno dei
  corrispondenti capitoli della sezione "*Google Tag Manager -- GTM e
  GA4 -- Tracciamento degli eventi Ecommerce*" di questo manuale

**Google Analytics -- Eventi Carrello e Wishlist:** consente di decidere
se attivare o meno il tracciamento dei seguenti eventi ecommerce.

- add_to_cart (Aggiunta in Carrello)

- remove_from_cart (Rimozione dal Carrello)

- add_to_wishlist (Aggiunta in Wishlist)

- view_cart (Visualizzazione Carrello)

E' possibile selezionare uno dei seguenti valori:

- **Disabilitato**: in queste condizioni il tracciamento degli eventi
  indicati verrà disabilitato e i relativi dati non verranno quindi
  inviati ad Analytics in nessun modo

- **Abilitato**: selezionando questa opzione verrà abilitata la gestione
  degli eventi sopra indicati per cui nel caso in cui si sia deciso di
  utilizzare:

  - **Il tracciamento diretto Sito -- GA4**: l'attivazione di questo
    parametro comporterà l'invio alla proprietà GA4 collegata degli
    eventi indicati secondo quanto descritto all'interno dei
    corrispondenti capitoli della sezione "*Google Analytics -- Google
    Analytics 4 -- Monitoraggio Ecommerce*" di questo manuale

  - **Il tracciamento mediante GTM:** l'attivazione di questo parametro
    comporterà l'attivazione degli eventi indicati e contestualmente la
    creazione del dataLayer secondo quanto indicato all'interno dei
    corrispondenti capitoli della sezione "*Google Tag Manager -- GTM e
    GA4 -- Tracciamento degli eventi Ecommerce*" di questo manuale

**Google Analytics -- Eventi Checkout:** consente di decidere se
attivare o meno il tracciamento dei seguenti eventi ecommerce.

- begin_checkout (Inizio Checkout)

- add_payment_info (Informazioni di pagamento)

- add_shipping_info (Informazioni di spedizione)

- purchase (Acquisto)

E' possibile selezionare uno dei seguenti valori:

- **Disabilitato**: in queste condizioni il tracciamento degli eventi
  indicati verrà disabilitato e i relativi dati non verranno quindi
  inviati ad Analytics in nessun modo

- **Abilitato**: selezionando questa opzione verrà abilitata la gestione
  degli eventi sopra indicati per cui nel caso in cui si sia deciso di
  utilizzare:

  - **Il tracciamento diretto Sito -- GA4**: l'attivazione di questo
    parametro comporterà l'invio alla proprietà GA4 collegata degli
    eventi indicati secondo quanto descritto all'interno dei
    corrispondenti capitoli della sezione "*Google Analytics -- Google
    Analytics 4 -- Monitoraggio Ecommerce*" di questo manuale

  - **Il tracciamento mediante GTM:** l'attivazione di questo parametro
    comporterà l'attivazione degli eventi indicati e contestualmente la
    creazione del dataLayer secondo quanto indicato all'interno dei
    corrispondenti capitoli della sezione "*Google Tag Manager -- GTM e
    GA4 -- Tracciamento degli eventi Ecommerce*" di questo manuale

**ATTENZIONE!** per attivare un tracciamento ecommerce completo è
necessario attivare tutti i parametri sopra indicati. Nel momento in cui
alcuni di essi non dovessero essere selezionati gli eventi
corrispondenti non verranno inviati ad Analytics e/o non verranno
inseriti nel dataLayer in uso al sito

**Google Analytics -- Eventi Utente:** consente di decidere se attivare
o meno il tracciamento dei seguenti eventi

- login (autenticazione al sito),

- sign_up (registrazione al sito)

- generate_lead (completamento form)

E' possibile selezionare uno dei seguenti valori:

- **Disabilitato**: in queste condizioni il tracciamento degli eventi
  indicati verrà disabilitato e i relativi dati non verranno quindi
  inviati ad Analytics in nessun modo

- **Abilitato**: selezionando questa opzione verrà abilitata la gestione
  degli eventi sopra indicati per cui nel caso in cui si sia deciso di
  utilizzare:

  - **Il tracciamento diretto Sito -- GA4**: l'attivazione di questo
    parametro comporterà l'invio alla proprietà GA4 collegata degli
    eventi indicati secondo quanto descritto all'interno dei
    corrispondenti capitoli della sezione "*Google Analytics -- Google
    Analytics 4 -- Monitoraggio Ecommerce*" di questo manuale

  - **Il tracciamento mediante GTM:** l'attivazione di questo parametro
    comporterà l'attivazione degli eventi indicati e contestualmente la
    creazione del dataLayer secondo quanto indicato all'interno dei
    corrispondenti capitoli della sezione "*Google Tag Manager -- GTM e
    GA4 -- Tracciamento degli eventi Ecommerce*" di questo manuale

##### PERSONALIZZAZIONE GOOGLE TAG

Come già evidenziato nei precedenti capitoli di questo manuale,
potrebbero configurarsi delle situazioni particolari in cui lo snippet
di codice relativo al Google Tag inserito automaticamente da Passweb
nelle varie pagine del sito, e indispensabile per gestire il
tracciamento diretto verso Google Analytics / Google Ads potrebbe
richiedere ulteriori personalizzazioni per gestire determinate
funzionalità che, allo stato attuale, non possono essere semplicemente
attivate con un corrispondente parametro Passweb

In queste condizioni **sarà necessario inserire integralmente tutto il
codice di tracciamento del Google Tag** in corrispondenza del campo
"**Codice Google Tag**" presente all'interno della sezione
"**Personalizzazione Google Tag**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\personalizzazione_google_tag.bmp](./assets/media/image194.png)

**Codice Google Tag:** consente di impostare manualmente lo snippet di
codice da utilizzare per inviare i dati di tracciamento a Google
Analytics / Google Ads.

Ovviamente nel momento in cui si dovesse decidere di personalizzare il
codice del Google Tag, valorizzando il campo in esame, sarà poi questo
(e non più quello gestito in automatico da Passweb) ad essere inserito
nelle varie pagine del sito per cui il consiglio è quello di valorizzare
il campo in esame solo se strettamente necessario e comunque sempre in
maniera più che consapevole inquanto eventuali errori di impostazione
nello snippet di codice del Google Tag potrebbero poi compromettere
l'interno sistema di tracciamento del sito.

Nel caso in cui si dovesse comunque decidere di personalizzare il codice
di tracciamento, il campo "**Seleziona un segnaposto**" presente
immediatamente al di sopra dell'editor di codice consente di inserire i
seguenti segnaposto:

- **Chiave Google Analytics:** consente di inserire nel codice di
  tracciamento il segnaposto **{chiaveGoogleAnalytics}** che verrà poi
  sostituito, in fase di costruzione della pagina web, con il valore
  eventualmente inserito in corrispondenza dell'omonimo campo presente
  all'interno della sezione "Google Analytics"

- **ID Conversioni Google Ads:** consente di inserire nel codice di
  tracciamento il segnaposto **{chiaveGoogleADS}** che verrà poi
  sostituito, in fase di costruzione della pagina web, con il valore
  eventualmente inserito in corrispondenza dell'omonimo campo presente
  all'interno della sezione "Google Ads"

- **Label della conversione di Acquisto Google Ads:** consente di
  inserire nel codice di tracciamento il segnaposto
  **{labelConvesioneAcquisto}** che verrà poi sostituito, in fase di
  costruzione della pagina web, con il valore eventualmente inserito in
  corrispondenza dell'omonimo campo presente all'interno della sezione
  "Google Ads"

- **User ID:** consente di inserire nel codice di tracciamento il
  segnaposto **{userId}** che verrà poi sostituito, in fase di
  costruzione della pagina web con il codice identificativo dell'utente,
  posto ovviamente che l'utente che sta navigando il sito abbia
  effettuato correttamente il login (per utenti non autenticati lo User
  Id avrà ovviamente valore nullo)

**ATTENZIONE!** nel momento in cui si dovesse decidere di utilizzare i
segnaposto sopra indicati sarà indispensabile, ovviamente, accertarsi di
aver inserito i corretti valori in corrispondenza dei relativi campi
Passweb

Si ricorda inoltre che nel caso in cui non ci sia la necessità di
personalizzare il codice di monitoraggio, o allo stesso modo, nel caso
in cui si dovesse decidere di implementare il sistema di tracciamento
del proprio sito mediante Google Tag Manager, sarà perfettamente
sufficiente inserire i relativi parametri di configurazione all'interno
delle sezioni "Google Analytics", "Google Ads", o "Google Tag Manager"
secondo quanto indicato nei precedenti capitoli di questo manuale
lasciando quindi vuota la sezione in oggetto.

Un'ultima considerazione di fondamentale importanza da fare è che il
campo "Codice Google tag" consente di personalizzare solo ed
esclusivamente lo snippet di codice dello stesso Google Tag che di per
sé potrebbe essere utilizzato per inviare ad analytics, ad esempio, la
sola pageview ma non gli eventi ecommerce (aggiunta al carrello,
acquisto ...) che continueranno ad essere gestiti in automatico da
Passweb e che dovranno quindi essere opportunamente attivati mediante i
parametri presenti all'interno della sezione "**Eventi Ecommerce per
Google Analytics e Google Tag Manager**" (per maggiori informazioni in
merito si rimanda a quanto indicato nel successivo capitolo di questo
manuale)

##### PARAMETRI GENERALI

La sezione "**Parametri Generali**" consente di impostare alcuni
parametri di configurazione che possono rivelarsi particolarmente utili
a livello generale sia per il tracciamento Google che per il
tracciamento Facebook.

Il data model utilizzato da GA4, come noto, è basato interamente sugli
eventi e uno dei principali vantaggi in questo senso è rappresentato
proprio dal fatto di poter completare autonomamente la struttura del
tracking decidendo esattamente quali parametri passare ad Analytics al
fine di tracciare, secondo le nostre specifiche esigenze, ogni evento in
maniera più dettagliata.

In altre parole, in base a quelli che sono i nostri obiettivi di analisi
potremo scegliere a nostra discrezione tutti i parametri utili a
descrivere meglio il contesto in cui l'evento si è verificato

In questo senso, ad esempio, un parametro particolarmente importante da
passare assieme ad ogni evento, soprattutto quelli contrassegnati come
conversioni, è sicuramente il parametro "**value**", parametro questo
che consente di assegnare all'evento stesso un ben preciso valore
monetario.

I campi presenti all'interno della sotto sezione "**Parametro Value
eventi Google Analytics, Google Tag Manager e Facebook Pixel**"
consentono proprio di impostare, per ciascuno degli eventi gestiti nelle
varie integrazioni, uno specifico valore per il parametro value,
assegnando quindi all'evento stesso il valore monetario desiderato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_parametro_value.bmp](./assets/media/image195.png)

Nello specifico il campo:

**GA4 - FB 🡪 purchase**: consente di impostare il valore da assegnare al
parametro value per l'evento "***purchase***". Il valore assegnato verrà
quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  con il "Totale Ordine" della transazione appena conclusa

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

**GA4 - FB 🡪 add_payment_info**: consente di impostare il valore da
assegnare al parametro value per l'evento "***add_payment_info***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore Monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al "Totale Merce Ivato" della transazione in essere

**GA4 - FB 🡪 add_shipping_info**: consente di impostare il valore da
assegnare al parametro value per l'evento "***add_shipping_info***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore Monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al "Totale Merce Ivato" della transazione in essere

**GA4 - FB 🡪 begin_checkout**: consente di impostare il valore da
assegnare al parametro value per l'evento "***begin_checkout***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore Monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al "Totale Merce Ivato" della transazione in essere

**GA4 - FB 🡪 add_to_wishlist**: consente di impostare il valore da
assegnare al parametro value per l'evento "***add_to_wishlist***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  alla quantità con cui il relativo articolo è stato aggiunto in
  wishlist

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al prezzo ivato dell'articolo che è stato aggiunto in
  wishlist

**GA4 - FB 🡪 add_to_cart**: consente di impostare il valore da assegnare
al parametro value per l'evento "***add_to_cart***". Il valore assegnato
verrà quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  alla quantità con cui il relativo articolo è stato aggiunto in
  carrello

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al prezzo ivato dell'articolo che è stato aggiunto in
  carrello

**GA4 - FB 🡪 remove_from_cart**: consente di impostare il valore da
assegnare al parametro value per l'evento "***remove_from_cart***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  alla quantità con cui il relativo articolo è stato rimosso dal
  carrello

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al prezzo ivato dell'articolo che è stato rimosso dal
  carrello

**GA4 - FB 🡪 view_item**: consente di impostare il valore da assegnare
al parametro value per l'evento "***view_item***". Il valore assegnato
verrà quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  al prezzo di vendita del corrispondente articolo

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

**GA4 - FB 🡪 select_item**: consente di impostare il valore da assegnare
al parametro value per l'evento "***select_item***". Il valore assegnato
verrà quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

- **Valore monetario**: in queste condizioni il valore del parametro
  value verrà assegnato automaticamente da Passweb e corrisponderà,
  nello specifico, al prezzo ivato del relativo articolo

**GA4 - FB 🡪 view_item_list**: consente di impostare il valore da
assegnare al parametro value per l'evento "***view_item_list***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

**GA4 - FB 🡪 view_cart**: consente di impostare il valore da assegnare
al parametro value per l'evento "***view_cart***". Il valore assegnato
verrà quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  assegnato automaticamente da Passweb e corrisponderà, nello specifico,
  al "Totale Carrello"

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

**GA4 - FB 🡪 search**: consente di impostare il valore da assegnare al
parametro value per l'evento "***search***". Il valore assegnato verrà
quindi inviato ad Analytics assieme all'evento stesso nel caso di
integrazione diretta Passweb -- Analytics oppure verrà inserito nella
struttura del corrispondente Data Layer nel caso in cui si sia deciso di
utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

**GA4 - FB 🡪 generate_lead**: consente di impostare il valore da
assegnare al parametro value per l'evento "***generate_lead***". Il
valore assegnato verrà quindi inviato ad Analytics assieme all'evento
stesso nel caso di integrazione diretta Passweb -- Analytics oppure
verrà inserito nella struttura del corrispondente Data Layer nel caso in
cui si sia deciso di utilizzare Google Tag Manager (GTM).

E' possibile selezionare una delle seguenti opzioni:

- **Default**: in queste condizioni il valore del parametro value verrà
  impostato automaticamente da Passweb sull'valore 1

- **Personalizzato**: selezionando questa opzione verrà visualizzato un
  ulteriore campo di input all'interno del quale poter inserire
  manualmente lo specifico valore da assegnare al parametro value

La sotto sezione "**Parametri personalizzabili Google Analytics**"
consente invece di definire i campi gestionali da cui prelevare
determinate informazioni che dovranno poi essere passate ad Analytics
(tracciamento diretto) e/o inserite nel data layer (tracciamento
mediante Google Tag Manager)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_personalizzabili_ga.bmp](./assets/media/image196.png)

In particolare il campo:

**Parametro Brand**: consente di definire il campo del gestionale o lo
specifico attributo passweb da cui dovrà essere prelevata l'informazione
relativa al Brand, informazione questa che verrà poi inserita nella
struttura dell'oggetto item passato ad Analytics e nei vari eventi
ecommerce gestiti dal data layer di Passweb.

E' possibile selezionare una delle seguenti opzioni:

- **Categoria Statistica**: selezionando questa opzione l'informazione
  relativa al Brand verrà prelevata dalla Categoria Statistica
  associata, lato gestionale, al corrispondente articolo

- **Natura**: selezionando questa opzione l'informazione relativa al
  Brand verrà prelevata dalla Natura associata, lato gestionale, al
  corrispondente articolo

- **Attributi Passweb:** selezionando questa opzione l'informazione
  relativa al Brand verrà prelevata dall' Attributo Passweb indicato

