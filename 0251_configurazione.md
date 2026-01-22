# CONFIGURAZIONE



Una volta inserito il **componente** all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-paragrafo-modcontenuto_res.bmp](./assets/media/image2.png){width="5.136111111111111in"
height="3.1430555555555557in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà poi possibile
inserire il contenuto e settare i principali parametri di configurazione
del componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Caricamento Javascript** e **Statico** si veda anche quanto indicato
> all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Staticizzazione e caricamento
> asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

- **Contenuto** consente di inserire, mediante l'apposito editor HTML,
  il contenuto vero e proprio del paragrafo che si intende inserire
  all'interno della pagina web.

> Il pulsante "**Aggiungi segnaposto**" situato immediatamente al di
> sotto del campo, consente di inserire nel relativo paragrafo uno dei
> segnaposto gestiti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_paragrafo_segnaposto.bmp](./assets/media/image3.png){width="4.402777777777778in"
height="3.0972222222222223in"}

- **Codice Articolo -- {{SKU}}** -- da utilizzare all'interno di
  componenti come il "Catalogo Ecommerce" o la "Scheda Prodotto". Verrà
  sostituito a runtime con il codice del relativo prodotto

- **Codice Cliente -- {{CUSTOMERCODE}} --** può essere utilizzato in una
  qualsiasi pagina del sito. Verrà sostituito a runtime con il codice
  gestionale dell'utente attualmente loggato sul sito. Ovviamente nel
  momento in cui l'utente non avesse ancora effettuato l'autenticazione
  il segnaposto non conterrà alcun valore

- **Data Ultima sincronizzazione -- {{SYNCAV}} --** può essere
  utilizzato in una qualsiasi pagina del sito. Verrà sostituito a
  runtime con la data dell'ultima sincronizzazione

- **Nominativo Cliente - {{CUSTOMERNAME}}:** può essere utilizzato in
  una qualsiasi pagina del sito. Verrà sostituito a runtime con il
  nominativo dell'utente attualmente loggato sul sito. Ovviamente nel
  momento in cui l'utente non avesse ancora effettuato l'autenticazione
  il segnaposto non conterrà alcun valore

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
>
> Per maggiori informazioni relativamente all'utilizzo di questo editor
> HTML si veda anche il relativo capitolo *("Live Editing per Varianti
> Responsive -- Contenuti -- Editor dei contenuti"*) di questo manuale.

- **Considera nel feed pagine: richiede attivazione su Passstore del
  modulo Clerk**

> Consente di inserire il contenuto del paragrafo in esame all'interno
> del feed delle pagine utilizzato per l'integrazione Passweb -- Clerk.
> Per maggiori informazioni relativamente al modulo Clerk e
> all'integrazione tra Passweb e questa piattaforma si rimanda a quanto
> indicato all'interno del capitolo "*Passweb e Clerk*" di questo
> manuale

- **Immagine** consente di associare al contenuto testuale, inserito
  mediante l'apposito editor, anche una specifica immagine.

> Cliccando sul pulsante "**Seleziona la Risorsa**" verrà aperta la
> maschera di "Gestione delle Risorse" attraverso la quale poter
> selezionare un'immagine, tra quelle già presenti nel database del
> sito, oppure aggiungerne di nuove attraverso l'upload delle relative
> risorse.
>
> Per maggiori informazioni relativamente alla gestione delle risorse
> grafiche all'interno di un sito Passweb si veda anche il relativo
> capitolo (*"Live Editing per Varianti Responsive -- Gestione Risorse
> del sito"*) di questo manuale.
>
> In ogni caso è sempre possibile inserire una o più immagini
> contestuali al testo del paragrafo utilizzando le apposite funzioni
> presenti all'interno dell'editor HTML
>
> In alternativa è anche possibile è possibile utilizzare come immagine
> un apposito Attributo precedentemente codificato all'interno della
> relativa sezione del Wizard.
>
> In questo senso il menu a tendina presente in corrispondenza del
> parametro "**Attributi Temi**" consente di selezionare, tra quelli
> presenti in elenco, lo specifico Attributo di tipo Immagine da
> utilizzare per il componente in questione
>
> **ATTENZIONE!** I campi "**Seleziona Risorsa**" e "**Seleziona
> Attributo Tema**" sono alternativi per cui l'immagine può essere
> inserita **o** manualmente selezionandola dal database delle risorse
> del sito **oppure** selezionando il relativo Attributo
>
> Per maggiori informazioni in merito alla creazione e alla gestione
> degli Attributi e dei Temi si veda anche la relativa sezione di questo
> manuale ("*Live Editing per Varianti Responsive - Temi*")
>
> Il pulsante "**Applica impostazione Immagine alle altre Lingue**"
> consente di utilizzare automaticamente l'immagine indicata per tutte
> le lingue attualmente gestite all'interno del sito

- **Testo Alternativo (per accessibilità):** consente di associare una
  descrizione aggiuntiva all\'immagine, fondamentale per la reperibilità
  sui motori di ricerca (es. Google Immagini) e per soddisfare la
  vigente normativa in materia di accessibilità (es. browser per non
  vedenti).

Una volta impostati i parametri richiesti il pulsante salva presente
nella parte bassa della maschera consentirà di salvare il componente in
oggetto inserendolo di fatto all'interno della pagina web.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

