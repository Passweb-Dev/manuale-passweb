# VERIFICA DEL TRACCIAMENTO



Per verificare che il tracciamento di Facebook sia stato implementato in
maniera corretta è possibile utilizzare diversi strumenti che possono
variare in relazione al fatto di prendere in considerazione solo il
tracciamento lato client, solo quello lato server o entrambi.

Nello specifico, se prendiamo in considerazione il tracciamento lato
client e consideriamo che, come ormai noto, esso si esplicita
direttamente sul browser dell'utente che visita il sito mediante
l'esecuzione di determinate istruzioni javascript (oltre all'utilizzo di
determinati cookie installati da facebook stesso sempre sul browser
dell'utente), lo strumento migliore che abbiamo a disposizione per
testarne il corretto funzionamento è, indubbiamente, il "**Facebook
Pixel Helper**", un estensione per Chrome (e in generale per i browser
webkit) che consente di controllare la presenza o meno del Pixel di
Facebook in una determinata pagina del sito, di verificare se
nell'implementazione effettuata sono stati commessi o meno degli errori
(es. pixel duplicato, impossibile caricare il pixel, id pixel non valido
ecc...), quali eventi vengono effettivamente tracciati e quali sono i
parametri, e quindi i dati, inviati a facebook con ogni evento ...

Il Pixel Helper può essere installato a partire da questo link

<https://chrome.google.com/webstore/detail/facebook-pixel-helper/fdgfkebogiimcoedlicjlajpkdmockpc>

Una volta attivata l'estensione vedremo comparire l'icona del Pixel
Helper alla destra della barra di ricerca del browser. L'icona sarà
grigia nel caso in cui non venga rilevato nessun pixel.

![](./assets/media/image37.png)

Nel momento in cui dovesse invece essere rilevata nella pagina la
presenza di un pixel di facebook l'icona del pixel helper si attiverà
diventando di colore blu

![](./assets/media/image38.png)

In questo caso cliccando su di essa si aprirà un piccolo pop up
all'interno del quale potremo trovare diverse informazioni relative al
pixel rilevato come ad esempio l'ID del pixel stesso, il suo tempo di
caricamento, l'URL della pagina ...

![](./assets/media/image39.png)

oltre che ovviamente agli specifici eventi tracciati con questo stesso
pixel e ai parametri passati con l'evento stesso.

![](./assets/media/image40.png)

Il consiglio dunque è quello di testare tutti gli eventi gestiti
completando le varie azioni (es. aggiunta di articoli in carrello,
completamento di un' ordine, aggiunta di articoli alla wishlist ...) che
dovrebbero effettivamente attivare il pixel e inviare i dati a Facebook.

Nel momento in cui a fianco dei diversi eventi rilevati dal pixel helper
dovesse comparire una spunta verde, potremo assumere che il tracciamento
lato client funzioni in maniera corretta e che quindi i browser degli
utenti che visitano il sito (e che ovviamente hanno prestato tutti i
consensi del caso) inviino correttamente i dati ai server di facebook.

Se al contrario a fianco di un determinato evento dovesse comparire
un'icona gialla (warning) o rossa (problema), qualcosa nel tracciamento
lato client di quel determinato evento non avrà funzionato in maniera
corretta. Potremo quindi aprire il dettaglio di quell'evento per
verificare cosa effettivamente non funzioni e agire poi di conseguenza

![](./assets/media/image41.png)

Un altro strumento particolarmente utile per verificare che tutto
funzioni in maniera corretta è quello rappresentato dalla sezione
"**Testa gli eventi**" presente direttamente sul Business Manager di
Facebook (sezione "**Gestione Eventi**"), sezione questa che rappresenta
una sorta di raccolta degli eventi in tempo reale

![](./assets/media/image42.png)

All'interno di questa sezione è infatti possibile testare la corretta
ricezione da parte di Facebook di tuti gli eventi (e relativi parametri)
inviati con il pixel in esame sia lato client che lato server.

Nello specifico per testare e verificare la corretta ricezione degli
eventi inviati lato client sarà sufficiente aprire e navigare il sito,
**con lo stesso browser con cui è già stato aperto il Business
Manager.** Per far questo potremo quindi inserire l'indirizzo del sito
direttamente all'interno del campo "**Inserisci l'URL del sito web**"
presente nel box "**Testa gli eventi del browser**" e cliccare poi sul
pulsante "**Apri il sito web**" in maniera tale da aprire il sito
indicato in una nuova tab dello stesso browser.

![](./assets/media/image43.png)

A questo punto ricaricando il tab in cui è stato aperto lo strumento
"Testa gli eventi" e iniziando a navigare il nostro sito, se tutto
funziona in maniera corretta, dovremmo veder arrivare i diversi eventi
raccolti dal pixel installato sul sito stesso

![](./assets/media/image44.png)

Per ciascuno degli eventi raccolti sarà possibile visualizzare:

- il nome dell'evento (es. Aggiunta al carrello)

- se l'evento è stato generato da un tracciamento lato client o lato
  server (campo "Ricevuto da")

- il metodo di configurazione del pixel utilizzato (nel nostro caso sarà
  sempre "Configurazione manuale")

- l'ID evento inviato

- la data di ricezione

Inoltre cliccando su uno degli eventi presenti in elenco sarà possibile
visualizzare anche il dettaglio di tutti i parametri (con relativi
valori) che sono stati inviati a facebook assieme all'evento stesso

![](./assets/media/image45.png)

Nel momento in cui l'esigenza dovesse invece essere quella di testare e
verificare la corretta ricezione degli eventi inviati lato server sarà
necessario, per prima cosa, copiare il "**test_event_code**" presente
all'interno del box "**Testa gli eventi server**"

![Videate\\facebook_test_event_code.bmp](./assets/media/image46.png)

e incollarlo poi all'interno del campo "**Codice di Test**" presente
alla pagina "**Sito -- Preferenze**" del Wizard, tab "**Tracciamento
Dati**" sezione "**Facebook Pixel -- Conversion API**"

![](./assets/media/image47.png)

**ATTENZIONE!** il codice in esame non è sempre lo stesso, per cui va
prelevato dal Business Manager di Facebook, ed inserito nel relativo
campo Passweb solo nel momento in cui si desideri effettuare dei test
sul tracciamento lato server.

Una volta inserito il codice, questo verrà infatti aggiunto
automaticamente al payload inviato da Passweb a Facebook al verificarsi
di ogni evento server effettivamente tracciabile (aggiunta al carrello,
acquisto

**ATTENZIONE! Una volta completati i test è necessario rimuovere il
codice inserito**

A questo punto, come già per la verifica del tracciamento lato client,
potremo utilizzare un nuovo tab dello stesso browser con cui è già stato
aperto il Business Manager, per navigare il nostro sito e, anche in
questo caso, se tutto funziona correttamente dovremmo veder arrivare
nella sezione "Testa gli eventi" i diversi eventi inviati a facebook,
questa volta però non dal browser degli utenti, ma direttamente
dall'applicativo e quindi dal server su cui è hostato il sito.

![](./assets/media/image48.png)

In queste condizioni dunque, in corrispondenza della colonna "Ricevuto
da" dovremo trovare per ogni singolo evento il valore "Server" ad
ulteriore testimonianza del fatto che l'evento registrato da facebook
non è stato inviato dal browser di un utente ma direttamente dal server
che ospita il sito.

Infine, un ultimo test particolarmente interessante che potremo fare
utilizzando sempre lo strumento "Testa gli eventi" è quello che ci
consente di verificare, nel momento in cui dovessimo aver attivato
contemporaneamente sia il tracciamento lato client che quello lato
server, che il sistema di deduplica utilizzato da facebook funzioni in
maniera corretta e che quindi lo stesso evento inviato sia lato server
che lato client venga di fatto conteggiato una sola volta.

Per poter effettuare questo tipo test dovremo verificare, prima di
tutto, di aver effettivamente attivato all'interno di Passweb sia il
tracciamento lato client (parametro "Tracciamento Client" selezionato)
che quello lato server (campo "Access Token" correttamente compilato) e
di aver inserito all'interno del campo "Codice di test" anche il
"test_event_code" attualmente presente nella sezione "Testa gli eventi"
del Business Manager di Facebook.

In queste condizioni navigando il sito, come sempre da un nuovo tab
dello stesso browser con cui è già stato aperto il Business Manager,
nella sezione "Testa gli eventi", se tutto funziona correttamente,
dovremmo trovarci di fronte ad una situazione del tipo di quella
evidenziata in figura

![](./assets/media/image49.png)

situazione questa che evidenzia come di fatto lo stesso evento (es.
PageView) sia stato inviato a Facebook sia lato client che lato server
(colonna ricevuto da) e come però i due eventi siano stati raggruppati e
processati in maniera tale da essere conteggiati una sola volta.
Osservando la figura si può infatti notare che l'evento server è stato
deduplicato e solo quello browser è stato correttamente elaborato e
conteggiato.
