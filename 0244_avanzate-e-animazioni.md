# AVANZATE E ANIMAZIONI



La sezione "**Avanzate e Animazioni**" presente nella maschera di
configurazione di ogni singolo Componente Passweb consente di:

- impostare la visibilità del componente in oggetto in relazione allo
  specifico dispositivo in cui verrà poi visualizzato il sito

- definire la larghezza di base del componente

- inserire eventuali regole CSS aggiuntive utili per stilizzare il
  componente in maniera avanzata

- associare al componente in esame classi CSS personalizzate

- associare al componete in esame attributi HTML addizionali

- attivare per il componente in esame specifiche animazioni CSS

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti_configurazione_3_res.bmp](./assets/media/image72.png)

Nello specifico dunque il parametro:

- **Visibilità:** consente di impostare la visibilità del componente in
  esame in relazione allo specifico dispositivo, o meglio, **in
  relazione alla specifica dimensione dello schermo del dispositivo**,
  su cui verrà poi visualizzato il sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visibilita_componente.bmp](./assets/media/image73.png)

> Grazie a questo parametro è possibile quindi decidere, in maniera
> piuttosto semplice, quali contenuti della pagina dovranno essere
> visualizzati e quali no sulle diverse tipologie di dispositivi,
> soddisfacendo uno dei principi base di un sito responsivo secondo cui
> non tutti i contenuti di una pagina web visualizzata su di uno schermo
> desktop devono obbligatoriamente essere riproposti anche quando la
> stessa pagina verrà visualizzata su di uno smartphone o su di un
> tablet.
>
> Tecnicamente, nel momento in cui si dovesse decidere, ad esempio, di
> rendere lo specifico componente visibile solo per "Dispositivi small e
> inferiori" (ossia per dispositivi di larghezza minore di 768 px)
> Passweb attribuirà al componente stesso una specifica classe CSS che,
> mediante l'utilizzo di apposite media query, imposterà automaticamente
> la sua proprietà "display" sul valore "none" per larghezze di pagina
> maggiori o uguali a 768 px e sul valore "block" per larghezze di
> pagina minori di 768 px.
>
> Il risultato di questa configurazione sarà dunque quello di
> visualizzare il componente in esame, sul front end del sito, solo ed
> esclusivamente nel momento in cui la larghezza dello schermo del
> dispositivo di visualizzazione dovesse essere effettivamente inferiore
> ai 768 px.
>
> In realtà la configurazione in esame avrà effetto non solo sul front
> end del sito ma anche nell'ambiente di back end, in maniera tale da
> mantenere inalterata la logica del WYSWYG dando a chi costruisce il
> sito sempre l'esatta percezione di quello che sarà poi il risultato
> finale, ovviamente, nelle stesse condizioni di visualizzazione.
>
> **In sostanza dunque supponendo di lavorare, in fase di costruzione
> del sito, su di uno schermo di larghezza superiore ai 768px una volta
> salvate le impostazioni indicate nell'esempio, il componente in
> oggetto diventerà invisibile anche all'interno del Wizard.**
>
> In queste condizioni sarà comunque possibile selezionare il componente
> (che resta ovviamente presente all'interno della pagina) per poterne
> variare contenuti e aspetto grafico, in due modi diversi:

- **Dall'albero dei Componenti**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_componente_albero.bmp](./assets/media/image74.png)

> In queste condizioni una volta selezionato il componente in esame
> compariranno nella barra degli strumenti tutte le icone di gestione
> normalmente presenti all'interno del R.O.C. del componente stesso
> (come se questo fosse selezionato direttamente all'interno della
> pagina) per cui utilizzando tali icone, anche in queste condizioni,
> sarà comunque possibile, ad esempio, aprire la maschera di
> configurazione del componente, accedere al suo style editor, copiarlo,
> collegarlo ad altre pagine ecc...
>
> Ovviamente il componente resterà non visibile all'interno della pagina
> per cui per verificare i risultati di determinate variazioni grafiche
> si dovrà agire dal front end del sito restringendo la finestra del
> browser fino a raggiungere una dimensione inferiore ai 768px (in
> maniera tale da far apparire il componente) oppure visualizzando il
> sito direttamente all'interno di uno smartphone.
>
> ATTENZIONE! sulla base di quanto detto è consigliabile agire in questo
> modo solo nel momento in cui l'esigenza dovesse essere quella di
> apportare alcune variazioni ai parametri di configurazione del
> componente
>
> Nel momento in cui l'esigenza dovesse essere invece quella di
> modificarne l'aspetto grafico si consiglia di procedere come di
> seguito indicato in maniera tale da avere un riscontro visivo
> immediato anche nel back end del sito.

- **Utilizzando il pulsante "Classi Responsive"** presente nel menu
  principale di Editing del sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\me_classi_responsive.bmp](./assets/media/image75.png)

> Cliccando su questo pulsante verrà infatti visualizzato immediatamente
> a fianco del menu di editing un piccolo box mediante il quale poter
> selezionare quali elementi, tra quelli che normalmente sarebbero
> nascosti in una visualizzazione desktop, dovranno invece essere
> visualizzati all'interno del Live Editing in maniera tale da poter
> essere correttamente gestiti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\classi_responsive.bmp](./assets/media/image76.png)

> Selezionando dunque, in relazione allo specifico esempio che stiamo
> considerando, l'opzione "**Medium e Superiori ( \>= 768px )**",
> verranno visualizzati all'interno del Live Editing tutti quei
> componenti il cui parametro visibilità è stato impostato sul valore
> "Small e Inferiori".
>
> Il risultato di questa operazione sarà dunque quello, da una parte, di
> mantenere inalterato il front end del sito, e dall'altra parte di
> rendere visibile nel back end anche quei componenti che sul front end
> sono invece visualizzati solo per risoluzioni inferiori ai 768 px.
>
> In queste condizioni il nostro componente tornerà quindi ad essere
> visibile e direttamente selezionabile anche all'interno dell'ambiente
> di sviluppo per cui anche eventuali variazioni grafiche ad esso
> apportate potranno essere visualizzate direttamente all'interno del
> Wizard.
>
> **ATTENZIONE!** le classi utilizzate per gestire la visibilità di un
> componente, in relazione alle diverse risoluzioni dello schermo del
> dispositivo su cui viene visualizzato il sito, sono esattamente le
> stesse classi utilizzate, per lo stesso scopo, da Bootstrap, il noto
> framework CSS integrato nativamente in Passweb per la gestione dei
> siti responsivi.

- **Larghezza:** consente di definire la larghezza e, per certi versi,
  anche il posizionamento che andrà ad assumere, a default, il
  componente all'interno della pagina e/o del contenitore in cui verrà
  poi inserito.

> **ATTENZIONE!** Dimensione e posizionamento di default del componente
> possono essere modificati in un qualsiasi momento utilizzando i
> normali strumenti di gestione di Passweb (es. Style Editor, CSS
> ecc...)
>
> E' possibile selezionare uno dei seguenti valori:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\larghezza_componente.bmp](./assets/media/image77.png)

- **Centrato con padding laterale**: selezionando questa opzione il
  componente in oggetto verrà centrato orizzontalmente rispetto alla
  pagina (o al contenitore) in cui è inserito, gli verrà assegnato un
  padding destro e sinistro (ossia uno scostamento rispetto ai bordi del
  contenitore padre) di 15 px e assumerà una larghezza massima variabile
  in relazione alla larghezza del dispositivo di visualizzazione
  utilizzato.

![Videate\\centrato_padding.bmp](./assets/media/image78.png)

> Nello specifico la larghezza massima assegnata a default al componente
> sarà di:

- **1140 px** per dispositivi di larghezza **maggiore o uguale a 1200
  px**

- **960 px** per dispositivi di larghezza **compresa tra 992 px e 1119
  px**

- **720 px** per dispositivi di larghezza **compresa tra 768 px e 991
  px**

- **540 px** per dispositivi di larghezza **compresa tra 576 px e 767
  px**

> Infine, per dispositivi di **larghezza inferiore a 576 px** il
> componente assumerà a default una **larghezza pari al 100% del
> contenitore in cui è inserito**
>
> **ATTENZIONE!** Tecnicamente questo comportamento è determinato dal
> fatto di assegnare al componente in oggetto la classe CSS
> "**bs-container**"

- **Centrato senza padding laterale**: selezionando questa opzione il
  componente in oggetto verrà centrato orizzontalmente rispetto alla
  pagina (o al contenitore) in cui è inserito e assumerà una larghezza
  massima variabile in relazione alla larghezza del dispositivo di
  visualizzazione utilizzato.

![Videate\\centrato_no_padding.bmp](./assets/media/image79.png)

> La larghezza massima assegnata a default al componente sarà
> esattamente analoga a quella della configurazione precedente

- **1140 px** per dispositivi di larghezza **maggiore o uguale a 1200
  px**

- **960 px** per dispositivi di larghezza **compresa tra 992 px e 1119
  px**

- **720 px** per dispositivi di larghezza **compresa tra 768 px e 991
  px**

- **540 px** per dispositivi di larghezza **compresa tra 576 px e 767
  px**

> Infine, per dispositivi di **larghezza inferiore a 576 px** il
> componente assumerà a default una **larghezza pari al 100% del
> contenitore in cui è inserito**
>
> **ATTENZIONE!** Tecnicamente questo comportamento è determinato dal
> fatto di assegnare al componente in oggetto le classi CSS
> "**bs-container**" e "**no-gutter**"

- **Fluido con padding laterale:** selezionando questa opzione il
  componente in oggetto assumerà sempre una larghezza pari al 100% del
  contenitore in cui è inserito e gli verrà assegnato inoltre un padding
  destro e sinistro di 15px

![Videate\\fluido_padding.bmp](./assets/media/image80.png)

> **ATTENZIONE!** Tecnicamente questo comportamento è determinato dal
> fatto di assegnare al componente in oggetto la classe
> "**container-fluid**"

- **Fluido senza padding laterale:** selezionando questa opzione il
  componente in oggetto assumerà sempre una larghezza pari al 100% del
  contenitore in cui è inserito.

![Videate\\fluido_no_padding.bmp](./assets/media/image81.png)

> **ATTENZIONE!** Tecnicamente questo comportamento è determinato dal
> fatto di assegnare al componente in oggetto le classi
> "**container-fluid**" e "**no-gutter**"

- **Custom:** selezionando questa opzione il dimensionamento e il
  posizionamento del componente in oggetto dipendono dallo specifico tag
  HTML (nel caso di un div ad esempio il componente assumerà una width
  del 100%) e, di base, potrà essere controllato direttamente dallo
  Style Editor mediante le specifiche proprietà CSS

> **ATTENZIONE!** in queste condizioni al componente non vengono
> assegnate classi particolari

- **Visibilità app:** disponibile solo nel caso in cui sia stato
  attivato il modulo di gestione dell'App mobile e la pagina in esame
  sia stata impostata come visibile tanto per il Sito quanto per l'App.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_visibilita_app.bmp](./assets/media/image82.png)

> Consente di impostare la visibilità del Componente a livello di Sito
> Web e/o di App Mobile. E' possibile selezionare uno dei seguenti
> valori:

- **Sia sito che app:** selezionando questa opzione il Componente in
  esame sarà visibile sia all'interno del sito sia all'interno dell'app
  mobile originata a partire dal sito stesso

- **Solo sito:** selezionando questa opzione il Componente in esame sarà
  visibile solo ed esclusivamente all'interno del sito web

- **Solo app:** selezionando questa opzione il Componente in esame sarà
  visibile solo ed esclusivamente all'interno dell'app mobile

<!-- -->

- **CSS:** consente di inserire regole CSS aggiuntive utili per
  stilizzare, in maniera avanzata, il componente in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\avanzate_animazioni_css.bmp](./assets/media/image83.png)

> Come già per gli altri editor di codice presenti nelle diverse sezioni
> di Passweb, anche in questo caso sono attivi i seguenti tasti
> funzione:

- **Ctrl + F / Cmd + F** Consente di abilitare la funzione di ricerca
  all'interno dell'editor di codice HTML, attivando il relativo campo di
  testo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_mirror_ricerca.bmp](./assets/media/image84.png)

- **Ctrl + G / Cmd + G**: Consente, una volta effettuata una specifica
  ricerca all'interno dell'editor di codice HTML, di attivare la
  funzione "**Passa al successivo**"

- **Shift + Ctrl + G / Shift + Cmd + G** : Consente, una volta
  effettuata una specifica ricerca all'interno dell'editor di codice
  HTML, di attivare la funzione "**Passa al precedente**"

- **Shift + Ctrl + F / Cmd + Option + F**: Consente di attivare la
  funzione di "**Cerca e sostituisci**".

- **Shift + Ctrl + R / Shift + Cmd + Option + F** : Consente di attivare
  la funzione di "**Cerca e sostituisci tutto**".

- **Alt + F**: Consente di attivare la funzione di ricerca
  "persistente".

> In queste condizioni nel caso in cui il testo ricercato dovesse
> presentare più occorrenze sarà possibile passare all'elemento
> successivo / precedente utilizzando rispettivamente i tasti
> "**Invio**" e "**Shift + Invio**"

- **Alt + G**: Consente di attivare la funzione "**Vai alla linea**".

> Utilizzando questa combinazione di tasti verrà quindi visualizzato un
> campo di input in cui inserire il numero di riga (ed eventualmente
> anche quello di colonna) in corrispondenza del quale spostare il
> cursore
>
> **ATTENZIONE!** Il codice CSS inserito all\'interno di questo campo
> verrà salvato in un apposito file (components.css) diverso da quello
> utilizzato per salvare le regole CSS inserite e gestite invece a
> livello di layout.
>
> **Tale campo diventa di fondamentale importanza e andrebbe utilizzato
> solo ed esclusivamente nel momento in cui l\'esigenza dovesse essere
> quella di esportare il componente in esame per poterlo importare e
> riutilizzare in una qualsiasi altra pagina della stessa variante e/o
> di varianti differenti.**
>
> Come evidenziato nei relativi capitoli di questo manuale infatti, in
> fase di esportazione di un componente verranno considerate (e quindi
> salvate) oltre alle proprietà di configurazione del componente stesso
> anche che eventuali regole CSS inserite all'interno del campo in
> esame. Non verranno invece considerate eventuali regole CSS e/o
> funzioni javascript aggiunte per il componente in esame a livello di
> layout.
>
> In realtà in relazione all\'utilizzo di questo campo è bene
> evidenziare un paio di cose di fondamentale importanza:

- Nel caso in cui l\'esigenza dovesse essere quella **di esportare il
  componente in esame per poterlo poi importare e riutilizzare una o più
  volte all\'interno della stessa Variante** è indubbiamente
  consigliabile inserire eventuali regole CSS aggiuntive direttamente a
  livello di layout (magari a livello di Layout di Variante).

> In questo modo infatti, da una parte si eviterà il rischio di scrivere
> all\'interno del file components.css più volte e inutilmente le stesse
> regole, e dall\'altra parte, sarà sicuramente più semplice gestirle
> potendo agire da un unico punto (il layout) anziché dover andare a
> ricercare la specifica regola nelle maschere di configurazione dei
> singoli componenti.

- Nel caso in cui l\'esigenza dovesse essere invece quella **di
  esportare il componente in esame per poterlo poi importare e
  riutilizzare all'interno di un'altra Variante dello stesso Sito**,
  allora è necessario, prima di effettuare l\'esportazione, riportare
  all\'interno di questo campo tutte le regole CSS aggiuntive utilizzate
  per stilizzare il componente stesso.

> In caso contrario infatti, il risultato che si otterrebbe andando poi
> a importare questo componente in un altra Variante potrebbe non
> coincidere esattamente, dal punto di vista grafico, con il componente
> originale.
>
> Se poi anche in questo caso, nella Variante di destinazione lo stesso
> componente dovesse essere importato ed utilizzato più volte nella
> stessa pagina o in pagine diverse, è sempre consigliabile, per le
> stesse ragioni sopra evidenziate, trasferire eventuali regole CSS
> aggiuntive inizialmente impostate sul componente, a livello di Layout
> eliminandole dunque dal campo CSS presente nella loro maschera di
> configurazione, ed inserendole nella sezione CSS del Layout di Pagina
> o di Variante.
>
> **ATTENZIONE! Nel caso in cui lo stesso componente dovesse essere
> importato ed utilizzato più volte all\'interno della stessa Variante è
> sempre consigliabile gestire codice CSS aggiuntivo a livello di Layout
> e non di singolo Componente.**
>
> In quest'ultimo caso infatti eventuali modifiche apportare alle regole
> CSS presenti nella maschera di configurazione di uno qualsiasi dei
> componenti importati potrebbero, da una parte ovviamente, andare ad
> influire anche sugli altri componenti dello stesso tipo e, dall\'altra
> parte, potrebbero portare a replicare più volte e inutilmente le
> stesse regole CSS all\'interno del file components.css rendendo quindi
> la loro gestione particolarmente complessa.
>
> In questo senso è quindi possibile agire mediante il pulsante
> "**Sposta il css nel layout**" presente all'interno dalla sezione
> "**CSS Componenti**" del layout di sito.
>
> Per maggiori informazioni in merito si veda anche la sezione "*Live
> Editing per Varianti Responsive -- Layout -- Gestisci -- CSS
> Componenti*" di questo manuale

- **Classi Addizionali:** consente di associare al componente in esame
  una o più classi CSS.

> Tali classi potranno poi essere richiamate ed utilizzate, ad esempio a
> livello di Layout, nel relativo editor di codice CSS, per
> personalizzare la grafica del componente. **Questo tipo di
> personalizzazione richiede specifiche conoscenze di codice CSS ed è
> quindi consigliato a soli utenti esperti in tal senso.**

- **Attributi addizionali:** consente di aggiungere al markup HTML del
  relativo componente degli attributi addizionali (particolarmente utili
  nell'applicazione e nell'utilizzo di vari plugin javascript).

> Ogni attributo, con il relativo valore, deve essere inserito
> esattamente come se si dovesse intervenire direttamente sul markup
> HTML del componente stesso.

- **Abilita Animazione:** consente di abilitare/disabilitare per il
  componente in esame specifiche animazioni CSS.

> Nel caso in cui si voglia visualizzare il componente in esame con una
> certa animazione sarà quindi necessario, per prima cosa, impostare
> questo parametro sul valore "**Animazione Abilitata**"
>
> Verranno quindi visualizzati ulteriori campi attraverso i quali poter
> impostare le caratteristiche e le proprietà dell'animazione che si
> intende applicare. In particolare il campo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti_configurazione_4_res.bmp](./assets/media/image85.png)

- **Animazione**: consente di selezionare, da un apposito menu a
  tendina, il tipo di animazione che si intende abilitare (bounce,
  fadeIn, fadeOut ecc...)

- **Ritardo di Animazione (in secondi)**: consente di impostare il
  ritardo dell'animazione, ossia l'intervallo temporale dopo il quale
  verrà avviata l'animazione di visualizzazione del componente

- **Durata Animazione (in secondo)**: consente di impostare la durata
  dell'animazione. Trascorso tale intervallo di tempo il componente sarà
  completamente visualizzato all'interno della pagina

**NOTA BENE**: per intervalli di tempo che richiedono l'uso di decimali
è necessario utilizzare il carattere "."

