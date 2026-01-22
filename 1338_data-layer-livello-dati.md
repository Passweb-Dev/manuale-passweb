# DATA LAYER (LIVELLO DATI)



Nei precedenti capitoli di questo manuale abbiamo visto come un
Attivatore altro non sia, in definitiva, se non un insieme di
condizioni, dettate da specifici Filtri, che dovranno essere valutate
allo scatenarsi di un certo evento, confrontando, con la logica indicata
da un ben preciso Operatore, un Valore indicato in fase di
configurazione del Filtro con lo stesso tipo di informazione memorizzata
a runtime all'interno di un'apposita Variabile

Il Tag relativo ad una conversione per una prenotazione di un sito hotel
ad esempio, dovrebbe essere attivato all'interno della pagina di
conferma della prenotazione. Il suo Attivatore dovrà quindi essere
definito in modo tale che la variabile predefinita url corrisponda
proprio a tale pagina.

Abbiamo anche visto poi che oltre alle Variabili predefinite messe a
disposizione da GTM, è sempre possibile utilizzare anche delle Variabili
personalizzate ciascuna delle quali dovrà contenere specifiche
informazioni al momento dell'attivazione del Tag e, soprattutto, abbiamo
anche detto che le Variabili, siano esse predefinite o personalizzate
possono non solo essere utilizzate negli Attivatori ma possono anche
essere trasmesse ai Tag.

In questo modo è possibile, ad esempio, definire una Variabile
personalizzata contenente l'importo di una transazione e trasmettere poi
questo valore anche ad un Tag di monitoraggio delle conversioni ad
esempio un Tag DoubleClick o Google Analytics, consentendo così ai
rapporti generati dai relativi strumenti di analisi di mostrare anche il
valore delle entrate delle transazioni.

Ora va anche detto però che, per implementare una funzionalità come
questa è necessario, generalmente, chiedere allo sviluppatore del sito
di impostare, nella pagina di conferma della transazione, uno specifico
**Data Layer o Livello Dati** che contenga proprio questa Variabile
personalizzata con il totale della transazione.

E' in questo Livello di Dati infatti che GTM e, nel caso specifico, il
Tag per il monitoraggio delle conversioni, andranno a cercare e a
prendere il dato di cui hanno bisogno e che deve essere trasmesso al
relativo strumento di analisi

**Il Data Layer, dunque, è lo strumento utilizzato per trasmettere le
informazioni dalle pagine web del nostro sito a GTM e a tutti i Tag del
Contenitore (e tramite essi ai relativi strumenti di analisi di terze
parti)**

In realtà i Tag utilizzati all'interno del nostro sito potrebbero anche
reperire le informazioni di cui hanno bisogno senza cercarle nel Data
Layer ma andandole a prendere direttamente nel DOM della pagina web.
Questo però potrebbe anche causare dei problemi nel momento in cui la
struttura HTML della pagina dovesse cambiare, ad esempio, a seguito di
un aggiornamento del sito.

Per comprendere meglio questo concetto e l'importanza del Data Layer
possiamo fare una semplice analogia.

Pensiamo al nostro sito come ad un ristorante in cui i Tag sono i
clienti, i dati sono il cibo e il Data Layer è il buffet. Preparare
correttamente il buffet fa si che tutti i clienti possano prendere
immediatamente quello di cui hanno bisogno senza dover aspettare di
ordinare direttamente ai camerieri.

Senza il buffet, al contrario, i clienti dipenderanno direttamente dai
camerieri per ottenere ciò di cui hanno bisogno. E' vero che se
pensassimo di assegnare tutte le volte lo stesso tavolo e lo stesso
cameriere allo stesso cliente poterebbe instaurarsi una routine tale per
cui i tempi di attesa potrebbero anche ridursi al minimo, poi però se un
giorno dovessimo decidere di ristrutturare il ristorante e di cambiare
camerieri i clienti, abituati alla precedente routine, potrebbero essere
confusi e potrebbero anche non riuscire a trovare il proprio tavolo e il
proprio cameriere fintanto che non gli vengano date nuove istruzioni.

La stessa cosa potrebbe succedere per i Tag che prendono le informazioni
di cui hanno bisogno direttamente dal HTML della pagina web. Se un
domani la struttura della pagina dovesse cambiare, ad esempio a seguito
di un semplice aggiornamento del sito, poi questi Tag potrebbero non
trovare più le informazioni di cui hanno bisogno smettendo quindi di
trasmettere i dati allo strumento di analisi ad essi collegato.

**L'utilizzo di un Data Layer rimuove questo tipo di problemi perché, di
fatto, separa i dati necessari ai Tag dalla struttura della pagina.**

Il Livello Dati sarà sempre lo stesso indipendentemente da quelle che
sono le modifiche che possono avvenire o non avvenire sulla struttura
HTML della pagina e quindi i Tag potranno usufruire di una sorgente dati
costante da cui poter andare a prendere quello di cui hanno bisogno
quando ne hanno bisogno.

**Da un punto di vista tecnico il Data Layer altro non è se non un
semplice oggetto Javascript, denominato dataLayer, che, mediante
l'utilizzo delle Variabili precedentemente esaminate, racchiude tutte le
informazioni da trasmettere a GTM e ai Tag del Contenitore.**

Un Data Layer vuoto sarà dunque un semplice oggetto javascript del tipo
di quello qui di seguito riportato

\<script\>

dataLayer = \[{

}\];

\</script\>

**ATTENZIONE!** Volendo è anche possibile modificare e personalizzare il
nome dell'oggetto javascript. Questo però richiede anche un'analoga
modifica da apportare al codice del Tag Contenitore

Per quanto detto, ovviamente, un Data Layer vuoto non servirà a molto.
Supponendo dunque di voler mettere in questo Livello Dati delle
Variabili che ci consentano di categorizzare la pagina del sito in cui è
inserito come la pagina di Login e di indentificare il relativo
visitatore come un utente piuttosto importante potremmo valorizzare ed
inserire nel Data Layer determinate Variabili come, ad esempio, di
seguito indicato

\<script\>

dataLayer = \[{

'pageCategory': 'Login,

'visitorType': 'high-value'

}\];

\</script\>

All'interno di un Data Layer, inoltre, possono essere inserite sì delle
informazioni statiche come la categoria di una pagina, il suto titolo
ecc... Allo stesso modo però possono anche essere inserite, soprattutto,
delle informazioni dinamiche che magari non si hanno a disposizione
immediatamente al caricamento della pagina ma solo a seguito di una
qualche interazione tra l'utente e la pagina stessa.

Supponiamo, ad esempio, che un visitatore del sito inserisca determinati
dati nei campi di un form, ad esempio il suo paese preferito, e
supponiamo di voler inviare questa informazione ad un certo strumento di
analisi utilizzando per questo un apposito Tag. Ovviamente al
caricamento della pagina non siamo ancora in possesso di questa
informazione e non possiamo quindi inserirla immediatamente nel Data
Layer.

Potremo però farlo nel momento stesso in cui l'utente inserirà nel form
l'informazione richiesta mediante un semplice comando di push del tipo
di quello qui di seguito riportato

dataLayer.push({Paese Preferito\': Italia});

In questo senso diventa dunque di fondamentale importanza sapere
esattamente quando si dispone delle informazioni da passare al Data
Layer, come passarle, dove inserire il Data Layer (se nel head della
pagina web o all'interno del body), e soprattutto diventa ovviamente di
fondamentale importanza sapere esattamente quando tutti i dati necessari
sono effettivamente presenti nel Data Layer in maniera tale da poter
eseguire correttamente i vari Tag ed essere certi che questi, pescando
dal Data Layer, inviino agli strumenti di analisi di terze parti tutte
le informazioni corrette.

Va da se, infine, che per eseguire questo tipo di operazioni e gestire
correttamente il Data Layer è necessario intervenire direttamente nel
codice sorgente della pagina web

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

**SITI PASSWEB**

Nel caso in cui il Data Layer debba essere inserito nel head della
pagina web, e quindi prima del codice relativo al Tag Contenitore, è
possibile utilizzare , in Passweb, la sezione Javascript del Layout
associato alla pagina in cui il Data Layer deve essere inserito.

Si ricorda in questo senso che, in questa sezione, non è necessario
utilizzare i tag di apertura \< script \> e chiusura \< / script \>

Nel caso in cui invece il Data Layer debba essere inserito direttamente
all'interno del body, e quindi dopo il codice relativo al Tag
Contenitore, è possibile utilizzare il componente HTML.

In questo caso è necessario inserire nel componente HTML, l'intero
oggetto javascript compresi i tag di apertura \< script \> e chiusura \<
/ script \>

Il fatto poi di dover inserire il Data Layer prima o dopo il codice
relativo al Tag Contenitore, dipende essenzialmente dal tipo di Tag cui
si vogliono inviare le informazioni e dal momento in cui queste stesse
informazioni sono effettivamente disponibili e possono quindi essere
inserite nel Data Layer

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

**ATTENZIONE! un corretto uso del Data Layer diventa indispensabile per
poter realizzare, mediante GTM, un tracciamento e-commerce, soprattutto
nel caso in cui si voglia implementare con GTM il monitoraggio ecommerce
avanzato (enanched ecommerce) di Universal Analytics o il monitoraggio
Ecommerce di GA4**

In questo senso, nei successivi capitoli di questo manuale
("*Implementare Google Analytics con GTM*"), verranno riportati alcuni
esempi del Data Layer gestito da Passweb utili per poter poi
implementare, sia nel monitoraggio ecommerce avanzato di Universal
Analytics che in quello di GA4, il tracciamento dei diversi eventi
(aggiunta / rimozioni di articoli dal carrello, impressioni, transazioni
...)

Si ricorda inoltre che è comunque possibile analizzare la struttura del
Data Layer gestito da Passweb in piena autonomia utilizzando la funzione
"**Anteprima**" di GTM (richiede l'installazione dell'estensione "**Tag
Assistant Companion**") o un qualsiasi altri strumento che consenta di
debuggare il codice sorgente della pagina.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\GTM_datalayer.bmp](./assets/media/image2.png){width="6.6625in"
height="4.528472222222222in"}

Per maggiori informazioni relativamente all'utilizzo della funzionalità
"Anteprima" di GTM e all'utilizzo dell'estensione "Tag Assistant
Companion" è necessario fare riferimento alla specifica documentazione
di prodotto.

