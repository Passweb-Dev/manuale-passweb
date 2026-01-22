# ESEMPIO -- PROPRIETA' STRUTTURATA (OGGETTO)



Supponiamo, questa volta, di dover indicare esplicitamente ai motori di
ricerca piuttosto che ad un sistema di AI o ad un qualsiasi altro
sistema automatico che analizza le pagine del sito, la marca dei
prodotti in vendita sul nostro Ecommerce.

Come nel caso precedente anche questa volta la prima cosa da fare sarà
sempre quella di analizzare il vocabolario di Schema.org per vedere
quale possa essere la specifica proprietà da utilizzare per codificare
l'informazione che ci interessa.

Nel caso in esame la proprietà che fa al caso nostro sarà "**brand**"

![](./assets/media/image29.png)

i cui valori però, a differenza dell'esempio precedente, non possono
essere delle semplici stringhe ma devono essere necessariamente degli
oggetti di tipo "**Brand**".

Cliccando sul link indicato in figura verremo ricondotti alla sezione di
Schema.org (<https://schema.org/Brand>) in cui sono indicate tutte le
possibili proprietà dell'oggetto Brand e, di conseguenza anche quella
che dovrà essere la struttura dati da inserire all'interno del JSON-LD
per gestire questo tipo di informazione.

Supponendo che la nostra esigenza sia semplicemente quella di indicare
il nome della marca, la proprietà dell'oggetto Brand da utilizzare dovrà
essere *"name"* (che accetta solo valori testuali) e la struttura dati
da inserire all'interno del JSON-LD dovrà quindi essere del tipo di
quella di seguito indicata:

*\"brand\": {*

*\"@type\": \"Brand\",*

*\"name\": \"Nike\"*

*}*

dove:

- brand 🡪 è il nome della proprietà (gestita come Oggetto) da utilizzare
  per gestire l'informazione relativa alla marca

- \"@type\": \"Brand\" 🡪 è una proprietà di "brand" utilizzare per
  indicare la tipologia di oggetto necessario per gestire questo tipo di
  informazione

- name 🡪 è una proprietà di "brand" utilizzata per indicare il nome
  della marca

Posto quindi di avere a disposizione un Attributo Passweb utilizzato per
gestire la marca dei vari prodotti (es. "Marca") per ricreare la
struttura dati richiesta da Schema.org per gestire la marca dei
prodotti, dovremo impostare il Json Builder come nella figura di seguito
riportata

![](./assets/media/image30.png)

In questo modo, una volta salvate le impostazioni e avviata la procedura
di rigenerazione dei dati (pulsante .....) il JSON-LD di un prodotto con
l'Attributo Passweb "Marca" impostato su "Nike" potrebbe essere analogo
a quello qui di seguito indicato

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
> ***\"brand\": {***
>
> ***"type":"Brand",***
>
> ***\"name\": \"Nike\"***
>
> ***}***
>
> *}*
>
> *\</script\>*

