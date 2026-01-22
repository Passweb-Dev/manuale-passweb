# ATTIVATORI



Le Regole o Attivatori, comunque li si voglia chiamare, sono il cervello
di GTM, sono loro che dicono quale Tag dovrà essere caricato all'interno
del Contenitore e quando dovrà essere eseguito, se al caricamento di una
pagina, a seguito di una interazione utente ecc...

Il tag di Google Analytics, ad esempio, andrebbe caricato su tutte le
pagine del sito, per cui potrebbe essere associato all' Attivatore
"Tutte le pagine".

Al contrario il Tag relativo al tracciamento delle conversioni AdWords
dovrebbe essere eseguito solo ed esclusivamente nelle relative thankyou
page. In questo caso dovremmo quindi creare in GTM un Attivatore
mediante il quale specificare che il Tag utilizzato per la conversione
AdWords venga inserito nel Contenitore ed eseguito solo se l'URL della
pagina sia esattamente quello della nostra thankyou page.

In ogni caso appare abbastanza evidente come **ogni Tag debba
necessariamente avere associato un determinato Attivatore** per poter
essere eseguito. Senza un suo Attivatore un Tag non ha senso di
esistere, ne tanto meno di essere inserito in una pagina del nostro sito
in quanto, di fatto, non potrà mai essere eseguito.

Gli Attivatori vengono valutati al verificarsi di determinati eventi e i
Tag ad essi associati verranno attivati (o non attivati) quando tutte le
condizioni dell'Attivatore stesso saranno soddisfatte (o non
soddisfatte).

Un Tag con un Attivatore basato, ad esempio, su un evento
"Visualizzazione di pagina" e con il seguente filtro

*url è uguale a www.nomesito.it*

sarà attivato solo ed esclusivamente quando l'utente visualizzerà la
home page di nomesito

**ATTENZIONE!** **Tutti i tag che si attivano in Google Tag Manager sono
attivati da eventi. Ogni volta che un evento è registrato da Google Tag
Manager, gli attivatori del contenitore vengono valutati e i tag vengono
attivati di conseguenza. Nessun tag può essere attivato se non si
verifica un evento**.

Un evento può essere una visualizzazione di pagina, un clic su un
pulsante, l\'invio di un modulo ecc...

Per maggiori informazioni relativamente alle diverse tipologie di eventi
gestibili in GTM si consiglia di fare riferimento alla specifica
documentazione di GTM.

In generale dunque ogni Attivatore sarà composto da un **Evento**, che
definisce quando valutarlo, e da uno o più **Filtri** che definiscono le
condizioni da soddisfare per poter effettivamente eseguire il Tag ad
esso associato

Ogni Filtro, a sua volta sarà quindi composto da tre distinti elementi,
una **Variabile**, un **Operatore** e un **Valore**:

- **Variabile**: è l'elemento utilizzato in GTM per memorizzare i dati
  generati a runtime. Il contenuto di queste Variabili dovrà poi essere
  confrontato con un determinato Valore per definire se la condizione
  indicata dal Filtro associato all'Attivatore è o meno soddisfatta.

> Nell'esempio di Filtro sopra indicato la Variabile è **URL** ed è
> utilizzata per memorizzare l' url della pagina visitata dall'utente

- **Operatore**: è l'operatore logico utilizzato nella definizione del
  Filtro associato all'Attivatore.

> Nell'esempio di Filtro sopra indicato l'Operatore è "**uguale a**"

- **Valore**: è quella specifica informazione, inserita in fase di
  configurazione del Filtro e in rapporto alla quale vengono valutati i
  dati memorizzati nella Variabile utilizzata dal Filtro stesso.

> Nell'esempio di Filtro sopra il Valore è "**www.nomesito.it**"

Ovviamente nel caso in cui ad uno stesso Attivatore siano associati più
Filtri affinchè il relativo Tag possa effettivamente essere eseguito
dovranno essere soddisfatte tutte le condizioni indicate nei vari
Filtri.

**ATTENZIONE! Gli Attivatori in GTM sono definiti a livello di
Contenitore e questo significa che uno stesso Attivatore può
tranquillamente essere riutilizzato anche su Tag diversi**

