# PAGINE E-COMMERCE



Le Pagine E-Commerce, rappresentate all'interno dell'albero da icone con
sfondo verde
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_pagina_ecommerce_res.bmp](./assets/media/image102.png) ), sono pagine fortemente tipizzate e
presenti unicamente nel caso in cui il sito sia collegato a Mexal oppure
ad uno dei gestionali Ho.Re.Ca.

Tali pagine sono collegate a precisi automatismi dell'applicazione e
possono accogliere, in generale, qualsiasi tipo di Componente
(e-commerce e non e-commerce). **Ciò che contraddistingue questa
tipologia di pagina rispetto alle altre è essenzialmente il fatto che
ogni pagina di questo tipo è destinata a contenere uno specifico
Componente E-commerce.**

Facendo riferimento, ad esempio, alla Pagina E-Commerce **"Carrello"**
occorrerà considerare che la destinazione del link **"Vai al Carrello"**
presente all'interno del Componente E-Commerce **"Carrellino"** è
proprio la pagina **"Carrello"** e tale destinazione non è in alcun modo
personalizzabile. Nel caso in cui, dunque, dovesse essere inserito
all'interno del sito il Componente "Carrellino" potrebbe verificarsi una
situazione in cui l'utente, nel processo di generazione dell'ordine,
venga obbligatoriamente ricondotto alla pagina Carrello. In queste
condizioni se non fosse stato inserito all'interno della pagina Carrello
il relativo Componente E-Commerce "Carrello" l'utente non potrebbe,
ovviamente, completare il processo e confermare così il proprio ordine.

Di seguito viene indicato per ciascuna delle pagine E-Commerce lo
specifico Componente che deve obbligatoriamente essere presente
all'interno della pagina stessa.

  ---------------------------------------------------
  **PAGINA E-COMMERCE**    **COMPONENTE
                           OBBLIGATORIO**
  ------------------------ --------------------------
                           

  Profilo Utente           Profilo Utente

  Registrazione Utente     Registrazione Utente

  Negozio                  Catalogo E-Commerce

  Carrello                 Carrello

  Ordine                   Ordine (Checkout)

  Ordini                   Ordini

  Prodotti                 Scheda Prodotto

  Wishlist                 Wishlist

  Reso                     Reso (RMA)

  Gift Card                Gift Card

  Lista Regalo             Lista Regalo

  Punti Premio             Punti Premio
  ---------------------------------------------------

**ATTENZIONE! Per poter garantire il corretto funzionamento
dell'applicazione è necessario che ogni pagina di tipo E-commerce abbia
al suo interno il relativo Componente indicato in tabella**

Nulla vieta comunque di poter inserire alcuni di questi componenti anche
all'interno di altre pagine. Il Componente "Carrellino" potrebbe, ad
esempio, essere inserito anche in una qualsiasi pagina generica.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> dei componenti E-commerce si rimanda ai relativi capitoli di questo
> manuale.
>
> **NOTA BENE:** non è possibile in alcun modo creare o eliminare in
> maniera manuale pagine di tipo E-Commerce. La gestione di tali pagine
> è interamente a carico di Passweb

Selezionando quindi una pagina di tipo E-commerce, all'interno
dell'albero delle pagine, gli unici pulsanti che si abiliteranno nella
barra degli strumenti saranno quelli relativi alle azioni **"Apri"** per
accedere ai contenuti della relativa pagina, e **"Modifica"** per
modificare le proprietà della pagina stessa.

In particolare cliccando sul pulsante **"Modifica"** verrà visualizzata,
sulla parte destra della maschera la sezione **"Modifica Pagina"**
attraverso la quale poter indicare uno specifico valore per i seguenti
campi:

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
  oggetto a livello di gruppi utente potendo quindi decidere quali
  utenti potranno accedere ad essa e quali no.

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
> Protette"** nel corrispondente parametro nella configurazione della
> relativa Variante Sito.
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
  associare alla corrispondente pagina E-commerce, selezionandolo tra
  quelli precedentemente creati.

> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione dei Layout si veda anche la sezione "Live Editing per
> Varianti Responsive -- Layout" di questo manuale.

- **Visibilità pagina:** disponibile solo nel caso in cui sia stato
  attivato il modulo di gestione dell'App mobile.

> Consente di impostare la visibilità della pagina a livello di sito web
> e/o di App mobile. E' possibile selezionare uno dei seguenti valori:

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

In particolare, per quel che riguarda la sezione SEO, il campo:

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

- **Head:** consente di inserire nella sezione \<head\> della pagina,
  dei Meta Tags aggiuntivi, non presenti nativamente in Passweb, e
  relativi quindi a specifiche esigenze dell'utente.

> **ATTENZIONE!** A differenza dei precedenti campi "Keywords" e
> "Description" in cui è necessario inserire solamente il contenuto del
> relativo meta tag (ossia le specifiche keywords e/o la specifica
> description) **all'interno di questo campo occorre inserire invece
> l'intero markup relativo al meta tag che si desidera utilizzare**. Per
> maggiori informazioni in merito si veda anche il capitolo "*Pagine
> Generiche*" di questo manuale.

**ATTENZIONE!** Volendo è anche possibile importare massivamente,
mediante un apposito file csv, i dati presenti all'interno della sezione
SEO per ciascuna delle pagine ecommerce gestite all'interno del sito.
Per maggiori informazioni in merito si veda anche quanto indicato in
corrispondenza del successivo capitolo "*Importazione / Esportazione dei
metadati di pagine generiche e ecommerce*"

I parametri presenti all'interno della sezione **SiteMap** consentono
invece di:

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
> del menu "**Sito -- Preferenze - SEO**" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sitemap_pagine_res.bmp](./assets/media/image112.png)

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

