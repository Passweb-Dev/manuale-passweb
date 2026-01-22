# CARATTERISTICHE DEI MEDIA



Sulla base di quanto detto fino ad ora in relazione alle media query,
appare abbastanza evidente come per poter sfruttare al meglio tutto il
loro potenziale diventa di fondamentale importanza conoscere le
caratteristiche dei media su cui si può intervenire per indirizzare le
regole CSS.

In questo senso si potrebbe decidere di applicare determinate regole CSS
in base, ad esempio, alle seguenti proprietà:

- **Larghezza dell'area di visualizzazione del documento -- width
  (min-width, max-width)**

> Come precedentemente indicato **l'area di visualizzazione del
> documento è rappresentata, su di un normale browser web, dal viewport
> e non ha assolutamente nulla a che fare con le dimensioni dello
> schermo del dispositivo**.
>
> Per poter applicare delle regole CSS in base a questo elemento è
> possibile utilizzare la proprietà **width** esprimendone i valori in
> una qualsiasi unità di misura (px, em, %)
>
> [Esempio]{.underline}

\@media screen and (width: 400px) {

/\* regole CSS \*/

}

> Nell'esempio sopra riportato le regole CSS verranno applicate solo ed
> esclusivamente nel momento in cui l'area di visualizzazione del
> documento (e quindi il viewport impostato) sia uguale esattamente a
> 400px
>
> **ATTENZIONE! Nella realizzazione di siti responsivi si tende ad
> indirizzare le varie regole CSS non tanto in base all'esatta larghezza
> del viewport quanto più genericamente in base a quella che possa
> essere la larghezza minima e/o massima dell'area di visualizzazione
> del documento**.
>
> In questo senso andranno quindi utilizzate le proprietà **min-width**
> e **max-width**
>
> [Esempio]{.underline}

\@media screen and (min-width: 400px) and (max-width: 1024px) {

/\* regole CSS \*/

}

> Nell'esempio sopra riportato le varie regole CSS verranno applicate
> quando l'area di visualizzazione del documento ha una larghezza
> compresa tra i 400 e i 1200 pixel

- **Altezza dell'area di visualizzazione del documento -- height
  (min-height**, **max-height)**

> Per poter applicare delle regole CSS in base a questo elemento è
> possibile utilizzare la proprietà **height** esprimendone i valori in
> una qualsiasi unità di misura (px, em, %).
>
> Come nel caso della larghezza anche questa volta è inoltre possibile
> ragionare in termini di altezza minima e massima utilizzando le
> proprietà **min-height** e **max-height**

- **Larghezza dell'intera area di rendering del dispositivo -
  device-width (min-device-width,** **max-device-width)**

> A differenza dell'area di visualizzazione del documento (il viewport)
> con il termine area di rendering del dispositivo si intende fare
> riferimento esattamente **alla larghezza dello schermo del dispositivo
> di visualizzazione**
>
> Per poter applicare delle regole CSS in base a questo elemento è
> quindi necessario utilizzare la proprietà **device-width**
>
> [Esempio]{.underline}

\@media screen and (device-width: 400px) {

/\* regole CSS \*/

}

> Nell'esempio sopra riportato le regole CSS verranno applicate solo ed
> esclusivamente nel momento in cui lo schermo del dispositivo di
> visualizzazione sia largo esattamente 400 pixel
>
> Anche in questo caso risulta molto più utile indirizzare le vari
> regole CSS non tanto in base all'esatta larghezza del dispositivo
> quanto più esattamente sulla base di quella che possa essere la sua
> larghezza minima o massima.
>
> In questo senso andranno quindi utilizzate le due proprietà
> **min-device-width** e **max-device-width**

- **Orientamento del dispositivo - orientation**

> Nella realizzazione di un sito responsivo può diventare molto
> importante adattare i contenuti della pagina anche in base a come
> l'utente ruota il dispositivo.
>
> In questo senso la proprietà **orientation** consente di indirizzare
> l'applicazione di determinate regole CSS in base al fatto che il
> dispositivo di visualizzazione sia posto in modalità **landscape**
> (orizzontale -- la larghezza è maggiore dell'altezza) oppure
> **portrait** (verticale -- l'altezza è maggiore della larghezza).
>
> [Esempio]{.underline}

\@media all and (min-device-width: 481px) and (max-device-width: 1024px)
and **(orientation:portrait)**{

/\* regole CSS \*/

}

> Nell'esempio sopra indicato le regole CSS verranno applicate solo ed
> esclusivamente sui dispositivi il cui schermo ha una larghezza
> compresa tra i 481 e i 1024 pixel e solo ed esclusivamente nel momento
> in cui questi dispostivi siano stati posti in modalità portrait (ossia
> in verticale)

- **Rapporto tra larghezza e altezza dell'area di visualizzazione del
  documento -- aspect-ratio**

> La proprietà **aspect-ratio** identifica il rapporto tra la larghezza
> e l'altezza dell'area di visualizzazione del documento (che ricordiamo
> ancora una volta essere identificata dal viewport).
>
> I valori di questa proprietà di esprimono attraverso due numeri interi
> separati dal simbolo /
>
> [Esempio]{.underline}

\@media screen and (device-aspect-ratio: 16/9){

/\* regole CSS \*/

}

> Nell'esempio sopra indicato le regole CSS verranno applicate solo ed
> esclusivamente su quei dispositivi in cui il rapporto tra la larghezza
> e l'altezza del viewport è di 16/9

- **Rapporto tra larghezza e altezza dell'area di rendering del
  dispositivo -- devie-aspect-ratio**

> La proprietà **device-aspect-ratio** identifica il rapporto tra la
> larghezza e l'altezza dell'area di rendering del dispositivo (che
> ricordiamo ancora una volta essere identificata dalla larghezza dello
> schermo).
>
> Anche in questo caso i valori di questa proprietà di esprimono
> attraverso due numeri interi separati dal simbolo /

- **Risoluzione del dispositivo di output - resolution**

> La proprietà **resolution** definisce la risoluzione (ovvero la
> densità di pixel) del dispositivo di output. I valori della
> risoluzione possono essere espressi in dpi (punti per pollice) oppure
> in dpcm (punti per centimetro).
>
> La proprietà può assumere anche i prefissi min e max per individuare
> rispettivamente la risoluzione minima e massima del dispositivo.
>
> [Esempio]{.underline}

\@media screen and (min-resolution: 300dpi){

/\* regole CSS \*/

}

> Nell'esempio sopra indicato le regole CSS verranno applicate solo ed
> esclusivamente su quei dispositivi con una risoluzione di output
> maggiore di 300 dpi

