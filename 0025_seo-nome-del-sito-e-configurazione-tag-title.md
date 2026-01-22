# SEO -- NOME DEL SITO E CONFIGURAZIONE TAG TITLE



La sezione "**Nome del Sito e Configurazione Tag Title**", presente
all'interno del menu **"Preferenze --SEO"** perette di impostare la
struttura che dovrà essere utilizzata per generare il Title delle
diverse tipologie di pagina presenti all'interno del sito web.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\preferenze_sito_seo.bmp](./assets/media/image22.png)

La scelta del **titolo di una pagina web** rappresenta il **primo
importante passo per un buon posizionamento della pagina sui motori di
ricerca**.

Il titolo di una pagina (corrispondente a quanto presente nel codice
della pagina stessa all'interno del tag HTML \<Title\>) comunica infatti
gli argomenti della pagina stessa sia agli utenti che ai motori di
ricerca

I motori di ricerca assegnano poi al Title della pagina un\'importanza
molto alta in quanto sono spinti a credere che i suoi contenuti siano
estremamente \"genuini\" e che riassumano bene i reali contenuti della
pagina.

**In questo senso all'interno di Passweb è possibile, definire, per
ciascuna delle tipologie di pagina gestite, una specifica struttura da
utilizzare per generare e valorizzare in maniera automatica il tag
\<Title\> per ognuna di queste pagine.**

**Per fare questo è possibile utilizzare anche appositi segnaposto che
verranno poi valorizzati pagina per pagina con specifici valori propri
della pagina stessa.**

Per utilizzare un segnaposto è sufficiente cliccare sul pulsante
"**Aggiungi segnaposto**" del relativo campo e selezionare uno dei
valori tra quelli proposti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\aggiungi_segnaposto_title.bmp](./assets/media/image23.png)

In particolare, nella definizione dei Title delle pagine, è possibile
utilizzare i seguenti elementi:

- **Sito:** segnaposto corrispondente **{ siteName }**. Utilizzabile per
  tutte le diverse tipologie di pagina.

> Sostituito in fase di creazione del Title di pagina con quanto
> inserito nel campo "**Nome Sito**" presente all'interno di questa
> stessa sezione del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_sitename.bmp](./assets/media/image24.png)

- **Pagina:** segnaposto corrispondente **{ pageName }**. Utilizzabile
  per le pagine semplici (pagine generiche, bianche, e pagine ecommerce,
  verdi) e per le pagine CMS

> Sostituito in fase di creazione del Title di pagina con quanto
> inserito all'interno del campo "**Titolo Pagina**" presente nelle
> proprietà della pagina stessa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_pagename.bmp](./assets/media/image25.png)

> **ATTENZIONE!**: Nel caso in cui il parametro "Titolo Pagina" non sia
> stato valorizzato il segnaposto in oggetto verrà sostituito con quanto
> presente all'interno del campo "Nome Pagina"

- **Categoria:** segnaposto corrispondente **{ categoryName }.**
  Utilizzabile per le pagine Catalogo (pagine azzurre) e per le pagina
  Prodotto( pagine rosse)

> Sostituito in fase di creazione del Title di pagina con quanto
> indicato in corrispondenza del campo "**Title**" presente
> nell'anagrafica Passweb della relativa Categoria Merceologica
>
> **ATTENZIONE!** Nel caso in cui non sia stato indicato per le
> Categorie Merceologiche uno specifico valore per il campo "Title" il
> segnaposto in esame verrà sostituito con il Nome della relativa
> categoria merceologica

- **Categoria e Padre:** segnaposto corrispondente
  **{categoryNameFather}.** Utilizzabile per le pagine Catalogo (pagine
  azzurre)

> Sostituito in fase di creazione del Title di pagina con quanto
> indicato in corrispondenza del campo "**Title**" presente
> nell'anagrafica Passweb della relativa Categoria Merceologica.
>
> **ATTENZIONE!** Nel caso in cui non sia stato indicato per una
> determinata Categoria Merceologica uno specifico valore per il campo
> "Title" il segnaposto in esame verrà sostituito con il Nome della
> relativa categoria merceologica e quello della sua diretta categoria
> padre (separati da "-")

- **Percorso Categoria:** segnaposto corrispondente
  **{categoryStructure}.** Utilizzabile per le pagine Catalogo (pagine
  azzurre) e per le pagine Prodotto (pagine rosse)

> Sostituito in fase di creazione del Title di pagina con l'elenco di
> tutte le categorie merceologiche (separate dal carattere "-" ) cui
> appartiene, all'interno dell'albero delle categorie merceologiche del
> gestionale, la specifica sotto-categorie o lo specifico articolo

- **Percorso Categoria Padre:** segnaposto corrispondente
  **{categoryStructureFather}.** Utilizzabile per le pagine Catalogo
  (pagine azzurre) e per le pagine Prodotto (pagine rosse)

> Sostituito in fase di creazione del Title di pagina con la categoria
> merceologica o quella di appartenenza del relativo articolo e con la
> sua diretta categoria padre (separate dal carattere "-")

- **Titolo:** segnaposto corrispondente **{productName}.** Utilizzabile
  per le pagine Prodotto (pagine rosse)

> Sostituito in fase di creazione del Title di pagina con quanto
> indicato in corrispondenza del campo "**Title**" presente
> nell'anagrafica Passweb del relativo articolo
>
> **ATTENZIONE!** Nel caso in cui non sia stato indicato per il singolo
> articolo uno specifico valore per il campo "Title" il segnaposto in
> esame verrà sostituito con il valore del campo Titolo del relativo
> prodotto
>
> **ATTENZIONE!** Si ricorda che il valore del campo Titolo dipende da
> come è stato impostato il parametro "**Tipo di dato da utilizzare**"
> presente all'interno della sezione "Titolo / Permalink Articolo" (per
> maggiori informazioni in merito si vedano i successivi capitoli di
> questo manuale)

- **Attributi articolo:** segnaposto corrispondente **{attr_N}**.
  Utilizzabile per le pagine Prodotto( pagine rosse)

> Sostituito in fase di creazione del Title di pagina dal valore
> dell'Attributo selezionato

- **Articolo:** segnaposto corrispondente **{ articleName }**.
  Utilizzabile per le pagine CMS (nello specifico le pagine utilizzate
  per la lettura del dettaglio di un post CMS)

> Sostituito in fase di creazione del Title di pagina Title con il
> Titolo dell'articolo di cui si sta visualizzando il dettaglio o con
> quanto inserito, in fase di configurazione dell'articolo stesso,
> all'interno del suo campo "Title"
>
> Per maggiori informazioni in merito si veda anche la sezione "*Sito --
> Gestione CMS -- Gestione Contenuti*" di questo manuale

**NOTA BENE**: affinché i segnaposto sopra indicati possano funzionare
in maniera corretta, ed essere quindi sostituiti pagina per pagina con
il relativo valore, è necessario non alterarne la struttura.

Nel caso in cui, dunque, si dovesse decidere di inserire i segnaposto
manualmente senza selezionarli dall'apposito menu occorre prestare molta
attenzione ad utilizzare il nome corretto e a non eliminare le parentesi
graffe. In caso contrario il segnaposto non verrà più considerato come
tale ma come del semplice testo da inserire in maniera uguale nel Title
di ogni singola pagina.

I segnaposto sopra indicati possono poi essere utilizzati (in relazione
ovviamente alle tipologie di pagina per cui sono effettivamente ammessi)
e combinati tra loro e/o assieme a del normale testo per definire la
struttura che dovrà poi essere utilizza nella generazione del Title
della specifica tipologia di pagina.

I campi presenti all'interno di questa sezione consentono
rispettivamente di:

**Nome del Sito (visualizzato nel Titolo):** consente di impostare il
nome del sito.

La stringa inserita all'interno di questo campo potrà poi essere
utilizzata, grazie all'apposito segnaposto **{sitename}**, nella
creazione del tag "Title" delle varie pagine

**Gestione Title:** consente di decidere se il Title delle pagine dovrà
essere generato sulla base del formato definito all'interno della
sezione "Preferenze Sito" del Wizard, oppure sulla base di quanto
indicato in fase di configurazione della specifica pagina / categoria /
prodotto.

E' possibile selezionare uno dei seguenti valori:

- **Generica:** selezionando questa opzione il Title delle varie pagine
  del sito verrà generato sulla base del formato indicato all'interno
  della sezione "Preferenze Sito" del Wizard (parametri "Formato Title
  per Pagina Semplice / Catalogo / Prodotto / CMS).

- **Specifica:** selezionando questa opzione il Title definito per le
  singole pagine avrà priorità su quanto impostato all'interno della
  sezione "Preferenze Sito" del Wizard.

> In queste condizioni dunque se il Title di una specifica pagina
> dovesse essere valorizzato correttamente verrà utilizzato quello
> indipendentemente da tutto il resto. Se invece, per determinate
> pagine, il Title non dovesse essere valorizzato in maniera specifica,
> verrà generato sulla base del formato indicato all'interno della
> sezione "Preferenze Sito" del Wizard (parametri "Formato Title per
> Pagina Semplice / Catalogo / Prodotto / CMS)

**Formato Title per Pagina Semplice:** consente di definire la struttura
del Title che dovrà essere generato per le pagine semplici, dove, per
pagine semplici si intendono le pagine generiche (pagine bianche) e le
pagine ecommerce (pagine verdi). A default il Title di queste pagine
verrà generato secondo la seguente struttura:

***{pageName} - {siteName}***

**Formato Title per Pagina Catalogo:** consente di definire la struttura
del Title che dovrà essere generato per le pagine Catalogo, (pagine
azzurre). A default il Title di queste pagine verrà generato secondo la
seguente struttura:

***{categoryName} - {siteName}***

**Formato Title per Pagina Prodotto:** consente di definire la struttura
del Title che dovrà essere generato per le pagine Prodotto, (pagine
rosse). A default il Title di queste pagine verrà generato secondo la
seguente struttura:

***{productName} - {categoryName} - {siteName}***

**Formato Title per Pagina CMS:** consente di definire la struttura del
Title che dovrà essere generato per le pagine utilizzate per la lettura
del dettaglio di un articolo o di un post CMS. A default il Title di
queste pagine verrà generato secondo la seguente struttura:

***{articleName} - {pageName} - {siteName}***

