# GESTIONE CONTENUTI



La sezione "**Gestione Contenuti**" consente di definire e gestire i
contenuti di ogni singolo Tab.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-tabs-contenuti_res.bmp](./assets/media/image179.png){width="5.149305555555555in"
height="3.1104166666666666in"}

In particolare nella parte sinistra di questa sezione è visualizzato
l'elenco delle schede (tabs) attualmente presenti all'interno del
componente.

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Aggiungi scheda** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png){width="0.18819444444444444in"
  height="0.18819444444444444in"} ): consente di aggiungere una nuova
  scheda.

- **Copia scheda** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_copia.bmp](./assets/media/image72.png){width="0.1951388888888889in"
  height="0.21458333333333332in"} ): consente di copiare la scheda
  attualmente selezionata in elenco

- **Elimina scheda** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image16.png){width="0.18194444444444444in"
  height="0.18194444444444444in"} ): consente di eliminare la scheda
  attualmente selezionata in elenco.

- **Sposta su / giù**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icone_su_giu.bmp](./assets/media/image17.png){width="0.3701388888888889in"
  height="0.21458333333333332in"} ): consente di riordinare tra loro le
  varie schede presenti all'interno del componente spostando verso
  l'alto o il basso la scheda attualmente selezionata in elenco.

Nella parte destra della sezione "**Gestione Contenuti**" è invece
possibile definire le proprietà e le caratteristiche della scheda
attualmente selezionata. In particolare è possibile impostare un valore
per i seguenti campi:

- **Titolo:** consente di impostare l'etichetta identificativa della
  specifica scheda. Il Titolo verrà poi visualizzato all'interno della
  linguetta della scheda che si sta realizzando.

- **Funzionamento:** consente di definire il modo in cui dovranno essere
  organizzati i contenuti all'interno della specifica scheda.

> In questo senso è possibile selezionare uno dei seguenti valori:

- **Contenuto:** impostando il parametro "Funzionamento" su questo
  valore sarà poi possibile inserire il contenuto della scheda in
  questione agendo **direttamente da questa stessa maschera** e
  utilizzando per questo il corrispondente editor HTML

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\slider_funzionamento_contenuto_res.bmp](./assets/media/image180.png){width="4.759722222222222in"
height="3.3506944444444446in"}

> Per maggiori informazioni relativamente all'utilizzo di questo editor
> HTML si veda anche il relativo capitolo ("*Live Editing per Varianti
> Responsive -- Contenuti -- Editor dei contenuti*") di questo manuale.
>
> In queste condizioni, dunque, compariranno all'interno della maschera
> le due ulteriori sezioni **"Contenuto"** e **"Eventuale Immagine"**
> attraverso cui poter poi, rispettivamente, editare il testo che dovrà
> essere inserito nella specifica scheda, e selezionare, eventualmente,
> un'immagine da associare a questo testo. Cliccando infatti sul
> pulsante **"Seleziona Risorsa"** si verrà ricondotti alla maschera di
> "Gestione Risorse" attraverso cui poter selezionare dall'elenco (o
> caricarla ex-novo dal proprio computer) l'immagine desiderata. La
> piccola x eventualmente posta a fianco del pulsante "Seleziona
> Risorsa" consentirà di azzerare il campo eliminando quindi
> l'associazione con la risorsa precedentemente selezionata.
>
> Una volta impostati i contenuti desiderati, il pulsante **"Aggiungi
> Elemento",** nella parte bassa della maschera, consentirà di
> aggiungere la scheda appena editata al Componente Tabs che si sta
> realizzando.

- **Contenitore:** impostando il parametro "Funzionamento" su questo
  valore la scheda che si sta realizzando verrà considerata come un vero
  e proprio contenitore di componenti. . **In questo caso dunque sarà
  possibile inserire all'interno di questa scheda non del semplice testo
  accompagnato eventualmente da un'immagine ma bensì dei veri e propri
  Componenti Passweb (Paragrafo, Immagine con Link, Rss, Menu, Contenuti
  su Tab ecc...)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore_res.bmp](./assets/media/image181.png){width="4.370138888888889in"
height="2.6104166666666666in"}

> **L'inserimento di questi componenti non potrà però avvenire
> direttamente da questa maschera di configurazione, come nel caso
> precedente, ma, trattandosi di veri e propri componenti Passweb, dovrà
> necessariamente avvenire in modalità "Live Editing" utilizzando le
> solite tecniche di Drag and Drop o Point and Click**.
>
> In sostanza dunque, nelle condizioni indicate, il componente
> "Contenuti su Tabs" diventerà a tutti gli effetti un vero e proprio
> **Componente di tipo Contenitore** e andrà quindi trattato e gestito
> come tale
>
> Per poter inserire dei contenuti all'interno delle schede gestite in
> questo modo, sarà quindi necessario, dopo aver ovviamente aggiunto le
> varie schede (pulsante "Aggiungi Elemento") e dopo aver salvato il
> componente (pulsante "Salva"), attivare la modalità di gestione dei
> componenti, portarsi col mouse sul componente in esame e, alla
> comparsa del R.O.C., cliccare sull'icona '**Accedi ai componenti
> interni**' in maniera tale da abilitare, nella barra degli strumenti i
> due pulsanti di gestione dei componenti interni alla sezione
> considerata
>
> Per maggiori informazioni relativamente alla gestione dei Componenti
> di tipo Contenitore si veda anche il corrispondente capitolo di questo
> manuale ("*Live Editing per Varianti Responsive -- Componenti --
> Componenti di tipo Contenitore*")
>
> **NOTA BENE:** i componenti da inserire all'interno delle schede di un
> componente Tabs, gestito nella maniera sopra indicata, possono variare
> in relazione alla specifica pagina e/o ad eventuali ulteriori
> componenti di tipo contenitore in cui il componente stesso è inserito
>
> Infine, nelle condizioni sopra indicate, sarà anche possibile
> assegnare ad ogni singola sezione del componente una specifica
> immagine di sfondo agendo in questo senso dal relativo parametro
> **"Immagine di Sfondo Sezione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore2_res.bmp](./assets/media/image182.png){width="4.370138888888889in"
height="2.6104166666666666in"}

- **Visibile da:** consente di impostare la visibilità della scheda in
  oggetto a livello di gruppi utente, potendo quindi decidere quali
  utenti potranno o meno visualizzarla.

> Impostando questo parametro sul valore **"Tutti"** la scheda ed i
> relativi contenuti saranno visibili ed accessibili a tutti i
> visitatori del sito.
>
> Impostando invece il parametro sul valore **"Solo i gruppi
> Specificati"** verranno visualizzati tutti i gruppi utente
> appositamente creati all'interno della corrispondente sezione "*Utenti
> -- Gruppi Utenti Sito*" del Wizard. **In queste condizioni la Scheda
> in oggetto, ed i relativi contenuti, potranno quindi essere visibili
> ai soli utenti appartenenti ai gruppi selezionati**.
>
> Per maggiori informazioni relativamente alla creazione dei Gruppi
> Utente si veda la corrispondente sezione "*Utenti -- Gruppi Utenti
> Sito*" di questo manuale.

