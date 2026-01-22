# FEEDS



All'interno della sezione **"Feeds"** accessibile dalla voce di menu
***"Sito -- Gestione CMS"*** è possibile creare **Feed RSS** collegati
ad una o più Categoria News.

![](./assets/media/image560.png)

Tali Feed potranno poi essere esposti attraverso le pagine del proprio
sito web e permetteranno dunque ai visitatori del sito di iscriversi a
questi stessi Feeds in maniera tale da poter essere costantemente
aggiornati sulle notizie pubblicate all'interno delle Categorie News
collegate allo specifico canale.

In linea generale, infatti, lo standard **RSS** (acronimo **Really
Simple Syndication**) può essere definito come uno dei più popolari
formati per la distribuzione di contenuti Web. Da un punto di vista più
tecnico, invece, un **Feed RSS** altro non è se non un file .XML che
contiene, in forma strutturata, informazioni sulla pagina al quale è
legato e sui suoi contenuti .

Nel caso specifico ogni Feed RSS creato all'interno di un sito Passweb,
conterrà informazioni e notizie relative alla specifica categoria/e cui
risulta essere collegato. Nel momento in cui si andrà quindi a
pubblicare all'interno del proprio sito una nuova notizia, associandola
alla Categoria News collegata al Feed RSS, verrà contemporaneamente
aggiornato, in maniera completamente automatica, anche questo stesso
Feed e conseguentemente tutti gli utenti ad esso iscritti potranno
ricevere e leggere la nuova notizia.

Il principio di funzionamento dei Feed RSS è quindi molto semplice:
molti siti, soprattutto blog, forum, testate giornalistiche, portali,
presentano un Feed RSS sulle proprie pagine attraverso il quale offrono
notizie costantemente aggiornate. L\'utente interessato può indicare al
proprio programma di **News Aggregator** (sono disponibili, in questo
senso, anche servizi on-line e funzioni o plugin integrati direttamente
nel Browser) i Feed di suo interesse: il News Aggregator li controlla
con frequenza specificabile e riporta le novità individuate consentendo
di leggere le news in modo del tutto identico a quanto consentono di
fare i programmi di posta elettronica con le e-mail.

I News Aggregator dunque altro non sono se non \"lettori\" di Feed RSS
ossia programmi attraverso i quali è possibile aggregare, interpretare e
visualizzare dati scritti e distribuiti in questo dialetto di XML.

Per molti aspetti, gli aggregatori sono simili ai programmi di posta
elettronica, riproponendone l\'interfaccia che prevede il classico
layout a tre pannelli. In genere, nel pannello a sinistra trova posto la
lista dei feed sottoscritti. Selezionandone uno, nel pannello superiore
destro viene visualizzato l\'elenco dei titoli, mentre in quello
inferiore viene proposto il testo degli articoli o un loro riassunto.
Tutti i principali News Aggregator prevedono poi meccanismi per
evidenziare gli articoli non letti e il loro numero o per contrassegnare
gli stessi come letti o non letti.

Oltre all\'interfaccia, anche il metodo di funzionamento è simile a
quello dei client di posta elettronica: una volta sottoscritti i feed,
si apre il News Aggregator, si scaricano gli aggiornamenti e si leggono
i contenuti.

**NOTA BENE**: ogni sito Passweb può disporre di un suo News Aggregator
(costituito dal "Componente RSS") attraverso il quale poter prelevare e
visualizzare direttamente all'interno del proprio sito i contenuti di
vari Feed RSS.

Oltre ai News Aggregator che si possono scaricare direttamente da
Internet, è possibile sfruttare anche programmi di posta elettronica
(come ad esempio Microsoft Outlook) per visualizzare i contenuti e le
notizie di questi feed oppure direttamente i Browser solitamente
impiegati per navigare sul Web. Per venire incontro ai propri utenti,
infatti, sia Microsoft che Mozilla che Chrome hanno deciso di integrare
nelle nuove versioni dei loro Browser la funzionalità grazie alla quale,
attraverso un foglio di stile, il contenuto grezzo di un Feed viene
formattato in modo tale da poter essere visualizzato in un formato
decisamente più user friendly. I moderni Browser, inoltre, hanno
lavorano molto su diverse funzioni orientate a questa tecnologia: fra
queste, anche sull\'individuazione dei feed associati ad una pagina
attraverso l\'autodiscovery link grazie al quale, navigando su un sito
che offre un feed RSS o Atom (altro standard di comunicazione), il
Browser avverte l\'utente della sua presenza (attraverso un'apposita
icona) offrendo una lista di funzioni correlate.

Chiariti questi concetti di carattere generale relativi a cosa sia un
Feed RSS o un News Aggregator e a come poter utilizzare questi
strumenti, la procedura da seguire all'interno di Passweb per creare ed
esporre un Feed associato ad una o più Categorie News, è estremamente
semplice.

Per poter creare infatti un nuovo Feed RSS è sufficiente cliccare sul
pulsante "**Nuovo Feed**" presente nella barra degli strumenti della
maschera "**Gestione CMS -- Feeds**".

Verrà quindi visualizzata nella parte bassa della pagina la maschera
**"Nuovo Feed CMS"**

![](./assets/media/image561.png)

attraverso cui poter definire le proprietà e le caratteristiche del Feed
che si intende realizzare. In particolare dunque sarà necessario
specificare un valore per i seguenti campi:

- **Slug:** lo slug di un feed RSS altro non è se non la parte finale
  del permalink che va a costituire l'indirizzo web di pubblicazione del
  Feed stesso. Nel caso in cui si decidesse, ad esempio, di realizzare
  per il sito **www.nome_sito.passweb.it,** un Feed collegato alla
  Categoria News "Rassegna Stampa", come Slug di questo feed si potrebbe
  pensare di utilizzare il valore "**Nome_Sito--Rassegna Stampa**".

> In queste condizioni l' url di pubblicazione del Feed sarebbe del
> tipo:
>
> **http://www.nomesito.passweb.it?rf=Nome_Sito-Rassegna Stampa**
>
> dove, come detto, lo slug andrà a costituire l'ultima parte (quella
> dopo il parametro rf?=) dell'indirizzo web.
>
> In definitiva dunque lo slug di un Feed RSS dovrà essere costituito da
> quelle poche parole utili ad identificare il contenuto del Feed stesso
> e, in conseguenza di ciò **andrà ad assumere un'importanza
> fondamentale in termini di SEO e quindi di indicizzazione del Feed in
> esame.**

- **Nome Feed:** consente di definire il nome (descrittivo) del Feed che
  si sta realizzando. Tale nome sarà poi quello visualizzato agli utenti
  una volta esposto il Feed attraverso le pagine del proprio sito e
  quello dunque che gli utenti utilizzeranno per individuarne i
  contenuti

- **Categorie Associate:** consente di definire la/le Categoria/e di
  News che dovranno contribuire alla generazione del Feed che si sta
  realizzando. Nel momento in cui si andrà quindi a pubblicare
  all'interno del proprio sito una nuova notizia, associandola alla
  Categoria News collegata al Feed RSS, verrà contemporaneamente
  aggiornato, in maniera completamente automatica, anche questo stesso
  Feed e, conseguentemente, tutti gli utenti ad esso iscritti potranno
  ricevere e leggere la nuova notizia.

- **Numero di News per Feed:** consente di specificare il numero
  complessivo di Notizie che dovranno essere pubblicate e visualizzate
  all'interno del Feed che si sta realizzando

- **Pagine di Lettura Predefinita:** ogni Notizia pubblicata all'interno
  di un Feed e inviata dunque a tutti gli utenti iscritti a questo
  stesso Feed conterrà anche il link di destinazione in cui poter
  visualizzare il contenuto completo della relativa notizia.

> All'interno di questo campo sarà quindi necessario specificare, per
> ogni singola Variante Sito gestita (selezionabile mediante l'apposita
> linguetta), la pagina cui verrà ricondotto l'utente iscritto al feed
> per poter visualizzare il contenuto completo della notizia.
> All'interno di questa pagina dovrà quindi essere necessariamente
> inserito un componente CMS di tipo "Dettaglio News".

**NOTA BENE**: è necessario impostare una "Pagina di Lettura
Predefinita" per le Varianti Sito (desktop e mobile) attualmente on
line.

**NOTA BENE**: nel caso in cui nella pagina impostata come "Pagina di
Lettura Predefinita" per il Feed non sia presente il componente CMS
"Dettaglio News" l'utente non avrà modo di visualizzare il contenuto
delle relative notizie

Una volta impostati i parametri sopra indicati il pulsante **"Salva"**
presente nella parte bassa della maschera consente di salvare e
conseguentemente di generare il Feed RSS desiderato.

I Feed così salvati verranno quindi inseriti nell'elenco visualizzato
nella parte alta della maschera.

Infine cliccando sul pulsante raffigurante una piccola i, posto in
corrispondenza di ogni singolo Feed, sarà possibile visualizzare gli
indirizzi di pubblicazione del Feed stesso, sia in formato RSS 2.0 che
in formato Atom 1.0

![](./assets/media/image562.png)

**Dopo aver creato uno o più Feed RSS sarà necessario esporre questi
stessi Feed attraverso una o più pagine del proprio sito. In caso
contrario infatti gli utenti non avranno alcun modo di potersi iscrivere
a questi Feed se non conoscendo esattamente lo specifico indirizzo di
pubblicazione e visitando dunque la relativa pagina.**

Per poter esporre uno specifico Feed attraverso le pagine del proprio
sito web è sufficiente agire dalle proprietà della pagina stessa.

All'interno della sezione **"Feed Associati"** verrà infatti
visualizzato l'elenco dei Feed precedentemente realizzati.

Per esporre uno di questi Feed attraverso la corrispondente pagina web
sarà quindi sufficiente selezionarlo e cliccare successivamente sul
pulsante "Salva"

![](./assets/media/image563.png)

Una volta esposti questi Feed, nel momento in cui un utente dovesse
visitare la pagina utilizzata per l'esposizione con un Browser
opportunamente abilitato (es. Chrome con "Estensione Iscrizioni RSS"
abilitata e reperibile gratuitamente nel Chrome Store), comparirà nella
barra degli indirizzi la classica icona RSS ( ) ad indicare appunto la
possibilità da parte dell'utente di iscriversi ai Feed messi a
disposizione da questa stessa pagina.

Cliccando su questa icona verrà quindi visualizzato l'elenco dei Feed
esposti e l'utente avrà la possibilità di iscriversi a quello desiderato

Un metodo alternativo, e volendo anche più sicuro, per garantire agli
utenti la possibilità di iscriversi ai propri Feed RSS potrebbe essere
quello di utilizzare, molto semplicemente, **un componente "Immagine con
Link" collegandolo all'indirizzo dello specifico Feed (indirizzo questo
reperibile, come precedentemente evidenziato, all'interno della maschera
"Gestione CMS -- Feeds")**

In questo modo cliccando sull'immagine evidenziata l'utente verrà
ricondotto esattamente alla pagina di pubblicazione del relativo Feed da
cui potrà effettuare la sua iscrizione.

**In queste condizioni non è quindi richiesta la presenza sul browser
dell'utente di nessun plugin o estensione particolare per potersi
iscrivere ai Feed messi a disposizione dal proprio sito web**

