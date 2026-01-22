# VARIABILI



Come già evidenziato all'interno del precedente capitolo di questo
manuale, le Variabili sono l'elemento utilizzato da GTM per memorizzare
delle informazioni.

Una Variabile è quindi una coppia nome -- valore in cui il valore viene
determinato a runtime. La Variabile predefinita "URL", ad esempio, è
stata definita in modo tale che il suo valore coincida con l' url della
pagina corrente.

In GTM le variabili vengono utilizzate:

- **negli Attivatori**: per definire i filtri che specificano quando un
  determinato Attivatore deve essere eseguito

- **nei Tag**: per acquisire valori in maniera dinamica (ad es.
  trasferimento del valore della transazione e dei prodotti acquistati
  al tag di monitoraggio delle conversioni).

Sotto questo aspetto poi GTM fornisce un insieme di variabili
predefinite da poter utilizzare per creare in maniera rapida i Tag e gli
Attivatori più comunemente utilizzati.

Oltre a queste Variabili predefinite è comunque possibile creare anche
delle Variabili personalizzate in base a quelle che sono le proprie
specifiche esigenze

Supponiamo, ad esempio di voler attivare un Tag di remarketing sulla
Rete Display di Google ogni volta che un visitatore spende più di € 100.
Per implementarlo dovremmo creare un Attivatore che viene valutato al
verificarsi dell'evento "visualizzazione di pagina" (dove la pagina che
dovrà essere visualizzata sarà ovviamente quella di conferma
dell'ordine) e aggiungere sull' Attivatore stesso un Filtro del tipo

**Importo transazione maggiore di € 100**

Poiché la variabile "Importo transazione" non esiste, dovremmo definirla
come Variabile personalizzata.

Dovremo quindi indicare a GTM di cercare il valore di "Importo
transazione" in una variabile JavaScript accertandoci che la variabile
indicata sia effettivamente presente sulla pagina di conferma
dell\'acquisto.

In fase di esecuzione, Google Tag Manager otterrà il valore di "Importo
transazione" dalla variabile JavaScript specificata. Successivamente,
l\'attivatore sopra indicato valuterà se il valore è o meno maggiore di
€ 100.

Oltre a utilizzare "Importo transazione" in un Attivatore, potremmo poi
utilizzarlo anche per trasmettere l\'importo della transazione a
qualsiasi tag di monitoraggio delle conversioni, ad esempio un tag
DoubleClick o Google Analytics, consentendo così ai rapporti generati
dai relativi strumenti di analisi di mostrare anche il valore delle
entrate delle transazioni.

Per maggiori informazioni sui diversi tipi di Variabili utilizzabili in
GTM si consiglia di fare riferimento alla specifica documentazione di
GTM.

