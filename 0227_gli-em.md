# GLI EM



**Un em è l'equivalente della dimensione (in pixel) definita nella
regola CSS font-size.**

Se ad esempio impostiamo per un \< div \> un testo con font-size 16
pixel, 1 em sarà uguale a 16 pixel, 2 em corrisponderanno a 32 pixel e
così via.

Gli em sono ridimensionabili in tutti i browser, rispondendo quindi
correttamente alle relative funzioni di zoom, e non è necessario
impostare il valore per ogni singolo elemento in quanto anche in questo
caso la regola può essere applicata "a cascata" dall'elemento "genitore"
all'elemento "figlio".

Ovviamente, anche per questa scelta ci sono dei pro e dei contro da
tenere in considerazione.

Da una parte bisogna infatti considerare che l'utilizzo di questa unità
di misura, oltre a garantire una corretta risposta alle funzioni di zoom
del browser, facilita notevolmente la manutenzione del sito. E' infatti
sufficiente apportare delle modifiche alla dimensione fissa in pixel cui
fanno riferimento tutti i vari elementi impostati in em, per far si che
questi si aggiornino poi di conseguenza.

Supponiamo ad esempio di aver impostato le seguenti regole CSS

body {

font-size: 16px;

}

p {

font-size: 1em;

}

h1 {

font-size: 1.5em;

}

In queste condizioni il testo presente all'interno dei paragrafi (tag p)
avrà dimensione pari a 16 x 1 = 16 px, mentre la dimensione dei titoli
h1 sarà di 16 x 1.5 = 24 px.

Supponendo ora di voler aumentare la dimensione del testo portando i
paragrafi a 17 px e gli h1 a 25.5 px non sarà necessario variare
singolarmente le due regole relative ai tag p e h1 ma sarà sufficiente
portare a 17 pixel il font-size del body per fare in modo che le due
dimensioni in em si aggiornino di conseguenza.

Va anche sottolineato però come il fatto che i cambiamenti impostati al
font-size di riferimento vengano applicati in automatico a tutti i
contenuti impostati in em, può rappresentare anche una difficoltà, in
conseguenza del fatto che nella realizzazione di una pagina web
occorrerà sempre trovare una buona proporzione tra i testi con
dimensioni differenti.

Inoltre bisogna anche considerare che il font-size in em di un certo
testo fa sempre riferimento al font-size dell'elemento "genitore" per
cui nel caso di elementi annidati potrebbe diventare complicato sapere
esattamente a quanti pixel corrisponde una dimensione impostata in em.
Cerchiamo di comprendere meglio questa affermazione con un semplice
esempio.

Consideriamo il seguente markup HTML

\<div class=\"contenitore_1\"\>

\<div class=\"paragrafo_1 \"\>

Testo Paragrafo 1

\</div\>

\<div class=\"contenitore_2\"\>

\<div class=\"paragrafo_2 \"\>

Testo Paragrafo 2

\</div\>

\</div\>

\</div\>

e le seguenti regole CSS

.contenitore_1 {

font-size: 15px;

}

.paragrafo_1 {

font-size: 1 em;

}

.contenitore_2 {

font-size: 1.5 em;

}

.paragrafo_2 {

font-size: 1 em;

}

Nell'esempio sopra indicato pur avendo considerato sia per il
paragrafo_1 che per il paragrafo_2, una dimensione di 1 em, questa
corrisponderà nel primo caso (paragrafo_1) a 15 px mentre nel secondo
caso (paragrafo_2) a 22.5 px.

Il paragrafo_2 infatti ha come elemento "genitore" il contenitore_2 per
il quale è stato considerato un font-size di 1.5 em, e che ha a sua
volta come elemento "genitore" il contenitore_1.

Per poter determinare a quanti pixel corrisponde il font-size del
paragrafo_2 occorre quindi per prima cosa determinare i pixel del
font-size del contenitore_2. Avremo quindi

font-size contentiore_2 🡪 1.5 x 15 = 22.5 px

fon-size paragrafo_2 🡪 1 x 22.5 = 22.5px

Considerando che il markup di una pagina HTML è generalmente costituito
da svariati elementi anche piuttosto annidati tra loro è semplice
comprendere come ci si possa facilmente perdere nel cercare di capire a
quanti pixel corrisponda esattamente una dimensione in em.

