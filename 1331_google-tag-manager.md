# GOOGLE TAG MANAGER



Il primo Ottobre 2012, all'eMetrics Summit di Boston, Google ha
presentato un nuovo strumento a supporto delle attività di web
analytics: il **Google Tag Manager (GTM).**

Per poter comprendere appieno cosa sia questo strumento, come possa
essere utilizzato e i vantaggi che se ne potrebbero effettivamente
trarre la prima domanda alla quale rispondere è, ovviamente, che cos'è
un TAG.

In ambito di web analytics, **con il termine TAG si tende ad indicare un
qualsiasi snippet di codice Javascript inserito all'interno del proprio
sito ed utilizzato per inviare dati e informazioni a strumenti di terze
parti** (come ad esempio a Google Analytics)

Detto questo è ora abbastanza semplice comprendere come, nella
realizzazione di un sito web, ci si possa trovare, molto probabilmente,
di fronte alla necessità di dover gestire numerosi Tag come possono
essere ad esempio gli script di Google Analytics, i codici di
Remarketing, di Google AdWords ecc...

Normalmente tutti questi Tag, o meglio il codice javascript necessario
per gestire ciascuno di essi, andrebbe implementato ed inserito
direttamente nelle pagine del sito in cui questi stessi Tag dovranno poi
essere effettivamente utilizzati e questo tipo di operazione potrebbe
comportare necessariamente un intervento, da parte degli sviluppatori
del sito, sul codice sorgente delle pagine web.

**Un Tag Manager è uno strumento che consente di astrarre di un livello
la messa in produzione e la modifica di questi Tag**.

In altri termini invece di operare direttamente sul codice sorgente
delle singole pagine, si applica un unico Tag (quindi un unico
pezzettino di codice javascript) , il cosiddetto **TAG CONTENITORE,** ad
inizio progetto e a tutte le pagine del sito.

Successivamente l'implementazione di nuovi Tag e/o la modifica di Tag
precedentemente inseriti verrà gestita completamente all'esterno del
sito, mediante l'interfaccia web messa a disposizione dal Tag Manager
stesso.

Con **Google Tag Manager (GTM)** è quindi sufficiente inserire
**un\'unica volta, un singolo script di codice, in tutte le pagine del
sito** e utilizzare poi la sua interfaccia web per decidere,
dinamicamente, quale Tag inserire in quale pagina e quando eseguirlo.

Google Tag Manager inoltre, mette a disposizione dell'utente anche tutta
una serie di Tag predefiniti che semplificano ulteriormente il lavoro di
chi deve gestire questo tipo di informazioni. Per aggiungere, ad
esempio, un tag di base di Google Analytics, senza alcuna
personalizzazione, è sufficiente selezionare il modello appropriato e
incollare il relativo ID di monitoraggio. Altri modelli predefiniti
possono essere quelli relativi ai codici delle conversioni di AdWords o
al remarketing.

In ogni caso sarà sempre possibile definire un Tag personalizzato
incollando il codice necessario direttamente nell'interfaccia web di GTM
piuttosto che all'interno del codice sorgente delle pagine del proprio
sito.

I Tag generati mediante GTM vengono poi eseguiti basandosi su delle
regole, chiamate più esattamente **Attivatori,** e che servono appunto
per dire al Tag Manager dove e quando eseguire un Tag piuttosto che un
altro. Possono essere creati Attivatori del tipo:

- esegui il Tag in tutte le pagine

- esegui il Tag tutte le pagine tranne...

- esegui il Tag solo se l' url della pagina contiene xyz

- esegui il Tag solo se viene scatenato un certo evento

- esegui il Tag solo se il referrer è...

- ...

Ogni Attivatore sarà poi composto da Variabili, Condizioni e Valori.

Combinando insieme Attivatori e Variabili è possibile identificare
puntualmente le condizioni sulla base delle quali scatenare un Tag
piuttosto che un altro, anche in modo molto complesso: arrivo sulla
pagina x dal referrer y, e se una certa variabile javascript ha un
determinato valore, estraggo dal DOM una stringa e la passo al tag
manager che la scrive nel tag di remarketing di AdWords.

Per quanto l'interfaccia del GTM possa essere semplice ed intuitiva,
come in tutte le cose, l'effettiva semplicità è dettata dalla
complessità di ciò che si vuole effettivamente realizzare.

In questo senso, visto e considerato che il grado di complessità cui si
può arrivare può essere anche piuttosto elevato, il GTM consente di
gestire anche il **versioning dei tag,** cosa questa estremamente utile
perché in caso di problemi con un solo click si può tornare indietro di
una o più versioni, ripristinando tutti i Tag all'ultima situazione
sicuramente funzionante.

Il versioning funziona inoltre anche per le versioni non ancora messe in
produzione.

Una volta effettuate delle modifiche è quindi possibile creare una nuova
versione del Tag Contenitore e pubblicarla in una "Sandbox", in maniera
tale che il tutto funzioni soltanto sui browser abilitati da chi ha
creato la versione di quello specifico Tag.

Questo permette quindi di poter testare "dal vivo" le proprie modifiche
e di passare effettivamente all'ambiente di produzione pubblicando in
maniera definitiva il proprio Tag solo se tutto funziona correttamente.

Una volta compreso che cos'è e come funziona il GTM, i vantaggi che si
possono ottenere da un suo corretto utilizzo sono piuttosto evidenti. Ad
esempio:

- **Gestione centralizzata degli script** e facilità di
  modifica/aggiunta/eliminazione dei tag senza intervenire nel codice
  sorgente della pagina web

- **Interfaccia utente semplice e intuitiva**

- **Maggiore velocità di caricamento del sito** grazie all'utilizzo di
  un unico script asincrono

- **Preview Mode**, per l'anteprima sul funzionamento dei tag

- **Versioni**: tutti i tag vengono memorizzati e possono essere
  ripristinati in qualsiasi momento in caso di problemi o errori;

- **Livelli di accesso diversificati per la gestione** e/o
  visualizzazione dei tag;

- **Configurazione avanzate attraverso a definizione di Regole e
  Macro**.

Nei successivi capitoli di questo manuale prenderemo in considerazione
la struttura di un Account di Google Tag Manager analizzando un po' più
nel dettaglio quelli che sono i suoi elementi principali (Tag,
Attivatori, Variabili, Data Layer ecc...) per poi passare poi ad
elencare i vari step necessari per attivare ed utilizzare Google Tag
Manager all'interno di un sito Passweb.

**ATTENZIONE! In ogni caso per maggiori informazioni sullo strumento
Google Tag Manager si consiglia di fare sempre riferimento alla relativa
documentazione presente in rete (
<https://support.google.com/tagmanager/?hl=it#topic=3441530> )**

