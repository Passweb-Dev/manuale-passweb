# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-immagine_res.bmp](./assets/media/image5.png){width="5.143055555555556in"
height="3.1041666666666665in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà poi possibile
inserire il contenuto e settare i principali parametri di configurazione
del componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

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

**Caricamento Immagine:** consente di decidere come dovrà essere
effettuato il caricamento dell'immagine gestita mediante il componente
in oggetto. È possibile selezionare uno dei seguenti valori:

- **Immediato**: selezionando questa opzione l'immagine verrà caricata
  sempre e comunque in maniera immediata, indipendentemente dal fatto di
  aver attivato o meno, a livello di sito, il caricamento delle immagini
  mediante lazy loading.

> In altre termini dunque, in queste condizioni, nel momento in cui il
> browser incontrerà, in fase di rendering della pagina, il relativo tag
> img effettuerà immediatamente il download della relativa risorsa e
> solo al termine di questo download proseguirà nel caricamento dei
> contenuti processando gli altri tag della pagina.
>
> **ATTENZIONE!** Nel momento in cui l'immagine in esame dovesse essere
> individuata come il **Largest Contentful Paint (LCP)** della pagina è
> consigliabile caricarla in maniera immediata in maniera tale da non
> dover attendere troppo tempo prima di averla effettivamente
> disponibile (con il rischio di ottenere poi dei punteggi bassi in
> relazione al corrispondente Core Web Vital)

- **Lazy**: selezionando questa opzione l'immagine verrà caricata
  mediante lazy loading secondo quanto indicato in corrispondenza del
  parametro "**Caricamento Immagini**" presente alla pagina "**Sito --
  Preferenze**" del Wizard (tab "**SEO**" sezione "**Caricamento
  Pagina**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\leggimi_71.bmp](./assets/media/image6.png){width="5.136111111111111in"
height="3.1104166666666666in"}

> Per maggiori informazioni relativamente alla possibilità e
> all'opportunità di caricare determinate immagini mediante lazy loading
> si veda anche quanto indicato al capitolo "*Sito -- Preferenze -- SEO
> Caricamento Pagina*" di questo manuale

**ATTENZIONE!** Il parametro "**Caricamento immagine**" presente nel
form di configurazione del singolo componente "**Immagine con Link**"
verrà preso in considerazione solo nel momento in cui sia stato
effettivamente abilitato il caricamento della immagini, a livello di
sito, mediante lazy loading. In caso contrario ogni immagine verrà
sempre e comunque caricata in maniera immediata

All'interno della sotto sezione "**Opzioni Immagine**" oltra a poter
definire come dovrà essere caricata la specifica immagine (se
immediatamente o mediante lazy loading) è anche possibile, ovviamente,
indicare la risorsa che dovrà essere visualizzata all'interno del
componente, selezionandola dal database delle risorse del proprio sito
oppure mappandola con uno degli Attributi Immagine precedentemente
codificati all'interno della sezione "Gestione Temi" del Wizard.

Oltre all'immagine di base è poi possibile indicare anche la specifica
risorsa che dovrà essere visualizzata:

- al passaggio del mouse sul componente

- nei Tablet

- negli Smartphone

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-immagine_2_res.bmp](./assets/media/image7.png){width="5.129861111111111in"
height="3.0909722222222222in"}

Nello specifico dunque il parametro:

**Immagine:** consente di selezionare la specifica immagine da inserire
all'interno della pagina web. Per caricare la risorsa desiderata è
sufficiente premere sul pulsante "**Seleziona la Risorsa**". In questo
modo si verrà infatti ricondotti alla maschera di "Gestione delle
Risorse" attraverso la quale verranno mostrate le cartelle e le risorse
caricate su Passweb, e da cui sarà possibile selezionare dall'elenco (o
caricarla ex-novo dal proprio computer) l'immagine da inserire
all'interno della pagina web.

La piccola x posta a fianco del pulsante "**Seleziona Risorsa**"
consente di azzerare il campo ed eliminare quindi l'associazione con la
risorsa precedentemente selezionata.

In alternativa è anche possibile utilizzare come immagine un apposito
Attributo precedentemente codificato all'interno della sezione "Gestione
Temi" del Wizard.

In questo senso il menu a tendina presente in corrispondenza del
parametro "**Attributi Temi**" consente di selezionare, tra quelli
presenti in elenco, lo specifico Attributo di tipo Immagine da
utilizzare.

**Immagine Rollover (opzionale):** permette di selezionare l'eventuale
immagine alternativa che apparirà al passaggio del mouse.

È possibile indicare una delle immagini presenti nel database del sito
oppure uno degli Attributi Immagine gestiti.

**Immagine per dispositivi Tablet:** consente di indicare la specifica
immagine che dovrà essere visualizzata, al posto di quella base, nel
momento in cui la dimensione del dispositivo di visualizzazione del sito
dovesse essere **inferiore ai 992px**

È possibile indicare una delle immagini presenti nel database del sito
oppure uno degli Attributi Immagine gestiti.

**Immagine per dispositivi Smartphone:** consente di indicare la
specifica immagine che dovrà essere visualizzata al posto di quella base
nel momento in cui la dimensione del dispositivo di visualizzazione del
sito dovesse essere **inferiore ai 576px**

È possibile indicare una delle immagini presenti nel database del sito
oppure uno degli Attributi Immagine gestiti.

**ATTENZIONE!** il pulsante "**Applica impostazione Immagine alle altre
Lingue**", presente in corrispondenza di ciascuno dei campi sopra
indicati, consente di utilizzare automaticamente l'immagine indicata per
tutte le lingue attualmente gestite all'interno del sito

**Testo Alternativo (per accessibilità)** **-- campo obbligatorio**
consente di impostare, in tutte le lingue attualmente gestite
all'interno del sito, il valore che dovrà avere, per l'immagine in
esame, l'**attributo alt** attributo questo di fondamentale importanza
inquanto:

- serve a descrivere il contenuto dell'immagine quando questa non viene
  caricata

- viene utilizzato dai lettori di schermo per l'accessibilità

- è interpretato dai motori di ricerca per capire il contenuto visivo
  della pagina

- è un fattore di ranking diretto per la Ricerca Immagini di Google

- aiuta a rafforzare la pertinenza semantica della pagina

- ...

**Title**: consente di impostare, in tutte le lingue attualmente gestite
all'interno del sito, il valore dell'**attributo title** che dovrà
essere utilizzato per l'immagine in esame.

A differenza dell'attributo alt, il title non ha un valore diretto per
il ranking dell'immagine e può anche essere ignorato dai browser mobili
e da alcuni screen reader. Il suo scopo è essenzialmente quello di
mostrare un tooltip (su desktop) al passaggio del mouse sull'immagine
per visualizzarne la descrizione e, in conseguenza di ciò, è utilizzato
più che altro per ottimizzare l'interfaccia utente.

**ATTENZIONE!** il consiglio, anche ai fini di eventuali test di
accessibilità sulla pagina, è quello di non valorizzare mai allo stesso
modo alt e title per la stessa immagine (il valore dei due attributi
dovrebbe essere diverso)

**Testo Didascalia:** consente, se valorizzato, di gestire il cosiddetto
"**caption**" sull'immagine, ossia del testo in formato HTML che verrà
poi utilizzato come "didascalia" all'immagine stessa. In questo senso il
successivo parametro "**Testo Didascalia Posizione**" permette di
decidere se tale didascalia dovrà essere visualizzata sopra o sotto
l'immagine in questione.

Ovviamente poi è sempre possibile utilizzare lo Style Editor di Passweb
e/o gli strumenti di editing avanzato (sezione CSS del Layout) per
intervenire tanto sull'immagine quanto sul relativo caption in maniera
tale da ottenere gli effetti grafici più disparati.

**Larghezza / Altezza:** consentono di specificare le dimensioni
dell'immagine come attributi "width" e "height" del tag img.

**ATTENZIONE:** E' buona norma indicare all'interno di questi campi le
esatte dimensioni dell'immagine. La presenza degli attributi "width" e
"height" all'interno del tag img permette infatti al browser di
effettuare un numero minore di operazioni in fase di rendering della
pagina migliorando, di conseguenza, la velocità di risposta e i tempi di
caricamento della pagina stessa.

Volendo è comunque possibile ridimensionare l'immagine utilizzando lo
Style Editor di Passweb e agendo quindi sulle relative proprietà CSS. In
questo senso è bene sottolineare però che un ridimensionamento
dell'immagine rispetto a quelle che sono le sue dimensioni originali
costringerà il browser ad effettuare un'operazione di resizing con un
conseguente deterioramento (proporzionale al numero di immagini) dei
tempi di caricamento della pagina.

**In definitiva dunque, è sempre bene utilizzare all'interno del sito
immagini già delle dimensioni corrette indicando tali dimensioni
direttamente all'interno di questi due campi ed evitando di effettuare
ridimensionamenti CSS**.

**Funzionamento:** consente di impostare la tipologia di immagine che si
intende inserire all'interno del sito. E' possibile selezionare uno dei
seguenti valori:

- **Solo Immagine:** selezionando questa opzione il componente
  consentirà di inserire all'interno del sito una semplice immagine

- **Immagine con Link:** selezionando questa opzione il componente
  consentirà di inserire all'interno del sito un'immagine con un link
  associato.

> **ATTENZIONE! Per siti in multilingua la destinazione e le proprietà
> del link andranno specificate e potranno quindi essere differenti per
> ciascuna delle lingue gestite all'interno del sito**
>
> Volendo sarà quindi possibile impostare il link di collegamento
> associato all'immagine in maniera tale che per il sito in Italiano
> punti ad una certa pagina (pagina A) mentre per il sito in Inglese
> punti invece ad una pagina completamente diversa dalla precedente
> (pagina B).

Nel momento in cui si dovesse decidere di associare all'immagine un link
sarà quindi necessario indicare un valore anche per i seguenti
parametri:

**Link:** consente di definire la tipologia di link che si intende
realizzare. E' possibile selezionare uno dei seguenti valori:

- **Link a pagina esterna / Link all'Area Riservata**: consente di
  indicare la pagina di destinazione del link. E' possibile digitare
  esplicitamente l' url della pagina che si vuole raggiungere (es.
  <http://www.google.it>).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\immagine_link_ar_2_res.bmp](./assets/media/image8.png){width="5.129861111111111in"
height="3.084722222222222in"}

> **ATTENZIONE!** Per creare il collegamento ad una pagina esterna è
> necessario indicare il percorso assoluto del link (nella forma
> http://www.indirizzosito.it)
>
> Nel momento in cui l'esigenza dovesse essere invece quella di creare
> un collegamento ad una delle diverse sezioni dell'Area Riservata del
> proprio sito sarà necessario selezionare tale sezione dal relativo
> menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\immagine_link_ar_1_res.bmp](./assets/media/image9.png){width="5.129861111111111in"
height="3.1041666666666665in"}

> In queste condizioni il link creato funzionerà in maniera diversa a
> seconda del fatto che l'utente abbia o meno già effettuato
> l'autenticazione al sito.
>
> Nel primo caso (utente già autenticato) il link porterà direttamente
> alla relativa sezione dell'Area Riservata
>
> Nel secondo caso (utente non ancora autenticato) il link porterà
> invece alla pagina di accesso in Area Riservata e l'utente dovrà, per
> poter accedere, inserire le proprie credenziali.

- **Link a Pagina del Sito**: consente di creare un collegamento ad una
  specifica pagina interna al sito. E' sufficiente selezionare la pagina
  desiderata dal sottostante albero delle pagine.

- **Link a Lingua**:consente di creare un collegamento alla versione del
  sito nella lingua indicata nel sottostante menu a tendina (un esempio
  un questo senso possono essere le classiche bandierine che consentono
  di passare dalla versione italiana del sito a quella in lingua).
  Richiede, ovviamente che il sito sia stato realizzato in più lingue.

> **ATTENZIONE!** nel caso di siti multilingua la destinazione del
> collegamento dovrà essere impostata per ciascuna delle lingue
> attualmente gestite all'interno del sito e potrebbe anche essere
> diversa da lingua a lingua.
>
> In queste condizioni dunque una il link impostato potrebbe puntare per
> il sito in Italiano ad una certa pagina (pagina A) mentre per il sito
> in Inglese lo stesso link potrebbe puntare ad una pagina diversa dalla
> precedente (pagina B)
>
> Nel caso in cui invece il collegamento dovesse essere lo stesso per
> tutte le lingue gestite il pulsante "**Applica impostazioni Link alle
> altre Lingue**" consente di velocizzare questa configurazione
> assegnando le stesse impostazioni settate per la lingua attualmente
> selezionata a tutte le altre lingue gestite sul sito

- **Link a Prodotto**: consente di creare un collegamento ad una
  specifica pagina prodotto del sito

> Il campo presente in corrispondenza di questo parametro è ad auto
> completamento per cui è sufficiente **digitare le prime lettere del
> titolo o del codice articolo** e selezionare poi, tra quelli presenti
> in elenco, il prodotto verso cui si vuole creare il collegamento.

- **Link a Risorsa**: consente di creare un collegamento ad una
  specifica risorsa del sito (es. file pdf), risorsa questa che potrà
  essere selezionata tra quelle presenti all'interno del proprio
  database cliccando sul pulsante "**Seleziona la risorsa**".

> La risorsa selezionata potrà poi essere scaricata dal front end del
> sito o visualizzata direttamente in una pagina del browser
> dipendentemente dalle impostazioni settate per il successivo parametro
> "**Destinazione del link**"

Il pulsante "**Applica impostazioni Link alle altre Lingue"** consente
di assegnare la destinazione del collegamento, settata per la lingua
attualmente selezionata, anche a tutte le altre lingue gestite sul sito

Indipendentemente dalla tipologia di link che si intende realizzare sarà
poi possibile indicare un valore anche per i seguenti parametri:

**Apri come Finestra Modale**: selezionando questo parametro la pagina
di destinazione del link di collegamento associato all'immagine verrà
aperta sotto forma di Popup. In queste condizioni inoltre il successivo
parametro "Destinazione Link" non verrà preso in considerazione.

Per maggiori informazioni relativamente alla gestione dei Popup si veda
anche la sezione "*Live Editing per Varianti Responsive -- Pagine --
Pagine Popup Creazione e Gestione"* di questo manuale

**Destinazione Link:** consente di indicare dove dovrà essere aperto il
collegamento ipertestuale associato all'immagine in esame. E' possibile
selezionare uno dei seguenti valori:

- **Stessa finestra**: il target del relativo link sarà "**\_self**" e
  quindi il collegamento di destinazione si aprirà nella stessa pagina
  del browser

- **Nuova finestra**: il target del relativo link sarà "**\_blank**" e
  quindi il collegamento di destinazione verrà aperto in una nuova
  pagina web

- **Finestra più esterna**: il target del relativo link sarà "**\_top**"
  (richiede che la pagina sia divisa in differenti framset)

- **Finestra Padre**: il target del relativo link sarà "**\_parent**"
  (richiede che la pagina sia divisa in differenti framset)

- **Download --** da utilizzare nel caso in cui il precedente parametro
  "**Link**" sia stato impostato sull'opzione "Link a risorsa" --
  Consente di effettuare il download della risorsa collegata al link.

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
creare un collegamento ad una risorsa del sito (es. file pdf) che
l'utente dovrà poi scaricare dal front end cliccando sul relativo link,
sarà necessario impostare i due parametri "**link**" e "**Destinazione
link**" rispettivamente sulle opzioni "**Link a Risorsa**" e
"**Download**"

**Relazione tra la pagina ed il link:** consente di impostare un valore
per l'attributo "**rel**" utilizzato nel link associato all'immagine.

L'attributo rel non è utilizzato in alcun modo dai browser; **al
contrario è particolarmente importante per fornire informazioni
aggiuntive ai motori di ricerca in merito al link stesso e alla
relazione che intercorre tra di esso e la pagina o l'elemento di
destinazione.**

Dipendentemente dal tipo di link e, di conseguenza, dal tipo di
informazione che si vuol dare al motore di ricerca, è possibile
impostare uno dei seguenti valori:

- **alternate:** link ad una rappresentazione alternativa della pagina
  attuale

- **bookmark:** permalink al contenuto del contenitore più vicino

- **help:** link ad un documento di aiuto

- **index:** link alla tabella dei contenuti o ad un indice (non alla
  home page del sito)

- **next:** link al documento successivo di una serie

- **prev:** link al documento precedente di una serie

- **stylesheet:** importazione di un foglio di stile

- **archives:** link ad una collezione di documenti o altro materiale
  gestito tramite un archivio

- **author:** link alle informazioni dell'autore del documento

- **external:** link che punta ad una pagina esterna del sito attuale

- **first:** link al primo documento di una serie

- **icon:** importa un'icona che rappresenta una pagina (Favicon)

- **last:** link all'ultimo documento di una serie

- **license:** link alle informazioni relative al copyright di un
  documento

- **nofollow:** indica che l'autore del documento non conferma la
  validità della pagina di destinazione. Questo valore è utilizzato
  anche per indicare agli spider di Google di non seguire il
  collegamento e, conseguentemente, di non visitare la relativa pagina
  di destinazione.

- **noreferrer:** impedisce l'invio del referrer nell' intestazione
  HTTP. Il referrer è utilizzato nei sistemi di statistica per indicare
  da dove proviene la visita ad una certa pagina del sito

- **prefetch:** consente di effettuare il preload del documento linkato
  caricandolo nella cache del browser

- **search:** link ad un documento di tipo Open Search

- **sidebar:** mostra il documento linkato in una sidebar del browser
  (se ne ha una)

- **tag:** indica un tag o una parola chiave applicabile al documento
  corrente

- **up:** link al documento padre del documento attuale

**ATTENZIONE!** Nel caso di siti in multilingua i parametri "**Apri come
Finestra Modale**", "**Destinazione Link**" e "**Relazione tra le pagine
ed il link**" potranno essere configurati in maniera diversa per ogni
singola lingua gestita

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

