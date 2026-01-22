# AGGIUNTA DELLE INFORMAZIONI DI PAGAMENTO -- AddPaymentInfo



**Nome Evento**: AddPaymentInfo

**Tipologia Evento:** standard

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà attivato
selezionando, in fase di checkout, un determinato metodo di pagamento

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'track\', AddPaymentInfo,*

*{*

*content_ids: 'Prod01A,Prod02B',*

*content_name: 'AddPaymentInfo',*

*content_category: 'checkout',*

*content_type: 'product',*

*contents: \[{*

*id: 'Prod01A',*

*quantity: 5*

*},*

*{*

*id: 'Prod02B',*

*quantity: 8*

*}*

*\],*

*currency: 'EUR',*

*value: 3,*

*dateTime: '11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: AddPaymentInfo-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_ids:** lista dei codici dei prodotti in ordine

- **content_name:** AddPaymentInfo

- **content_category**: checkout'

- **content_type**: product

- **contents**: lista dei codici (id) e quantità (quantity) dei prodotti
  in ordine

- **currency:** codice ISO della valuta in uso ai prodotti in ordine

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**add_payment_info**" presente alla pagina
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
> verificato l'evento più un ulteriore codice univoco (es.
> "*AddPaymentInfo-20221110145456-779*")

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

