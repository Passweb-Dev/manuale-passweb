# GESTIONE NEWSLETTER -- TEMPLATES



All'interno di questa sezione l'utente avrà la possibilità di
sincronizzare e configurare tutti i template precedentemente salvati
all'interno del proprio account MailChimp nella sezione "**Templates**"

![](./assets/media/image63.png)

Il pulsante **"Sincronizza da MailChimp"** presente nella barra degli
strumenti consente di effettuare la sincronizzazione tra il sito Passweb
ed il proprio account MailChimp **limitatamente ai soli template
presenti nella sezione "Templates"**

**NOTA BENE**: i template presenti in elenco riflettono ovviamente la
situazione aggiornata all'ultima sincronizzazione

Per ogni Template in elenco sono indicate le seguenti informazioni:

- **Stato:** indica lo stato del template e, conseguentemente, il fatto
  che possa o meno essere utilizzato all'interno di una campagna. Sono
  gestiti diversi stati:

  - **Sezioni da assegnare:** i template in questo stato presentano
    ancora delle sezioni da configurare e, eventualmente, da collegare
    ai contenuti CMS e/o ai prodotti gestiti e pubblicati all'interno
    del proprio sito.

> **ATTENZIONE! Un Template in queste condizioni non può essere
> utilizzato all'interno delle varie Campagne**

- **Sezioni Miste:** i template in questo stato presentano alcune
  sezioni configurate per prelevare automaticamente i contenuti da
  elementi non coerenti tra loro. Alcune sezioni possono essere state
  impostate, ad esempio, per prelevare contenuti da post CMS e altre per
  prelevare invece i contenuti da prodotti gestiti sul sito o da Liste
  Regalo.

> **ATTENZIONE! Un template in questo stato, pur essendo interamente
> configurato, non potrà essere utilizzato all'interno di nessuna
> Campagna**

- **Ok:** i template in questo stato sono stati correttamene configurati
  e potranno quindi essere utilizzati all'interno delle varie Campagne

<!-- -->

- **Tipologia:** indica la tipologia del relativo template. Le diverse
  tipologie sono definite in base a come sono state configurate le
  sezioni del template e a quelli che possono essere dunque i loro
  contenuti:

  - **CMS:** identifica un template in cui le sezioni effettivamente
    modificabili sono tutte di tipo **CMS** (prelevando quindi il
    contenuto in maniera automatica dai post pubblicati sul sito) e/o
    **Personalizzato** (con contenuti inseriti manualmente in fase di
    editing del template)

  - **Ecommerce:** identifica un template in cui le sezioni
    effettivamente modificabili sono tutte di tipo **Ecommerce**
    (prelevando quindi il contenuto in maniera automatica dai prodotti
    gestiti sul sito) e/o **Personalizzato** (con contenuti inseriti
    manualmente in fase di editing del template)

  - **GiftRegistry:** identifica un template in cui le sezioni
    effettivamente modificabili sono tutte di tipo **Lista Regalo**
    (prelevando quindi il contenuto in maniera automatica dai dati di
    una ben precisa Lista Regalo) e/o **Personalizzato** (con contenuti
    inseriti manualmente in fase di editing del template)

  - **Semplice:** identifica un template in cui le sezioni
    effettivamente modificabili sono solo di tipo **Personalizzato**
    (con contenuti inseriti manualmente in fase di editing del template)

- **Data:** indica la data di importazione del template

- **ID:** indica il codice identificativo del template.

**Al fine di poter utilizzare uno qualsiasi dei template in elenco per
inviare delle Campagne direttamente dal proprio sito Passweb, è
necessario, per prima cosa, configurare in maniera adeguata il Template
stesso definendo quelli che dovranno essere i contenuti delle sue
diverse sezioni.**

In questo senso occorre quindi avere sempre ben chiari alcuni concetti
di fondamentale importanza:

- Il layout del template (struttura, colori, immagini di sfondo ecc... )
  potrà essere modificato solo ed esclusivamente all'interno di
  MailChimp (per maggiori informazioni in merito a questo tipo di
  operazione si vedano anche i precedenti capitoli di questo manuale).

- Dipendentemente dal template selezionato, alcune delle immagini in
  esso presenti potranno essere variate solo ed esclusivamente
  all'interno di MailChimp mentre altre potranno essere personalizzate e
  gestite direttamente da Passweb.

- A seguito di ogni modifica apportata in MailChimp ad un template sarà
  necessario effettuare una nuova sincronizzazione in modo tale da
  riportare anche in Passweb le variazioni appena effettuate.

> **ATTENZIONE!** A seguito della sincronizzazione potrebbe essere
> necessario riconfigurare alcuni template

- Ogni template creato in MailChimp ha delle sezioni (**Section**) ben
  definite, proprie del template stesso. **E' all'interno di queste
  sezioni che andranno inseriti i vari contenuti della Newsletter,
  contenuti questi che potranno essere editati, in diversi modi,
  direttamente all'interno di Passweb.**

##### MODIFICA E CONFIGURAZIONE DI UN TEMPLATE

Prima di poter utilizzare uno dei Template importati da MailChimp
all'interno di una Campagna creata a partire dal proprio sito Passweb, è
indispensabile configurare correttamente il Template stesso in relazione
alla Tipologia di Campagna all'interno della quale dovrà poi essere
utilizzato.

In questo senso cliccando sul pulsante "**Modifica**" (
![](./assets/media/image64.png) ) presente nella barra degli strumenti
della tabella contenente l'elenco dei Template sincronizzati da
MailChimp, sarà possibile accedere alla maschera di configurazione del
Template attualmente selezionato.

![](./assets/media/image65.png)

- **Le sezioni del template non ancora configurate** verranno
  evidenziate da un riquadro con **bordo tratteggiato di colore blu**.

- **Le sezioni del template già configurate in maniera corretta**
  saranno invece evidenziate da un riquadro con **bordo tratteggiato di
  colore arancione**

- **Qualsiasi altro elemento che non rientri in una delle sezioni
  evidenziate all'interno del template potrà essere eventualmente
  modificato solo ed esclusivamente all'interno di MailChimp.**

Per poter configurare una delle sezioni del Template, definendo quindi
quelli che dovranno essere i suoi contenuti, è sufficiente posizionarsi
e cliccare col mouse sopra di essa. In questo modo verrà infatti aperta
la maschera **"Modifica Sezione Template"**

![](./assets/media/image66.png)

all'interno della quale poter appunto impostare i parametri di
configurazione della relativa sezione.

In particolare sarà necessario impostare un valore per i seguenti
parametri

**Nome Sezione (campo di sola visualizzazione):** all'interno di questo
campo verrà visualizzato, e non potrà in alcun modo essere modificato,
il nome reale della sezione in esame ereditato direttamente dalla
struttura del modello considerato.

**Nome Descrittivo:** consente di associare alla sezione in esame
un'etichetta identificativa, personalizzabile e quindi più semplice da
ricordare, per individuare all'interno del template la sezione in esame
rispetto a quanto non consenta di fare il nome reale di questa stessa
sezione

**Tipologia del Contenuto associato alla Sezione:** consente di definire
la tipologia dei contenuti che dovranno essere inseriti all'interno
della sezione in esame. E' possibile selezionare uno dei seguenti
valori:

- **Valore Personalizzato:** selezionando questa opzione il contenuto
  della sezione in **esame dovrà necessariamente essere inserito, in
  fase di invio della campagna, in maniera manuale attraverso un
  apposito Editor HTML** (lo stesso già utilizzato per i componenti
  Paragrafo di Passweb)

> In queste condizioni, inoltre, il campo **Contenuto di Default**
> consente di inserire, con lo stesso Editor HTML, dei contenuti che
> verranno poi proposti, a default, all'interno di questa stessa sezione
> del template in fase di creazione ed invio della Campagna

![](./assets/media/image67.png)

- **Valore di un campo CMS:** selezionando questa opzione il contenuto
  della sezione in esame verrà prelevato automaticamente da uno dei post
  CMS pubblicati all'interno del sito. In fase di invio della campagna
  non sarà quindi necessario editare manualmente questa sezione del
  template ma sarà sufficiente indicare lo specifico post CMS da cui
  prelevare il contenuto.

> Il successivo parametro **"Campo associato alla Sezione"**

![](./assets/media/image68.png)

> consente di indicare lo specifico elemento del post CMS da cui
> prelevare il contenuto da inserire all'interno della sezione. In
> questo senso è possibile selezionare uno dei seguenti elementi:

- **Titolo Articolo CMS:** selezionando questa opzione, il contenuto
  della relativa sezione verrà popolato automaticamente, in fase di
  creazione e invio della Campagna, con il Titolo dell'Articolo CMS
  collegato alla campagna stessa.

- **Sommario CMS:** selezionando questa opzione, il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il Sommario dell'Articolo CMS collegato
  alla campagna stessa.

- **Articolo CMS:** selezionando questa opzione, il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il Contenuto dell'Articolo CMS collegato
  alla campagna stessa.

- **Immagine Sommario CMS:** selezionando questa opzione, il contenuto
  della relativa sezione verrà popolato automaticamente, in fase di
  creazione e invio della Campagna, con l'"Immagine Sommario"
  dell'Articolo CMS collegato alla campagna stessa.

- **Immagine Articolo CMS:** selezionando questa opzione, il contenuto
  della relativa sezione verrà popolato automaticamente, in fase di
  creazione e invio della Campagna, con l'"Immagine Articolo"
  dell'Articolo CMS collegato alla campagna stessa.

> **NOTA BENE**: per maggiori informazioni relativamente alla
> possibilità di creare delle Campagne inviando Newsletter popolate in
> automatico con i contenuti degli articoli CMS gestiti e pubblicati
> all'interno del proprio sito Passweb, si veda anche il successivo
> capitolo di questo manuale (Gestione Newsletter - Campagne)

- **Valore di un campo Articolo:** selezionando questa opzione il
  contenuto della sezione in esame verrà prelevato automaticamente dai
  dati relativi ad uno dei prodotti gestiti all'interno del sito. In
  fase di invio della campagna non sarà quindi necessario editare
  manualmente questa sezione del template ma sarà sufficiente indicare
  lo specifico prodotto da cui prelevare le informazioni.

> Il successivo parametro **"Campo associato alla Sezione"**

![](./assets/media/image69.png)

> consente di indicare quale informazione relativa allo specifico
> prodotto dovrà essere prelevata ed inserita all'interno della sezione.
> In questo senso è possibile selezionare uno dei seguenti elementi:

- **Codice Prodotto:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con il Codice gestionale dello specifico prodotto
  collegato alla campagna stessa.

- **Titolo Prodotto:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con la Descrizione gestionale dello specifico prodotto
  collegato alla campagna stessa.

- **Categoria Merceologica Prodotto:** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con la Categoria Merceologica di appartenenza
  dello specifico prodotto collegato alla campagna stessa.

- **Codice Alternativo Prodotto:** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il Codice Alternativo impostato
  all'interno del gestionale per lo specifico prodotto collegato alla
  campagna stessa.

- **Categoria Statistica Prodotto:** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con la Categoria Statistica di appartenenza
  dello specifico prodotto collegato alla campagna stessa.

- **Natura Prodotto:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con la Natura associata all'interno del gestionale
  allo specifico prodotto collegato alla campagna stessa.

- **Taglia/Colore Prodotto::** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il valore della Taglia/Colore dello
  specifico prodotto collegato alla campagna stessa.

- **Descrizione HTML /2/3 Prodotto:** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il contenuto dei campi Descrizione HTML
  /2/3 relativi allo specifico prodotto collegato alla campagna stessa.

- **Attributi Passweb Prodotto:** in questo caso il contenuto della
  relativa sezione verrà popolato automaticamente, in fase di creazione
  e invio della Campagna, con il valore dello specifico attributo
  Passweb legato al prodotto collegato alla campagna stessa.

<!-- -->

- **Valore di un campo Lista Regalo:** selezionando questa opzione il
  contenuto della sezione in esame verrà prelevato automaticamente dai
  dati relativi alla Lista Regalo che sarà poi oggetto della campagna.

> In fase di invio della campagna non sarà quindi necessario editare
> manualmente questa sezione del template anche e soprattutto perché gli
> invii relativi a Campagne di tipo "Lista Regalo" (le uniche in cui
> poter utilizzare Template con sezioni configurate in questo modo)
> verranno create automaticamente nel momento in cui l'utente, creatore
> di una Lista Regalo, dovesse decidere di condividerla via mail.
>
> **ATTENZIONE!** Per campagne di tipo "Lista Regalo" gli invii verranno
> gestiti in maniera automatica dall'applicazione
>
> Il successivo parametro **"Campo associato alla Sezione"**

![](./assets/media/image70.png)

> consente di indicare quale informazione relativa alla specifica Lista
> Regalo dovrà essere prelevata ed inserita all'interno della sezione in
> esame.
>
> Le informazioni disponibili sono ovviamente quelle inserite, sul front
> end del sito, direttamente in fase di creazione della Lista Regalo dal
> creatore della lista stessa
>
> ![](./assets/media/image71.png)
>
> Nello specifico sarà quindi possibile selezionare uno dei seguenti
> elementi:

- **Titolo Evento:** in questo caso il contenuto della relativa sezione
  verrà popolato automaticamente, in fase di creazione e invio della
  Campagna, con il Titolo assegnato alla relativa Lista Regalo

- **Luogo Evento:** in questo caso il contenuto della relativa sezione
  verrà popolato automaticamente, in fase di creazione e invio della
  Campagna, con quanto inserito in fase di creazione della Lista Regalo
  all'interno del campo "Luogo Evento"

- **Data Evento:** in questo caso il contenuto della relativa sezione
  verrà popolato automaticamente, in fase di creazione e invio della
  Campagna, con quanto inserito in fase di creazione della Lista Regalo
  all'interno del campo "Data Evento"

- **Descrizione Evento:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con quanto inserito in fase di creazione della Lista
  Regalo all'interno del campo "Descrizione Evento"

- **Organizzatori Evento:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con quanto inserito in fase di creazione della Lista
  Regalo all'interno del campo "Organizzatori Evento"

- **Messaggio Evento:** in questo caso il contenuto della relativa
  sezione verrà popolato automaticamente, in fase di creazione e invio
  della Campagna, con quanto inserito, in fase di condivisione della
  Lista Regalo all'interno del campo "Inserisci il messaggio per i tuoi
  amici"

![Videate\\wl_lista_regalo_5.bmp](./assets/media/image72.png)

- **Link Evento:** in questo caso il contenuto della relativa sezione
  verrà popolato automaticamente, in fase di creazione e invio della
  Campagna con il link alla pagina del sito contenente la relativa lista
  regalo contente l'elenco dei prodotti che l'utente potrà acquistare

> **Per ovvie ragioni è di fondamentale importanza inserire, all'interno
> del Template, una sezione di questo tipo**
>
> In caso contrario infatti pur ricevendo la mail di invito l'utente non
> avrà a disposizione il link di accesso alla relativa Lista Regalo
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla gestione
> e alla condivisione delle Liste Regalo si veda anche la sezione
> "*Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componente
> Lista Regalo*" di questo manuale

**Ovviamente le sezioni modificabili all'interno di un Template possono
essere sezioni testuali ma anche sezioni contenenti solo ed
esclusivamente delle immagini.**

La procedura e la maschera di configurazione delle sezioni "Immagine"
sono esattamente analoghe a quanto appena analizzato. Cambieranno
ovviamente il tipo di dati da poter utilizzare per popolare la sezione.

Nello specifico impostando il campo **Tipologia del contenuto associato
alla sezione** su "**Valore Personalizzato**" il contenuto di default da
inserire non sarà più gestito con un editor HTML ma con un controllo di
tipo immagine

![](./assets/media/image73.png)

Allo stesso modo nel caso in cui il campo **Tipologia del contenuto
associato alla sezione** fosse impostato su "**Valore di un campo CMS**"
gli unici contenuti prelevabili dal post CMS saranno:

![](./assets/media/image74.png)

- **Immagine Sommario CMS:** selezionando questa opzione, l'immagine in
  esame verrà automaticamente sostituita, in fase di creazione e invio
  della Campagna, con l'"Immagine Sommario" dell'Articolo CMS collegato
  alla campagna stessa.

- **Immagine Articolo CMS:** selezionando questa opzione, l'immagine in
  esame verrà automaticamente sostituita, in fase di creazione e invio
  della Campagna, con l'"Immagine Articolo" dell'Articolo CMS collegato
  alla campagna stessa.

Nel caso in cui invece il campo **Tipologia del contenuto associato alla
sezione** fosse impostato su "**Valore di un campo Articolo**" gli unici
contenuti prelevabili da prodotto saranno:

![](./assets/media/image75.png)

- **Immagine Catalogo Prodotto:** selezionando questa opzione,
  l'immagine in esame verrà automaticamente sostituita, in fase di
  creazione e invio della Campagna, con l' Immagine del prodotto
  utilizzata all'interno del sito nel componente "Catalogo Ecommerce"

- **Immagine della Scheda Prodotto:** selezionando questa opzione,
  l'immagine in esame verrà automaticamente sostituita, in fase di
  creazione e invio della Campagna, con l'Immagine del prodotto
  utilizzata all'interno del sito nel componente "Scheda Prodotto"

Infine nel momento in cui il campo **Tipologia del contenuto associato
alla sezione** fosse impostato su "**Valore di un campo Lista Regalo"**
l'unico contenuto prelevabile dalla corrispondente lista regalo sarà il
seguente

![](./assets/media/image76.png)

- **Immagine Evento:** selezionando questa opzione, l'immagine in esame
  verrà automaticamente sostituita, in fase di creazione e invio della
  Campagna, con quanto inserito in fase di creazione della Lista Regalo
  all'interno del campo "Immagine Evento"

