# ORDINAMENTO ARTICOLI



Come evidenziato nel precedente capitolo il parametro "**Visualizza
Ordinamento**" presente nella maschera di configurazione del "Catalogo
Ecommerce", consente se selezionato, di visualizzare, lato sito, una
combo box contenente l'elenco degli elementi sulla base dei quali poter
effettuare l'ordinamento degli articoli presenti all'interno del
componente.

La combo box di selezione sarà preceduta inoltre da un testo indicativo,
"Ordina per:", modificabile nella sezione **"Gestione Testi/Messaggi
Sito"** del Wizard agendo sulla voce **"Catalogo Ecommerce"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ordinamento_articoli_combo_box.bmp](./assets/media/image12.png){width="4.883333333333334in"
height="3.5708333333333333in"}

**ATTENZIONE!** il valore selezionato inizialmente all'interno della
combo box sarà quello dell'elemento sulla base del quale è stato
impostato l'ordinamento di default.

Al cambio della selezione verrà ricaricato il componente (non l'intera
pagina) e il suo contenuto verrà ordinato in base al nuovo campo di
ordinamento.

Dipendentemente poi da come è stato settato, in fase di configurazione
del componente, il parametro **Identificatore per ordinamento,**
l'ordinamento applicato ad un componente "Catalogo Ecommerce" potrebbe
essere applicato automaticamente anche ad altri componenti dello stesso
tipo presenti all'interno della stessa pagina

**NOTA BENE:** nel caso in cui il componente sia paginato un'eventuale
variazione del campo di ordinamento riporterà il componente stesso sulla
prima pagina.

L'ordinamento inoltre, non verrà mantenuto in fase di navigazione del
sito. Questo significa dunque che, se dopo aver modificato l'ordinamento
del componente si dovesse continuare la navigazione del sito cambiando
pagina, al ritorno nella pagina che ospita il componente in oggetto, il
suo ordinamento sarà nuovamente quello di default.

Per impostare gli elementi sulla base dei quali poter effettuare
l'ordinamento degli articoli, è necessario agire dalla sezione
**"Gestione Campi di Ordinamento"**, presente anch'essa all'interno
della maschera di configurazione del componente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_catalogo_ecommerce2_res.bmp](./assets/media/image13.png){width="4.889583333333333in"
height="2.417361111111111in"}

All'interno di questa sezione, sulla sinistra sono elencati gli elementi
di ordinamento attualmente codificati, sulla destra sono invece
riportate le proprietà dell'elemento attualmente selezionato in elenco.
Per modificare uno di questi elementi sarà quindi sufficiente
selezionarlo e agire poi sui parametri presenti all'interno della
sezione "**Modifica Campo Ordinamento**".

Allo stesso modo per codificare un nuovo elemento sarà necessario
cliccare sull'icona raffigurante un piccolo + (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image14.png){width="0.19027777777777777in"
height="0.19027777777777777in"} ) e definire poi le proprietà
dell'elemento stesso.

In particolare per ogni singolo elemento di ordinamento occorrerà
specificare un valore per i seguenti campi:

**Testo:** etichetta identificativa dell'elemento di ordinamento che si
sta codificando. Tale etichetta comparirà poi, come possibile opzione di
selezione, all'interno della combo box visualizzata lato sito nel
momento in cui dovesse essere stato selezionato il parametro "Visualizza
Ordinamento".

**Tipo di ordinamento:** consente di specificare il campo sulla base del
quale dovranno essere ordinati gli articoli presenti all'interno del
componente nel momento in cui, lato sito, dovesse essere selezionato
l'elemento di ordinamento che si sta codificando.

E' possibile indicare una delle seguenti opzioni:

- **Campo Articolo:** selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Campo di
  Ordinamento**") lo specifico campo del gestionale che dovrà essere
  utilizzato per definire l'ordinamento degli articoli. E' possibile
  selezionare una delle seguenti opzioni:

  - **Titolo**: l'ordinamento verrà determinato sulla base del campo
    "Descrizione" presente all'interno dell'Anagrafica Articoli del
    gestionale.

  - **Codice**: l'ordinamento verrà determinato sulla base del campo
    "Codice" presente all'interno dell'Anagrafica Articoli del
    gestionale.

  - **Codice Alternativo (solo Ecommerce Mexal):** l'ordinamento verrà
    determinato sulla base del campo "Codice Alternativo"
    dell'Anagrafica Articoli di Mexal

  - **Descrizione**: l'ordinamento verrà determinato sulla base del
    campo Descrizione presente all'interno della maschera "Modifica
    Articolo" accessibile, in Passweb, dalla voce di menu "Catalogo --
    Gestione Articoli" dopo aver selezionato, ovviamente, uno specifico
    articolo ed aver cliccato sul pulsante "Modifica Articolo"

  - **Codice Categoria Statistica Articolo**: l'ordinamento verrà
    determinato sulla base del codice della Categoria Statistica di
    appartenenza degli articoli presenti all'interno del componente.

  - **Descrizione Categoria Statistica Articolo**: l'ordinamento verrà
    determinato sulla base della descrizione della Categoria Statistica
    di appartenenza degli articoli presenti all'interno del componente

  - **Codice Categoria Merceologica**: l'ordinamento verrà determinato
    sulla base del codice della Categoria Merceologica degli articoli
    presenti all'interno del componente

  - **Descrizione Categoria Merceologica**: l'ordinamento verrà
    determinato sulla base della descrizione della Categoria
    Merceologica degli articoli presenti all'interno del componente

  - **Codice Natura** (solo Ecommerce Mexal): l'ordinamento verrà
    determinato sulla base del codice della Natura associata in Mexal
    agli articoli presenti all'interno del componente

  - **Descrizione Natura** (solo Ecommerce Mexal): l'ordinamento verrà
    determinato sulla base della descrizione della Natura associata in
    Mexal agli articoli presenti all'interno del componente.

  - **Data di Creazione:** l'ordinamento verrà determinato sulla base
    della data di creazione degli articoli presenti all'interno del
    componente.

> **ATTENZIONE!** Per "**Data di creazione**" si intende la data in cui
> l'articolo è stato inserito per la prima volta nel database del sito

- **Disponibilità:** l'ordinamento verrà determinato sulla base del
  valore della disponibilità degli articoli presenti all'interno del
  componente.

> **ATTENZIONE!** Il valore della disponibilità è sempre quello
> aggiornato all'ultima sincronizzazione utile (e potrebbe quindi non
> coincidere con l'effettiva disponibilità degli articoli). La formula
> secondo cui determinare tale valore è invece quella indicata
> all'interno del relativo campo della maschera "Catalogo
> Mexal/Ho.Re.Ca"

- **Listino:** l'ordinamento verrà determinato sulla base dei prezzi
  definiti, per i vari articoli, nel listino utilizzato per l'utente che
  sta navigando il sito.

> **ATTENZIONE: una volta impostato l'ordinamento dunque, ogni articolo
> verrà posizionato in base al suo effettivo prezzo di listino e non
> verrà quindi considerata nessun tipo di particolarità e/o scontistica
> definita all'interno del gestionale o in fase di configurazione del
> sito stesso.**
>
> [Nel caso infatti di particolarità prezzo e/o sconto il prezzo
> effettivo degli articoli non è memorizzato nel database di Passweb ma
> viene calcolato in tempo reale sulla base delle condizioni commerciali
> definite per lo specifico articolo e/o per lo specifico utente che sta
> navigando il sito]{.underline}.
>
> **Nel caso in cui si dovesse quindi decidere di utilizzare un
> ordinamento per prezzo e, allo stesso tempo, anche delle particolarità
> prezzo e/o sconto, una volta impostato l'ordinamento gli articoli
> soggetti a particolarità potrebbero non soddisfare i criteri di
> ordinamento effettivamente impostati.**
>
> **Allo stesso modo anche gli articoli con "Prezzo a Richiesta**"
> **verranno posizionati, in fase di ordinamento, sulla base del loro
> effettivo prezzo di listino.**
>
> **ATTENZIONE! Impostando questo tipo di ordinamento per la prima
> volta, sarà necessario effettuare una sincronizzazione totale in modo
> tale da aggiornare il database del sito con i prezzi di listino
> corretti.**

- **Attributo Articolo**: selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Attributo di
  Ordinamento**") l'Attributo Articolo (sia esso di tipo Passweb, sia
  esso di tipo Mexal) che dovrà essere utilizzato per definire
  l'ordinamento degli articoli. E' possibile selezionare uno qualsiasi
  degli Attributi Articolo precedentemente codificati all'interno della
  corrispondente sezione del Wizard.

- **Casuale**: impostando questo valore l'ordine di visualizzazioni
  degli articoli presenti all'interno del componente sarà casuale. Tale
  ordinamento, stabilito ad una prima vista della pagina che ospita il
  componente in oggetto, verrà poi mantenuto per tutta la durata della
  sessione (compreso un tempo di inattività fissato a 20 minuti).
  Esaurito questo intervallo di tempo successive visite alla pagina
  contenente il componente determineranno un nuovo ordinamento casuale.

- **Articoli più vist**i: selezionando questo valore gli articoli
  presenti all'interno del componente verranno ordinati sulla base della
  loro popolarità.

> **ATTENZIONE!** **il criterio di popolarità utilizzato per ordinare
> gli articoli all'interno del componente è determinato da quello che è
> il numero di visite ricevute dalle relative pagine prodotto**.
>
> In questo caso sarà anche possibile impostare, mediante il successivo
> campo **"Periodo (giorni)"**, il numero esatto di giorni che dovranno
> essere considerati per valutare gli articoli più popolari.
>
> E' quindi possibile ordinare gli articoli presenti all'interno del
> componente in base a quelli che sono, ad esempio, i più visti
> dell'ultima settimana

- **Articoli più venduti**: selezionando questo valore gli articoli
  presenti all'interno del componente verranno ordinati in base a quelli
  che risultano essere i più venduti

> **ATTENZIONE! gli articoli più acquistati sono determinati solo ed
> esclusivamente sulla base degli ordini attualmente presenti in Passweb
> e del numero di volte in cui uno stesso articolo compare all'interno
> di questi stessi ordini.**
>
> Come per il parametro precedente anche in questo caso il successivo
> campo **"Periodo (giorni)"**, consente di indicare il numero esatto di
> giorni che dovranno essere considerati per valutare gli articoli più
> acquistati.
>
> E' quindi possibile ordinare gli articoli presenti all'interno del
> componente in base a quelli che sono, ad esempio, i più venduti
> dell'ultima settimana.

**NOTA BENE:** lato Wizard l'ordinamento casuale degli articoli, una
volta impostato, sarà sempre le stesso e non varierà quindi al termine
della sessione.

**Modo di Ordinamento:** consente di specificare se, in relazione
all'elemento che si sta codificando, dovrà essere applicato un
ordinamento di tipo Crescente o Decrescente. Tale campo non sarà
ovviamente presente nel caso in cui sia stato impostato un ordinamento
di tipo Casuale.

**Default:** se selezionato, il corrispondente elemento verrà
considerato come elemento sulla base del quale ordinare a default gli
articoli presenti all'interno del componente.

**NOTA BENE:** è obbligatorio indicare un ordinamento di default. Nel
caso in cui questo non dovesse essere indicato al salvataggio del
componente verrà visualizzato un apposito messaggio di errore.

Infine va anche ricordato che i campi sulla base dei quali poter
stabilire l'ordine di visualizzazione degli articoli presenti
all'interno dei componenti saranno sempre considerati come testuali. In
conseguenza di ciò, un articolo con il campo di ordinamento impostato,
ad esempio sul valore 10, verrà visualizzato nel caso di ordinamento
Crescente (Decrescente) prima (dopo) di un articolo con il campo di
ordinamento impostato sul valore 2.

Il pulsante "**Aggiungi** **Elemento**" presente nella parte alta della
maschera consentirà di aggiungere in elenco l'elemento appena
codificato.

