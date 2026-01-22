# COMPONENTE HTML



Il Componente consente di inserire all'interno della pagina web snippet
di codice HTML completamente personalizzabili.

![](./assets/media/image169.png)

L'utilizzo di questo componente, assieme alla gestione del layout della
pagina web, con le possibilità di inclusione di file CSS e Javascript,
offre quindi all'utente la possibilità di realizzare il template grafico
del sito senza dover necessariamente ricorrere all'utilizzo dei
componenti grafici messi a disposizione da Passweb.

**Ovviamente l'utilizzo di tali strumenti (componente HTML, Layout, CSS
e Javascript) è consigliato ad utenti con specifiche conoscenze in
merito e, in ogni caso, al fine di non compromettere il normale
funzionamento del sito stesso, il codice HTML inserito all'interno della
pagina attraverso il componente in oggetto dovrà comunque soddisfare
specifici vincoli.**

In questo senso è bene ricordare che nel caso in cui si decida di
inserire all'interno di un componente HTML del codice javascript,
affinchè questo possa poi essere eseguito correttamente è necessario
inserirlo all'interno di un apposito tag \<script\>.

Inoltre nel momento in cui si dovesse decidere di utilizzare anche
jQuery occorre ricordare che l'istruzione per il caricamento della
relativa libreria (inclusa a default nel proprio sito Passweb) è
posizionata (per ottimizzare le prestazioni della pagina) alla fine del
tag \<body\>.

**Per utilizzare correttamente tale libreria è quindi necessario
verificare, per prima cosa, che il DOM della pagina sia stato
correttamente caricato, inserendo quini il codice jQuery all'interno
della seguente istruzione:**

**window.addEventListener(\'DOMContentLoaded\', function() {**

\$(document).ready(function() {

Codice Jquery

});

**});**

**NOTA BENE:** non è possibile gestire, a livello di codice HTML, i
componenti predefiniti messi a disposizione da Passweb (Componenti
E-commerce, Componenti Interazione Utente, Componenti CMS ecc ...)

**NOTA BENE:** lato Wizard i CSS e i javascript possono essere
disabilitati. Codice scritto in maniera non corretta potrebbe infatti,
se eseguito, compromettere il corretto funzionamento del Wizard stesso.
In conseguenza di ciò l'effettivo risultato di eventuali componenti HTML
che implementano questo tipo di codice, potrà essere visualizzato solo
ed esclusivamente lato Front end (ossia visitando la corrispondente
pagina del sito)

