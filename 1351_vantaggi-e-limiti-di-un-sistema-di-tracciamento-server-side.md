# VANTAGGI E LIMITI DI UN SISTEMA DI TRACCIAMENTO SERVER SIDE



In considerazione di tutto quanto detto nel precedente capitolo di
questo manuale e una prima osservazione di fondamentale importanza da
fare è che **l'implementazione di un sistema di tracciamento server side
non vuol dire assolutamente abbandonare in maniera definitiva il
tracciamento lato client fino ad ora implementato per il nostro sito**.

Come visto infatti, il tracciamento lato client rappresenta il punto
iniziale di tutto il processo essendo il sistema deputato a raccogliere
tutte le informazioni relative agli eventi che si verificano sul nostro
sito. In considerazione di ciò dovrà continuare ad essere gestito
esattamente allo stesso modo in cui lo si gestiva prima di attivare
anche il tracciamento server side (quindi mediante integrazione nativa
sul sito o mediante l'utilizzo di un contenitore GTM di tipo web).
L'unica differenza in questo senso è rappresentata dal fatto che, una
volta attivato il tracciamento server side, quello lato client dovrà
essere configurato in maniera tale che i dati raccolti non vengano più
inviati direttamente agli endpoint dei server di Analytics ma bensì al
contenitore GTM di tipo server che avremo attivato.

**L'altro elemento imprescindibile di tutto il sistema è dunque il
contenitore GTM di tipo server** deputato ad acquisire i dati di
tracciamento inviati dal nostro sito per poi elaborarli e ritrasmetterli
ai server di Analytics.

Avendo ben chiari questi aspetti e considerando anche come opera tutto
il sistema risulta abbastanza semplice comprendere che i suoi vantaggi
più evidenti possono essere quelli di seguito elencati:

- **[Meno script caricati nella pagina e quindi potenzialmente maggiori
  performance per il sito]{.underline}**

> Come precedentemente evidenziato in un sistema di tracciamento client
> side "tradizionale" ogni singolo Tag che andremo ad implementare
> comporterà poi l'installazione sul sito di una ben precisa libreria
> javascript indispensabile per gestire le chiamate al relativo endpoint
> e per inviargli, nella maniera in cui l'endpoint stesso richiede,
> tutti i dati di tracciamento.
>
> In sostanza se dovessimo tracciare una page view su Analytics, su
> Facebook e su Hotjar dovremo avere tre distinte librerie javascript
> installate sul sito, e tre distinti flussi di dati in uscita dal sito
> e diretti verso i tre distinti endpoint di Google, di facebook e di
> Hotjar
>
> In un sistema di tracciamento server side, potenzialmente, potremo
> avere invece un unico flusso di dati in uscita dal sito (e quindi
> un\'unica libreria javascript installata) che porta con se
> l'informazione della page view generando quindi un\'unica richiesta al
> contenitore server side di GTM. Qui un Client potrebbe interpretare
> questa richiesta e far attivare conseguentemente tre distinti Tag
> (sempre di tipo server) appositamente configurati per inoltrare
> l'evento di page view ai tre distinti endpoint di Google, di facebook
> e di Hotjar.

- **[Maggior controllo e maggior qualità dei dati]{.underline}**

> Uno dei vantaggi più evidenti in un sistema di tracciamento server
> side è rappresentato dal fatto che i dati raccolti sul nostro sito non
> vengono inviati direttamente ai server di Google ma passano prima
> attraverso un server esterno di nostra proprietà su cui è installato
> un contenitore GTM server side
>
> In questo senso il punto fondamentale è che possiamo avere il pieno
> controllo sia di questo server che, ovviamente, del contenitore GTM
> che andremo ad installare. Avremo accesso completo ai dati provenienti
> dal sito web e questo ci consente, prima di passare queste
> informazioni ad un qualunque servizio di terze parti (Google
> Analytics, Facebook ...) di "ripulirle", modificarle o addirittura,
> potenzialmente, di integrarle con altre informazioni che per noi
> possono essere particolarmente rilevanti.
>
> Parte di queste operazioni possono essere fatte direttamente dalle
> configurazioni dei Tag che andremo a gestire sul contenitore Server di
> GTM (ad esempio per GA4 è possibile decidere esattamente quali dei
> parametri in ingresso al server devono effettivamente essere esclusi o
> inoltrati ai server di Analytics), altre (come ad esempio
> l'integrazione dei dati in ingresso con altre informazioni prelevate
> ad esempio dal nostro CRM) richiedono invece apposite conoscenze di
> programmazione e sono quindi più complesse da realizzare
>
> In ogni caso il fatto di poter collocare quello che di fatto è il
> nostro server proxy in Europa, assieme al fatto di avere il pieno
> controllo dei dati in ingresso e di decidere esattamente quali dati
> passare e quali no ai server di Google aumenta di molto la sicurezza
> di tutto il sistema e aiuta parecchio (anche se al momento non è una
> soluzione definitiva al 100%) in termini di GDPR

- **[Maggior controllo sull'utilizzo di cookie di terze
  parti]{.underline}**

> Come precedentemente evidenziato uno dei problemi principali in un
> sistema di tracciamento client side "tradizionale" è rappresentato dal
> fatto che la tendenza generale di tutti i browser (compreso lo stesso
> Chrome) è ormai quella di arrivare a bloccare completamente l'utilizzo
> dei cookie di terze parti.
>
> In questo senso l'utilizzo di un sistema server side può aiutare
> moltissimo nella misura in cui al server su cui andremo a gestire il
> tutto venga assegnato un sotto dominio del dominio principale in uso
> al sito che si vuole tracciare. In altri termini, supponendo che il
> sito risponda al dominio www.clobis.net, al server su cui andremo ad
> installare GTM dovrebbe essere assegnato un sottodominio del tipo
> gtm.cloblis.net.
>
> In queste condizioni infatti il nostro sito web e il server GTM si
> troveranno ad operare in un contesto di same-site e questo significa
> che i cookie installati sul browser dell'utente (non più dai server di
> Analytics con cui non c'è comunicazione diretta ma bensì dal nostro
> contenitore server side) e che resteranno comunque fondamentali per
> poter implementare tutto il tracciamento lato client, verranno
> installati come cookie di prima parte e non saranno quindi più
> soggetti ai blocchi implementati dai vari browser.
>
> In aggiunta a tutto ciò, un ulteriore vantaggio introdotto
> recentemente da Google, è rappresentato dalla possibilità di
> personalizzare, in fase di configurazione del Tag Server di GA4, anche
> la durata dei cookie che verranno installati sul browser dell'utente,
> superando quindi anche il limite della durata di 7 giorni imposto
> sempre dai vari browser per i cookie di prima parte.

Per quel che riguarda invece gli aspetti "negativi", occorre sicuramente
tenere in considerazione i seguenti limiti connessi ad un sistema di
tracciamento server side

- **[Sistema che richiede un know-how tecnico abbastanza
  elevato]{.underline}**

> Considerando i concetti che stanno alla base di un sistema di
> tracciamento server side appare già evidente, anche senza entrare nei
> dettagli specifici dell'implementazione, che per poter mettere in
> piedi questo tipo di sistema sono richieste conoscenze tecniche
> piuttosto elevate.
>
> Da una parte è assolutamente vero che si stanno diffondendo
> piattaforme come Stape.io che facilitano notevolmente
> l'implementazione di tutto il sistema, dall'altra parte però resta
> valido il fatto che per poter implementare tutto correttamente occorre
> avere una certa familiarità con concetti come server e client, dns,
> richieste http ... concetti che non sempre sono richiesti a chi si
> deve occupare di analisi dati e digital marketing. Il tutto poi
> aumenterebbe esponenzialmente se, per ridurre i costi, si volesse
> implementare e gestire in casa il server dedicato ad ospitare GTM

- **[Sistema a pagamento]{.underline}**

> Questa è forse la nota più dolente per chi è abituato ad utilizzare
> gratuitamente gli strumenti di tracciamento e analisi dati messi a
> disposizione da Google. Il sistema di tracciamento server side
> richiede necessariamente una spesa che tra l'altro, a seconda dei
> casi, potrebbe anche non essere di poco conto
>
> **ATTENZIONE!** Quello che si paga in un sistema di tracciamento
> server side non è GTM che rimane sempre uno strumento gratuito
>
> Quello che si paga è il server intermedio su cui dovrà essere
> installato GTM e, generalmente, il traffico generato verso di esso. In
> considerazione di ciò nel momento in cui si dovesse optare per un
> deploy di questo server su piattaforme come Google Cloud, Amazon AWS,
> Azure ... occorre fare particolare attenzione a come viene configurato
> il tutto e anche a quelli che sono effettivamente gli eventi che si
> vogliono tracciare perché anche un piccolo errore di configurazione
> potrebbe portare ad aumentare notevolmente il traffico in ingresso e
> in uscita da questo server facendo quindi salire rapidamente i costi,
> che per questo tipo di sistemi variano proprio in base all'utilizzo
> (oltre che ovviamente alla spazio a disposizione per la memorizzazione
> dei dati, alle prestazioni del server, alla scalabilità automatica di
> tutto il sistema al crescere del traffico gestito ...)
>
> E' vero che esistono piattaforme come Stape.io che consentono per siti
> di piccole/medie dimensioni di contenere i costi in un range
> accettabile (si parla più o meno di 200€ annui per 500000 richieste in
> ingresso al server) ma sono comunque costi da tenere in considerazione
> rispetto ad un tradizionale tracciamento client side che poteva essere
> implementato a 0

- **[Scarsa disponibilità (al momento) di vendor in grado di gestire end
  point server side]{.underline}**

> Tra i vantaggi precedentemente elencati per il tracciamento server
> side abbiamo indicato il fatto di poter avere in uscita dal sito,
> potenzialmente, un unico flusso di dati che viene poi tradotto da un
> apposito Client presente sul contenitore GTM di tipo server generando
> un evento in grado si poter essere gestito da N Tag anch'essi di tipo
> server che invieranno l'informazione ad altrettanti distinti sistemi
> di tracciamento.
>
> Ora se da una parte è vero che, effettivamente, tutto ciò potrebbe
> portarci ad installare non N ma una sola libreria javascript
> aumentando quindi le prestazioni del sito (oltre a facilitare la
> gestione di tutto il sistema di tracciamento lato client) dall'altra
> parte è altrettanto vero che affinché tutto il sistema possa
> funzionare in maniera corretta è necessario poter disporre sul
> contenitore di tipo server di Client in grado di gestire le richieste
> in ingresso e di Tag di tipo server in grado di prendersi in carico
> gli eventi generati da questo Client e di inoltrare le informazioni di
> tracciamento al relativo endpoint.
>
> Il problema in questo senso è rappresentato proprio dal fatto che,
> attualmente, i vendor in grado di mettere a disposizione all'interno
> di GTM server side dei Client e dei Tag in grado di interagire con i
> loro sistemi sono piuttosto limitati. Tanto per capirci se non
> avessimo avuto a disposizione nel contenitore GTM di tipe server un
> Client GA4 e il relativo Tag non avremmo potuto implementare per GA4
> questo tipo di tracciamento.
>
> Nel momento in cui lo specifico vendor, come può essere ad esempio
> Hotjar, dovesse quindi richiedere obbligatoriamente l'installazione di
> una libreria javascript sul sito e/o non dovesse metterci a
> disposizione una gestione server side del suo endpoint (con appositi
> Client e Tag) non potremmo far altro che mantenere per esso il
> tradizionale tracciamento lato client.

- **[Non elimina assolutamente il tracciamento lato client e,
  conseguentemente, l'utilizzo "tradizionale" di GTM]{.underline}**

> E' vero che in teoria in un tracciamento server side potrebbe essere
> eliminato completamente l'utilizzo di GTM lato client ma questo
> richiederebbe l'implementazione lato codice, da parte degli
> sviluppatori del sito, di tute le chiamate dirette al contenitore GTM
> server side (che resta invece una parte imprescindibile di tutto il
> sistema) anziché effettuare semplici push di dati nel data leyer
>
> Nella realtà dei fatti però, vuoi per il fatto di lasciare libertà di
> gestione a chi si occupa di marketing e analisi dati, vuoi per il
> fatto che in certi casi (vedi Hotjar) andrebbe praticamente
> reimplementata tutta la gestione del sistema di tracciamento, vuoi
> ancora per la scarsa disponibilità di vendor in grado di gestire
> endpoint server side, l'utilizzo di GTM "tradizionale" come strumento
> di raccolta dati lato client resta ancora la soluzione migliore

- **[Non è la soluzione definitiva ai problemi e alle norme imposte dal
  GDPR]{.underline}**

> Sicuramente l'utilizzo di un sistema di tracciamento server side, con
> la possibilità di utilizzare server collocati in Europa, di poter
> decidere esattamente quali dati inviare o meno ai server di analytics,
> con il fatto di avere il controllo dei cookie effettivamente
> installati sul browser degli utenti ... aiuta notevolmente ad
> aumentare la privacy e la sicurezza degli utenti del nostro sito,
> avvicinandosi molto a tutto quanto effettivamente richiesto dal GDRP.
>
> Allo stato attuale però ci sono ancora alcuni aspetti (non ultimo
> quello relativo al fatto che il server intermedio su cui installare
> GTM faccia comunque uso di servizi offerti da società in qualche modo
> controllate da aziende con sede in USA) no perfettamente chiari che
> non possono permetterci di affermare al 100% che il tracciamento
> server side sia al 100% GDPR Compliance

