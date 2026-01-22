# SEO -- PERMALINK ARTICOLO



La sezione "**Permalink Articolo**", presente all'interno del menu
**"Preferenze --SEO"** consente di definire il tipo di dato che dovrà
essere utilizzato per gestire il "Permalink" degli articoli presenti
all'interno del sito.

![](./assets/media/image42.png)

**ATTENZIONE! Il dato utilizzato per gestire il "Permalink" degli
articoli è di fondamentale importanza anche e soprattutto in ottica SEO
in quanto questo andrà poi a definire la parte finale dell' url delle
relative Pagine Prodotto**

E' possibile selezionare una delle seguenti opzioni:

- **Descrizione Gestionale:** in queste condizioni il "Permalink" dell'
  Articolo verrà creato sulla base della Descrizione impostata per i
  singoli prodotti all'interno del corrispondente campo (Descrizione)
  della loro anagrafica gestionale

![](./assets/media/image35.png)

> **ATTENZIONE! Per i siti multilingua collegati a Mexal la Descrizione
> in Italiano, utilizzata per generare il Permalink dell'articolo,
> potrebbe anche NON essere inserita nel campo "Descrizione"
> dell'Anagrafica Articolo ma bensì in uno dei campi relativi alle
> lingue aggiuntive gestite in Mexal stesso.**

![](./assets/media/image36.png)

> Una scelta di questo tipo potrebbe rivelarsi particolarmente utile in
> quanto consentirebbe di definire, direttamente all'interno del
> gestionale e senza il bisogno di creare apposite videate aggiuntive,
> una descrizione articolo "SEO Friendly" che ben si sposa cioè con
> quelle che possono essere esigenze tipicamente web lasciando
> inalterata la "Descrizione principale" nell'Anagrafica Articolo che,
> al contrario, potrebbe invece essere stata creata secondo altre
> logiche puramente gestionali che poco anche a che vedere con il
> posizionamento di una pagina web.
>
> **ATTENZIONE! Per adottare questa soluzione è necessario aver mappato
> in "*Configurazione -- Parametri Paese, Lingua e Valuta -- Gestione
> Lingua*" del Wizard anche la lingua Italiana con una delle lingue
> "Extra" abilitate e gestite all'interno del gestionale**

![](./assets/media/image37.png)

> Nel caso in cui non dovesse essere effettuato questo tipo di Mapping
> il Permalink degli Articoli verrà generato sempre e soltanto sulla
> base del campo Descrizione presente in Anagrafica Articolo.
>
> Per maggiori informazioni relativamente alla gestione delle lingue
> estere in Mexal e sul corrispondente sito Passweb si veda anche la
> sezione "*Configurazione Gestionale -- Parametri Paese Lingua e Valuta
> -- Gestione Lingua*" di questo manuale.

- **Codice:** in queste condizioni il Permalink dell' Articolo verrà
  creato sulla base del Codice ad esso assegnato all'interno del
  gestionale

- **Attributo Gestionale (solo siti Ecommerce collegati a Mexal):** in
  queste condizioni il Permalink dell' Articolo verrà creato sulla base
  del valore assunto, per ogni singolo prodotto, dall'Attributo Mexal
  indicato all'interno del campo "Attributo da utilizzare"

![](./assets/media/image43.png)

> **ATTENZIONE! All'interno del campo "Attributo da utilizzare" verranno
> visualizzati solo ed esclusivamente Attributi Articolo di tipo Mexal**
>
> Per maggiori informazioni relativamente alla creazione e alla gestione
> degli Attributi Articolo in Passweb si veda anche la relativa sezione
> ( *Catalogo -- Gestione Attributi* ) di questo manuale.
>
> Nel caso invece di siti in multilingua sarà necessario:

- creare uno specifico campo di una Videata Aggiuntiva Articoli Mexal
  per ciascuna delle lingue gestite all'interno del sito

![](./assets/media/image44.png)

- in fase di creazione dell' Attributo articolo in Passweb, mappare
  ciascuna delle lingue gestite con il corrispondente campo Mexal creato
  al punto precedente

<!-- -->

- **Passweb:** selezionando questa opzione il Permalink dell' Articolo
  verrà creato sulla base di quanto inserito all'interno del campo
  "Titolo" presente nell' Anagrafica Passweb di ogni singolo prodotto

![](./assets/media/image41.png)

> **ATTENZIONE!** A differenza dei siti Ecommerce collegati ad uno dei
> gestionali Ho.Re.Ca. dove il campo "Titolo" dell'Anagrafica Passweb è
> sempre modificabile, per siti collegati a Mexal il campo in oggetto
> sarà modificabile solo ed esclusivamente nel momento in cui si sia
> scelto di impostare anche il campo "Tipo di dato da Utilizzare"
> presente all'interno della sezione "Titolo Articolo" sull'opzione
> "Passweb".
>
> In queste condizioni, ovviamente, oltre a poter variare manualmente il
> Titolo di ogni singolo articolo dalla sua Anagrafica Passweb, sarà
> anche possibile effettuare una valorizzazione massiva mediante
> l'import di un file csv correttamente strutturato. Per maggior
> informazioni relativamente all'importazione massiva di dati articolo
> tramite file si veda anche la sezione "*Catalogo -- Gestione Articoli
> -- Articoli -- Anagrafica Articolo / Servizio -- Importazione /
> Esportazione dei dati articoli tramite file*" di questo manuale

E' bene inoltre sottolineare che nel momento in cui, per una qualsiasi
ragione, il campo impostato per il parametro in oggetto dovesse:

- avere lo stesso valore per due o più articoli, i rispettivi permalink
  verranno generati con un numero progressivo che ne assicuri
  l'univocità e renda comunque visibili, all'interno del sito, le
  relative pagine prodotto.

- essere privo di valori, verrà utilizzato come permalink per costruire
  l' url della relativa pagina prodotto l'ID Passweb del corrispondente
  articolo

**ATTENZIONE!** **un' eventuale modifica alle impostazioni del campo in
oggetto comporterà, al salvataggio della maschera, l'avvio di una
procedura (in background) di rigenerazione dei permalink di tutti i
prodotti attualmente presenti all'interno del sito.** Al termine della
procedura verrà inviata un'apposita mail all'amministratore con l'esito
dell'operazione

E' bene evidenziare inoltre, che eventuali modifiche ai permalink degli
articoli potrebbero incidere significativamente, ai fini SEO, sul
posizionamento delle relative pagine prodotto.

Modificando l' url delle pagina prodotto, infatti, potrebbero generarsi
diversi errori di tipo 404 (pagina non trovata) causati dalle vecchie
url precedentemente indicizzate, errori questi che, se non correttamente
gestiti, potrebbero pregiudicare il posizionamento del sito.

Nel momento in cui si dovesse, per qualche ragione, variare le
impostazioni di questo parametro, si consiglia quindi di creare i
corrispondenti Alias dalla relativa sezione del Wizard (*Sito --
Gestione Alias*) oppure di aver correttamente attivato la generazione
automatica degli Alias, lasciando quindi a Passweb il compito di gestire
questo tipo di variazioni.

Per maggiori informazioni relativamente alla generazione automatica
degli Alias si veda anche il successivo capitolo di questo manuale.

