# FLUSH DELLA CACHE



Come evidenziato nei precedenti capitoli di questo manuale l'utilizzo
della cache può essere uno strumento molto utile per incrementare le
prestazioni del proprio sito. Una volta attivata e costruita la cache
infatti la maggior parte dei dati richiesti dalle pagine web verranno
prelevati direttamente da essa senza andare ad effettuare interrogazioni
sul db del sito facendo quindi diminuire i tempi di caricamento delle
pagine.

D'altra parte occorre però considerare anche che una volta attivata la
cache nel momento in cui dovessero poi essere effettuate delle
modifiche, lato back end o a seguito di una sincronizzazione "sito --
gestionale", ai dati da visualizzare all'interno di una pagina web,
queste modifiche verranno ovviamente salvate e memorizzate sul database
del sito (**NON** nella cache).

E' semplice comprendere quindi come in queste condizioni il dato
prelevato dalla cache potrebbe anche non essere correttamente aggiornato
con quello presente nel database.

**In queste condizioni diventa quindi di fondamentale importanza poter
resettare il contenuto della cache in maniera tale che questa possa poi
essere ricostruita con i dati correttamente aggiornati.**

Una volta effettuato il flush infatti le successive richieste di
visualizzazione delle pagine non trovando i dati all'interno della cache
andranno automaticamente a prelevarli dal database del sito e a
memorizzarli nuovamente, per le future richieste, all'interno della
cache che tornerà quindi ad essere aggiornata con i dati corretti.

Tenendo conto di quanto appena detto, dunque, è abbastanza semplice
comprendere che:

- **il processo di creazione della cache non è istantaneo**. Mano a mano
  che il sito riceverà delle visite i dati richiesti verranno
  memorizzati in cache diventando quindi disponibili per eventuali
  future richieste

- **ogni qual volta dovessero essere effettuate delle modifiche lato
  back end / gestionale a dati da visualizzare all'interno di una
  pagina** potrebbe essere necessario resettare la cache in maniera tale
  che questa possa poi essere ricostruita con i dati correttamente
  aggiornati

In quest'ultimo caso per verificare se le eventuali modifiche apportate
ai contenuti o ai parametri di configurazione del sito richiedano
effettivamente un reset della cache sarà sufficiente accedere alla
pagina "**Gestione Cache**" del Wizard e controllare la colonna
"**Variata**" presente all'interno della sezione "**Tipologie di
Cache**"

![Videate\\gestione_cache_6.bmp](./assets/media/image266.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

**ATTENZIONE!** Nel momento in cui l'icona della piccola batteria
visualizzata in corrispondenza della cache di pagina dovesse essere
colorata di rosso, questo starà ad indicare la necessità di svuotare la
cache per fare in modo che gli utenti possano visualizzare sul front end
del sito i dati correttamente aggiornati.

Inoltre nel momento in cui dovesse esserci la necessità di effettuare il
reset della cache Passweb segnalerà tale esigenza visualizzando l'icona
della piccola batteria rossa anche nella parte alta del menu principale
del Wizard

![Videate\\gestione_cache_7.bmp](./assets/media/image267.png){width="5.746527777777778in"
height="3.5194444444444444in"}

Tenendo conto di tutto quanto detto fino ad ora un'osservazione molto
importante da fare è sicuramente quella che riguarda l'utilizzo della
cache in relazione alla dinamicità del proprio sito.

**Se i dati del sito (es. prezzi, immagini, informazioni articolo ...)
dovessero variare più volte al giorno, gli intervalli di tempo, tra un
flush e l'altro, potrebbero anche non essere sufficienti a ricostruire
la cache con i dati correttamente aggiornati**. In queste condizioni
ovviamente i benefici apportati dall'attivazione della cache potrebbero
essere minimi (considerando che il dato nel 90% dei casi verrà prelevato
dal database) e potrebbe quindi essere il caso di valutare altre
soluzioni per cercare di ottimizzare le prestazioni del proprio sito.

Per quel che riguarda invece il flush della cache, come evidenziato nei
precedenti capitoli di questo manuale, è possibile operare in tre modi
diversi **manuale, temporizzato e automatico** dipendentemente dalle
impostazioni settate per il parametro **Flush** presente all'interno
della maschera "Gestione Cache"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flush_cache_1.bmp](./assets/media/image268.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

**ATTENZIONE!** **indipendentemente dal fatto di operare in modalità
manuale, automatica o temporizzata nel momento in cui di dovesse partire
un reset della cache quando ci sono delle sessioni attive sul front end
del sito, per queste stesse sessioni la cache verrà automaticamente
disabilitata mentre continuerà ad essere correttamente gestita per le
nuove sessioni (quelle attivate dopo il reset).**

Ciò significa dunque che eventuali utenti che stavano navigando il sito
durante un'operazione di reset della cache continueranno la loro
sessione di navigazione con la cache disabilitata (indipendentemente
dalle impostazioni settate all'interno del Wizard). Questo perché le
sessioni che si sono attivate prima del reset potrebbero avere delle
impostazioni differenti rispetto ai motivi per cui è stato avviato il
reset e si correrebbe quindi il rischio di visualizzare, per loro, dei
dati non corretti. Disabilitando la cache si avrà invece la certezza che
fino al termine della loro sessione di navigazione le pagine
visualizzate (essendo costruite in maniera dinamica, effettuando tutte
le query del caso sul db del sito) mostrino effettivamente i dati
corretti.

Per le sessioni di navigazione avviate dopo l'operazione di reset questo
problema non sarà ovviamente presente, per cui per esse si potrà
continuare a gestire la cache in maniera normale.

Nei successivi capitoli vedremo più nel dettaglio le caratteristiche ed
il funzionamento delle tre diverse opzioni di flush.

