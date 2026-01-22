# IMPRESSIONE PRODOTTI -- VIEW_ITEM_LIST



**Nome Evento**: view_item_list

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Articolo**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà generato ed inviato
ad Analytics ogni volta in cui viene visualizzata una pagina del sito in
cui è presente almeno un elenco di prodotti ovvero una pagina del sito
in cui è presente un componente come il "Catalogo Ecommerce", "Offerte /
Novità", "Abbinati Ecommerce", "Popolarità Prodotto" ...

**ATTENZIONE!** nel momento in cui in una pagina del sito dovessero
essere presenti, ad esempio, due diversi elenchi di prodotti (es. un
"Offerte / Novità" e un "Popolarità Prodotto") verranno generati ed
inviati ad Analytics due distinti eventi view_item_list (ciascuno con i
relativi parametri determinati dai prodotti in esso contenuti)

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'view_item_list',*

*{*

*event_label:'Vista Prodotti in Offerta' ,*

*currency:'EUR',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: "Prod01A",*

*item_name: "Magic Mouse",*

*currency: "EUR",*

*discount: 2.22,*

*index: 0,*

*item_brand: "Apple",*

*item_category: "Apple",*

*item_category2: "Accessori",*

*item_category3: "Informatica",*

*item_list_name: "**Prodotti in Offerta",*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 1*

*},*

*....*

*{*

*...parametri articolo N...*

*}*

*\]*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_label:** Vista + Nome assegnato in Passweb al componente che
  individua l'elenco di prodotti

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**GA4 -- view_item_list**" presente alla
  pagina "***Sito Preferenze***" del Wizard, tab "***Tracciamento
  Dati***" sezione "***Parametro Value eventi Analytics e Tag
  Manager***". Per maggiori informazioni in merito si veda anche quanto
  indicato all'interno del relativo capitolo di questo manuale ("*Sito
  -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per maggiori informazioni relativamente ai parametri gestiti per ogni
singolo prodotto presente nell'array items si veda quanto indicato nel
corrispondente capitolo (*"Google Analytics 4 -- Monitoraggio Ecommerce
-- Array items"*) di questo manuale

