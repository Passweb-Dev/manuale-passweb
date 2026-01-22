# GESTIONE DEI CONTENUTI INTERNI AL CONFIGURATORE



Nel precedente capitolo di questo manuale abbiamo evidenziato come per
quel che riguarda la logica di gestione dei contenuti interni al
componente Configuratore questo possa essere considerato a tutti gli
effetti come un componente di tipo Contenitore.

**In realtà sotto questo aspetto il Configuratore viene gestito in
maniera leggermente diversa rispetto a tutti gli altri Componenti
Ecommerce di tipo Contenitore**.

In questo caso infatti i vari componenti che potremo andare ad inserire
all'interno del Configuratore serviranno essenzialmente per visualizzare
determinate informazioni (es. immagine articolo, codice, descrizione,
attributi aggiuntivi ecc...) relativamente alle diverse possibili
configurazioni di prodotto finito che potranno poi essere visualizzate
all'interno del configuratore stesso.

Ora il fatto di poter visualizzare direttamente all'interno del
configuratore le diverse possibili configurazioni di prodotto finito
(quindi i diversi possibili articoli figlio) oppure ricaricare l'intera
scheda prodotto sostituendo i dati dell' articolo padre inizialmente
visualizzati con quelli dello specifico articolo figlio che l'utente è
arrivato a selezionare, dipende esattamente dalla particolare modalità
di visualizzazione che si è deciso di adottare per la struttura cui
appartiene lo specifico articolo padre.

In questo senso infatti è bene ricordare che

- Nel caso in cui per la struttura in esame sia stata impostata una
  modalità di visualizzazione lineare, una volta configurato uno
  specifico prodotto finito e posto ovviamente che il corrispondente
  articolo sia già stato codificato sul gestionale ed esportato
  all'interno del sito, tutte le informazioni inizialmente visualizzate
  all'interno della scheda prodotto dell'articolo padre (immagini,
  singoli Attributi Articolo, interi Set di Attributi ...), verranno
  ricaricate e sostituite dalle stesse informazioni relative però allo
  specifico prodotto finito.

> Nel caso in cui l'articolo figlio configurato dall'utente non sia
> ancora gestito all'interno del sito continueranno invece ad essere
> visualizzate le stesse informazioni dell'articolo padre.
>
> **In ogni caso in queste condizioni (Modalità di Visualizzazione
> Lineare) all'interno del Configuratore non verranno mai visualizzate
> le diverse possibili configurazioni di articoli figlio per cui non
> verranno visualizzati neppure eventuali componenti inseriti, lato
> Wizard, all'interno del Configuratore stesso.**

![Videate\\modalita_visualizzazione_lineare.bmp](./assets/media/image111.png)

> In definitiva dunque, in queste condizioni, il componente
> Configuratore verrà trattato come un normale componente che non
> ammette al suo interno altri contenuti se non quelli definiti dalla
> logica di funzionamento del componente stesso. Gli unici contenuti del
> configuratore saranno quindi le diverse possibili opzioni di scelta
> presenti in corrispondenza dei vari livelli di selezione e di
> configurazione del prodotto finito.

- Nel caso in cui per la struttura in esame sia stata impostata invece
  una modalità di visualizzazione Tabellare (Tabella Esplosa, Tabella
  Esplosa Divisa o Tabella Matrice), gli ultimi due livelli della
  struttura oppure l'ultimo livello più la Taglia/Colore del prodotto
  (nel caso in cui ovviamente l'articolo strutturato in esame sia
  gestito mediante la tabella Taglie/Colori di Mexal) verranno
  visualizzati all'interno di una tabella in cui ogni cella rappresenta
  una specifica configurazione di prodotto finito e dunque uno specifico
  articolo figlio.

> **In queste condizioni quindi non verrà mai ricaricata la scheda
> prodotto dell'articolo padre per visualizzare le informazioni di uno
> specifico articolo figlio in quanto tali informazioni saranno già
> presenti all'interno della cella relativa a quello stesso articolo
> figlio e dipenderanno esattamente da quelli che sono i componenti
> inseriti, lato Wizard, all'interno del Configuratore**

![Videate\\modalita_visualizzazione_tabella_matrice.bmp](./assets/media/image114.png)

> In definitiva dunque, in queste condizioni, il Configuratore verrà
> trattato effettivamente come un Componente di tipo Contenitore e i
> dati visualizzati, per ogni singolo articolo figlio presente
> all'interno della tabella, dipenderanno da quelli che sono i
> componenti inseriti all'interno del Configuratore stesso.

La modalità di inserimento di eventuali componenti interni al
configuratore è la medesima adottata per tutti gli altri componenti
Passweb. Sarà quindi necessario attivare la modalità di gestione dei
componenti, portarsi sul Componente Configuratore e, alla comparsa del
R.O.C. cliccare sull'icona "**Accedi ai componenti interni".**

Nello specifico poi all'interno in un Componente Configuratore, potranno
essere inserti oltre ovviamente a componenti comuni quali Paragrafo,
Immagine, Contenitore, Griglia ecc... anche i seguenti Componenti
Ecommerce:

- **Titolo:** inserendo questo componente, all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzato il
  Titolo del corrispondente articolo figlio, posto ovviamente che tale
  articolo sia stato correttamente esportato e gestito anche all'interno
  del sito.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito verrà visualizzato il Titolo
> dell'articolo padre più la descrizione della configurazione della
> struttura che ha portato alla definizione di quello specifico articolo
> figlio

- **Immagine Rappresentativa:** inserendo questo componente, all'interno
  del Configuratore, in ogni cella della tabella, verrà visualizzata l'
  "Immagine Catalogo" del corrispondente articolo figlio, posto
  ovviamente che tale articolo sia stato correttamente esportato e
  gestito anche all'interno del sito.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito verrà visualizzata l'
> "Immagine Catalogo" dell'articolo padre

- **Descrizione:** inserendo questo componente, all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzata la
  Descrizione del corrispondente articolo figlio, posto ovviamente che
  tale articolo sia stato correttamente esportato e gestito anche
  all'interno del sito.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito verrà visualizzata la
> Descrizione dell'articolo padre

- **Prezzo:** inserendo questo componente, all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzato il
  Prezzo del corrispondente articolo figlio, posto ovviamente che tale
  articolo sia stato correttamente esportato e gestito anche all'interno
  del sito e che abbia ovviamente un suo specifico Prezzo.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito, o non abbia un suo prezzo
> specifico, verrà visualizzato il Prezzo calcolato a partire dal prezzo
> dell'articolo padre più l'utilizzo di eventuali modificatori presenti
> nella configurazione della struttura che ha portato alla definizione
> di quello specifico articolo figlio

- **Dati Articolo:** inserendo questo componente, all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzata
  l'informazione corrispondente per il relativo articolo figlio posto
  ovviamente che tale articolo sia stato correttamente esportato e
  gestito anche all'interno del sito.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito verrà l'informazione
> corrispondente relativa però all'articolo padre

- **Disponibilità:** inserendo questo componente all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzata la
  disponibilità (o il pulsante per richiederla dipendentemente da come è
  stato configurato il componente stesso) del corrispondente articolo
  figlio, posto ovviamente che tale articolo sia stato correttamente
  esportato e gestito anche all'interno del sito.

> Nel caso in cui l'articolo figlio in esame non sia stato ancora
> esportato e gestito all'interno del sito la disponibilità mostrata
> sarà quella relativa al padre

- **Notifica Disponibilità:** inserendo questo componente in ogni cella
  della tabella, verrà visualizzato, se il relativo articolo figlio è
  esaurito, il componente per la richiesta di notifica disponibilità.

> Nel caso in cui il relativo articolo figlio non sia ancora esaurito o
> non sia stato esportato e gestito all'interno del sito, ovviamente non
> verrà visualizzato nulla

- **Rating Review:** inserendo questo componente all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzato il
  rating del corrispondente articolo figlio, posto ovviamente che tale
  articolo sia stato correttamente esportato e gestito anche all'interno
  del sito.

> Nel caso in cui il relativo articolo figlio non sia ancora esaurito o
> non sia stato esportato e gestito all'interno del sito verrà
> visualizzato il Rating dell'articolo padre

- **Aggiunta al Comparatore:** inserendo questo componente all'interno
  del Configuratore, in ogni cella della tabella, verrà visualizzato il
  pulsante per aggiungere al comparatore il corrispondente articolo
  figlio.

> Nel caso in cui l'articolo figlio non dovesse ancora essere stato
> esportato e gestito all'interno del sito, verrà aggiunto al
> Comparatore l'articolo padre con la descrizione della configurazione
> della struttura che ha portato alla definizione di quello specifico
> articolo figlio
>
> **ATTENZIONE!** nel momento in cui l'esigenza dovesse essere quella di
> aggiungere automaticamente al Comparatore più articoli
> contemporaneamente e senza dover quindi cliccare ogni volta sul
> pulsante di aggiunta, sarà sufficiente gestire un componete
> "**Aggiunta al Comparatore**" anche esternamente al configuratore.
>
> Cliccando infatti sul pulsante di aggiunta al comparatore posto al di
> fuori del configuratore verranno automaticamente inseriti in
> comparazione tutti gli articoli presenti all'interno della tabella del
> configuratore per i quali è stata indicata una quantità maggiore di 0

- **Aggiunta alla Wishlist:** inserendo questo componente all'interno
  del Configuratore, in ogni cella della tabella, verrà visualizzato il
  pulsante per aggiungere il corrispondente articolo figlio alla
  Wishlist.

> Nel caso in cui l'articolo figlio non dovesse ancora essere stato
> esportato e gestito all'interno del sito, verrà aggiunto alla Wishlist
> l'articolo padre con la descrizione della configurazione della
> struttura che ha portato alla definizione di quello specifico articolo
> figlio
>
> **ATTENZIONE!** nel momento in cui l'esigenza dovesse essere quella di
> aggiungere automaticamente in Wishlist più articoli contemporaneamente
> e senza dover quindi cliccare ogni volta sul pulsante di aggiunta,
> sarà sufficiente gestire un componete "**Aggiunta alla Wishlist**"
> anche esternamente al configuratore.
>
> Cliccando infatti sul pulsante di aggiunta alla wishlist posto al di
> fuori del configuratore verranno automaticamente inseriti in wishlist
> tutti gli articoli presenti all'interno della tabella del
> configuratore per i quali è stata indicata una quantità maggiore di 0

- **Aggiunta al Carrello:** inserendo questo componente all'interno del
  Configuratore, in ogni cella della tabella, verrà visualizzato il
  campo di input necessario per definire la quantità con cui si desidera
  aggiungere in carrello il corrispondente articolo figlio.

> **ATTENZIONE!** nelle singole celle della tabella del configuratore
> sarà presente il campo di input delle quantità ma non il pulsante di
> aggiunta in carrello
>
> **In queste condizioni sarà quindi necessario gestire un componente
> "Aggiunta al Carrello" anche esternamente al configuratore**.
>
> A differenza di quello inserito all'interno del configuratore infatti,
> il componente "Aggiunta al Carrello" gestito esternamente avrà il solo
> pulsante di aggiunta (e non il campo di input delle quantità) e
> cliccando su di esso verranno automaticamente inseriti in carrello
> tutti gli articoli presenti all'interno della tabella del
> configuratore per i quali è stata indicata una quantità maggiore di 0

