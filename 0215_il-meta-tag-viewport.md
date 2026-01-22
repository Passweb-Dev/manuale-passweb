# IL META TAG VIEWPORT



Un altro prerequisito fondamentale per realizzare un sito responsivo è
quello di utilizzare correttamente il **viewport** per indicare in
maniera specifica al browser quale debba essere la larghezza della
superficie su cui disegnare la pagina web.

Tecnicamente questo è un meta tag da inserire nella sezione \< head \>
della pagina e che dovrà avere una struttura analoga a quella qui di
seguito riportata.

\<meta name=\"viewport\" content=\"width=device-width,
initial-scale=1.0\"\>

**Il meta tag viewport fornisce al browser istruzioni utili per adattare
le dimensioni e le proporzioni della pagina alla larghezza dello schermo
del dispositivo**.

In assenza di tale elemento, i browser dei dispositivi mobili applicano
l\'impostazione predefinita, ovvero eseguono il rendering della pagina
alla larghezza utilizzata per gli schermi desktop. Sulla base di ciò,
per migliorare l\'aspetto dei contenuti, i browser aumentano
automaticamente la dimensione dei caratteri e/o ridimensionano i
contenuti in base allo schermo, assicurandosi di visualizzare l'intera
pagina senza costringere l'utente a dover scrollare orizzontalmente

Per gli utenti, questo significa che le dimensioni dei caratteri
potrebbero avere un aspetto disomogeneo e che potrebbe essere necessario
toccare due volte lo schermo o avvicinare le dita eseguendo lo zoom per
visualizzare e interagire con i contenuti. Per Google, invece, la pagina
potrebbe **non essere riconosciuta come ottimizzata per i dispositivi
mobili**, poiché richiede questo tipo di interazione.

Al contrario utilizzando il meta tag viewport come sopra indicato,
stiamo dicendo in maniera specifica al browser del dispositivo di
assegnare al viewport esattamente la larghezza del device perché saremo
poi noi ad occuparci di ottimizzare i contenuti e non avremo quindi
bisogno di alcun adattamento automatico.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gr_1.png](./assets/media/image46.png)

Per la pagina raffigurata a sinistra non è stato specificato alcun meta
tag viewport. Di conseguenza il browser del dispositivo mobile
presuppone che lo schermo abbia l\'ampiezza di un computer desktop e
adatta in modo conforme le proporzioni della pagina, ostacolando la
lettura dei contenuti.

A destra è rappresentata la stessa pagina con un viewport specificato,
che corrisponde all\'ampiezza dello schermo del dispositivo. Il browser
del dispositivo mobile, pertanto, non ridimensiona la pagina e non
impedisce la lettura dei contenuti.

A questo punto potrebbe però sorgere anche un dubbio: come facciamo a
sapere, in pixel, quanto è largo il viewport dei vari dispositivi per
ottimizzare i contenuti?

In realtà, come capiremo meglio in seguito, questa informazioni potrebbe
non servirci affatto. In ogni caso se proprio non possiamo farne a meno,
a [questo indirizzo](http://viewportsizes.com/) è possibile trovare una
lista delle dimensioni del viewport su tutti i principali dispositivi.

