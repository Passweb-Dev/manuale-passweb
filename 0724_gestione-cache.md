# GESTIONE CACHE



All'interno di questa sezione è possibile gestire il modulo di cache
messo a disposizione da Passweb per ottimizzare le prestazioni del
proprio sito web.

**ATTENZIONE! per poter accedere a questa sezione è necessario aver
acquistato il corrispondente modulo presente all'interno di Passstore**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_cache_1.bmp](./assets/media/image259.png){width="5.850694444444445in"
height="3.863888888888889in"}

I parametri presenti all'interno della sezione "Generale" consentono
rispettivamente di:

**Abilitata**: consente di attivare / disattivare la cache del proprio
sito Passweb.

**ATTENZIONE!** di base la cache verrà attivata **per i soli utenti non
autenticati.**

Ciò significa, dunque, che nel momento in cui il parametro in esame
dovesse essere:

- **Attivato**: le pagine restituite agli utenti che non hanno ancora
  effettuato l'autenticazione al sito verranno prelevate, se presenti,
  direttamente dalla cache minimizzando quindi i tempi di caricamento.
  Nel caso in cui una determinata pagina non dovesse ancora essere
  presente in cache (perché non ancora visitata), alla prima visita
  utile verrà creata in maniera dinamica (con i relativi tempi di
  caricamento) e, contestualmente, il suo codice HTML verrà anche
  memorizzato nel server di cache per poter poi essere riutilizzato nel
  momento in cui un altro utente, sempre non autenticato, dovesse
  richiederlo visitando la stessa pagina.

> In queste condizioni inoltre le pagine restituite agli utenti
> autenticati non verranno mai cachate e saranno quindi costruire sempre
> e comunque in maniera dinamica.
>
> Nel momento in cui l'esigenza dovesse essere quella di attivare la
> cache anche per gli utenti autenticati sarà quindi necessario agire
> mediante il successivo parametro "**Cache per singolo utente**"

- **Disattivato**: le pagine restituite a tutti gli utenti del sito,
  autenticati e non, verranno costruite sempre e comunque in maniera
  dinamica effettuando quindi, ad ogni visita, tutte le query necessarie
  sul database del sito per ottenere i dati da mostrare all'utente

**Cache per singolo utente**: consente di attivare / disattivare la
**cache per gli utenti autenticati**

In particolare dunque, nel momento in cui il parametro in esame dovesse
essere:

- **Attivato:** le pagine restituite ad ogni utente autenticato verranno
  prelevate, se presenti, direttamente dalla cache, minimizzando quindi
  anche in questo caso i tempi di caricamento. Nel caso in cui una
  determinata pagina non dovesse essere presente in cache, perché non
  ancora **visitata da quello specifico utente**, alla prima vista utile
  verrà creata in maniera dinamica, effettuando tutte le query del caso
  sul database del sito e, contestualmente, verrà anche messa in cache
  per poter poi essere riutilizzata nel momento in cui **lo stesso
  utente** dovesse visitarla una seconda volta

- **Disattivato**: le pagine restituite ad ogni utente autenticato
  verranno costruite sempre e comunque in maniera dinamica effettuando
  quindi, ad ogni visita, tutte le query necessarie sul database del
  sito per ottenere i dati da mostrare all'utente

**ATTENZIONE!** l'attivazione del parametro in oggetto verrà
effettivamente considerata solo nel caso in cui sia stato attivato anche
il precedente parametro "**Abilitata**" che, di fatto, consente di
attivare il modulo di cache. In altri termini, dunque, non è possibile
attivare la cache per gli utenti autenticati senza prima aver attivato
anche quella per gli utenti non autenticati

**Filtro Articoli Crawler**: consente di impostare un filtro articoli
per identificare le pagine prodotto che dovranno essere visitate dal
Crawler Passweb utilizzabile per automatizzare la creazione **di un
massimo di 100 pagine** di cache senza dover quindi attendere che queste
stesse pagine vengano effettivamente visualizzate da utenti reali.

**ATTENZIONE!** ovviamente la cache creata in automatico dal Crawler
Passweb sarà utilizzabile dai soli utenti non autenticati

Per maggiori informazioni in merito al Crawler Passweb si rimanda a
quanto indicato nel successivo capitolo "*Crawler Passweb"* di questo
manuale

**Flush**: consente di definire il metodo da utilizzare per azzerare la
cache del proprio sito. E' possibile selezionare una delle seguenti
opzioni:

- **Automatico:** selezionando questa opzione il flush della cache verrà
  gestito in automatico dal programma

- **Manuale:** selezionando questa opzione il flush della cache dovrà
  poi essere gestito in maniera manuale dall'amministratore del sito
  cliccando sui relativi pulsanti presenti all'interno della pagina
  "Gestione Cache"

- **Temporizzato:** selezionando questa opzione il flush della cache
  verrà eseguito in maniera automatica ogni N minuti, dove il valore
  degli N minuti potrà essere indicato all'interno del successivo campo
  "**Durata in minuti**" (campo questo visualizzato solo nel caso in cui
  il parametro Flush sia stato impostato sul valore "Temporizzato")

Per maggiori informazioni relativamente alla diverse modalità di flush
della cache si rimanda a quando indicato nel successivo capitolo "*Flush
della cache*" di questo manuale

All'interno della sezione "**Tipologia di Cache**" sono indicate le
tipologie di cache gestite da Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tipologie_cache.bmp](./assets/media/image260.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

Come si può facilmente osservare, al momento, Passweb gestisce solamente
un cache di pagina che, se attivata, consentirà di salvare il codice
HTML dell'intera pagina web.

In realtà considerando che non tutti i componenti Passweb possono essere
cachati potranno anche verificarsi situazioni in cui verrà salvata in
cache solamente una porzione del codice HTML della pagina

L'icona raffigurante una piccola batteria presente all'interno della
colonna "**Variata**" consente invece di evidenziare se la
corrispondente tipologia di cache debba essere resettata (**batteria
piena e colorata di rosso**) o meno (**batteria vuota**)

I pulsanti presenti all'interno della sezione "**Gestione Cache**"
(molti dei quali visualizzati solo dopo aver confermato l'attivazione
della cache) consentono infine di:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsanti_gestione_cache.bmp](./assets/media/image261.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

**Evidenziatore** ( ): consente di evidenziare, all'interno del Live
Editing gli elementi che, in fase di visualizzazione della pagina,
verranno effettivamente prelevati dalla cache del sito.

Come già evidenziato infatti non tutti i componenti potranno essere
cachati (basta pensare al componente Carrello o al componente Checkout
che, per ovvie ragioni, dovranno essere sempre dei componenti dinamici)
e, volendo, si potrà decidere di rendere non cachabili anche quei
componenti che, di base invece, lo sono.

Cliccando su questo pulsante verrà aperta, in un nuovo tab del browser,
una versione "particolare" del front end del sito. Nella parte bassa,
sulla sinistra della pagina, verrà visualizzata un'icona raffigurante
una piccola puntina.

![Videate\\evidenziatore_cache.bmp](./assets/media/image262.png){width="5.850694444444445in"
height="3.8180555555555555in"}

Cliccando su quest'icona, verranno quindi evidenziati, con un riquadro
rosso, tutti i componenti presenti all'interno della pagina che sono
stati prelevati direttamente dalla cache del sito.

**Reset Cache** (
![Videate\\pulsante_reset_cache.bmp](./assets/media/image263.png){width="0.6625in"
height="0.2076388888888889in"} ): consente di effettuare il reset, e
quindi di azzerare, l'intera cache del sito. Lo stesso risultato si
otterrebbe anche effettuando il flush della cache di pagina mediante il
corrispondente pulsante ("**Flush Cache**"
![Videate\\pulsante_flush_cache.bmp](./assets/media/image264.png){width="0.6361111111111111in"
height="0.21458333333333332in"} ) presente all'interno della sezione
"Tipologie di Cache"

Per maggiori informazioni relativamente alle operazioni di flush della
cache si veda anche il successivo capitolo ("*Flush della Cache*") di
questo manuale.

**Avvia Crawler** ( ): consente di lanciare il **Crawler Passweb** che
andrà a scansionare le pagine prodotto (fino ad un massimo di 100)
risultanti dal filtro articoli impostato in corrispondenza del parametro
"Filtro Articoli Crawler" precedentemente analizzato in maniera tale da
mettere immediatamente in cache queste stesse pagine senza attendere che
vengano effettivamente visitate da utenti reali.

**ATTENZIONE!** La cache generata dal Crawler Passweb sarà fruibile solo
da utenti non autenticati.

Per maggiori informazioni in merito si veda anche quanto indicato
all'interno del successivo capitolo " *Crawler Passweb*".

**Log Crawler** (
![Videate\\pulsante_log_crawler.bmp](./assets/media/image265.png){width="0.6430555555555556in"
height="0.2076388888888889in"} ): consente di scaricare un file di log
contenente i dettagli relativi alle pagine visitate dal Crawler Passweb
durante l'ultima scansione del sito.

Dopo aver analizzato nel dettaglio i parametri di configurazione è bene
ora fare alcune considerazioni di fondamentale importanza in relazione a
come verrà effettivamente costruita e gestita la cache del sito.

Nello specifico è bene sottolineare che:

- Nel momento in cui si dovesse decidere di **gestire la cache solamente
  per gli utenti non autenticati** (parametro "Cache per singolo utente"
  disattivato) verrà creata e messa in cache, per ogni singola pagina
  del sito, una stessa versione che sarà poi quella restituita ad un
  qualsiasi utente che dovesse visitare quella stessa pagina senza aver
  ancora effettuato l'autenticazione.

> **ATTENZIONE!** In queste condizioni in realtà, potrebbero essere
> messe in cache anche versioni diverse della stessa pagina a seconda
> della nazione da cui arriva la visita. In ogni caso comunque per tutti
> gli utenti non autenticati in arrivo da una determinata nazione la
> pagina restituita dalla cache sarà sempre la stessa
>
> Una volta effettuata l'autenticazione invece i contenuti della pagina
> potrebbero cambiare e non solo rispetto a quelli che erano prima
> dell'autenticazione ma anche a seconda dello specifico utente che ha
> effettuato il login.
>
> In conseguenza di ciò nel momento in cui si dovesse decidere di
> **gestire la cache anche per gli utenti autenticati** (parametro
> "Cache per singolo utente" attivato) verranno salvate in cache più
> versioni della stessa pagina, una (o più) per gli utenti non
> autenticati e una per ogni utente autenticato che ha effettivamente
> visualizzato, almeno una volta, la pagina in questione

- La cache gestita da Passweb è, come detto, una cache di pagina per
  cui, di base, una volta attivata verrà messo in cache il codice HTML
  dell'intera pagina web. Ci sono però alcune eccezioni rispetto a
  quanto appena detto.

> Non tutti i componenti del sito possono infatti essere cachati. Basta
> pensare, in questo senso, a componenti come il Carrello o il Checkout
> il cui contenuto non potrà mai, per ovvie ragioni, essere staticizzato
> ma dovrà sempre essere costruito in maniera dinamica effettuando tutte
> le query del caso direttamente sul db del sito.
>
> Allo stesso modo alcuni componenti che nascono come cachabili,
> possono, volendo, essere resi non cachabili agendo per questo mediante
> il parametro "**Disabilita Cache**" presente nella loro maschera di
> configurazione (per maggiori informazioni in merito si rimanda a
> quanto indicato all'interno di questo manuale relativamente ai
> parametri di configurazione di ogni singolo componente)
>
> In conseguenza di ciò per le pagine che ospitano componenti non
> cachabili verrà salvata e messa in cache solamente una parte del loro
> codice HTML ottenendo quindi, a livello di prestazioni, una via di
> mezzo tra quello che si avrebbe staticizzando l'intera pagina e quello
> che si avrebbe invece costruendo l'intera pagina in maniera dinamica
> (cache disattiva)

- Un altro aspetto molto importante, derivante sempre dal fatto di
  utilizzare una cache di pagina, è quello che riguarda **l'utilizzo di
  componenti paginati (es. Catalogo Ecommerce)** **con la paginazione
  impostata in maniera asincrona** (parametro "Tipo di paginazione"
  impostato sulle opzioni "Senza il caricamento della pagina", "A
  richiesta" oppure "Scroll infinito")

> In questo senso infatti è bene sottolineare che, mettendo in cache il
> codice HTML dell'intera pagina web verrà salvata, la prima pagina di
> eventuali componenti paginati presenti al suo interno ma non le pagine
> successive che verranno invece caricate in maniera asincrona
> (attraverso apposite chiamate javascript).
>
> In altri termini dunque nel momento in cui l'utente dovesse decidere
> di interagire con il sito sfogliando il componente paginato, passando
> ad esempio dalla pagina 1 alla pagina 2, il contenuto della seconda
> pagina non verrà mai prelevato dalla cache ma verrà costruito sempre
> in maniera dinamica effettuando tutte le query necessarie direttamente
> sul db del sito (come avverrebbe anche nel caso di cache disattiva).
>
> In queste condizioni dunque il primo accesso alla pagina avverrà nella
> maniera più veloce possibile e le successive interazioni caricheranno
> in maniera dinamica solamente il contenuto delle specifico componente
> con cui è avvenuta l'interazione (non quello dell'intera pagina)
> riducendo quindi al minimo indispensabile le query necessarie per
> mostrare all'utente il contenuto che ha effettivamente richiesto
>
> Ovviamente questo discorso e questo modo di operare vale non solo per
> i componenti paginati ma anche per tutti quei componenti il cui
> contenuto potrebbe variare, rispetto a quello presente inizialmente
> nella pagina, a seguito di un'interazione da parte dell'utente.
> Pensiamo ad esempio al pulsante che consente di richiedere la
> disponibilità di un prodotto in tempo reale o, ancora,
> all'applicazione di un filtro di ricerca articoli.
>
> In quest'ultimo caso, in particolare, il contenuto di un componente
> come il Catalogo Ecommerce cui viene applicato un filtro articoli non
> sarà, ovviamente, lo stesso di quello mostrato al primo caricamento
> della pagina e, allo stesso modo, diventerebbe piuttosto complesso
> salvare in cache ogni singola ricerca effettuata da ogni singolo
> utente del sito, per cui, come per la paginazione, anche in questo
> caso all'applicazione del filtro verranno effettuate tutte le query
> necessarie sul db del sito per ottenere il risultato richiesto e
> quindi il contenuto dei (soli) componenti interessati dal filtro non
> verrà prelevato dalla cache ma verrà costruito in maniera dinamica

- Un discorso leggermente diverso rispetto a quanto indicato al punto
  precedente è quello che riguarda il caso in cui, a cache attiva, si
  dovesse decidere di stampare comunque, all'interno delle pagine
  prodotto, la disponibilità dell'articolo aggiornata all'ultima
  sincronizzazione.

> In queste condizioni quando verrà effettuato un ordine all'interno del
> sito, e questo stesso ordine verrà inserito immediatamente all'interno
> del gestionale, variando di conseguenza i progressivi dell'articolo,
> il valore della disponibilità stampato nella pagina prodotto (che come
> sottolineato è stata inserita in cache) non potrà essere aggiornato e
> non sarà più, quindi, quello corretto.
>
> Il problema dovrebbe quindi essere risolto facendo in modo che, a
> seguito della sincronizzazione parziale che ha inserito l'ordine
> all'interno del gestionale, venisse anche resettata la cache in
> maniera tale da poter ricostruire la pagina prodotto con il corretto
> valore della disponibilità. Considerando però la frequenza con cui
> potrebbero essere effettuati ordini all'interno del sito, come è
> semplice comprendere, questo modo di operare renderebbe di fatto
> inutile l'utilizzo della cache che non avrebbe mai il tempo utile per
> potersi costruire.
>
> Quello che farà Passweb in queste condizioni, posto di aver impostato
> il flush della cache sull'opzione "Automatico", sarà andare a
> valutare, prima di resettare la cache, se la variazione della
> disponibilità di un articolo a seguito dell'acquisizione di un ordine
> è stata o meno una variazione sensibile, dove per sensibile si intende
> che l'articolo è passato da disponibile a non disponibile.
>
> In maniera più precisa dunque se, a seguito dell'acquisizione di un
> ordine almeno uno degli articoli coinvolti dovesse passare da
> disponibile a non disponibile, verrà effettuato il reset della cache
> in maniera tale che alla successiva vista della pagina gli utenti
> possano vedere che quello specifico articolo non è più disponibile.
>
> In caso contrario invece, se la variazione della disponibilità degli
> articoli coinvolti nell'ordine dovesse essere tale da mantenerli
> comunque disponibili e quindi ancora acquistabili, non verrà
> effettuato alcun reset.
>
> Questo da una parte farà si che il valore della disponibilità stampato
> all'interno della pagina prodotto non sia effettivamente quello
> corretto ma dall'altra parte, evitando il reset, darà alla cache il
> tempo di costruirsi rendendo quindi i suoi effetti, in termini di
> prestazioni, più evidenti.
>
> Resterebbe, è vero, il problema del valore della disponibilità
> stampato all'interno della pagina che non è esattamente quello più
> aggiornato, ma questo problema potrebbe essere facilmente aggirato
> utilizzando anziché il numero esatto il classico semaforo (verde /
> rosso) oppure inserendo il testo che indica la data di ultimo
> aggiornamento del valore mostrato e il pulsante per richiedere il
> valore corretto in tempo reale.

- L'ordinamento casuale, impostabile su determinati componenti è
  ovviamente incompatibile con la possibilità di mettere in cache quegli
  stessi componenti. Ordinamento casuale significa infatti che ad ogni
  caricamento della pagina il contenuto mostrato da questi componenti
  dovrà essere differente e questo rende chiaramente impossibile, per
  questi componenti, memorizzare in cache un codice HTML univoco da
  restituire ad ogni vista della pagina.

> In sostanza dunque, impostando per un determinato componente un
> ordinamento casuale questo stesso componente non verrà mai cachato
> indipendentemente dal fatto di aver attivato o meno in fase di
> configurazione il suo parametro "Disabilita Cache"

- Per quel che riguarda i componenti innestati a più livelli il fatto di
  poter impostare o meno i componenti interni, di livello maggiore di 1,
  come cachabili dipende non solo dalla presenza del parametro
  "Disabilita Cache" nella loro maschera di configurazione, ma anche
  dalle specifiche caratteristiche del componente stesso.

> Ad esempio, i componenti Ecommerce, Interazione Utente e CMS di
> secondo livello, quelli, tanto per intenderci, come il "Titolo
> Articolo" che può essere inserito all'interno di un Catalogo
> Ecommerce, il "Sommario CMS" che può essere inserito all'interno di un
> "Archivio CMS", i campi Form che possono essere inserti all'interno di
> componenti di primo livello come il "Form di Registrazione Utente"
> ecc... non avranno nella loro maschera di configurazione il parametro
> "Disabilita Cache" e quindi il fatto di inserirli o meno in cache
> dipenderà sempre da quelle che sono le impostazioni settate per il
> loro componente padre.
>
> In sostanza dunque non sarà mai possibile impostare come cachabile, ad
> esempio, il Catalogo Ecommerce e allo stesso tempo impostare invece
> come non cachabili il Titolo o il Prezzo degli articoli inseriti
> all'interno del catalogo stesso.
>
> Per maggiori informazioni in merito si rimanda a quanto indicato,
> all'interno di questo manuale, relativamente alla configurazione di
> ogni singolo componente

- Ovviamente nel momento in cui, una volta attivata la cache, dovesse
  essere effettuata una qualsiasi modifica a un componente o ad un
  qualche parametro di configurazione del sito, e tale modifica dovesse
  comportare la variazione del codice HTML di una o più pagine web
  (pensiamo ad esempio al cambiamento della modalità di visualizzazione
  di una struttura, della modalità di visualizzazione del controllo di
  selezione delle taglie, ad una possibile variazione da apportare alle
  categorie secondarie associate ad un determinato articolo ...),
  affinché questa variazione possa essere correttamente visualizzata
  dagli utenti del sito, sarà necessario effettuare un reset della cache
  in maniera tale che le pagine interessate possano, alla prima visita
  utile, ricreare il codice HTML corretto da mettere nuovamente in
  cache.

> **ATTENZIONE!** a seguito di una modifica che dovesse richiedere il
> reset della cache per garantire la corretta visualizzazione dei
> contenuti sul front end del sito, Passweb segnalerà tale esigenza
> all'interno del Wizard mostrando l'icona di una piccola batteria
> rossa, sia all'interno della pagina di gestione della cache sia nella
> parte alta del menu di navigazione.

![Videate\\gestione_cache_6.bmp](./assets/media/image266.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

![Videate\\gestione_cache_7.bmp](./assets/media/image267.png){width="5.746527777777778in"
height="3.5194444444444444in"}

**ATTENZIONE!** **Per ovvie ragioni, in fase di sviluppo del sito, è
consigliabile NON abilitare la cache (indipendentemente dalla tipologia
considerata)**

**Allo stesso modo occorre considerare anche che in Live Editing così
come nella visualizzazione del sito a partire dal Wizard tramite il
pulsante "Accedi Sito" non verrà mai gestita nessun tipo di cache.**

