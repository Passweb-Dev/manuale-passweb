# SEO -- CARICAMENTO PAGINA



La sezione "**Caricamento Pagina**", presente all'interno del menu
**"Preferenze -- SEO"**, consente di settare alcuni parametri mediante i
quali poter definire la modalità di caricamento delle risorse presenti
all'interno delle pagine del proprio sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\caricamento_pagina.bmp](./assets/media/image55.png)

**[CARICAMENTO IMMAGINI]{.underline}**

Consente di decidere come dovrà essere effettuato il caricamento delle
immagini inserite nella pagina web, mediante uno dei componenti presenti
all'interno della libreria Passweb.

**ATTENZIONE!** Il parametro in esame ha effetto unicamente sui tag \<
img **\> e non prende quindi in considerazione eventuali immagini di
background.** Tale parametro inoltre potrebbe andare ad impattare in
maniera notevole sul tempo di caricamento del **Largest Contentful Paint
(LCP)**, uno dei tre Core Web Vital presi in considerazione da Google
per assegnare dei punteggi di prestazione al sito

E' possibile selezionare una delle seguenti opzioni:

- **Immediatamente**: selezionando questa opzione tutte le immagini
  presenti all'interno della pagina web, quindi anche quelle non
  immediatamente visualizzate perché non presenti inizialmente nel
  viewport, verranno caricate in maniera immediata.

> In altri termini ogni qualvolta il browser dovesse incontrare, ad
> esempio, un tag \< img \> provvederà, prima al download della relativa
> risorsa, e solo al termine di questo download proseguirà nel
> caricamento dei contenuti processando gli altri tag della pagina.
>
> In queste condizioni ovviamente il tempo di risposta della pagina sarà
> direttamente proporzionale al numero e al peso delle immagini
> effettivamente presenti all'interno della pagina stessa

- **Tramite Javascript**: selezionando questa opzione verrà effettuato,
  via javascript, il lazy loading delle immagini presenti all'interno
  della pagina.

> Al termine del caricamento della pagina web (e del relativo markup
> HTML) apposite funzioni javascript si preoccuperanno dunque di
> inserire all'interno della pagina stessa le varie immagini. E'
> semplice comprendere quindi come, in queste condizioni, il peso
> iniziale della pagina, e conseguentemente, anche il suo tempo di
> risposta, possano essere sensibilmente ridotti.
>
> D'altra parte però occorre anche considerare che spesso il LCP di una
> pagina web è proprio una delle immagini presenti nel viewport iniziale
> e, in questo caso, il fatto di dover attendere il caricamento della
> pagina e l'esecuzione delle funzioni javascript prima di aver
> disponibile l'immagine potrebbe peggiorare il punteggio assegnato da
> Google a questo Core Web Vital.

- **Tramite Attributo Loading:** anche in questo caso verrà effettuato
  il lazy loading delle immagini presenti all'interno della pagina,
  questa volta però non utilizzando javascript ma sfruttando le
  funzionalità native dei singoli browser e, nello specifico, il loro
  supporto all'attributo "loading" (
  <https://www.w3schools.com/tags/att_img_loading.asp> )

> Il vantaggio rispetto al caso precedente è rappresentato dal fatto che
> in queste condizioni non sarà necessario attendere l'esecuzione di una
> funzione javascript per avere l'immagine disponibile all'interno della
> pagina (essendo, di fatto, il browser stesso a decidere quando
> effettivamente scaricarla dal server) e questo potrebbe indubbiamente
> abbassare i tempi di caricamento del LCP (posto ovviamente che questo
> sia una delle immagini presenti nel viewport iniziale) migliorando di
> conseguenza i punteggi ad esso assegnati da Google.
>
> Anche in questo caso comunque, in relazione al solo LCP, la soluzione
> migliore resterebbe sempre quella di caricare l'immagine in maniera
> immediata evitando quindi per essa un qualsiasi tipo di lazy loading
>
> **ATTENZIONE!** per maggiori informazioni relativamente al supporto
> dei vari browser per l'attributo "loading", è possibile fare
> riferimento a quanto indicato al seguente indirizzo
> <https://caniuse.com/loading-lazy-attr>

Sulla base di quanto appena detto è abbastanza semplice comprendere che,
in relazione al caricamento delle immagini, **la soluzione migliore da
adottare è indubbiamente quella che prevede di utilizzare il lazy
loading (preferibilmente mediante la funzionalità nativa offerta dai
browser) evitando però di applicarlo, laddove possibile, a
quell'immagine che dovesse essere valutata da Google come il Largest
Contentful Paint.**

In questo modo si andrebbe infatti, da una parte a ridurre il peso
iniziale della pagina e, conseguentemente, anche il suo tempo di
caricamento e, dall'altra parte, effettuando il caricamento immediato
della sola immagine valutata da Google come il LCP si andrebbero anche
ad ottimizzare i punteggi assegnati da Google stesso a questo Core Web
Vital.

In questo senso dunque nel momento in cui si dovesse optare per una
gestione delle immagini mediante lazy loading Passweb attiverà
automaticamente, per determinati componenti, una specifica gestione.

In particolare per il componente:

- **Contenuti su Accordion:** non verrà mai effettuato il lazy loading
  di eventuali immagini inserite all'interno dell'elemento inizialmente
  attivo mediante il parametro "**Immagine**" presente nella maschera di
  configurazione del componente (tab "**Gestione Contenuti**" sezione
  "**Eventuale Immagine**")

- **Contenuti su Tabs:** non verrà mai effettuato il lazy loading di
  eventuali immagini inserite all'interno del tab inizialmente attivo
  mediante il parametro "**Immagine**" presente nella maschera di
  configurazione del componente (tab "**Gestione Contenuti**" sezione
  "**Eventuale Immagine**")

- **Contenuti su Slider**: considerando che il componente in esame
  necessita obbligatoriamente dell'applicazione di determinate funzioni
  javascript per poter funzionare in maniera corretta, nel momento in
  cui il LCP dovesse essere effettivamente una delle immagini presenti
  all'interno della slide inizialmente attiva, diventerà di fondamentale
  importanza, ai fini dell'ottimizzazione del LCP, l'utilizzo dei campi
  "**Immagine Segnaposto**", "**Immagine Segnaposto Smartphone**" e
  "**Immagine Segnaposto Tablet**" presenti nella maschera di
  configurazione del componente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\caricamento_immagini_slider.bmp](./assets/media/image56.png)

> Tali parametri offrono infatti la possibilità di indicare una
> specifica immagine (per i vari dispositivi) che verrà poi caricata e
> visualizzata all'interno della pagina (senza lazy loading) prima che
> lo Slider sia inizializzato dalle apposite funzioni javascript (per
> maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Varianti Sito Responsive -- Lista
> Componenti Comuni -- Contenuti su Slider*" di questo manuale).
>
> **ATTENZIONE!** In queste condizioni è ovviamente di fondamentale
> importanza che l'immagine utilizzata come segnaposto sia esattamente
> la stessa o che abbia quanto meno le stesse esatte dimensioni
> dell'immagine che verrà poi effettivamente visualizzata nella prima
> Slide del componente (in maniera tale da evitare effetti grafici
> indesiderati che potrebbero portare anche ad un aumento del Cumulative
> Layout Shift, un altro dei Core Web Vitals valutati da Google)

- **Galleria di Immagini:** non verrà mai effettuato il lazy loading
  della prima immagine presente in galleria

- **Immagine con link:** una volta attivato il caricamento delle
  immagini mediante lazy loading, sarà poi possibile decidere per ogni
  singola immagine gestita mediante il componente in esame se questa
  dovrà essere caricata immediatamente o attraverso il lazy loading
  abilitato a livello di sito, utilizzando per questo il parametro
  "**Caricamento Immagine**" presente nel form di configurazione del
  componente stesso (per maggiori informazioni in merito a questo
  parametro si veda anche quanto indicato all'interno del capitolo
  "*Varianti Sito Responsive -- Lista Componenti Comuni -- Immagine con
  link*" di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\caricamento_immagini_immagine.bmp](./assets/media/image57.png)

- **Articolo (CMS) / Sommario (CMS):** in relazione alle eventuali
  "**Immagini Articolo**" e "**Immagini Sommario**" inserite mediante i
  componenti in esame all'interno di una lista di post (**Lista News** o
  **Archivio News**) non verrà mai effettuato il lazy loading delle
  immagini presenti nel primo post della lista. Allo stesso modo non
  verrà effettuato neppure il lazy loading di eventuali "Immagini
  Articolo" e / o "Immagini Sommario" inserite mediante i componenti in
  esame all'interno di un "**Dettaglio News**"

- **Immagine Rappresentativa (Ecommerce)**: in relazione a componenti
  quali il "**Catalogo Ecommerce**", "**Offerte / Novità**",
  "**Popolarità Prodotto**" ... non verrà mai effettuato il lazy loading
  dell'immagine relativa al primo articolo presente in elenco.

> In relazione invece al componente "Immagine Rappresentativa" inserito
> all'interno di una "**Scheda Prodotto**" non verrà mai effettuato il
> lazy loading dell'immagine visualizzata come primo elemento della
> galleria (immagine inizialmente attiva)

**ATTENZIONE!** nel momento in cui non dovesse essere attivato il
caricamento delle immagini mediante lazy loading a livello di sito, i
componenti Passweb continueranno a funzionare in maniera "standard" e
tutte le immagini presenti all'interno del sito verranno caricate sempre
in maniera immediata.

**[ATTIVA CONTROLLO SU FORMATO IMMAGINI .WEBP E .JP2]{.underline}**

Consente, se selezionato, di abilitare l'utilizzo all'interno del sito
di immagini in formato .webp e .jp2

**ATTENZIONE!** .webp e .jp2 sono nuovi formati di immagine che
garantiscono una maggior compressione, con conseguente riduzione dei
tempi di caricamento della pagina, senza perdita di qualità. Purtroppo
non sono ancora standard universalmente riconosciuti e quindi il loro
supporto è diverso da browser a browser. (il formato jp2 è un formato
proprietario di Apple ed è quindi correttamente supportato da Safari
mentre il formato webp, sviluppato da Google, è attualmente supportato
da Chrome, Opera, Firefox ed Edge). Per maggiori informazioni
relativamente al supporto da parte dei vari browser a questi nuovi
formati è possibile consultare il sito <https://caniuse.com/>

Nel momento in cui si dovesse decidere di selezionare questo parametro,
abilitando quindi la relativa funzionalità, sarà poi necessario
procedere in maniera differente a seconda del fatto di voler utilizzare
immagini in formato .jp2 o .web.

In particolare per poter utilizzare **immagini in formato jp2** sarà
necessario procedere in questo modo:

- **In fase di configurazione di un componente Passweb utilizzare,
  laddove richiesto immagini "tradizionali",** possibilmente in formato
  .jpg o .png a seconda del fatto di voler mantenere o meno la
  trasparenza delle immagini

- Caricare **all'interno della stessa cartella in cui risiedono le
  immagini "tradizionali"** anche le immagini corrispondenti in formato
  .jp2 **facendo attenzione ad utilizzare esattamente lo stesso nome
  file**

In queste condizioni, in fase di caricamento della pagina, Passweb
verificherà in maniera totalmente automatica l'eventuale presenza, oltre
ai file in formato "tradizionale" anche delle corrispondenti versioni
.jp2 e, se presenti, le andrà ad inserire correttamente all'interno
della pagina garantendo comunque un fallback sulle immagini
"tradizionali" per quei browser che non supportano questa particolare
estensione.

**ATTENZIONE**: Allo stato attuale non è possibile utilizzare il formato
.jp2 per le immagini articolo.

Per quel che riguarda invece l'utilizzo delle **immagini in formato
webp**, Passweb mette a disposizione dei tool automatici di conversione
verso questo particolare formato.

A differenza del formato .jp2 sarà quindi possibile utilizzare il
formato .webp anche per le immagini relative ai prodotti pubblicati
all'interno del sito indipendentemente dal fatto di aver caricato queste
immagini partendo dal gestionale oppure operando direttamente
all'interno del Wizard di Passweb.

**In ogni caso l'utente dovrà preoccuparsi di caricare sempre e soltanto
immagini in formati "tradizionali" (.jpeg, .png ecc..) sarà poi Passweb
a convertire automaticamente queste immagini nel formato .webp**

Considerando che l'utilizzo di questi formati comporterà una modifica
nel markup HTML dei componenti Passweb utilizzati per gestire le
immagini (in maniera tale da garantire sempre il fallback verso formati
di immagine "tradizionali"), selezionando il parametro in esame verrà
visualizzato un messaggio per informare l'utente relativamente al fatto
che **l'attivazione del parametro stesso richiede una conversione
preventiva** di tutte le immagini attualmente utilizzate all'interno del
sito nel formato corretto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversione_webp_generale.bmp](./assets/media/image58.png)

**ATTENZIONE!** Nel momento in cui si dovesse decidere di attivare il
parametro in esame senza aver prima convertito tutte le immagini in
formato webp, queste stesse immagini, sul front end, potrebbero anche
non essere visualizzate in maniera corretta (generando quindi degli
errori 404)

Il pulsante "**Converti adesso le immagini in webp**" permette di
avviare direttamente da questa sezione del Wizard la conversione in
formato webp di tutte le immagini presenti sul sito (immagini articolo,
immagini di categoria e immagini presenti in "Gestione Risorse")

Cliccando su questo pulsante verrà quindi visualizzata la maschera
"**Conversione in webp**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversione_webp_generale_2.bmp](./assets/media/image59.png)

all'interno della quale poter impostare la qualità da utilizzare nel
processo di conversione (ovviamente più alto sarà il grado di qualità
impostata maggiore sarà il peso della relativa immagine .webp) e, una
volta fatto questo, avviare il processo cliccando sul pulsante "**Avvia
conversione**".

La procedura di conversione potrebbe richiedere diversi minuti in base
la numero complessivo di immagini da gestire.

Chiudendo la finestra prima dell'avvenuta conversione di tutte le
immagini, la procedura andrà comunque avanti ma non avremo più modo di
sapere l'esatto momento in cui l'operazione stessa sarà completata.

In alternativa è possibile accedere alle sezioni "**Gestione Risorse del
sito**" e "**Gestione Articoli**" e lanciare singolarmente la procedura
di conversione in formato webp rispettivamente, delle immagini
utilizzate per costruire il layout grafico e delle immagini relative
alle categorie merceologiche e agli articoli pubblicati all'interno del
sito (per maggiori informazioni in merito si vedano anche i rispettivi
capitoli di questo manuale).

In ogni caso una volta attivato il parametro in questione, ogni
qualvolta si andranno poi ad aggiungere nuove immagini alle risorse del
sito e/o ai prodotti gestiti (ad esempio importando nuove risorse a
seguito di una sincronizzazione) Passweb si preoccuperà di convertire
automaticamente in formato .webp anche queste nuove immagini.

In queste condizioni dunque la possibilità di lanciare manualmente una
conversione di tutte le immagini presenti in "Gestione Risorse" e/o di
tutte le immagini articolo dovrebbe servire solo ed esclusivamente per
risolvere eventuali problemi come ad esempio l'eliminazione accidentale
dalle risorse del sito di alcune immagini in formato .webp
precedentemente generate.

**ATTENZIONE!** Eventuali modifiche apportate al parametro "Attiva
Controllo su formato immagini .webp e .jp2" richiedono un riciclo del
pool di gestione del sito per cui potrebbero essere necessari alcuni
minuti prima di poterle effettivamente visualizzare sul front end.

**[CARICAMENTO JAVASCRIPT E CSS]{.underline}**

Relativamente ai file css e js gestiti automaticamente dall'applicazione
(e quindi non caricati manualmente in specifiche sezioni della pagina
web) occorre sottolineare che:

- I file css verranno inseriti nella sezione head della pagina in
  maniera tale da ottimizzare i tempi di caricamento del LCP (uno dei
  Core Web Vital presi in considerazione da Google). Diversamente
  sarebbe infatti necessario attendere il caricamento di tutta la pagina
  prima di avere disponibili le proprietà css necessarie al browser per
  renderizzare il LCP

- I file js verranno differiti in maniera automatica (laddove possibile)
  mediante l'utilizzo dell'attributo defer e il loro caricamento verrà
  effettuato (solo per Varianti Responsive) subito prima della chiusura
  del tag body

