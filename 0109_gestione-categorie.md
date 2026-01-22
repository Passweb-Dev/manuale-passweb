# GESTIONE CATEGORIE



La pagina **"Categorie"** accessibile dalla voce di menu ***"Sito --
Gestione CMS"*** consente di creare e definire l'insieme di argomenti
mediante i quali poter poi categorizzare le notizie pubblicate
all'interno del sito.

Come evidenziato nel precedente capitolo di questo manuale infatti, ad
ogni singola notizia, ad ogni singolo post pubblicato all'interno del
sito potranno essere associate una o più Categorie di News.

**NOTA BENE**: per maggiori informazioni relativamente a come associare
una o più categorie di News ai singoli post si veda anche il precedente
capitolo di questo manuale.

In quest'ottica dunque i post con contenuti sportivi potrebbero, ad
esempio, essere associati ad un'apposita categoria Sport, mentre le
notizie di tecnologia potrebbero essere associate alla corrispondente
categoria "Tecnologia".

I componenti CMS disponibili in Passweb, consentiranno poi di sfruttare
queste associazioni in diversi modi, dando all'utente, ad esempio, la
possibilità di generare dei menu di categoria attraverso i quali poter
filtrare e ricercare all'interno del sito solo le notizie di uno
specifico argomento o ancora dando all'utente la possibilità di
pubblicare, ad esempio, in una pagina del sito una "Lista News" tematica
contenente cioè i soli post appartenenti alla categoria Sport e in
un'altra pagina un'altra lista contenenti invece i soli post della
categoria "Tecnologia"

All'interno della pagina "Categorie" verrà quindi visualizzata la
maschera **"Gestione CMS -- Categorie"**

![](./assets/media/image544.png)

contenente l'elenco di tutte le categorie attualmente codificate
all'interno del sito e organizzate secondo una ben precisa struttura
gerarchica sviluppata su N distinti livelli.

In particolare nella parte sinistra della maschera verranno
visualizzate, organizzate secondo la loro struttura gerarchica le varie
categorie di news, mentre nella parte destra verranno visualizzate le
caratteristiche e le proprietà della categoria attualmente selezionata
all'interno dell'albero.

I pulsanti presenti nella contestuale barra degli strumenti consento
rispettivamente di:

**Elimina** (
![](./assets/media/image347.png) ): consente di eliminare la categoria
attualmente selezionata all'interno dell'albero.

**NOTA BENE**: l'eliminazione di una categoria di News causerà solo ed
esclusivamente l'eliminazione delle eventuali associazioni a questa
categoria dei vari post pubblicati all'interno del sito. In nessun caso
l'eliminazione di una categoria causerà la cancellazione dei post ad
essa associati.

**Nuova**
(![](./assets/media/image545.png) ): consente di creare e definire una
nuova categoria di News. Cliccando su questo pulsante verrà quindi
visualizzata, nella parte destra della finestra, la maschera "**Nuova
Categoria Contenuto**"

![](./assets/media/image546.png)

all'interno della quale poter definire le caratteristiche e le proprietà
della categoria di News che si intende realizzare.

In particolare sarà necessario indicare un valore per i seguenti
parametri:

- **Codice (non obbligatorio):** consente di impostare un codice di
  integrazione (alfanumerico) che verrà poi utilizzato nelle procedure
  di creazione / modifica massiva di contenuti CMS per associare i
  singoli post alla categoria in esame

> **ATTENZIONE!** Il campo "**Codice**" non è di per se obbligatorio ma
> lo diventa nel momento in cui i contenuti CMS debbano poi poter essere
> associati automaticamente a determinate categorie nelle procedure di
> importazione massiva via csv
>
> In questo senso è bene ricordare anche che l'associazione di un post
> ad una categoria per cui è stata correttamente definita una specifica
> pagina di lettura può anche essere, dipendentemente dalle impostazioni
> settate per il parametro "**Formato Permalink Contenuti CMS**" (pagina
> "**Sito -- Preferenze**" del Wizard, tab "**SEO**" sezione
> "**Permalink**"), una condizione obbligatoria per la corretta
> visualizzazione del post sul front end del sito.
>
> Per maggiori informazioni in merito alle procedure di export / import
> di contenuti CMS si veda anche quanto indicato all'interno del
> precedente capitolo "*Importazione / Esportazione massiva di contenuti
> CMS*" di questo manuale

- **Nome:** consente di specificare, in tutte le lingue gestite
  all'interno del sito, il nome della categoria di News che si sta
  codificando.

- **Descrizione:** consente di associare alla categoria di News che si
  sta realizzando una specifica descrizione.

- **Immagine:** consente di associare alla categoria in oggetto una
  specifica immagine che potrà poi essere visualizzata all'interno del
  componente "Risultati di Ricerca sul Sito" nel momento in cui
  eventuali post CMS che dovessero soddisfare i criteri di ricerca
  impostati non avessero una specifica Immagine del Sommario.

- **Nascondi categoria sul sito:** se selezionato, questo parametro,
  consente di nascondere la corrispondente categoria all'interno del
  sito, considerandola a tutti gli effetti, dunque, come una Categoria
  Logica.

**NOTA BENE**: per maggiori informazioni relativamente alle Categorie
Logiche, a che cosa sono e a che cosa consentono di realizzare si veda
anche il successivo capitolo di questo manuale.

> Le Categorie Nascoste, o Logiche, comunque le si voglia chiamare
> verranno evidenziate in grigio all'interno dell'albero.

![](./assets/media/image547.png)

- **Pagina Categoria (opzionale):** per poter sfruttare appieno tutte le
  potenzialità della componentistica CMS messa a disposizione da
  Passweb, sarà indispensabile gestire all'interno del sito, almeno una
  pagina "Dettaglio" e una pagina "Archivio" in cui inserire i
  corrispondenti componenti CMS.

> La prima (pagina Dettaglio) consentirà infatti di visualizzare il
> dettaglio delle varie notizie selezionate dall'utente all'interno del
> sito. In questo senso, volendo sarebbe possibile gestire anche solo
> un'unica pagina di questo tipo, in cui inserire cioè il componente
> "Dettaglio News", in quanto il contenuto di questo componente varierà
> poi in maniera dinamica ed in base alla specifica notizia di cui
> l'utente del sito a richiesto di visualizzare il dettaglio (in
> sostanza potremmo tranquillamente paragonare la pagina dettaglio CMS
> alla pagina Prodotto di un sito e-commerce).
>
> La seconda (pagina Archivio) consentirà invece di gestire, attraverso
> il corrispondente componente "Archivio News" un vero e proprio
> archivio di tutte le notizie pubblicate all'interno del sito.
>
> Fatta questa premessa va ora detto che il parametro **"Pagina
> Categoria"** consente di associare alla categoria che si sta
> realizzando una specifica pagina del sito all'interno della quale
> poter poi collocare un componente "Archivio News" che filtrerà in
> automatico tutti i post appartenenti a quella specifica categoria.
>
> In questo modo sarà quindi possibile utilizzare pagine archivio
> diverse, magari anche con grafiche differenti, per le differenti
> categorie di News.
>
> **I tab presenti nella parte alta di questa sezione consentono di
> definire una specifica pagina di Categoria per ogni singola Variante
> Sito Gestita.**

![](./assets/media/image548.png)

> Nel caso in cui, per una certa Variante Sito, non dovesse essere
> associata alla categoria in oggetto una corrispondente pagina di
> categoria per essa verrà utilizzata la pagina Archivio "generale" di
> quella stessa Variante

- **Pagina di Lettura (opzionale):** consente di indicare una specifica
  pagina da utilizzare come pagina di lettura per le notizie
  appartenenti alla categoria in oggetto.

> Anche in questo caso è possibile definire una specifica Pagina di
> Lettura per ogni singola Variante Sito gestita.

**NOTA BENE**: è necessario inserire all'interno della pagina indicata
come "Pagina di Lettura" per la categoria il componente "Dettaglio News"
(in caso contrario non sarà possibile visualizzare il contenuto della
news selezionata).

