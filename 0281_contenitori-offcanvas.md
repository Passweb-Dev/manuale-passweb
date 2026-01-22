# CONTENITORI OFFCANVAS



Per poter gestire un Contenitore e tutto il suo contenuto come elementi
Offcanvas è sufficiente selezionare il relativo parametro presente nella
maschera di configurazione del Contenitore stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenitore_offcanvas_0.bmp](./assets/media/image93.png){width="4.363888888888889in"
height="3.1625in"}

**Menu Offcanvas:** consente di trattare il Contenitore che si sta
considerando nello stesso modo in cui vengono trattati i Menu Off
Canvas.

Selezionando questa opzione dunque, il Componente Contenitore (e gli
elementi in esso contenuti) verrà posizionato, inizialmente, al di fuori
della pagina web dove invece comparirà soltanto un pulsante.

Cliccando su questo pulsante il Contenitore verrà richiamato e
visualizzato nella pagina secondo quelle che sono le impostazioni
settate dall'amministratore in fase di configurazione del componete
stesso.

![Videate\\contenitore_offcanvas.bmp](./assets/media/image94.png){width="5.110416666666667in"
height="3.2402777777777776in"}

**ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
inserire all'interno del Contenitore gestito come elemento Offcanvas più
contenuti corrispondenti a più Componenti Passweb, sarà necessario
racchiudere tutti questi componenti all'interno di un ulteriore
Componente Contenitore (che dovrà quindi essere il primo elemento
presente all'interno del contenitore offcanvas). In caso contrario
infatti non tutti gli elementi dell'offcanvas potrebbero essere
visualizzati correttamente

Una volta selezionato questo parametro, compariranno quindi ulteriori
campi mediante i quali poter impostare rispettivamente:

- **Inizializzazione menù:** consente di impostare la modalità di
  apertura iniziale del contenitore

- **Posizionamento del menu:** consente di indicare la posizione in cui
  dovrà essere visualizzato il Contenitore nel momento in cui l'utente
  dovesse decidere di richiamarlo. È possibile decidere di visualizzarlo
  sulla parte sinistra / destra oppure nella parte alta / bassa della
  pagina stessa

- **Sposta il contenuto del sito all'apertura del menu:** se selezionato
  nel momento in cui l'utente dovesse decidere di richiamare il
  Contenitore, questo verrà visualizzato facendo scorrere la parte
  restante della pagina web verso sinistra/destra/alto/basso
  dipendentemente dalle impostazioni settate per il precedente
  parametro.

> Nel caso in cui il parametro in oggetto non venga selezionato, il
> Contenitore verrà invece visualizzato andando a sovrapporsi ai
> contenuti della pagina lasciando comunque una porzione della pagina
> stessa sempre visibile.

- **Immagine per Off canvas:** consente di indicare la specifica
  immagine da utilizzare per il pulsante di apertura del Contenitore
  (l'unico elemento visualizzato inizialmente all'interno della pagina
  web).

> È possibile indicare una delle immagini presenti nel database del sito
> oppure uno degli Attributi Immagine gestiti (campo "**Attributi
> Temi**").
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![Videate\\icona_menu_offcanvas.bmp](./assets/media/image95.png){width="0.2465277777777778in"
> height="0.21458333333333332in"}

- **Alt-text immagine offcanvas**: consente di impostare, in tutte le
  lingue attualmente gestite all'interno del sito, il valore che dovrà
  avere l'attributo alt assegnato all'immagine impostata in
  corrispondenza del precedente parametro "Immagine per Off canvas"

- **Testo del bottone offcanvas**: consente di indicare il testo di un
  eventuale label da mostrare a fianco dell'immagine di apertura del
  Contenitore

Ora, considerando che, come appena detto, i Contenitori Offcanvas sono
posizionati inizialmente al di fuori della pagina web (e questo non solo
sul front end del sito ma anche all'interno del back end), **per poterli
gestire sia dal punto di vista grafico che, soprattutto, dal punto di
vista dei loro contenuti e quindi degli ulteriori elementi da inserire
al loro interno, la prima cosa da fare sarà ovviamente quella di
richiamarli rendendoli visibili all'interno della pagina.**

Per far questo sarà sufficiente cliccare sul relativo pulsante di
apertura esattamente come farebbe un normale visitatore del sito.

In alternativa è anche possibile cliccare sulla corrispondente icona di
apertura
(![Videate\\icona_apri_chiudi_menu.bmp](./assets/media/image96.png){width="0.1361111111111111in"
height="0.14305555555555555in"}) presente nel R.O.C. di questa
particolare tipologia di componente

**ATTENZIONE!** A differenza di quanto avveniva per i Menu Off Canvas,
la visualizzazione dei Contenitori Off Canvas all'interno dell'ambiente
di sviluppo è leggermente diversa rispetto a quella che sarà poi la
visualizzazione di questi stessi elementi sul front end del sito.

In effetti indipendentemente da quelle che sono le opzioni di
configurazione del componente, questo, **all'interno dell'ambiente di
sviluppo, verrà visualizzato sempre e soltanto al di sotto del pulsante
di apertura** in maniera tale da poter poi inserire in esso ulteriori
componenti utilizzando le solite modalità di interazione proprie di
Passweb.

In queste condizioni, per avere un'idea chiara soprattutto del
dimensionamento dei vari elementi, si consiglia sempre di controllare il
risultato finale sul front end del sito.

