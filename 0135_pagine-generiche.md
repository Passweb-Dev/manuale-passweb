# PAGINE GENERICHE



Le Pagine Generiche, rappresentate all'interno dell'albero da icone con
sfondo bianco
(![](./assets/media/image101.png) ), sono pagine NON tipizzate, alle quali
non è collegato alcun automatismo dell'applicazione e adatte dunque ad
accogliere un qualsiasi Componente (e-commerce e non e-commerce).

> **NOTA BENE:** le pagine generiche sono le uniche a poter essere
> spostate secondo le specifiche esigenze dell'utente

Tali pagine, generalmente impiegate per realizzare la parte vetrina del
sito ("Home" "Chi Siamo" "Come Contattarci" ecc ...), possono essere
create e/o eliminate in maniera manuale dai vari utenti, in relazione
sempre a quelli che sono gli specifici permessi ad essi associati.

In ogni caso comunque tali pagine **non possono essere create in una
qualsiasi posizione all'interno dell'albero**.

**In particolare non sarà possibile creare una nuova Pagine Generica ne
tanto meno spostare una pagina già esistente al di sotto di pagine di
tipo "E-commerce", di tipo "Catalogo" o di tipo "Prodotto".**

Per poter creare una nuova Pagina Generica sarà quindi necessario, per
prima cosa, selezionare all'interno dell'albero delle pagine quella al
di sotto della quale dovrà essere creata la nuova pagina e,
successivamente, cliccare sul pulsante **Nuova**
(![](./assets/media/image93.png) ) presente nella barra degli strumenti.

Prima di confermare la creazione della nuova pagina occorrerà impostare
in maniera corretta i parametri relativi alle proprietà della pagina
stessa (sezione "**Nuova Pagina**")

![](./assets/media/image107.png)

In particolare dunque il campo:

- **Nome Pagina (campo obbligatorio):** consente di specificare, in
  ciascuna delle lingue gestite all'interno del sito, il nome della
  pagina che si sta realizzando. **Non è possibile utilizzare lo stesso
  "Nome Pagina" per lingue diverse.**

<!-- -->

- **Pagina Pubblica:** consente di impostare la visibilità della pagina
  lato sito web.

> Se selezionato la corrispondente pagina verrà correttamente pubblicata
> e visualizzata all'interno del sito.
>
> Nel caso in cui invece tale parametro non sia stato selezionato, la
> corrispondente pagina passerà in modalità "**Offline**", sarà quindi
> visibile all'interno del Wizard, dove potrà essere normalmente gestita
> ed editata, ma non verrà pubblicata e visualizzata all'interno del
> sito.
>
> In queste condizioni nel caso in cui un utente tenti di visitare
> questa pagina verrà automaticamente ridiretto alla pagina impostata
> come **"Pagina non esistente"** nel corrispondente parametro presente
> nella configurazione della relativa Variante Sito.

- **Visibile da:** consente di impostare la visibilità della pagina in
  oggetto a livello di gruppi utente decidendo dunque quali utenti
  potranno effettivamente accedere ad essa e quali no.

![](./assets/media/image108.png)

> Impostando questo parametro sul valore **"Tutti"** la pagina sarà
> visibile ed accessibile a tutti i visitatori del sito.
>
> Impostando invece il parametro sul valore **"Solo i gruppi
> Specificati"** verranno visualizzati tutti i gruppi utente
> appositamente creati all'interno della corrispondente sezione "*Utenti
> -- Gruppi Utenti Sito*" del Wizard. **In queste condizioni la pagina
> in oggetto potrà quindi essere accessibile ai soli utenti appartenenti
> ai gruppi selezionati**. Nel caso in cui un utente non abilitato tenti
> di accedere a questa pagina verrà automaticamente ridiretto alla
> pagina impostata come "**Pagina di destinazione per le Pagine
> Protette"** nel corrispondente parametro presente nella configurazione
> della relativa Variante Sito.
>
> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> dei Gruppi Utente si veda la corrispondente sezione "Utenti -- Gruppi
> Utenti Sito" di questo manuale.

- **Briciole di Pane:** consente di indicare se la pagina in oggetto
  dovrà o meno essere inserita nelle Briciole di Pane.

> Per maggiori informazioni relativamente alle "Briciole di Pane" si
> veda anche il capitolo "*Live Editing -- Lista Componenti Comuni --
> Componente Info Navigazione*" di questo manuale.
>
> **ATTENZIONE!** Le pagine non pubbliche non verranno mai considerate
> nella generazione delle Briciole di Pane indipendentemente da quanto
> impostato per il parametro in oggetto.

- **Feed Associati:** consente di selezionare uno o più Feed RSS tra
  quelli creati all'interno della corrispondente sezione del Wizard da
  poter esporre attraverso la pagina web in esame.

> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione dei Feed RSS si veda la corrispondente sezione di
> questo manuale ("Sito -- Gestione CMS -- Feeds").

- **Layout Associato:** consente di selezionare lo specifico layout da
  associare alla pagina che si sta realizzando, selezionandolo tra
  quelli precedentemente creati.

![](./assets/media/image109.png)

> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione dei Layout si veda anche la sezione "Live Editing per
> Varianti Responsive -- Layout" di questo manuale.

- **Utilizza come Popup:** permette di utilizzare la Pagina come Popup.

> **ATTENZIONE!** Se impostata come Popup la Pagina non sarà
> raggiungibile dal suo percorso Web, ma potrà essere richiamata sotto
> forma di Popup dai link che permettono di visualizzare questo tipo di
> elementi.
>
> **NOTA BENE:** per maggiori informazioni relativamente a come --creare
> o richiamare una pagina di tipo Popup si veda la corrispondente
> sezione di questo manuale

- **Visibilità pagina:** disponibile solo nel caso in cui sia stato
  attivato il modulo di gestione dell'App mobile.

> Consente di impostare la visibilità della pagina a livello di Sito Web
> e/o di App Mobile. E' possibile selezionare uno dei seguenti valori:

- **Sia sito che app:** selezionando questa opzione la pagina in esame
  sarà visibile sia all'interno del sito sia all'interno dell'app mobile
  originata a partire dal sito stesso

- **Solo sito:** selezionando questa opzione la pagina in esame sarà
  visibile solo ed esclusivamente all'interno del sito web

- **Solo app:** selezionando questa opzione la pagina in esame sarà
  visibile solo ed esclusivamente all'interno dell'app mobile

> **ATTENZIONE! Le pagine destinate unicamente all'App Mobile non
> verranno inserite, ovviamente, nella sitemap del sito**

Le sezioni **SEO** e **SiteMap** consentono, rispettivamente, di gestire
i parametri necessari per una corretta indicizzazione della pagina e
quelli attraverso cui poter decidere se la pagina stessa dovrà o meno
comparire all'interno della SiteMap del sito, ed eventualmente, con che
priorità e con che frequenza di aggiornamento.

![](./assets/media/image110.png)

In particolare, per quel che riguarda la sezione **SEO**, il campo:

- **Titolo Pagina:** consente di indicare, in ciascuna delle lingue
  gestite all'interno del sito, uno specifico titolo per la pagina che
  si sta realizzando. Tale valore potrà poi essere utilizzato, a livello
  HTML, per generare il \<Title\> della relativa pagina e sarà quindi di
  fondamentale importanza per una corretta indicizzazione del sito.

> Nello specifico quanto inserito all'interno di questo campo verrà poi
> utilizzato per valorizzare il segnaposto {pageName} utilizzato nella
> definizione del Title stabilita per la tipologia di pagina
> considerata.
>
> **NOTA BENE:** nel caso in cui il parametro in oggetto non venga
> valorizzato, il segnaposto {pageName} utilizzato nella definizione del
> Title stabilita per la tipologia di pagina considerata, verrà
> valorizzato con quanto inserito all'interno del precedente campo "Nome
> Pagina".
>
> Per maggiori informazioni relativamente alla gestione e alla
> definizione dei Title da generare per le diverse tipologie di pagina,
> si veda anche la sezione *"Sito -- Preferenze"* di questo manuale

- **Keywords:** consente di specificare, per ciascuna delle lingue
  gestite all'interno del sito le parole chiave (corrispondenti al
  contenuto del Meta tag HTML KEYWORDS) associate alla pagina che si sta
  realizzando e che verranno utilizzate per fornire informazioni
  relative a questa stessa pagina agli utenti o ai motori di ricerca.
  Tali informazioni saranno quindi di fondamentale importanza per una
  corretta indicizzazione del sito.

- **Description:** consente di specificare, per ciascuna delle lingue
  gestite all'interno del sito la descrizione (corrispondente al
  contenuto del Meta tag HTML DESCRIPTION) associata alla pagina che si
  sta realizzando e che verrà utilizzata per fornire informazioni
  relative a questa stessa pagina agli utenti o ai motori di ricerca.
  Tali informazioni saranno quindi di fondamentale importanza per una
  corretta indicizzazione del sito.

- **Head:** consente di inserire nella sezione \< head \> della pagina,
  dei Meta Tags aggiuntivi, non presenti nativamente in Passweb, e
  relativi quindi a specifiche esigenze dell'utente.

> **ATTENZIONE!** A differenza dei precedenti campi "Keywords" e
> "Description" in cui è necessario inserire solamente il contenuto del
> relativo meta tag (ossia le specifiche keywords e/o la specifica
> description) **all'interno di questo campo occorre inserire invece
> l'intero markup relativo al meta tag che si desidera utilizzare.**
>
> Il pulsante **"Seleziona un segnaposto"** consente di inserire, nella
> definizione del meta tag, dei segnaposto che verranno poi valorizzati
> automaticamente da Passweb.
>
> Sono gestiti i seguenti segnaposto:

- **Url sito:** il segnaposto verrà sostituito a runtime con il domino
  del sito (es. www.miosito.it)

- **Url pagina:** il segnaposto verrà sostituito a runtime con l' url
  della relativa pagina web, esclusi eventuali parametri di query string
  (es. www.miosito.it\\catalogo-articoli)

- **Url pagina completo della stringa di Query:** il segnaposto verrà
  sostituito a runtime con l' url competo della relativa pagina web (es.
  www.miosito/cms/blog/dettaglio-post?a=phasellus-fringilla)

- **Titolo Pagina:** il segnaposto verrà sostituito a runtime con lo
  stesso valore utilizzato per il meta tag \< title \>

> Per inserire un nuovo segnaposto è sufficiente posizionare il cursore
> nella posizione in cui questo dovrà essere effettivamente inserito,
> cliccare sul pulsante "Aggiungi segnaposto" e selezionare dal relativo
> menu contestuale la tipologia di segnaposto da inserire.
>
> **NOTA BENE:** oltre che a livello di singola pagina i Meta Tag
> possono essere aggiunti e gestiti anche a livello di Layout Sito. Per
> maggiori informazioni in merito si veda anche la sezione "Live Editing
> -- Layout" di questo manuale
>
> **Esempio**
>
> Questo campo può essere particolarmente utile per gestire i problemi
> di penalizzazione da parte dei motori di ricerca legati a contenuti
> duplicati presenti all'interno del nostro sito, problema questo che si
> potrebbe risolvere utilizzando, appunto, il meta tag "**canonical**".
>
> I motori di ricerca analizzano sommariamente il contenuto di una
> pagina calcolando la percentuale di testo simile alle altre pagine e
> penalizzano, in fase di indicizzazione, le pagine con contenuti
> duplicati; inoltre se la duplicazione è molto estesa all'interno del
> dominio potrebbe anche essere penalizzato l'intero sito.
>
> Una buona norma da prendere sempre in considerazione dunque, consiste
> nel diversificare i contenuti del proprio sito evitando di avere più
> pagine diverse con lo stesso contenuto.
>
> Va anche detto però che in determinati casi non è possibile evitare
> questi problemi. Ad esempio potrebbe esserci la necessità di gestire
> sul proprio sito il dominio con e senza il www (es. miosito.com e
> www.miosito.com). Per Passweb, inoltre la home page del sito è
> richiamabile sia come www.miosito.com sia come www.miosito.com/home
> (posto, ovviamente, di aver assegnato "home" come nome a tale pagina).
> Per gli spider dei motori di ricerca che passano ad analizzare i
> contenuti del nostro sito gli indirizzi miosito.com, www.miosito.com,
> miosito.com/home e www.miosito.com/home corrispondono sempre e
> comunque a quattro pagine diverse tutte esattamente con lo stesso
> contenuto, e in conseguenza di ciò, potrebbero portare, in fase di
> indicizzazione della pagina ad alcune penalizzazioni.
>
> Per risolvere questo problema è necessario indicare allo spider quale
> dei 4 sopra indicati dovrà essere considerato come l' url predefinito
> e, dunque, l'unico ad essere indicizzato. Questo lo si fa utilizzando
> il meta tag canonical che va inserito nella sezione \<head\> della
> pagina.
>
> E' quindi sufficiente inserire nel campo in oggetto, per la pagina
> home, la seguente stringa
>
> **\<link rel=\"canonical\" href=\"http://www.miosito.com\" /\>**
>
> dove, ovviamente, www.miosito.com è quello che abbiamo scelto come url
> predefinito.

**ATTENZIONE!** Volendo è anche possibile importare massivamente,
mediante un apposito file csv, i dati presenti all'interno della sezione
SEO per ciascuna delle pagine generiche gestite all'interno del sito.
Per maggiori informazioni in merito si veda anche quanto indicato in
corrispondenza del successivo capitolo "*Importazione / Esportazione dei
metadati di pagine generiche e ecommerce*"

I parametri presenti all'interno della sezione **SiteMap** consentono
invece di:

![](./assets/media/image111.png)

- **SiteMap:** consente di decidere se la pagina in oggetto dovrà o meno
  essere inclusa nella SiteMap del sito generata dinamicamente
  dall'applicazione.

> **ATTENZIONE! Le pagine destinate unicamente all'App Mobile non
> verranno inserite, ovviamente, nella sitemap del sito**

- **ChangeFrequency:** consente di impostare, per la pagina in oggetto,
  il valore del campo della SiteMap utilizzato per informare il motore
  di ricerca relativamente alla frequenza di aggiornamento dei contenuti
  della pagina stessa.

- **Priority:** consente di impostare, per la pagina in oggetto, il
  valore del campo della SiteMap utilizzato per informare il motore di
  ricerca relativamente alla priorità assegnata ai contenuti della
  pagina stessa.

> **ATTENZIONE!** Nel caso in cui per i tre parametri sopra indicati non
> sia stato specificato alcun valore, verrà considerato il valore
> assegnato, allo stesso parametro, nella sezione "**SiteMap Pagine**"
> del menu "**Sito -- Preferenze -- SEO**" del Wizard

![](./assets/media/image112.png)

> **Nel caso in cui i parametri in esame non siano stati opportunamente
> valorizzati neppure all'interno del menu "Sito -- Preferenze - SEO"
> del Wizard, la pagina in oggetto sarà sempre inserita nella SiteMap
> con le seguenti impostazioni: "ChangeFrequency = Settimanale" e
> "Priority = 0.8"**
>
> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> della SiteMap del sito si veda anche la sezione "Sito -- Preferenze --
> SiteMap Pagine" di questo manuale.

Una volta impostati questi parametri il pulsante **"Salva"** presente
nella parte bassa della maschera confermerà le variazioni eventualmente
apportate.

