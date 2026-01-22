# ACQUISIZIONE CONTATTO -- Lead



**Nome Evento**: Lead

**Tipologia Evento:** standard

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà attivato ogni
volta in cui verrà compilato un form del sito

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'track\', Lead,*

*{*

*content_category: 'Lead',*

*content_name: 'form_contatti',*

*status: true*

*dateTime: '11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: Lead-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_category**: Lead

- **content_name**: Form + nome assegnato in passweb al componente form

- **status**: true

- **dateTime:** data e ora in cui si è verificato l'evento

- **eventID / event_id:** nel tracciamento lato client verrà utilizzato
  il parametro 'eventID'; nel tracciamento lato server verrà invece
  utilizzato il parametro 'event_id'.

> In entrambi i casi, per garantire la deduplica dell'evento secondo
> quanto richiesto da facebook, il parametro in esame verrà valorizzato
> con un identificativo univoco costituito dal nome dell'evento da
> tracciare più un timestamp di ora, minuti e secondi in cui si è
> verificato l'evento più un ulteriore codice univoco (es. "
> *Lead-20221110145456-779*")

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

