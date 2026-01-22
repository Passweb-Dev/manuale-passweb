# INFORMAZIONI DI SPEDIZIONE -- ADD_SHIPPING_INFO



**Nome Evento**: add_shipping_info

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Checkout**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato
selezionando, in fase di checkout, un determinato metodo di spedizione

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', '**add_shipping_info',*

*{*

*event_label: 'Add Shipping Info Bartolini',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*shipping_tier: 'Bartolini',*

*payment: 10,*

*coupon: 'eventuale codice del coupon applicato',*

*coupon_value: 'eventuale importo del coupon',*

*promozione_name: 'eventuale nome della promo applicata',*

*promozione_value: 'eventuale importo della promo applicata',*

*value: 517.69,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: "Prod01A",*

*item_name: "Magic Mouse",*

*currency: "EUR",*

*discount: 11.17,*

*index: 1,*

*item_brand: "Apple",*

*item_category: "Apple",*

*item_category2: "Accessori",*

*item_category3: "Informatica",*

*item_variant: 'eventuale variante del prodotto',*

*price: 100.54,*

*quantity: 5*

*}*

*....*

*{*

*...parametri articolo N...*

*}*

*\]*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_label:** Add Shipping Info + Descrizione del metodo di
  spedizione selezionato

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in ordine)

- **tax**: totale iva documento

- **totale_documento**: totale documento ivato

- **totale_merce**: totale merce

- **shipping:** eventuale importo delle spese di spedizione

- **shipping_tier:** descrizione del metodo di spedizione selezionato

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **value:** 1 (valore di Default), totale merce ivato oppure il valore
  personalizzato impostato per il parametro "**GA4 --
  add_shipping_info**" presente alla pagina "***Sito Preferenze***" del
  Wizard, tab "***Tracciamento Dati***" sezione "***Parametro Value
  eventi Analytics e Tag Manager***". Per maggiori informazioni in
  merito si veda anche quanto indicato all'interno del relativo capitolo
  di questo manuale ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in ordine

Per maggiori informazioni relativamente ai parametri gestiti per ogni
singolo prodotto presente nell'array items si veda quanto indicato nel
corrispondente capitolo (*"Google Analytics 4 -- Monitoraggio Ecommerce
-- Array items"*) di questo manuale

