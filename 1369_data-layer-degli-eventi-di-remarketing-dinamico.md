# DATA LAYER DEGLI EVENTI DI REMARKETING DINAMICO



Una volta abilitato il parametro "**Attiva Remarketing Dinamico**", come
indicato nel precedente capitolo di questo manuale, il data layer
gestito da Passweb in relazione agli eventi di:

- **view_item_list**

- **view_item**

- **add_to_cart**

- **purchase**

avrà una struttura del tipo di quella di seguito indicata

*{*

*"event": "view_item_list",*

*"ecommerce": {*

*"event_category": "Ecommerce Avanzato",*

*"event_action": "Impression Product",*

*"event_label": "Vista Catalogo",*

*"dateTime": "12/02/2025, 14:47:09",*

*"currency": "EUR",*

*"value": 1,*

*2items": \[*

*{*

*"item_id": "ACAB03",*

*"item_name": "Slvr Basi Cap",*

*"currency": "EUR",*

*"discount": 11.5,*

*"index": 1,*

*"item_brand": "POLIESTERE",*

*"item_category": "UOMO",*

*"item_category2": \"ACCESSORI\",*

*"item_category3": \"BERRETTI\",*

*"item_list_name\": \"Catalogo\",*

*"price": 21.1,*

*"quantity": 1*

*},*

*....*

*\]*

*},*

*"user_id": "552",*

*"user_data": {*

*"sha256_email_address":
\"bef0252b248286ca858a3e99d977f3bec4341d7c8702ff4c0274c0e3c9ba2a31\",*

*"sha256_phone_number":
\"6872056c3d1d4453f79cdf0d7a6678efd04d82d19de9bac8773460dd8556a0de\",*

*"address": {*

*"sha256_last_name2:
\"832a7b7c8f70716f98bc9dc0f8c9891b7de9b0563b68ebb5de380a2af01197c3\",*

*"street": \"Via dei Mille\",*

*"city": \"Rimini\",*

*"postal_code": \"47892\",*

*"country": "IT"*

*}*

*},*

***"remarketing_ads": {***

***"value": 837.26,***

***"items": \[***

***{***

***"id": "ACAB03",***

***"google_business_vertical": "retail"***

***},***

***...***

***{***

***"id": "ACAB05",***

***"google_business_vertical": "retail"***

***},***

***\]***

***},***

***}***

Sostanzialmente dunque, all'interno di questo data layer potremmo
trovare tre distinti oggetti:

- l'oggetto '**ecommerce'** sempre presente e necessario per poter
  implementare correttamente in tracciamento verso GA4

- l'oggetto '**user_data**' presente solo nel momento in cui si sia
  deciso di attivare il parametro "Raccolta Dati Utente nel Data Layer"
  e utile per gestire la raccolta degli User Provided Data e le
  conversioni Avanzate

- l'oggetto '**remarketing_ads**'

Quest'ultimo, in particolare, è quello aggiunto a seguito
dell'attivazione del parametro "**Attiva Remarketing Dinamico**" e
contiene quindi tutti i dati necessari per una corretta configurazione,
su GTM, del relativo Tag di Remarketing.

Nello specifico il parametro:

- **value:** rappresenta la somma dei prezzi ivati dei prodotti
  coinvolti nell'evento

- **items:** è l'array dei prodotti coinvolti nell'evento (ovviamente
  per gli eventi di add_to_cart e view_item si avrà un array di un solo
  elemento)

- **id:** codice del prodotto coinvolto nell'evento

- **google_buinsess_vertical**: valorizzato sempre con la stringa
  '**retail'**.

> Come evidenziato nei precedenti capitoli, questo parametro è quello
> utilizzato per fornire a Google l'indicazione relativa a dove andare a
> reperire le informazioni (titolo, prezzo, descrizione, sconto ...) dei
> prodotti che verranno poi inseriti nei vari annunci pubblicitari. La
> stringa 'retail', nello specifico, indica a Google di cercare queste
> informazioni all'interno del Merchant Center utilizzando come chiave
> di ricerca il valore del corrispondente parametro id

