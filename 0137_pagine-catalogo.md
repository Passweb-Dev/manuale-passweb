# PAGINE CATALOGO



Le Pagine Catalogo, rappresentate all'interno dell'albero da icone con
sfondo azzurro chiaro
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_pagina_cat_articoli_res.bmp](./assets/media/image103.png){width="0.8097222222222222in"
height="0.1597222222222222in"} ), sono pagine fortemente tipizzate,
presenti unicamente nel caso in cui il sito sia collegato a Mexal o ad
uno dei gestionali Ho.Re.Ca. e nel caso in cui siano state codificate in
maniera corretta, all'interno del gestionale, delle categorie
merceologiche.

**Ciò che contraddistingue infatti questa tipologia di pagina rispetto
alle altre è proprio il fatto che ad ognuna di esse corrisponde una ben
precisa categoria merceologica codificata all'interno del gestionale.**

Per maggiori informazioni relativamente a come la gestione delle
categorie merceologiche possa riflettersi in Passweb, si veda anche il
capitolo *"Catalogo - Classificazione Articoli sulla base dei Gruppi
Merceologici Mexal / Ho.Re.Ca."* di questo manuale.

Al pari delle pagine di tipo E-Commerce, inoltre, anche **le pagine di
tipo "Catalogo" sono collegate a precisi automatismi dell'applicazione e
per poter funzionare in maniera corretta è obbligatorio inserire al loro
interno uno specifico componete E-Commerce rappresentato, nello
specifico, dal Componente "Catalogo E-Commerce".**

Ad ogni pagina di tipo "Catalogo" è infatti associato (in maniera
completamente automatica) anche uno specifico filtro **che consente di
visualizzare all'interno di quella pagina i soli articoli associati alla
corrispondente categoria merceologica** (per questo, dunque, è
obbligatorio inserire all'interno di queste pagine il Componente
Catalogo E-Commerce)

La radice di tutta questa struttura è rappresentata dalla pagina
**"Negozio**" che, volendo, può essere considerata dunque sia una pagina
di tipo **"E-Commerce"** che una pagina di tipo **"Catalogo".**

> **NOTA BENE:** la pagina Negozio è la radice di tutte le pagine di
> tipo "Catalogo" e consente di visualizzare al suo interno tutti gli
> articoli gestiti sul sito indipendentemente dalla specifica categoria
> merceologica.

E' chiaro dunque che la creazione e/o l'eliminazione di queste pagine è
interamente a carico del gestionale. **Non è possibile in alcun modo
creare o eliminare direttamente da Passweb, in maniera manuale, pagine
di tipo** **"Catalogo".** Per poter fare questo tipo di operazioni
occorre necessariamente operare direttamente all'interno del gestionale
creando o eliminando le relative categorie merceologiche.

> **NOTA BENE:** per creare una nuova pagina di tipo "Catalogo" è
> necessario innanzitutto definire all'interno del gestionale la
> relativa categoria Merceologica. Allo stesso modo per poter eliminare
> una pagina di tipo "Catalogo" occorre innanzitutto eliminare dal
> gestionale la corrispondente categoria merceologica.

Una volta apportate le varie **modifiche all'interno del gestionale sarà
necessario lanciare una sincronizzazione per consentire a Passweb di
leggere la nuova struttura delle categorie merceologiche** e aggiornare
di conseguenza la struttura delle pagine Catalogo presenti sul sito e
dei menu di categoria da esse generati.

Selezionando una pagina di tipo **"Catalogo"**, all'interno dell'albero
delle pagine, gli unici pulsanti che si abiliteranno nella barra degli
strumenti saranno quelli relativi alle azioni **"Apri"** per accedere ai
contenuti della relativa pagina, e **"Modifica"** per modificare le
proprietà della pagina stessa.

In particolare cliccando sul pulsante **"Modifica"** verrà visualizzata,
sulla parte destra della maschera, la sezione **"Modifica Pagina"**
attraverso la quale poter indicare uno specifico valore per i seguenti
campi:

- **Nome Pagina:** consente visualizzare in tutte le lingue gestite
  all'interno del sito, l'etichetta identificativa del nome della pagina
  e della corrispondente categoria merceologica. Il valore di questo
  campo corrispondente alla lingua Italiana, inizialmente, è prelevato
  direttamente dal campo "**Descrizione**" della maschera "**Anagrafica
  gruppo merceologico**" del gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\anagrafica_gruppo_merceologico.bmp](./assets/media/image113.png){width="3.6381944444444443in"
height="2.097916666666667in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_anagrafica_gruppo_merceologico2.bmp](./assets/media/image114.png){width="5.398611111111111in"
height="3.99375in"}

> Tale valore può poi essere modificato e gestito anche all'interno del
> Wizard di Passweb.
>
> **NOTA BENE:** a differenza del valore in italiano, il "Nome Pagina"
> in lingua può essere gestito e variato solo ed esclusivamente
> all'interno del Wizard di Passweb
>
> Per maggiori informazioni in merito a come gestire, all'interno di
> Passweb, il "Nome Pagina" delle Pagine Catalogo si veda anche la
> sezione *"Catalogo -- Gestione Articoli -- Categorie Merceologiche"*
> di questo manuale

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
> pagina impostata come "Pagina di destinazione per le Pagine Protette"
> nel corrispondente parametro presente nella configurazione della
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
  associare alla corrispondente pagina Catalogo, selezionandolo tra
  quelli precedentemente creati.

> **In questo senso dunque Passweb offre la possibilità di creare
> gestire per ogni singola pagina Catalogo un diverso layout grafico**
>
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

All'interno delle sezioni **SEO** è possibile visualizzare il contenuto
dei campi **Title, Keywords, Description, Head** attualmente assegnati
alla relativa Pagina Catalogo, in tutte le lingue di gestione del sito

**ATTENZIONE!** Per le pagine di tipo Catalogo i dati presenti
all'interno di questa sezione sono dati in sola visualizzazione. Nel
momento in cui l'esigenza dovesse essere dunque quella di modificare
questo tipo di informazioni sarà necessario agire all'interno della
corrispondente sezione del Wizard ("*Modifica Categoria Articolo -- SEO
SiteMap*")

All'interno della sezione **SiteMap** invece è possibile visualizzare
quelli che sono i parametri attualmente impostati per la Pagina Catalogo
in relazione alla gestione di questa stessa pagina all'interno della
SiteMap del sito

**ATTENZIONE!** **A differenza di quanto avveniva, ad esempio, per le
Pagine Generiche non è possibile, per le Pagine Catalogo, modificare il
valore dei parametri presenti all'interno delle sezioni Seo e SiteMap
agendo direttamente dalle proprietà della pagina stessa**

Per poter gestire tali parametri occorre agire necessariamente
all'interno dell'Anagrafica Passweb delle rispettive Categorie
Merceologiche. Per maggiori informazioni in merito si veda anche la
sezione "*Catalogo -- Gestione Articoli -- Articoli -- Categorie
Merceologiche*" di questo manuale.

Una volta impostati questi parametri il pulsante **"Salva"** presente
nella parte bassa della maschera confermerà le variazioni eventualmente
apportate.

