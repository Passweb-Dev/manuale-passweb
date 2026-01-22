# SELEZIONE PRODOTTO -- SelectItem



**Nome Evento**: SelectItem

**Tipologia Evento:** custom

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà attivato nel
momento in cui un utente del sito dovesse cliccare su di un campo di una
cella articolo presente all'interno di componenti quali il "Catalogo
Ecommerce", "Offerte / Novità", "Abbinati Ecommerce", "Popolarità
Prodotto" ... per visualizzare il dettaglio del relativo prodotto

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'trackCustom\', SelectItem,*

*{*

*content_ids: 'Prod01A',*

*content_name: 'Magic Mouse',*

*content_category: 'Informatica/Accessori',*

*content_type: 'product',*

*contents: \[{*

*id: 'Prod01A',*

*quantity: 1*

*}\],*

*currency: 'EUR',*

*value: 3,*

*dateTime: '11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: SelectItem-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_ids:** codice del prodotto selezionato

- **content_name:** titolo del prodotto selezionato

- **content_category**: percorso della categoria merceologica di
  appartenenza dell'articolo selezionato

- **content_type**: product

- **contents**: codice (id) e quantità unitaria (quantity=1) del
  prodotto selezionato

- **currency:** codice ISO della valuta in uso al prodotto selezionato

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**select_item**" presente alla pagina
  "***Sito Preferenze***" del Wizard, prezzo di vendita dell'articolo
  (valore di Default) oppure il valore personalizzato impostato per il
  parametro "**view_item**" tab "***Tracciamento Dati***" sezione
  "***Parametro Value eventi Analytics, Tag Manager e Facebook
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
> *SelectItem-20221110145456-779*")

**ATTENZIONE!** nell'evento in esame i parametri che prevedono la
presenza di un array di prodotti conterranno sempre un solo articolo,
quello effettivamente interessato dall'evento in questione

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

