# DEFINIRE I BREAKPOINT



Come abbiamo visto nel capitolo precedente di questa guida grazie alle
media query è possibile indicare al browser di applicare o meno
determinate regole CSS al verificarsi di determinate condizioni.

I punti in cui si verificano queste condizioni sono esattamente ciò che
viene definito **breakpoint**.

**In altri termini dunque un breakpoint è un punto, su di una linea
ideale che parte da 0, in cui si verifica una qualche modifica (tramite
CSS) al layout di una pagina web.**

Consideriamo un esempio per meglio comprendere questa definizione.

Supponiamo di dover progettare una pagina web il cui colore di sfondo
dovrà variare in base alla larghezza dell'area di visualizzazione del
documento (viewport) secondo le seguenti specifiche:

- Colore di sfondo predefinito ROSSO

- Viewport raggiunge i 480 px -- Colore di sfondo GIALLO

- Viewport raggiunge i 768 px -- Colore di sfondo VERDE

- Viewport raggiunge i 1024 px -- Colore di sfondo BLU

- Viewport super i 1200 px -- Colore di sfondo GRIGIO

Per tradurre in codice queste specifiche dovremo, ovviamente, ricorre a
delle media query utilizzando, per indirizzare l'applicazione delle
regole CSS, la proprietà **width,** e impostando i nostri breakpoint
rispettivamente a **480 px, 768 px, 1024 px e 1200 px** come qui di
seguito indicato:

body {

background: red;

}

\@media screen and (**min-width: 480px**) {

body {

background: yellow;

}

}

\@media screen and (**min-width: 768px**) {

body {

background: green;

}

}

\@media screen and (**min-width: 1024px**) {

body {

background: blue;

}

}

\@media screen and (**min-width: 1200px**) {

body {

background: gray;

}

}

Una volta compreso il meccanismo che sta alla base delle media query
viene naturale porsi una domanda:

**Nella realizzazione di un sito responsivo, quanti breakpoint è
opportuno/necessario gestire?**

In linea generale la risposta a questa domanda dipende da vari fattori
quali le caratteristiche del sito, il suo layout, le dimensioni degli
schermi dei dispositivi su cui il sito dovrà essere visualizzato, le
tecniche di implementazione adottate ecc ... il che in sostanza equivale
a dire "quanti ne servono affinchè la pagina si adatti al meglio alle
caratteristiche dei dispositivi su cui dovrà essere visualizzata".

Fatta questa considerazione, va anche detto però che **la pratica ad
oggi prevalente è quella che prevede di fissare i breakpoint in funzione
alle dimensioni, in particolare alla larghezza, del viewport** per poi
inserire qualche media query più specifica solo nel caso in cui ci si
dovesse accorgere di qualche problema su determinati modelli di
dispositivi.

In questo senso è anche abbastanza evidente, considerando l'ampia gamma
di dispositivi disponibili sul mercato, come non possa essere possibile
scrivere delle media query specifiche per ogni dispositivo, considerando
esattamente quelle che sono le dimensioni del suo viewport. La tendenza
è quindi quella di ragionare per tipologia di dispositivo prendendo in
considerazione, per il layout del proprio sito, tre diverse versioni:

- un layout per gli **smartphone**

- un layout per i **tablet**

- un layout per i **pc desktop**

In considerazione di ciò, sia che si decida di adottare l'approccio
mobile first, sia che si decida di lavorare in maniera "tradizionale",
avremo sempre bisogno di almeno due media query generali.

Supponendo infatti di adottare l'approccio mobile first, il layout per
smartphone non avrà bisogno di specifiche media query (essendo il
default); saranno invece necessarie due media query: una per indirizzare
la visualizzazione del sito sui tablet ed una per indirizzare la
visualizzazione del sito sugli schermi pc.

Allo stesso modo, nel caso in cui si voglia utilizzare l'approccio
tradizionale considerando come standard il layout per desktop, avremo
comunque bisogno di almeno due media query necessarie questa volta per
indirizzare la visualizzazione del sito su tablet e smartphone. Alcuni
esempio di queste media query possono essere trovate al seguente
indirizzo:

<https://css-tricks.com/snippets/css/media-queries-for-standard-devices/>

**ATTENZIONE!** I valori utilizzati in queste media query sono più o
meno standard e nella maggior parte dei casi hanno come riferimento i
device Apple. Questo non vuol dire però realizzare dei siti ottimizzati
solo per iPhone o iPad a discapito di altri device; i valori indicati
infatti servono più che altro come punto di riferimento per una
specifica tipologia di dispositivo

Ognuna delle media query indicate potrebbe poi essere sdoppiata in base
all'orientamento del dispositivo (portrait o landscape)

