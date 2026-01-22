# RIMOZIONE DAL CARRELLO -- RemoveFromCart



**Nome Evento**: RemoveFromCart

**Tipologia Evento:** custom

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà attivato ogni
volta in cui verrà rimosso un articolo dal carrello

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'trackCustom\', RemoveFromCart,*

*{*

*content_ids: 'Prod01A',*

*content_name: 'Magic Mouse',*

*content_category: 'Informatica/Accessori',*

*content_type: 'product',*

*contents: \[{*

*id: 'Prod01A',*

*quantity: 5*

*}\],*

*currency: 'EUR',*

*value: 3,*

*dateTime: '11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: RemoveFromCart-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_ids:** codice del prodotto rimosso dal carrello

- **content_name:** titolo del prodotto rimosso dal carrello

- **content_category**: percorso della categoria merceologica di
  appartenenza dell'articolo rimosso dal carrello

- **content_type**: product

- **contents**: codice (id) e quantità (quantity) del prodotto rimosso
  dal carrello

- **currency:** codice ISO della valuta in uso al prodotto rimosso dal
  carrello

- **value:** quantità (negativa) rimossa dal carrello (valore di
  Default) oppure il valore personalizzato impostato per il parametro
  "**remove_from_cart**" presente alla pagina "***Sito Preferenze***"
  del Wizard, tab "***Tracciamento Dati***" sezione "***Parametro Value
  eventi Analytics, Tag Manager e Facebook Pixel***".

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
> *RemoveFromCart-20221110145456-779*")

**ATTENZIONE!** nell'evento in esame i parametri che prevedono la
presenza di un array di prodotti conterranno sempre un solo articolo,
quello effettivamente interessato dall'evento in questione

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

