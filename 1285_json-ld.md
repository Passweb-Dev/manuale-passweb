# JSON-LD



Tra le diverse tipologie di dati strutturati il **JSON-LD** è oggi
quello che si è affermato come lo standard più diffuso e raccomandato da
Google e dagli altri principali motori di ricerca. Il motivo è semplice:
**JSON-LD è leggibile, flessibile, pulito e facilmente integrabile in
qualsiasi pagina web**, senza interferire con il codice HTML.

**ATTENZIONE!** **Per attivare la gestione dei dati strutturati nel
formato JSON-LD è necessario attivare il relativo modulo su Passstore**

Il termine JSON-LD è l'acronimo di **JavaScript Object Notation for
Linked Data**.

Per capire il suo significato, possiamo scomporlo in due parti:

- **JSON (JavaScript Object Notation)** è un formato leggero per la
  rappresentazione dei dati, basato su coppie chiave/valore e facilmente
  interpretabile sia dagli esseri umani sia dai computer. È ampiamente
  usato nello sviluppo web per scambiare dati tra client e server.

- **LD (Linked Data)** si riferisce al concetto di dati collegati, cioè
  informazioni connesse tra loro secondo una logica semantica, in modo
  che le macchine possano comprendere non solo i singoli elementi ma
  anche le loro relazioni.

Prima dell'introduzione di JSON-LD il formato più utilizzato per i dati
strutturati era quello dei Microdati che, come visto nel precedente
capitolo di questo manuale, prevede l'inserimento di queste meta
informazioni direttamente all'interno del codice HTML, utilizzando
attributi speciali come itemtype e itemprop.

Sebbene questo metodo risulti essere sicuramente corretto ed ancora
piuttosto utilizzato presenta comunque diversi svantaggi:

- **Complica l'HTML**: i tag diventavano lunghi e difficili da
  mantenere.

- **Difficile aggiornamento**: ogni variazione dei dati richiedeva
  modifiche dirette nell'HTML.

- **Maggiore rischio di errore**: un tag aperto o chiuso nel modo
  sbagliato poteva invalidare la struttura.

- **Scarsa separazione tra contenuto e metadati**.

Il formato JSON-LD risolve tutti questi problemi. I metadati sono
separati dal contenuto visibile e sono raccolti in un unico blocco
facilmente leggibile e modificabile.

Dal punto di vista tecnico infatti un JSON-LD non è altro che un piccolo
frammento di codice JSON che **descrive il significato dei dati presenti
nella pagina**.

In pratica, si tratta di uno script con tipo **application/ld+json**
inserito all'interno della pagina web (solitamente nel tag \< head \> ma
è piuttosto comunque trovarlo anche all'interno del tag \< body \>).
All'interno di questo script si trovano le informazioni semantiche: il
nome di un prodotto, il suo prezzo, la disponibilità, la valutazione
media, le recensioni e così via.

Ecco un piccolo esempio:

*\<script type=\"application/ld+json\"\>*

*{*

*\"@context\": \"https://schema.org/\",*

*\"@type\": \"Product\",*

*\"name\": \"Scarpe da corsa uomo\",*

*\"image\": \[*

*\"https://www.miosito.it/media/products/airspeed-x-front.jpg\",*

*\"https://www.miosito.it/media/products/airspeed-x-side.jpg\",*

*\"https://www.miosito.it/media/products/airspeed-x-back.jpg\"*

*\],*

*\"description\": \"Scarpe da corsa leggere con suola ammortizzata.\",*

*\"sku\": \"SC12345\",*

*\"offers\": {*

*\"@type\": \"Offer\",*

*\"priceCurrency\": \"EUR\",*

*\"price\": \"89.90\",*

*\"availability\": \"https://schema.org/InStock\"*

*}*

*}*

*\</script\>*

Questo piccolo blocco di codice è completamente separato dal markup
HTML, non è visibile per l'utente, ma comunica ai motori di ricerca
esattamente che cosa rappresenta il contenuto della pagina. Quando
Google analizza la pagina, riconosce che si tratta di un prodotto, ne
legge il nome, la descrizione, l'immagine, il prezzo e lo stato di
disponibilità, e può utilizzare queste informazioni per arricchire il
risultato di ricerca con **rich snippets**, ovvero elementi visivi
aggiuntivi come stelle, prezzi, o immagini.

Ogni frammento JSON-LD inizia con una proprietà chiamata
***\@context***.

Il suo valore tipico è:

*\"@context\": \"https://schema.org/\",*

Questo indica che il vocabolario semantico utilizzato per interpretare i
dati è, come per i Microdati, quello di **Schema.org**, un progetto
collaborativo avviato da Google, Microsoft, Yahoo e Yandex. Schema.org
che, come detto, definisce centinaia di tipi di entità (come *Product*,
*Event*, *Person*, *Organization*, *Recipe*, ecc.) e le relative
proprietà standardizzate.

Il contesto è fondamentale perché consente ai motori di ricerca di
sapere a quale significato attribuire ogni proprietà. Ad esempio, "name"
può essere il nome di un prodotto, di una persona o di un evento; è il
contesto che stabilisce come deve essere interpretato.

Accanto al contesto, il JSON-LD utilizza la proprietà ***\@type*** per
indicare la tipologia di entità descritta. Ad esempio:

- \"@type\": \"Product\" indica che si tratta di un prodotto.

- \"@type\": \"Organization\" indica che si tratta di un'azienda.

- \"@type\": \"BreadcrumbList\" indica che si tratta di una struttura di
  navigazione.

- \"@type\": \"Review\" rappresenta una recensione.

- ...

Spesso, in una stessa pagina, vengono usati più tipi diversi per
descrivere entità collegate tra loro. È possibile, ad esempio, inserire
in un unico script JSON-LD sia il *Product* principale sia le *Review*
dei clienti, oppure utilizzare la struttura *\@graph* per collegare
logicamente più entità (ad esempio un prodotto, il suo marchio e
l'organizzazione venditrice).

Una volta compreso il modo in cui il formato JSON-LD tende a
rappresentare e ad esporre le informazioni ai motori di ricerca,
piuttosto che ai sistemi di AI, alle piattaforme social, a Google
Shopping o ad un qualunque altro sistema automatico, resta ora da capire
come poter effettivamente riportare tutto questo all'interno del proprio
sito Passweb.

Come per i microdati, anche in questo caso, è possibile procedere in due
modi diversi dipendentemente dal tipo di informazione (quindi dal tipo
di Schema, visto che il vocabolario semantico è comunque sempre quello
di schema.org) che si intende adottare e dallo specifico Componente
Passweb utilizzato.

Nel caso in cui l'informazione da descrivere tramite JSON-LD sia
relativa ad una Persona, un Indirizzo, un Video, un Numero di Telefono o
comunque relativa ad un qualche cosa **implementabile in Passweb con
componenti non Ecommerce**, è possibile utilizzare il **componente
HTML** e inserire direttamente al suo interno lo script contente il
JSON-LD desiderato

**Nel caso in cui invece l'informazione da descrivere mediante JSON-LD
sia relativa ad elementi più prettamente Ecommerce (Recensioni,
Prodotti, Prezzi, Disponibilità ecc...),** sarà necessario agire, come
per i microdati, dalla sezione "**Dati Strutturati"**" presente
all'interno della pagina "*Sito -- Preferenze -- Integrazioni*" del
Wizard impostando, questa volta, il parametro "**Formato dati
strutturati**" sull'opzione "JSON-LD"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_1.bmp](./assets/media/image3.png)

**ATTENZIONE!** nel momento in cui si dovesse variare l'impostazione
settata per il parametro "Formato dati strutturati", passando ad esempio
da Microdata a Json-ld o viceversa, per vedere l'effettiva modifica nel
codice sorgente della pagina sarà necessario eliminare prima i cookie
del browser

I check presenti in corrispondenza del parametro "**Proprietà gestite**"
(sezione "**Schema Ecommerce**") consentono poi di abilitare o meno
determinate proprietà del JSON-LD relative al tipo di informazione che
si vuole o non si vuole rappresentare

Nello specifico il check:

- **Schema BreadcrumbList:** consente di abilitare lo Schema relativo
  alle cosiddette "Briciole di Pane" e di inserire quindi, in maniera
  automatica, in tutte le pagine del sito in cui è presente il
  componente Passweb "**Info Navigazione**" un JSON-LD analogo a quello
  di seguito indicato:

> *\<script type=\"application/ld+json\"\>*
>
> *{*
>
> *\"@context\": \"https://schema.org/\",*
>
> *\"@type\": \"BreadcrumbList\",*
>
> *\"itemListElement\": \[*
>
> *{*
>
> *\"@type\": \"ListItem\",*
>
> *\"position\": 1,*
>
> *\"name\": \"Home\",*
>
> *\"item\": \"https://www.miosito.it/\"*
>
> *},*
>
> *{*
>
> *\"@type\": \"ListItem\",*
>
> *\"position\": 2,*
>
> *\"name\": \"Calzature sportive\",*
>
> *\"item\": \"https://www.miosito.it/prodotti/calzature-sportive\"*
>
> *},*
>
> *{*
>
> *\"@type\": \"ListItem\",*
>
> *\"position\": 3,*
>
> *\"name\": \"Scarpe running AirSpeed X\",*
>
> *\"item\":
> \"https://www.miosito.it/prodotto/scarpe-running-airspeed-x\"*
>
> *}*
>
> *\]*
>
> *\</script\>*

- **Schema Product:** consente di abilitare lo Schema Product relativo
  ai prodotti venduti all'interno di un sito Ecommerce e di inserire
  quindi, in maniera automatica, in tutte le **Pagine Prodotto** del
  sito un JSON-LD analogo a quello di seguito indicato:

> *\<script type=\"application/ld+json\"\>*
>
> *{*
>
> *\"@context\": \"https://schema.org/\",*
>
> *\"@type\": \"Product\",*
>
> *\"name\": \"Scarpe running AirSpeed X\",*
>
> *\"description\": \"Scarpe da corsa ultraleggere con tecnologia di
> ammortizzazione AirSpeed. Ideali per allenamenti e gare.\",*
>
> *\"sku\": \"ASX-2025\",*
>
> *\"image\": \[*
>
> *\"https://www.miosito.it/media/products/airspeed-x-front.jpg\",*
>
> *\"https://www.miosito.it/media/products/airspeed-x-side.jpg\",*
>
> *\"https://www.miosito.it/media/products/airspeed-x-back.jpg\"*
>
> *\],*
>
> *\"offers\": {*
>
> *\"@type\": \"Offer\",*
>
> *\"url\":
> \"https://www.miosito.it/prodotto/scarpe-running-airspeed-x\",*
>
> *\"priceCurrency\": \"EUR\",*
>
> *\"price\": \"129.90\",*
>
> *\"availability\": \"https://schema.org/InStock\",*
>
> *\"seller\": {*
>
> *\"@type\": \"Organization\",*
>
> *\"name\": \"SportTech Store\"*
>
> *}*
>
> *},*
>
> *\"aggregateRating\": {*
>
> *\"@type\": \"AggregateRating\",*
>
> *\"ratingValue\": \"4.7\",*
>
> *\"reviewCount\": \"138\",*
>
> *\"bestRating\": \"5\",*
>
> *\"worstRating\": \"1\"*
>
> *},*
>
> *\"review\": \[*
>
> *{*
>
> *\"@type\": \"Review\",*
>
> *\"author\": {*
>
> *\"@type\": \"Person\",*
>
> *\"name\": \"Marco Rossi\"*
>
> *},*
>
> *\"datePublished\": \"2025-09-15\",*
>
> *\"reviewBody\": \"Scarpe leggerissime e davvero comode. Ideali per
> correre su strada!\",*
>
> *\"reviewRating\": {*
>
> *\"@type\": \"Rating\",*
>
> *\"ratingValue\": \"5\",*
>
> *\"bestRating\": \"5\",*
>
> *\"worstRating\": \"1\"*
>
> *}*
>
> *},*
>
> *{*
>
> *\"@type\": \"Review\",*
>
> *\"author\": {*
>
> *\"@type\": \"Person\",*
>
> *\"name\": \"Laura Bianchi\"*
>
> *},*
>
> *\"datePublished\": \"2025-09-28\",*
>
> *\"reviewBody\": \"Ottimo comfort e materiali di qualità. Spedizione
> veloce.\",*
>
> *\"reviewRating\": {*
>
> *\"@type\": \"Rating\",*
>
> *\"ratingValue\": \"4\",*
>
> *\"bestRating\": \"5\",*
>
> *\"worstRating\": \"1\"*
>
> *}*
>
> *}*
>
> *\]*
>
> *\</script\>*
>
> dove le singole proprietà (e quindi le singole informazioni) possono
> anche essere gestite individualmente attivando o meno i relativi
> check.
>
> In questo senso infatti i check "sotto" lo "Schema Product" consentono
> rispettivamente di:

- **Codice Prodotto:** consente, se attivato, di inserire all'interno
  del JSON-LD la proprietà

> *\"sku\": \"ASX-2025\"*
>
> utilizzata per indicare ai motori di ricerca che il valore
> *\"ASX-2025\"* è esattamente il codice di quello specifico prodotto

- **Descrizione Prodotto:** consente, se attivato, di inserire
  all'interno del JSON-LD la proprietà

> *\"description\": \"Scarpe da corsa ultraleggere con tecnologia di
> ammortizzazione AirSpeed. Ideali per allenamenti e gare.\"*
>
> utilizzata per segnalare ai motori di ricerca che il valore indicato
> in corrispondenza della chiave *"description"* è esattamente la
> descrizione di quello specifico prodotto.

- **Immagine Prodotto:** consente, se attivato, di inserire all'interno
  del JSON-LD la proprietà

> *\"image\": \[*
>
> *\"https://www.miosito.it/media/products/airspeed-x-front.jpg\",*
>
> *\"https://www.miosito.it/media/products/airspeed-x-side.jpg\",*
>
> *\"https://www.miosito.it/media/products/airspeed-x-back.jpg\"*
>
> *\]*
>
> utile per indicare al motore di ricerca quelle che sono le immagini
> del prodotto in esame

- **Titolo Prodotto:** consente, se attivato, di inserire all'interno
  del JSON-LD la proprietà

> *\"name\": \"Scarpe running AirSpeed X\",*
>
> utilizzata per indicare ai motori di ricerca che il valore *\" Scarpe
> running AirSpeed X \"* è esattamente il nome di quello specifico
> prodotto

- **Schema Offer/AggregateOffer:** consente, se abilitato, di inserire
  all'interno dello Schema Product, la proprietà *"offers*"

> *\"offers\": {*
>
> *\"@type\": \"Offer\",*
>
> *\"url\":
> \"https://www.miosito.it/prodotto/scarpe-running-airspeed-x\",*
>
> *\"priceCurrency\": \"EUR\",*
>
> *\"price\": \"129.90\",*
>
> *\"availability\": \"https://schema.org/InStock\",*
>
> *\"seller\": {*
>
> *\"@type\": \"Organization\",*
>
> *\"name\": \"SportTech Store\"*
>
> *}*
>
> *}*
>
> gestita come un oggetto con le relative proprietà, e utilizzata quindi
> per indicare al motore di ricerca informazioni di diverso tipo. Nello
> specifico la proprietà:

- *"url"* verrà valorizzata con l'url della corrispondente pagina
  prodotto e servirà quindi per indicare al motore di ricerca dove
  andare a verificare effettivamente la correttezza delle informazioni
  inserite

- *\"priceCurrency\"* verrà utilizzata per indicare al motore di ricerca
  la valuta utilizzata nella definizione del prezzo articolo

- *"price"* verrà utilizzata per segnalare al motore di ricerca che il
  valore indicato è esattamente il prezzo del relativo prodotto

- *\"availability\"* verrà utilizzata per segnalare al motore di ricerca
  (con notazione "*https://schema.org/InStock"* o
  *"https://schema.org/OutOfStock"*) se il prodotto in esame risulta o
  meno disponibile

> **ATTENZIONE!** a differenza delle altre proprietà dell'oggetto
> "*offers*" la proprietà *\"availability\"* verrà inserita o meno nel
> JSON-LD a seconda del fatto di aver selezionato o deselezionato il
> successivo check "**Disponibilità prodotto**"

- *"seller"* gestita a sua volta come un oggetto in cui la proprietà
  *"name"* verrà utilizzata per indicare al motore di ricerca il nome
  del venditore di quello specifico prodotto

> **ATTENZIONE**! la proprietà *"name"* dell'oggetto *"seller"* verrà
> valorizzata automaticamente con il "**Nome del Sito**" inserito in
> corrispondenza del relativo campo presente alla pagina "**Preferenze
> Sito**" (sezione SEO) del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_seller_name.bmp](./assets/media/image4.png)

- **Disponibilità prodotto:** consente, se attivato, di inserire
  all'interno del JSON-LD, nella sezione relativa all'oggetto *"offers"*
  la proprietà

> *\"availability\": \"https://schema.org/InStock\"*
>
> gestita, come detto con notazione "*https://schema.org/InStock"* o
> *"https://schema.org/OutOfStock"* e utilizzata per indicare al motore
> di ricerca se il prodotto in esame risulta o meno disponibile

- **Venditore -- gestito solo per JSON-LD**: consente, se attivato, di
  inserire all'interno del JSON-LD, nella sezione relativa all'oggetto
  *"offers"* l'oggetto

> *\"seller\": {*
>
> *\"@type\": \"Organization\",*
>
> *\"name\": \"SportTech Store\"*
>
> *}*
>
> in cui la proprietà *"name"* valorizzata, come precedentemente
> indicato con il "**Nome del Sito**" inserito in corrispondenza del
> relativo campo presente alla pagina "**Preferenze Sito**" (sezione
> SEO) del Wizard, verrà utilizzata per indicare al motore di ricerca il
> nome del venditore dello specifico prodotto
>
> **ATTENZIONE!** lo schema **Offer/AggregateOffer** (così anche come le
> proprietà "Disponibilità Prodotto" e "Venditore") richiede la
> precedente attivazione dello Schema Product e, in conseguenza di ciò,
> verrà applicato solo ed esclusivamente al JSON-LD presente nelle
> pagine prodotto del sito.

- **Schema AggregateRating:** consente, se abilitato, di inserire
  all'interno dello Schema Product, la proprietà *"aggregateRating*"

> *\"aggregateRating\": {*
>
> *\"@type\": \"AggregateRating\",*
>
> *\"ratingValue\": \"4.7\",*
>
> *\"reviewCount\": \"138\",*
>
> *}*
>
> legata al Componente Passweb "**Rating Review**" e utilizzata quindi
> per indicare al motore di ricerca, rispettivamente, la media e il
> numero di voti espressi dagli utenti sul prodotto in esame
>
> **ATTENZIONE!** lo schema **AggregateRating** richiede, ovviamente, la
> precedente attivazione dello Schema Product e, in conseguenza di ciò,
> verrà applicato solo ed esclusivamente al JSON-LD presente nelle
> pagine prodotto del sito. Inoltre essendo legato al componente
> "**Rating Review**" verrà effettivamente inserito solo nel caso in cui
> tale componente sia stato effettivamente utilizzato e il prodotto
> abbia ricevuto dei voti.

- **Schema Review:** consente, se abilitato, di inserire all'interno
  dello Schema Product l'array di oggetti "*review*"

> *\"review\": \[*
>
> *{*
>
> *\"@type\": \"Review\",*
>
> *\"author\": {*
>
> *\"@type\": \"Person\",*
>
> *\"name\": \"Marco Rossi\"*
>
> *},*
>
> *\"datePublished\": \"2025-09-15\",*
>
> *\"reviewBody\": \"Scarpe leggerissime e davvero comode. Ideali per
> correre su strada!\"*
>
> *},*
>
> *...*
>
> *{*
>
> *\"@type\": \"Review\",*
>
> *\"author\": {*
>
> *\"@type\": \"Person\",*
>
> *\"name\": \"Laura Bianchi\"*
>
> *},*
>
> *\"datePublished\": \"2025-09-28\",*
>
> *\"reviewBody\": \"Ottimo comfort e materiali di qualità. Spedizione
> veloce.\"*
>
> *}*
>
> *\]*
>
> legato al Componente Passweb **"Commenti Associati"** e utilizzato
> quindi per indicare al motore di ricerca quelli che sono i
> commenti/recensioni effettuati dagli utenti del sito relativamente al
> prodotto in esame
>
> Come per lo Schema Offer/AggregateOffer, trattandosi di un oggetto, o
> meglio ancora di un array di oggetti, i successivi check consentiranno
> di abilitarne o meno le singole proprietà.
>
> In particolare il check:

- **Testo commento**: consente, se abilitato, di inserire all'interno
  dell'oggetto "*review*" la proprietà "*reviewBody"* utilizzata per
  segnalare al motore di ricerca che il valore indicato in
  corrispondenza di questa chiave è esattamente il commento effettuato
  dall'utente

- **Data commento**: consente, se abilitato, di inserire all'interno
  dell'oggetto "*review*" la proprietà "*datePublished"* utilizzata per
  segnalare al motore di ricerca che il valore indicato in
  corrispondenza di questa chiave è esattamente la data in cui l'utente
  ha effettuato il commento in esame

- **Autore commento**: consente, se abilitato, di inserire all'interno
  dell'oggetto *"review"* l' oggetto *"author"* la cui proprietà "name"
  verrà utilizzata per segnalare al motore di ricerca che il valore
  indicato in corrispondenza di questa chiave è esattamente il nome
  dell'autore del commento

> **ATTENZIONE!** lo schema **Review** richiede, ovviamente, la
> precedente attivazione dello Schema Product e, in conseguenza di ciò,
> verrà applicato solo ed esclusivamente al JSON-LD presente nelle
> pagine prodotto del sito. Inoltre essendo legato al componente
> "**Commenti Associati**" verrà effettivamente inserito solo nel caso
> in cui tale componente sia stato effettivamente utilizzato e il
> prodotto abbia quindi delle recensioni

Come si può facilmente comprendere i check presenti in corrispondenza
del parametro "Proprietà gestite" consentono di attivare solo una parte
delle proprietà disponibili per lo Schema Product, nello specifico
quelle gestite in automatico da Passweb su cui l'utente non avrebbe
possibilità di intervento se non optando per un inserimento manuale di
tutto il JSON-LD all'interno di ogni singola scheda prodotto.

Nel momento in cui l'esigenza dovesse essere dunque quella di integrare
il JSON-LD gestito in automatico da Passweb aggiungendo altre proprietà,
relative sempre allo Schema Product, ma diverse da quello che può essere
il titolo, la descrizione, il prezzo, la disponibilità ecc... sarà
necessario utilizzare il JSON Builder presente all'interno della sezione
"**Struttura JSON-LD**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder.bmp](./assets/media/image5.png)

Per maggiori informazioni in merito all'utilizzo di questo strumento si
veda quanto indicato nel successivo capitolo "*JSON Builder*" di questo
manuale.

Una volta abilitati i check relativi alle proprietà del JSON-LD gestite
in automatico da Passweb e impostate anche eventuali proprietà custom
tramite l'utilizzo del JSON Builder, sarà poi necessario avviare la
creazione del JSON-LD utilizzando per questo il pulsante "**Generazione
JsonLD prodotti**"

**ATTENZIONE!** il pulsante "**Generazione JsonLD prodotti**" avvia il
processo di creazione del JSON-LD per tutti i prodotti attualmente
gestiti sul sito. Tale processo potrebbe quindi richiedere diverso tempo
in relazione al numero effettivo di prodotti da processare.
L'amministratore del sito verrà avvisato mediante un'apposita mail al
termine del processo

Per maggiori informazioni in merito a come Passweb provvederà poi alla
creazione dei JSON-LD configurati all'interno di questa sezione del
Wizard, si rimanda a quanto indicato nel successivo capitolo
"Generazione dei JSON-LD" di questo manuale.

