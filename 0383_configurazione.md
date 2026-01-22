# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image176.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**ATTENZIONE!** Per maggiori informazioni relativamente al parametro
**Caricamento Javascript** si veda anche quanto indicato all'interno del
capitolo "*Configurazione Componenti -- Caratteristiche generali* --
*Staticizzazione e caricamento asincrono*" di questo manuale

**Tipo di paginazione:** consente di definire la tipologia del
contenitore degli articoli che dovrà essere pubblicato all'interno del
sito.

E' possibile selezionare uno dei seguenti valori:

- **Slider:** selezionando questa opzione gli articoli presenti
  all'interno del componente verranno disposti tutti su di un\'unica
  riga all'interno di uno slider a scorrimento orizzontale.

![](./assets/media/image177.png)

- **Senza caricamento della pagina:** selezionando questa opzioni gli
  articoli presenti all'interno del componente verranno visualizzati in
  una griglia paginata perfettamente responsiva e organizzata su di un
  certo numero di righe e di colonne impostabili mediante i successivi
  parametri presenti all'interno di questa stessa maschera di
  configurazione. Inoltre ad ogni cambio pagina verrà ricaricato solo lo
  specifico componente

- **Con caricamento della pagina:** selezionando questa opzioni gli
  articoli presenti all'interno del componente verranno visualizzati in
  una griglia paginata perfettamente responsiva e organizzata su di un
  certo numero di righe e di colonne impostabili mediante i successivi
  parametri presenti all'interno di questa stessa maschera di
  configurazione. In queste condizioni inoltre ad ogni cambio pagina
  verrà ricaricata l'intera pagina web.

**Numero di Righe da Visualizzare (solo per visualizzazioni a
griglia):** consente di impostare il numero di righe della griglia di
visualizzazione degli articoli. **Sono accettati solo valori minori o
uguali a 30**

Nel momento in cui l'esigenza dovesse essere quella di visualizzare un
numero di righe superiore a 30, si consiglia quindi di utilizzare una
paginazione di tipo "Scroll infinito (Lazy loading)"

**ATTENZIONE!** Nel caso in cui per il componente in oggetto sia stata
impostata come tipologia di visualizzazione lo Slider, gli articoli
verranno disposti sempre e soltanto su di un\'unica riga

**Numero di Articoli da visualizzare (solo per visualizzazioni a
griglia):** consente di impostare il numero di articoli per riga.

In relazione a questo parametro vanno fatte poi alcune considerazioni di
fondamentale importanza legate al comportamento responsivo del
componente.

In particolare dunque è bene ricordare che:

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  la griglia, indipendentemente dal numero di articoli che si è scelto
  di visualizzare all'interno di ogni singola riga, per risoluzioni
  **inferiori ai 992 px** verranno sempre visualizzati 2 articoli per
  riga.

Analogamente per risoluzioni **inferiori a 768 px** la griglia si
linearizzerà mostrando un articolo per ogni riga

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  lo slider per risoluzioni **inferiori ai 992 px** questo mostrerà
  sempre e soltanto un solo articolo alla volta

**Posizione bottoni Slider (solo per visualizzazioni a slider):**
consente di decidere, selezionando una delle possibili combinazioni
presenti all'interno del corrispondente menu a tendina, dove dovranno
essere collocati i pulsanti di scorrimento dello slider.

**Visualizzazione Paginazione (solo per visualizzazioni a griglia):**
consente di decidere se e dove visualizzare (rispetto al Componente
stesso) i collegamenti alle varie pagine del catalogo.

**Numero di Pagine (solo per visualizzazioni a griglia):** consente di
impostare, selezionandolo dal relativo menu a tendina, il numero di
pagine che dovranno essere visualizzate nei controlli di paginazione.
Ovviamente oltre al numero indicato all'interno di questo campo nei
controlli di paginazione saranno sempre visibili anche la prima e
l'ultima pagina disponibili.

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Paginazione con Precedente e Successivo (solo per componenti a
griglia):** se selezionato, nei controlli di paginazione, verranno
visualizzati anche i pulsanti "Precedente" e "Successivo".

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Visualizzazione Risultati:** se selezionato, consentirà di
visualizzare, nella parte bassa del componente, una stringa di testo
contenente il numero complessivo degli articoli presenti all'interno del
componente stesso.

La sezione **"Gestione Campi di Ordinamento"** consente, infine, di
impostare il criterio di ordinamento per gli articoli presenti
all'interno del componente.

![](./assets/media/image13.png)

All'interno di questa sezione, sulla sinistra sono elencati gli elementi
di ordinamento attualmente codificati, sulla destra sono invece
riportate le proprietà dell'elemento attualmente selezionato in elenco.
Per modificare uno di questi elementi sarà quindi sufficiente
selezionarlo e agire poi sui parametri presenti all'interno della
sezione "**Modifica Campo Ordinamento**".

Allo stesso modo per codificare un nuovo elemento sarà necessario
cliccare sull'icona raffigurante un piccolo + (
![](./assets/media/image14.png) ) e definire poi le proprietà
dell'elemento stesso.

In particolare per ogni singolo elemento di ordinamento occorrerà
specificare un valore per i seguenti campi:

**Testo:** etichetta identificativa dell'elemento di ordinamento che si
sta codificando.

**Tipo di ordinamento:** consente di specificare il campo sulla base del
quale dovranno essere ordinati gli articoli presenti all'interno del
componente.

E' possibile indicare una delle seguenti opzioni:

- **Campo Articolo:** selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Campo di
  Ordinamento**") lo specifico campo del gestionale che dovrà essere
  utilizzato per definire l'ordinamento degli articoli. E' possibile
  selezionare una delle seguenti opzioni:

  - **Titolo:** l'ordinamento verrà determinato sulla base del campo
    "**Descrizione**" presente all'interno dell'Anagrafica Articoli del
    gestionale.

  - **Codice:** l'ordinamento verrà determinato sulla base del campo
    "**Codice**" presente all'interno dell'Anagrafica Articoli del
    gestionale.

  - **Codice Alternativo (solo Ecommerce Mexal):** l'ordinamento verrà
    determinato sulla base del campo "Codice Alternativo"
    dell'Anagrafica Articoli di Mexal

  - **Descrizione:** l'ordinamento verrà determinato sulla base del
    campo **Descrizione** presente all'interno della maschera "Modifica
    Articolo" accessibile, in Passweb, dalla voce di menu *"Catalogo --
    Gestione Articoli"* dopo aver selezionato, ovviamente, uno specifico
    articolo ed aver cliccato sul pulsante "Modifica Articolo"

  - **Codice Categoria Statistica Articolo:** l'ordinamento verrà
    determinato sulla base del codice della Categoria Statistica di
    appartenenza degli articoli presenti all'interno del componente.

  - **Descrizione Categoria Statistica Articolo:** l'ordinamento verrà
    determinato sulla base della descrizione della Categoria Statistica
    di appartenenza degli articoli presenti all'interno del componente

  - **Codice Categoria Merceologica:** l'ordinamento verrà determinato
    sulla base del codice della Categoria Merceologica degli articoli
    presenti all'interno del componente

  - **Descrizione Categoria Merceologica:** l'ordinamento verrà
    determinato sulla base della descrizione della Categoria
    Merceologica degli articoli presenti all'interno del componente

  - **Codice Natura (solo Ecommerce Mexal):** l'ordinamento verrà
    determinato sulla base del codice della Natura associata in Mexal
    agli articoli presenti all'interno del componente

  - **Descrizione Natura (solo Ecommerce Mexal):** l'ordinamento verrà
    determinato sulla base della descrizione della Natura associata in
    Mexal agli articoli presenti all'interno del componente.

  - **Data di Creazione:** l'ordinamento verrà determinato sulla base
    della data di creazione degli articoli presenti all'interno del
    componente.

> **ATTENZIONE!** Per "**Data di creazione**" si intende la data in cui
> l'articolo è stato inserito per la prima volta nel database del sito

- **Disponibilità:** l'ordinamento verrà determinato sulla base del
  valore della disponibilità degli articoli presenti all'interno del
  componente.

> **ATTENZIONE!** Il valore della disponibilità è sempre quello
> aggiornato all'ultima sincronizzazione utile (e potrebbe quindi non
> coincidere con l'effettiva disponibilità degli articoli). La formula
> secondo cui determinare tale valore è invece quella indicata
> all'interno del relativo campo della maschera **"Catalogo
> Mexal/Ho.Re.Ca"**

- **Listino:** l'ordinamento verrà determinato sulla base dei prezzi
  definiti, per i vari articoli, nel listino utilizzato per l'utente che
  sta navigando il sito.

> **ATTENZIONE: una volta impostato l'ordinamento dunque, ogni articolo
> verrà posizionato in base al suo effettivo prezzo di listino e non
> verrà quindi considerata nessun tipo di particolarità e/o scontistica
> definita all'interno del gestionale o in fase di configurazione del
> sito stesso.**
>
> [Nel caso infatti di particolarità prezzo e/o sconto il prezzo
> effettivo degli articoli non è memorizzato nel database di Passweb ma
> viene calcolato in tempo reale sulla base delle condizioni commerciali
> definite per lo specifico articolo e/o per lo specifico utente che sta
> navigando il sito]{.underline}.
>
> **Nel caso in cui si dovesse quindi decidere di utilizzare un
> ordinamento per prezzo e, allo stesso tempo, anche delle particolarità
> prezzo e/o sconto, una volta impostato l'ordinamento gli articoli
> soggetti a particolarità potrebbero non soddisfare i criteri di
> ordinamento effettivamente impostati.**
>
> **Allo stesso modo anche gli articoli con "Prezzo a Richiesta**"
> **verranno posizionati, in fase di ordinamento, sulla base del loro
> effettivo prezzo di listino**
>
> **ATTENZIONE! Impostando questo tipo di ordinamento per la prima
> volta, sarà necessario effettuare una sincronizzazione totale in modo
> tale da aggiornare il database del sito con i prezzi di listino
> corretti.**

- **Attributo Articolo:** selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Attributo di
  Ordinamento**") l'Attributo Articolo (sia esso di tipo Passweb, sia
  esso di tipo Mexal) che dovrà essere utilizzato per definire
  l'ordinamento degli articoli. E' possibile selezionare uno qualsiasi
  degli Attributi Articolo precedentemente codificati all'interno della
  corrispondente sezione del Wizard.

- **Casuale:** impostando questo valore l'ordine di visualizzazioni
  degli articoli presenti all'interno del componente sarà casuale. Tale
  ordinamento, stabilito ad una prima vista della pagina che ospita il
  componente in oggetto, verrà poi mantenuto per tutta la durata della
  sessione (compreso un tempo di inattività fissato a 20 minuti).
  Esaurito questo intervallo di tempo successive visite alla pagina
  contenente il componente determineranno un nuovo ordinamento casuale.

- **Articoli più visti:** selezionando questo valore gli articoli
  presenti all'interno del componente verranno ordinati sulla base della
  loro popolarità.

> **ATTENZIONE!** **il criterio di popolarità utilizzato per ordinare
> gli articoli all'interno del componente è determinato da quello che è
> il numero di visite ricevute dalle relative pagine prodotto**.
>
> In questo caso sarà anche possibile impostare, mediante il successivo
> campo **"Periodo (giorni)"**, il numero esatto di giorni che dovranno
> essere considerati per valutare gli articoli più popolari.
>
> E' quindi possibile ordinare gli articoli presenti all'interno del
> componente in base a quelli che sono, ad esempio, i più visti
> dell'ultima settimana

- **Articoli più venduti:** selezionando questo valore gli articoli
  presenti all'interno del componente verranno ordinati in base a quelli
  che risultano essere i più venduti

> **ATTENZIONE! gli articoli più acquistati sono determinati solo ed
> esclusivamente sulla base degli ordini attualmente presenti in Passweb
> e del numero di volte in cui uno stesso articolo compare all'interno
> di questi stessi ordini.**
>
> Come per il parametro precedente anche in questo caso il successivo
> campo **"Periodo (giorni)"**, consente di indicare il numero esatto di
> giorni che dovranno essere considerati per valutare gli articoli più
> acquistati.
>
> E' quindi possibile ordinare gli articoli presenti all'interno del
> componente in base a quelli che sono, ad esempio, i più venduti
> dell'ultima settimana.

**Modo di Ordinamento:** consente di specificare se, in relazione
all'elemento che si sta codificando, dovrà essere applicato un
ordinamento di tipo Crescente o Decrescente. Tale campo non sarà
ovviamente presente nel caso in cui sia stato impostato un ordinamento
di tipo Casuale.

**Default:** se selezionato, il corrispondente elemento verrà
considerato come quello sulla base del quale ordinare gli articoli
presenti all'interno del componente.

**ATTENZIONE! Per il componente "Selezione Regalo" verrà considerato
solo ed esclusivamente l'ordinamento di default**

Ciò significa dunque che, a differenza di quanto avviene per componenti
quali "Catalogo Ecommerce", "Offerte/Novità" , "Popolarità Prodotto"
ecc.., per il componente "Selezione Regalo" non è possibile abilitare
sul front end del sito un menu a tendina mediante il quale consentire
agli utenti di selezionare diversi criteri di ordinamento.

**Gli articoli presenti all'interno di questo componente saranno quindi
ordinati sempre e soltanto sulla base di quello che è stato definito, in
fase di configurazione del componente stesso, l'ordinamento di
default.**

Infine va anche ricordato che i campi sulla base dei quali poter
stabilire l'ordine di visualizzazione degli articoli presenti
all'interno del componente saranno sempre considerati come testuali. In
conseguenza di ciò, un articolo con il campo di ordinamento impostato,
ad esempio sul valore 10, verrà visualizzato nel caso di ordinamento
Crescente (Decrescente) prima (dopo) di un articolo con il campo di
ordinamento impostato sul valore 2.

Per quel che riguarda la logica di gestione del suo contenuto, il
Componente **"**Selezione Regalo**" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore.** Sarà quindi possibile
inserire al suo interno tutta una serie di campi necessari per poter
definire che tipo di informazioni gestionali e non, dovranno essere
visualizzate per ogni singolo articolo. Tali campi, in ogni caso, per
poter esser gestiti liberamente, dovranno inevitabilmente esser trattati
a loro volta come Componenti autonomi editabili singolarmente..

Una volta inserito quindi il Componente all'interno della pagina per
poterlo poi personalizzare a livello di contenuti sarà necessario,
attivare la modalità di gestione dei componenti, portarsi sul Componente
in esame e, alla comparsa del R.O.C. cliccare sull'icona **Accedi ai
componenti interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Selezione Regalo"
sarà possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce:** contiene tutti i componenti E-Commerce,
  ossia quei componenti necessari per abilitare e gestire determinate
  funzionalità (es. "Aggiunta al Carrello") oltre che, ovviamente, per
  poter definire che tipo di informazioni gestionali dovranno essere
  visualizzate per ogni singolo articolo.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Offerte/Novità" si veda
> la corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

L'inserimento di questi elementi all'interno del Componente "Selezione
Regalo" avviene utilizzando le solite tecniche di interazione con
l'editor (Drag and Drop o Point and Click) già esaminate all'interno di
questo manuale (per maggiori informazioni si rimanda allo specifico
capitolo di questo manuale).

