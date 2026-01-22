# GESTIONE PROTEZIONE



All'interno della sezione "**Gestione Protezione**" attivabile cliccando
sulla corrispondente icona presente nella "Barra degli Strumenti del
Live Editing" o, in alternativa, sulla stessa icona presente anche
all'interno del menu principale

![Videate\\menu_protezione_barra_strumenti.bmp](./assets/media/image103.png)

![Videate\\menu_editing_gestione_protezione.bmp](./assets/media/image104.png)

è possibile gestire operazioni massive di diverso tipo.

Nello specifico sarà possibile, ad esempio:

- Attivare / disattivare la pubblicazione massiva di tutti i componenti
  di una determinata tipologia presenti all'interno di una specifica
  pagina piuttosto che all'interno dell'intero sito

- Gestire in maniera massiva la visibilità sul front end dei componenti
  di una determinata tipologia presenti all'interno di una specifica
  pagina piuttosto che all'interno dell'intero sito (rendendoli quindi
  visibili a tutti oppure solo a determinati Gruppi Utente)

- Settare in blocco i permessi di gestione dei componenti all'interno
  del Wizard

- Gestire in maniera massiva operazioni relative alla protezione e / o
  alla pubblicazione delle pagine del sito

- Gestire in maniera massiva, per tutti i componenti di una determinata
  tipologia presenti all'interno di una specifica pagina piuttosto che
  all'interno dell'intero sito, il parametro che consente di decidere se
  questi stessi componenti potranno o meno essere messi in cache

Cliccando su uno qualsiasi dei due pulsanti precedentemente evidenziati
verrà infatti visualizzata la maschera "**Gestione Protezione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione.bmp](./assets/media/image105.png)

all'interno della quale poter specificare un valore per i seguenti
parametri:

**Entità:** consente di definire l'entità su cui dovranno poi essere
effettuate eventuali operazioni massive. E' possibile selezionare una
delle seguenti opzioni:

- **Componente:** in queste condizioni le operazioni massive che andremo
  poi ad impostare saranno relative ai componenti presenti all'interno
  di una specifica pagina piuttosto che dell'interno sito

- **Pagina:** in questo caso invece sarà possibile impostare operazioni
  massive relativamente alle varie pagine del sito

**Ambiente:** consente di decidere su quale ambiente dovremo andare ad
agire e conseguentemente che tipo di operazione massiva potremo poi
effettuare.

E' possibile selezionare una delle seguenti opzioni

- **Sito -- Pubblicazione:** in queste condizioni **l'ambiente di
  riferimento sarà il front end del sito** e l'azione massiva da poter
  eseguire varierà in relazione all'Entità selezionata nel precedente
  parametro.

> In particolare nel momento in cui l'Entità su cui si è deciso di
> lavorare dovessero essere le **Pagine** del sito allora l'azione
> massiva da poter eseguire sarà quella che riguarda la pubblicazione o
> meno di determinate pagine

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\protezione_pagine_2.bmp](./assets/media/image106.png)

> In corrispondenza del parametro "**Pagine**" sarà possibile
> selezionare le pagine che dovranno essere coinvolte nell'operazione.
>
> All'interno della sezione "**Impostazioni**" comparirà invece il
> parametro **"Pubblico"** mediante il quale poter decidere se
> pubblicare o spubblicare in blocco tutte le pagine precedentemente
> selezionate
>
> Nel momento in cui l'Entità su cui si è deciso di lavorare dovessero
> essere invece i **Componenti**, allora, l'azione massiva da poter
> eseguire sarà quella che riguarda la pubblicazione o meno di
> determinati componenti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione_pubblica_articoli.bmp](./assets/media/image107.png)

> In queste condizioni i parametri "**Livello**", "**Classi**" e
> "**Classi addizionali**" consentono di decidere, rispettivamente se
> l'operazione dovrà essere effettuata a livello di singola pagina o di
> intera Variante e su quali Componenti andare effettivamente ad agire
> (selezionandoli in base alle loro classi CSS)
>
> Il parametro **"Pubblico"**, presente all'interno della sezione
> "**Impostazioni**" consente invece di decidere se pubblicare o
> spubblicare in blocco i componenti indicati

- **Sito -- Protezione:** selezionando questa opzione, **l'ambiente di
  riferimento sarà il front end del sito** e l'azione massiva da poter
  eseguire varierà in relazione all'Entità selezionata nel precedente
  parametro.

> In particolare nel momento in cui l'Entità su cui si è deciso di
> lavorare dovessero essere le **Pagine** del sito allora l'azione
> massiva da poter eseguire sarà quella che riguarda la visibilità delle
> pagine indicate, sul front end del sito, a tutti o solo a determinati
> gruppi utente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\protezione_pagine_1.bmp](./assets/media/image108.png)

> In corrispondenza del parametro "**Pagine**" sarà possibile
> selezionare le pagine che dovranno essere coinvolte nell'operazione.
>
> All'interno della sezione "**Impostazioni**" sarà invece possibile
> decidere se le pagine selezionate dovranno essere visibili, sul front
> end del sito, a tutti oppure solo a determinati gruppi di utenti
>
> Nel momento in cui l'Entità su cui si è deciso di lavorare dovessero
> essere invece i **Componenti** allora l'azione massiva da poter
> eseguire sarà quella che riguarda le impostazioni di visibilità dei
> componenti indicati per tutti o solo per determinati Gruppi Utente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione2.bmp](./assets/media/image109.png)

> Anche in questo caso i parametri "**Livello**", "**Classi**" e
> "**Classi addizionali**" consentono di decidere, rispettivamente se
> l'operazione dovrà essere effettuata a livello di singola pagina o di
> intera Variante e su quali Componenti andare effettivamente ad agire
> (selezionandoli in base alle loro classi CSS)
>
> Il parametro "**Visibile da**" (sezione "**Impostazioni**") permetterà
> invece di decidere se i componenti indicati dovranno essere visibili,
> sul front end del sito, a tutti oppure solo a determinati gruppi di
> utenti.

- **Sito -- Cache**: solo per Entità di tipo "Componente". Selezionando
  questa opzione, **l'ambiente di riferimento sarà il front end del
  sito** e l'azione massiva da poter eseguire sarà quella che riguarda
  la possibilità di disattivare il caching dei componenti indicati.

> In queste condizioni infatti, all'interno della sezione "Impostazioni"
> comparirà il parametro "**Disabilita Cache**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione_disabilita_cache.bmp](./assets/media/image110.png)

> grazie al quale poter decidere se disabilitare o meno, in blocco, il
> caching di tutti i componenti della tipologia indicata presenti
> all'interno della pagina in esame piuttosto che all'interno
> dell'interno sito.
>
> I parametri "**Livello**", "**Classi**" e "**Classi addizionali**"
> consentono infatti di decidere, rispettivamente, se l'operazione dovrà
> essere effettuata a livello di singola pagina o di intera Variante e
> su quali Componenti andare effettivamente ad agire (selezionandoli in
> base alle loro classi CSS)
>
> **ATTENZIONE!** Ovviamente questo tipo di operazione avrà un senso
> solo nel momento in cui sia stato attivato, per il proprio sito, il
> modulo di Cache. Per maggiori informazioni relativamente alla gestione
> della cache in Passweb e all'attivazione del relativo modulo presente
> su Passstore, si rimanda a quanto indicato nel corrispondente capitolo
> di questo manuale ("*Configurazione -- Cache*")

- **Wizard -- Protezione:** solo per Entità di tipo "Componente".
  Selezionando questa opzione, **l'ambiente di riferimento sarà il back
  end del sito** e l'azione massiva da poter eseguire sarà quella che
  riguarda la protezione, lato Wizard, di determinati componenti

> In queste condizioni infatti, all'interno della sezione "Impostazioni"
> comparirà il parametro "**Protezione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione3.bmp](./assets/media/image111.png)

> mediante il quale poter decidere chi, fra i vari utenti del Wizard,
> potrà avere o meno la possibilità di gestire, secondo il relativo
> schema di permessi, i componenti che soddisfano le condizioni
> impostate mediante i parametri Livello, Classi e Classi addizionali

**Livello** **--** disponibile solo per Entità di tipo "Componente":
consente di decidere se dovranno essere presi in considerazione tutti i
componenti del sito o solo quelli di una specifica pagina.

E' possibile selezionare uno dei seguenti valori:

- **Pagina**: selezionando questa opzione verranno presi in
  considerazione tutti i componenti della pagina corrente

- **Variante:** selezionando questa opzione verranno presi in
  considerazione tutti i componenti del sito, o meglio, tutti i
  componenti presenti all'interno di una qualsiasi pagina della Variante
  Sito attualmente caricata all'interno del Wizard.

**Classi** **--** disponibile solo per Entità di tipo "Componente":
consente di decidere se dovranno essere effettivamente presi in
considerazione, all'interno della pagina corrente piuttosto che
all'interno dell'intero sito, tutti i componenti (opzione **Tutte**)
oppure solamente quelli di una determinata tipologia (opzione
**Alcune**).

In quest'ultimo caso sarà necessario specificare la tipologia di
componenti desiderati all'interno del box evidenziato in figura.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_protezione4.bmp](./assets/media/image112.png)

E' sufficiente indicare le prime lettere del nome dei Componenti (così
come questo compare all'interno della libreria dei componenti Passweb)
per attivare la funzione di autocompletamento che aiuta a scegliere il
componente desiderato, tra quelli effettivamente gestibili dall'utente
attualmente connesso sul Wizard:

**ATTENZIONE!** La funzione di autocompletamento prende in
considerazione le classi effettivamente gestibili dal ruolo dell\'utente
connesso sul Wizard.

Affinchè un determinato componente possa essere inserito nel box
evidenziato in figura è necessario quindi che, per il ruolo dell\'utente
connesso, siano stati assegnati i permessi di "**Accesso**",
"**Modifica"** e di "**Config. e Distribuzione"**.

**Classi addizionali --** disponibile solo per Entità di tipo
"Componente": consente di selezionare i componenti che dovranno essere
presi in considerazione, nell'ambito dell'operazione massiva che si
intende eseguire, indicando esattamente la classe CSS personalizzata che
è stata loro assegnata in fase di creazione.

Nel momento in cui l'esigenza dovesse essere quella di inserire,
all'interno del campo in esame, due o più classi personalizzate i
relativi valori dovranno essere separati da uno spazio

**ATTENZIONE!** E' sufficiente che nel campo "Classi addizionali" di un
componente Passweb sia indicata almeno una delle classi inserite in
corrispondenza del parametro in esame per fare in modo che l'operazione
indicata venga effettivamente eseguita

Per maggiori informazioni relativamente a come poter assegnare ai vari
componenti una classe CSS personalizzata si veda anche quanto indicato
nei precedenti capitoli di questo manuale ("*Varianti Sito Responsive --
Configurazione Componenti Caratteristiche Generali -- Avanzate e
Animazioni*")

**ATTENZIONE!** Anche in questo caso l'operazione indicata verrà
eseguita solo ed esclusivamente nel momento in cui la classe CSS
indicata sia relativa ad un componente che l'utente attualmente loggato
può effettivamente gestire (sulla base ovviamente di quello che è lo
schema di permessi associato al suo Ruolo Utente)

Al salvataggio della maschera "Gestione Protezione" le impostazioni
settate verranno applicate:

- Se è stato impostato il Livello "Pagina" a tutti i componenti della
  pagina corrente che fanno riferimento alle classi indicate nel campo
  "Classi" e/o "Classi addizionali" e per i quali sia stata indicata una
  protezione lato Wizard che consenta all\'utente connesso di poterli
  effettivamente modificare.

- Se è stato impostato il Livello "Variante" ai componenti di tutte le
  pagine della Variante corrente che fanno riferimento alle classi
  indicate nel campo "Classi" e/o "Classi addizionali" e per i quali sia
  stata indicata una protezione lato Wizard che consenta all\'utente
  connesso di poterli effettivamente modificare.

La funzione in oggetto può rivelarsi particolarmente utile nel momento
in cui l'esigenza dovesse essere, ad esempio, quella di abilitare la
visualizzazione dei prezzi e l'aggiunta in carrello ai soli utenti
autenticati (opzione questa piuttosto comune all'interno di siti di
tipologia B2B).

In questo senso infatti, anziché agire singolarmente su tutti i
componenti "Prezzo" e su tutti i componenti "Aggiunta al Carrello" che
possono essere presenti all'interno del sito, sarà perfettamente
sufficiente agire dalla maschera "Gestione Protezione" appena analizzata
impostando i parametri in essa presenti come di seguito indicato:

- Ambiente = **Sito -- Protezione**

- Livello = **Variante**

- Classi = **ecFieldprice** **ecFieldaddtocatrt**

- Visibile da = **Utente** **Autenticato**
