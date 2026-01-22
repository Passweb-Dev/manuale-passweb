# GESTIONE CONTENUTI



La sezione "**Gestione Contenuti**" consente di definire e gestire i
contenuti di ogni singolo Pannello scorrevole.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-accordion-contenuti_res.bmp](./assets/media/image186.png)

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Aggiungi pannello** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png) ): consente di aggiungere una nuova
  pannello al componente in oggetto.

- **Copia pannello** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_copia.bmp](./assets/media/image72.png) ): consente di copiare il pannello
  attualmente selezionato in elenco.

- **Elimina pannello**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image16.png) ): consente di eliminare il pannello
  attualmente selezionata in elenco.

- **Sposta su / giù**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icone_su_giu.bmp](./assets/media/image17.png) ): consente di riordinare tra loro i
  vari pannelli presenti all'interno del componente spostando verso
  l'alto o il basso il pannello attualmente selezionata in elenco.

Nella parte destra della sezione "Gestione Contenuti" è invece possibile
definire per ogni singolo pannello presente all'interno del componente,
un valore per le seguenti proprietà:

- **Titolo:** consente di impostare l'etichetta identificativa dello
  specifico pannello. Il Titolo verrà poi visualizzato all'interno della
  linguetta identificativa del pannello che si sta realizzando.

- **Funzionamento:** consente di definire il modo in cui dovranno essere
  organizzati i contenuti all'interno dello specifico pannello.

> In questo senso è possibile selezionare uno dei seguenti valori:

- **Contenuto:** impostando il parametro "Funzionamento" su questo
  valore sarà poi possibile inserire il contenuto dello specifico
  pannello agendo **direttamente da questa stessa maschera** e
  utilizzando per questo il corrispondente editor HTML**.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\slider_funzionamento_contenuto_res.bmp](./assets/media/image180.png)

> Per maggiori informazioni relativamente all'utilizzo di questo editor
> HTML si veda anche il relativo capitolo ("Live Editing per Varianti
> Responsive -- Contenuti -- Editor dei contenuti") di questo manuale.
>
> In queste condizioni, quindi ,compariranno all'interno della maschera
> le due ulteriori sezioni **"Contenuto"** e **"Eventuale Immagine"**
> attraverso cui poter poi, rispettivamente, editare il testo che dovrà
> essere inserito nello specifico pannello, e selezionare,
> eventualmente, un'immagine da associare a questo testo. Cliccando
> infatti sul pulsante **"Seleziona Risorsa"** si verrà ricondotti alla
> maschera di "Gestione Risorse" attraverso cui poter selezionare
> dall'elenco (o caricarla ex-novo dal proprio computer) l'immagine
> desiderata. La piccola x eventualmente posta a fianco del pulsante
> "Seleziona Risorsa" consentirà di azzerare il campo eliminando quindi
> l'associazione con la risorsa precedentemente selezionata.
>
> Una volta impostati i contenuti desiderati, il pulsante **"Aggiungi
> Elemento",** nella parte bassa della maschera, consentirà di
> aggiungere il pannello appena editata al Componente Accordion che si
> sta realizzando.

- **Contenitore:** impostando il parametro "Funzionamento" su questo
  valore il pannello che si sta realizzando verrà considerato come un
  vero e proprio contenitore di componenti. **In questo caso dunque sarà
  possibile inserire all'interno di questo pannello non del semplice
  testo accompagnato eventualmente da un'immagine ma bensì dei veri e
  propri Componenti Passweb (Paragrafo, Immagine con Link, Rss, Menu,
  Contenuti su Tab ecc...)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore_res.bmp](./assets/media/image181.png)

> **L'inserimento di questi componenti non potrà però avvenire
> direttamente da questa maschera di configurazione, come nel caso
> precedente, ma, trattandosi di veri e propri componenti Passweb, dovrà
> necessariamente avvenire in modalità "Live Editing" utilizzando le
> solite tecniche di Drag and Drop o Point and Click**.
>
> In sostanza dunque, nelle condizioni indicate, il componente
> "Contenuti su Accordion" diventerà a tutti gli effetti un vero e
> proprio **Componente di tipo Contenitore** e andrà quindi trattato e
> gestito come tale
>
> Per poter inserire dei contenuti all'interno dei pannelli gestiti in
> questo modo, sarà quindi necessario, dopo aver ovviamente aggiunto i
> vari pannelli (pulsante "Aggiungi Elemento") e dopo aver salvato il
> componente (pulsante "Salva"), attivare la modalità di gestione dei
> componenti, portarsi col mouse sul componente in esame e, alla
> comparsa del R.O.C., cliccare sull'icona '**Accedi ai componenti
> interni**' in maniera tale da abilitare, nella barra degli strumenti i
> due pulsanti di gestione dei componenti interni al pannello
> considerato
>
> Per maggiori informazioni relativamente alla gestione dei Componenti
> di tipo Contenitore si veda anche il corrispondente capitolo di questo
> manuale ("Live Editing per Varianti Responsive -- Componenti --
> Componenti di tipo Contenitore")
>
> **NOTA BENE:** i componenti da inserire all'interno dei pannelli di un
> componente Accordion, gestito nella maniera sopra indicata, possono
> variare in relazione alla specifica pagina e/o ad eventuali ulteriori
> componenti di tipo contenitore in cui il componente stesso è inserito
>
> Infine, nelle condizioni sopra indicate, sarà anche possibile
> assegnare ad ogni singola sezione del componente una specifica
> immagine di sfondo agendo in questo senso dal relativo parametro
> **"Immagine di Sfondo Sezione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenuti_tabs_contenitore2_res.bmp](./assets/media/image182.png)

- **Visibile da:** consente di impostare la visibilità del pannello in
  oggetto a livello di gruppi utente, potendo quindi decidere quali
  utenti potranno o meno visualizzarlo.

> Impostando questo parametro sul valore **"Tutti"** il pannello ed i
> relativi contenuti saranno visibili ed accessibili a tutti i
> visitatori del sito.
>
> Impostando invece il parametro sul valore **"Solo i gruppi
> Specificati"** verranno visualizzati tutti i gruppi utente
> appositamente creati all'interno della corrispondente sezione "*Utenti
> -- Gruppi Utenti Sito*" del Wizard. **In queste condizioni il pannello
> in oggetto, ed i relativi contenuti, potranno quindi essere visibili
> ai soli utenti appartenenti ai gruppi selezionati**.
>
> Per maggiori informazioni relativamente alla creazione dei Gruppi
> Utente si veda la corrispondente sezione "Utenti -- Gruppi Utenti
> Sito" di questo manuale.

