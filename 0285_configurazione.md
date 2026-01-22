# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico la sua maschera **di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_griglia_res.bmp](./assets/media/image101.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" è possibile settare i
principali parametri di configurazione del componente.

In particolare dunque il parametro:

- **Nome:** consente di assegnare un nome alla Griglia che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
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

Come già visto per il Componente Contenitore classico, anche in questo
caso sono disponibili poi diversi parametri di configurazione mediante i
quali poter abilitare o meno determinate funzionalità aggiuntive sulla
Griglia che si sta realizzando.

In particolare dunque il parametro:

- **Sticky:** consente di "fissare" la Griglia in esame in una specifica
  posizione, mantenendola quindi sempre visibile allo scrolling del sito
  verso il basso.

> Una volta assunta la posizione "sticky" al componente verrà assegnata
> in maniera del tutto automatica la classe CSS "**pw-sticky**" che può
> risultare particolarmente utile nel momento in cui si dovesse decidere
> di assegnargli, in queste particolari condizioni, una diversa
> formattazione grafica.
>
> Selezionando questo parametro compariranno poi due ulteriori campi
> "**Top Position per lo Sticky**" e "**Classe o elemento per fermare lo
> sticky**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\griglia_sticky_1.bmp](./assets/media/image102.png)

> che consentono rispettivamente di:

- **Top Position per lo Sticky:** consente di impostare l'offset,
  rispetto al bordo alto della pagina, in corrispondenza del quale la
  griglia in esame dovrà diventare sticky.

> Supponendo dunque di inserire all'interno di questo campo il valore
> 100, la griglia seguirà lo scrolling del sito fintanto che la distanza
> tra essa ed il bordo superiore della pagina risulti essere maggiore o
> uguale a 100px. Una volta raggiunta tale distanza la griglia si
> fisserà invece alla pagina mantenendo quindi inalterata la sua
> posizione indipendentemente dal fatto che l'utente continui a
> scrollare il sito verso il basso.
>
> **ATTENZIONE!** Lasciando il campo vuoto o, in alternativa, impostando
> il valore 0 la Griglia diventerà sticky una volta raggiunto
> esattamente il bordo alto della pagina web

- **Classe o elemento per fermare lo sticky:** consente di impostare la
  classe CSS (.classeElemento) o l'identificativo (#idElemento) dello
  specifico Componente che dovrà interrompere, una volta entrato
  nell'area visibile della pagina web, per la Griglia in questione, il
  posizionamento sticky.

> Per maggiori informazioni relativamente a come poter individuare la
> classe o l'id di un componente Passweb si veda anche la sezione "*Live
> Editing -- Componenti -- Azioni Componente -- Informazioni
> Componente*" di questo manuale.
>
> **ATTENZIONE!** **Per ovvie ragioni il parametro Sticky potrà
> funzionare correttamente solo se applicato ad un Contenitore Griglia
> di primo livello (che non è stato cioè inserito all'interno di altri
> componenti di tipo Contenitore)**

- **Menu Offcanvas:** consente di trattare la Griglia che si sta
  realizzando nello stesso modo in cui vengono trattati i Contenitori
  Off Canvas.

> Selezionando questa opzione dunque, la Griglia (e con essa ovviamente
> anche tutti gli elementi presenti nelle varie colonne) verrà
> posizionata, inizialmente, al di fuori della pagina web dove invece
> comparirà soltanto un pulsante.
>
> Cliccando su questo pulsante la griglia verrà richiamata e
> visualizzata nella pagina secondo quelle che sono le impostazioni
> settate dall'amministratore in fase di configurazione del componete
> stesso (esattamente come avveniva per un normale Contenitore Off
> Canvas).
>
> Una volta selezionato questo parametro, compariranno quindi ulteriori
> campi mediante i quali poter impostare rispettivamente:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\griglia_offcanvas.bmp](./assets/media/image103.png)

- **Posizionamento del menu:** consente di indicare la posizione in cui
  dovrà essere visualizzata la Griglia nel momento in cui l'utente
  dovesse decidere di richiamarla. È possibile decidere di visualizzarla
  sulla parte sinistra / destra oppure nella parte alta / bassa della
  pagina stessa

- **Sposta il contenuto del sito all'apertura del menu:** se selezionato
  nel momento in cui l'utente dovesse decidere di richiamare la Griglia,
  questa verrà visualizzato facendo scorrere la parte restante della
  pagina web verso sinistra/destra/alto/basso dipendentemente dalle
  impostazioni settate per il precedente parametro.

> Nel caso in cui il parametro in oggetto non venga selezionato, la
> Griglia verrà invece visualizzata andando a sovrapporsi ai contenuti
> della pagina lasciando comunque una porzione della pagina stessa
> sempre visibile.

- **Immagine per Off canvas:** consente di indicare la specifica
  immagine da utilizzare per il pulsante mediante il quale poter
  richiamare la Griglia (l'unico elemento visualizzato inizialmente
  all'interno della pagina web).

> È possibile indicare una delle immagini presenti nel database del sito
> oppure uno degli Attributi Immagine gestiti (campo "**Attributi
> temi**")
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![Videate\\icona_menu_offcanvas.bmp](./assets/media/image95.png)

- **Alt-text immagine offcanvas**: consente di impostare, in tutte le
  lingue attualmente gestite all'interno del sito, il valore che dovrà
  avere l'attributo alt assegnato all'immagine impostata in
  corrispondenza del precedente parametro "Immagine per Off canvas"

- **Testo del bottone offcanvas**: consente di indicare il testo di un
  eventuale label da mostrare a fianco dell'immagine di apertura della
  Griglia

> Ora, considerando che, come appena detto, le Griglie Off Canvas, così
> come i Contenitori Offcanvas, sono posizionate inizialmente al di
> fuori della pagina web (e questo non solo sul front end del sito ma
> anche all'interno del back end), **per poterle gestire sia dal punto
> di vista grafico che, soprattutto, dal punto di vista dei loro
> contenuti e quindi degli ulteriori elementi da inserire al loro
> interno, la prima cosa da fare sarà ovviamente quella di richiamarle
> rendendole visibili all'interno della pagina.**
>
> Per far questo sarà sufficiente cliccare sul relativo pulsante di
> apertura esattamente come farebbe un normale visitatore del sito.
>
> In alternativa è anche possibile cliccare sulla corrispondente icona
> di apertura
> (![Videate\\icona_apri_chiudi_menu.bmp](./assets/media/image96.png)) presente nel R.O.C. di questa
> particolare tipologia di componente
>
> **ATTENZIONE!** A differenza di quanto avveniva per i Menu Off Canvas,
> la visualizzazione delle Griglie Off Canvas all'interno dell'ambiente
> di sviluppo è leggermente diversa rispetto a quella che sarà poi la
> visualizzazione di questi stessi elementi sul front end del sito.
>
> In effetti indipendentemente da quelle che sono le opzioni di
> configurazione del componente, questo, **all'interno dell'ambiente di
> sviluppo, verrà visualizzato sempre e soltanto al di sotto del
> pulsante di apertura** in maniera tale da poter poi inserire in esso
> ulteriori componenti utilizzando le solite modalità di interazione
> proprie di Passweb.
>
> In queste condizioni, per avere un'idea chiara soprattutto del
> dimensionamento dei vari elementi, si consiglia sempre di controllare
> il risultato finale sul front end del sito.

- **Tipologia di collapse:** consente di rendere il contenuto delle
  Griglia che si sta realizzando, collassabile dando quindi al
  visitatore del sito la possibilità di visualizzare / nascondere i
  relativi contenuti al click su di un apposito pulsante.

> Impostando dunque il parametro in oggetto sul valore "**Bottone (il
> contenitore verrà visualizzato premendo il bottone)**" compariranno
> poi due ulteriori campi mediante i quali poter rispettivamente:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\griglia_collapse.bmp](./assets/media/image104.png)

- **Immagine del bottone di Collapse**: consente di indicare la
  specifica immagine da utilizzare per il pulsante di apertura della
  Griglia (l'unico elemento visualizzato inizialmente all'interno della
  pagina web)

- **Testo del bottone di Collapse:** consente di indicare il testo da
  utilizzare per il pulsante di apertura della Griglia (l'unico elemento
  visualizzato inizialmente all'interno della pagina web)

> Come per l'opzione Off Canvas, anche in questo caso, inizialmente, i
> contenuti della Griglia non saranno visibili all'interno della pagina
> (né sul front end né tanto meno sul back end del sito) per cui per
> poterli editare e gestire correttamente sarà necessario per prima cosa
> renderli visibili cliccando per questo sul relativo pulsante di
> apertura esattamente come farebbe un normale visitatore del sito
>
> Una volta reso visibile il Contenitore Collassabile sarà poi possibile
> gestirlo sia a livello grafico che a livello di contenuti secondo le
> normali modalità di interazione proprie di Passweb

Il pulsante "**Salva**" presente nella parte alta della maschera
consentirà di salvare tutte le modifiche apportate al componente in
oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali" di questo
manuale.

**ATTENZIONE! Una volta settati i parametri di configurazione della
Griglia sarà necessario, ovviamente, andare a definire le colonne da
inserire al suo interno stabilendo anche il comportamento che queste
colonne dovranno avere in corrispondenza delle diverse risoluzioni del
dispositivo di visualizzazione del sito.**

In questo senso va detto dunque che il Componente "Contenitore Griglia"
è a tutti gli effetti un componente di tipo contenitore e come tale
andrà trattato.

Sarà quindi necessario per prima cosa accedere alla gestione dei
componenti interni al Contenitore Griglia e successivamente abilitare la
modalità di aggiunta nuovi componenti.

La differenza rispetto ad un normale componente Contenitore è
rappresentata dal fatto che all'interno della griglia potranno essere
inseriti solo ed esclusivamente delle Colonne che saranno a loro volta
dei componenti di tipo Contenitore.

Sarà quindi all'interno di queste colonne che andranno poi inseriti e
gestiti i reali contenuti del sito (es. Paragrafi, Immagini, Tabs ,
Contenitori, Offerte ecc...)

