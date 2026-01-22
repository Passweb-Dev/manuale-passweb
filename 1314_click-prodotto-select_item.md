# CLICK PRODOTTO -- SELECT_ITEM



**Nome Evento**: select_item

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Articolo**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato nel
momento in cui un utente del sito dovesse cliccare su di un campo di una
cella articolo presente all'interno di componenti quali il "Catalogo
Ecommerce", "Offerte / Novità", "Abbinati Ecommerce", "Popolarità
Prodotto" ... per visualizzare il dettaglio del relativo prodotto

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'select_item',*

*{*

*event_label: 'Click Product Magic Mouse',*

*content_type: 'product',*

*currency: 'EUR',*

*value: 1,*

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

*quantity: 1*

*}*

*\]*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_label:** Click Product + Titolo del prodotto clicclato

- **content_type**: product

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **value:** 1 (valore di Default) oppure il prezzo ivato del relativo
  articolo o ancora il valore personalizzato impostato per il parametro
  "**GA4 --** **select_item**" presente alla pagina "***Sito
  Preferenze***" del Wizard, tab "***Tracciamento Dati***" sezione
  "***Parametro Value eventi Analytics e Tag Manager***".

> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del relativo capitolo di questo manuale ("*Sito --
> Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco

Per maggiori informazioni relativamente ai parametri gestiti per ogni
singolo prodotto presente nell'array items si veda quanto indicato nel
corrispondente capitolo (*"Google Analytics 4 -- Monitoraggio Ecommerce
-- Array items"*) di questo manuale

**ATTENZIONE!** Per ovvie ragioni nell'evento in esame l'array items
conterrà un solo prodotto

