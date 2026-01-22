# CONFIGURAZIONE



**Il Componente "Campionario"** **può essere inserito, per sua stessa
natura, unicamente all'interno del componente "Scheda Prodotto".**

In particolare, lavorando **all'interno della pagina "Prodotti"
generica**, accessibile dalla corrispondente voce del menu "Gestione
Pagine" o all'interno di una Pagina Prodotto corrispondente ad una
specifica categoria merceologica, i vari campi inseriti all'interno del
componente "Campionario" non potranno, ovviamente, essere valorizzati
con delle informazioni reali, relative cioè ad uno specifico articolo e
prelevate ad esempio direttamente dal gestionale.

Al posto di queste informazioni verranno quindi inseriti all'interno del
componente dei segnaposto identificativi dello specifico campo e
conseguentemente della specifica informazione che si vorrà visualizzare
in quella specifica posizione.

Lavorando invece **all'interno della pagina Prodotto relativa ad uno
specifico articolo Campionario o con DBA**, andando poi a personalizzare
il Componente, i vari campi in esso inseriti verranno valorizzati con
delle informazioni reali, relative esattamente allo specifico articolo.

**ATTENZIONE!** Lavorando **all'interno della pagina Prodotto relativa
ad un normale articolo di Magazzino** (es. articoli Mexal di tipo A), è
comunque possibile inserire il componente "Campionario" all'interno
della scheda prodotto ma questo, per ovvie ragioni, non verrà
visualizzato e non potrà quindi essere personalizzato in maniera
corretta.

Le celle dei vari articoli componenti il Campionario saranno precedute
da un'etichetta modificabile alla pagina "*Testi dei Componenti*"
(componente **Campionario**) del Wizard (etichetta che potrà essere
diversa a seconda del fatto di utilizzare il Campionario per creare o
meno dei Box configurabili)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campionario_etichetta.bmp](./assets/media/image104.png)

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e di configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_campionario_configurazione_res.bmp](./assets/media/image105.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome**: consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default)**: consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione**: consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Numero di colonne della griglia**: consente di specificare il numero
  delle colonne da cui dovrà essere formata la griglia in cui verranno
  visualizzati i componenti del campionario.

> Anche in questo caso poi, come già per la griglia di visualizzazione
> del catalogo o delle offerte, è bene ricordare che indipendentemente
> dal numero di colonne impostate, per risoluzioni **inferiori ai 992
> px** verranno sempre visualizzati 2 articoli per riga. Analogamente
> per risoluzioni **inferiori a 768 px** la griglia si linearizzerà
> mostrando un articolo per ogni riga

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Campionario E-Commerce" può essere considerato a tutti
gli effetti come un "Componente di tipo Contenitore".**

Sarà quindi possibile inserire al suo interno tutta una serie di campi
necessari per poter definire che tipo di informazioni gestionali e non,
dovranno essere visualizzate per ogni singolo articolo componente il
campionario. Tali campi, in ogni caso, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Una volta inserito quindi il Componente "Campionario E-Commerce"
all'interno del Componente "Scheda Prodotto" per poterlo poi
personalizzare sarà necessario, attivare la modalità di gestione dei
componenti interni alla Scheda Prodotto, portarsi sul Componente in
esame e, alla comparsa del R.O.C. cliccare sull'icona "**Accedi ai
componenti interni".**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Campionario
E-Commerce" sarà possibile inserire due differenti tipologie di
componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce**: contiene tutti i componenti E-Commerce,
  ossia quei componenti necessari per abilitare e gestire determinate
  funzionalità oltre che, ovviamente, per poter definire che tipo di
  informazioni gestionali dovranno essere visualizzate per ogni singolo
  articolo componente il Campionario.

> **ATTENZIONE!** Sulla base di quanto evidenziato nei precedenti
> capitoli di questo manuale i Componenti Interni "**Configuratore
> E-commerce**", "**Prezzo**", "**Aggiunta al Carrello**" potranno
> essere inseriti all'interno di un qualsiasi Componente Campionario ma
> verranno poi visualizzati (sia lato Back-end che lato Front-End) solo
> ed esclusivamente nel momento in cui l'articolo in esame sia
> effettivamente un Campionario \\ Composto Configurabile
>
> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Campionario" si veda la
> corrispondente sezione di questo manuale (Varianti Sito Responsive --
> Lista Componenti E-Commerce -- Componenti Interni ai Componenti
> Ecommerce).

L'inserimento di questi componenti all'interno del Componente
"Campionario E-Commerce" avviene utilizzando le solite tecniche di
interazione con l'editor (Drag and Drop o Point and Click) già esaminate
all'interno di questo manuale (per maggiori informazioni si rimanda allo
specifico capitolo di questo manuale).

In ogni caso, comunque, il Componente "Campionario E-Commerce" sarà
costituito da un certo numero di celle (una per ogni articolo componente
il Campionario stesso). **I vari componenti (siano essi Componenti
Comuni o Componenti E-Commerce) potranno essere inseriti indistintamente
all'interno di una qualsiasi di queste celle (penserà poi l'applicazione
a ripeterli, in maniera completamente automatica all'interno di tutte le
altre celle)**

