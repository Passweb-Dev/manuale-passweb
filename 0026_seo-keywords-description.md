# SEO -- KEYWORDS DESCRIPTION



Al pari del processo di assegnazione di uno specifico "Title" alle
pagine prodotto, anche il processo di assegnazione di determinate
Keywords e Description agli articoli gestiti all'interno del proprio
sito è di fondamentale importanza per una corretta indicizzazione dei
relativi prodotti sui vari motori di ricerca e per una loro più semplice
reperibilità da parte dell'utente che effettua ricerche in rete.

In questo senso Passweb offre all'utente la possibilità di
personalizzare e automatizzare la creazione di Keywords e Description
per gli articoli, utilizzando direttamente le informazioni per essi
pubblicate all'interno del sito.

La sezione "**Keywords e Description**", presente all'interno del menu
**"Preferenze --SEO",** consente infatti di impostare sia a livello di
pagine di categoria che a livello di singole pagine prodotto, la
struttura che dovrà essere utilizzata per poi generare le Keywords e le
Description relative agli articoli gestiti all'interno del proprio sito
e-commerce.

![](./assets/media/image26.png)

I campi presenti all'interno di questa sezione consentono
rispettivamente di:

**Gestione Keywords / Description**: consente di decidere se le Keywords
/ Description delle varie pagine dovranno essere generate tenendo conto
anche di quanto indicato all'interno di questa sezione del Wizard oppure
dando priorità a quanto inserito per le Pagine di Categoria e/o per le
Pagine Prodotto nei relativi campi

E' possibile selezionare uno dei seguenti valori:

- **Generica:** selezionando questa opzione le Keywords / Description
  delle pagine di Categoria e delle pagine Prodotto verranno generate
  sulla base del formato definito all'interno di questa sezione del
  Wizard.

> Eventuali Keywords / Description inserite in maniera specifica nelle
> singole pagine di Categoria e/o nelle singole pagine Prodotto, e che
> non dovessero rientrare già nei segnaposto impostati per il formato
> utilizzato, verranno aggiunte in coda a tutto il resto

- **Specifica:** selezionando questa opzione le Keywords / Description
  definite per le singole pagine di Categoria e / o per le singole
  pagine Prodotto avranno priorità su quanto impostato all'interno della
  sezione "Preferenze Sito" del Wizard.

> In queste condizioni, dunque se le Keywords / Description di una
> specifica pagina dovessero essere impostate correttamente verranno
> utilizzate quelle indipendentemente da tutto il resto.
>
> Se invece, per determinate pagine, questi dati non dovessero essere
> valorizzati, verrà considerato allora quanto impostato nel formato
> definito nei corrispondenti campi della sezione "Preferenze Sito" del
> Wizard

**Formato Keywords / Description Pagina Prodotto**: consente di
impostare la struttura che dovrà essere utilizzata per automatizzare la
creazione delle Keywords / Description da inserire nelle Pagine Prodotto
dei vari articoli gestiti all'interno del sito

Cliccando sul pulsante "**Aggiungi Segnaposto**" verrà infatti
visualizzato l'elenco dei campi attualmente utilizzati per fornire
informazioni sugli articoli. I segnaposto selezionati verranno poi
sostituiti, nel processo di generazione delle Keywords / Description,
articolo per articolo, con il valore del corrispondente campo

Sono gestiti i seguenti segnaposto:

- **Titolo:** segnaposto corrispondente **{productName}**

> Sostituito in fase di creazione delle Keywords / Description dal
> "**Titolo**" utilizzato per i vari articoli.
>
> **ATTENZIONE!** Si ricorda che il valore del campo Titolo dipende da
> come è stato impostato il parametro "**Tipo di dato da utilizzare**"
> presente all'interno della sezione "Titolo / Permalink Articolo" (per
> maggiori informazioni in merito si vedano i successivi capitoli di
> questo manuale)

- **Meta:** segnaposto corrispondente **{productMeta}**

> Sostituito in fase di creazione delle Keywords / Description con
> quanto inserito all'interno del campo "**Keywords Meta**" /
> "**Description Meta**" presente nell' Anagrafica Passweb (sezione
> "*SEO -- Sitemap*") del relativo articolo

![](./assets/media/image27.png)

> **ATTENZIONE!** Nel caso in cui per un determinato articolo non sia
> stato specificato nulla per i campi Meta evidenziati in figura, il
> segnaposto in oggetto verrà sostituito con il Titolo del prodotto

- **Descrizione:** segnaposto corrispondente **{productDescription}**

> Sostituito in fase di creazione delle Keywords / Description dalla
> Descrizione (ripulita di eventuali tag html) utilizzata per i vari
> articoli
>
> **ATTENZIONE!** Si ricorda che la Descrizione dei vari articoli
> coincide esattamente con quanto visualizzato all'interno del
> Componente "Descrizione"

- **Descrizione HTML / 2 / 3:** segnaposto corrispondente
  **{\$productDescriptionHTML\$}** (**\$productDescriptionHTML2\$ -
  \$productDescriptionHTML3\$**)

> Sostituito in fase di creazione delle Keywords / Description da quanto
> presente all'interno dei campi Descrizione HTML /2 /3 presenti
> nell'anagrafica Passweb dei vari articoli (il tutto ripulito da
> eventuali tag html)

- **Descrizione Dettagliata:** segnaposto corrispondente
  **{\$productDescriptionDetailed\$}**

> Sostituito in fase di creazione delle Keywords / Description da quanto
> presente all'interno del campo "**Descrizione Dettagliata**" presente
> nell'anagrafica Passweb dei vari articoli (il tutto ripulito da
> eventuali tag html)

- **Categoria:** segnaposto corrispondente **{categoryName}**

> Sostituito in fase di creazione delle Keywords / Description dalla
> categoria merceologica di appartenenza dei singoli articoli

- **Percorso Categoria:** segnaposto corrispondente
  **{categoryStructure}**

> Sostituito in fase di creazione delle Keywords / Description
> dall'elenco di tutte le categorie merceologiche ( separate dal
> carattere "-" ) cui appartiene il relativo articolo
>
> Supponendo quindi che un determinato articolo appartenga alla
> categoria "CAT 4", all'interno di un albero così strutturato
>
> CAT1
>
> \| CAT2
>
> \| CAT3
>
> \| CAT4
>
> il segnaposto in oggetto verrà sostituito dai valori "CAT1 -- CAT2 --
> CAT3 -- CAT4"

- **Percorso Categoria Padre:** segnaposto corrispondente
  **{categoryStructureFather}**

> Sostituito in fase di creazione delle Keywords / Description dalla
> categoria merceologica di appartenenza del relativo articolo e dalla
> sua diretta categoria padre ( separate dal carattere "-" )
>
> Supponendo quindi che un determinato articolo appartenga alla
> categoria "CAT 4", all'interno di un albero così strutturato
>
> CAT1
>
> \| CAT2
>
> \| CAT3
>
> \| CAT4
>
> il segnaposto in oggetto verrà sostituito dai valori "CAT3 -- CAT4"

- **Descrizione Categoria:** segnaposto corrispondente
  **{categoryDescription}**

> Sostituito in fase di creazione delle Keywords / Description dalla
> descrizione della categoria merceologica di appartenenza del relativo
> articolo

- **Attributi articolo:** segnaposto corrispondente **{attr_N}**

> Sostituito in fase di creazione delle Keywords / Description dal
> valore dell'Attributo selezionato

**ATTENZIONE!** A default i campi in esame vengono valorizzato con il
segnaposto **{productName}** corrispondente al campo **"Titolo".**

**NOTA BENE**: affinchè i segnaposto sopra indicati possano funzionare
in maniera corretta, ed essere quindi sostituiti articolo per articolo
con il relativo valore, è necessario non alterarne la struttura. Nel
caso in cui, dunque, vengano eliminate le parentesi graffe e/o venga
modificato il nome del segnaposto, questi non verranno più considerati
come tali ma come del semplice testo da utilizzare allo stesso modo per
le Keywords di tutti gli articoli gestiti sul sito.

**Formato Description Pagina Catalogo:** consente di impostare la
struttura che dovrà essere utilizzata per automatizzare la creazione
delle Description da inserire nelle Pagine Catalogo corrispondenti alle
varie categorie merceologiche gestite all'interno del sito.

Anche in questo caso cliccando sul pulsante "**Aggiungi Segnaposto**"
verrà visualizzato l'elenco dei segnaposto effettivamente utilizzabili.

A differenza del caso precedente, per il campo in esame sono gestiti i
seguenti segnaposto:

- **Categoria:** segnaposto corrispondente **{categoryName}**

> Sostituito in fase di creazione della Description dal nome della
> relativa categoria merceologica

- **Descrizione Categoria:** segnaposto corrispondente
  **{categoryDescription}**

> Sostituito in fase di creazione della Description dalla descrizione
> della relativa categoria merceologica

- **Meta Categoria:** segnaposto corrispondente {**categoryMeta}**

> Sostituito in fase di creazione della Description con quanto inserito
> all'interno del campo "**Description Meta**" presente nell' Anagrafica
> Passweb (sezione "*SEO -- Sitemap*") della relativa categoria
> merceologica

![](./assets/media/image28.png)

> **ATTENZIONE!** Nel caso in cui per una determinata categoria non sia
> stato specificato nulla per il campo Meta evidenziati in figura, il
> segnaposto in oggetto verrà sostituito con il Nome della Categoria
> stessa

- **Meta Percorso Categoria Padre:** segnaposto corrispondente
  **{categoryMetaFather}**

> Sostituito in fase di creazione della Description con quanto inserito
> all'interno del campo "**Description Meta**" presente nell' Anagrafica
> Passweb (sezione "*SEO -- Sitemap*") della relativa categoria
> merceologica

![](./assets/media/image28.png)

> **ATTENZIONE!** A differenza del caso precedente, in queste condizioni
> se per una determinata categoria non dovesse essere stato specificato
> nulla per il campo Meta evidenziato in figura, il segnaposto in
> oggetto verrà sostituito con il Nome della Categoria stessa e quello
> della sua diretta categoria padre (separati da "-")

- **Percorso Categoria:** segnaposto corrispondente
  **{categoryStructure}**

> Sostituito in fase di creazione della Description dall'elenco di tutte
> le categorie merceologiche ( separate dal carattere "-" ) fino ad
> arrivare alla categoria in esame
>
> Supponendo quindi che la categoria in esame sia "CAT 4", all'interno
> di un albero così strutturato
>
> CAT1
>
> \| CAT2
>
> \| CAT3
>
> \| CAT4
>
> il segnaposto in oggetto verrà sostituito dai valori "CAT1 -- CAT2 --
> CAT3 -- CAT4"

- **Percorso Categoria Padre:** segnaposto corrispondente
  **{categoryStructureFather}**

> Sostituito in fase di creazione della Description dalla categoria
> merceologica in esame e dalla sua diretta categoria padre ( separate
> dal carattere "-" )
>
> Supponendo quindi che la categoria in esame sia "CAT 4", all'interno
> di un albero così strutturato
>
> CAT1
>
> \| CAT2
>
> \| CAT3
>
> \| CAT4
>
> il segnaposto in oggetto verrà sostituito dai valori "CAT3 -- CAT4"

- **Sito:** segnaposto corrispondente **{siteName}**

> Sostituito in fase di creazione della Description con quanto inserito
> nel campo "**Nome Sito**"

In ogni caso l'utente avrà sempre la possibilità di personalizzare
ulteriormente le Keywords o la Description da utilizzare per uno
specifico articolo agendo per questo dall'apposita sezione (SEO)
dell'anagrafica Passweb dell'articolo in esame ( per maggiori
informazioni in merito si veda anche la sezione "*Catalogo -- Gestione
Articoli -- Articoli*" di questo manuale).

