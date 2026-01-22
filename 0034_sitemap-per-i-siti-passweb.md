# SITEMAP PER I SITI PASSWEB



Una Sitemap XML altro non è se non uno specifico file .xml costruito
seguendo standard ben definiti e utilizzato per fornire agli spider dei
vari motori di ricerca l'elenco di tutti gli URL del proprio sito web
che si desidera sottoporre a questi stessi motori, ai fini di una loro
corretta indicizzazione.

Tale file è quindi particolarmente utile per cercare di ottimizzare il
proprio sito web e migliorarne l'indicizzazione ed il posizionamento sui
motori di ricerca (la presenza di una Sitemap xml rende la scansione del
sito più semplice per Google così come per qualsiasi altro motore di
ricerca).

L'utilizzo del file Sitemap è anche un metodo per far sapere a Google
quale versione di un dato URL è da preferirsi rispetto alle altre

Generalmente questi file possono essere ottenuti attraverso uno dei
tanti tool gratuiti disponibili in rete ( si possono ottenere ad esempio
anche tramite gli Strumenti per i Webmaster di Google stesso) e
andrebbero poi caricati manualmente nella root del sito stesso.

**In questo senso Passweb implementa un tool completamente automatico
per la generazione e la gestione della Sitemap del proprio sito web
mettendo quindi a disposizione degli spider dei vari motori di ricerca
una Sitemap sempre aggiornata e coerente con la struttura attuale del
proprio sito web.**

Inoltre è possibile decidere, per ogni singola pagina, per ogni singolo
prodotto e per ogni singolo articolo CMS se questo stesso elemento dovrà
o meno essere inserito nella SiteMap e, in caso affermativo, quale sia
la frequenza di aggiornamento e la priorità che dovrà essergli assegnata
all'interno della SiteMap stessa.

**Nota Bene:** per maggiori informazioni in merito a come poter decidere
se una specifica pagina dovrà o meno essere inserita nella SiteMap ed
eventualmente con che frequenza di aggiornamento e con che priorità si
veda anche il capitolo "Sito -- Preferenze -- SiteMap Pagine" di questo
manuale

**ATTENZIONE!!!** impostare per ogni singola pagina del sito, articolo o
contenuto CMS che si vuol indicizzare, e che si è quindi deciso di
inserire nella SiteMap, il corretto valore della frequenza di
aggiornamento e della priorità, **creando quindi una SiteMap il più
realistico** **possibile,** è uno dei fattori determinanti per una
corretta indicizzazione dei contenuti del proprio sito.

Per visualizzare la Sitemap del proprio sito, generata in automatico da
Passweb, è sufficiente digitare nella barra degli indirizzi del browser
l'indirizzo del sito stesso seguito dalla stringa **"/sitemap.xml**".

**Supponendo quindi di fare riferimento al sito con dominio
www.esempio.passweb.it, la Sitemap sarà accessibile e visualizzabile
all'indirizzo www.esempio.passweb.it/sitemap.xml e soprattutto verrà
generata dinamicamente nel momento stesso in cui verrà richiesta questa
specifica risorsa.**

E' semplice comprendere dunque come l'utente non debba preoccuparsi, a
seguito di eventuali variazioni apportate alla struttura del proprio
sito web, di andare a rigenerare manualmente la Sitemap e di sostituirla
alla vecchia, in quanto, come detto, la nuova Sitemap verrà generata
dinamicamente nel momento stesso in cui i vari spider la richiederanno e
rifletterà sempre l'esatta struttura e configurazione del proprio sito
web.

**ATTENZIONE! Passweb genera automaticamente la sitemap del sito, è
necessario però indicare in maniera esplicita agli spider il percorso in
cui poter localizzare tale risorsa. Per far questo è sufficiente
inserire, come da specifiche di Google, in un qualsiasi punto del file
robots.txt la seguente riga:**

**Sitemap: www.esempio.passweb.it/sitemap.xml**

**dove, ovviamente, al posto di www.esempio.passweb.it andrà inserito l'
url del proprio sito web**

Per quel che riguarda, infine**, i siti multilingua**, la sitemap
generata in automatico da Passweb conterrà l'elenco completo degli url
di tutte le pagine che si è deciso di inserire all'interno della sitemap
stessa, in tutte le lingue di gestione del sito.

In queste condizioni, inoltre, per ogni url verrà indicata anche la sua
versione equivalente nelle altre lingue del sito, utilizzando per questo
gli attributi **rel=\"alternate\"** e **hreflang=\"x\"** (attributi
questi utilizzati poi da Google per visualizzare la lingua o l\'URL
locale corretti nei risultati di ricerca) e seguendo esattamente,
dunque, le specifiche in materia indicate da Google stesso

(<https://support.google.com/webmasters/answer/189077?hl=it> ,
<https://support.google.com/webmasters/answer/2620865?hl=it> )

Di seguito viene riportato un esempio di sitemap generata in automatico
da Passweb relativamente ad un sito gestito in italiano, francese e
inglese.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sitemap_multilingua.bmp](./assets/media/image61.png){width="4.616666666666666in"
height="4.825in"}

Tipicamente nella realizzazione e nella gestione di sitemap per siti
multilingua, del tipo dunque di quella rappresentata in figura, è
possibile incappare in due diverse tipologie di errori piuttosto comuni
che potrebbero portare gli spider, come indicato da google stesso, ad
ignorare o a non interpretare nella maniera corretta le indicazioni
relative alle pagine in lingua:

- **Codici lingua sbagliati**: i codici lingua utilizzati nella sitemap
  devono identificare esattamente la lingua secondo le specifiche ISO
  639-1 e, facoltativamente, l\'area geografica (in formato ISO 3166-1
  Alpha 2)

- **Assenza di link di conferma:** se la pagina A, inserita nella
  sitemap rimanda alla pagina B, la pagina B deve rimandare
  necessariamente alla pagina A.

Ora, mentre il primo problema è risolto direttamente da Passweb che
genera automaticamente la sitemap del sito utilizzando esattamente i
codici lingua come da specifiche ISO 639-1, per il secondo problema
dovrà essere invece l'amministratore del sito ad accertarsi che la
pagina A contenga un link alla pagina B e che la pagina B contenga a sua
volta un link alla pagina A, utilizzando per questo, ad esempio, un
semplice componente menu con link alla versione in lingua della stessa
pagina e accertandosi di distribuire questo componente in tutte le
pagine presenti nella sitemap.

Un altro aspetto particolarmente importante da prendere in
considerazione in queste condizioni infine, è che l'inserimento in
sitemap di tutti gli url delle pagine, in tutte le lingue gestite e con
i vari riferimenti incrociati, potrebbe ovviamente comportare un aumento
considerevole del numero di voci presenti all'interno della sitemap
stessa.

Questo di per se potrebbe comportare un problema, considerando che
all'interno di una singola sitemap non è possibile inserire più di 50000
voci.

Il tool di generazione automatica della sitemap di Passweb gestisce
anche questo tipo di casistica ricorrendo, come da specifiche Google
(<https://support.google.com/webmasters/answer/75712?hl=it> ), alla
cosiddetta sitemap index e a più sitemap distinte.

Nello specifico, nel momento in cui le voci presenti in sitemap,
dovessero superare le 50000 unità (ad esempio a causa della gestione
multilingua) richiamando l'indirizzo
**www.esempio.passweb.it/sitemap.xml** non verrà più generata e
restituita la sitemap del sito ma bensì la sua **Sitemap Index** che
avrà un formato del tipo di quello indicato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sitemap_index.bmp](./assets/media/image62.png){width="3.9479166666666665in"
height="1.363888888888889in"}

In sostanza dunque questa Sitemap Index non fa altro che indicare allo
spider i percorsi delle singole sitemap (generate sempre in automatico
da Passweb) ciascuna però con un massimo di 50000 voci.

Nel momento in cui lo spider, leggendo la sitemap index, andrà poi a
visitare l' url **www.esempio.passweb.it/sitemap1.xml** Passweb generà
in automatico la prima sitemap del sito contenente tutti gli url dal
numero 1 al numero 50000; quando invece lo spider andrà visitare
l'indirizzo **www.esempio.passweb.it/sitemap2.xml** Passweb genererà la
seconda sitemap con tutti gli url dal 50001 al 100000.

**ATTENZIONE! Si ricorda ancora la necessità di indicare esplicitamente
agli spider il percorso della sitemap inserendo, come da specifiche
Google, in un qualsiasi punto del file robots.txt la riga Sitemap:
www.esempio.passweb.it/sitemap.xml**

