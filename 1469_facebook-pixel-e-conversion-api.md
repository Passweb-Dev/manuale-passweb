# FACEBOOK PIXEL E CONVERSION API



Il sistema di tracciamento messo a disposizione da Facebook prevede che
i diversi eventi (visualizzazione di pagine, aggiunta articoli in
carrello, acquisto ecc...) possano essere tracciati in due modi diversi:

- lato **Client** -- mediante Facebook Pixel.

> In questo caso sarà il browser dell'utente che si occuperà di inviare
> ai server di Facebook tutte le informazioni necessarie per poter
> tracciare i diversi eventi. Affinchè tutto questo possa avvenire in
> maniera corretta sarà necessario, generalmente:

- essere in possesso dell'ID di un Pixel di Facebook appositamente
  creato all'interno del proprio Business Manager (è l'equivalente dell'
  "ID Misurazione" necessario per implementare il tracciamento lato
  client di Google Analytics)

- inserire sul sito web il codice javascript necessario per fare in modo
  che il browser dell'utente possa effettivamente inviare ai server di
  facebook i dati relativi agli eventi da tracciare.

<!-- -->

- lato **Server** -- mediante Conversion API .

> In questo caso tutte le informazioni necessarie per tracciare i
> diversi eventi che si verificano sul sito verranno inviate a facebook
> direttamente dall'applicazione utilizzata per realizzare e gestire il
> sito (e quindi direttamente dal server su cui il sito stesso è
> hostato).
>
> Affinchè tutto questo possa avvenire in maniera corretta sarà
> necessario, generalmente:

- essere in possesso di un "Access Token" appositamente generato
  all'interno del proprio Business Manager (come il Pixel ID, questo
  Access Token altro non è se non la chiave che consente di mettere in
  comunicazione il nostro sito con il sistema di tracciamento di
  Facebook)

- configurare adeguatamente l'applicazione, il plugin o il modulo
  utilizzato per implementare questo tipo di tracciamento

> In queste condizioni, generalmente, non dovrà essere inserito nessun
> codice javascript all'interno del sito ma ci si dovrà preoccupare
> solamente di configurare in maniera corretta l'applicazione o il
> modulo utilizzato per implementare questo tipo di tracciamento

Fatte queste considerazioni di carattere generale, possiamo ora
evidenziare come all'interno del proprio sito Passweb sia effettivamente
possibile decidere di attivare ed implementare il tracciamento di
Facebook solo mediante Pixel (quindi solo lato client), solo mediante
Conversion API (quindi solo lato server) oppure utilizzando
contemporaneamente sia il Pixel di Facebook che le Conversion API

Nei successi capitoli di questo manuale verranno quindi illustrate, più
nel dettaglio, le procedure da seguire per poter attivare e gestire il
tracciamento di Facebook sia lato client che lato server

**ATTENZIONE!** In ogni caso il presente manuale non è una guida
completa, esaustiva ed aggiornata del Business Manager di Facebook. In
conseguenza di ciò per maggiori informazioni relativamente a come poter
impostare e configurare il Business Manager per quel che riguarda sia la
generazione del Pixel di Facebook che l'attivazione delle Conversion API
con generazione del relativo Access token, si consiglia di fare sempre
riferimento alla relativa documentazione presente direttamente sui siti
di Facebook.

