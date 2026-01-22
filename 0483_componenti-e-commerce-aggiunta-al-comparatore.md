# COMPONENTI E-COMMERCE -- AGGIUNTA AL COMPARATORE



Il Componente **"Aggiunta al Comparatore"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_aggiunta_comparatore_res.bmp](./assets/media/image510.png){width="2.5340277777777778in"
height="3.1041666666666665in"}

consente di inserire all'interno corrispondente Componente Ecommerce di
primo livello (es. Catalogo Ecommerce), un pulsante mediante il quale
poter aggiungere lo specifico articolo al Comparatore.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_ecommerce_aggiungi_comparatore.bmp](./assets/media/image511.png){width="5.588888888888889in"
height="3.8159722222222223in"}

Per maggiori informazioni relativamente alla gestione in Passweb del
componente "Comparatore" si veda anche la relativa sezione di questo
manuale.

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\aggiungi_comparatore_configurazione_res.bmp](./assets/media/image512.png){width="5.760416666666667in"
height="3.675in"}

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
  che comparirà al passaggio del mouse sul pulsante di "Aggiungi al
  Comparatore"

- **Visualizza sempre il messaggio quando si aggiunge l'articolo:**
  selezionando questo parametro dopo aver aggiunto un articolo al
  Comparatore verrà sempre visualizzato un apposito messaggio di
  notifica per avvisare l'utente dell'avvenuta operazione
  (indipendentemente dal fatto che nella stessa pagina sia presente o
  meno anche il componente Mini Comparatore).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_aggiungi_comparatore.bmp](./assets/media/image513.png){width="5.631944444444445in"
height="3.8465277777777778in"}

> **ATTENZIONE**! Il messaggio di notifica può essere personalizzato
> inserendo l'apposito codice HTML all'interno del campo "**Aggiunta**"
> presente nella sezione "Gestione Testi / Messaggi del Sito" in
> corrispondenza del componente "**Aggiunta al Comparatore**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_aggiungi_comparatore_personalizzazione.bmp](./assets/media/image514.png){width="5.392361111111111in"
height="3.4784722222222224in"}

> Nel caso in cui il questo parametro non venga selezionato l'evento
> utilizzato dall'applicazione per notificare all'utente l'avvenuto
> inserimento nel Comparatore dell'articolo selezionato sarà diverso a
> seconda del fatto che nella stessa pagina sia presente o meno anche il
> componente Mini Comparatore. Nello specifico:

- **nel caso in cui nella pagina in questione non sia presente un
  componente Mini Comparatore** a seguito dell'aggiunta di una articolo
  al Comparatore verrà visualizzato lo stesso messaggio di notifica
  evidenziato nella figura sopra riportata

- **nel caso in cui nella pagina in questione sia presente anche un
  componente Mini Comparatore**, a seguito dell'inserimento di un
  articolo al Comparatore non verrà visualizzato nessun messaggio ma
  verrà avviata una specifica animazione per notificare all'utente
  l'avvenuto inserimento.

<!-- -->

- **Tempo di chiusura popup messaggio (ms):** consente di indicare
  l'intervallo di tempo (in millisecondi) trascorso il quale il popup di
  aggiunta al Comparatore si chiuderà in maniera automatica

- **Pagina di destinazione all'inserimento di un articolo nella lista di
  comparazione:** consente di specificare la pagina del sito cui
  l'utente verrà automaticamente ridiretto dopo aver cliccato sul
  pulsante "Aggiungi al Comparatore" ed aver completato la
  corrispondente azione.

> La ridirezione automatica verso una specifica pagina potrebbe
> impiegare un secondo in maniera tale da consentire ad eventuali
> animazioni collegate all'aggiunta dell'articolo al Comparatore di
> terminare correttamente.
>
> Nel caso in cui non sia presente nella stessa pagina in cui è inserito
> il componente "Aggiungi al Comparatore" anche il componente "Mini
> Comparatore", l'aggiunta di un articolo alla lista di comparazione non
> comporterà, come precedentemente evidenziato, l'avvio di nessuna
> animazione. In queste condizioni quindi dopo aver aggiunto l'articolo
> verrà visualizzato un messaggio relativo all'esito positivo
> dell'operazione e successivamente l'utente verrà ridiretto verso la
> specifica pagina di destinazione.

Relativamente all'inserimento di un articolo nella lista di comparazione
occorre inoltre ricordare che:

- Se l'articolo che si desidera aggiungere al comparatore è un padre di
  struttura, cliccando sul pulsante di Aggiunta al Comparatore l'utente
  verrà automaticamente ricondotto alla relativa pagina prodotto dove,
  prima di poter inserire l'articolo alla lista di comparazione, dovrà
  necessariamente indicare i vari elementi della struttura arrivando
  così a definire uno specifico articolo figlio.

- Se l'articolo che si desidera aggiungere al comparatore è un articolo
  a taglie/colori, questo potrà essere inserito nella lista di
  comparazione anche senza aver necessariamente indicato per esso una
  specifica taglia/colore

- Se si tenta di inserire nella lista di comparazione un articolo
  appartenente ad una categoria merceologica con associato un set di
  attributi differente da quello associato agli altri articoli già
  presenti nel comparatore, verrà visualizzato un apposito messaggio di
  errore e l'articolo non sarà inserito nella lista di comparazione.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

