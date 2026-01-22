# VW (VIEWPORT WIDTH) E VH (VIEWPORT HEIGHT)



VW (Viewport Width) e VH (Viewport Height) sono due nuove unità di
misura introdotte dalle specifiche CSS 3 che possono rivelarsi
particolarmente utili e preziose nei design responsive perché forniscono
un rapporto diretto con le dimensioni della Viewport (dove con viewport
si intende identificare la dimensione della finestra del browser),
evitando quindi, in molti casi, di dover scrivere apposite media query.

Quando viene modificata l'altezza o la larghezza della finestra del
browser (ossia della viewport) la dimensione degli elementi gestita
mediante queste unità di misura varierà di conseguenza in maniera
completamente automatica.

Nello specifico l'unità di misura

- **VW (Viewport Width):** gestisce il dimensionamento di un elemento in
  relazione alla larghezza della finestra del browser. L'unità vw è pari
  all'1% della larghezza della viewport.

> In queste condizioni, dunque, per rendere un elemento ampio sempre
> quanto l'intera larghezza della finestra del browser sarà necessario
> impostare la sua width sul valore 100vw.
>
> Allo stesso modo, la larghezza della viewport fosse ad esempio di
> 1920px, impostando la dimensione del font di un elemento sul valore
> 1vw il suo font-size sarebbe esattamente di 19.2 px. Restringendo le
> dimensioni della finestra a 1024px il font size di quello stesso
> elemento passerà in maniera automatica al valore 10.24px.

- **VH (Viewport Height):** gestisce il dimensionamento di un elemento
  in relazione all'altezza della finestra del browser. L'unità vh è pari
  all'1% dell'altezza della viewport.

> In queste condizioni, dunque, per rendere un elemento alto sempre come
> l'intera finestra del browser sarà necessario impostare la sua height
> sul valore 100vh.

In sostanza dunque il grande vantaggio che si può avere nell'utilizzare
queste unità di misura è rappresentato dal fatto che esse creano un
rapporto diretto con le dimensioni della finestra del browser e, di
fatto, con le diverse risoluzioni dei dispositivi di visualizzazione,
permettendoci, ad esempio di scalare le dimensione del testo per ogni
formato di schermo senza il bisogno di utilizzare apposite media query.

Inoltre essendo delle unità di misura possono essere utilizzate, secondo
lo stesso principio, non solo per il font del testo ma anche su di una
qualsiasi altra proprietà CSS che accetti come valore una lunghezza.

Il lato negativo della medaglia è rappresentato dalla compatibilità con
i diversi browser, che comunque ha raggiunto al giorno d'oggi, valori
più che accettabili come è possibile verificare al seguente indirizzo:

<https://caniuse.com/#search=vw>

In ogni caso è sempre possibile fornire un ripiego ai browser che non
supportano queste unità di misura scrivendo regole CSS che i browser più
vecchi possano comprendere, e che vengano invece sovrascritte per i
browser più moderni dall'analoga regola che utilizza però i valori di vw
e vh come nell'esempio di seguito riportato

h1 {\
font-size: 36px; font-size: 5.4vw;\
margin-top: 21px; margin-top: 7vw;\
}

