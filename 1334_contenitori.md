# CONTENITORI



Come già accennato nei precedenti capitoli di questo manuale, **i
Contenitori sono l'elemento fondamentale su cui si basa tutta la
struttura di GTM**.

**Un Contenitore infatti altro non è se non del codice javascript (più
esattamente l'unico pezzettino di codice javascript)** **che dovrà
essere inserito direttamente in tutte le pagine del nostro sito** è che
sarà poi destinato a contenere tutti gli altri Tag ossia tutti gli altri
pezzettini di codice javascript che dovranno essere utilizzati dal
nostro sito per inviare informazioni e dati a strumenti di terze parti.

Di seguito viene riportato quello che potrebbe essere lo snippet di
codice javascript relativo ad un Contenitore

\< !\-- Google Tag Manager \--\>

\< **noscript**\>\< iframe
src=\"//www.googletagmanager.com/ns.html?id=GTM-7JRL\" height=\"0\"
width=\"0\" style=\"display:none;visibility:hidden\"\>

\<
script\>(function(w,d,s,l,i){w\[l\]=w\[l\]\|\|\[\];w\[l\].push({\'gtm.start\':

new Date().getTime(),event:**\'gtm.js\'**});var
f=d.getElementsByTagName(s)\[0\],

j=d.createElement(s),dl=l!=\'dataLayer\'?\'&l=\'+l:\'\';j.async=true;j.src=

\'//www.googletagmanager.com/gtm.js?id=\'+i+dl;f.parentNode.insertBefore(j,f);

})(window,document,\'script\',\'dataLayer\',**\'GTM-XXXX\'**);

\< !\-- End Google Tag Manager \--\>

**ATTENZIONE! Lo snippet di codice relativo al Contenitore di GTM va
inserito, tipicamente, subito dopo il tag html \< body \> di apertura
della pagina web**

Osservando questo codice possiamo notare, innanzitutto, la presenza del
noscript come "istruzione" di apertura di tutto lo snippet. Questo modo
di operare è di fondamentale importanza in quanto permette poi ai
singoli tag opportunamente configurati con la relativa opzione
**noscript**, di poter essere eseguiti anche nel caso in cui il browser
dovesse essere impostato per non eseguire codice javascript.

Come tutti i tag manager poi, anche GTM utilizza un'apposita libreria
javascript, **gtm.js**, che contiene tutta la logica di cui GTM stesso
ha bisogno per eseguire i singoli tag che verranno caricati all'interno
del Contenitore.

Altra cosa interessante da osservare, infine, è la presenza, nella parte
finale dello snippet, dell'**ID dello specifico Account di Google Tag
Manager** (**GTM-XXX**). E' la presenza di questo ID che consente di
realizzare e gestire il legame tra il Contenitore presente nelle pagine
del nostro sito e il nostro Account GTM.

Una volta compreso, anche dal punto di vista tecnico, che cosa sia un
Contenitore, è bene ricordare ancora una volta come sia perfettamente
possibile generare e gestire all'interno dello stesso Account GTM più
Contenitori differenti.

Tipicamente infatti, **andrebbe creato un Contenitore diverso per ogni
dominio** e quindi per ogni singolo sito che si desidera gestire
mediante lo stesso Account GTM.

Tuttavia, se l\'esperienza utente deve essere valutata sul complesso di
più siti differenti e i tag impostati per un certo sito possono andare
bene anche per domini differenti, potrebbe essere consigliabile
impostare uno stesso Contenitore per tutti i domini interessati. In
questo senso per scegliere quale politica di implementazione adottare
(uno stesso Contenitore su più siti o Contenitori diversi su siti
diversi) è sempre opportuno valutare diverse cose come ad esempio il
fatto che:

- la configurazioni di un certo Contenitore (regole, variabili,
  attivatori ecc...) non può essere condivisa con altri Contenitori, per
  cui se i tag e le logiche di attivazione sono simili in più domini
  differenti, allora potrebbe essere effettivamente consigliabile
  utilizzare un singolo Contenitore in quanto gestire più configurazioni
  simili oltre a richiedere più tempo potrebbe anche causare più
  facilmente degli errori.

- più elevata è la quantità di tag all'interno di un Contenitore, più
  difficile sarà poi la sua gestione. Se il fatto di utilizzare uno
  stesso Contenitore per più siti differenti dovesse quindi portarci ad
  inserire all'interno di quello stesso Contenitore un numero troppo
  elevato di Tag si dovrebbe prendere in considerazione l'ipotesi di
  passare a più Contenitori diversi anche in virtù del fatto che più
  sono gli snippet all'interno di un Contenitore, maggiore sarà la
  dimensione del Contenitore stesso e quindi più lento potrebbe essere
  il caricamento delle pagine che lo ospitano;

- le autorizzazioni utente possono essere impostate solo a livello di
  Contenitore. Nel caso in cui l'esigenza dovesse quindi essere quella
  di impedire agli amministratori di domini diversi di modificare le
  configurazioni appartenenti ad altri, l'unica possibilità sarebbe
  quella di utilizzare un contenitore diverso per ogni dominio.

- la pubblicazione di un Contenitore è effettiva a prescindere dal sito
  in cui quel Contenitore viene poi utilizzato. Nel caso in cui
  l'esigenza dovesse quindi essere quella di applicare le modifiche ad
  un singolo dominio, ancora una volta l'unica soluzione possibile
  sarebbe quella di utilizzare un Contenitore diverso per ogni dominio.

Ogni Contenitore, infine, ha al suo interno due componenti diversi:

- **Tags:** sono i singoli snippet di codice che potranno essere
  inseriti mediante l'interfaccia web di GTM all'interno del nostro sito
  e che, come orami noto, hanno la funzione di inviare dati ed
  informazioni dal nostro sito a strumenti di terze parti.

- **Attivatori:** sono il cervello di GTM. Le Regole o Attivatori,
  comunque li si voglia chiamare, individuano esattamente quale tag
  dovrà essere eseguito e quando. Sono quindi delle condizioni che, al
  momento della loro valutazione, potranno restituire due soli valori,
  "true" o "false"

Per maggiori informazioni relativamente a questi tre elementi si vedano
anche i successivi capitoli di questo manuale.

