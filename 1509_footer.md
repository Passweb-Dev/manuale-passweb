# FOOTER



L'elemento \< footer \> **identifica il "piede" per il più vicino
elemento che ne definisce l'ambito.** In altri termini è semplicemente
il "piè di pagina" per la specifica sezione della pagina web cui fa
riferimento.

**Ogni sezione della pagina dovrebbe quindi avere un header che
racchiuda la sua intestazione ed un footer che racchiuda invece le sue
specifiche informazioni " di piede".**

Le informazioni racchiuse da questo tag sono, tipicamente, informazioni
relative all'autore dei contenuti della sezione cui il footer fa
riferimento, al copyright, ai termini di licenza ecc...

![](./assets/media/image9.png)

Ovviamente, sulla base di quanto detto, è semplice comprendere come
anche in questo caso possano esistere più elementi footer all'interno di
una stessa pagina web e come sia quindi sbagliato identificare questo
tag solo ed esclusivamente con il piede dell'intera pagina.

Un'interessante notazione presente nelle specifiche di questo tag indica
come questo elemento possa anche essere utilizzato per racchiudere molto
materiale: menu di navigazione, testi, immagini ecc.... E' infatti
prassi comune nel design attuale dei siti web avvalersi dei cosiddetti
"fat footers" ossia sezioni footer molto consistenti in termini di
spazio visivo occupato e quantità di contenuti ospitati.

Per poter implementare in Passweb questo tag semantico è necessario
utilizzare un Componente Contenitore configurato come nella figura di
seguito riportata:

![](./assets/media/image10.png)

I contenuti del footer della sezione andranno quindi inseriti, mediante
gli appositi componenti Passweb, all'interno di questo contenitore.

