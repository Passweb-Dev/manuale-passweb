# FONT-SIZE -- CONCLUSIONI



Da quanto detto nei precedenti capitoli di questo manuale dovrebbe ormai
essere chiaro che il principio base da seguire per riuscire a creare una
effettiva tipografia responsive è quello che prevede di **implementare
un font ridimensionabile**.

In questo senso la maggior parte dei webmaster utilizza gli em o i rem
per le dimensioni del testo. **in quanto queste unità di misura
permettono agli utenti di ridimensionare il font nel browser.**

Gli em sono però \"relativi\", dipendono cioè, dall\'elemento padre e
questo vuol dire che è un po\' più complicato rispetto all\'uso dei
pixel, perché si dovrebbero fare dei calcoli per avere una dimensione di
font omogenea, quando nello stesso sito sono presenti diversi elementi
che necessitano diverse dimensioni del font.

I rem offrono una valida alternativa agli em. Si comportano alla stessa
maniera ad eccezione di una differenza fondamentale: i rem sono relativi
all\'elemento html piuttosto che ad ogni loro elemento padre. Questa
differenza sostanziale agevola non di poco il corretto ridimensionamento
del font.

**Nel momento in cui dovessero essere utilizzati i rem quale unità di
misura per i font, è importante applicare una dichiarazione CSS
all\'elemento html, e non al body del documento.**

La regola dovrebbe essere la seguente**:**

html { font-size:100%; }

In questo modo le unità di misura rem verranno applicate alla dimensione
di default del dispositivo.

Oltre a ciò è necessario anche specificare la dimensione del font per
ciascuna dimensione del device e, in questo senso, ci vengono in aiuto
ancora una volta, le media query. Sarebbe opportuno provare diverse
dimensioni di font su dispositivi reali, al fine di ottenere una
perfetta leggibilità (considerando, tra le altre cose, che il tutto
dipende anche dal tipo di font scelto).

Potremmo utilizzare ad esempio delle media queries come quelle qui di
seguito riportate:

\@media (max-width: 640px)

{

body {font-size:1.3rem;}

}

\@media (min-width: 641px)

{

body {font-size:1.2rem;}

}

\@media (min-width:960px)

{

body {font-size:1.4rem;}

}

\@media (min-width:1100px)

{

body {font-size:1.6rem;}

}

Infine se il fatto di supportare le versioni più datate dei browser (es.
IE 10 o versioni precedenti) non dovesse essere un requisito
indispensabile la soluzione delle unità di misura vw e vh rappresenta
una scelta altrettanto valida (se non addirittura migliore) di quella
dei rem.

Nulla vieta comunque di poter utilizzare per elementi diversi diverse
unità di misura.

