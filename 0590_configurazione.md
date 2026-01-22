# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_libro_res.bmp](./assets/media/image11.png){width="4.597222222222222in"
height="2.876388888888889in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di definire un nome per il Componente che si sta
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

> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

**Categoria Filtro:** consente di visualizzare nei componenti di
navigazione (es. Navigazione Libro ed Indice Libro) che verranno poi
inseriti all'interno del componente considerato, solo ed esclusivamente
elementi relativi a notizie o post appartenenti alla categoria indicata

> **NOTA BENE:** nel caso in cui non venga specificata alcuna categoria
> i componenti di navigazioni inseriti all'interno del libro non saranno
> sottoposti ad alcun tipo di filtraggio.

**Tipo di Paginazione:** consente di impostare il tipo di paginazione
che dovrà essere adottata dai contenuti che verranno inseriti
all'interno di questo componente. E' possibile selezionare uno dei
seguenti valori:

- **Con caricamento della pagina:** in queste condizioni cliccando sui
  link presenti in corrispondenza dei componenti "Navigazione Libro" e
  "Indice Libro" inseriti all'interno del componente in esame, per
  visualizzare i nuovi contenuti verrà ricaricata l'intera pagina web

- **Senza caricamento della pagina:** in queste condizioni cliccando sui
  link presenti in corrispondenza dei componenti "Navigazione Libro" e
  "Indice Libro" inseriti all'interno del componente in esame, verranno
  aggiornati tramite javascript i seguenti componenti:

  - Dettaglio News

  - Libro

  - Navigazione News

  - Contenuti Correlati

> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> non aggiornare uno dei componenti sopra indicati sarà sufficiente
> assegnare al componente stesso la classe "**nojsrefresh**"

- **Scroll infinito (Lazy Loading):** in queste condizioni si otterrà lo
  stesso funzionamento della precedente opzione "Senza caricamento della
  pagina". Inoltre verrà anche abilitata la gestione del Lazy Loading
  sul componente "Dettaglio News".

> Nello specifico poi **affinché il caricamento progressivo (Lazy
> Loading) del componente Dettaglio News possa funzionare in maniera
> corretta sarà necessario inserire all'interno del Libro in esame un
> componente "Navigazione Libro" configurato con il campo "Tipo di
> navigazione" impostato sul valore "Successivo (linearmente)"**
>
> In queste condizioni quando, allo scroll della pagina, verrà raggiunto
> il componente "Navigazione Libro" il contenuto successivo verrà
> automaticamente aggiunto di seguito a quello corrente (creando quindi
> uno scroll infinito)
>
> Nel momento in cui all'interno del Libro non dovesse invece essere
> presente nessun componente "Navigazione Libro" configurato come appena
> indicato, non sarà possibile, per ovvie ragioni, attivare il Lazy
> Loading del Dettaglio News e verrà quindi gestita una normale
> paginazione "Senza caricamento della pagina"
>
> **ATTENZIONE!** una volta attivato questo tipo di paginazione, se
> l'esigenza dovesse poi essere quella di gestire correttamente, tramite
> Analytics, le statistiche sulle visite ai contenuti CMS, sarà
> necessario utilizzare Tag Manager impostando correttamente "Google Tag
> Manager History Change trigger". Ogni volta che viene caricato un
> nuovo contenuto tramite javascript verrà infatti modificato l'url del
> browser tramite histry.pushState

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Libro" può essere considerato a tutti gli effetti come
un "Componente di tipo Contenitore".** Sarà infatti possibile inserire
al suo interno dei campi che, per poter esser gestiti liberamente,
dovranno inevitabilmente esser trattati a loro volta come Componenti
autonomi editabili singolarmente.

Per poter far questo occorre, innanzitutto, attivare la modalità di
gestione dei componenti, sarà poi necessario portarsi sul Componente
"Libro" e, alla comparsa del R.O.C. cliccare sull'icona "**Accedi ai
componenti interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Libro" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il layout del
  componente. Per maggiori informazioni relativamente all'utilizzo di
  questi componenti si vedano le corrispondenti sezioni di questo
  manuale.

- **Componenti CMS:** contiene quei componenti necessari a visualizzare
  all'interno del componente in oggetto i singoli elementi componenti
  una notizia. Nel caso specifico, in particolare, per poter inserire
  all'interno di un Libro, elementi quali il Titolo della Notizia,
  l'autore, la data ecc ... sarà necessario per prima cosa passare
  attraverso il componente "Dettaglio News". Come precedentemente
  evidenziato poi, assumerà un'importanza particolare il componente
  "Navigazione Libro", che potrà essere inserito solo ed esclusivamente
  all'interno di un Libro e consentirà di mettere a disposizione
  dell'utente tutta una serie di controlli grazie ai quali poter
  navigare interattivamente fra i vari post componenti la struttura
  della Notizia selezionata.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i componenti CMS interni ad un componente "Libro" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti CMS -- Componenti Interni ai Componenti
> CMS).

L'inserimento di questi componenti all'interno del Componente Libro
avviene utilizzando le solite tecniche di interazione con l'editor (Drag
and Drop o Point and Click) già esaminate all'interno di questo manuale
(per maggiori informazioni si rimanda allo specifico capitolo di questo
manuale).

