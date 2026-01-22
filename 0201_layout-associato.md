# LAYOUT ASSOCIATO



Il parametro "**Layout Associato**" presente nella parte alta della
maschera "**Modifica Variante Sito**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_layout_associato_res.bmp](./assets/media/image22.png){width="5.111805555555556in"
height="3.1416666666666666in"}

consente di associare alla Variante in esame uno specifico Layout
selezionandolo tra quelli attualmente codificati per la Variante stessa.

**Grazie a questo campo è quindi possibile definire un layout comune a
tutto il sito che verrà applicato automaticamente a tutte le pagine nel
momento in cui si dovesse decidere di portare on line la Variante in
esame.**

Come evidenziato nel relativo capitolo di questo manuale oltre che a
livello di Variante, è poi possibile definire e gestire un layout anche
a livello di singola pagina, e non necessariamente il layout associato
alla singola pagina deve coincidere con quello associato all'intera
Variante.

Nel caso in cui si dovesse decidere di gestire due diversi layout, per
la Variante e per la singola pagina, sarà necessario considerare che:

- le impostazioni dei contenitori strutturali definite sul layout di
  Pagina avranno priorità rispetto a quelle eventualmente definite sul
  layout di Variante

- i Meta Tag definiti sul layout di Pagina andranno a sommarsi a quelli
  eventualmente definiti a livello di Variante.

> In particolare, nel codice HTML della pagina web verranno inseriti
> prima i Meta Tag definiti sul layout associato alla Variante Sito, e
> poi quelli definiti sul layout associato alla specifica pagina web

- le inclusioni definite sul layout di Pagina andranno a sommarsi a
  quelle eventualmente definiti a livello di Variante.

> In particolare, nel codice HTML della pagina web verranno inserite
> prima le inclusioni definite sul layout associato alla Variante Sito,
> e poi quelle definite sul layout associato alla specifica pagina web

- il codice CSS personalizzato definito sul layout di Pagina andrà ad
  accodarsi a quello eventualmente definito a livello di Variante

> In particolare nel caso in cui si sia deciso di inserire questo codice
> in un file esterno verrà caricato prima il file CSS generato dal
> layout definito a livello di Variante, e dopo quello generato dal
> layout definito a livello di pagina.
>
> Allo stesso modo nel caso in cui si sia deciso di gestire questo
> codice in-line alla pagina, all'interno del apposito tag style verrà
> inserito prima il CSS definito sul layout di Variante, e in coda
> quello definito sul layout di pagina.

- il codice javascript personalizzato definito sul layout di Pagina
  andrà ad accodarsi a quello eventualmente definito a livello di
  Variante

> In particolare nel caso in cui si sia deciso di inserire questo codice
> in un file esterno verrà caricato prima il file javascript generato
> dal layout definito a livello di Variante, e dopo quello generato dal
> layout definito a livello di pagina.
>
> Allo stesso modo nel caso in cui si sia deciso di gestire questo
> codice in-line alla pagina, all'interno del apposito tag script verrà
> inserito prima il javascript definito sul layout di Variante, e in
> coda quello definito sul layout di pagina.
>
> **NOTA BENE: p**er maggiori informazioni relativamente alla gestione
> dei layout si veda anche il capitolo "Live Editing per Varianti
> Responsive -- Layout" di questo manuale.

