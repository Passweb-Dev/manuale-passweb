# ARTICOLI A TAGLIE E A COLORI GESTITI CON STRUTTURA + TABELLA TAGLIE/COLORI DI MEXAL



In questo scenario, supponendo di gestire la variante colore in
struttura e le taglie con la tabella Taglie di Mexal (ma sarebbe
sostanzialmente la stessa cosa invertendo i due elementi e gestendo
quindi le taglie in struttura e i colori nella Tabella Mexal) ci
troveremo a dover trattare:

- **un prodotto padre di struttura** con un suo codice, un suo url per
  la pagina prodotto ed eventualmente anche un suo prezzo specifico

- **N prodotti figlio**, corrispondenti alle varianti colore esportate
  sul sito, ciascuno con il suo codice, il suo url di pagina prodotto ed
  il suo prezzo. Ciascuna di queste varianti avrà poi N possibili taglie
  definite all'interno della corrispondente tabella gestionale

In queste condizioni verranno quindi gestiti due diversi formati di
JSON-LD uno, inserito nella pagina prodotto del padre di struttura e
l'altro inserito invece nelle pagine prodotto degli articoli figli e
dovremo indicare, in qualche modo, ai motori di ricerca qual' è
esattamente l'articolo padre, ossia il contenitore di tutte le varianti,
che come tale non potrà mai essere acquistato direttamente e quelli che
sono i prodotti figlio che potranno invece essere effettivamente
acquistati.

**[JSON-LD PER IL PADRE DI STRUTTURA]{.underline}**

Come detto l'articolo padre di struttura sarà solamente un "contenitore"
di tutte le possibili varianti, avrà un suo codice specifico, un suo
specifico url per la pagina prodotto e volendo potrebbe anche avere un
suo prezzo ma non potrà comunque essere mai acquistato. Inoltre a questo
padre di struttura dovranno essere collegati in qualche modo anche tutti
i prodotti figlio (varianti colore e taglie) che da esso derivano e che
potranno poi essere acquistati.

Per indicare al motore di ricerca, in maniera esplicita, tutte queste
cose, seguendo ovviamente le indicazioni del vocabolario di Schema.org,
e supponendo di gestire il colore come ultimo livello della struttura e
le taglie con la Tabella Taglie/Colori di Mexal, verrà utilizzato un
JSON-LD del tipo di quello di seguito indicato:

*\<script type=\"application/ld+json\"\>*

*{*

*\"@context\": \"https://schema.org/\",*

***\"@type\": \"ProductGroup\",***

***\"productGroupID\": \"FELPAUOMO01\",***

*\"name\": \"Felpa Uomo con Cappuccio\",*

*\"description\": \"Felpa in cotone con cappuccio disponibile in diversi
colori.\",*

*\"image\": \[*

*\"https://www.miosito.it/images/felpa-uomo-nero.jpg\",*

*\"https://www.miosito.it/images/fepa-uomo-rosso.jpg\",*

*\"https://www.miosito.it/images/felpa-uomo-blu.jpg\"*

*\],*

*\"offers\":{*

*\"@type\": \"Offer\",*

*\"url\": \"https://www.sito.it/felpa-uomo\",*

*\"priceCurrency\": \"EUR\",*

*\"price\": \"129.90\",*

*\"availability\": \"https://schema.org/InStock\",*

*\"seller\": {*

*\"@type\": \"Organization\",*

*\"name\": \"SportTech Store\"*

*}*

*},*

***\"hasVariant\":** \[*

*{*

*\"@type\": \"Product\",*

*\"name\": \"Felpa Uomo Blu\",*

*\"sku\": \"FELPAUOMO01-BLU\",*

*\"url\": \"https://www.sito.it/felpa-uomo-blu\",*

***"color": "Blu"***

*},*

*{*

*\"@type\": \"Product\",*

*\"name\": \"Felpa Uomo Rossa\",*

*\"sku\": \"FELPAUOMO01-ROSSA\",*

*\"url\": \"https://www.sito.it/felpa-uomo-rossa\",*

***"color": "Rosso"***

*}*

*\],*

*\"aggregateRating\":{*

*\"@type\": \"AggregateRating\",*

*\"ratingValue\": \"4.7\",*

*\"reviewCount\": \"68\"*

*},*

*\"review\": \[*

*{*

*\"@type\": \"Review\",*

*\"author\": {*

*\"@type\": \"Person\",*

*\"name\": \"Marco Rossi\"*

*},*

*\"datePublished\": \"2025-09-15\",*

*\"reviewBody\": \"Leggerissime e davvero comodo!\"*

*},*

*{*

*\"@type\": \"Review\",*

*\"author\": {*

*\"@type\": \"Person\",*

*\"name\": \"Laura Bianchi\"*

*},*

*\"datePublished\": \"2025-09-28\",*

*\"reviewBody\": \"Ottimo comfort e materiali di qualità. Spedizione
veloce.\"*

*}*

*\]*

*}*

*\</script\>*

dove:

- ***\"@type\": \"ProductGroup\"*** indica ai motori di ricerca che
  quello di cui si sta parlando non è un prodotto acquistabile ma una
  sorta di contenitore di N varianti, ciascuna con il suo codice e la
  sua pagina prodotto che saranno poi gli articoli effettivamente
  acquistabili

- ***\"productGroupID\": \"FELPAUOMO01\"*** valorizzato con il codice
  articolo del prodotto padre di struttura. Viene utilizzato come
  identificativo del gruppo di prodotti e dovrà essere poi indicato
  anche nel JSON-LD dei prodotti figlio per specificare esattamente a
  che "gruppo prodotti" appartengono e, in sostanza dunque, da quale
  articolo padre derivano

- le proprietà *name, url, description ...* definite a livello di
  "ProductGroup" fanno riferimento all'articolo padre di struttura

- la sezione *offers* definita a livello di "*ProductGroup*" fa
  riferimento all'articolo padre. La proprietà *availability* gestita al
  suo interno verrà impostata:

  - sul valore "*https://schema.org/InStock"* nel momento in cui almeno
    uno dei prodotti figlio dovesse risultare effettivamente disponibile
    e quindi acquistabile

  - sul valore "*https://schema.org/OutOfStock"* nel momento in cui
    nessuno dei prodotti figlio dovesse essere disponibile

- ***\"hasVariant\"*** è un array di oggetti prodotto (*\"@type\":
  \"Product\"*) che contiene i riferimenti (nome, codice, url scheda
  prodotto, colore/taglia) di tutte la varianti colore/taglie derivanti
  dall'articolo padre e serve quindi per indicare ai motori di ricerca i
  riferimenti di tutti i prodotti acquistabili che fanno parte dello
  stesso gruppo.

> All'interno dell'array *"hasVariant"* **verranno inseriti i dati dei
> soli articoli figlio effettivamente esportati e gestiti all'interno
> del sito e che, come tali, avranno anche uno specifico url di pagina
> prodotto**.
>
> Considerando che, nelle condizioni in esame, una delle due
> informazioni colore o taglia è gestita in struttura e l'altra nella
> Tabella Taglie/Colori di Mexal, il fatto di avere all'interno di ogni
> oggetto "*Product*" di "*hasVariant*" la proprietà "*color*" o la
> proprietà "*size*", dipenderà da come è stato marcato il livello della
> struttura che gestisce questo tipo di informazione e, più nello
> specifico dunque, da come è stato impostato il parametro "**Tipologia
> Livello**" presente nella maschera di configurazione del relativo
> Campo di Struttura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_struttura_tipologia_livello.bmp](./assets/media/image8.png)

> Nell'esempio in questione, come precedentemente evidenziato, il colore
> è gestito come ultimo livello della struttura mentre le taglie sono
> gestite con la relativa tabella del gestionale.
>
> In conseguenza di ciò, e supponendo di aver marcato il relativo
> livello della struttura come "livello colore", per ciascuno dei figli
> indicati all'interno di "*hasVariant*" verrà inserita la proprietà
> "*color*" utilizzando come valore quanto indicato all'interno del
> campo "**Titolo**" presente nella maschera di configurazione del
> relativo "elemento colore"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\elemento_colore_titolo.bmp](./assets/media/image9.png)

> Il dettaglio delle taglie (quindi la proprietà "size") verrà invece
> inserito nel Json-ld della pagina prodotto dello specifico articolo
> figlio.
>
> Infine considerando che i prodotti indicati nell'array *"hasVariant"*
> non sono quelli effettivamente presenti nella pagina in cui è stato
> inserito questo JSON-LD (che ricordiamo essere quella dell'articolo
> padre di struttura) nei singoli Schema Product può tranquillamente
> essere omesso l'oggetto *"offers"* e tutto ciò che contiene (compresa
> la proprietà *"availability"*). Queste informazioni saranno infatti
> riportate nella specifica pagina del prodotto figlio.

**[JSON-LD PER ARTICOLI FIGLO]{.underline}**

Nelle condizioni in esame, come detto, ogni articolo figlio
rappresenterà un articolo effettivamente acquistabile, avrà il suo
codice, il suo url di pagina prodotto, il suo colore, il suo prezzo e N
possibili taglie definite all'interno della corrispondente tabella
gestionale.

In definitiva dunque ci troviamo, sostanzialmente, nelle stesse
condizioni della situazione già analizzata nel precedente capitolo di
questo manuale, con l'unica differenza di dover in qualche modo indicare
al motore di ricerca che il prodotto in esame deriva da uno specifico
articolo padre e che fa parte quindi di un ben determinato gruppo di
prodotti.

In conseguenza di ciò il JSON-LD inserito nella pagina prodotto degli
articoli figlio sarà del tipo di quello di seguito indicato:

*\<script type=\"application/ld+json\"\>*

*{*

*\"@context\": \"https://schema.org/\",*

***\"@type\": \"Product\",***

*\"name\": \"Felpa Uomo Blu\",*

*\"sku\": \"FELPAUOMO01-BLU\",*

*\"description\": \"Felpa uomo in cotone blu con cappuccio, disponibile
nelle taglie S, M, L.\",*

*\"image\": \[*

*\"https://www.miosito.it/images/felpa-uomo-blu-1.jpg\",*

*\"https://www.miosito.it/images/fepa-uomo-blu-2.jpg\",*

*\"https://www.miosito.it/images/felpa-uomo-blu-3.jpg\"*

*\],*

*\"offers\": {*

*\"@type\": \"Offer\",*

*\"price\": \"59.90\",*

*\"priceCurrency\": \"EUR\",*

*\"url\": \"https://www.sito.it/felpa-uomo-blu\",*

*\"availability\": \"https://schema.org/InStock\",*

*\"seller\": {*

*\"@type\": \"Organization\",*

*\"name\": \"SportTech Store\"*

*}*

*},*

***\"isVariantOf\": {***

***\"@type\": \"ProductGroup\",***

***\"productGroupID\": \"FELPAUOMO01\",***

***\"name\": \"Felpa Uomo con Cappuccio\"***

***},***

***\"size\": \[\"S\", \"M\", \"L\"\],***

***"color":"Blu",***

*\"aggregateRating\":{*

*\"@type\": \"AggregateRating\",*

*\"ratingValue\": \"4.7\",*

*\"reviewCount\": \"68\"*

*},*

*\"review\": \[*

*{*

*\"@type\": \"Review\",*

*\"author\": {*

*\"@type\": \"Person\",*

*\"name\": \"Marco Rossi\"*

*},*

*\"datePublished\": \"2025-09-15\",*

*\"reviewBody\": \"Leggerissime e davvero comodo!\"*

*},*

*{*

*\"@type\": \"Review\",*

*\"author\": {*

*\"@type\": \"Person\",*

*\"name\": \"Laura Bianchi\"*

*},*

*\"datePublished\": \"2025-09-28\",*

*\"reviewBody\": \"Ottimo comfort e materiali di qualità. Spedizione
veloce.\"*

*}*

*\]*

*}*

*\</script\>*

dove:

- ***\"@type\": \"Product\"*** indica al motore di ricerca che si sta
  parlando di un prodotto effettivamente acquistabile (e che richiederà
  quindi obbligatoriamente la proprietà *"offers"*)

- ***\"isVariantOf\"*** è l'oggetto utilizzato per indicare ai motori di
  ricerca che il prodotto in esame fa parte di un ben determinato gruppo
  di prodotti e le sue proprietà *"**name**"* e " ***productGroupID***"
  verranno quindi valorizzate con i relativi dati (titolo e codice) del
  corrispondente padre di struttura

- ***\"size\": \[\"S\", \"M\", \"L\"\]*** In questo esempio, le taglie
  sono gestite con la Tabella Taglie/Colori di Mexal per cui la
  proprietà *size* verrà gestita esattamente secondo quanto già indicato
  nel precedente capitolo di questo manuale.

> Anche questa volta dunque all'interno di questo array verranno
> inserite le sole taglie disponibili piuttosto che tutte le taglie
> gestite a seconda della particolare tipologia di gestione ("**Acquista
> Sempre**" o "**Acquista solo se disponibile**") effettivamente attiva
> per l'articolo in esame e a seconda anche del fatto di aver attivato o
> meno il parametro "**Mostra solo le taglie disponibili**" presente
> nella maschera di configurazione della serie cui appartiene l'articolo
> stesso.

- ***"color"**:**"Blu"*** In questo esempio il colore è gestito come
  ultimo elemento della struttura. Supponendo dunque di aver marcato
  correttamente questo livello come "livello colore", all'interno del
  Json-ld verrà inserita anche la proprietà "*color*" utilizzando come
  valore quanto indicato all'interno del campo "**Titolo**" presente
  nella maschera di configurazione del relativo "elemento colore".

