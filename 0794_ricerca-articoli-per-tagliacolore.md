# RICERCA ARTICOLI PER TAGLIA/COLORE



Nel momento in cui l'esigenza dovesse essere quella di attivare
all'interno del proprio sito Ecommerce una ricerca articoli basata sui
valori di una determinata serie di Taglie/Colori (definita mediante
l'apposita tabella gestionale) sarà necessario inserire all'interno del
relativo pannello di ricerca un componente "**Filtro Indice**",
"**Filtro Checkbox**" o "**Filtro Lista**" mappato sul Campo Articolo
"**Taglie**" o "**Taglie Disponibili**"

![](./assets/media/image346.png)

In queste condizioni infatti nella maschera di configurazione del
componente verrà visualizzato anche il campo **Serie Taglie**

![](./assets/media/image347.png)

mediante il quale poter indicare, selezionandola dal relativo menu a
tendina, la specifica serie di Taglie/Colori in relazione a cui dovranno
poi essere mostrate le varie opzioni di ricerca.

In particolare:

- nel momento in cui per il campo "**Serie Taglie**" dovesse essere
  indicata una specifica serie di Taglie/Colori, le opzioni di ricerca
  visualizzate sul front end del sito saranno relative unicamente a
  quella stessa serie.

![Videate\\ricerca_articolo_taglie_colori.bmp](./assets/media/image328.png)

> In queste condizioni inoltre se non dovesse essere indicata una
> specifica Label, come intestazione del campo di ricerca verrà
> utilizzata automaticamente la descrizione associata all'interno del
> gestionale alla serie di Taglie/Colori in questione

- nel momento in cui per il campo **"Serie Taglie**" non dovesse invece
  essere indicata nessuna serie in particolare, lasciando quindi il
  campo stesso non valorizzato, allora le opzioni di ricerca
  visualizzate sul front end del sito dipenderanno esattamente dalla
  specifica pagina in cui è stato inserito il componente di ricerca.

> In questo senso se il componente di ricerca dovesse essere inserito
> nella pagina "Negozio" (e quindi nel catalogo generale) le opzioni di
> ricerca visualizzate sul front end del sito saranno relative a tutte
> le serie di Taglie/Colori attualmente gestite.

![Videate\\filtri_articolo_taglie_colori2.bmp](./assets/media/image348.png)

> Se il componente di ricerca dovesse invece essere inserito in una
> determinata pagina di categoria le opzioni di ricerca visualizzate sul
> front end del sito saranno relative unicamente alle serie di
> Taglie/Colori associate agli articoli di quella stessa categoria.
>
> Come evidenziato nella figura sopra riportata, in queste condizioni
> verrà creata una "sezione di ricerca" per ciascuna delle serie di
> Taglie/Colori effettivamente coinvolte e come intestazione di questa
> sezione verrà utilizzata automaticamente la descrizione associata,
> all'interno del gestionale, alla serie stessa (non verrà quindi preso
> in considerazione quanto eventualmente inserito in fase di
> configurazione del componente all'interno del campo "Label"). Ad ogni
> singola "sezione di ricerca" verrà inoltre associata anche una
> specifica classe css (**optiongroup\_\<id serie\>**) utilizzabile nel
> momento in cui l'esigenza dovesse essere quella di stilizzare in
> maniera diversa le singole sezioni.

Infine, in relazione alla possibilità di implementare all'interno del
proprio sito una ricerca per Taglia/Colore è sempre bene tenere in
considerazione alcune osservazioni di fondamentale importanza.

Nello specifico:

- **La ricerca per Taglia/Colore funziona unicamente in relazione ai
  valori delle serie definite all'interno della corrispondente Tabella
  Mexal.** Nel momento in cui la taglia/colore dovesse essere gestita
  come elemento di una struttura sarà quindi necessario implementare una
  ricerca per "Campi Struttura" (per maggiori informazioni in merito si
  veda quanto indicato all'interno del capitolo "*Ricerca Articoli su
  Campi Struttura*" di questo manuale)

- Per i **padri di struttura** con articoli figlio gestiti a
  Taglie/Colori, verranno considerati sempre tutti gli elementi della
  serie di Taglie/Colori cui appartiene l'articolo stesso (non verranno
  quindi valutate le reali disponibilità di tutti i possibili articoli
  figlio)

- I valori mostrati sul front end del sito come possibili opzioni della
  ricerca per Taglia/Colore sono esattamente quelli definiti, in
  relazione alla serie considerata, all'interno della maschera
  "**Modifica Elementi della serie**"

![](./assets/media/image325.png)

> Per maggiori informazioni in merito a come poter personalizzare questi
> elementi si veda anche quanto indicato all'interno del relativo
> capitolo di questo manuale ("*Catalogo -- Gestione Articoli --
> Articoli -- Taglie o Colori (Ecommerce Mexal) -- Personalizzazione
> degli elementi di una serie di taglie/colori*")
>
> **ATTENZIONE!** Il colore eventualmente associato agli elementi di una
> serie verrà effettivamente visualizzato sul front end del sito come
> possibile opzione di ricerca assieme alla descrizione testuale dello
> stesso elemento solo per Varianti Responsive e solo per controlli di
> tipo Filtro Indice, Filtro Lista o Filtro Checkbox

- Dipendentemente dalla impostazioni settate per il filtro di ricerca,
  le opzioni visualizzate poi sul front end del sito potrebbero anche
  essere particolarmente numerose (soprattutto nel momento in cui
  dovessero essere gestite tante diverse serie di Taglie/Colori).

> Per evitare quindi di andare a gravare in maniera eccessiva su quelle
> che possono essere le prestazioni del sito, o su quella che sarà poi
> l'effettiva usabilità dei filtri di ricerca, **si consiglia sempre di
> gestire la ricerca per Taglia/Colore solo nelle pagine di categoria in
> cui sono effettivamente presenti prodotti gestiti in questo modo
> (evitando quindi di impostare questo tipo di filtri a livello generale
> sull'intero catalogo)**.

- Nel momento in cui il filtro di ricerca dovesse essere configurato
  impostando il parametro "Campo su cui far Filtro" sul valore
  "**Taglie**" le opzioni di ricerca visualizzate sul front end del sito
  **faranno riferimento a tutti gli elementi delle serie di
  Taglie/Colori coinvolte**

> Se l'esigenza dovesse invece essere quella di mostrare come opzione di
> ricerca solamente i valori delle serie corrispondenti alle
> Taglie/Colori effettivamente disponibili per gli articoli in catalogo,
> sarà allora necessario configurare il filtro di ricerca impostando il
> parametro "Campo su cui far Filtro" sul valore "**Taglie
> Disponibili**"

- Nel momento in cui il filtro di ricerca dovesse essere configurato
  impostando il parametro "**Campo su cui far Filtro**" sul valore
  "**Taglie Disponibili**" e un determinato articolo dovesse essere
  gestito in modalità "**Acquista Sempre**", nel filtro di ricerca
  verranno visualizzate sempre e comunque tutte le taglie/colori della
  relativa serie (non solo quelle effettivamente disponibili)

- Per evitare un disallineamento dei dati, il mapping di un filtro di
  ricerca su tutte le Taglie/Colori di una determinata serie o solamente
  su quelle effettivamente disponibili, dovrebbe andare ovviamente di
  pari passo con la modalità di gestione adottata per l'acquisto degli
  articoli associati a quella stessa serie di Taglie/Colori.

> Nel momento in cui si dovesse decidere, ad esempio, di gestire gli
> articoli in "**Acquista sempre**" è chiaro che tutte le taglie
> risulterebbero essere sempre acquistabili e, pertanto, sempre
> disponibili. In queste condizioni nel filtro di ricerca verrebbero
> chiaramente visualizzati sempre tutti gli elementi della serie.
>
> Se invece gli articoli dovessero essere gestiti in "**Acquista solo se
> disponibile**" e il filtro di ricerca dovesse invece essere impostato
> per visualizzare comunque tutte le Taglie/Colori della serie, è chiaro
> che potrebbero anche verificarsi situazioni in cui determinate
> ricerche porteranno a non ottenere alcun risultato

