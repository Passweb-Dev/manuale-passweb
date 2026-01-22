# ACQUISTO -- PURCHASE



**Nome Evento**: purchase

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Checkout**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà concluso un ordine

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'purchase',*

*{*

*event_label: 'Acquisto confermato + id_transazione Passweb',*

*transaction_id: 1658,*

*affiliation: 'Store Clobis',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*payment: 10,*

*shipping_tier: 'Bartolini',*

*payment_type: 'PayPal',*

*coupon: 'Promo 2022',*

*coupon_value: '-15.10,*

*promozione_name: 'Promo Telefoni',*

*promozione_value: '-105.10,*

*value: 517.69,*

*gift_card: 'False',*

*punti_premio: 'True',*

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

- **event_label:** Acquisto confermato

- **transaction_id:** id della transazione Passweb

> **ATTENZIONE!** l'id della transazione (essendo ricollegabile allo
> specifico utente) può essere considerato come un dato di
> identificazione personale. In conseguenza di ciò nel momento in cui
> tale informazione dovesse essere inviata ad Analytics è necessario
> accertarsi di aver gestito in maniera corretta le richieste preventive
> di consenso e di aver inserito tutto il necessario nelle varie
> informative privacy presenti sul sito

- **affiliation:** valore del parametro "**Nome Sito**" (pagina "Sito --
  Preferenze" del Wizard, tab "SEO")

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

- **payment_type:** descrizione del pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **gift_card:** "True / False" a seconda del fatto che per il pagamento
  dell'ordine sia stato utilizzato o meno il credito presente in una
  Gift Card

- **punti_premio:** "True / False" a seconda del fatto che per il
  pagamento dell'ordine siano stati utilizzati o meno dei punti premio

- **dateTime:** data e ora in cui si è verificato l'evento

- **value:** totale documento (valore di Default) oppure il valore
  personalizzato impostato per il parametro "**GA4 -- purchase**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro Value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **items:** array dei prodotti presenti in elenco

Per maggiori informazioni relativamente ai parametri gestiti per ogni
singolo prodotto presente nell'array items si veda quanto indicato nel
corrispondente capitolo (*"Google Analytics 4 -- Monitoraggio Ecommerce
-- Array items"*) di questo manuale

