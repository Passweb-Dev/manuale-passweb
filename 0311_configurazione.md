# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_html_configurazione_res.bmp](./assets/media/image170.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**HTML:** l'editor presente all'intero di questa sezione consente di
inserire nella pagina del codice HTML personalizzato. In fase di
inserimento del codice HTML è possibile utilizzare i seguenti
segnaposto:

- **Codice Articolo -- {{SKU}}** -- utilizzabile all'interno di
  componenti come il "Catalogo Ecommerce" o la "Scheda Prodotto". Verrà
  sostituito a runtime con il codice del relativo prodotto

- **Codice Categoria Merceologica** -- {{**CATEGORYCODE**}} --
  utilizzabile nelle Pagine di Categoria. Verrà sostituito a runtime con
  il codice della corrispondente categoria merceologica

- **Elenco codici articolo in carrello** -- **{{PRODUCTSCODECART}}** --
  utilizzabile nella Pagina Carrello. Verrà sostituito a runtime con un
  array di stringhe relative ai codici articolo attualmente presenti in
  carrello

- **Codice Cliente -- {{CUSTOMERCODE}} --** può essere utilizzato in una
  qualsiasi pagina del sito. Verrà sostituito a runtime con il codice
  gestionale dell'utente attualmente loggato sul sito. Ovviamente nel
  momento in cui l'utente non avesse ancora effettuato l'autenticazione
  il segnaposto non conterrà alcun valore

- **ID post CMS -** {{**IDCMSPOST**}} -- utilizzabile nella pagina di
  visualizzazione del dettaglio dei post CMS all'interno del componente
  "Dettaglio News". Verrà sostituito a runtime con il codice del
  relativo post CMS

- **Nominativo Cliente - {{CUSTOMERNAME}}:** può essere utilizzato in
  una qualsiasi pagina del sito. Verrà sostituito a runtime con il
  nominativo dell'utente attualmente loggato sul sito. Ovviamente nel
  momento in cui l'utente non avesse ancora effettuato l'autenticazione
  il segnaposto non conterrà alcun valore

- **Email Cliente - {{USEREMAIL}}:** può essere utilizzato in una
  qualsiasi pagina del sito. Verrà sostituito a runtime con l'indirizzo
  mail dell'utente attualmente loggato sul sito. Ovviamente nel momento
  in cui l'utente non avesse ancora effettuato l'autenticazione il
  segnaposto non conterrà alcun valore

- **Data Ultima sincronizzazione -- {{SYNCAV}} --** può essere
  utilizzato in una qualsiasi pagina del sito. Verrà sostituito a
  runtime con la data dell'ultima sincronizzazione

- **URL Pagina -- {{URI}} --** può essere utilizzato in una qualsiasi
  pagina del sito. Verrà sostituito a runtime con l' url della pagina in
  cui è stato inserito

- **Zona Spedizione -** **{{ZONE}} --** può essere utilizzato in una
  qualsiasi pagina del sito. Verrà sostituito a runtime con i dati
  relativi alla zona di spedizione merce attualmente considerata
  dall'applicativo, dati questi che potranno variare in relazione al
  fatto che l'utente abbia o meno effettuato l'autenticazione al sito
  e/o abbia indicato in carrello o in checkout uno specifico indirizzo
  di spedizione.

> Per alcuni esempi di utilizzo del segnaposto in questione si consiglia
> di fare riferimento ai seguenti capitoli di questo manuale
>
> *"Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componenti
> interni ai Componenti Ecommerce -- Spedizione -- Visualizzazione dei
> costi di spedizione"*
>
> *"Ordini -- Tasse -- One Stop Shop (OSS)"*

Per inserire uno dei suddetti segnaposto è sufficiente posizionare il
cursore nell'esatta posizione in cui deve essere inserito, cliccare poi
sul pulsante "**Seleziona un segnaposto**" e selezionare l'elemento
desiderato dal relativo menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_html_configurazione_segnaposto_res.bmp](./assets/media/image171.png)

In alternativa è possibile inserire il segnaposto stesso anche inserendo
direttamente il relativo codice (es. {{SKU}})

**ATTENZIONE! nel caso di siti in multilingua il codice HTML dovrà
essere inserito specificatamente per ogni singola lingua gestita.**

Nell'editor HTML sono attivi inoltre, i seguenti tasti funzione:

- **Ctrl + F / Cmd + F** Consente di abilitare la funzione di ricerca
  all'interno dell'editor di codice HTML, attivando il relativo campo di
  testo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_mirror_ricerca.bmp](./assets/media/image172.png)

- **Ctrl + G / Cmd + G**: Consente, una volta effettuata una specifica
  ricerca all'interno dell'editor di codice HTML, di attivare la
  funzione "**Passa al successivo**"

- **Shift + Ctrl + G / Shift + Cmd + G** : Consente, una volta
  effettuata una specifica ricerca all'interno dell'editor di codice
  HTML, di attivare la funzione "**Passa al precedente**"

- **Shift + Ctrl + F / Cmd + Option + F**: Consente di attivare la
  funzione di "**Cerca e sostituisci**".

- Utilizzando questa combinazione di tasti verrà quindi visualizzato un
  primo campo di input in cui inserire il testo da ricercare (campo
  "Replace")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_mirror_cerca_sostituisci.bmp](./assets/media/image173.png)

> Una volta inserito il testo desiderato sarà necessario premere il
> tasto "Invio" in maniera tale da visualizzare un nuovo campo di input
> (campo "With") in cui inserire il nuovo testo che dovrà essere
> sostituito a quello precedentemente ricercato.

![Videate\\code_mirror_cerca_sostituisci_2.bmp](./assets/media/image174.png)

> Infine premendo nuovamente il taso invio verranno visualizzate tutte
> le possibili opzioni di sostituzione

![Videate\\code_mirror_cerca_sostituisci_3.bmp](./assets/media/image175.png)

- **Shift + Ctrl + R / Shift + Cmd + Option + F** : Consente di attivare
  la funzione di "**Cerca e sostituisci tutto**".

- **Alt + F**: Consente di attivare la funzione di ricerca
  "persistente".

> In queste condizioni nel caso in cui il testo ricercato dovesse
> presentare più occorrenze sarà possibile passare all'elemento
> successivo / precedente utilizzando rispettivamente i tasti
> "**Invio**" e "**Shift + Invio**"

- **Alt + G**: Consente di attivare la funzione "**Vai alla linea**".

> Utilizzando questa combinazione di tasti verrà quindi visualizzato un
> campo di input in cui inserire il numero di riga (ed eventualmente
> anche quello di colonna) in corrispondenza del quale spostare il
> cursore

Il pulsante "**Aggiungi Attributo Tema**" consente di aggiungere al
proprio codice HTML uno degli attributi associati al tema attualmente
gestito.

Per maggiori informazioni in merito alla gestione dei Temi si rimanda al
relativo capitolo di questo manuale ("*Live Editing per Varianti
Responsive -- Temi*" )

Per operare in modalità full screen utilizzare il tasto funzione
**"F11"**. Per tornare alla modalità di visualizzazione di default
utilizzare il tasto ESC

**ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
utilizzare il componente HTML per creare dei link a specifiche sezioni
dell' Area Riservata, sarà necessario utilizzare come valore
dell'attributo href appositi segnaposto. Per maggiori informazioni in
merito si veda anche la sezione "*Live Editing per Varianti Responsive
-- Contenuti -- Editor dei Contenuti Inserimento Link -- Link all'Area
Riservata*" di questo manuale.

Appositi segnaposto andranno utilizzati anche nel momento in cui
l'esigenza dovesse essere quella di utilizzare il componente HTML per
realizzare link a specifici prodotti e/o a specifici articoli CMS. In
questo senso si consiglia sempre di visualizzare il codice sorgente
generato in automatico da Passweb realizzando, ad esempio mediante un
componente Paragrafo, il relativo link.

> **NOTA BENE:** non utilizzare tag strutturali quali \<body\> \<head\>
> all'interno di un componente HTML. L'utilizzo di questi tag
> all'interno di un componente HTML potrebbe infatti compromettere il
> corretto e normale funzionamento di Passweb.

Il pulsante '**Salva**' presente nella parte alta della maschera
consentirà di salvare tutte le modifiche apportate al componente in
oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

