# ACQUISTO DA UNA LISTA REGALO



Dopo aver creato e condiviso una Lista Regalo, l'ultimo step sarà
ovviamente quello che prevede l'acquisto degli articoli in essa presenti
da parte degli "invitati" alla Lista stessa.

Affinchè questo possa avvenire è necessario, innanzitutto, accertarsi di
aver **creato e configurato correttamente la pagina "Lista Regalo"
inserendo al suo interno l'omonimo componente**.

**E' infatti a partire da questa pagina e grazie a questo componente che
gli invitati alla Lista potranno acquistare gli articoli in essa
presenti**

Per maggiori informazioni relativamente alla corretta configurazione del
Componente "Lista Regalo" si rimanda ai precedenti capitoli di questo
manuale ("*Varianti Sito Responsive -- Lista Componenti Ecommerce --
Componente Lista Regalo -- Configurazione*")

In queste condizioni dunque, nel momento in cui un invitato dovesse
accedere alla pagina "Lista Regalo" del sito, potrebbero configurarsi,
dipendentemente da come la lista stessa è stata condivisa, due diverse
possibili situazioni. Ogni Lista Regalo è infatti accessibile in due
modi diversi:

- **Tramite link diretto** -- es.
  <https://www.clobis.net/it/lista-regalo/giftrid/B39565032221> --
  (giftrid è una porzione del permalink gestita in automatico
  dall'applicazione e che non corrisponde quindi ad una vera e propria
  pagina del sito) fornito agli invitati mediante condivisione della
  lista (effettuata via mail o via social)

- **Tramite Ricerca** inserendo, in questo senso, l'identificativo della
  Lista Regalo all'interno del corrispondente pannello di ricerca
  presente alla pagina "Lista Regalo" del sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ricerca_lista_regalo.bmp](./assets/media/image234.png)

> Nulla vieta infatti al gestore della lista di far pervenire ai suoi
> invitati, nella maniera che ritiene più opportuna, l'identificativo
> della lista da lui creata con le eventuali istruzioni di utilizzo.
>
> **ATTENZIONE!** **L'identificativo della Lista Regalo è una stringa
> univoca di 12 caratteri assegnato alla lista stessa in maniera
> completamente automatica dall'applicazione, al momento della sua
> creazione (es. B39565032221).**
>
> Tale identificativo può essere prelevato direttamente dall' url
> presente nella barra degli indirizzi del browser nel momento in cui si
> decida di visualizzare l'anteprima della Lista in esame (è l'ultima
> parte del permalink di pagina), oppure dal relativo campo presente nel
> form di modifica della Lista stessa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\identificativo_lista_regalo.bmp](./assets/media/image235.png)

> **ATTENZIONE!** Per visualizzare il campo "**Identificativo Evento**"
> (campo ovviamente non editabile) è necessario salvare la Lista Regalo
> e cliccare poi sul pulsante "**Modifica**" presente in corrispondenza
> della Lista stessa all'interno della tabella delle Wishlist

In ogni caso una volta caricata la specifica Lista Regalo, l'utente si
troverà di fronte un mini catalogo contenente esattamente tutti gli
articoli che il creatore della lista desidererebbe ricevere, ordinati,
magari, per priorità di acquisto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_acquisto_1.bmp](./assets/media/image236.png)

Nella parte alta della pagina, immediatamente al di sotto del pannello
di ricerca, verranno inoltre visualizzate anche tutte le informazioni
(es. immagine, organizzatori, luogo e data dell'evento ecc...) relative
alla Lista Regalo in esame.

**ATTENZIONE!** Gli articoli visualizzati all'interno del componente
"Lista Regalo" varieranno, ovviamente, in relazione alla specifica Lista
selezionata per cui nel momento in cui un utente dovesse accedere alla
pagina "Lista Regalo" senza aver selezionato o indicato una specifica
Lista il componente potrebbe essere privo di articoli.

**In generale verrà comunque mantenuto in sessione l'identificativo
dell'ultima Lista Regalo visualizzata** per cui, una volta visualizzati
gli articoli presenti all'interno di una certa lista se, durante la
stessa sessione di navigazione, lo stesso utente dovesse accedere con lo
stesso browser alla pagina "Lista Regalo" verrà comunque visualizzata
l'ultima Lista Regalo consultata senza doverla per forza di cose
ricercare dall'apposito pannello di ricerca

Le modalità di acquisto degli articoli presenti all'interno di una Lista
Regalo sono, di base, le stesse con cui si acquista un qualsiasi altro
articolo presente all'interno del sito.

In questo senso però è bene evidenziare alcune cose di fondamentale
importanza che caratterizzano l'acquisto di articoli appartenenti ad una
Lista Regalo rispetto a quelli che sono gli articoli presenti
all'interno del "tradizionale" catalogo web.

Nello specifico è bene sottolineare che

- Per ogni articolo presente in lista, accanto alla quantità da
  acquistare verrà visualizzato anche un ulteriore campo all'interno del
  quale sarà indicata la quantità attualmente ricevuta, per il relativo
  articolo, dal gestore della lista.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\agg_carrello_lista_regalo.bmp](./assets/media/image237.png)

> **Inoltre, la quantità visualizzata a default nel campo di input sarà
> data dalla differenza tra la quantità desiderata e quella attualmente
> ricevuta.**

- Nel caso in cui per un dato articolo presente in lista **la quantità
  ricevuta dovesse essere uguale alla quantità desiderata**, non verrà
  mostrato il pulsante di "Aggiunta al carrello", ma verrà visualizzato
  al suo posto un testo di "**Articolo completato**" (personalizzabile
  alla sezione Testi/Messaggi Sito del Wizard)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_acquisto_2.bmp](./assets/media/image238.png)

- Per articoli a taglie verrà sempre utilizzata la "**Modalità grafica
  estesa**", con la possibilità di impostare a zero la quantità di una
  determinata taglia in maniera tale da evitare che essa venga poi
  aggiunta in carrello.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\taglie_in_lista_regalo.bmp](./assets/media/image239.png)

- I prezzi degli articoli presenti in Lista Regalo sono sottoposti ad
  eventuali particolarità prezzo e/o sconto associate all'utente che sta
  effettuando l'acquisto e non ad eventuali particolarità definite per
  il creatore/gestore della lista

- E' possibile acquistare articoli appartenenti ad una data Lista Regalo
  solo ed esclusivamente a partire da questa stessa Lista Regalo
  (cliccando cioè sul pulsante di "Aggiunta in Carrello" presente
  all'interno delle celle della Lista).

> **ATTENZIONE! Inserimenti in carrello di articoli presenti in una
> certa Lista Regalo, fatti però a partire dalla relativa pagina
> Catalogo e/o dalla relativa Scheda Prodotto non saranno vincolati in
> alcun modo alla corrispondente Lista Regalo**

- **Non è possibile aggiungere in carrello, contemporaneamente, articoli
  appartenenti ad una Lista Regalo e articoli che non hanno nulla a che
  vedere con essa**.

> Nel caso in cui un'utente dovesse quindi inserire in carrello un
> articolo di una certa Lista Regalo (partendo ovviamente dalla Lista
> stessa) e, successivamente, dovesse poi tentare di aggiungere anche un
> altro articolo partendo però, questa volta, dal Catalogo Web, dalla
> relativa Scheda Prodotto o addirittura da una Lista diversa dalla
> precedente, verrà visualizzato un apposito messaggio di errore e
> l'articolo in esame, ovviamente, non verrà aggiunto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_messaggio_errore_1.bmp](./assets/media/image240.png)

> Il messaggio in questione può essere personalizzato dalla sezione
> "Testi / Messaggi del Sito" agendo sul testo "**Articolo non relativo
> alla Lista Regalo**" presente in corrispondenza del componente
> "**Aggiunta in Carrello**"
>
> Allo stesso modo nel caso in cui un'utente dovesse inserire in
> carrello un articolo "generico" partendo cioè dal Catalogo Web e/o
> dalla relativa Scheda Prodotto, e successivamente dovesse poi tentare
> di aggiungere anche un articolo, appartenente questa volta però ad una
> certa Lista Regalo (partendo quindi dalla Lista stessa), verrà
> visualizzato un altro messaggio di errore e l'articolo in esame,
> ovviamente, non verrà aggiunto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_messaggio_errore_2.bmp](./assets/media/image241.png)

> Anche in questo caso il messaggio di errore può essere personalizzato
> dalla sezione "Testi / Messaggi del Sito" agendo questa volta sul
> testo "**Articolo relativo ad una Lista Regalo**" presente in
> corrispondenza del componente "**Aggiunta in Carrello**"

- In fase di checkout, come indirizzo di spedizione, **verrà selezionato
  a default l'indirizzo indicato dal gestore della lista in fase di
  creazione della Lista stessa,** posto ovviamente di aver inserito
  correttamente nel form di creazione della lista regalo anche il campo
  relativo all'indirizzo di spedizione.

> Per maggiori informazioni in merito si veda anche la sezione "*Utenti
> -- Wishlist -- Gestione Liste Regalo -- Tipologia*" di questo manuale.
>
> In ogni chi acquista dalla lista regale potrà sempre avere la
> possibilità di modificare questa impostazione indicando quindi un suo
> specifico indirizzo di spedizione (nel caso ad esempio in cui volesse
> farsi arrivare a casa la merce per poi consegnarla di persona al
> gestore delle lista)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_acquisto_3.bmp](./assets/media/image242.png)

- In fase di conferma ordine (nel momento cioè in cui l'ordine verrà
  inserito sul gestionale) verrà inviata una mail al gestore della lista
  contenente il dettaglio del relativo documento e, contestualmente,
  verranno aggiornate anche le "Quantità Ricevute" per gli articoli
  presenti in ordine

> **ATTENZIONE!** Gli ordini inerenti Liste Regalo avranno nel corpo del
> documento un'apposita nota con l'indicazione della Lista cui l'ordine
> stesso fa riferimento (**#RIF LISTA REGALO n \<numero\>#**)
>
> Per maggiori informazioni relativamente all'invio della mail si veda
> anche la sezione "*Ordini -- Configurazione Ordini -- Dati Email*" di
> questo manuale

- **In caso di variazione di un ordine legato ad una Lista Regalo (es.
  cancellazione dell'intero ordine, modifica delle quantità, rimozione
  di alcune righe ecc...) sarà poi necessario aggiornare manualmente i
  valori delle quantità ricevute agendo, in questo senso, dalla
  corrispondente sezione del Wizard**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\wizard_dettaglio_lista_regalo.bmp](./assets/media/image243.png)

> Per maggiori informazioni in merito si veda anche la sezione
> **"***Utenti -- Wishlist -- Gestione Liste Regalo***"** di questo
> manuale

- **In fase di aggiunta articoli in carrello, di modifica delle quantità
  e durante il passaggio dal carrello al checkout** (sempre in relazione
  ovviamente ad ordini inerenti ad una data Lista Regalo) verrà
  effettuato un controllo sulle quantità indicate per gli articoli in
  ordine rispetto a quelle effettivamente rimaste in Lista.

> In queste condizioni nel caso in cui la quantità indicata per un dato
> articolo dovesse superare quella ancora disponibile in Lista, verrà
> visualizzato un apposito messaggio di errore con evidenziata
> l'effettiva quantità ancora acquistabile per quello stesso articolo e,
> contemporaneamente, verranno anche aggiornate le quantità in ordine
> con i valori corretti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\lista_regalo_messaggio_errore_3.bmp](./assets/media/image244.png)

> Come per gli altri messaggi di errore anche in questo caso è possibile
> personalizzare il testo del messaggio dalla sezione "Testi / Messaggi
> del Sito" del Wizard agendo, nello specifico, sui testi "**Massima
> disponibilità Lista Regalo**" e "**Massima disponibilità taglia Lista
> Regalo**" presente in corrispondenza del componente "**Aggiunta in
> Carrello**"

