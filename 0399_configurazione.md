# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_lista_regalo_res.bmp](./assets/media/image220.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Caricamento Javascript**: se selezionato, consente di caricare il
  relativo componente in maniera asincrona al termine del caricamento
  della pagina web.

> **ATTENZIONE!** Per maggiori informazioni relativamente al parametro
> **Caricamento Javascript** si veda anche quanto indicato all'interno
> del capitolo "*Configurazione Componenti -- Caratteristiche generali*
> -- *Staticizzazione e caricamento asincrono*" di questo manuale

- **Tipologia di visualizzazione:** consente di definire la tipologia di
  visualizzazione della Lista Regalo. E' possibile selezionare uno dei
  seguenti valori:

  - **Griglia:** selezionando questa opzioni gli articoli presenti nella
    Lista Regalo verranno visualizzati all'interno di una griglia
    paginata perfettamente responsiva e organizzata su di un certo
    numero di righe e di colonne impostabili mediante i successivi
    parametri presenti all'interno di questa stessa maschera di
    configurazione

  - **Slider:** selezionando questa opzione gli articoli presenti nella
    Lista Regalo verranno disposti su di un\'unica riga all'interno di
    uno slider a scorrimento orizzontale.

- **Numero massimo di slide caricabili (solo per configurazioni di tipo
  Slider):** consente di impostare il numero massimo di slide che
  dovranno essere caricate all'interno del componente.

> **ATTENZIONE! Un numero troppo elevato di slide potrebbe rallentare il
> caricamento del componente**

- **Numero di Righe da Visualizzare (solo per configurazioni di tipo
  griglia):** consente di impostare il numero di righe della griglia di
  visualizzazione della Lista Regalo. **Sono accettati solo valori
  minori o uguali a 30**

> Nel momento in cui l'esigenza dovesse essere quella di visualizzare un
> numero di righe superiore a 30, si consiglia quindi di utilizzare una
> paginazione di tipo "Scroll infinito (Lazy loading)"
>
> **ATTENZIONE!** Nel caso in cui per la Lista Regalo sia stata
> impostata come tipologia di visualizzazione "Slider", gli articoli
> verranno disposti sempre e soltanto su di un\'unica riga

- **Numero di Articoli da visualizzare:** consente di impostare il
  numero di articoli per riga.

> In relazione a questo parametro vanno fatte poi alcune considerazioni
> di fondamentale importanza legate al comportamento responsivo del
> componente.
>
> In particolare dunque è bene ricordare che:

- Nel caso in cui per la Lista Regalo sia stata impostata come tipologia
  di visualizzazione "Griglia", indipendentemente dal numero di articoli
  che si è scelto di visualizzare all'interno di ogni singola riga, per
  risoluzioni **inferiori ai 992 px** verranno sempre visualizzati 2
  articoli per riga.

> Analogamente per risoluzioni **inferiori a 768 px** la griglia si
> linearizzerà mostrando un articolo per ogni riga

- Nel caso in cui per la Lista Articoli sia stata impostata come
  tipologia di visualizzazione "Slider", indipendentemente dal numero di
  articoli che si è scelto di visualizzare all'interno della singola
  riga, per risoluzioni **inferiori ai 992 px** lo slider mostrerà
  sempre e soltanto un solo articolo alla volta

<!-- -->

- **Posizione bottoni Slider (solo per configurazioni di tipo Slider):**
  consente di decidere, selezionando una delle possibili combinazioni
  presenti all'interno del corrispondente menu a tendina, dove dovranno
  essere collocati i pulsanti di scorrimento dello slider.

- **Visualizzazione Paginazione (solo per configurazioni di tipo
  griglia):** consente di decidere se e dove visualizzare (rispetto al
  Componente stesso) i controlli di paginazione.

- **Numero di Pagine (solo per configurazioni di tipo griglia):**
  consente di impostare, selezionandolo dal relativo menu a tendina, il
  numero di pagine che dovranno essere visualizzate nei controlli di
  paginazione. Ovviamente oltre al numero indicato all'interno di questo
  campo nei controlli di paginazione saranno sempre visibili anche la
  prima e l'ultima pagina disponibili.

> **Questo campo viene visualizzato solo nel caso in cui il parametro
> "Visualizza Paginazione" sia stato impostato su di un valore diverso
> da "Non Visualizzare".**

- **Paginazione con Precedente e Successivo (solo per configurazioni di
  tipo griglia):** se selezionato, nei controlli di paginazione,
  verranno visualizzati anche i pulsanti "Precedente" e "Successivo".

> Il testo di questi pulsanti è modificabile alla sezione \"Gestione
> Testi/Messaggi del Sito\" e agendo sull\'elemento generico
> \"Paginazione\".
>
> **Questo campo viene visualizzato solo nel caso in cui il parametro
> "Visualizza Paginazione" sia stato impostato su di un valore diverso
> da "Non Visualizzare".**

- **Tipo di Paginazione per dispositivi desktop (**\>= **992px) (solo
  per configurazioni di tipo griglia):** consente di definire il tipo di
  paginazione da utilizzare, per il componente in oggetto, su
  dispositivi desktop (risoluzione maggiore o uguale a 992px)

> E' possibile selezionare uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scroll bar per visualizzare i
  risultati presenti all'interno della nuova pagina)

- **A richiesta:** selezionando questa tipologia di paginazione verrà
  visualizzato sopra e/o sotto il componente (dipendentemente da come è
  stato impostato il precedente parametro "Visualizza Paginazione") un
  pulsante "**Mostra Altri Risultati**" che l'utente dovrà utilizzare
  per richiedere la visualizzazione degli articoli presenti nelle pagine
  successive.

- **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
  paginazione gli articoli distribuiti all'interno delle varie pagine,
  verranno visualizzati automaticamente mano a mano che l'utente
  scorrerà la pagina web verso il basso

<!-- -->

- **Tipo di Paginazione per dispositivi mobile (\<** **992px) (solo per
  configurazioni di tipo griglia):** consente di definire il tipo di
  paginazione da utilizzare, per il componente in oggetto, su
  dispositivi mobile (risoluzione minore a 992px). E' possibile
  selezionare uno dei seguenti valori:

  - **A richiesta:** selezionando questa tipologia di paginazione verrà
    visualizzato sopra e/o sotto il componente (dipendentemente da come
    è stato impostato il precedente parametro "Visualizza Paginazione")
    un pulsante "**Mostra Altri Risultati**" che l'utente dovrà
    utilizzare per richiedere la visualizzazione degli articoli presenti
    nelle successive pagine del catalogo.

  - **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
    paginazione gli articoli distribuiti all'interno delle varie pagine,
    verranno visualizzati automaticamente mano a mano che l'utente
    scorrerà la pagina web verso l'alto

  - **Come paginazione desktop:** selezionando questa opzione verrà
    applicata, anche per dispositivi con risoluzione minore a 992px lo
    stesso tipo di paginazione impostata per dispositivi "Desktop"

- **Elementi per pagina (solo per configurazioni di tipo griglia):**
  consente di indicare una lista di valori, sperati da virgole,
  corrispondenti al numero di elementi che potranno essere visualizzati
  in ogni singola pagina del componente. Gli unici caratteri ammessi
  all'interno di questo campo sono quelli numerici (0-9) e la virgola
  che dovrà essere utilizzata come carattere separatore.

> Nel momento in cui questo campo dovesse essere valorizzato in maniera
> corretta, sul sito verrà poi visualizzato un menu a tendina contenente
> l'elenco dei valori immessi.
>
> Selezionando uno dei valori presenti in elenco il componente verrà
> ricaricato e popolato con il numero di articoli per pagina indicati
> dall'utente.
>
> **ATTENZIONE! Modificando il numero di articoli per pagina il
> componente ripartirà sempre dalla prima pagina**

- **Visualizzazione Risultati:** se selezionato, consentirà di
  visualizzare, nella parte bassa del componente, una stringa di testo
  contenente il numero complessivo degli articoli presenti nella Lista
  Regalo.

- **Visualizza Ordinamento:** se selezionato, consentirà di
  visualizzare, lato sito, una combo box contenente l'elenco degli
  elementi sulla base dei quali poter effettuare l'ordinamento degli
  articoli presenti all'interno del componente.

> **ATTENZIONE! Nel caso in cui si decida di non selezionare questo
> parametro sarà comunque necessario agire dalla sezione "Gestione Campi
> di Ordinamento" per impostare, sul componente, un ordinamento di
> default.**
>
> Per maggiori informazioni in merito all'ordinamento degli articoli
> presenti in catalogo si veda anche il successivo capitolo di questo
> manuale.

- **Identificatore**: consente di stabilire se l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, dovranno essere applicati a livello di pagina oppure
  a livello di singolo componente. E' possibile selezionare uno dei
  seguenti valori:

  - **Pagina:** selezionando questa opzione l'ordinamento, la
    paginazione e gli elementi per pagina impostati dall'utente lato
    front end, mediante gli appositi controlli, verranno applicati a
    livello di pagina.

> Ciò significa dunque che, nel caso in cui all'interno della pagina
> dovessero essere presenti due o più componenti dello stesso tipo le
> impostazioni settate, su uno di questi componenti per l'ordinamento,
> la paginazione e gli elementi per pagina, avranno effetto anche sugli
> altri.
>
> **Tale opzione risulta particolarmente utile nel momento in cui, ad
> esempio, si dovessero utilizzare, all'interno di un componente Tab,
> due distinti componenti "Lista Regalo" realizzati con layout grafici
> diversi per ottenere ad esempio il classico passaggio dalla
> visualizzazione a griglia a quello a lista**
>
> In queste condizioni avendo impostato come "Identificatore" l'intera
> pagina saremo sicuri che nel momento in cui un utente dovesse
> ordinare, ad esempio, la Lista Regalo con visualizzazione a griglia in
> un certo modo, tale ordinamento verrà poi mantenuto anche nel
> passaggio alla visualizzazione a lista (e la stessa cosa vale anche
> per la paginazione e per gli elementi per pagina).

- **Nome Componente:** selezionando questa opzione l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, mediante gli appositi controllo verranno applicati
  solo ed esclusivamente al componente indicato

<!-- -->

- **Posizionamento barra controlli superiore:** consente di stabilire,
  selezionando la relativa combinazione da un apposito menu a tendina,
  l'ordine di posizionamento degli elementi principali presenti nella
  barra dei controlli posta immediatamente al di sopra del componente.

> In questo senso gli elementi ordinabili sono: "Elementi per pagina",
> "Ordinamento", "Paginazione"
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato**

- **Posizionamento barra controlli inferiore:** consente di stabilire,
  selezionando la relativa combinazione da un apposito menu a tendina,
  l'ordine di posizionamento degli elementi principali presenti nella
  barra dei controlli posta immediatamente al di sotto del componente.

> In questo senso gli elementi ordinabili sono: "Risultati" e
> "Paginazione"
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato**

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, il
Componente **"**Lista Regalo**" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore.** Sarà infatti
possibile inserire al suo interno tutta una serie di campi che, per
poter esser gestiti liberamente, dovranno inevitabilmente esser trattati
a loro volta come Componenti autonomi editabili singolarmente.

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Lista Regalo" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente la propria Lista Regalo.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce:** contiene quei componenti necessari per
  abilitare e gestire determinate funzionalità (es. "Aggiunta al
  Carrello") oltre che, ovviamente per inserire e gestire all'interno
  del sito determinate informazioni prelevate direttamente dal
  gestionale.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al "Catalogo E-Commerce" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

L'inserimento di questi componenti all'interno del Catalogo E-Commerce
avviene utilizzando le solite tecniche di interazione con l'editor (Drag
and Drop o Point and Click) già esaminate all'interno di questo manuale
(per maggiori informazioni si rimanda allo specifico capitolo di questo
manuale).

In ogni caso, comunque, la Lista Regalo avrà, in ogni sua pagina, un
certo numero di celle (coincidente con quanto precedentemente impostato
in fase di configurazione del componente). **I vari componenti (siano
essi Componenti Comuni o Componenti E-Commerce) utilizzati per costruire
la propria Lista Regalo potranno essere inseriti indistintamente
all'interno di una qualsiasi di queste celle (penserà poi l'applicazione
a ripeterli, in maniera completamente automatica all'interno di tutte le
celle presenti in Lista)**

