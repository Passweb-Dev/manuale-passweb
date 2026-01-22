# CHECKOUT A STEP CON ACCORDION



Impostando il parametro "**Tipologia Fase di Checkout**" presente nella
maschera di configurazione del componente "Ordine Custom Checkout)"
sull'opzione "**Visualizzazione a Step con Accordion**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\checkout_step_accordion.bmp](./assets/media/image292.png)

la procedura di conferma ordine verrà gestita attraverso un componente
di tipo Accordion e sarà quindi organizzata a step verticali.

In ogni step dovranno essere inserite informazioni di un determinato
tipo (tipo di documento da generare, metodo di trasporto, pagamento
ecc...) e il numero di step potrà variare in relazione alle specifiche
configurazioni adottate per la gestione dell'ordine.

In queste condizioni occorre inoltre ricordare che:

- **Il passaggio ad uno step successivo potrà avvenire, cliccando sul
  relativo pulsante "Procedi", soltanto dopo aver inserito tutte le
  informazione obbligatorie richieste dallo step corrente.**

- Arrivati ad un determinato step sarà sempre possibile tornare indietro
  e modificare le scelte precedentemente effettuate. In questo senso per
  tornare a step precedenti è possibile utilizzare l'apposito pulsante
  "Indietro" o cliccare sull'intestazione della relativa sezione e
  passare quindi anche ad uno step che non è quello immediatamente
  precedente all'attuale. Una volta tornati indietro per procedere oltre
  sarà però necessario passare attraverso ogni singolo step cliccano per
  questo sul pulsante "Procedi"

- Ogni volta che si passa ad uno step successivo verranno valutati i
  dati inseriti nello step attuale e, se necessario, verranno aggiornati
  i relativi totali dell'ordine (es. si è impostato un pagamento con una
  spesa accessoria, si è modificato un' indirizzo di spedizione ...)

- Eventuali campi custom gestiti mediante Set di Opzioni Ordine verranno
  inseriti nello Step relativo alle Note

- Nel momento in cui dovesse essere abilitata la gestione del pagamento
  / spedizione abituale e l'utente che effettua l'ordine dovesse avere
  effettivamente un pagamento / spedizione abituale già associato nella
  relativa anagrafica gestionale con associato anche un determinato
  costo aggiuntivo, i totali dell'ordine potrebbero già, nel primo step,
  prendere in considerazione anche questi eventuali costi aggiuntivi
  (che potranno comunque essere modificati nel momento in cui l'utente
  dovesse selezionare, negli step successivi, un diverso pagamento e/o
  una diversa modalità di spedizione)

- In assenza di eventuali spedizioni abituali o già selezionate a
  default, i costi di spedizione verranno applicati e visualizzati nei
  totali dell'ordine solo dopo che l'utente avrà confermato il suo
  indirizzo di spedizione. Nello specifico questo potrà avvenire nello
  step dedicato alla selezione degli indirizzi di spedizione, nel caso
  in cui non dovesse essere abilitato il One Page Checkout, oppure, con
  il One Page Checkout abilitato, già in uscita dal primo step dove
  l'utente avrà effettivamente dichiarato l'indirizzo di spedizione da
  utilizzare.

- In assenza di eventuali pagamenti abituali o già selezionati a
  default, i costi aggiuntivi verranno applicati e visualizzati nei
  totali del documento solo dopo che l'utente avrà indicato
  esplicitamente, nel relativo step, la modalità di pagamento che
  intende utilizzare

**ATTENZIONE!** Nel momento in cui si dovesse decidere di adottare
questa particolare tipologia di checkout e, allo stesso tempo, di
utilizzare anche il One Step Checkout per rendere possibile la creazione
di un ordine come utente "Ospite", sarà di fondamentale importanza
accertarsi di rendere visibile il componente "Registrazione", inserito
nel primo step, a tutti gli utenti del sito

Se il componente "Registrazione" dovesse infatti essere visibile solo a
determinati gruppi utente potrebbero anche configurarsi delle situazioni
in cui il primo step del checkout risulterà vuoto impendendo di fatto
agli utenti di completare l'ordine.

In questa particolare configurazione, infine, non sarà possibile
visualizzare il riepilogo degli articoli in ordine assieme ai vari step
di conferma

