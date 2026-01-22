# PAGINE PRODOTTO



Come precedentemente evidenziato all'interno di Passweb ad ogni singola
pagina Catalogo, e conseguentemente ad ogni singola categoria
Merceologica, corrisponde una specifica "**Pagina Prodotto**",
evidenziata in rosso all'interno dell'albero
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_pagina_prodotto_res.bmp](./assets/media/image104.png) ).

Come per le pagine Catalogo dunque anche le Pagine Prodotto sono pagine
fortemente tipizzate, presenti unicamente nel caso in cui il sito sia
collegato a Mexal oppure ad uno dei gestionali Ho.Re.Ca. e nel caso in
cui siano state codificate in maniera corretta, all'interno del
gestionale, delle categorie merceologiche.

E' chiaro dunque che anche in questo caso la creazione e/o
l'eliminazione di queste pagine è interamente a carico del gestionale.
**Non è possibile in alcun modo creare o eliminare direttamente da
Passweb, in maniera manuale, pagine di tipo** **"Prodotto".** Per poter
fare questo tipo di operazioni occorre necessariamente operare
direttamente all'interno del gestionale creando o eliminando le relative
categorie merceologiche.

> **NOTA BENE:** per creare una nuova pagina di tipo "Prodotto" è
> necessario, innanzitutto, creare all'interno del gestionale la
> relativa categoria Merceologica. Allo stesso modo per poter eliminare
> una pagina di tipo "Prodotto" occorre innanzitutto eliminare sul
> gestionale la corrispondente categoria merceologica.

Una volta apportate le varie **modifiche all'interno del gestionale sarà
necessario lanciare una sincronizzazione per consentire a Passweb di
leggere la nuova struttura delle categorie merceologiche** e aggiornare
di conseguenza la struttura delle pagine Prodotto presenti all'interno
del sito.

Alla sincronizzazione l'applicazione si preoccuperà quindi di creare,
per ciascuna delle categorie merceologiche presenti all'interno del
gestionale, oltre alla corrispondente Pagina Catalogo, anche una
corrispondente Pagina Prodotto.

**Lo scopo di queste Pagine Prodotto sarà essenzialmente quello di
offrire all'utente la possibilità di creare schede prodotto differenti a
seconda della categoria merceologica associata all'articolo che si sta
visualizzando.**

Ad ognuna di queste pagine prodotto sarà infatti possibile associare uno
specifico layout e diversi componenti in modo tale dunque da poter
facilmente arrivare a realizzare, ad esempio, per i prodotti della
categoria merceologica "Televisori" una certa pagina prodotto con uno
specifico layout e certi componenti e per i prodotti della categoria
merceologica "Computer" un'altra pagina prodotto differente dalla
precedente e quindi con un diverso layout e diversi componenti.

A livello di navigazione del sito nel caso in cui l'utente selezioni
all'interno del catalogo un articolo non associato a nessuna categoria
merceologica verrà ricondotto alla pagina prodotto generica,
contestualizzata ovviamente sullo specifico articolo, ma con il layout e
i componenti presenti all'interno della pagina prodotto generica.

Nel caso invece in cui dovesse essere selezionato un articolo
appartenente ad una specifica categoria merceologica l'utente verrà
ricondotto alla pagina prodotto creata per quella specifica categoria
merceologica, contestualizzata anche in questo caso sullo specifico
articolo, ma con il layout e i componenti inseriti nella specifica
pagina prodotto.

Come per le pagine Catalogo, anche in questo caso, selezionando una
pagina di tipo **"Prodotto"**, all'interno dell'albero delle pagine, gli
unici pulsanti che si abiliteranno nella barra degli strumenti saranno
quelli relativi alle azioni **"Apri"** per accedere ai contenuti della
relativa pagina, e **"Modifica"** per modificare le proprietà della
pagina stessa.

In particolare cliccando sul pulsante **"Modifica"** verrà visualizzata,
sulla parte destra della maschera, la sezione **"Modifica Pagina"**
attraverso la quale poter indicare uno specifico valore per i seguenti
campi:

- **Nome Pagina:** consente di visualizzare, in tutte le lingue gestite
  all'interno del sito, l'etichetta identificativa del nome della
  pagina.

> **NOTA BENE:** il "Nome Pagina" delle Pagine Prodotto è esattamente lo
> stesso di quello definito per la corrispondente "Pagina Catalogo"

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
  associare alla corrispondente pagina Prodotto, selezionandolo tra
  quelli precedentemente creati.

> **In questo senso dunque Passweb offre la possibilità di creare
> gestire per ogni singola pagina Prodotto un diverso layout grafico**
>
> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione dei Layout si veda anche la sezione "Live Editing per
> Varianti Responsive-- Layout" di questo manuale.
>
> Si potrebbe quindi pensare, ad esempio, di utilizzare per le pagine
> prodotto relative agli articoli della categoria merceologica
> "Televisori" un certo layout grafico, magari a una sola colonna, e di
> utilizzare invece per le pagine prodotto relative agli articoli della
> categoria merceologica "Computer" un altro layout, differente dal
> precedente e magari a tre colonne.
>
> L'assegnazione di uno specifico layout ad una pagina prodotto potrà
> inoltre avvenire anche direttamente sulla relativa pagina agendo per
> questo attraverso il corrispondente pulsante "Layout" presente nella
> barra degli strumenti del live Editing.
>
> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione dei Layout si veda anche la sezione "Live Editing --
> Layout" di questo manuale.

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
alla relativa Pagina Prodotto, in tutte le lingue di gestione del sito

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

**ATTENZIONE!** **Per le Pagine Prodotto i valori di Title, keywords,
Description, Meta Tag, SiteMap, SiteMap Frequency e SiteMap Priority
sono ereditati direttamente dalla relativa Pagina Catalogo e quindi
dalla corrispondente Categoria Merceologica**

Va fatta, infine, un'ultima importante considerazione.

I parametri inseriti in fase di configurazione della pagina e necessari
per una corretta indicizzazione della stessa, così come quelli utili a
definire se e come la pagina in esame dovrà comparire nella SiteMap,
sono generici e relativi alla pagina in quanto tale, che di per se
potrebbe anche non essere indicizzata e/o inserita nella SiteMap del
sito.

Questo tipo di pagine, come precedentemente evidenziato, sono, più che
altro, dei contenitori utili a specificare e a diversificare i contenuti
che dovranno poi essere visualizzati al loro interno dipendentemente
dalla categoria merceologia di appartenenza dello specifico prodotto.

Tali contenuti, e conseguentemente l' url della pagina, vengono quindi
dettagliati in maniera più precisa sulla base dello specifico prodotto
che l'utente ha scelto di visualizzare. Ciò che dovrà essere
indicizzato, dunque, ed inserito nella SiteMap del sito non è tanto la
pagina

www.miosito.com/catalogo-articoli/prodotti/informatica

che di per se potrebbe anche essere priva di contenuti interessanti,
quanto più esattamente la pagina prodotto di ogni singolo articolo
appartenente alla categoria merceologia "Informatica" e quindi, ad
esempio, la pagina

www.miosito..com/catalogo-articoli/prodotti/informatica/magic-mouse

Ora, per ovvie ragioni, come Title, Keywords o Description della pagina
prodotto relativa al "Magic Mouse" difficilmente potranno andar bene i
valori impostati sulla pagina Prodotto, generici e relativi a tutti gli
articoli dell'Informatica; tali valori, al contrario, andranno
specificati e diversificati proprio in base allo specifico articolo che
l'utente ha scelto di visualizzare.

Un discorso del tutto analogo può essere fatto per i parametri relativi
alla SiteMap del sito. I contenuti delle schede prodotto di due diversi
articoli della categoria "Informatica" potrebbero, ad esempio, essere
aggiornati con una frequenza diversa e le relative pagine anderebbero
quindi inserite nella SiteMap con un valore diverso per il parametro
ChangeFrequency.

**In definitiva, dunque, per una corretta gestione ed indicizzazione del
sito non è sufficiente impostare correttamente i parametri SEO e quelli
relativi alla SiteMap in fase di configurazione della Pagina Prodotto
generica, ma occorre anche specificare e dettagliare tali parametri in
fase di configurazione dello specifico articolo.**

Per maggiori informazioni in merito a come personalizzare queste
informazioni per ogni singolo prodotto, si vedano anche le sezioni
"*Catalogo -- Gestione Articoli -- Articoli -- Anagrafica Articolo /
Servizio -- Anagrafica Passweb*" e "*Sito - Preferenze*" di questo
manuale

