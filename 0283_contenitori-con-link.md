# CONTENITORI CON LINK



Nel caso in cui l'esigenza dovesse essere quella di associare ad un
componente Contenitore e a tutto il suo contenuto uno stesso link sarà
sufficiente selezionare il relativo parametro presente nella maschera di
configurazione del Contenitore stesso.

![](./assets/media/image99.png)

**Abilita Link sul contenitore:** consente, se selezionato, di associare
al Contenitore e a tutto il suo contenuto uno specifico link.

Una volta selezionato questo parametro sarà poi necessario definire la
tipologia di link che si intende realizzare e impostare tutti i
parametri di configurazione richiesti da questo stesso link.

Nello specifico dunque il parametro:

**Mappa un link:** consente di definire la tipologia di link che si
intende realizzare. E' possibile selezionare uno dei seguenti valori:

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
>
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

**ATTENZIONE! Nel momento in cui si dovesse decidere di associare al
Contenitore uno specifico link sarà necessario considerare alcune cose
di fondamentale importanza. Nello specifico:**

- Come già avviene per le immagini e per le voci di menu anche in questo
  caso la destinazione del link associato al componente dovrà essere
  definita e configurata per tutte le lingue attualmente gestite
  all'interno del sito.

> Volendo si potrebbe anche pensare dunque di puntare il link, per la
> lingua italiana verso una certa pagina del sito (pagina A) e per la
> lingua inglese verso una pagina diversa dalla precedente (pagina B)

- Associando un link ad un Contenitore questo stesso Contenitore non
  potrà, ovviamente, essere gestito ne in modalità Offcanvas ne tanto
  meno in modalità Collassabile

- Associando un link ad un Contenitore, questo stesso link varrà anche
  per tutti i contenuti interni al Contenitore stesso. In queste
  condizioni dunque non avrebbe alcun senso inserire all'interno del
  Contenitore altri link (magari anche diversi da quello associato al
  Contenitore stesso) anche e soprattutto perché oltre a non aver senso
  un'operazione del genere potrebbe compromettere il funzionamento
  dell'interno componente con tutti ciò che ne consegue a livello di
  markup della pagina web

