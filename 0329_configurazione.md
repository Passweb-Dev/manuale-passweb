# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e di configurazione**

![](./assets/media/image207.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome**: consente di definire un nome per il Componente che si sta
  editando

- **Pubblico** (selezionato a default): consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione**: consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Abilita la Ricerca sui Titoli delle Pagine:** selezionando questo
  parametro verranno visualizzati all'interno del componente in oggetto
  i risultati di ricerche di tipo testuale effettuate sui Titoli delle
  Pagine Generiche, e più esattamente dunque sui valori inseriti
  all'interno del campo "**Nome Pagina**" e/o "**Titolo Pagina**"
  presenti tra le proprietà della pagina stessa.

- **Abilita la Ricerca sui Contenuti delle Pagine:** selezionando questo
  parametro verranno visualizzati all'interno del componente in oggetto
  i risultati di ricerche effettuate sui componenti di tipo Testuale
  inseriti all'interno delle Pagine Generiche del proprio sito.

> **Per componenti di tipo testuale si intendono i testi inseriti
> all'interno delle pagine generiche del sito mediante i seguenti
> componenti: Paragrafo, News, HTML, Contenuti su Tabs, Contenuti si
> Accordion, Contenuti su Slider.**

- **Abilita la Ricerca sui Titoli delle Pagine Catalogo:** selezionando
  questo parametro verranno visualizzati all'interno del componente in
  oggetto i risultati di ricerche di tipo testuale effettuate sui Titoli
  delle Pagine di tipo Catalogo/Prodotto, e più esattamente dunque sui
  valori inseriti all'interno del campo "**Nome Pagina**" e/o "**Titolo
  Pagina**" presenti tra le proprietà della pagina stessa.

- **Abilita la Ricerca sui Contenuti delle Pagine Catalogo:**
  selezionando questo parametro verranno visualizzati all'interno del
  componente in oggetto i risultati di ricerche effettuate sui
  componenti di tipo Testuale inseriti all'interno delle Pagine di tipo
  Catalogo/Prodotto del proprio sito.

> **Per componenti di tipo testuale si intendono i testi inseriti
> all'interno delle pagine generiche del sito mediante i seguenti
> componenti: Paragrafo, News, HTML, Contenuti su Tabs, Contenuti si
> Accordion, Contenuti su Slider.**

- **Abilita la Ricerca sui Contenuti CMS:** impostando questo parametro
  a **SI**, all'interno del componente in oggetto verranno visualizzati
  anche i risultati di ricerche effettuate sui contenuti CMS inseriti
  mediante gli appositi componenti e appartenenti alle Categorie
  indicate in corrispondenza del successivo parametro "**Filtro
  Categorie**"

![](./assets/media/image208.png)

> Nello specifico le ricerche CMS verranno effettuate su quanto
> inserito, per le varie news, all'interno dei campi "**Sommario**",
> "**Contenuto**" e "**Descrizione 1 /2 /3**"
>
> **ATTENZIONE!!!:Per poter visualizzare i risultati relativi ad una
> qualsiasi notizia CMS pubblicata all'interno del sito,
> indipendentemente dalla sua categoria di appartenenza, sarà necessario
> impostare il campo "Filtro su singola Categoria" sul valore radice
> "Categorie CMS"**
>
> Nel momento in cui il parametro in oggetto dovesse essere impostato a
> SI, come risultato della ricerca verrà visualizzato il link di
> collegamento al dettaglio del relativo articolo CMS.
>
> In queste condizioni diventa dunque di fondamentale importanza il
> successivo parametro **"Pagina di Lettura di Default per i Risultati
> CMS"** grazie al quale poter indicare la specifica pagina cui dovrà
> portare il link di collegamento visualizzato come risultato della
> ricerca e che dovrà, ovviamente, contenere un componente CMS di tipo
> "Dettaglio News" (in assenza del quale non sarà possibile visualizzare
> il dettaglio della corrispondente notizia).

- **Abilita la Ricerca sui Tag Cms** (visualizzato solo nel caso in cui
  il precedente campo "Abilita la ricerca sui Contenuti CMS" sia stato
  impostato a SI): selezionando questo parametro le ricerche sui
  contenuti CMS verranno estese anche ai Tag associati ad ogni singola
  notizia pubblicata all'interno del sito.

- **Ricerca contestuale** (visualizzato solo nel caso in cui il
  precedente campo "Abilita la ricerca sui Contenuti CMS" sia stato
  impostato a SI): selezionando questo parametro la ricerca verrà
  effettuata solo ed esclusivamente sul dettaglio del contenuto
  attualmente caricato all'interno del sito (senza prendere in
  considerazione quanto impostato all'interno del campo "Filtro
  Categorie")

> Tale parametro potrebbe quindi rivelarsi particolarmente utile nel
> caso in cui si volessero effettuare delle ricerche all'interno di un
> determinato contenuto strutturato limitando i risultati ai soli
> contenuti di quella specifica gerarchia.

- **Abilita la Ricerca sui Dati Ecommerce:** impostando questo parametro
  sul valore **Si**, all'interno del componente in oggetto verranno
  visualizzati anche i risultati di ricerche di tipo testuale effettuate
  sui dati Ecommerce indicati attraverso il successivo parametro **Dati
  Ecommerce**

> **ATTENZIONE**! in queste condizioni come risultato della ricerca
> verrà visualizzato il link di collegamento alla scheda prodotto del
> relativo articolo

- **Dati Ecommerce --** visibile solo nel caso in cui il precedente
  parametro "Abilita la Ricerca sui Dati Ecommerce" sia stato impostato
  sul valore Si.

> Consente di specificare quali dati Ecommerce dovranno essere
> effettivamente considerati in fase di ricerca articoli.

![](./assets/media/image209.png)

> E' possibile selezionare una delle seguenti opzioni:

- **Generici:** selezionando questa opzione la ricerca articoli verrà
  effettuata prendendo in considerazione per ogni articolo i seguenti i
  campi: codice, titolo, descrizione, codice alternativo, categoria
  merceologica, categoria statistica, natura e attributi articolo (tutti
  quelli attualmente gestiti all'interno del sito)

- **FullText:** selezionando questa opzione la ricerca articoli verrà
  effettuata prendendo in considerazione solamente il campo FullText e,
  in conseguenza di ciò, i soli Campi e/o Attributi Articolo selezionati
  in fase di creazione del campo stesso

![](./assets/media/image210.png)

> Per maggiori informazioni relativamente a come creare e gestire il
> campo FullText evidenziato in figura si veda anche la corrispondente
> sezione di questo manuale "*Catalogo -- Configurazione Parametri
> Catalogo -- Catalogo Mexal / Ho.Re.Ca. -- Ricerca FullText*"

- **Pagina di Lettura di Default per i Risultati CMS:** consente di
  indicare la specifica pagina cui dovrà portare il link di collegamento
  visualizzato come risultato di ricerche effettuate sui contenuti delle
  notizie inserite all'interno del proprio sito mediante i relativi
  componenti CMS. **E' di fondamentale importanza che nella pagina
  selezionata all'interno di questo campo sia presente il componente CMS
  "Dettaglio News".**

> **NOTA BENE:** nel caso in cui all'interno della pagina selezionata
> come pagina di lettura non sia presente il componente "Dettaglio News"
> non sarà possibile visualizzare in alcun modo, in questa stessa
> pagina, il contenuto della notizia presente come risultato della
> ricerca inizialmente effettuata.

- **Numero di risultati per pagina:** consente di specificare il numero
  dei risultati di ricerca che verranno visualizzati all'interno di ogni
  singola pagina

- **Visualizzazione Paginazione:** consente di specificare dove dovranno
  essere visualizzati i controlli relativi alla paginazione dei
  risultati ottenuti dalla ricerca effettuata.

- **Numero di Pagine:** consente di impostare, selezionandolo dal
  relativo menu a tendina, il numero di pagine che dovranno essere
  visualizzate nei controlli di paginazione. Ovviamente oltre al numero
  indicato all'interno di questo campo nei controlli di paginazione
  saranno sempre visibili anche la prima e l'ultima pagina disponibili.

> **Questo campo viene visualizzato solo nel caso in cui il parametro
> "Dove vuoi visualizzare la Paginazione" sia stato impostato su di un
> valore diverso da "Non Visualizzare".**

- **Paginazione con Precedente e Successivo:** se selezionato, nei
  controlli di paginazione, verranno visualizzati anche i pulsanti
  "Precedente" e "Successivo".

> Il testo di questi pulsanti è modificabile alla sezione \"Gestione
> Testi/Messaggi del Sito\" e agendo sull\'elemento generico
> \"Paginazione\".
>
> **Questo campo viene visualizzato solo nel caso in cui il parametro
> "Dove vuoi visualizzare la Paginazione" sia stato impostato su di un
> valore diverso da "Non Visualizzare".**

- **Tipo di Paginazione per dispositivi desktop (**\>= **992px):**
  consente di definire il tipo di paginazione da utilizzare, per il
  componente in oggetto, su dispositivi desktop (risoluzione maggiore o
  uguale a 992px)

> E' possibile selezionare uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scroll bar per visualizzare i
  risultati presenti all'interno della nuova pagina)

<!-- -->

- **Tipo di Paginazione per dispositivi mobile (\<** **992px):**
  consente di definire il tipo di paginazione da utilizzare, per il
  componente in oggetto, su dispositivi mobile (risoluzione minore a
  992px). E' possibile selezionare uno dei seguenti valori:

  - **A richiesta:** selezionando questa tipologia di paginazione verrà
    visualizzato sopra e/o sotto il componente (dipendentemente da come
    è stato impostato il precedente parametro "Visualizza Paginazione")
    un pulsante "**Mostra Altri Risultati**" che l'utente dovrà
    utilizzare per richiedere la visualizzazione dei risultati di
    ricerca presenti nelle successive pagine.

  - **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
    paginazione i risultati di ricerca, distribuiti all'interno delle
    varie pagine, verranno visualizzati automaticamente mano a mano che
    l'utente scorrerà la pagina web verso l'alto

<!-- -->

- **Elementi per Pagina:** consente di indicare una lista di valori,
  sperati da virgole, corrispondenti al numero di elementi che potranno
  essere visualizzati in ogni singola pagina del componente. Gli unici
  caratteri ammessi all'interno di questo campo sono quelli numerici
  (0-9) e la virgola che dovrà essere utilizzata come carattere
  separatore.

> Nel momento in cui questo campo dovesse essere valorizzato in maniera
> corretta, sul sito verrà poi visualizzato, in corrispondenza del
> componente in oggetto, un menu a tendina contenente l'elenco dei
> valori immessi (compreso anche, ovviamente, il valore indicato
> all'interno del precedente parametro "Numero articoli da
> visualizzare").
>
> Selezionando uno dei valori presenti in elenco il componente verrà
> ricaricato e popolato con il numero di articoli per pagina indicati
> dall'utente.
>
> **ATTENZIONE! Modificando il numero di articoli per pagina il
> componente ripartirà sempre dalla prima pagina**

- **Visualizzazione Risultati:** se selezionato, consentirà di
  visualizzare, nella parte bassa del componente, una stringa di testo
  contenente il numero complessivo dei risultati che soddisfano la
  ricerca effettuata.

> Il testo di questa stringa può essere modificato e personalizzato alla
> sezione \"Gestione Testi/Messaggi del Sito\" agendo sui testi del
> componente in oggetto.

- **Visualizza URL completo:** se selezionato verrà visualizzato, nei
  risultati delle ricerca, l'indirizzo completo della pagina del sito
  contente le keywords ricercate.

- **Visualizzare il testo intorno alle Keywords riscontrate:** se
  selezionato verrà visualizzato, nei risultati della ricerca e nel caso
  in cui il tipo del risultato lo consenta, il testo presente nella
  pagina di destinazione attorno alle varie keywords (il numero di
  caratteri visualizzati dipenderà poi dai due parametri precedentemente
  impostati). Nel caso in cui questo parametro non venga selezionato non
  verrà mai visualizzato alcun testo attorno alle keywords di ricerca
  indipendentemente da quanto indicato nei parametri precedentemente
  considerati.

- **Numero di caratteri del testo ritagliato intorno alle keyword/s:**
  consente di indicare il numero di caratteri (arrotondato alla parola
  intera) che potranno essere visualizzati, nei risultati della ricerca,
  attorno ad ogni occorrenza delle keywords ricercate.

- **Visualizza immagine correlata:** nel caso in cui il risultato della
  ricerca faccia riferimento ad un articolo gestito all'interno del
  sito, selezionando questo parametro verrà visualizzata, come risultato
  della ricerca, anche la sua "Immagine Catalogo".

> Nel caso in cui il risultato faccia riferimento ad una categoria
> merceologica verrà visualizzata anche la relativa "Immagine di
> Categoria".
>
> Infine nel caso in cui il risultato faccia riferimento ad uno
> specifico Post CMS nel risultato della ricerca verrà visualizzata
> anche l'eventuale immagine del sommario.

- **Visualizza Data Cms** (visualizzato solo nel caso in cui il
  precedente campo "Abilita la ricerca sui Contenuti CMS" sia stato
  impostato a SI): selezionando questo parametro nei risultati di
  ricerca verrà visualizzata anche la data di pubblicazione relativa ad
  eventuali News oggetto della ricerca effettuata.

- **Formato Data** (visualizzato solo nel caso in cui il precedente
  campo "Abilita la ricerca sui Contenuti CMS" sia stato impostato a
  SI): consente di impostare il formato di visualizzazione per la Data
  di pubblicazione delle News visualizzata nei relativi risultati di
  ricerca.

- **Visualizza Ordinamento:** se selezionato, consentirà di
  visualizzare, lato sito, una combo box contenente l'elenco degli
  elementi sulla base dei quali poter effettuare l'ordinamento dei
  risultati di ricerca ottenuti.

> **ATTENZIONE! Nel caso in cui si decida di non selezionare questo
> parametro sarà comunque necessario agire dalla sezione "Gestione Campi
> di Ordinamento" per impostare, sul componente, un ordinamento di
> default.**
>
> Per maggiori informazioni in merito all'ordinamento dei risultati di
> ricerca ottenuti si veda anche il successivo capitolo di questo
> manuale.

- **Identificatore**: consente di stabilire se l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, dovranno essere applicati a livello di pagina oppure
  a livello di singolo componente. E' possibile selezionare uno dei
  seguenti valori:

  - **Pagina:** selezionando questa opzione l'ordinamento, la
    paginazione e gli elementi per pagina impostati dall'utente lato
    front end, mediante gli appositi controlli, verranno applicati a
    livello di pagina.

> Ciò significa dunque che, nel caso in cui all'interno della pagina
> dovessero essere presenti due o più componenti dello stesso tipo le
> impostazioni settate, su uno di questi componenti per l'ordinamento,
> la paginazione e gli elementi per pagina, avranno effetto anche sugli
> altri.

- **Nome Componente:** selezionando questa opzione l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, mediante gli appositi controllo verranno applicati
  solo ed esclusivamente al componente indicato

<!-- -->

- **Posizionamento barra controlli superiore:** consente di stabilire,
  selezionando la relativa combinazione da un apposito menu a tendina,
  l'ordine di posizionamento degli elementi principali presenti nella
  barra dei controlli posta immediatamente al di sopra dell'elenco dei
  risultati di ricerca.

> In questo senso gli elementi ordinabili sono: "Elementi per pagina",
> "Ordinamento", "Paginazione"
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato**

- **Posizionamento barra controlli inferiore:** consente di stabilire,
  selezionando la relativa combinazione da un apposito menu a tendina,
  l'ordine di posizionamento degli elementi principali presenti nella
  barra dei controlli posta immediatamente al di sotto dell'elenco dei
  risultati di ricerca.

> In questo senso gli elementi ordinabili sono: "Risultati" e
> "Paginazione"
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato**

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- Il risultato di ricerca

- L'eventuale immagine correlata allo specifico risultato di ricerca

> E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame (Risultato Ricerca e Immagine
> Correlata), permettendo dunque, già in fase di configurazione del
> componente stesso di decidere quale elemento dovrà essere visualizzato
> prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

