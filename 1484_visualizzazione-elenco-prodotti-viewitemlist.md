# VISUALIZZAZIONE ELENCO PRODOTTI -- ViewItemList



**Nome Evento**: ViewItemList

**Tipologia Evento:** custom

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà generato ed
inviato a Facebook ogni volta in cui viene visualizzata una pagina del
sito in cui è presente almeno un elenco di prodotti ovvero una pagina
del sito in cui è presente un componente come il "Catalogo Ecommerce",
"Offerte / Novità", "Abbinati Ecommerce", "Popolarità Prodotto" ...

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'trackCustom\', ViewItemList,*

*{*

*content_ids: 'Prod01A,Prod02B',*

*content_name: 'Vista Offerte Novità',*

*content_category: 'ViewItemList',*

*content_type: 'product',*

*contents: \[{*

*id: 'Prod01A',*

*quantity: 1*

*},*

*{*

*id: 'Prod02B',*

*quantity: 1*

*}*

*\],*

*currency: 'EUR',*

*value: 1,*

*dateTime: '11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: ViewItemList-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_ids:** lista dei codici dei prodotti in elenco

- **content_name:** Vista + Nome assegnato in Passweb al componente che
  individua l'elenco di prodotti

- **content_category**: ViewItemList

- **content_type**: product

- **contents**: lista dei codici (id) e quantità unitaria (quantity=1)
  dei prodotti in elenco

- **currency:** codice ISO della valuta in uso ai prodotti in elenco

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**view_item_list**" presente alla pagina
  "***Sito Preferenze***" del Wizard, tab "***Tracciamento Dati***"
  sezione "***Parametro Value eventi Analytics, Tag Manager e Facebook
  Pixel***".

> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del relativo capitolo di questo manuale ("*Sito --
> Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **eventID / event_id:** nel tracciamento lato client verrà utilizzato
  il parametro 'eventID'; nel tracciamento lato server verrà invece
  utilizzato il parametro 'event_id'.

> In entrambi i casi, per garantire la deduplica dell'evento secondo
> quanto richiesto da facebook, il parametro in esame verrà valorizzato
> con un identificativo univoco costituito dal nome dell'evento da
> tracciare più un timestamp di ora, minuti e secondi in cui si è
> verificato l'evento più un ulteriore codice univoco (es. "
> *ViewItemList-20221110145456-779*")

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

