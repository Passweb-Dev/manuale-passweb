# AGGIUNTA IN CARRELLO -- ADD_TO_CART



**Nome Evento**: add_to_cart

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Carrello e Wishlist**" presente alla pagina
"**Sito -- Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà aggiunto un articolo in carrello

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'add_to_cart',*

*{*

*event_label: 'Add to Cart Magic Mouse',*

*currency: 'EUR',*

*value: 3,*

*discount_pwb: 2.22,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: "Prod01A",*

*item_name: "Magic Mouse",*

*currency: "EUR",*

*discount: 2.22,*

*index: 1,*

*item_brand: "Apple",*

*item_category: "Apple",*

*item_category2: "Accessori",*

*item_category3: "Informatica",*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*}*

*\]*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_label:** Add to Cart + Titolo del prodotto aggiunto in
  carrello

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **value:** quantità con cui l'articolo è stato aggiunto in carrello
  (valore di Default), il corrispondente valore monetario (prezzo
  ivato), oppure il valore personalizzato impostato per il parametro
  "**GA4 --add_to_cart**" presente alla pagina "***Sito Preferenze***"
  del Wizard, tab "***Tracciamento Dati***" sezione "***Parametro Value
  eventi Analytics e Tag Manager***".

> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del relativo capitolo di questo manuale ("*Sito --
> Preferenze -- Tracciamento Dati*")

- **discount_pwb**: valore **ivato** dell'eventuale sconto relativo al
  prodotto aggiunto in carrello

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per maggiori informazioni relativamente ai parametri gestiti per ogni
singolo prodotto presente nell'array items si veda quanto indicato nel
corrispondente capitolo (*"Google Analytics 4 -- Monitoraggio Ecommerce
-- Array items"*) di questo manuale

**ATTENZIONE!** Per ovvie ragioni nell'evento in esame l'array items
conterrà un solo prodotto

