# MODULO DI RICERCA



Il modulo **Search** di Clerk.io è uno degli strumenti fondamentali per
migliorare l'esperienza utente all'interno del proprio e-commerce.
Basato su tecnologie avanzate di intelligenza artificiale e machine
learning, il modulo "Search" consente di fornire risultati istantanei,
predittivi e personalizzati, capaci di guidare l'utente verso i prodotti
più pertinenti fin dai primi caratteri digitati.

Il sistema di ricerca si basa si basa su un motore semantico
intelligente, che apprende automaticamente in base al comportamento
reale degli utenti (click, acquisti, ricerche precedenti), al loro
intento di ricerca (non solo parole chiave, ma sinonimi, contesto e
tendenze) e, ovviamente, anche in base ai dati dei prodotti a catalogo
condivisi dal sito ecommerce (prezzi, disponibilità, categorie,
attributi personalizzati ....).

Ogni query inserita nella barra di ricerca viene interpretata non solo
in termini letterali, ma anche in base alla probabilità statistica che
rappresenti una certa intenzione di acquisto.

Il risultato è un sistema di ricerca che anticipa l'utente tramite
autocompletamento e suggerimenti in tempo reale, ritorna prodotti
ordinati per rilevanza (non solo per corrispondenza testuale),
personalizza i risultati per ciascun visitatore in base alla sessione e
allo storico.

Questo modulo offre tre soluzioni di ricerca distinte che possono essere
implementate insieme o separatamente. Nello specifico:

- **Search Page**: è una pagina di "Risultati di ricerca" ottimizzata
  per la navigazione potendo disporre anche di filtri che consentono di
  affinare i risultati inizialmente visualizzati

- **Instant Search**: è una sorta di ricerca ad autocompletamento,
  ottimizzata per la velocità, i cui risultati vengono mostrati in
  all'interno di un Dropdown in tempo reale mano a mano che l'utente
  digita la sua query di ricerca. Può essere facilmente collegata ad uno
  dei campi di input presenti in uno dei pannelli di ricerca gestiti sul
  sito. Non consente di inserire ulteriori filtri per raffinare i
  risultati ottenuti

![](./assets/media/image24.png)

- **Omnisearch**: combina il meglio dell' Instant Search e della Search
  Page in un singolo overlay che mostra i risultati mentre il visitatore
  sta digitando la query di ricerca. Contiene prodotti, filtri (facet),
  categorie e pagine, offrendo ai visitatori una panoramica piuttosto
  dettaglia e in un unico punto di tutto il catalogo prodotti e, in
  generale, anche di quelli che possono essere tutti i contenuti
  testuali del sito

![](./assets/media/image25.png)

![](./assets/media/image26.png)

Per maggiori informazioni relativamente alle caratteristiche e alle
funzionalità dei moduli di ricerca messi a disposizione da Clerk si
rimanda a quanto indicato nella relativa documentazione di prodotto (es.
<https://help.clerk.io/it/platform/search/intro/> )

Per quel che riguarda i dati visualizzabili in corrispondenza di ogni
singolo risultato di ricerca sarà possibile, ovviamente, inserire il
nome dell'articolo, l'immagine, il prezzo, la disponibilità ... e in
generale uno qualsiasi dei dati presenti all'interno dei vari feed
(articoli, categorie, pagine) utilizzati per condividere i dati del
proprio sito Ecommerce (per maggiori informazioni relativamente alla
generazione dei vari feed si vedano anche i precedenti capitoli di
questo manuale)

In questo senso va fatta una considerazione di fondamentale importanza
relativa al prezzo degli articoli visualizzato all'interno di questi
moduli di ricerca, **prezzo che** **sarà esattamente lo stesso prezzo di
listino inserito anche nel Feed Articoli** utilizzato per l'integrazione
Passweb -- Clerk.

Ora, se da una parte questo potrebbe essere corretto per un sito B2C in
cui il prezzo dei prodotti non cambia a seconda dell'utente loggato,
dall'altra parte potrebbe anche non andar bene nel caso in cui il prezzo
dei prodotti dovesse invece variare a seconda dell'utente. In queste
condizioni potrebbe quindi essere necessario non inserire nel template
dei risultati di ricerca il prezzo dei prodotti, prezzo questo che dovrà
così essere visualizzato normalmente all'interno della corrispondente
scheda prodotto.

Altra cosa importante da mettere in evidenza **è che i moduli di ricerca
di Clerk non sono implementabili con componenti nativi di Passweb** per
cui, una volta configurata in maniera corretta l'integrazione tra le due
piattaforme, tutto il lavoro di configurazione e personalizzazione
(grafica e di contenuto) del modulo di ricerca dovrà essere eseguita
interamente dal back end di Clerk.

In questo senso sarà necessario, per prima cosa, definire un
"**Design**" ossia l'interfaccia grafica del modulo di ricerca che si
andrà poi ad implementare agendo dalla sezione "**Search -- Design**"
del proprio account Clerk

![](./assets/media/image27.png)

Il pulsante "**New design**" presente nella parte alta della maschera
consente di creare un nuovo Design selezionando anche, tra le tre
precedentemente indicate, la tipologia di modulo di ricerca per cui si
desidera implementare l'interfaccia.

![](./assets/media/image28.png)

![](./assets/media/image29.png)

Selezionato il modulo per cui si desidera operare Clerk metterà poi a
disposizione dei template precostituiti che rappresentano una buona base
di partenza su cui andare a lavorare.

![](./assets/media/image30.png)

Generalmente, per arrivare ad ottenere un risultato in linea con il
proprio sito, i template messi a disposizione da Clerk dovranno comunque
essere personalizzati sia a livello grafico che a livello di contenuti.
In questo senso il modo di lavorare sarà diverso a seconda del fatto di
utilizzare il modulo di Omnisearch piuttosto che l'Instant Search

Nel caso dell' **Omnisearch** infatti l'interfaccia grafica dovrà essere
costruita lavorando interamente a livello di codice sfruttando, per la
parte HTML, il linguaggio di templating (Liquid) messo a disposizione da
Clerk

![](./assets/media/image31.png)

Lato CSS invece sarà possibile inserire il codice necessario per le
personalizzazioni grafiche richieste direttamente all'interno di Clerk
(sezione "CSS") oppure, volendo, questo tipo di personalizzazione potrà
essere effettuata anche lato Passweb utilizzando i vari layout.

Ovviamente il fatto di lavorare a livello di codice se da una parte
richiede specifiche conoscenze tecniche, dall'altra parte offre estrema
libertà di movimento mettendo quindi uno sviluppatore nelle condizioni
di poter arrivare ad effettuare anche personalizzazioni piuttosto
spinte.

Nel caso dell' **Instant** **Search** invece l'interfaccia grafica potrà
essere costruita in maniera visuale utilizzando l'editor messo a
disposizione da Clerk che lavora in maniera piuttosto simile all'editor
di Passweb stesso

![](./assets/media/image32.png)

Si tratterà sostanzialmente di selezionare i vari componenti da
aggiungere all'interfaccia (box, griglie, campi testo, campi HTML ...)

![](./assets/media/image33.png)

e settarne poi le relative proprietà sia a livello grafico che a livello
di contenuto.

![](./assets/media/image34.png)

Il componente "Testo" ad esempio potrà essere mappato (analogamente a
quanto avviene per gli Attributi articolo di Passweb) con uno dei dati
inseriti all'interno del feed articoli utilizzato per l'integrazione tra
le due piattaforme.

Ovviamente il fatto di lavorare a livello visuale, da una parte, rende
possibile effettuare personalizzazioni all'interfaccia senza la
necessità di avere specifiche conoscenze tecniche, dall'altra parte però
offre meno possibilità di personalizzazione rispetto a quello che si
potrebbe ottenere lavorando interamente lato codice, anche se comunque
determinate personalizzazioni (come il fatto di collegare la visibilità
o meno di un elemento al verificarsi di determinate condizioni, o il
fatto di poter utilizzare un componente HTML) possono essere effettuate
anche dall'editor visuale

![](./assets/media/image35.png)

**ATTENZIONE!** per maggiori informazioni relativamente alla creazione
dei Design si consiglia di fare riferimento sempre alla specifica
documentazione di prodotto
(<https://help.clerk.io/it/platform/designs/design-editor/> -
<https://help.clerk.io/it/platform/designs/code-designs/> ) e/o di
rivolgersi direttamente all'assistenza Clerk

Una volta completato il Design e impostata quindi l'interfaccia grafica,
il passo successivo sarà quello di creare e configurare il modulo di
ricerca che dovrà poi essere effettivamente utilizzato all'interno del
sito e questo lo si farà operando all'interno della sezione "**Search --
Elements**"

![](./assets/media/image36.png)

Il pulsante "**New Element**" presente nella parte alta della maschera
consentirà di creare un nuovo elemento, dopo di che sarà necessario
configurarlo impostando quanto richiesto in ciascuna delle sezioni
indicate

![](./assets/media/image37.png)

Nello specifico la sezione:

**Element name**: consente di assegnare un nome e delle label al modulo
che si sta configurando, informazioni queste molto importanti perché
verranno poi utilizzate nei vari cruscotti di analisi dati messe a
disposizione da Clerk per capire l'impatto prodotto dai risultati
mostrati da questo modulo di ricerca sulle vendite registrate

**Elemnt type**: consente di impostare i parametri di configurazione del
modulo di ricerca definendo quindi se si tratta di un Omnisearch
piuttosto che di un Instant Search o di una Search Page, di impostare
una logica che definisca quali prodotti visualizzare prima che l'utente
inizi a digitare la sua query di ricerca, di impostare filtri di
preselezione degli articoli visualizzati ...

![](./assets/media/image38.png)

**Design:** consente di impostare e configurare, selezionandolo tra
quelli precedentemente realizzati, il Design e quindi l'interfaccia
grafica che dovrà essere utilizzata per il modulo di ricerca che si sta
realizzando. Nel caso di Omnisearch sarà anche possibile definire anche
i campi da utilizzare per i filtri di ricerca (sezione Facets)

![](./assets/media/image39.png)

**Insert into website:** consente di impostare la modalità da utilizzare
per visualizzare il modulo di ricerca all'interno del nostro sito. In
questo senso è possibile operare in due modi diversi:

- **Injection:** selezionando questa opzione il modulo di ricerca verrà
  iniettato nella pagina web direttamente da Clerk. In queste condizioni
  sarà quindi indispensabile indicare all'interno della sezione
  "**Display when visitor click**" il selettore CSS dell'elemento
  presente all'interno della pagina del sito Passweb su cui l'utente
  dovrà cliccare per far comparire il modulo di ricerca in esame

![](./assets/media/image40.png)

- **Embedded code:** selezionando questa opzione verrà fornito da Clerk
  lo snippet di codice che dovremo poi inserire (mediante un componente
  HTML) all'interno della/e pagina/e del sito Passweb in cui far
  comparire il modulo di ricerca in questione

![](./assets/media/image41.png)

> **ATTENZIONE!** lo snippet di codice fornito da Clerk dovrà comunque
> essere personalizzato inserendo (attributo "data-trigger-element")
> anche in questo caso il selettore CSS dell'elemento su cui l'utente
> dovrà cliccare per far comparire il modulo di ricerca

Per maggiori informazioni relativamente alla configurazione dello
specifico modulo di ricerca, così come per tutte le ulteriori
possibilità offerte da Clerk in relazione a questa tipologia di moduli
(utilizzo di sinonimi, regole, redirect ...) si consiglia di fare
riferimento alla relativa documentazione di prodotto e/o di chiedere
direttamente all'assistenza Clerk

