# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![Videate\\ricerca_ecommerce0_res.bmp](./assets/media/image25.png)

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

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Tipo:** consente di indicare la tipologia del pannello di ricerca che
si sta realizzando specificando quindi anche la funzione che tale
pannello dovrà espletare. Nel caso specifico tale parametro dovrà
ovviamente essere impostato sul valore **"Ricerca E-commerce"**

> **NOTA BENE:** una volta impostata la tipologia del pannello di
> ricerca che si intende realizzare e confermato il componente, tale
> tipologia non potrà più essere modificata.

**Identificatore:** consente di legare tra loro due o più pannelli di
ricerca in maniera tale da poterli poi gestire come se fossero il
medesimo pannello.

Il campo è **numerico** ed opzionale per cui andrà valorizzato solo ed
esclusivamente nel momento in cui sia effettivamente necessario legare
tra loro due o più pannelli distinti.

Supponiamo, ad esempio, di dover fare in modo che i filtri impostati in
un pannello di ricerca presente nella Home Page del sito siano mantenuti
anche all'interno di un altro pannello di ricerca, collocato, ad
esempio, in una diversa posizione della pagina Catalogo.

Considerando che i due pannelli di ricerca sono due distinti componenti
Passweb, e **NON** lo stesso componente distribuito sulle due diverse
pagine, l'unica possibilità che avremo per soddisfare questa esigenza
sarà quella di impostare il campo "Identificatore" di entrambi i
pannelli sullo stesso valore numerico (es. 1).

**Ovviamente il pannello di ricerca in Home Page dovrà essere
configurato in maniera tale che la sua destinazione sia la pagina
Catalogo, mentre il pannello di ricerca presente all'interno della
pagina Catalogo dovrà essere configurato per restare in questa stessa
pagina**

In queste condizioni nel momento in cui un utente del sito dovesse
effettuare una ricerca partendo dal pannello presente in Home Page verrà
poi ricondotto alla pagina Catalogo dove, oltre a visualizzare il
risultato della ricerca effettuata, si ritroverà anche, nel pannello di
ricerca presente in questa pagina gli stessi valori del filtro impostato
nel pannello della Home Page

**ATTENZIONE!** Ovviamente affinchè il pannello di ricerca presente
nella pagina di applicazione del filtro mantenga gli stessi valori
impostati nel pannello di ricerca di partenza, è necessario che il campo
utilizzato per impostare il filtro sia presente in entrambi i pannelli

In caso contrario l'unica possibilità di rimuovere, nella pagina di
destinazione della ricerca, il filtro inizialmente impostato sarà quella
di agire sul pulsante "Rimuovi Filtro" eventualmente abilitato a livello
di Catalogo Articoli.

**ATTENZIONE!** I pannelli di ricerca collegati unicamente mediante il
parametro "Identificatore" restano sempre e comunque componenti distinti
per cui eventuali modifiche (grafiche e/o di configurazione) effettuato
per uno di essi non verranno riportate automaticamente anche sugli altri

**Colore di Sfondo Valore Attivo:** consente di impostare il colore di
sfondo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

**Colore del Testo Valore Attivo:** consente di impostare il colore del
Testo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

**Tipologia di filtro:** attraverso questo parametro (**visualizzato
solo per ricerche ecommerce**) è possibile decidere se il pannello di
ricerca dovrà gestire i vari campi utilizzati per realizzare il filtro
di ricerca, vincolandoli o meno l'uno all'altro.

E' possibile selezionare uno dei seguenti valori:

- **Non vincolato:** in queste condizioni i campi utilizzati per
  realizzare il filtro di ricerca non saranno in alcun modo legati tra
  loro.

> Gli elementi visualizzati all'interno di "Filtri Lista", "Filtri
> Indice" o "Filtro Set Attributi" non dipenderanno, quindi, da che cosa
> l'utente ha o non ha selezionato all'interno di questi campi ma
> solamente dagli articoli presenti all'interno del componente "Catalogo
> Ecommerce" o "Risultati Ricerca" che si trova nella pagina di
> destinazione del filtro.

- **Vincolato al livello precedente:** in queste condizioni gli elementi
  presenti all'interno di "Filtri Lista", "Filtri Indice" o "Filtro Set
  Attributi" dipenderanno non solo dagli articoli presenti all'interno
  del componente "Catalogo Ecommerce" o "Risultati Ricerca" che si trova
  nella pagina di destinazione del filtro, ma anche da quello che
  l'utente ha selezionato nei controlli precedenti a quello corrente.

> **Inoltre il controllo successivo a quello corrente verrà visualizzato
> solo dopo che l'utente avrà indicato uno specifico valore per il
> controllo corrente**

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\filtri_vincolati_1.bmp](./assets/media/image26.png)

> Nel caso in cui, in virtù o meno delle selezioni precedenti, un
> controllo non presenti alcun valore o abbia un'unica possibilità di
> scelta, verrà visualizzato il controllo immediatamente successivo (se
> presente) senza obbligo di interazione utente.
>
> In queste condizioni la ricerca potrà essere avviata anche senza dover
> arrivare per forza di cose a valorizzare l'ultimo controllo ma, in
> ogni caso, **per poterla avviare ed applicare così il relativo filtro,
> sarà sempre necessario cliccare sul pulsante "Ricerca"**
>
> **ATTENZIONE! nel momento in cui si dovesse decidere di realizzare un
> pannello di ricerca vincolato al precedente livello che, per sua
> stessa natura deve essere un componente altamente dinamico, occorre
> prestare particolare attenzione al fatto di non aver selezionato il
> parametro "Statico".**
>
> In queste condizioni, infatti, una eventuale staticizzazione del
> componente ne precluderebbe il corretto funzionamento

- **Vincolato a tutti i livelli:** in queste condizioni gli elementi
  presenti all'interno di "Filtri Lista", "Filtri Indice" o "Filtro Set
  Attributi" dipenderanno non solo dagli articoli presenti all'interno
  del componente "Catalogo Ecommerce" o "Risultati Ricerca" che si trova
  nella pagina di destinazione del filtro, ma anche da quello che
  l'utente ha selezionato nei vari controlli presenti all'interno del
  pannello di ricerca.

> **A differenza del caso precedente, in queste condizioni, verranno
> sempre visualizzati tutti i campi di filtro (lista, indice o set
> attributi) presenti nel pannello di ricerca.**

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\filtri_vincolati_2.bmp](./assets/media/image27.png)

> Selezionando uno specifico valore per uno qualsiasi dei controlli
> presenti all'interno del pannello di ricerca (es. 50''per il filtro
> indice "Dimensione Schermo"), verrà immediatamente applicato il
> relativo filtro articoli (senza dover quindi cliccare sul pulsante
> "Ricerca") e, contestualmente, verranno aggiornati anche tutti i
> possibili valori di selezione presenti negli altri controlli
> disponibili all'interno del pannello di ricerca.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\filtri_vincolati_3.bmp](./assets/media/image28.png)

> **NOTA BENE:** è possibile vincolare tra loro, ovviamente, solo
> controlli di tipo "Filtro Lista" "Filtro Indice" o "Filtro Set
> Attributi". Per maggiori informazioni relativamente ai controlli di
> tipo "Filtro Lista", "Filtro Indice" o "Filtro Set Attributi" si
> vedano i relativi capitoli di questo manuale (sezione "Componenti
> Interni ai Componenti Ecommerce")

**Considera le combinazioni di attributi (visibile solo in
corrispondenza di filtri vincolati):** in queste condizioni gli elementi
presenti all'interno di "Filtri Lista", "Filtri Indice" o "Filtro Set
Attributi" oltre a dipendere dagli articoli presenti all'interno del
componente "Catalogo Ecommerce" o "Risultati Ricerca" che si trova nella
pagina di destinazione del filtro e da quello che l'utente ha
selezionato nei controlli precedenti a quello corrente (come normalmente
avviene per i filtri vincolati), dipenderanno anche dalle combinazioni
di attributi definite per il/i set di attributi in cui è stato inserito
l'attributo in esame.

> **NOTA BENE:** per maggiori informazioni sull'utilizzo dei filtri
> vincolati si veda anche il successivo capitolo di questo manuale

**Ricerca Iniziale:** consente di dichiarare il filtro che dovrà essere
applicato in maniera automatica ogni volta in cui l'utente effettuerà
l'accesso ad una pagina del sito in cui è contenuto il pannello di
ricerca in questione.

Tale parametro potrebbe quindi essere particolarmente utile, ad esempio,
nel momento in cui si volesse fare in modo di mostrare automaticamente,
ad ogni utente che accede alla pagina catalogo, i soli articoli
effettivamente disponibili.

**ATTENZIONE!** In considerazione del fatto che ad ogni accesso alla
pagina in cui è presente il pannello di ricerca in esame dovrà essere
determinato un sotto insieme dei prodotti effettivamente presenti in
catalogo, l'utilizzo di questo parametro potrebbe anche aumentare i
tempi di caricamento del componente (il tutto in relazione sempre a
quelli che sono effettivamente gli articoli gestiti, la complessità del
filtro impostato ...)

Per maggiori informazioni relativamente a come poter determinare
l'effettivo valore da inserire all'interno di questo campo si veda anche
il successivo capitolo "*Querystring di ricerca -- Applicazione di un
filtro iniziale*" di questo manuale.

**Filtro Articoli:** consente di impostare una condizione di pre
filtraggio mediante la quale poter stabilire quali articoli dovranno
comparire o meno all'interno di eventuali componenti di tipo "Filtro
Indice" "Filtro Lista" o "Filtro Treeview" utilizzati all'interno del
pannello di ricerca.

Per maggiori informazioni relativamente alla creazione di un filtro
articoli si veda anche la sezione *"Utenti -- Gruppi Utenti Sito --
Filtri Utente e Filtri Articolo -- Filtri Articolo"* di questo manuale

**ATTENZIONE!** L'applicazione di un filtro articoli su di un pannello
di ricerca potrebbe limitare le opzioni di scelta disponibili
all'interno dei componenti "Filtro Indice", "Filtro Lista" o "Filtro
Treeview", pregiudicando quindi agli utenti la possibilità di effettuare
determinate ricerche.

Inoltre a differenza di un eventuale "Filtro iniziale" (parametro
"**Ricerca Iniziale**") i filtri impostati mediante il parametro in
oggetto non potranno essere rimossi a front end dagli utenti del sito.

Per ovvie ragioni l'applicazione di un filtro articoli su di un pannello
di ricerca non avrà invece alcun effetto sui normali componenti di tipo
"Filtro Testo" inseriti all'interno del pannello stesso.

**In conseguenza di ciò l'applicazione di un filtro articoli su di un
pannello di ricerca andrebbe necessariamente considerata soltanto nel
momento in cui sia stata impostata un'analoga condizione di pre
filtraggio anche sul componente "Catalogo Ecommerce" oggetto effettivo
delle ricerche.**

In questo modo si potrebbe infatti evitare di visualizzare, come
possibili opzioni per la creazione del filtro di ricerca, articoli che
di fatto non risulterebbero visualizzabili all'interno del componente
"Catalogo Ecommerce".

Per comprendere meglio l'utilizzo di questo campo supponiamo di aver
impostato sul componente Catalogo Ecommerce collegato al nostro pannello
di ricerca, un filtro tale da non visualizzare gli articoli in offerta;
supponiamo inoltre di aver inserito all'interno del pannello di ricerca
un componente "Filtro Lista" che mostri l'elenco dei codici articolo
presenti in catalogo.

In queste condizioni se non impostassimo anche sul pannello di ricerca
un filtro atto a nascondere gli articoli in offerta, tra le opzioni
selezionabili dal menu a tendina presente all'interno del pannello di
ricerca troveremmo anche codici relativi ad articoli in offerta che, se
selezionati, applicherebbero al catalogo un filtro articoli privo di
risultati.

Applicando invece anche al pannello di ricerca la stessa condizione di
pre filtraggio impostata sul componente catalogo ecommerce, gli articoli
in offerta non comparirebbero più come possibili opzioni di scelta
all'interno del menu a tendina, allineando di fatto l'elenco delle
opzioni con quanto effettivamente visualizzabile all'interno del
componente Catalogo Ecommerce

**Destinazione:** consente di definire la pagina di destinazione
all'interno della quale dovranno essere visualizzati i risultati del
filtro impostato. E' possibile selezionare uno dei seguenti valori:

- **Rimani su questa pagina:** in queste condizioni il filtro impostato
  mediante il pannello di ricerca in esame verrà applicato al componente
  "Catalogo Ecommerce / Risultati Ricerca" presente nella pagina del
  pannello stesso.

- **Rimanda alla pagina:** in queste condizioni il filtro impostato
  mediante il pannello di ricerca in esame verrà applicato al componente
  "Catalogo Ecommerce / Risultati Ricerca" presente nella pagina
  selezionata in corrispondenza di questo stesso parametro

In ogni caso dunque, affinché la ricerca possa funzionare in maniera
corretta, è indispensabile che nella pagina di destinazione sia presente
uno tra il componente "Catalogo E-Commerce" e il componente "Risultati
Ricerca".

**ATTENZIONE!!** L'applicazione automatica di un filtro iniziale
(parametro "**Ricerca Iniziale**") non produrrà mai un cambio di pagina.
Questo tipo di filtri quindi, verranno applicati sempre e soltanto alla
pagina in cui si trova il pannello in questione

Inoltre nel caso in cui **il pannello di ricerca sia impostato per
gestire dei filtri vincolati (in particolar modo "vincolati a tutti i
livelli") e la pagina di destinazione del filtro sia diversa dalla
pagina corrente, è opportuno che nella pagina di destinazione sia
presente lo stesso componente di ricerca presente anche nella pagina di
partenza oppure che i due pannelli di ricerca siano collegati tra loro
mediante il parametro "Identificatore"**.

In caso contrario infatti una volta applicato il filtro verrà effettuato
un cambio pagina e non sarà più possibile proseguire nel filtraggio
selettivo degli articoli presenti in catalogo.

In relazione all'utilizzo dei filtri vincolati occorre poi ricordare che
:

- Nel momento in cui il pannello di ricerca dovesse essere **vincolato
  al precedente livello** e la Destinazione dovesse essere una pagina
  diversa da quella in cui si trova il pannello stesso, il cambio pagina
  verrà fatto automaticamente al termine dell'impostazione dell'ultimo
  campo di filtro.

- Nel momento in cui il pannello di ricerca dovesse essere **vincolato a
  tutti i livelli** e la Destinazione dovesse essere una pagina diversa
  da quella in cui si trova il pannello stesso, per effettuare il cambio
  pagina (e vedere quindi i risultati del filtro) sarà necessario
  cliccare sul relativo pulsante di Ricerca

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- Il pannello di ricerca (Campi)

- Il pulsante per avviare la ricerca (Submit)

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

Relativamente alla possibilità da parte dell'utente che visita il sito
di eliminare eventuali filtri di ricerca precedentemente impostati vanno
poi considerate le seguenti casistiche:

- Nel caso in cui il pannello di ricerca gestisca "**filtri vincolati al
  precedente livello**", l'eliminazione di uno dei valori selezionati
  azzererà completamente il filtro eventualmente applicato agli articoli
  in catalogo. Verranno invece mantenuti tutti i valori delle selezioni
  effettuate per i controlli precedenti a quello di rimozione.

- Nel caso in cui il pannello di ricerca gestisca dei "**filtri
  vincolati a tutti i livelli**" l'eliminazione di uno dei valori
  selezionati azzererà solamente la relativa condizione di filtro.
  Eventuali altre condizioni di filtro applicate a seguito della
  selezione di determinati valori presenti in altri controlli del
  pannello di ricerca, rimarranno applicate. Per azzerare completamente
  i filtri impostati sarà quindi necessario rimuoverli uno ad uno oppure
  cliccare sul pulsante "Rimuovi il filtro applicato" associato ai
  componenti "Catalogo Ecommerce" o "Risultati Ricerca".

- Nel caso in cui la pagina di destinazione del filtro contenga
  esattamente lo stesso componente di ricerca utilizzato per impostare
  il filtro (stesso componente distribuito in pagine diverse), oppure
  nel caso in cui i due distinti pannelli di ricerca siano collegati tra
  loro mediante il parametro "Identificatore" e nel caso in cui
  contengano ovviamente gli stessi campi di ricerca, il filtro impostato
  nella pagina di parenza continuerà ad essere evidenziato anche nel
  pannello di ricerca della pagine di destinazione e potrà quindi essere
  eliminato cliccando sul corrispondente pulsante di azzeramento
  **(x)**.

- Nel caso in cui la pagina di destinazione del filtro contenga un
  componente di ricerca differente da quello utilizzato per impostare il
  filtro e non collegato ad esso mediante il parametro "Identificatore",
  il filtro inizialmente impostato NON potrà, ovviamente, essere
  eliminato operando all'interno del componente di ricerca.

> In queste condizioni sarà comunque possibile eliminare eventuali
> filtri presenti sul "Catalogo Ecommerce" e/o sul componente "Risultati
> Ricerca" agendo sul pulsante "Rimuovi filtro applicato" contestuale a
> questi stessi componenti
>
> **NOTA BENE:** il pulsante "Rimuovi filtro applicato" contestuale ai
> componenti "Catalogo E-commerce" e "Risultati Ricerca" verrà
> visualizzato non appena dovesse essere applicato, a questi stessi
> componenti, uno specifico filtro di ricerca.

- Al cambio di pagina, verranno automaticamente azzerati tutti i filtri
  precedentemente impostati sui componenti "Catalogo E-commerce" e/o
  "Risultati Ricerca".

> **NOTA BENE:** la rimozione automatica dei filtri di ricerca al cambio
> pagina non avviene nel caso in cui ci si sposti dalla pagina di
> destinazione del filtro alla pagina Prodotto di uno specifico articolo
> presente nei risultati del filtro precedentemente impostato.
>
> In questo modo dunque nel caso in cui un utente dovesse applicare un
> certo filtro di ricerca e, successivamente, cliccare su un articolo
> risultante dal filtro per visualizzarne il dettaglio, avrebbe comunque
> la possibilità di tornare alla pagina precedente mantenendo
> memorizzati i risultati del filtro precedentemente impostato (filtro
> questo che potrebbe poi essere rimosso manualmente, ad esempio
> attraverso il pulsante "Rimuovi Filtro").

Il pulsante "**Salva**" consentirà invece di salvare le modifiche
apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, il
Componente **"Ricerca" può essere considerato a tutti gli effetti come
un "Componente di tipo Contenitore** Sarà infatti possibile inserire al
suo interno tutta una serie di campi che andranno a definire lo
specifico filtro di ricerca e che per poter esser gestiti liberamente,
dovranno, inevitabilmente, esser trattati a loro volta come Componenti
autonomi editabili singolarmente.

Per poter costruire quindi il proprio filtro di ricerca sarà necessario,
innanzitutto, attivare la modalità di gestione dei componenti. Occorrerà
poi portarsi sul Componente "Filtro/Ricerca Catalogo" presente nella
pagina e, alla comparsa del R.O.C. cliccare sull'icona "**Accedi ai
componenti interni".**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Varianti Sito Responsive -- Componenti -- Componenti di tipo
Contenitore")**

In particolare all'interno di un componente di tipo "Ricerca Ecommerce"
sarà possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale

- **Componenti E-Commerce:** contiene i componenti che potranno essere
  inseriti all'interno del componente "Ricerca" per poter realizzare e
  definire il proprio filtro.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Ricerca" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

Ad ogni Componente E-commerce inserito all'interno del pannello di
ricerca dovrà necessariamente corrispondere uno specifico campo Mexal o
uno specifico Attributo Articolo, e sarà poi su questi elementi che
verrà effettuata la ricerca, lato sito, sulla base dei valori indicati
dall'utente all'interno di questi stessi campi.

**Per poter creare un filtro di ricerca valido sarà quindi necessario
inserire all'interno del Componente Ricerca almeno un Componente
E-Commerce**.

> **NOTA BENE:** utilizzando due o più Componenti E-Commerce il filtro
> di ricerca verrà definito considerando i vari campi in AND tra loro.

