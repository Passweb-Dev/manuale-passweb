# SEO -- TITOLO ARTICOLO



La sezione "**Titolo Articolo**", presente all'interno del menu
**"Preferenze --SEO"** consente di definire il tipo di dato che dovrà
essere utilizzato per gestire il "Titolo" degli articoli presenti
all'interno del sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\seo_titolo_articolo.bmp](./assets/media/image34.png)

**ATTENZIONE!** il dato utilizzato per gestire il Titolo degli articoli
definisce l'informazione che verrà poi visualizzata sul front end del
sito all'interno del componente Ecommerce "Titolo"

E' possibile selezionare una delle seguenti opzioni:

- **Descrizione Gestionale:** in queste condizioni il "Titolo"
  dell'Articolo verrà creato sulla base della Descrizione impostata per
  i singoli prodotti all'interno del corrispondente campo (Descrizione)
  della loro anagrafica gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_descrizione_articolo_mexal.bmp](./assets/media/image35.png)

> **ATTENZIONE! Per i siti multilingua collegati a Mexal la Descrizione
> in Italiano, utilizzata per generare il Titolo dell'articolo, potrebbe
> anche NON essere inserita nel campo "Descrizione" dell'Anagrafica
> Articolo ma bensì in uno dei campi relativi alle lingue aggiuntive
> gestite in Mexal stesso.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lingue_aggiuntive_italiano.bmp](./assets/media/image36.png)

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lingue_aggiuntive_italiano2.bmp](./assets/media/image37.png)

> Nel caso in cui non dovesse essere effettuato questo tipo di Mapping
> il Titolo degli Articoli verrà generato sempre e soltanto sulla base
> del campo Descrizione presente in Anagrafica Articolo.
>
> Per maggiori informazioni relativamente alla gestione delle lingue
> estere in Mexal e sul corrispondente sito Passweb si veda anche la
> sezione "*Configurazione Gestionale -- Parametri Paese Lingua e Valuta
> -- Gestione Lingua*" di questo manuale.

- **Codice:** in queste condizioni il "Titolo" dell' Articolo verrà
  creato sulla base del Codice ad esso assegnato all'interno del
  gestionale

- **Attributo Gestionale (solo siti Ecommerce collegati a Mexal):** in
  queste condizioni il "Titolo" dell' Articolo verrà creato sulla base
  del valore assunto, per ogni singolo prodotto, dall'Attributo Mexal
  indicato all'interno del campo "Attributo da utilizzare"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\titolo_attributo_mexal.bmp](./assets/media/image38.png)

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\titolo_attributo_mexal_multilingua.bmp](./assets/media/image39.png)

- in fase di creazione dell' Attributo articolo in Passweb, mappare
  ciascuna delle lingue gestite con il corrispondente campo Mexal creato
  al punto precedente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\titolo_attributo_mexal_multilingua2.bmp](./assets/media/image40.png)

- **Passweb:** selezionando questa opzione il "Titolo" dell' Articolo
  verrà creato sulla base di quanto inserito all'interno del campo
  "Titolo" presente nell' Anagrafica Passweb di ogni singolo prodotto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\permalink_passweb.bmp](./assets/media/image41.png)

> **ATTENZIONE!** A differenza dei siti Ecommerce collegati ad uno dei
> gestionali Ho.Re.Ca. dove il campo "Titolo" dell'Anagrafica Passweb è
> sempre modificabile, nel caso di siti collegati a Mexal il campo in
> oggetto sarà modificabile solo ed esclusivamente nel momento in cui si
> sia scelto di gestire il titolo utilizzando come tipo di dato
> l'opzione "Passweb".
>
> In queste condizioni, ovviamente, oltre a poter variare manualmente il
> Titolo di ogni singolo articolo dalla sua Anagrafica Passweb, sarà
> anche possibile effettuare una valorizzazione massiva mediante
> l'import di un file csv correttamente strutturato. Per maggior
> informazioni relativamente all'importazione massiva di dati articolo
> tramite file si veda anche la sezione "*Catalogo -- Gestione Articoli
> -- Articoli -- Anagrafica Articolo / Servizio -- Importazione /
> Esportazione dei dati articoli tramite file*" di questo manuale

Ovviamente nel momento in cui, per una qualsiasi ragione, il campo
impostato per il parametro in oggetto dovesse essere privo di valori,
allo stesso modo anche il componente "Titolo" risulterà vuoto.

Analogamente se il campo impostato per il parametro in oggetto dovesse
assumere per due o più articoli lo stesso valore, anche il componente
Titolo sarà valorizzato, per i prodotti in questione, allo stesso modo.

**ATTENZIONE! Un' eventuale modifica alle impostazioni del campo in
oggetto non comporta, di per sé, nessuna variazione al Titolo degli
articoli.**

**In generale dunque, per fare in modo che le nuove impostazioni abbiano
effetto è necessario eseguire una Sincronizzazione Totale a seguito
della quale il Titolo verrà correttamente aggiornato sulla base delle
nuove impostazioni settate.**

