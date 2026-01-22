# CACHE DEI COMPONENTI



Un altro strumento particolarmente utile, e sicuramente più efficace
rispetto alle due opzioni esaminate nel precedente capitolo di questo
manuale (staticizzazione e caricamento javascript), per abbattere i
tempi di caricamento delle pagine web è rappresentato, indubbiamente,
dal modulo di cache attivabile per ogni sito Passweb.

La cache offre infatti una sorta di staticizzazione dinamica dell'intera
pagina web che non è sottoposta agli stessi vincoli validi per la
staticizzazione dei singoli componenti e che, soprattutto, può essere
attivata e gestita anche per ogni singolo utente autenticato

**ATTENZIONE!** per maggiori informazioni relativamente al modulo di
cache attivabile per il proprio sito Passweb si consiglia di fare
riferimento a quanto indicato all'interno del corrispondente capitolo
("*Configurazione -- Cache*") di questo manuale

In quest'ottica il parametro "**Disabilita Cache**" presente nella
maschera di configurazione di molti, ma non di tutti i componenti
Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\disabilita_cache.bmp](./assets/media/image71.png){width="3.8958333333333335in"
height="2.7465277777777777in"}

è quello che consente effettivamente di decidere se quello specifico
componente dovrà o meno essere messo in cache

**ATTENZIONE! il parametro "Disabilita Cache" a default è
disabilitato.** Nel momento in cui l'esigenza dovesse essere dunque, una
volta attivata la cache, quella di rendere determinati componenti non
cachabili sarà necessario agire direttamente su quello specifico
componente mediante il parametro in questione.

Occorre anche considerare però che, come detto, il parametro "Disabilita
Cache" non è presente nella maschera di configurazione di tutti i
componenti Passweb e questo per diverse possibili ragioni. Nello
specifico:

- Non tutti i componenti Passweb potranno essere messi in cache.
  Componenti come il Carrello o il Checkout, per loro stessa natura,
  dovranno essere, per forza di cose, sempre e comunque dei componenti
  dinamici

- Il componente Contenitore per come è strutturato e per quello che è il
  suo utilizzo, a livello 1 sarà sempre e comunque un componente
  cachabile e non si potrà mai decidere di escluderlo dalla cache. Nel
  momento in cui dovesse invece essere gestito come componente di
  livello maggiore o uguale a 2 (ed essere quindi inserito all'interno
  di un altro componenti di tipo contenitore) verrà o meno cachato a
  seconda delle impostazioni settate per il componente padre.

- Per i componenti Ecommerce, Interazione Utente e CMS di secondo
  livello, quelli, tanto per intenderci, come il "Titolo Articolo" che
  può essere inserito all'interno di un Catalogo Ecommerce, il "Sommario
  CMS" che può essere inserito all'interno di un "Archivio CMS", i campi
  Form che possono essere inserti all'interno di componenti di primo
  livello come il "Form di Registrazione Utente" ecc... il fatto che
  vengano o meno messi in cache dipenderà sempre da quelle che sono le
  impostazioni settate per il loro componente padre.

> In sostanza dunque non sarà mai possibile impostare come cachabile, ad
> esempio, il Catalogo Ecommerce e allo stesso tempo impostare invece
> come non cachabili il Titolo o il Prezzo degli articoli inseriti
> all'interno del catalogo stesso.

Per maggiori informazioni relativamente alla possibilità di mettere o
meno in cache un determinato componente si consiglia di fare riferimento
a quanto indicato all'interno di questo manuale relativamente ai
parametri di configurazione di quello stesso componente

**ATTENZIONE!** **eventuali variazioni apportate al parametro
"Disabilita Cache" per un determinato componente richiedono, per poter
essere effettivamente attive, un reset della cache attualmente in uso al
sito**

