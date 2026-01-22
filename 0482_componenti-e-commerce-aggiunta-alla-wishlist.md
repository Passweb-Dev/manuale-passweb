# COMPONENTI E-COMMERCE -- AGGIUNTA ALLA WISHLIST



Il Componente **"Aggiunta alla Wishlist"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_aggiunta_wishlist_res.bmp](./assets/media/image502.png){width="2.5340277777777778in"
height="3.1041666666666665in"}

consente di inserire all'interno del corrispondente Componente Ecommerce
di primo livello (es. Catalogo Ecommerce), un pulsante mediante il quale
poter aggiungere lo specifico articolo ad una delle proprie Wishlist.

Il funzionamento di tale pulsante potrà inoltre essere diverso a seconda
del fatto che l'utente abbia o meno effettuato l'autenticazione al sito.

In particolare:

- nel caso in cui l'utente **NON abbia ancora effettuato
  l'autenticazione**, cliccando sul pulsante in oggetto il relativo
  articolo verrà aggiunto alla "**Wishlist Corrente**" (l'unica
  effettivamente disponibile per utenti non autenticati).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_ecommerce_aggiungi_wishlist.bmp](./assets/media/image503.png){width="6.386805555555555in"
height="4.502777777777778in"}

- nel caso in cui, invece, l'utente **abbia già effettuato
  l'autenticazione al sito e abbia anche delle Wishlist precedentemente
  salvate,** accanto al pulsante di Aggiunta alla Wishlist comparirà
  anche una piccola freccia rivolta verso il basso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\aggiunta-ws-lista-regalo.bmp](./assets/media/image504.png){width="6.386805555555555in"
height="4.502777777777778in"}

> In queste condizioni cliccando sul pulsante in oggetto verrà aperto un
> piccolo menu contestuale contenente l'elenco (ordinato per nome) di
> tutte le Wishlist precedentemente create e salvate dall'utente stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\aggiunta-ws-lista-regalo2.bmp](./assets/media/image505.png){width="6.386805555555555in"
height="4.502777777777778in"}

> Oltre alle Wishlist salvate, ovviamente, sarà presente in elenco anche
> la "**Wishlist corrente"**, indicata come "**Nuova**" (il testo è
> comunque modificabile dalla sezione "Testi e Messaggi Sito" del Wizard
> agendo sul componente "Aggiunta alla Wishlist"), collocata come primo
> elemento della lista ed opportunamente evidenziata rispetto alle
> altre.
>
> L'utente avrà quindi la possibilità di selezionare una o più Wishlist
> tra quelle presenti (semplicemente selezionando l'apposito check) e
> cliccare sul pulsante "**Aggiungi**" per aggiungere il relativo
> articolo a tutte le Wishlist indicate.

Per maggiori informazioni relativamente alla gestione, in Passweb, delle
"Wishlist" (Liste dei desideri) si veda anche la sezione di questo
manuale relativa ai componenti Ecommerce "**Wishlist**" e/o "**Wishlist
Custom**"

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_aggiungi_wishlist_configurazione_res.bmp](./assets/media/image506.png){width="5.760416666666667in"
height="3.6625in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di impostare un nome per il Componente che si sta
  editando.

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

- **Title:** consente di indicare una stringa che verrà poi utilizzata
  come attributo title del componente e visualizzata quindi nel tooltip
  che comparirà al passaggio del mouse sul pulsante di "Aggiungi alla
  Wishlist"

- **Apertura Popup:** consente di decidere se il menu contestuale
  contenente l'elenco delle Wishlist precedentemente create dovrà
  aprirsi sopra o sotto al pulsante di aggiunta.

- **Visualizza sempre il messaggio quando si aggiunge l'articolo:**
  selezionando questo parametro dopo aver aggiunto un articolo alla
  Wishlist corrente verrà sempre visualizzato un apposito messaggio di
  notifica per avvisare l'utente dell'avvenuta operazione
  (indipendentemente dal fatto che nella stessa pagina sia presente o
  meno anche il componente Mini Wishlist).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_aggiungi_wishlist.bmp](./assets/media/image507.png){width="5.502777777777778in"
height="3.33125in"}

> **ATTENZIONE**! Il messaggio di notifica può essere personalizzato
> inserendo l'apposito codice HTML all'interno del campo "**Aggiunta**"
> presente nella sezione "Gestione Testi / Messaggi del Sito" in
> corrispondenza del componente "**Aggiunta alla Wishlist**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_aggiungi_wish_personalizzazione.bmp](./assets/media/image508.png){width="5.392361111111111in"
height="3.4784722222222224in"}

> In relazione a quelli che sono i contenuti del pop up di aggiunta in
> wishlist occorre poi sottolineare che le quantità eventualmente
> mostrate al suo interno dipenderanno anche dalle impostazioni settate
> per il parametro "**Gestione articoli in carrello / wishlist**"
> presente alla pagina "**Configurazione Catalogo**" del Wizard (menu
> "*Catalogo -- Catalogo Mexal / Ho.Re.Ca.*") e quindi dal fatto che
> l'aggiunta in carrello del prodotto selezionato vada a creare una
> nuova riga articolo oppure ad aggiornare una riga dello stesso
> prodotto già presente in carrello.
>
> In particolare nel momento in cui il parametro **Gestione articoli in
> carrello / wishlist** dovesse essere impostato sull'opzione:

- **Nuova riga articolo**: le quantità presenti nel pop up saranno
  sempre riferite alla quantità del prodotto che è stato effettivamente
  aggiunto indipendentemente dal fatto che in wishlist siano già
  presenti o meno altre righe dello stesso prodotto.

> In queste condizioni dunque se dovessimo andare ad aggiungere in
> wishlist, per due volte consecutive, un prodotto dal prezzo unitario
> pari a 38.61€ in quantità 2, in entrambi i casi verrà visualizzato un
> pop up del tipo di quello di seguito riportato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popup_aggiunta_wishlisti_nuova_riga.bmp](./assets/media/image509.png){width="2.3131944444444446in"
height="1.0555555555555556in"}

> in cui cioè la quantità indicata sarà sempre pari a 2

- **Modifica riga articolo**: quantità e subtotale presenti nel pop up
  di aggiunta faranno riferimento alle condizioni della riga del
  prodotto in esame eventualmente già presente in wishlist.

> In queste condizioni dunque se dovessimo andare ad aggiungere in
> carrello, per due volte consecutive, un prodotto dal prezzo unitario
> pari a 38.61€ in quantità 2, supponendo anche che inizialmente tale
> prodotto non sia presente in wishlist, la prima volta otterremo un pop
> up analogo al precedente quindi con quantità pari a 2.
>
> La seconda volta invece, considerando che l'articolo aggiunto è già
> presente in wishlist in quantità 2, all'interno del pop up di aggiunta
> verrà indicata una quantità pari a 4.
>
> **ATTENZIONE!** Nel caso in cui il parametro "**Visualizza sempre il
> messaggio quando si aggiunge l'articolo**" non venga selezionato
> l'evento utilizzato dall'applicazione per notificare all'utente
> l'avvenuto inserimento nella Wishlist corrente dell'articolo
> selezionato sarà diverso a seconda del fatto che nella stessa pagina
> sia presente o meno anche il componente Mini Wishlist. Nello
> specifico:

- **nel caso in cui nella pagina in questione NON sia presente un
  componente Mini Wishlist** a seguito dell'aggiunta di una articolo
  alla Wishlist corrente verrà visualizzato lo stesso messaggio di
  notifica evidenziato nella figura sopra riportata

- **nel caso in cui nella pagina in questione sia presente anche un
  componente Mini Wishlist**, a seguito dell'inserimento di un articolo
  alla Wishlist corrente non verrà visualizzato nessun messaggio ma
  verrà avviata una specifica animazione per notificare all'utente
  l'avvenuto inserimento.

<!-- -->

- **Tempo di chiusura popup messaggio (ms):** consente di indicare
  l'intervallo di tempo (in millisecondi) trascorso il quale il popup di
  aggiunta alla Wishlist si chiuderà in maniera automatica

- **Pagina di destinazione all'inserimento di un articolo in Wishlist:**
  consente di specificare la pagina del sito cui l'utente verrà
  automaticamente ridiretto dopo aver cliccato sul pulsante "Aggiungi
  alla Wishlist" ed aver completato la corrispondente azione.

> La ridirezione automatica verso una specifica pagina potrebbe
> impiegare un secondo in maniera tale da consentire ad eventuali
> animazioni collegate all'aggiunta dell'articolo in Wishlist di
> terminare correttamente.
>
> Nel caso in cui non sia presente nella stessa pagina in cui è inserito
> il componente "Aggiungi alla Wishlist" anche il componente "Mini
> Wishlist", l'aggiunta di un articolo in Wishlist non comporterà
> l'avvio di nessuna animazione. In queste condizioni quindi dopo aver
> aggiunto l'articolo in carrello verrà visualizzato un messaggio
> relativo all'esito positivo dell'operazione e successivamente l'utente
> verrà ridiretto verso la specifica pagina di destinazione.

**ATTENZIONE!** Il componente "Aggiungi alla Wishlist" **consente
l'inserimento dei vari articoli, nella Wishlist corrente, in quantità
intere o decimali** in perfetto accordo con quanto impostato per lo
specifico articolo all'interno del gestionale (ECommerce Mexal) o della
sua Anagrafica Passweb (Ecommerce Ho.Re.Ca.) e con quanto inserito
dall'utente all'interno del corrispondente campo di input delle
quantità.

Nello specifico infatti il componente "Aggiungi alla Wishlist" non ha un
suo campo di input per le quantità; in questo senso verranno quindi
considerate le quantità inserite nel campo di input relativo al
componente "Aggiungi al Carrello" presente all'interno della stessa
pagina.

Nel caso in cui all'interno della stessa pagina siano presenti più
componenti "Aggiungi in Carrello", per determinare la quantità
dell'articolo da inserire nella Wishlist, verrà considerata la quantità
indicata nel campo di input del componente "Aggiungi al Carrello" più
vicino (a livello di markup HTML) al componente "Aggiungi alla Wishlist"
utilizzato.

> **NOTA BENE:** nel caso in cui per uno specifico articolo non dovesse
> essere presente all'interno di componenti quali "Catalogo Ecommerce",
> "Offerte/Novità", "Risultati Ricerca", "Abbinati" ecc... il pulsante
> "Aggiungi al Carrello" e/o il corrispondente campo di input per
> l'inserimento delle quantità, il pulsante "Aggiungi alla Wishlist"
> permetterà comunque di inserire l'articolo nella Wishlist corrente ma
> solo in quantità unitaria. Eventuali variazioni in questo senso
> dovranno poi essere apportate direttamente all'interno dalla pagina di
> gestione delle Wishlist

In relazione alle diverse tipologie di articoli che possono o meno
essere inserite in Wishlist, occorre infine ricordare che:

- **Possono essere aggiunti** alla Wishlist anche articoli con "Prezzo a
  Richiesta" a patto che non siano Articoli a Taglie oppure Padri di
  Struttura. Inoltre nel caso in cui si aggiungano in Wishlist articoli
  con prezzo a richiesta, questi non potranno comunque essere poi
  trasferiti dalla Wishlist al Carrello

- **Possono essere aggiunti alla Wishlist articoli di tipo Campionario
  (non configurabili).** In questo caso in Wishlist comparirà lo stesso
  articolo Campionario presente in negozio, passandolo poi in carrello
  verranno esplosi anche i suoi componenti

- **Non possono essere aggiunti alla Wishlist** articoli a Taglie senza
  selezione di una specifica taglia, padri di struttura e/o Campionari
  configurabili senza aver prima stabilito per essi una specifica
  configurazione

- **Non possono essere aggiunti in Wishlist** Trattamenti e/o Servizi
  (siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.)

**ATTENZIONE!** In relazione agli articoli di tipo Campionario è di
fondamentale importanza ricordare che nel momento in cui dovessero
essere rimossi, lato gestionale, alcuni componenti di un dato
Campionario, tali componenti continueranno comunque ad essere
visualizzati in eventuali articoli Campionario precedentemente salvati
all'interno di una o più Wishlist (indipendentemente dal fatto che siano
Wishlist di tipo Personale o Lista Regalo)

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

