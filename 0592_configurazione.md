# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_indice_libro_res.bmp](./assets/media/image13.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di definire un nome per il Componente che si sta
editando.

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Tipo di Caricamento:** consente di specificare come dovrà essere
gestita la visualizzazione delle voci dell'indice libro di livello
maggiore a 1.

E' possibile selezionare una delle seguenti opzioni:

- **A Richiesta:** in queste condizioni al caricamento della pagina web
  saranno presenti (nel DOM della pagina stessa) solo ed esclusivamente
  voci dell'indice libro di primo livello. Eventuali voci di livello
  maggiore o uguale a 2 verranno inserite all'interno della pagina solo
  ed esclusivamente nel momento in cui un utente dovesse richiederne la
  visualizzazione (cliccando per questo sull'apposita icona di apertura
  delle relative sotto voci).

> **Tale opzione potrebbe essere utile per diminuire i tempi di
> caricamento della pagina soprattutto nel caso in cui il numero delle
> sotto voci sia estremamente elevato**

- **Tutto in una Volta:** in queste condizioni al caricamento della
  pagina web saranno presenti (nel DOM della pagina stessa) tutte le
  voci dell'indice libro coerentemente, sempre, con il livello di
  profondità impostato in fase di configurazione del componente stesso

**Tipo di Stili applicati al Menu:** consente di impostare la tipologia
e conseguente lo stile di visualizzazione dell'indice libro.

**ATTENZIONE!** Le tipologie di menu selezionabili dipendono anche da
quanto impostato per il precedente parametro "Tipo di Caricamento"

E' possibile selezionare uno tra i seguenti valori.

- **Offcanvas:** selezionando questa opzione l'indice libro verrà
  posizionato al di fuori della pagina web dove invece comparirà
  soltanto un pulsante utile a richiamarlo.

> I successivi parametri consentono poi di decidere dove e come dovrà
> essere visualizzato l'indice libro nel momento in cui un utente
> dovesse richiamarlo cliccando sull'apposito pulsante.
>
> Nello specifico dunque il parametro:

- **Inizializzazione menù:** consente di impostare la modalità di
  apertura iniziale del menu

- **Posizionamento del menu:** consente di indicare la posizione in cui
  dovrà essere visualizzato il menu nel momento in cui l'utente dovesse
  decidere di richiamarlo. E' possibile decidere di visualizzarlo sulla
  parte sinistra / destra oppure nella parte alta / bassa della pagina
  stessa

- **Sposta il contenuto del sito all'apertura del menu:** se selezionato
  nel momento in cui l'utente dovesse decidere di richiamare il menu,
  questo verrà visualizzato facendo scorrere la parte restante della
  pagina web verso sinistra/destra/alto/basso dipendentemente dalle
  impostazioni settate per il precedente parametro.

> Nel caso in cui il parametro in oggetto non venga selezionato, il menu
> verrà invece visualizzato andando a sovrapporsi ai contenuti della
> pagina lasciando comunque una porzione della pagina stessa sempre
> visibile.

- **Immagine per Off canvas:** consente di indicare la specifica
  immagine da utilizzare per il pulsante di apertura del menu (l'unico
  elemento visualizzato inizialmente all'interno della pagina web).

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![Videate\\icona_menu_offcanvas.bmp](./assets/media/image14.png)

- **Treeview:** selezionando questo valore verranno visualizzate
  soltanto le voci dell'indice libro di primo livello. Eventuali
  sotto-voci potranno essere visualizzate (nascoste) al click del mouse.

> In queste condizioni sarà inoltre necessario indicare un valore per i
> seguenti parametri:

- **Immagine Controllo Apri/Chiudi Ramo:** consente di selezionare una
  specifica immagine da poter utilizzare per il controllo di apertura /
  chiusura delle sotto voci. E' possibile indicare una delle immagini
  presenti nel database del sito oppure uno degli Attributi Immagine
  gestiti.

> Nel caso in cui non venga specificata nessun immagine il controllo di
> apertura delle sotto voci sarà rappresentato da un **\[+\]** e quello
> di chiusura da un **\[-\].**

**Tipo di Stili applicati al Menu per dispositivi mobili \< 992px:**
visibile solo nel caso in cui il parametro "**Tipo di Stili applicati al
Menu**" non sia stato impostato sull'opzione Off Canvas

Consente di indicare la tipologia di menu che dovrà essere utilizzata
nel momento in cui il dispositivo di visualizzazione del sito dovesse
avere una larghezza inferiore ai 992px.

In questo senso è possibile decidere di utilizzare un menu a **Lista**,
un menu **Off Canvas** oppure (parametro "**Non Visualizzare**")
mantenere esattamente la stessa tipologia di menu utilizzata anche per
dispositivi di visualizzazione del sito con larghezza maggiore o uguale
a 992px

**ATTENZIONE!** Grazie al parametro "Tipo di Stili applicati al Menu per
dispositivi mobili \< 992px" è possibile cambiare dinamicamente la
tipologia di menu utilizzata per l'indice libro in base alla larghezza
del dispositivo di visualizzazione del sito senza dover per forza di
cose realizzare due differenti menu con le relative opzioni di
visualizzazione.

**Pagina di Destinazione per il Dettaglio News:** consente di
selezionare la pagina del sito che dovrà essere utilizzata come pagina
per la visualizzazione del dettaglio delle notizie presenti all'interno
di questo componente. Ovviamente poi per poter garantire agli utenti del
sito di visualizzare correttamente il dettaglio della notizia
selezionata, nella pagina di destinazione per il Dettaglio News dovrà
necessariamente essere presente il Componente "**Dettaglio News**" con
al suo interno il Componente "**Articolo**"

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Dettaglio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.

**Pagina di Destinazione Archivio News:** consente di selezionare la
pagina del sito che dovrà essere destinata a contenere l'archivio
all'interno del quale poter ricercare le varie notizie. Ovviamente
all'interno di questa stessa pagina dovrà poi essere necessariamente
presente il componente CMS "Archivio News".

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Archivio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.
>
> **NOTA BENE:** in relazione ai due campi sopra indicati valgono per
> essi le stesse considerazioni fatte relativamente al componente "Lista
> News".

**Profondità**: consente di impostare il livello di profondità in
relazione al quale visualizzare i vari elementi presenti all'interno
della struttura della notizia considerata.

Impostando ad esempio questo campo sul valore 3 l'indice libro
visualizzerà i soli elementi della notizia strutturata presenti al primo
secondo e terzo livello della struttura stessa:

**Formato Data:** permette di impostare un particolare formato della
Data di Pubblicazione tra quelli proposti.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Indice Libro" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore".** Sarà infatti
possibile inserire al suo interno dei campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Per poter far questo occorre, innanzitutto, attivare la modalità di
gestione dei componenti, sarà poi necessario portarsi sul Componente in
esame e, alla comparsa del R.O.C. cliccare sull'icona "**Accedi ai
componenti interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Indice Libro" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il layout del
  componente. Per maggiori informazioni relativamente all'utilizzo di
  questi componenti si vedano le corrispondenti sezioni di questo
  manuale.

- **Componenti CMS:** contiene quei componenti necessari a visualizzare
  all'interno del componente in oggetto i singoli elementi componenti
  una notizia (Titolo, Autore, Sommario, Articolo ecc ...).

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i componenti CMS interni ad un componente "Lista News" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti CMS -- Componenti Interni ai Componenti
> CMS).

L'inserimento di questi componenti all'interno del Componente Indice
Libro avviene utilizzando le solite tecniche di interazione con l'editor
(Drag and Drop o Point and Click) già esaminate all'interno di questo
manuale (per maggiori informazioni si rimanda allo specifico capitolo di
questo manuale).

In ogni caso, comunque, l'Indice Libro sarà costituito da un certo
numero di celle (una per ogni notizia pubblicata al suo interno). **I
vari componenti (siano essi Componenti Comuni o Componenti CMS)
utilizzati per costruire il proprio indice potranno essere inseriti
indistintamente all'interno di una qualsiasi di queste celle (penserà
poi l'applicazione a ripeterli, in maniera completamente automatica,
all'interno di tutte le altre)**

