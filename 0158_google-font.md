# GOOGLE FONT



Sino all\'avvento dei CSS3 gli sviluppatori di pagine web erano
\"costretti\" ad utilizzare nei loro progetti unicamente i cosiddetti
font standard ovvero i set di caratteri universalmente diffusi e quindi
presenti sulla stragrande maggioranza dei pc.

Nel momento in cui si sviluppa una pagina web, infatti, lo sviluppatore
\"dice al client\" quale font utilizzare pre renderizzare il testo. Il
client cerca quindi tra i font presenti sullo specifico pc per vedere se
è disponibile quello definito dal web designer: se presente procede come
da istruzioni, in caso contrario utilizzerà invece uno dei font di
default.

Questo meccanismo imponeva ai webmaster, al fine di mantenere un
risultato visuale omogeneo, di utilizzare sempre gli stessi font (come
ad esempio Times New Roman, Verdana, Arial, ecc.) con una grossa
limitazione dell\'aspetto creativo del lavoro.

Con i CSS3, fortunatamente, è stata introdotta la possibilità per i
webmaster di utilizzare, nelle proprie pagine web, anche font non
standard. Attraverso il comando \@font-face, infatti, è possibile
inviare al client il file (nei formati TTF, EOT, WOFF o SVG a seconda
del browser in uso) contenente il set di caratteri da utilizzare per
quella specifica pagina web.

In questo modo il client non deve più cercare se il font è già
installato sul computer in uso ma utilizza direttamente il set di
caratteri \"linkato\" nel foglio di stile.

Il servizio Google Fonts API nasce sulla scia delle novità introdotte da
CSS3.

Nei laboratori di Google è stato sviluppato un sistema (basato sulla
tecnologia appena descritta) che consente a tutti i web designer di
incorporare nelle proprie pagine web, in modo molto semplice e con
minimi interventi sul codice, font non standard senza dover implementare
direttamente le direttive CSS3 e, soprattutto, senza dover caricare i
file del font nel proprio spazio web (tutti i file necessari, infatti,
risiedono stabilmente sui server di Google).

Di base, il funzionamento del servizio è molto semplice:

- si accede alla libreria dei font disponibili;

- si sceglie il font preferito;

- si aggiunge una riga di codice al sito;

In questo modo il nuovo font-family sarà disponibile per essere
utilizzato nelle pagine del nostro sito web.

L'implementazione dei tre passaggi sopra indicati è già presente in
Passweb in maniera nativa per cui per poter utilizzare un Google Font
all'interno del proprio sito è sufficiente includerlo mediante
l'apposita funzionalità presente nei vari Layout di pagina e/o di sito.

Nel successivo capitolo di questo manuale verrà esaminata nel dettaglio
la procedura da seguire attivare ed integrare i Google Font all'interno
del proprio sito

