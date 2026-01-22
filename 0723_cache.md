# CACHE



**ATTENZIONE! per poter attivare la cache sul proprio sito Passweb è
necessario innanzitutto acquistare il relativo modulo all'interno di
Passstore**

Passweb offre diversi strumenti per ridurre i tempi di caricamento delle
pagine e ottimizzare così le prestazioni del proprio sito web. Tra
questi i più interessanti sono sicuramente quelli che riguardano **la
staticizzazione dei componenti e la gestione della cache**.

Il punto fondamentale in tutto ciò è rappresentato dal fatto che i siti
Passweb sono siti dinamici per cui ogni pagina del sito viene costruita
a runtime nel momento stesso in cui viene richiesta prelevando tutti i
dati necessari direttamente dal server web. Se, da una parte, questo
costituisce un enorme vantaggio perché consente, ad esempio, di
visualizzare contenuti diversi (prezzi, prodotti, condizioni commerciali
ecc...) a seconda dell'utente che sta navigano il sito, dall'altra parte
occorre anche considerare che per ogni componente presente all'interno
della pagina dovranno essere fatte, dipendentemente dalla tipologia di
componente considerata, diverse interrogazioni lato server in maniera
tale da poter prelevare i contenuti corretti e questo, ovviamente,
potrebbe aumentare i tempi di caricamento della pagina stessa.

Il fatto di **staticizzare dei componenti** migliora sicuramente questo
processo. Infatti se per determinare e visualizzare il contenuto di un
componente dinamico possono essere necessarie diverse interrogazioni
lato server, una volta staticizzato sarà sufficiente una sola query per
ottenere e visualizzare questo stesso contenuto.

D'altra parte occorre sempre considerare anche che una volta
staticizzato un componente poi i contenuti da esso visualizzati sul
front end del sito saranno sempre gli stessi indipendentemente
dall'utente che sta navigando e/o dalla pagina in cui il componente
stesso si trova. In conseguenza di ciò:

- Se il componente in esame dovesse mostrare dati diversi a seconda
  dell'utente che naviga il sito

- Se il componente dovesse essere distribuito su più pagine e, a seconda
  della pagina in cui si trova, dovesse mostrare informazioni diverse

allora, in queste condizioni, non andrebbe staticizzato perché si
correrebbe poi il rischio di visualizzare sul front end informazioni non
corrette.

**ATTENZIONE!** Per maggiori informazioni relativamente alla
staticizzazione dei componenti si veda anche quanto indicato all'interno
del relativo capitolo di questo manuale ("*Varianti Responsive --
Configurazione Componenti Caratteristiche generali -- Staticizzazione e
caricamento asincrono dei componenti*")

Il **sistema di cache** messo a disposizione da Passweb affronta sempre
lo stesso tipo di problema risolvendolo però in maniera leggermente
diversa e sicuramente più performante rispetto alla semplice
staticizzazione di un singolo componente, tenendo anche in
considerazione, se necessario, i diversi dati che dovranno poi essere
mostrati ai diversi utenti.

In sostanza una volta attivata la cache, quando un utente non
autenticato visiterà, per la prima volta, una determinata pagina del
sito, il risultato di tutte le query necessarie per costruire la pagina
(vale a dire il codice HTML della pagina stessa) oltre ad essere
utilizzato, ovviamente, per visualizzare, in quel momento, la pagina
richiesta verrà anche salvato in un apposito database, diverso da quello
del sito, il cui unico scopo è appunto quello di memorizzare e gestire i
risultati di queste query.

Ora, nel momento in cui un altro utente, ovviamente sempre non
autenticato, dovesse visitare la stessa pagina web, considerando che il
contenuto da mostrare sarà esattamente lo stesso di quello già mostrato
al visitatore precedente, il codice HTML della pagina non dovrà essere
costruito nuovamente da zero ma potrà essere prelevato direttamente, e
senza ulteriori elaborazioni, dal server di cache riducendo quindi
notevolmente il tempo di caricamento della pagina.

In queste condizioni dunque ogni volta che verrà richiesta una pagina
web, l'applicativo verificherà per prima cosa se il codice HTML di
quella pagina è già presente o meno all'interno del server di cache. In
caso affermativo la pagina verrà prelevata direttamente da qui senza
ulteriori elaborazioni, in caso negativo la stessa pagina tornerà invece
ad essere costruita in maniera dinamica effettuando tutte le query del
caso.

Per comprendere ancora meglio i vantaggi che si possono ottenere
attivando questo sistema di cache possiamo anche pensare ad una pagina
del sito contenente, tra gli altri, il componente Catalogo Ecommerce.

Il contenuto di questo componente (che articoli visualizzare, con che
prezzi, in che modo ...) di base sarà disponibile solo dopo un certo
periodo di tempo, tempo questo necessario per effettuare sul database
del sito tutta una serie di query che, tenendo conto della struttura
della pagina richiesta, dei parametri di configurazione del componente,
dell'utente che ne ha richiesto la visualizzazione ecc... daranno come
risultato proprio l'effettivo codice HTML di quel componente necessario
per visualizzarlo all'interno della pagina web.

Oltre al componente Catalogo Ecommerce, nella stessa pagina saranno poi
presenti anche altri componenti come pannelli di ricerca, menu di
categoria ecc... il cui codice HTML, come per il componente Catalogo
sarà disponibile solo dopo aver eseguito un certo numero di query.

In definitiva il tempo necessario per ottenere il codice HTML
dell'intera pagina aumenterà in relazione al numero e al tipo di
componenti presenti in quella stessa pagina.

Inoltre bisogna anche considerare che il tempo di esecuzione delle query
dipende dal tempo di elaborazione del server che ospita il sito, va da
sé dunque che questi tempi potrebbero anche aumentare se i visitatori
dovessero passare ad esempio da 10 a 100 e il sistema si dovesse trovare
quindi ad eseguire non 10 ma 100 query (indipendentemente dal fatto che
poi il risultato di quelle 10 o 100 query sia sempre lo stesso).

In assenza di cache infatti questo processo dovrà essere eseguito ogni
volta indipendentemente dal fatto che lo stesso contenuto sia già stato
richiesto o meno anche in un momento precedente.

Nel momento in cui si dovesse invece decidere di attivare il sistema di
Cache messo a disposizione da Passweb le cose potrebbero decisamente
migliorare. In questo caso infatti dopo aver effettuato, almeno una
volta, le query necessarie per ottenere il codice HTML della pagina
questo verrà memorizzato anche nel server dedicato alla gestione della
cache. Qualora un altro utente dovesse poi, successivamente, richiedere
lo stesso tipo di contenuto, questo non dovrà più attendere il tempo di
esecuzione delle query necessarie per ottenere quel risultato perché il
risultato stesso sarà già disponibile e verrà quindi prelevato
direttamente dal server di cache.

Tutto ciò porta ad un duplice vantaggio:

- Da una parte, come detto, avendo già disponibile il risultato delle
  query e quindi il codice HTML della pagina, verranno ridotti i tempi
  di attesa per la sua visualizzazione

- Dall'altra parte avremo anche una diminuzione del numero di query che
  il database del sito si troverà a dover gestire. In questo caso
  infatti, indipendentemente dal fatto di avere 10 o 100 visitatori che
  richiedono una certa pagina, il sistema eseguirà le query necessarie
  per ottenere il codice HTML una sola volta e per le restanti 9 0 99
  visite il risultato verrà prelevato (già finito) direttamente dal
  server di cache abbassando quindi il carico sul database del sito che,
  da parte sua, potrà andare a lavorare e ad utilizzare le proprie
  risorse solamente per eseguire query "nuove" che non producano cioè un
  risultato già prodotto in precedenza

Un'altra cosa di fondamentale importanza da tenere in considerazione è
il fatto che, ovviamente, il contenuto di una pagina web (pensiamo ad
esempio al prezzo degli articoli, e quindi il suo codice HTML, potrebbe
anche variare a seconda del fatto che la pagina venga richiesta da un
utente non autenticato tic oppure da un utente che ha effettuato
l'autenticazione e che avrà quindi le sue specifiche condizioni
commerciali.

In questo senso Passweb offre la possibilità di attivare anche una cache
per singolo utente, memorizzando quindi non solo le pagine che dovranno
poi essere visualizzate a tutti gli utenti non autenticati ma anche
quelle di ogni singolo utente autenticato

Ovviamente affinché il tutto possa funzionare in maniera corretta
riducendo, da una parte, i tempi di caricamento della pagina e mostrando
comunque, dall'altra parte, i contenuti corretti all'utente che li ha
effettivamente richiesti è necessario:

- **avere già a disposizione il codice HTML della pagina**.

> La cache si dovrà quindi "costruire" e potrà farlo solo mano a mano
> che il sito verrà visitato da tutte le diverse tipologie di utenti che
> possono effettivamente visualizzare un certo tipo di risultato.
>
> In tutti i casi la prima visita sarà essere più lenta perché dovrà
> attendere il tempo di esecuzione delle query necessarie per ottenere
> il risultato richiesto. Le visite successive (da parte della stessa
> tipologia di utenza o dello stesso utente autenticato) saranno invece
> più veloci inquanto potranno sfruttare il risultato già prodotto dalla
> visita precedente.

- **essere certi che il risultato presente nel server di cache, e quindi
  il contenuto effettivo che verrà poi mostrato all'utente, sia quello
  corretto**.

> Nello specifico se dopo aver prodotto un certo risultato ed averlo
> memorizzato nel server di cache dovessero poi cambiare le condizioni
> che lo hanno generato (modifica del prezzo, cambiamento delle
> impostazioni di configurazione del componente, modifica delle
> condizioni commerciali dell'utente all'interno del gestionale ...) è
> evidente che il risultato attualmente presente nel server di cache non
> sarebbe più quello corretto per cui andrebbe eliminato mettendo
> Passweb nelle condizioni ,di poterlo ricreare, a seguito della prima
> visita utile, sulla base delle nuove impostazioni.

Considerando quanto appena detto e tenendo presente che, in fin dei
conti, anche il processo di staticizzazione porta alla creazione di un
codice HTML che poi viene riutilizzato senza effettuare nuovamente le
relative query sul database, potrebbe essere lecito domandarsi se il
sistema di cache messo a disposizione da Passweb possa essere
effettivamente migliore rispetto ad un semplice processo di
staticizzazione.

In questo senso la risposta è abbastanza semplice.

Il processo di staticizzazione infatti può essere effettuato solo da
backend e pertanto il risultato prodotto sarà sempre lo stesso
indipendentemente dalla particolare tipologia di utenza che andrà poi a
richiederlo.

Questo fa sì che staticizzando determinati componenti come il catalogo
ecommerce, la scheda articolo ..., è altamente probabile che il
risultato prodotto non possa poi andar bene per tutte le tipologie di
utenza e, in conseguenza di ciò, determinati utenti potrebbero quindi
trovarsi a visualizzare un dato non corretto.

La cache mette invece a disposizione una sorta di "staticizzazione
dinamica" nel senso che la generazione del codice HTML che verrà poi
utilizzato come risultato da mostrare anche ad altri utenti avviene in
maniera dinamica a seguito di visite ricevute direttamente sul front end
del sito e questo fa sì che possano essere memorizzati e messi in cache
anche risultati diversi per utenti diversi.

In queste condizioni dunque eventuali condizioni commerciali, filtri
articoli ecc ... attivi solo per determinati utenti continueranno ad
essere validi anche nel momento in cui il dato dovesse essere prelevato
direttamente dalla cache.

**ATTENZIONE!** Per evitare problemi si consiglia di non attivare
contemporaneamente staticizzazione e cache.

Nel momento in cui si dovesse infatti decidere di attivare la cache,
l'unico vantaggio che si potrebbe avere nell'utilizzare anche la
staticizzazione dei componenti (considerando tra l'altro che componenti
quali ad esempio il catalogo ecommerce sono difficilmente
staticizzabili) potrebbe essere solamente quello di velocizzare il primo
accesso alla pagina e conseguentemente la creazione della relativa
cache.

Riassumendo l'utilizzo del sistema di cache messo a disposizione da
Passweb ha, indubbiamente, i suoi vantaggi, tra cui ad esempio:

- Riduzione dei tempi di caricamento della pagina

- Diminuzione del numero di query gestite dal database del sito

- Possibilità di memorizzare e riutilizzare risultati diversi per utenti
  diversi

- ...

D'altra parte occorre comunque considerare che possono essere presenti
anche degli "aspetti negativi" che andranno quindi opportunamente
valutati prima di attivare il relativo modulo. Ad esempio:

- La cache del sito si costruisce in maniera automatica mano a mano che
  il sito stesso riceve delle visite, per cui i benefici apportati da
  questa gestione potrebbero non essere immediatamente visibili per
  determinati utenti e/o per determinate pagine.\
  Allo stesso modo se i contenuti dovessero essere altamente dinamici
  (es. modifica dei prezzi più volte al giorno) la cache potrebbe non
  fare in tempo a costruirsi per cui i benefici apportati da questo
  sistema potrebbero non essere evidenti

- Non tutte le pagine possono essere interamente cachate, principalmente
  a causa dei componenti che andranno a contenere. Componenti come il
  Carrello o il Checkout, dovranno per forza di cose essere creati
  sempre in maniera dinamica

- Ogni qual volta dovessero essere effettuate delle modifiche lato back
  end / gestionale a dati memorizzati in cache sarà poi necessario
  eliminare dalla cache i dati vecchi per fare in modo che la cache
  possa essere ricostruita e che gli utenti possano quindi visualizzare
  sempre il dato correttamente aggiornato.

Nei successivi capitoli di questo manuale verranno analizzati più nel
dettaglio i diversi aspetti di gestione della cache, come abilitarla,
come poter eliminare (flush) i dati memorizzati, come poter lanciare un
crawler per la creazione automatica di un massimo di 100 pagine di cache
ecc...

