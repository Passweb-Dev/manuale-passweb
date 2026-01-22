# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image61.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome**: consente di definire un nome per il Componente che si sta
  editando

- **Pubblico** (selezionato a default): consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

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

- **Riferimento Articoli Strutturati:** consente di impostare l'elemento
  che dovrà essere utilizzato come riferimento nel momento in cui i dati
  visualizzati all'interno della scheda prodotto dovessero essere quelli
  di un articolo strutturato.

> E' possibile selezionare una delle seguenti opzioni:

- **Figlio:** selezionando questa opzione nel momento in cui l'utente
  dovesse utilizzare un eventuale configuratore presente all'interno
  della pagina prodotto e la configurazione impostata dovesse
  corrispondere ad un articolo figlio correttamente esportato e gestito
  anche all'interno del sito, allora al termine della configurazione i
  dati inizialmente presenti all'interno della scheda in esame
  (immagini, prezzo, singoli Attributi Articolo, interi Set di Attributi
  ...) riferiti ovviamente al corrispondente articolo padre, verranno
  automaticamente aggiornati e sostituiti dalle stesse informazioni
  relative però allo specifico prodotto finito.

- **Padre:** selezionando questa opzione nel momento in cui l'utente
  dovesse utilizzare un eventuale configuratore presente all'interno
  della pagina prodotto e la configurazione impostata dovesse
  corrispondere ad un articolo figlio correttamente esportato e gestito
  anche all'interno del sito, al termine della configurazione **i dati
  presenti all'interno della scheda in esame non verranno aggiornati e
  rimarranno sempre, quindi, quelli iniziali relativi al corrispondente
  articolo padre**

> Il fatto di impostare il parametro in questione sull'opzione "Padre"
> potrebbe, da una parte, rivelarsi particolarmente utile nel momento in
> cui i figli di un determinato padre di struttura dovessero avere,
> effettivamente, un set di informazioni identiche a quelle
> dell'articolo padre. In queste condizioni infatti non ci sarebbe
> bisogno di valorizzare gli stessi campi allo stesso modo per
> l'articolo padre e anche per i relativi articoli figlio (perché
> comunque i dati presenti all'interno della scheda prodotto sarebbero
> sempre e comunque quelli dello stesso articolo padre).
>
> Dall'altra parte però occorre prestare particolare attenzione al fatto
> che tutte le informazioni presenti all'interno di una scheda prodotto
> configurata in questo modo saranno sempre relative all'articolo padre,
> e questo vale anche per il prezzo, per l'aggiunta al carrello, alla
> wishlist ecc... e questo potrebbe, chiaramente, essere un problema nel
> momento in cui, ad esempio, l'articolo figlio dovesse avere un prezzo
> diverso da quello del padre o anche solo per il fatto che il
> componente di aggiunta al carrello non verrà mai visualizzato
> all'interno di una scheda prodotto impostata per visualizzare sempre e
> comunque i dati del padre.
>
> **In sostanza dunque nel momento in cui l'esigenza dovesse essere
> quella di gestire un set di informazioni identiche tra l'articolo
> padre ed i relativi figli, sarà indispensabile utilizzare sempre due
> distinte schede prodotto.**
>
> Una con il campo "Riferimento articoli strutturati" impostato sul
> valore "Padre" e con al suo interno tutti i campi articolo che avranno
> poi lo stesso valore per il padre di struttura e per i relativi figli
> (es. attributi articolo, descrizioni ecc...).
>
> L' altra invece con il campo "Riferimento articoli strutturati"
> impostato sul valore "Figlio" e con al suo interno, questa volta, i
> campi articolo il cui valore potrebbe essere differente tra l'articolo
> padre ed i relativi figli (es. prezzo, immagini, schede tecniche,
> pulsante di aggiunta in carrello ...)

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Anche il Componente "Scheda Prodotto", al pari di altri componenti
precedentemente esaminati **può essere considerato a tutti gli effetti
come un "Componente di tipo Contenitore".**

Sarà quindi possibile inserire al suo interno tutta una serie di campi
necessari per poter definire che tipo di informazioni, Mexal e non,
dovranno essere visualizzate per lo specifico articolo. Tali campi, in
ogni caso, per poter esser gestiti liberamente, dovranno inevitabilmente
esser trattati a loro volta come Componenti autonomi editabili
singolarmente.

Una volta inserito quindi il Componente "Scheda Prodotto" all'interno
della pagina per poterlo poi personalizzare sarà necessario, attivare la
modalità di gestione dei componenti, portarsi sul Componente in esame e,
alla comparsa del R.O.C. cliccare sull'icona "**Accedi ai componenti
interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Scheda Prodotto"
sarà possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti E-Commerce:** contiene tutti i componenti E-Commerce,
  ossia quei componenti necessari per abilitare e gestire determinate
  funzionalità (es. "Aggiunta al Carrello") oltre che, ovviamente, per
  poter definire che tipo di informazioni gestionali dovranno essere
  visualizzate per lo specifico articolo.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Scheda Prodotto" si veda
> la corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

L'inserimento di questi componenti all'interno del Componente "Scheda
Prodotto" avviene utilizzando le solite tecniche di interazione con
l'editor (Drag and Drop o Point and Click) già esaminate all'interno di
questo manuale (per maggiori informazioni si rimanda allo specifico
capitolo di questo manuale).

