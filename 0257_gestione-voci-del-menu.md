# GESTIONE VOCI DEL MENU



La sezione **"Gestione Voci"** presente nella maschera di configurazione
di un componente Menu consente di definire e impostare le singole voci
appartenenti al menu stesso

![](./assets/media/image15.png)

Tale sezione risulta quindi suddivisa in due distinte parti:

- nella parte di sinistra viene visualizzato l'albero delle voci del
  menu

- nella parte destra vengono invece visualizzate le proprietà della voce
  attualmente selezionata all'interno dell'albero

I pulsanti presenti nella barra degli strumenti posta immediatamente al
di sopra dell'albero delle voci di menu, consentono rispettivamente di:

**Aggiungi elemento** ( ): consente di aggiungere una nuova voce di menu
immediatamente al di sotto della voce attualmente selezionata
all'interno dell'albero.

> **NOTA BENE:** per creare una voce di livello 1 occorre selezionare
> l'elemento "Radice del Menu" e cliccare sul pulsante "Aggiungi
> elemento"

**Modifica elemento** ( ): consente di visualizzare ed eventualmente
modificare le proprietà della voce di menu attualmente selezionata
all'interno dell'albero.

**Elimina elemento** (
![](./assets/media/image16.png) ): consente di eliminare la voce di menu
attualmente selezionata all'interno dell'albero.

**Sposta elemento** ( ) (
![](./assets/media/image17.png) ): è possibile spostare e riordinare tra
loro le varie voci di menu.

In questo senso i pulsanti raffiguranti due piccole frecce consentono di
spostare la voce attualmente selezionata all'interno dell'albero,
rispettivamente verso l'alto e verso il basso, **mantenendola comunque
sempre allo stesso livello**.

Nel caso in cui l'esigenza sia invece quella di aumentare o diminuire il
livello di una voce di menu sarà necessario per prima cosa selezionare
all'interno dell'albero la voce che si intende spostare, cliccare quindi
sul pulsante raffigurante 4 piccole freccettine ( ) e infine selezionare
la nuova destinazione in cui andare a collocare l'elemento inizialmente
considerato.

Verrà quindi richiesta un'ulteriore conferma relativamente allo
spostamento che si intende effettuare.

![](./assets/media/image18.png)

Cliccando sul pulsante "**Conferma**" lo spostamento sarà definitivo.

Nella parte destra della sezione "**Gestione Voci**" è possibile invece
specificare, per ciascuna delle lingue attualmente gestite, le proprietà
e le caratteristiche di ogni singola voce di menu.

In particolare per ciascuna di esse sarà possibile indicare:

**Testo Voce:** consente di definire l'etichetta della voce di menu in
oggetto.

**Link:** consente di definire il tipo di link che dovrà essere
associato alla voce di menu in oggetto. E' possibile creare:

- dei normali link di navigazione indicando esattamente la pagina di
  destinazione del collegamento

- delle porzioni di menu autogenerate

Nel momento in cui l'esigenza dovesse essere dunque quella di creare un
normale link di collegamento ad una pagina interna o esterna al sito
sarà necessario impostare il parametro "**Link**" sull'opzione "**Crea
un Link**"

![](./assets/media/image19.png)

In queste condizioni sarà poi necessario specificare un valore anche per
i seguenti parametri:

- **Link a pagina esterna / Link all'Area Riservata**: consente di
  indicare la pagina di destinazione del link.

> E' possibile digitare esplicitamente l' url della pagina che si vuole
> raggiungere (es. <http://www.google.it>).
>
> **ATTENZIONE!** Per creare il collegamento ad una pagina esterna è
> necessario indicare il percorso assoluto del link (nella forma
> http://www.indirizzosito.it)
>
> Nel momento in cui l'esigenza dovesse essere invece quella di creare
> un collegamento ad una delle diverse sezioni dell'Area Riservata del
> proprio sito sarà necessario selezionare tale sezione dal relativo
> menu a tendina

![](./assets/media/image20.png)

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

- **Link a Pagina del Sito:** consente di creare un collegamento ad una
  pagina del proprio sito. E' sufficiente selezionare la pagina
  desiderata all'interno del sottostante albero delle pagine.

- **Link a Lingua:** nel caso di siti in multilingua consente di creare
  un collegamento per gestire il passaggio alla visualizzazione del sito
  nella versione in lingua desiderata (un tipico esempio in questo senso
  è l'icona a forma di bandiera per passare alle versione tradotta di un
  sito vetrina/hotel, ecc...)

> **ATTENZIONE!** nel caso di siti multilingua la destinazione del
> collegamento dovrà essere impostata per ciascuna delle lingue
> attualmente gestite all'interno del sito e potrebbe anche essere
> diversa da lingua a lingua.
>
> In queste condizioni dunque una stessa voce di menu potrebbe puntare
> per il sito in Italiano ad una certa pagina (pagina A) mentre per il
> sito in Inglese la stessa voce potrebbe puntare ad una pagina diversa
> dalla precedente (pagina B)
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

Nel momento in cui l'esigenza dovesse invece essere quella di creare una
porzioni di menu autogenerata, sarà necessario impostare il parametro
"**Link**" sull'opzione "**Crea una porzione di menu autogenerata**"

![](./assets/media/image21.png)

In questo modo l'applicazione non si limiterà a creare una singola voce
di menu, ma si preoccuperà di replicare in maniera completamente
automatica l'intera struttura dell'albero delle pagine a partire dalla
voce selezionata all'interno della sezione "**Voce del Menu -- Ramo
Autogenerato**"

![](./assets/media/image22.png)

In queste stesse condizioni sarà inoltre possibile indicare un valore
anche per i seguenti parametri:

- **Utilizza il nome dell'elemento linkato:** consente di utilizzare il
  nome di ogni singola pagina come etichetta delle varie voci di menu
  autogenerate

- **Includi solo le pagine di Categoria (presente solo per siti
  Ecommerce):** permette, se selezionato, di includere nell'elenco delle
  voci autogenerate solo ed esclusivamente le pagine di categoria.

> Tale parametro risulta quindi particolarmente utile nel momento in cui
> dovesse essere utilizzata come radice dell'autogenerazione la pagina
> "Catalogo".
>
> In queste condizioni sarà infatti possibile, selezionando il parametro
> in oggetto, escludere dall'elenco delle voci autogenerate pagine quali
> "Carrello", "Ordine" ,"Ordini" ecc... pagine queste che, a livello
> gerarchico sono collocate proprio sotto la pagina Catalogo, ottenendo
> così un vero e proprio menu di categoria articoli.

- **Nascondi le Categorie che non hanno articoli associati (presente
  solo per siti Ecommerce):** permette, se selezionato, di escludere
  dall'elenco delle voci autogenerate, le pagine di categoria che non
  hanno articoli associati.

- **Profondità:** consente di impostare il livello di profondità per la
  visualizzazione delle voci di menu autogenerate. Impostando ad esempio
  questo campo sul valore 3 verranno visualizzate le voci di primo
  secondo e terzo livello (a partire dalla voce selezionata all'interno
  dell'albero delle pagine).

**ATTENZIONE!** Per porzioni di menu autogenerate non è possibile
differenziare il link di collegamento in base alla lingua. Se l'esigenza
dovesse essere questa sarà quindi necessario creare e mappare delle voci
di menu singole

Infine, indipendentemente dal fatto di creare singole voci di menu,
indicando esplicitamente la pagina di destinazione del collegamento, o
porzioni di menu autogenerate, i restanti parametri presenti all'interno
di questa maschera consentiranno rispettivamente di:

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

La sezione "**Voce del Menu -- Personalizzazioni grafiche**" consente di
gestire, per ciascuna delle lingue attualmente presenti sul sito, le
immagini eventualmente associate alla varie voci di menu

![](./assets/media/image23.png)

In particolare il campo:

- **Immagine Voce:** immagine che verrà visualizzata in corrispondenza
  della voce di menu. Può essere utilizzata una risorsa caricata su
  Passweb premendo su 'Cambia Risorsa'

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.

- **Immagine Voce (Rollover)**: immagine che verrà visualizzata al
  passaggio del mouse sulla voce di menu. Può eventualmente essere
  utilizzata un' immagine differente rispetto a quella utilizzata per il
  campo "Immagine Voce"

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.

- **Immagine Voce Attiva:** immagine che verrà visualizzata in
  corrispondenza della voce di menu quando sarà attiva la relativa
  pagina web. Può eventualmente essere utilizzata un' immagine
  differente rispetto a quella utilizzata per i precedenti campi

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.
>
> **ATTENZIONE!** Il pulsante "**Applica impostazione Immagine alle
> altre Lingue**", presente in corrispondenza di ciascuno dei campi
> sopra indicati, consente di utilizzare automaticamente l'immagine
> indicata per tutte le lingue attualmente gestite all'interno del sito

- **Testo Alternativo (accessibilità):** consente di impostare un testo
  alternativo per la voce di menu in oggetto. Nello specifico quanto
  indicato all'interno di questo campo verrà poi utilizzato come valore
  dell'attributo **title** per il link associato alla voce di menu.

- **Larghezza (px):** nel caso si vogliano impostare le voci di menù con
  dimensioni differenti, in questo campo è possibile definire la
  larghezza in pixel specifica

- **Altezza (px):** altezza della voce di menù specifica

- **Larghezza Rollover (px):** è la larghezza della voce al passaggio
  del mouse

- **Altezza Rollover (px):** opzionale, è l'altezza della voce al
  passaggio del mouse

- **Visualizza il Testo della Voce:** molto importante attivare questo
  campo se, ad esempio, è stata selezionata una immagine di 'sfondo'
  come voce di menù, in questo modo il contenuto testuale della voce può
  essere letto dai motori di ricerca.

<!-- -->

- **Apri come Finestra Modale:** consente di gestire il collegamento del
  link come un pop up. Selezionando questo parametro infatti, la pagina
  di destinazione del link associato alla voce di menu verrà aperta
  all'interno di un'apposita finestra modale.

> **ATTENZIONE!** In queste condizioni inoltre il parametro
> "Destinazione Link" non verrà preso in considerazione.
>
> Per maggiori informazioni relativamente alla gestione dei Popup si
> veda anche la sezione "*Live Editing per Varianti Responsive -- Pagine
> -- Pagine Popup Creazione e Gestione*" di questo manuale

- **Classi Addizionali Contenitore Link:** consente di impostare una o
  più classi css personalizzate che verranno associate al contenitore
  della relativa voce di menu.

> Nello specifico, considerando che il markup di ogni voce di menu è del
> tipo
>
> \<li id=\"menu_entry_29514_2255\"
> class=\"**classi-personalizzate**\"\>
>
> \<a href=\"/chi-siamo\" target=\"\_self\" \>Chi Siamo\</a\>
>
> \</li\>
>
> le classi personalizzate aggiunte mediante il parametro in oggetto
> verranno associate al tag \< li \>.

**ATTENZIONE!** Dopo aver creato/modificato una voce di menu sarà
necessario cliccare sul pulsante **"Aggiungi/Modifica Elemento",**
presente nella parte alta della maschera, per aggiungere la voce stessa
al menu che si sta realizzando.

Una volta create ed aggiunte al menu tutte le voci desiderate, il
pulsante **"Salva"** consentirà di salvare il Componente in oggetto.

> **NOTA BENE:** per i siti E-Commerce è possibile creare menu misti
> costituiti da voci che consentono di navigare tra le varie pagine del
> sito e da voci che consentono invece di navigare fra i vari articoli
> presenti in catalogo.

