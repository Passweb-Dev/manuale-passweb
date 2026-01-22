# LE MEDIA QUERY



Il concetto principale del web design responsivo è quello di **mantenere
inalterato il codice html della pagina e agire sui fogli di stile per
assegnare regole diverse in base al dispositivo da cui si sta
navigando**.

In questo modo, ad esempio, è possibile nascondere sugli smartphone,
alcuni elementi della pagina web che si è deciso invece di visualizzare
su schermi più larghi quali possono essere quelli di un tablet o di un
pc.

Per ottenere questo risultato dobbiamo ricorrere ad una funzionalità del
CSS 3 chiamata **media query**. In sostanza andremo a porre delle
condizioni in base alle quali un blocco di regole CSS potrà essere o non
essere applicato.

Come recita la definizione che appare nelle specifiche CSS 3 *"una media
query consiste nella dichiarazione di un tipo di media e di zero o più
espressioni che verifichino le condizioni di validità o non validità
delle caratteristiche di un certo media"*. Un semplice esempio chiarisce
ogni dubbio in merito:

\<link rel=\"stylesheet\" media=\"only screen and (color)\"
href=\"colore.css\" /\>

Con l'istruzione sopra evidenziata stiamo indicando di collegare il
foglio di stile, colore.css, alla pagina web solo nel caso in cui questa
pagina venga visualizzata sullo schermo di un pc e solo nel caso in cui
questo sia uno schermo a colori. Cerchiamo di capire meglio come si
arriva a questa conclusione.

Come si accennava nella definizione, una media query prevede
innanzitutto l'uso di un tipo di media il che, in altre parole, equivale
a specificare esattamente per quale dispositivo la regola CSS
interessata dalla media query dovrà essere applicata. In questo senso
possono essere presi in considerazione i seguenti media:

- **all**: il CSS si applica a tutti i dispositivi di visualizzazione;

- **screen**: schermo di computer;

- **print**: pagina stampata;

- **projection**: presentazioni e proiezioni;

- **speech**: dispositivi a sintesi vocale;

- **braille**: supporti basati sull'uso del braille;

- **embossed**: stampanti braille;

- **handheld**: dispositivi mobili con schermo piccolo e in genere
  dotati di browser con limitate capacità grafiche;

- **tty**: dispositivi a carattere fisso come i terminali;

- **tv**: visualizzazione su schermi televisivi.

**ATTENZIONE!** Nel caso in cui in una media query non venga indicato
alcun media si intenderà che le specifiche regole CSS e/o lo specifico
foglio di stile interessato dalla media query stessa sia rivolto a tutti
i tipi di dispositivi (il che, in altri termini, equivale ad utilizzare
come media della query il valore all)

Nell'esempio precedentemente considerato abbiamo usato come media il
valore **screen** indicando, di fatto, che il foglio di stile colore.css
debba essere applicato solo ed esclusivamente nel momento in cui il sito
venga consultato da una specifica categoria di dispositivi: gli schermi
dei computer.

Tornando ora sulla definizione, si ha anche che una media query è
un'espressione logica che può essere vera o falsa a seconda del fatto
che soddisfi o meno le condizioni indicate nella query. Ora, per
costruire query più o meno complesse è possibile ricorre ad operatori
logici come and, not, or ...

Nell' esempio, media="screen **and** (color)", abbiamo inserito la
parola chiave **and**. Il suo significato non è diverso da quello comune
presente in tutti i linguaggi di programmazione ed indica quindi di
eseguire un'unione logica tra le due espressioni.

La prima espressione, screen, indica, come detto, il fatto di applicare
la media query solo nel caso in cui il sito venga visto sullo schermo di
un pc; la seconda espressione, color, rappresenta invece una delle tante
caratteristiche possibili dello schermo di un pc, nello specifico
designa uno schermo a colori.

**ATTENZIONE! da notare come, a livello sintattico, la seconda parte
della media query, quella con le caratteristiche del tipo di media,
debba essere racchiusa tra parentesi tonde**

A questo punto il significato della nostra query è chiaro. Essa sarà
vera (ovvero sarà applicato il foglio di stile colore.css) se la pagina
viene visualizzata su uno schermo di computer a colori.

Una volta compreso il meccanismo si possono costruire query molto
specifiche e complesse, per esempio concatenando tramite and più
espressioni:

media=\"screen and (color) and (device-aspect-ratio: 16/9)\"

Nell'esempio sopra indicato la query è vera se la pagina viene
visualizzata su uno schermo a colori con aspect ratio di 16/9.

**ATTENZIONE! Più media query possono essere raggruppate in una lista
separandole con una virgola:**

media=\"screen and (color), projection and (color)\"

