# COMPONENTI E-COMMERCE -- NAVIGAZIONE PRODOTTI



Il Componente **"Navigazione Prodotti"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_navigazione_prodotti_res.bmp](./assets/media/image542.png){width="2.5395833333333333in"
height="3.1166666666666667in"}

può essere inserito solo ed esclusivamente all'interno del componente
ecommerce di primo livello "**Scheda Prodotto**" e consente di inserire
all'interno di questa stessa scheda dei controlli per sfogliare il
catalogo passando da un articolo all'altro operando direttamente
all'interno dalla pagina prodotto e senza dover quindi tornare per forza
di cose al Catalogo Articoli.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\navigazione_prodotti.bmp](./assets/media/image543.png){width="5.165972222222222in"
height="3.607638888888889in"}

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\navigazione_prodotti_configurazione_res.bmp](./assets/media/image544.png){width="4.613194444444445in"
height="2.938888888888889in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Azione:** consente di definire l'azione da associare al componente
  in oggetto. E' possibile selezionare uno dei seguenti valori.

  - **Articolo Precedente:** selezionando questa opzione il pulsante
    inserito all'interno della pagina consentirà di accedere al prodotto
    immediatamente precedente a quello attualmente visualizzato

  - **Articolo Successivo:** selezionando questa opzione il pulsante
    inserito all'interno della pagina consentirà di accedere al prodotto
    immediatamente successivo a quello attualmente visualizzato

> **ATTENZIONE!** Il criterio di ordinamento sulla base del quale
> determinare il prodotto precedente e/o successivo a quello attualmente
> visualizzato è stabilito da quanto impostato per il successivo
> parametro "Tipo di Ordinamento"
>
> Nel caso in cui si stia visualizzando il primo articolo tra quelli
> presenti in catalogo (sempre secondo quello che è il criterio di
> ordinamento stabilito) il pulsante per accedere all'articolo
> precedente non verrà visualizzato. Allo stesso modo nel caso in cui si
> stia visualizzando l'ultimo articolo non verrà ovviamente visualizzato
> il pulsante per accedere a quello successivo.

- **Contesto:** consente di impostare quello che dovrà essere il
  contesto di navigazione fra le schede prodotto. E' possibile
  selezionare uno dei seguenti valori:

  - **Catalogo:** selezionando questa opzione la navigazione avverrà tra
    tutti gli articoli presenti in catalogo

  - **Categoria Merceologica:** selezionando questa opzione la
    navigazione avverrà solo ed esclusivamente tra gli articoli
    appartenenti alla stessa categoria merceologica.

> In queste condizioni quindi la navigazione terminerà nel momento in
> cui si dovesse raggiungere l'ultimo articolo presente nella categoria
> merceologica in esame senza poter quindi passare al primo articolo
> della categoria successiva.

La sezione "**Ordinamento Elenco**" consente invece di impostare il
criterio di ordinamento sulla base del quale determinare il prodotto
precedente e/o successivo a quello attualmente visualizzato.

Nello specifico dunque il parametro:

- **Tipo di Ordinamento:** consente di definire l'elemento sulla base
  del quale verrà poi stabilito l'ordinamento da seguire nel passaggio
  da un prodotto all'altro.

> E' possibile selezionare uno dei seguenti valori:

- **Articoli più venduti:** in queste condizioni l'articolo
  precedente/successivo a quello attualmente visualizzato sarà il
  precedente/successivo nell'insieme degli articoli più venduti.

> Il successivo campo "**Periodo**" consente di impostare anche uno
> specifico periodo temporale da utilizzare nella definizione degli
> articoli più venduti (es. articoli più venduti dell'ultimo mese)

- **Articoli più visti:** in queste condizioni l'articolo
  precedente/successivo a quello attualmente visualizzato sarà il
  precedente/successivo nell'insieme degli articoli più visti.

> Il successivo campo "**Periodo**" consente di impostare anche uno
> specifico periodo temporale da utilizzare nella definizione degli
> articoli più visti (es. articoli più visti dell'ultimo mese)

- **Attributo Articolo:** selezionando questa opzione sarà poi possibile
  specificare dal sottostante menu a tendina ("**Attributo di
  Ordinamento**") l'Attributo Articolo (sia esso di tipo Passweb, sia
  esso di tipo Mexal) che dovrà essere utilizzato per definire
  l'ordinamento degli articoli.

- **Campo Articolo:** selezionando questa opzione sarà poi possibile
  specificare dal sottostante menu a tendina ("**Campo di
  Ordinamento**") lo specifico campo del gestionale che dovrà essere
  utilizzato per definire l'ordinamento degli articoli

<!-- -->

- **Modo di Ordinamento:** permette di definire se l'ordinamento
  definito mediante il precedente parametro dovrà essere di tipo
  Crescente o Decrescente

**ATTENZIONE! Al fine di creare un sistema di navigazione coerente tra
le varie schede prodotto è necessario, ovviamente, impostare lo stesso
criterio di navigazione sia per il pulsante "Precedente" che per quello
"Successivo"**

La sezione "Immagini" consente infine di associare una specifica
immagine al relativo controllo di navigazione

Nello specifico dunque il parametro:

- **Immagine:** permette di selezionare l'immagine che dovrà essere
  associata al controllo di navigazione in esame.

- **Immagine Rollover:** permette di selezionare l'eventuale immagine
  alternativa che apparirà al passaggio del mouse sul controllo in
  esame.

> Il pulsante "**Applica impostazione Immagine alle altre Lingue**",
> presente in corrispondenza di ciascuno dei due campi sopra indicati,
> consente di utilizzare automaticamente l'immagine indicata per tutte
> le lingue attualmente gestite all'interno del sito

**ATTENZIONE!** Le immagini da associare ai controlli di navigazione non
sono dati obbligatori

Nel momento in cui, dunque, si dovesse decidere di non utilizzare alcuna
immagine, all'interno dei controlli di navigazione verranno visualizzati
i testi indicati alla pagina "Gestione Testi / Messaggi del sito"
(sezione "Testi dei Componenti") in corrispondenza del componente
"**Navigatore Prodotti**"

