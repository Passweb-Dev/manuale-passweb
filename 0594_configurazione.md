# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_contenuti_correlati_res.bmp](./assets/media/image16.png){width="4.597222222222222in"
height="3.071527777777778in"}

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

> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

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

**Argomento:** consente di indicare, selezionandolo tra quelli
precedentemente codificati all'interno della corrispondente sezione del
Wizard, lo specifico argomento in relazione al quale dovranno essere
visualizzate, all'interno del componente in oggetto, eventuali liste di
correlazione.

**Non visualizzare in lista i contenuti appartenenti alla struttura di
origine :** se selezionato consente di non visualizzare all'interno
della lista di correlazione considerata, oltre allo specifico post di
cui si sta visualizzando il dettaglio, anche tutti quelli appartenenti
alla sua stessa struttura. Ovviamente tale parametro ha senso solo ed
esclusivamente in relazione a notizie strutturate.

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
**il Componente "Contenuti Correlati" può essere considerato a tutti gli
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

In particolare all'interno di un componente di tipo "Contenuti
Correlati" sarà possibile inserire due differenti tipologie di
componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il layout del
  componente. Per maggiori informazioni relativamente all'utilizzo di
  questi componenti si vedano le corrispondenti sezioni di questo
  manuale.

- **Componenti CMS:** contiene quei componenti necessari a visualizzare
  all'interno del componente in oggetto i singoli elementi componenti
  una notizia (Titolo, Autore, Sommario, Articolo ecc ...).

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i componenti CMS interni ad un componente "Contenuti Correlati" si
> veda la corrispondente sezione di questo manuale (Live Editing per
> Varianti Responsive -- Lista Componenti CMS -- Componenti Interni ai
> Componenti CMS).

L'inserimento di questi componenti all'interno del Componente Lista News
avviene utilizzando le solite tecniche di interazione con l'editor (Drag
and Drop o Point and Click) già esaminate all'interno di questo manuale
(per maggiori informazioni si rimanda allo specifico capitolo di questo
manuale).

In ogni caso, comunque, anche il componente "Contenuti Correlati" sarà
costituito da un certo numero di celle (una per ogni notizia pubblicata
al suo interno). **I vari componenti (siano essi Componenti Comuni o
Componenti CMS) utilizzati per costruire la propria lista di
correlazione potranno essere inseriti indistintamente all'interno di una
qualsiasi di queste celle (penserà poi l'applicazione a ripeterli, in
maniera completamente automatica, all'interno di tutte le altre celle
della lista)**

