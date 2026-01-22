# COMPONENTI CMS -- NAVIGAZIONE LIBRO



Il Componente **"Navigazione libro"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\cms_componente_navigazione_libro_res.bmp](./assets/media/image86.png){width="2.5520833333333335in"
height="2.545138888888889in"}

consente di inserire all'interno di un componente CMS "Libro", tutta una
serie di controlli grazie ai quali poter navigare interattivamente fra i
vari post componenti la struttura della notizia attualmente visualizzata
all'interno del Libro stesso.

> **NOTA BENE:** il componente "Navigazione Libro" può essere inserito
> solo ed esclusivamente all'interno di un componente CMS "Libro" ed è
> ciò che lo contraddistingue e lo differenzia rispetto ad un semplice
> componente "Dettaglio News".

Sulla base di quanto appena detto è quindi evidente che anche il
componente "Navigazione Libro", così come il suo componente contenitore
"Libro", assume un significato ed un'utilità particolare solo ed
esclusivamente in relazione a Notizie strutturate.

A livello di configurazione, una volta inserito il Componente
all'interno della pagina web, verrà aperta in automatico **la sua
maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_navigazione_libro_configurazione_res.bmp](./assets/media/image87.png){width="4.629861111111111in"
height="3.0972222222222223in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di indicare il nome del componente che si sta
realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Pagina di Destinazione per il Dettaglio News:** consente di
specificare la pagina del sito che dovrà essere utilizzata come pagina
per la visualizzazione del dettaglio della notizia selezionata.
Ovviamente poi per poter garantire agli utenti del sito di visualizzare
correttamente il dettaglio della notizia selezionata all'interno del
componente in oggetto, nella pagina di destinazione per il Dettaglio
News dovrà necessariamente essere presente il Componente "**Dettaglio
News**" con al suo interno il Componente "**Articolo**"

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Dettaglio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.

**Pagina di Destinazione per l'Archivio News:** consente di selezionare
la pagina del sito che dovrà essere destinata a contenere l'archivio
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

**Tipo di Navigazione:** consente di specificare il tipo di controllo
che dovrà essere visualizzato all'interno del componente in oggetto. E'
possibile selezionare uno dei seguenti valori:

- **Precedente (linearmente):** selezionando questo valore, il
  componente "Navigazione Libro" conterrà informazioni relativamente al
  post immediatamente precedente, nella struttura considerata, a quello
  attualmente visualizzato all'interno del corrispondente componente
  "Libro".

- **Successivo (linearmente):** selezionando questo valore, il
  componente "Navigazione Libro" conterrà informazioni relativamente al
  post immediatamente successivo, nella struttura considerata, a quello
  attualmente visualizzato all'interno del corrispondente componente
  "Libro".

- **Risali:** selezionando questo valore, il componente "Navigazione
  Libro" conterrà informazioni relativamente al post padre, nella
  struttura considerata, di quello attualmente visualizzato all'interno
  del corrispondente componente "Libro".

- **Facenti parte dello stesso ramo:** selezionando questo valore, il
  componente "Navigazione Libro" conterrà informazioni relativamente a
  tutti i post presenti, nella struttura considerata, allo stesso
  livello (nello stesso ramo) di quello attualmente visualizzato
  all'interno del corrispondente componente "Libro".

- **Paginazione lineare:** selezionando questo valore, all'interno del
  componente "Navigazione Libro" verranno visualizzate in maniera
  lineare informazioni relative all'intera struttura della notizia
  attualmente visualizzata all'interno del corrispondente componente
  "Libro"

- **Paginazione lineare:** selezionando questo valore, il componente
  "Navigazione Libro" conterrà informazioni relativamente al post radice
  della struttura della notizia visualizzata all'interno del
  corrispondente componente "Libro".

- **Briciole di Pane:** selezionando questo valore, all'interno del
  componente "Navigazione Libro" verranno visualizzate informazioni
  relative all'esatto percorso di localizzazione, all'interno della
  struttura considerata, del post attualmente visualizzato nel
  corrispondente componente "libro"

> **NOTA BENE:** ciascuno degli elementi sopra indicati potrebbe
> rappresentare, dipendentemente dalla configurazione degli elementi
> inseriti all'interno del componente "Navigazione Libro", un link al
> dettaglio della corrispondente notizia.

**Formato Data:** permette di impostare un particolare formato della
Data di Pubblicazione tra quelli proposti.

Per quel che riguarda invece la logica di gestione del suo contenuto, il
Componente "Navigazione Libro" si comporta allo stesso modo dei
componenti "Form" e "Contenitore" e anch'esso come questi componenti,
dunque, **può essere considerato a tutti gli effetti come un
"Contenitore di Componenti".** Sarà infatti possibile, secondo le stesse
modalità più volte analizzate all'interno di questo manuale, inserire al
suo interno tutta una serie di campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i componenti interni ad un componente "Navigazione Libro" si vedano
> anche i precedenti capitoli di questo manuale.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

