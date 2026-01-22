# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e di configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_popolarita_prodotto_configurazione_desktop_res.bmp](./assets/media/image21.png){width="4.889583333333333in"
height="2.9875in"}

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

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

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

**Intestazione:** consente di indicare, in tutte le lingue attualmente
gestite all'interno del sito, un paragrafo che verrà poi visualizzato,
sul front end del sito, come intestazione del componente in esame.

**Tipologia:** consente di impostare la modalità di funzionamento del
componente e, conseguentemente, cosa esso dovrà visualizzare. E'
possibile selezionare uno dei seguenti valori:

- **Articoli più visti:** selezionando questa opzione il componente
  visualizzerà un elenco degli articoli più cliccati.

> **ATTENZIONE!** **il criterio di popolarità utilizzato per ordinare
> gli articoli all'interno del componente è basato sul numero di visite
> ricevute dalle relative pagine prodotto**.
>
> L'ordinamento principale degli articoli presenti all'interno del
> componente corrisponde quindi con il "**Report Pagine del Sito**"
> presente nella corrispondente sezione del Wizard e, ovviamente,
> filtrato per "**Prodotti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popolarita_prodotto_res.bmp](./assets/media/image22.png){width="4.883333333333334in"
height="2.9569444444444444in"}

> Nel caso in cui alcune pagine abbiano ricevuto lo stesso numero di
> visite, e abbiano quindi la stessa popolarità, i corrispondenti
> articoli verranno ordinati sulla base di quanto impostato all'interno
> della successiva sezione "Gestione Campi di Ordinamento".

- **Articoli Visti di recente:** selezionando questa opzione il
  componente visualizzerà l'elenco degli articoli di cui l'utente ha
  visitato, **durante la sessione corrente**, la relativa Pagina
  Prodotto.

> **ATTENZIONE! gli articoli "visiti di recente" fanno riferimento solo
> ed esclusivamente alla sessione di visita corrente. Nel caso in cui
> l'utente non dovesse essere entrato, durante la sessione corrente, in
> nessuna pagina Prodotto il componente risulterà quindi privo di
> articoli.**
>
> In queste condizioni, infine, l'ordinamento degli articoli
> visualizzati all'interno del componente sarà determinato solo ed
> esclusivamente in base a quanto impostato all'interno della successiva
> sezione "Gestione Campi di Ordinamento"

- **Articoli più acquistati:** selezionando questa opzione il componente
  visualizzerà l'elenco degli articoli più acquistati.

> **ATTENZIONE! gli articoli più acquistati sono determinati solo ed
> esclusivamente sulla base degli ordini attualmente presenti in Passweb
> e del numero di volte in cui uno stesso articolo compare all'interno
> di questi stessi ordini.**
>
> All'interno del componente gli articoli saranno quindi ordinati in
> maniera decrescente in base al numero dello loro presenze all'interno
> degli ordini Passweb.
>
> Nel momento in cui determinati articoli dovessero comparire lo stesso
> numero di volte all'interno degli ordini Passweb, il loro ordinamento
> verrà impostato sulla base di quando settato all'interno della
> successiva sezione "Gestione Campi di Ordinamento".

- **Articoli più acquistati dall'utente:** come nel caso precedente
  selezionando questa opzione il componente visualizzerà l'elenco degli
  articoli più acquistati questa volta però in relazione allo specifico
  utente attualmente loggato sul sito.

> **ATTENZIONE!** Nel caso in cui il parametro "Tipologia" dovesse
> essere impostato su questo valore e l'utente che naviga il sito non
> dovesse ancora aver effettuato l'autenticazione, all'interno del
> componente Popolarità non verrà visualizzato, ovviamente, nessun
> prodotto

- **Articoli acquistati insieme:** selezionando questa opzione il
  componente visualizzerà l'elenco degli articoli che sono stati
  acquistati assieme ad un altro specifico prodotto.

> Ovviamene, in queste condizioni, il componente dovrà necessariamente
> essere inserito all'interno di una Pagina Prodotto oppure all'interno
> della Pagina Carrello.
>
> **ATTENZIONE! per determinare quali articoli sono stati acquistati
> assieme ad un altro specifico prodotto vengono presi in considerazione
> solo ed esclusivamente gli ordini attualmente presenti in Passweb.**
>
> Nel momento in cui il componente dovesse essere inserito all'interno
> di **una Pagina Prodotto**, verranno quindi visualizzati al suo
> interno tutti gli articoli che, facendo riferimento agli ordini
> attualmente presenti in Passweb, sono stati acquistati assieme
> all'articolo di cui si sta visualizzando il dettaglio.
>
> Nel momento in cui il componente dovesse invece essere inserito, con
> questa configurazione, all'interno **della Pagina Carrello**, al suo
> interno verranno visualizzati tutti gli articoli che, facendo sempre
> riferimento agli ordini attualmente presenti in Passweb, risultano
> essere stati acquistati assieme ad uno qualsiasi dei prodotti
> attualmente presenti in carrello.
>
> All'interno del componente gli articoli saranno poi ordinati in
> maniera decrescente in base al numero di volte in cui questi stessi
> articoli compaiono negli ordini attualmente presenti in Passweb
> assieme allo specifico articolo di cui si sta consultando la pagina
> prodotto
>
> Anche in questo caso inoltre, nel momento in cui determinati articoli
> dovessero comparire lo stesso numero di volte all'interno degli ordini
> Passweb il loro ordinamento verrà impostato sulla base di quando
> settato all'interno della successiva sezione "Gestione Campi di
> Ordinamento".

- **Articoli Abbinati -- opzione valida solo per la pagina Carrello:**
  nel momento in cui il componente dovesse essere inserito all'interno
  della pagina Carrello, selezionando questa opzione sarà possibile
  visualizzare al suo interno l'elenco degli articoli abbinati a tutti i
  prodotti attualmente presenti in Carrello.

> **ATTENZIONE!** gli abbinati presenti all'interno del componente
> "Popolarità Prodotto" non sono suddivisi per Categoria come avviene
> invece per il componente "Abbinati Ecommerce" gestibile all'interno di
> una pagina Prodotto.
>
> A differenza quindi delle altre opzioni precedentemente esaminate, in
> questo caso gli articoli mostrati all'interno del componente non
> saranno determinati dinamicamente da azioni effettuate dagli stessi
> utenti del sito (acquisti o visite alle pagine prodotto) ma saranno
> stabiliti a tavolino sulla base degli abbinamenti realizzati
> all'interno del gestionale
>
> **ATTENZIONE!** Ovviamente, nel caso in cui il carrello dovesse essere
> vuoto o il componente Popolarità Prodotto dovesse essere inserito, con
> questa configurazione, in una pagina diversa dalla pagina Carrello, al
> suo interno non verrà mai visualizzato nessun articolo

- **Articoli Categoria:** selezionando questa opzione il componente
  visualizzerà articoli delle Categorie Merceologiche specificate
  mediante il successivo parametro "**Categoria**"

- **Reccomendations Clerk:** selezionando questa opzione il componente
  verrà utilizzato per mostrare al suo interno i prodotti suggeriti
  dalla Raccomandazione Clerk indicata poi all'interno del successivo
  campo "**Logica Raccomandazione Clerk.io**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popolarita_prodotto_clerk_2.bmp](./assets/media/image23.png){width="4.355555555555555in"
height="3.061111111111111in"}

> **ATTENZIONE!** **l'opzione "Reccomendations Clerk" richiede
> necessariamente l'attivazione del modulo Clerk presente all'interno di
> Passstore**.
>
> Per maggiori informazioni in merito si rimanda a quanto indicato
> all'interno dei capitoli "*Passweb e Clerk*" e "*Passweb e Clerk --
> Raccomandazioni -- Raccomandazioni implementate mediante componente
> Popolarità Prodotto*" di questo manuale

**Periodo (giorni) -- non disponibile per Raccomandazioni Clerk -- :**
consente di impostare il numero di giorni che dovranno essere
considerati per valutare gli articoli più popolari, quelli più
acquistati e/o quelli acquistati assieme ad un altro specifico prodotto.

Nel caso in cui si decida, ad esempio, di inserire all'interno di questo
campo il valore 7 il componente visualizzerà gli articoli più popolari,
quelli più acquistati e/o quelli acquistati assieme ad una altro
specifico prodotto durante l'ultima settimana.

Non impostando alcun valore, verranno invece considerati tutti i dati
attualmente presenti in Passweb.

Tale parametro, infine, non verrà ovviamente considerato nel momento in
cui il componente dovesse essere stato impostato per visualizzare gli
articoli più recenti.

**Categoria -- non disponibile per Raccomandazioni Clerk --** : consente
di impostare un eventuale filtro di visualizzazione, basato sulle
Categorie Merceologiche, per gli articoli presenti all'interno del
componente.

Grazie a questo parametro è quindi possibile decidere di far
visualizzare all'interno del componente "Popolarità Prodotto" tutti gli
articoli che soddisfano le condizioni impostate tramite il parametro
"Tipologia" oppure solamente quelli che, oltre a soddisfare queste
stesse condizioni, appartengono però anche a ben precise Categorie
Merceologiche

È possibile selezionare uno dei seguenti valori:

- **Tutte (default):** selezionando questa opzione all'interno del
  componente "Popolarità Prodotto" verranno visualizzati sempre tutti
  gli articoli che soddisfano le condizioni impostate mediante il
  precedente parametro "Tipologia" indipendentemente, quindi, dalla loro
  specifica Categoria Merceologica di appartenenza

- **Attuale:** selezionando questa opzione all'interno del componente
  "Popolarità Prodotto" verranno visualizzati, tra tutti gli articoli
  che soddisfano le condizioni impostate mediante il precedente
  parametro "Tipologia", solo ed esclusivamente quelli che appartengono
  alla Categoria Merceologica (e ad eventuali Categorie Figlie) relativa
  alla pagina in cui è stato inserito il componente.

> Nello specifico, nel caso in cui il componente sia stato inserito
> all'interno di una:

- **Pagina Prodotto:** la categoria merceologica alla quale fare
  riferimento sarà quella di appartenenza del relativo articolo.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono a questa stessa Categoria Merceologica o ad una delle
> sue eventuali Categorie Figlie.

- **Pagina Carrello:** le categorie merceologiche alle quali fare
  riferimento saranno quelle di appartenenza di tutti gli articoli
  presenti in carrello.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono ad una qualsiasi di queste stesse Categorie
> Merceologiche o ad una delle loro eventuali Categorie Figlie

- **Pagina di Categoria (pagine blu):** la categoria merceologica alla
  quale fare riferimento sarà quella relativa alla pagina in esame.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono a questa stessa Categoria Merceologica o ad una delle
> sue eventuali Categorie Figlie

- **Padre:** selezionando questa opzione all'interno del componente
  "Popolarità Prodotto" verranno visualizzati, tra tutti gli articoli
  che soddisfano le condizioni impostate mediante il precedente
  parametro "Tipologia", solo ed esclusivamente quelli che appartengono
  alla Categoria Merceologica Padre (e ad eventuali Categorie Figlie) di
  quella relativa alla pagina in cui è stato inserito il componente.

> Nello specifico, nel caso in cui il componente sia stato inserito
> all'interno di una

- **Pagina Prodotto:** la categoria merceologica alla quale fare
  riferimento sarà la Categoria Padre di quella cui appartiene il
  relativo articolo.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono a questa stessa Categoria Merceologica o ad una delle
> sue eventuali Categorie Figlie.

- **Pagina Carrello:** le categorie merceologiche alle quali fare
  riferimento saranno le Categorie Padre di quelle cui appartengono gli
  articoli presenti in carrello.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono ad una qualsiasi di queste stesse Categorie
> Merceologiche o ad una delle loro eventuali Categorie Figlie

- **Pagina di Categoria (pagine blu):** la categoria merceologica alla
  quale fare riferimento sarà la Categoria Padre di quella relativa alla
  pagina in esame.

> All'interno del componente "Popolarità Prodotto" verranno quindi
> visualizzati, tra tutti gli articoli che soddisfano le condizioni
> impostate mediante il precedente parametro "Tipologia", solo quelli
> che appartengono a questa stessa Categoria Merceologica o ad una delle
> sue eventuali Categorie Figlie

**[Esempio:]{.underline}**

Supponendo di avere quest\'albero di categorie:

R

\|\_R1

\|\_R2

\|\_R21

\|\_R22

\|\_R221

\|\_R222

\|\_R2221

\|\_R22211

\|\_R22212

\|\_R2222

\|\_R223

\|\_R23

\|\_R3

Nel caso in cui il componente fosse inserito all'interno di una pagina
Prodotto si potrebbero avere, dipendentemente dalla impostazioni settate
per il parametro in oggetto, le seguenti possibilità:

-) **Attuale**: vengono considerati gli articoli appartenenti alle
categorie R222, R2221, R22211, R22212, R2222

-) **Padre**: vengono considerati gli articoli appartenenti alle
categorie R22, R221, R222, R2221, R22211, R22212, R2222, R223

**ATTENZIONE! Nel caso in cui il componente "Popolarità Prodotto" sia
stato inserito all'interno di una Pagina Generica verranno visualizzati
sempre e comunque tutti gli articoli che soddisfano le condizioni
definite mediante il parametro "Tipologia", indipendentemente da quanto
impostato per il campo "Categoria".**

**Prodotti Random:** consente se selezionato, e nel caso in cui
all'interno del componente non dovesse essere presente, sulla base di
quanto impostato per il precedente parametro "Tipologia", nessun
articolo, di visualizzare comunque una serie di articoli casuali che
soddisfino sempre eventuali ulteriori condizioni impostate mediante i
parametri "Categoria" e "Filtro Articoli".

**ATTENZIONE!** Il numero massimo di articoli visualizzabili con questa
opzione è uguale al valore specificato per il parametro "Numero di
articoli da visualizzare"

**Tipologia di visualizzazione:** come per il componente Catalogo
Ecommerce, anche in questo caso consente di definire la tipologia del
contenitore degli articoli che dovrà essere pubblicato all'interno del
sito.

È possibile selezionare uno dei seguenti valori:

- **Griglia:** selezionando questa opzioni gli articoli presenti
  all'interno del componente verranno visualizzati in una griglia
  paginata perfettamente responsiva e organizzata su di un certo numero
  di righe e di colonne impostabili mediante i successivi parametri
  presenti all'interno di questa stessa maschera di configurazione

- **Slider:** selezionando questa opzione gli articoli presenti
  all'interno del componente verranno disposti su di un\'unica riga
  all'interno di uno slider a scorrimento orizzontale.

**Numero massimo di slide caricabili (solo per configurazioni di tipo
Slider):** consente di impostare il numero massimo di slide che dovranno
essere caricate all'interno del componente.

**ATTENZIONE! Un numero troppo elevato di slide potrebbe rallentare il
caricamento del componente**

**Autoplay (solo per configurazioni di tipo Slider):** consente di
decidere se abilitare o meno l'autoplay dello slider.

Se impostato sul valore "**Si avvia lo slider al caricamento**", al
caricamento della pagina web verrà attivato lo scorrimento automatico
delle varie Slide.

Se impostato a **NO** per passare da una Slide all'atra sarà necessario
cliccare su uno dei controlli di scorrimento abilitati.

**ATTENZIONE!** una volta abilitato l'autoplay, occorre comunque
ricordare che nel momento in cui l'utente dovesse decidere di cliccare
sui pulsanti di controllo, lo scorrimento automatico verrà arrestato.

**Tempo di pausa per autoplay (ms)**: visibile solo nel caso in cui il
precedente parametro "Autoplay" sia stato impostato sul valore "SI avvia
lo slider al caricamento".

Consente di impostare l'intervallo di tempo (in millisecondi) che dovrà
intercorrere tra il passaggio da una Slide all'altra.

**Tempo di animazione:** consente di impostare la durata, in
millisecondi, dell\'animazione di passaggio da una slide all'altra.

**Numero di Righe da Visualizzare (solo per configurazioni di tipo
griglia):** consente di impostare il numero di righe della griglia di
visualizzazione degli articoli. **Sono accettati solo valori minori o
uguali a 30**

Nel momento in cui l'esigenza dovesse essere quella di visualizzare un
numero di righe superiore a 30, si consiglia quindi di utilizzare una
paginazione di tipo "Scroll infinito (Lazy loading)"

**ATTENZIONE!** Nel caso in cui per il componente popolarità sia stata
impostata come tipologia di visualizzazione lo Slider, gli articoli
verranno disposti sempre e soltanto su di un\'unica riga

**Numero di Articoli da visualizzare:** consente di impostare il numero
di articoli per riga.

In relazione a questo parametro vanno fatte poi alcune considerazioni di
fondamentale importanza legate al comportamento responsivo del
componente.

In particolare dunque è bene ricordare che:

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  la griglia, indipendentemente dal numero di articoli che si è scelto
  di visualizzare all'interno di ogni singola riga, per risoluzioni
  **inferiori ai 992 px** verranno sempre visualizzati 2 articoli per
  riga.

Analogamente per risoluzioni **inferiori a 768 px** la griglia si
linearizzerà mostrando un articolo per ogni riga

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  lo slider, indipendentemente dal numero di articoli che si è scelto di
  visualizzare all'interno della singola riga, per risoluzioni
  **inferiori ai 992 px** lo slider mostrerà sempre e soltanto un solo
  articolo alla volta

**Posizione bottoni Slider (solo per configurazioni di tipo Slider):**
consente di decidere, selezionando una delle possibili combinazioni
presenti all'interno del corrispondente menu a tendina, dove dovranno
essere collocati i pulsanti di scorrimento dello slider.

**Visualizzazione Paginazione (solo per configurazioni di tipo
griglia):** consente di decidere se e dove visualizzare (rispetto al
Componente stesso) i collegamenti alle varie pagine del catalogo.

**Numero di Pagine (solo per configurazioni di tipo griglia):** consente
di impostare, selezionandolo dal relativo menu a tendina, il numero di
pagine che dovranno essere visualizzate nei controlli di paginazione.
Ovviamente oltre al numero indicato all'interno di questo campo nei
controlli di paginazione saranno sempre visibili anche la prima e
l'ultima pagina disponibili.

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Paginazione con Precedente e Successivo (solo per configurazioni di
tipo griglia):** se selezionato, nei controlli di paginazione, verranno
visualizzati anche i pulsanti "Precedente" e "Successivo".

Il testo di questi pulsanti è modificabile alla sezione \"Gestione
Testi/Messaggi del Sito\" e agendo sull\'elemento generico
\"Paginazione\".

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Visualizza Paginazione" sia stato impostato su di un valore diverso da
"Non Visualizzare".**

**Tipo di Paginazione per dispositivi desktop (**\>= **992px) (solo per
configurazioni di tipo griglia):** consente di definire il tipo di
paginazione da utilizzare, per il componente in oggetto, su dispositivi
desktop (risoluzione maggiore o uguale a 992px)

È possibile selezionare uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scrollbar per visualizzare i
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

**Tipo di Paginazione per dispositivi mobile (\<** **992px) (solo per
configurazioni di tipo griglia):** consente di definire il tipo di
paginazione da utilizzare, per il componente in oggetto, su dispositivi
mobile (risoluzione minore a 992px). È possibile selezionare uno dei
seguenti valori:

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

**Elementi per pagina (solo per configurazioni di tipo griglia):**
consente di indicare una lista di valori, sperati da virgole,
corrispondenti al numero di elementi che potranno essere visualizzati in
ogni singola pagina del componente. Gli unici caratteri ammessi
all'interno di questo campo sono quelli numerici (0-9) e la virgola che
dovrà essere utilizzata come carattere separatore.

Nel momento in cui questo campo dovesse essere valorizzato in maniera
corretta, sul sito verrà poi visualizzato un menu a tendina contenente
l'elenco dei valori immessi.

Selezionando uno dei valori presenti in elenco il componente verrà
ricaricato e popolato con il numero di articoli per pagina indicati
dall'utente.

**ATTENZIONE! Modificando il numero di articoli per pagina il componente
ripartirà sempre dalla prima pagina**

**Filtro Articoli:** consente di definire il filtro di visualizzazione
articoli attraverso il quale poter stabilire quali articoli dovranno
comparire o meno all'interno del componente**.** Per maggiori
informazioni relativamente alla creazione di un filtro articoli si veda
anche la sezione *"Utenti -- Gruppi Utenti Sito -- Filtri Utente e
Filtri Articolo -- Filtri Articolo"* di questo manuale

**ATTENZIONE! Eventuali filtri impostati all'interno di questo campo
sono da considerarsi in AND con quelli impostati mediante il precedente
parametro "Categoria"**

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

**Visualizza Ordinamento -- non disponibile per Raccomandazioni Clerk
--** : se selezionato, consentirà di visualizzare, lato sito, una combo
box contenente l'elenco degli elementi sulla base dei quali poter
effettuare l'ordinamento degli articoli presenti all'interno del
componente.

**ATTENZIONE!** l'ordinamento iniziale è sempre determinato sulla base
della specifica modalità di funzionamento del componente.

Va ricordato inoltre che nel momento in cui il componente dovesse essere
utilizzato per inserire all'interno del sito le Raccomandazioni Clerk,
il parametro in questione, per ovvie ragioni, non verrà visualizzato e
l'ordinamento degli articoli sarà dettato esclusivamente dalla specifica
Raccomandazione di Clerk che si è deciso di visualizzare

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
> altri.
>
> **Tale opzione risulta particolarmente utile nel momento in cui si
> dovessero utilizzare, all'interno di un componente Tab, due distinti
> componenti popolarità realizzati con layout grafici diversi per
> ottenere ad esempio il classico passaggio dal layout a griglia a
> quello a lista**
>
> In queste condizioni avendo impostato come "Identificatore" l'intera
> pagina saremo sicuri che nel momento in cui un utente dovesse, ad
> esempio, ordinare il componente a griglia in un certo modo, tale
> ordinamento verrà poi mantenuto anche nel passaggio alla
> visualizzazione a lista (e la stessa cosa vale anche per la
> paginazione e per gli elementi per pagina).

- **Nome Componente:** selezionando questa opzione l'ordinamento, la
  paginazione e gli elementi per pagina, impostati sul front end dagli
  utenti del sito, mediante gli appositi controlli verranno applicati
  solo ed esclusivamente al componente indicato

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
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali" di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, il
Componente **"**Popolarità Prodotto**" può essere considerato a tutti
gli effetti come un "Componente di tipo Contenitore.** Sarà infatti
possibile inserire al suo interno tutta una serie di campi che, per
poter esser gestiti liberamente, dovranno inevitabilmente esser trattati
a loro volta come Componenti autonomi editabili singolarmente.

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Varianti Sito Responsive -- Componenti -- Componenti di tipo
Contenitore")**

In particolare all'interno di un componente di tipo "Popolarità
Prodotto" sarà possibile inserire due differenti tipologie di
componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente. Per
  maggiori informazioni relativamente all'utilizzo di questi componenti
  si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce:** contiene quei componenti necessari per
  abilitare e gestire determinate funzionalità (es. "Aggiunta al
  Carrello") oltre che, ovviamente per inserire e gestire all'interno
  del sito determinate informazioni prelevate direttamente dal
  gestionale.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Offerte/Novità" si veda
> la corrispondente sezione di questo manuale (Varianti Sito Responsive
> -- Lista Componenti E-Commerce -- Componenti Interni ai Componenti
> Ecommerce).

L'inserimento di questi componenti all'interno del Componente
"Offerte/Novità" avviene utilizzando le solite tecniche di interazione
con l'editor (Drag and Drop o Point and Click) già esaminate all'interno
di questo manuale (per maggiori informazioni si rimanda allo specifico
capitolo di questo manuale).

In ogni caso, comunque, il Componente "Popolarità Prodotto" avrà, in
ogni sua pagina, un certo numero di celle (coincidente con quanto
precedentemente impostato per il parametro "Numero di Articoli da
Visualizzare"). **I vari componenti (siano essi Componenti Comuni o
Componenti E-Commerce) potranno essere inseriti indistintamente
all'interno di una qualsiasi di queste celle (penserà poi l'applicazione
a ripeterli, in maniera completamente automatica all'interno di tutte le
altre celle)**

