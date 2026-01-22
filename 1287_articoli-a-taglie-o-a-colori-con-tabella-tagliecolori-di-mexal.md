# ARTICOLI A TAGLIE O A COLORI CON TABELLA TAGLIE/COLORI DI MEXAL



In questo scenario per Passweb (così come per Mexal) ogni variante di
Taglia o di Colore di fatto è sempre lo stesso prodotto. Al variare
della Taglia o del Colore infatti non varia né il codice dell'articolo
né tanto meno il suo prezzo o l'url della sua pagina prodotto.

In conseguenza di ciò il JSON-LD inserito da Passweb all'interno delle
corrispondenti schede prodotto sarà del tutto analogo a quello dei
"prodotti semplici" con l'unica differenza rappresentata dall'utilizzo
di un'ulteriore proprietà **(*"color"*** o ***"size"***) utilizzata
(come previsto dal vocabolario di Schema.org) per indicare in maniera
esplicita ai motori di ricerca quelle che possono essere tutte le
possibili taglie o tutti i possibili colori di quello stesso articolo.

*\<script type=\"application/ld+json\"\>*

*{*

*\"@context\": \"https://schema.org\",*

*\"@type\": \"Product\",*

*\"name\": \"Scarpe Running AirSpeed X\",*

*\"description\": \"Scarpe da corsa leggere e traspiranti, disponibili
in vari colori.\",*

*\"image\": \[*

*\"https://www.miosito.it/images/scarpe-airspeed-x-nero.jpg\",*

*\"https://www.miosito.it/images/scarpe-airspeed-x-rosso.jpg\",*

*\"https://www.miosito.it/images/scarpe-airspeed-x-blu.jpg\"*

*\],*

***\"color\": \[\"Nero\", \"Rosso\", \"Blu\"\],***

*\"sku\": \"ASX-001\",*

*\"offers\":{*

*\"@type\": \"Offer\",*

*\"url\": \"https://www.miosito.it/scarpe-running-airspeed-x\",*

*\"priceCurrency\": \"EUR\",*

*\"price\": \"129.90\",*

*\"availability\": "https://schema.org/InStock",*

*\"seller\": {*

*\"@type\": \"Organization\",*

*\"name\": \"SportTech Store\"*

*}*

*},*

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

*\"reviewBody\": \"Scarpe leggerissime e davvero comode. Ideali per
correre su strada!\"*

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

In questa struttura l'utilizzo della proprietà ***"color"*** o
***"size"*** dipende da come è stata marcata, in Passweb, la specifica
serie di Taglie/Colori cui risulta associato il singolo prodotto.

In particolare nel caso in cui il parametro "**Tipologia Serie**"

![](./assets/media/image6.png)

presente nella maschera di configurazione della Serie di Taglie / Colori
cui appartiene l'articolo in esame dovesse essere impostato sull'opzione

- **Taglie**: nel JSON-LD verrà inserita la proprietà ***"size"**,*
  gestita come un array di stringhe e valorizzata con tutte le possibili
  Taglie definite per questa stessa serie

- **Colore:** nel JSON-LD verrà inserita la proprietà ***"color"***,
  gestita come un array di stringhe e valorizzata con tutti i possibili
  colori definiti per quella stessa serie

**ATTENZIONE!** i valori delle Taglie / Colori inseriti all'interno
degli array *"size" / "color"* saranno quelli definiti, per i singoli
elementi della serie, in corrispondenza del campo "**Testo**" presente
all'interno della maschera "**Modifica Elementi della Serie**"

![](./assets/media/image7.png)

In questo senso poi è bene sottolineare anche che, al fine di soddisfare
la condizione obbligatoria secondo cui **quanto indicato all'interno del
Json-ld deve sempre e comunque riflettere quanto effettivamente
visualizzato anche nella pagina web**, nell'array *"size" / "color"*
verranno inserite le sole taglie / colori disponibili piuttosto che
tutte le taglie / colori gestiti a seconda della particolare modalità di
gestione ("**Acquista Sempre**" o "**Acquista solo se disponibile**")
attiva per l'articolo in esame e dipendentemente anche dal fatto di aver
attivato o meno il parametro "**Mostra solo le taglie disponibili**",
presente nella maschera di configurazione della serie di appartenenza
dell'articolo stesso.

Infine, un altro aspetto importante da sottolineare relativamente alle
informazioni inserite nel JSON-LD di questa particolare tipologia di
prodotti è poi quello che riguarda il valore della proprietà
***"availability"*** (utilizzata, come detto, per indicare ai motori di
ricerca se il prodotto in esame è o meno disponibile)

In questo caso infatti, sebbene lato gestionale si possano avere
disponibilità specifiche per le singole Taglie/Colori, lato web abbiamo
pur sempre a che fare con un singolo prodotto che dovrà quindi avere una
singola disponibilità.

In conseguenza di ciò la proprietà "*availability*" verrà valorizzata
con l'opzione:

- ***https://schema.org/InStock*** se almeno una delle Taglie / Colori
  dell'articolo in esame dovesse essere disponibile

- ***https://schema.org/OutOfStock*** se tutte le Taglie / Colori
  dell'articolo in esame dovessero risultare non disponibili

