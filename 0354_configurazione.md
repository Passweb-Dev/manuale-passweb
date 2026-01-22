# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image57.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
che si sta realizzando

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
essere reso statico.

**Considerando la tipologia di componente, prima di staticizzarlo
occorre verificare attentamente che i dati presenti al suo interno
(prezzi, sconti ecc...) siano effettivamente gli stessi per tutti gli
utenti del sito**. In caso contrario infatti si correrebbe il rischio di
visualizzare, a determinati utenti, informazioni non corrette.

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

**Numero di Righe da Visualizzare:** consente di impostare il numero di
righe della griglia di visualizzazione degli articoli. Sono accettati
solo valori minori o uguali a 30

Nel momento in cui l'esigenza dovesse essere quella di visualizzare un
numero di righe superiore a 30, si consiglia quindi di utilizzare una
paginazione di tipo "Scroll infinito (Lazy loading)"

**Numero di Articoli:** consente di impostare il numero di articoli per
riga.

In relazione a questo è bene ricordare che indipendentemente dal numero
di articoli che si è scelto di visualizzare all'interno di ogni singola
riga, per risoluzioni **inferiori ai 992 px** verranno sempre
visualizzati 2 articoli per riga.

Analogamente per risoluzioni **inferiori a 768 px** la griglia si
linearizzerà mostrando un articolo per ogni riga

**Visualizzazione Paginazione:** consente di decidere se e dove
visualizzare (rispetto al Componente stesso) i collegamenti alle varie
pagine del catalogo.

**Numero di Pagine:** consente di impostare, selezionandolo dal relativo
menu a tendina, il numero di pagine che dovranno essere visualizzate nei
controlli di paginazione. Ovviamente oltre al numero indicato
all'interno di questo campo nei controlli di paginazione saranno sempre
visibili anche la prima e l'ultima pagina disponibili.

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Paginazione con Precedente e Successivo:** se selezionato, nei
controlli di paginazione, verranno visualizzati anche i pulsanti
"Precedente" e "Successivo".

Il testo di questi pulsanti è modificabile alla sezione \"Gestione
Testi/Messaggi del Sito\" e agendo sull\'elemento generico
\"Paginazione\".

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Tipo di Paginazione per dispositivi desktop (**\>= **992px):**
consente di definire il tipo di paginazione da utilizzare, per il
componente in oggetto, su dispositivi desktop (risoluzione maggiore o
uguale a 992px)

E' possibile selezionare uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scroll bar per visualizzare i
  risultati presenti all'interno della nuova pagina)

- **A richiesta:** selezionando questa tipologia di paginazione verrà
  visualizzato sopra e/o sotto il componente (dipendentemente da come è
  stato impostato il precedente parametro "Visualizza Paginazione") un
  pulsante "**Mostra Altri Risultati**" che l'utente dovrà utilizzare
  per richiedere la visualizzazione degli articoli presenti nelle
  successive pagine del catalogo.

- **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
  paginazione gli articoli distribuiti all'interno delle varie pagine,
  verranno visualizzati automaticamente mano a mano che l'utente
  scorrerà la pagina web verso l'alto

**Tipo di Paginazione per dispositivi mobile (\<** **992px):** consente
di definire il tipo di paginazione da utilizzare, per il componente in
oggetto, su dispositivi mobile (risoluzione minore a 992px). E'
possibile selezionare uno dei seguenti valori:

- **A richiesta:** selezionando questa tipologia di paginazione verrà
  visualizzato sopra e/o sotto il componente (dipendentemente da come è
  stato impostato il precedente parametro "Visualizza Paginazione") un
  pulsante "**Mostra Altri Risultati**" che l'utente dovrà utilizzare
  per richiedere la visualizzazione degli articoli presenti nelle
  successive pagine del catalogo.

- **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
  paginazione gli articoli distribuiti all'interno delle varie pagine,
  verranno visualizzati automaticamente mano a mano che l'utente
  scorrerà la pagina web verso l'alto

**Elementi per pagina:** consente di indicare una lista di valori,
sperati da virgole, corrispondenti al numero di elementi che potranno
essere visualizzati in ogni singola pagina del componente. Gli unici
caratteri ammessi all'interno di questo campo sono quelli numerici (0-9)
e la virgola che dovrà essere utilizzata come carattere separatore.

Nel momento in cui questo campo dovesse essere valorizzato in maniera
corretta, sul sito verrà poi visualizzato un menu a tendina contenente
l'elenco dei valori immessi.

Selezionando uno dei valori presenti in elenco il componente verrà
ricaricato e popolato con il numero di articoli per pagina indicati
dall'utente.

**ATTENZIONE! Modificando il numero di articoli per pagina il componente
ripartirà sempre dalla prima pagina**

**Visualizzazione iniziale degli articoli:** se selezionato, il
componente visualizzerà a default tutti gli articoli presenti in
catalogo. Non selezionando questo parametro, invece, a default il
componente non visualizzerà nessun articolo. In queste condizioni
eventuali articoli verranno quindi visualizzati all'interno di questo
componente solo dopo aver applicato uno specifico filtro di ricerca.

**Filtro Articoli:** consente di definire il filtro di visualizzazione
articoli attraverso il quale poter stabilire quali articoli dovranno
comparire o meno all'interno del componente**.** Per maggiori
informazioni relativamente alla creazione di un filtro articoli si veda
anche la sezione *"Utenti -- Gruppi Utenti Sito -- Filtri Utente e
Filtri Articolo -- Filtri Articolo"* di questo manuale

**Rimozione Filtro:** consente di visualizzare, se selezionato, un
pulsante (**Rimuovi filtro applicato**) attraverso il quale eliminare in
blocco tutti i filtri attualmente applicati al componente in oggetto.

> **NOTA BENE:** il pulsante "Rimuovi filtro applicato" contestuale al
> componente "Risultati Ricerca" verrà visualizzato non appena dovesse
> essere applicato, a questo stesso componente, uno specifico filtro di
> ricerca.

Per maggiori informazioni relativamente alla possibilità, da parte
dell'utente che visita il sito, di eliminare eventuali filtri di
ricerca, si veda anche il paragrafo "*Componente Ricerca -- Ricerca
Ecommerce*" di questo manuale.

**Visualizzazione Risultati:** se selezionato, consentirà di
visualizzare, nella parte bassa del componente, una stringa di testo
contenente il numero complessivo degli articoli presenti all'interno del
componente stesso.

Il testo di questa stringa può essere modificato e personalizzato alla
sezione \"Gestione Testi/Messaggi del Sito\" agendo sui testi del
componente in oggetto.

In particolare il testo in esame per il componente "Popolarità Prodotto"
sarà esattamente lo stesso di quello impostato per il componente
"Catalogo Ecommerce"

**Visualizza Ordinamento:** se selezionato, consentirà di visualizzare,
lato sito, una combo box contenente l'elenco degli elementi sulla base
dei quali poter effettuare l'ordinamento degli articoli presenti
all'interno del componente.

**NOTA BENE: l'ordinamento iniziale è sempre determinato sulla base
della specifica modalità di funzionamento del componente.**

**Posizionamento barra controlli superiore:** consente di stabilire,
selezionando la relativa combinazione da un apposito menu a tendina,
l'ordine di posizionamento degli elementi principali presenti nella
barra dei controlli posta immediatamente al di sopra del componente.

In questo senso gli elementi ordinabili sono: "Elementi per pagina",
"Ordinamento", "Paginazione"

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato**

**Identificatore**: consente di stabilire se l'ordinamento, la
paginazione e gli elementi per pagina, impostati sul front end dagli
utenti del sito, dovranno essere applicati a livello di pagina oppure a
livello di singolo componente. E' possibile selezionare uno dei seguenti
valori:

- **Pagina:** selezionando questa opzione l'ordinamento, la paginazione
  e gli elementi per pagina impostati dall'utente lato front end,
  mediante gli appositi controlli, verranno applicati a livello di
  pagina.

> Ciò significa dunque che, nel caso in cui all'interno della pagina
> dovessero essere presenti due o più componenti dello stesso tipo le
> impostazioni settate, su uno di questi componenti per l'ordinamento,
> la paginazione e gli elementi per pagina, avranno effetto anche sugli
> altri
>
> **Tale opzione risulta particolarmente utile nel momento in cui si
> dovessero utilizzare, all'interno di un componente Tab, due distinti
> "Risultati Ricerca" realizzati con layout grafici diversi per ottenere
> ad esempio il classico passaggio dal layout a griglia a quello a
> lista**
>
> In queste condizioni avendo impostato come "Identificatore" l'intera
> pagina saremo sicuri che nel momento in cui un utente dovesse, ad
> esempio, ordinare il componente a griglia in un certo modo, tale
> ordinamento verrà poi mantenuto anche nel passaggio alla
> visualizzazione a lista (e la stessa cosa vale anche per la
> paginazione e per gli elementi per pagina).

- **Nome Componente:** selezionando questa opzione l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, mediante gli appositi controllo verranno applicati
  solo ed esclusivamente al componente indicato

**Posizionamento barra controlli inferiore:** consente di stabilire,
selezionando la relativa combinazione da un apposito menu a tendina,
l'ordine di posizionamento degli elementi principali presenti nella
barra dei controlli posta immediatamente al di sotto del componente.

In questo senso gli elementi ordinabili sono: "Risultati" e
"Paginazione"

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato**

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, il
Componente **"**Risultati Ricerca**" può essere considerato a tutti gli
effetti come un Componente di tipo Contenitore.** Sarà infatti possibile
inserire al suo interno tutta una serie di campi che, per poter esser
gestiti liberamente, dovranno inevitabilmente esser trattati a loro
volta come Componenti autonomi editabili singolarmente.

Per poter far questo occorre, innanzitutto, attivare la modalità di
gestione dei componenti, sarà poi necessario portarsi sul Componente
"Risultati Ricerca" e, alla comparsa del R.O.C. cliccare sull'icona
**Accedi ai componenti interni**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Risultati Ricerca"
sarà possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il proprio componente.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce:** contiene quei componenti necessari per
  abilitare e gestire determinate funzionalità (es. "Aggiunta al
  Carrello") oltre che, ovviamente per inserire e gestire all'interno
  del sito determinate informazioni prelevate direttamente dal
  gestionale.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al "Catalogo E-Commerce" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

L'inserimento di questi componenti all'interno del componente Risultati
Ricerca avviene utilizzando le solite tecniche di interazione con
l'editor (Drag and Drop o Point and Click) già esaminate all'interno di
questo manuale (per maggiori informazioni si rimanda allo specifico
capitolo di questo manuale).

