# ESEMPIO -- PROPRIETA' SEMPLICE



Supponiamo di dover indicare esplicitamente ai motori di ricerca
piuttosto che ad un sistema di AI o ad un qualsiasi altro sistema
automatico che analizza le pagine del sito, il materiale con cui sono
realizzati i prodotti in vendita sul nostro Ecommerce.

Questo tipo di informazione non può essere inserita nel JSON-LD prodotto
in automatico da Passweb attivando semplicemente uno dei check presenti
in corrispondenza del parametro "**Proprietà gestite**", per cui dovremo
necessariamente andare ad integrare quanto già prodotto da Passweb
utilizzando il Json Builder esaminato nel precedente capitolo di questo
manuale.

In questo senso la prima cosa da fare sarà quella di analizzare il
vocabolario di Schema.org per vedere quale possa essere effettivamente
la proprietà da utilizzare per inserire questo tipo di informazione
all'interno del JSON-LD e con che tipo di struttura dati dovremo poi
gestirla.

Analizzando le proprietà riportate al seguente url
<https://schema.org/Product> potremo verificare, in maniera abbastanza
semplice, che la proprietà che fa al caso nostro è "**material**" e che
tale proprietà può avere dei semplici valori testuali utilizzati appunto
per indicare il materiale di cui è fatto un determinato prodotto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_esempio_1.bmp](./assets/media/image27.png)

In sostanza dovremo quindi andare ad integrare il JSON-LD prodotto da
Passweb con un'informazione del tipo:

*"material":"cotone"*

dove ovviamente il tipo di materiale (es. "cotone") non essendo lo
stesso per tutti i prodotti in vendita sul sito, e non essendo neppure
uno dei campi dell'anagrafica articoli standard del gestionale, dovrà
necessariamente essere prelevato, articolo per articolo, da un apposito
attributo.

Supponendo dunque di avere effettivamente a disposizione un Attributo
Passweb chiamato "Materiale" valorizzato in maniera corretta per tutti
gli articoli gestiti sul sito, per inserire questa informazione
all'interno del JSON-LD dovremo utilizzare il Json Builder creando una
**proprietà semplice** (del tipo "chiave":"valore") analoga a quella di
seguito indicata:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_esempio_2.bmp](./assets/media/image28.png)

- Nome proprietà 🡪 **material**

- Struttura dati 🡪 **Valore Semplice**

- Tipologia di campo con cui mappare la proprietà 🡪 **Attributo**

- Attributo Passweb da cui prelevare il valore 🡪 **Materiale**

In questo modo, una volta salvate le impostazioni e avviata la procedura
di rigenerazione dei dati (pulsante .....) il JSON-LD di un prodotto con
l'Attributo Passweb "Materiale" impostato su "Cotone" sarà analogo a
quello qui di seguito indicato

> *\<script type=\"application/ld+json\"\>*
>
> *{*
>
> *\"@context\": \"https://schema.org/\",*
>
> *\"@type\": \"Product\",*
>
> *\"name\": \"T-Shirt con logo Nike\",*
>
> *\"description\": \"Maglietta a maniche corte con logo Nike su
> schiena\",*
>
> *\"sku\": \"TSN125A\",*
>
> *\"image\": \[*
>
> *\"https://www.miosito.it/media/products/tshirtnike-front.jpg\",*
>
> *\"https://www.miosito.it/media/products/ tshirtnike-back.jpg \",*
>
> *\],*
>
> *\"offers\": {*
>
> *\"@type\": \"Offer\",*
>
> *\"url\": \"https://www.miosito.it/prodotto/TShirt-logo-Nike \",*
>
> *\"priceCurrency\": \"EUR\",*
>
> *\"price\": \"68.90\",*
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
> *\"reviewCount\": \"138\"*
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
> *\"reviewBody\": \"Maglia leggera bella e comoda per i runner\",*
>
> *}*
>
> *\],*
>
> ***\"material\": \"Cotone\"***
>
> *}*
>
> *\</script\>*

