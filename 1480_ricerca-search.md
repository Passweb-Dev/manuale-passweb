# RICERCA -- Search



**Nome Evento**: Search

**Tipologia Evento:** standard

**Modalità invio**: Server, Client

**Generazione dell' evento**: l'evento in esame verrà attivato ogni
volta in cui verrà effettuata una ricerca sul sito utilizzando, per
questo, i relativi componenti presenti nativamente in ogni sito Passweb

L'attivazione dell'evento in questione determinerà l'invio a facebook
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*fbq(\'track\', Search,*

*{*

*search_category: 'Ricerca ECommerce',*

*content_type: 'product',*

*content_category: Search,*

*campi_ricerca: \[{*

*campo: 'search_titolo,*

*valore: 'MAGIC-mouse'*

*},*

*{*

*campo: 'search_Disponibilita,*

*valore: 1*

*}*

*\],*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56'*

*},*

*{*

*eventID / event_id: Search-20221110145456-779*

*}*

*);*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **content_type**: product

- **search_category:** Ricerca Ecommerce / Ricerca Testuale / Ricerca
  CMS

> **ATTENZIONE!** il parametro search_category assumerà uno dei tre
> valori sopra indicati in base alla tipologia del componente utilizzato
> per effettuare la ricerca sul sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_173.bmp](./assets/media/image35.png){width="4.597222222222222in"
height="3.045138888888889in"}

- **campi_ricerca**: lista dei valori presenti nei campi di ricerca del
  relativo pannello. Per ogni campo valorizzato in fase di ricerca verrà
  inserita la coppia "**chiave -- valore**" dove:

> **chiave = search_Nome_Campo** -- coincide esattamente con quanto
> inserito nella maschera di configurazione del relativo componente di
> ricerca in corrispondenza del campo "Nome Tracciamento" (il tutto
> riportato in minuscolo)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_173_a.bmp](./assets/media/image36.png){width="4.623611111111111in"
height="3.045138888888889in"}

> **ATTENZIONE!** Eventuali spazi presenti all'interno del campo
> evidenziato in figura verranno sostituiti dal carattere \_
>
> Nel momento in cui il campo in esame dovesse essere lasciato vuoto, al
> suo posto verrà utilizzato il nome (tutto in minuscolo) assegnato al
> componente
>
> **valore** = valore inserito nel relativo campo di ricerca -- Il
> valore effettivamente passato a Facebook potrà variare, ovviamente, in
> relazione al tipo di campo utilizzato per la ricerca
>
> Nel momento in cui all'interno del pannello di ricerca dovesse essere
> inserito, ad esempio, un componente di tipo "Filtro Checkbox", il
> valore che esso potrà assumere sarà solamente 1 e questo si potrà
> verificare solo se, in fase di ricerca, il check in esame dovesse
> essere effettivamente selezionato
>
> Supponendo dunque di utilizzare un pannello di ricerca di tipo
> Ecommerce con all'interno:

- un componente "Filtro Testo" con "Nome Tracciamento = Codice"

- un componente "Filtro Checkbox" con "Nome Tracciamento =
  Disponibilità"

- un componente "Filtro TreeView" con "Nome Tracciamento = Categoria
  Merceologica"

> e di effettuare una ricerca con il check relativo al campo
> "Disponibilità" selezionato e con il campo relativo al "Codice"
> valorizzato con la stringa "prod01A", il parametro "campi_ricerca" del
> corrispondente evento "*search*" verrà valorizzato come di seguito
> indicato
>
> *campi_ricerca:\[{"campo":"search_codice","valore":"prod01A"},{"campo":"search_disponibilita","valore":"1"}\]*

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**search**" presente alla pagina "***Sito
  Preferenze***" del Wizard, tab "***Tracciamento Dati***" sezione
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
> verificato l'evento più un ulteriore codice univoco (es.
> *"Search-20221110145456-779*")

**ATTENZIONE!** ai parametri indicati vanno poi aggiunti, se
disponibili, anche quelli relativi alle informazioni dei clienti
(indirizzo mail, città, fbp, fbc ...) disponibili per l'evento stesso
secondo quanto specificato nei precedenti capitoli di questo manuale

