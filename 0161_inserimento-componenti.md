# INSERIMENTO COMPONENTI



L'inserimento di un nuovo Componente nella pagina del sito può avvenire
attraverso due diverse modalità che possono variare in funzione di una
precisa scelta da parte dell'utente.

Tale scelta è attuabile grazie al parametro "**Interazione editor**"
presente alla pagina "**Profilo Utente**" del Wizard

![](./assets/media/image183.png)

Per inserire un nuovo Componente all'interno di una pagina del sito è
necessario, come prima cosa, abilitare la modalità di "**Aggiunta Nuovi
Componenti**" cliccando per questo sul corrispondente pulsante presente
all'interno del menu di Editing del sito

![](./assets/media/image184.png)

o, in alternativa, sulla corrispondente icona presente nella Barra degli
Strumenti del Live Editing

![](./assets/media/image185.png)

In ogni caso, una volta abilitata questa specifica modalità di gestione
verrà visualizzata immediatamente la libreria dei componenti Passweb,
all'interno della quale poter poi selezionare lo specifico elemento da
inserire nella pagina web

![](./assets/media/image186.png)

Tale libreria è suddivisa in 5 distinte sezioni ciascuna delle quali
raggruppa una specifica tipologia di componenti:

- **Comuni:** all'interno di questa sezione sono raggruppati tutti i
  Componenti normalmente utilizzati per costruire l'interfaccia grafica
  del sito (es. Paragrafo, Immagine con Link, Contenitore, Contenitore
  Griglia ecc...).

> I contenuti di questi componenti dovranno essere stabiliti in fase di
> configurazione del componente stesso oppure direttamente all'interno
> del Wizard mediante, ad esempio, l'inserimento di altri componenti.

- **PWB-App:** all'interno di questa sezione sono raggruppati tutti quei
  Componenti che potranno poi essere utilizzati esclusivamente per
  costruire l'interfaccia grafica dell' App Mobile.

> **ATTENZIONE!** La sezione PWB-App sarà disponibile solo ed
> esclusivamente nel caso in cui il sito in esame abbia attiva e
> collegata un App Mobile.
>
> I componenti presenti all'interno di questa sezione non potranno mai
> essere inseriti in pagine dedicate esclusivamente al sito e,
> ovviamente, saranno poi visibili solo all'interno dell'App mobile
> collegata al sito stesso
>
> Per maggiori informazioni in merito all'App Mobile e all'utilizzo di
> questi componenti si veda anche il capitolo "*App Mobile e Progressive
> web app*" di questo manuale.

- **Interazione Utente:** all'interno di questa sezione sono raggruppati
  i Componenti utilizzati per gestire l'accesso e la registrazione al
  sito da parte dei vari utenti (es. Login Utente, Recupero Credenziali,
  Registrazione Utente ecc...)

- **Cms:** all'interno di questa sezione sono raggruppati tutti i
  componenti utilizzati per gestire in maniera strutturata la
  pubblicazione di post e notizie all'interno del proprio sito (es.
  Archivio Notizie, Dettaglio Notizie, Menu di categoria, Tag ecc...)

> I contenuti di questi componenti, di norma, dovranno essere inseriti
> operando all'interno dell'apposita sezione del Wizard ("*Sito --
> Gestione CMS -- Contenuti*")

- **Ecommerce:** all'interno di questa sezione sono raggruppati tutti i
  componenti utilizzati per gestire la parte Ecommerce del proprio sito
  (es. Catalogo Articoli, Scheda Prodotto, Menu di Categorie
  Merceologiche, Abbinati, Offerte, Campionari, Configuratori ecc...)

> **I contenuti di questa particolare tipologia di componenti (di base
> gli articoli gestiti all'interno del sito) verranno prelevati e
> potranno quindi essere gestiti direttamente dallo specifico gestionale
> Passepartout collegato al sito.**

**ATTENZIONE!** I componenti disponibili all'interno delle sezioni sopra
indicate possono variare in relazione alla specifica pagina in cui si
sta operando e al fatto di voler inserire il componente stesso come
elemento di primo livello oppure all'interno di un altro componente di
tipo Contenitore (per maggiori informazioni sui componenti di tipo
Contenitore si vedano anche i successivi capitoli di questo manuale)

I pulsanti presenti nella barra degli strumenti della libreria
consentono rispettivamente di:

- **Minimizza (**
  ![](./assets/media/image187.png) **):** consente di minimizzare la
  libreria dei componenti in maniera tale da aumentare lo spazio di
  lavoro senza comunque dover uscire completamente dalla modalità di
  "Aggiunta nuovi Componenti"

![](./assets/media/image188.png)

> Una volta minimizzata, la libreria dei componenti può essere riportata
> alle sue dimensioni originali in un qualsiasi momento cliccando sul
> relativo pulsante di massimizzazione (
> ![](./assets/media/image189.png) )

- **Sposta (**
  ![](./assets/media/image190.png) **):** consente di spostare, con una
  semplice operazione di Drag and Drop l'intera libreria dei componenti
  in una qualsiasi altra posizione della pagina Web in maniera tale da
  non interferire con l'area della pagina in cui si intende lavorare

> Per effettuare lo spostamento è sufficiente posizionarsi con il mouse
> sul pulsante in esame, tenere premuto il tasto sinistro e trascinare
> l'icona stessa nella posizione desiderata. Rilasciando il pulsante la
> libreria dei componenti verrà effettivamente spostata.
>
> **ATTENZIONE!** Passweb memorizza l'ultima posizione utile in cui è
> stata spostata la libreria dei componenti.
>
> Alle successive attivazioni della modalità di "Aggiunta nuovi
> Componenti" la libreria verrà quindi aperta esattamente nell'ultima
> posizione utile.

- **Opacità (**
  ![](./assets/media/image191.png) **):** consente di abbassare l'opacità
  della libreria dei componenti lasciando quindi intravedere gli
  elementi della pagina web posti al di sotto di essa.

- **Chiudi (**
  ![](./assets/media/image192.png) **):** consente di chiudere la
  libreria dei componenti e, conseguentemente, di uscire dalla modalità
  di "Aggiunta Nuovi Componenti"

Detto della libreria e delle opzioni di gestione, vediamo ora come poter
inserire uno dei suoi elementi all'interno della pagina web.

L'inserimento di un nuovo Componente nella pagina può avvenire, come
detto inizialmente, in due modi diversi:

- **Drag and Drop** (la cui traduzione migliore è "clicca, trascina e
  rilascia"), che consiste nel cliccare sul Componente desiderato col
  tasto sinistro del mouse e, mantenendo premuto il tasto stesso,
  trascinare il Componente nella pagina web per poi rilasciarlo nella
  posizione della pagina in cui si desidera posizionarlo.

> Una volta selezionato il Componente e trascinato nella pagina, il
> punto in cui rilasciarlo sarà suggerito da appositi focus che ne
> evidenzieranno l'eventuale posizionamento all'interno della pagina
> (nel caso si tratti di una sezione vuota della pagina) o sopra/sotto
> uno specifico componente già presente all'interno della pagina stessa
> (nel caso si tratti di un Componente già esistente).

![](./assets/media/image193.png)

- **Point and Click** (punta e clicca), che consiste nel cliccare col
  tasto sinistro sul Componente desiderato e poi nel Contenitore della
  pagina nella quale si desidera posizionarlo. Una volta selezionato
  quindi il Componente, muovendo il mouse nella pagina web, verranno
  evidenziati, attraverso specifici focus, tutti i Componenti già
  esistenti o i Contenitori della pagina nei quali sarà possibile
  rilasciare il nuovo Componente.

> Una volta cliccato nel punto desiderato, comparirà la finestra "**Dove
> vuoi aggiungere il Componente?**" contenente le seguenti opzioni:

- **All'interno del Contenitore ...** : E' l'unica opzione disponibile
  in caso il Componente venga rilasciato in un Contenitore vuoto (privo
  cioè di altri Componenti).

- **Come primo Componente di ... :** Nel caso vi siano uno o più
  Componenti nel contenitore all'interno del quale si desidera inserire
  il nuovo Componente verrà chiesto, in funzione del Contenitore stesso
  (colonna centrale, colonna destra, testata etc.), se rilasciare il
  Componente come primo (in alto) tra tutti quelli già inseriti.

- **Come Ultimo Componente di ... :** Nel caso vi siano uno o più
  Componenti nel Contenitore all'interno del quale si desidera inserire
  il nuovo Componente verrà chiesto, in funzione del Contenitore stesso
  (colonna centrale, colonna destra, testata etc.), se rilasciare il
  Componente Come ultimo (in basso) tra tutti quelli già inseriti.

- **Prima del Componente ...:** Nel caso vi siano uno o più Componenti
  nel Contenitore all'interno del quale si desidera inserire il nuovo
  Componente verrà chiesto, in funzione del Componente già inserito e
  sul quale si è cliccato, se rilasciare il nuovo Componente
  posizionandolo prima (sopra) di esso.

- **Dopo del Componente ...:** Nel caso vi siano uno o più Componenti
  nel Contenitore all'interno del quale si desidera inserire il nuovo
  Componente verrà chiesto, in funzione del Componente già inserito e
  sul quale si è cliccato, se rilasciare il nuovo Componente
  posizionandolo dopo (sotto) di esso.

Indipendentemente dalla modalità di inserimento componenti utilizzata,
una volta rilasciato ed inserito un Componente all'interno della pagina,
verrà visualizzata **la maschera di gestione e di configurazione del
componente** stesso

![](./assets/media/image194.png)

maschera questa suddivisa, come evidenziato dalla figura sopra
riportata, in varie sezioni, alcune delle quali possono variare in
relazione anche al particolare componente considerato.

Per maggiori informazioni relativamente alla configurazione dei vari
componenti Passweb si rimanda alla corrispondente sezione di questo
manuale ("*Varianti Sito Responsive* *-- Configurazione Componenti
Caratteristiche generali / Lista Componenti*")

