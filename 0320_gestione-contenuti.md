# GESTIONE CONTENUTI



La sezione **"Gestione Contenuti"**, presente all'interno della maschera
di configurazione del componente consente di definire le varie slide e
di gestire quindi il contenuto di ogni singola sezione di questo
componente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_slider_gestione_contenuti_res.bmp](./assets/media/image196.png)

Sulla sinistra è visualizzato l'elenco delle sezioni attualmente
presenti all'interno del componente. I pulsanti presenti nella
contestuale barra degli strumenti consentono rispettivamente di:

- **Aggiungi Slide singola** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png) ): consente di aggiungere una nuova
  Slide al componente in oggetto.

- **Aggiungi Slide Multiple** ( ): utile nel caso in cui l'esigenza
  dovesse essere quella **di creare in blocco N slide con all'interno
  componenti di tipo "Immagine".**

> Cliccando su questo pulsante verrà aperta immediatamente la maschera
> di "Gestione Risorse". A differenza del caso precedente (Aggiunta
> Slide singola), questa volta sarà però possibile selezionare una delle
> cartelle presenti all'interno di questa sezione per poi cliccare sul
> pulsante "Seleziona" (senza dover quindi indicare specificatamente una
> singola risorsa della cartella).
>
> In questo modo verranno aggiunte allo Slider, in maniera completamente
> automatica, tante Slide per quante sono le immagini presenti
> all'interno della cartella selezionata (**non verrà considerato in
> questa operazione il contenuto di eventuali sotto cartelle**).
>
> Ogni Slide creata in automatico attraverso questo processo potrà poi
> essere editata sia a livello grafico che a livello di contenuti
> esattamente come se fosse stata creata in maniera manuale.

- **Copia Slide** ( ): consente di copiare la Slide attualmente
  selezionata in elenco

- **Sposta su / giù**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icone_su_giu.bmp](./assets/media/image17.png) ): consente di riordinare tra loro le
  varie Slide presenti all'interno del componente spostando verso l'alto
  o il basso la Slide attualmente selezionata in elenco.

- **Elimina slide**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image16.png) ): consente di eliminare la slide
  attualmente selezionata in elenco.

Nella parte destra della sezione "Gestione Contenuti" è invece possibile
definire, per ogni singola slide presente all'interno del componente, un
valore per le seguenti proprietà:

- **Titolo:** consente di impostare l'etichetta identificativa della
  specifica sezione dello slider che si sta realizzando

- **Funzionamento:** consente di definire il modo in cui dovranno essere
  organizzati i contenuti all'interno della specifica sezione dello
  slider.

> In questo senso è possibile selezionare uno dei seguenti valori:

- **Contenuto:** impostando il parametro "Funzionamento" su questo
  valore sarà poi possibile inserire all'interno della specifica sezione
  dello slider solamente del testo, accompagnato eventualmente da
  un'immagine. **L'inserimento di questi contenuti dovrà avvenire,
  inoltre, direttamente da questa stessa maschera.**

> In queste condizioni, infatti ,compariranno all'interno della maschera
> le due ulteriori sezioni **"Contenuto"** e **"Eventuale Immagine"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\slider_funzionamento_contenuto_res.bmp](./assets/media/image180.png)

> attraverso cui poi poter, rispettivamente, editare il testo che dovrà
> essere inserito nella specifica sezione dello slider, e selezionare
> un'immagine da associare a questo testo. Cliccando infatti sul
> pulsante **"Seleziona Risorsa"** si verrà ricondotti alla maschera di
> "Gestione Risorse" attraverso cui poter selezionare dall'elenco (o
> caricarla ex-novo dal proprio computer) l'immagine desiderata. La
> piccola x eventualmente posta a fianco del pulsante "Seleziona
> Risorsa" consentirà di azzerare il campo eliminando quindi
> l'associazione con la risorsa precedentemente selezionata.
>
> Una volta impostati i contenuti desiderati, il pulsante **"Aggiungi
> Elemento",** presente nella parte alta della maschera consentirà di
> aggiungere la sezione appena editata al Componente Slider che si sta
> realizzando.

- **Contenitore:** impostando il parametro "Funzionamento" su questo
  valore la sezione dello slider che si sta realizzando verrà
  considerata come un vero e proprio contenitore di componenti. . **In
  questo caso dunque sarà possibile inserire all'interno di questa slide
  non del semplice testo accompagnato eventualmente da un'immagine ma
  bensì dei veri e propri Componenti Passweb (Paragrafo, Immagine con
  Link, Rss, Menu, Contenuti su Tab ecc...)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore_res.bmp](./assets/media/image181.png)

> **L'inserimento di questi componenti non potrà però avvenire
> direttamente da questa maschera di configurazione, come nel caso
> precedente, ma, trattandosi di veri e propri componenti, dovrà
> necessariamente avvenire in modalità "Live Editing" utilizzando le
> solite tecniche di Drag and Drop o Point and Click**.
>
> In sostanza dunque, nelle condizioni indicate, il componente
> "Contenuti su Slider" diventerà a tutti gli effetti un vero e proprio
> **Componente di tipo Contenitore** e andrà quindi trattato e gestito
> come tale
>
> Per poter inserire dei contenuti all'interno delle slide gestite in
> questo modo, sarà quindi necessario, dopo aver ovviamente aggiunto le
> varie slide, attivare la modalità di gestione dei componenti e
> portarsi sulla slide all'interno della quale si vogliono inserire dei
> nuovi elementi utilizzando, per questo, gli stessi controlli di
> scorrimento messi a disposizione dal componente. Alla comparsa del
> R.O.C. sarà quindi sufficiente cliccare sull'icona '**Accedi ai
> componenti interni**' e una volta ottenuto l'accesso ai componenti
> interni alla slide sarà sufficiente, come al solito, abilitare la
> modalità di Aggiunta nuovi Componenti, selezionare dalla libreria
> Passweb il componente desiderato ed inserirlo all'interno della slide
> secondo le normali modalità di interazione proprie di Passweb (Drag &
> Drop o Point & Click)
>
> Per maggiori informazioni relativamente alla gestione dei Componenti
> di tipo Contenitore si veda anche il corrispondente capitolo di questo
> manuale ("*Live Editing per Varianti Responsive -- Componenti --
> Componenti di tipo Contenitore*")
>
> **NOTA BENE:** i componenti da inserire all'interno delle slide di un
> componente "Slider", gestito nella maniera sopra indicata, possono
> variare in relazione alla specifica pagina e/o ad eventuali ulteriori
> componenti di tipo contenitore in cui il componente stesso è inserito
>
> Infine, nelle condizioni sopra indicate, sarà anche possibile
> assegnare ad ogni singola slide del componente una specifica immagine
> di sfondo agendo in questo senso dal relativo parametro **"Immagine di
> Sfondo Sezione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore2_res.bmp](./assets/media/image182.png)

- **Visibile da:** consente di impostare la visibilità della slide in
  oggetto a livello di gruppi utente, potendo quindi decidere quali
  utenti potranno o meno visualizzarla.

> Impostando questo parametro sul valore **"Tutti"** la slide ed i
> relativi contenuti saranno visibili ed accessibili a tutti i
> visitatori del sito.
>
> Impostando invece il parametro sul valore **"Solo i gruppi
> Specificati"** verranno visualizzati tutti i gruppi utente
> appositamente creati all'interno della corrispondente sezione "*Utenti
> -- Gruppi Utenti Sito*" del Wizard. **In queste condizioni la slide in
> oggetto, ed i relativi contenuti, potranno quindi essere visibili ai
> soli utenti appartenenti ai gruppi selezionati**.
>
> Per maggiori informazioni relativamente alla creazione dei Gruppi
> Utente si veda la corrispondente sezione "Utenti -- Gruppi Utenti
> Sito" di questo manuale.

