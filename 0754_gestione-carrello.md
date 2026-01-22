# GESTIONE CARRELLO



La sezione "**Gestione Carrello**" presente all'interno della maschera
"**Configurazione Catalogo**" consente di impostare:

- il comportamento del carrello utente in relazione alle operazioni di
  login /logout

- la specifica modalità di inserimento articoli in carrello / wishlist

- la modalità di gestione degli articoli Campionario in relazione ad
  eventuali filtri articolo che possono essere fatti all'interno di
  Passweb in fase di configurazione delle Promozioni, dei Buoni Sconto,
  dei Pagamenti, dei Metodi di Trasporto ecc...

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_catalogo_gestione_carrello.bmp](./assets/media/image9.png)

Nello specifico dunque il parametro:

**Gestione Carrello al Login:** consente di definire come dovrà essere
gestito, al login, il carrello utente.

E' possibile selezionare uno dei seguenti valori:

- **RILEVA CARRELLO UTENTE -- GESTIONE SEPARATA**

> Selezionando questa opzione, nel momento in cui un utente dovesse
> effettuare l'autenticazione al sito **senza aver aggiunto ( durante la
> stessa sessione) nessun articolo in carrello** verrà effettuata una
> ricerca per rilevare l'ultimo carrello eventualmente associato a
> quello stesso utente.
>
> Nel momento in cui tale ricerca dovesse dare esito positivo, Passweb
> **effettuerà una copia** del carrello rilevato caricandola poi sul
> front end del sito
>
> **ATTENZIONE!** In queste condizioni dunque una volta effettuata
> l'autenticazione l'utente si troverà automaticamente in carrello gli
> stessi articoli presenti nell'ultimo carrello ad esso associato **ma,
> per la sessione in corso, andrà a lavorare sempre e comunque su di una
> copia di quello stesso carrello**
>
> **ATTENZIONE!** l'ultimo carrello associato all'utente è quello
> dell'ultimo browser / dispositivo su cui è stata effettuata
> l'autenticazione
>
> Tale impostazione potrebbe quindi rivelarsi particolarmente utile nel
> momento in cui l'esigenza dovesse essere quella di fare in modo che lo
> stesso utente possa loggarsi e operare contemporaneamente su due
> dispositivi / browser differenti, aprendo di fatto due diverse
> sessioni di lavoro, senza che le modifiche effettuate sul carrello
> della sessione A vengano automaticamente riproposte anche sul carrello
> della sessione B.
>
> Di contro il fatto di lavorare contemporaneamente su due dispositivi /
> browser differenti, aprendo contemporaneamente due differenti sessioni
> che andranno a lavorare su due distinte copie dello stesso carrello
> associato all'utente, potrebbe causare dei problemi nel momento in cui
> una delle due sessioni dovesse terminare senza concludere l'ordine.
>
> Per comprendere meglio quello che potrebbe avvenire in queste
> condizioni consideriamo dunque il seguente esempio:
>
> **[ESEMPIO]{.underline}**
>
> Supponiamo che l'utente X effettui una prima autenticazione al sito
> dal browser / dispositivo A e supponiamo anche che l'ultimo carrello
> associato allo stesso utente X (creato durante una precedente sessione
> di lavoro) contenga gli articoli PROD01 e PROD02.
>
> Nelle condizioni considerate Passweb rileverà questo carrello, ne farà
> una copia e lo caricherà sul front end del sito. Di fatto dunque, una
> volta effettuata l'autenticazione l'utente X si troverà
> automaticamente caricati nel suo carrello i due prodotti PROD01 e
> PROD02.
>
> Supponiamo ora che lo stesso utente effettui una seconda
> autenticazione al sito dal browser / dispositivo B senza aver
> effettuato nessuna variazione al carrello attualmente presente sul
> browser / dispositivo A
>
> Anche in questo caso Passweb rileverà l'ultimo carrello associato
> all'utente, carrello questo che conterrà ancora i due prodotti PROD01
> e PROD02, ne farà una copia e lo caricherà sul front end del sito.
>
> In questo modo quindi anche sul carrello del browser / dispositivo B
> l'utente si troverà automaticamente caricati i due prodotti PROD01 e
> PROD02
>
> A questo punto l'utente, operando dal browser / dispositivo A,
> aggiunge in carrello il prodotto PROD03.
>
> **Considerando che i browser / dispositivi A e B lavorano di fatto su
> due copie distinte dello stesso carrello originale il prodotto PROD03
> sarà presente solo ed esclusivamente nel carrello del browser /
> dispositivo A** per cui anche andando ad aggiornare la pagina carrello
> del browser / dispositivo B questo continuerà ad avere solo ed
> esclusivamente i prodotti PROD01 e PROD02. In sostanza dunque fintanto
> che saranno attive contemporaneamente le due sessioni A e B i due
> carrelli non saranno sincronizzati e l'utente potrà portare a termine
> contemporaneamente sui due browser / dispositivi A e B due ordini
> distinti senza che le modifiche effettuate al carrello A si
> ripercuotano sul carrello B e viceversa
>
> Allo stesso modo dunque, nel momento in cui l'utente dovesse andare ad
> aggiungere in carrello dal browser / dispositivo B il prodotto PROD04
> questo sarà presente solo ed esclusivamente nel carrello del browser /
> dispositivo B.
>
> Supponiamo ora che l'utente decida di effettuare il logout dal browser
> / dispositivo A o, analogamente, decida di non operare più su questo
> dispositivo lasciando scadere la sessione in maniera naturale senza
> concludere l'ordine su nessuno dei due browser / dispositivi.
>
> Supponiamo anche che in fase di configurazione del sito si sia deciso
> di impostare il parametro "**Gestione carrello al Logout**"
> sull'opzione "**Annulla**".
>
> Terminata quindi la sessione sul dispositivo / browser A l'ultimo
> carrello associato all'utente X sarà ora quello ancora attivo sul
> dispositivo / browser B che contiene i prodotti PROD01, PROD02 e
> PROD04.
>
> In conseguenza di ciò se l'utente dovesse ora aprire una nuova
> sessione dal dispositivo / browser A, nelle condizioni considerate
> Passweb rileverà l'ultimo carrello associato all'utente caricando ora
> in front end anche sul browser / dispositivo A i prodotti PROD01,
> PROD02 e PROD04. In questo modo dunque il prodotto PROD03
> precedentemente caricato dall'utente sul browser / dispositivo A andrà
> perso e, eventualmente, dovrà essere nuovamente aggiunto in carrello.
>
> Un'altra considerazione di fondamentale importanza da fare è che in un
> sito B2B, in cui entrano in gioco anche gli Agenti, il contenuto degli
> articoli in carrello una volta effettuato il login per un determinato
> utente potrebbe dipendere anche dal fatto che l'ultimo carrello
> associato a quello stesso utente sia stato creato direttamente da lui
> oppure dal suo Agente.
>
> In questo senso dunque occorre sottolineare che, nelle condizioni
> indicate, **verrà comunque considerato l'ultimo carrello associato al
> cliente indipendentemente dal fatto che tale carrello sia stato
> riempito direttamente dal cliente stesso o, per suo conto, da un
> Agente opportunamente abilitato e si andrà sempre e comunque a
> lavorare su di una sua copia (con tutto ciò che ne consegue)**
>
> Ciò significa dunque che nel caso in cui l'Agente X dovesse
> valorizzare un carrello per il Cliente Y, l'applicazione si comporterà
> come di seguito indicato:

- Se ad autenticarsi sul sito è direttamente il Cliente Y, una volta
  effettuato il login, troverà in carrello gli articoli precedentemente
  inseriti dall'Agente X

- Se ad autenticarsi sul sito è l'Agente X per conto del Cliente Y, una
  volta effettuato il login, troverà in carrello gli articoli da lui
  stesso precedentemente inseriti

- Se ad autenticarsi sul sito è l'Agente Z per conto del Cliente Y, una
  volta effettuato il login, anch'esso troverà in carrello gli articoli
  precedentemente inseriti dall'Agente X

> **ATTENZIONE!** Il comportamento sarà del tutto analogo nel momento in
> cui a valorizzare il primo carrello dovesse essere direttamente il
> Cliente Y
>
> Infine, tenendo conto di quanto visto fino a questo momento, è
> abbastanza semplice comprendere che, nel caso in cui su di uno stesso
> cliente possano lavorare due distinti agenti, potrebbero anche
> verificarsi casi in cui inizialmente l'Agente X aggiunga determinati
> articoli senza completare l'ordine; successivamente l'Agente Z
> potrebbe fare delle modifiche a questo carrello, anche in questo caso
> senza completare l'ordine per cui se, dopo l'intervento dell'Agente Z,
> l'Agente X dovesse effettuare nuovamente l'autenticazione per conto
> dello stesso cliente si troverà in carrello non gli articoli da lui
> inizialmente inseriti ma bensì quelli inseriti dall'Agente Z.
>
> Ovviamente anche nel caso degli Agenti, lavorando per lo stesso
> cliente su due sessioni contemporanee, potrebbero verificarsi
> situazioni analoghe a quelle evidenziate nell'esempio precedente.
>
> In definitiva dunque, nel momento in cui si dovesse decidere di
> adottare questa impostazione, occorrerà poi prestare particolare
> attenzione al fatto di non mantenere aperte contemporaneamente, per lo
> stesso utente, due diverse sessioni con articoli diversi in carrello.
> In questo caso infatti, come visto, quando una delle due sessione
> scadrà gli articoli presenti in carrello per quella sessione
> potrebbero anche andare persi.

- **RILEVA CARRELLO UTENTE/AGENTE -- GESTIONE SEPARATA (ECOMMERCE
  MEXAL)**

> Selezionando questa opzione (disponibile solo per siti Ecommerce
> collegati a Mexal) si avrà, sostanzialmente, lo stesso comportamento
> descritto per l'opzione precedente (Rileva Carrello Utente -- Gestione
> Separata).
>
> Anche in questo caso dunque nel momento in cui un utente dovesse
> effettuare l'autenticazione al sito **senza aver aggiunto ( durante la
> stessa sessione) nessun articolo in carrello** verrà effettuata una
> ricerca per rilevare l'ultimo carrello eventualmente associato a
> quello stesso utente e, nel caso in cui tale ricerca dovesse dare
> esito positivo Passweb **effettuerà una copia** del carrello rilevato
> caricandola poi sul front end del sito, con tutto ciò che ne consegue.
>
> Quello che cambia, invece, impostando il parametro "Gestione Carrello
> al Login" sull'opzione "Rileva Carrello Utente / Agente -- Gestione
> Separata", è il comportamento dell'applicativo in relazione al fatto
> che l'ultimo carrello associato ad un determinato cliente sia stato
> creato dal cliente stesso o da uno degli Agenti abilitati a gestirlo.
>
> In particolare dunque, in queste condizioni, nel caso in cui l'ultimo
> carrello associato, ad esempio, al Cliente Y dovesse essere stato
> creato direttamente da lui allora:

- Se ad autenticarsi sul sito è lo stesso Cliente Y, una volta
  effettuato il login, troverà in carrello gli articoli da lui stesso
  inseriti

- Se ad autenticarsi sul sito è l'Agente X o l'Agente Z per conto del
  Cliente Y, una volta effettuato il login, troverà il carrello vuoto

> Nel caso in cui, invece, l'ultimo carrello associato al Cliente Y
> dovesse essere stato creato per suo conto dall'Agente X allora:

- Se ad autenticarsi sul sito è direttamente il Cliente Y, una volta
  effettuato il login, troverà il carrello vuoto

- Se ad autenticarsi sul sito è l'Agente Z per conto del Cliente Y, una
  volta effettuato il login, troverà il carrello vuoto

- Se ad autenticarsi sul sito è l'Agente X per conto del Cliente Y, una
  volta effettuato il login, troverà in carrello gli articoli da lui
  stesso inseriti

<!-- -->

- **RILEVA CARRELLO UTENTE -- GESTIONE UNIFICATA**

> Selezionando questa opzione, nel momento in cui un utente dovesse
> effettuare l'autenticazione al sito **senza aver aggiunto ( durante la
> stessa sessione) nessun articolo in carrello** verrà effettuata una
> ricerca per rilevare l'ultimo carrello eventualmente associato a
> quello stesso utente.
>
> Nel momento in cui tale ricerca dovesse dare esito positivo, Passweb
> caricherà sul front end del sito direttamente quello stesso carrello
> **senza effettuarne una copia**
>
> **ATTENZIONE!** In queste condizioni dunque una volta effettuata
> l'autenticazione l'utente andrà a lavorare direttamente sull'ultimo
> carrello ad esso associato (e non su di una sua copia)
>
> In considerazione di ciò, un' altra cosa fondamentale da tenere in
> considerazione è che **nel momento in cui si dovesse decidere di
> attivare la "Gestione Unificata" eventuali mail di recupero dei
> carrelli abbandonati (contenenti link per il recupero di un
> determinato carrello) non avrebbero molto senso.** Con la gestione
> unificata infatti l'ultimo carrello abbandonato da un determinato
> utente diventerà automaticamente il carrello attivo nel momento in cui
> l'utente stesso dovesse effettuare nuovamente l'accesso al sito.
>
> In queste condizioni dunque eventuali mail contenenti link di recupero
> di vecchi carrelli abbandonati porteranno l'utente sempre e comunque
> al carrello attivo in quel preciso momento, carrello questo che
> potrebbe anche contenere articoli diversi da quelli presenti nel
> momento in cui il vecchio carrello abbandonato era stato generato.
>
> In definitiva dunque l'impostazione per la "Gestione Unificata" del
> carrello potrebbe rivelarsi particolarmente utile nel momento in cui
> l'esigenza dovesse essere quella di fare in modo che passando da un
> dispositivo / browser ad un altro l'utente si ritrovi in carrello
> sempre e comunque gli stessi articoli, indipendentemente dal fatto che
> questi siano stati aggiunti da un dispositivo / browser A piuttosto
> che da un dispositivo / browser B
>
> Di contro il fatto di lavorare sempre e comunque sullo stesso carrello
> anche operando, in maniera contemporanea, da due dispositivi / browser
> differenti, potrebbe causare dei problemi di sovrascrittura dei dati
> che, in una gestione non standard, potrebbero anche portare l'utente a
> concludere un ordine con articoli indesiderati.
>
> Per comprendere meglio quello che potrebbe avvenire in queste
> condizioni consideriamo anche questa volta un semplice esempio:
>
> **[ESEMPIO]{.underline}**
>
> Supponiamo che l'utente X effettui una prima autenticazione al sito
> dal browser / dispositivo A e supponiamo anche che l'ultimo carrello
> associato allo stesso utente X (creato durante una precedente sessione
> di lavoro) contenga gli articoli PROD01 e PROD02.
>
> Nelle condizioni considerate Passweb rileverà questo carrello e lo
> caricherà direttamente sul front end del sito.
>
> Di fatto dunque, una volta effettuata l'autenticazione l'utente X
> andrà a lavorare direttamente sul suo ultimo carrello in cui si
> ritroverà automaticamente i prodotti PROD01 e PROD02.
>
> Supponiamo ora che l'utente X aggiunga in carrello il prodotto PROD03
> e che poco dopo, senza effettuare il logout e senza concludere la
> sessione sul dispositivo / browser A, decida di effettuare una seconda
> autenticazione al sito dal browser / dispositivo B
>
> Anche in questo caso Passweb rileverà l'ultimo carrello associato
> all'utente, carrello questo che era stato modificato poco fa dal
> browser / dispositivo A con l'aggiunta dell'articolo PROD03, e lo
> caricherà direttamente sul front end del sito.
>
> In questo modo quindi anche sul carrello del browser / dispositivo B
> l'utente si troverà automaticamente i prodotti PROD01, PROD02 e PROD03
>
> **Ora considerando che i browser / dispositivi A e B lavorano di fatto
> sullo stesso carrello, eventuali modifiche ad esso apportate sul
> browser / dispositivo A verranno riportate anche sul carrello del
> browser / dispositivo B e viceversa**.
>
> Il fatto però è che per visualizzare su di uno dei due browser /
> dispositivi eventuali modifiche apportate al carrello dall'altro
> browser / dispositivo sarà necessario, ovviamente, aggiornare la
> pagina oppure effettuare prima il logout (avendo il parametro
> "**Gestione carrello al Logout**" impostato sull'opzione
> "**Annulla**") e successivamente un nuovo login e se questo non
> dovesse avvenire, continuando a lavorare sullo stesso carrello
> contemporaneamente da due dispositivi / browser diversi ci potrebbe
> anche essere una sovrascrittura di dati indesiderata.
>
> Per cercare di capire come questo possa avvenire, supponiamo che
> l'utente vada ad aggiungere in carrello dal browser / dispositivo B
> l'articolo PROD04 e che decida anche di eliminare l'articolo PROD03
> senza comunque concludere l'ordine.
>
> Supponiamo poi che lo stesso utente decida di concludere l'ordine dal
> browser / dispositivo A senza prima aggiornare la pagina carrello e
> senza di fatto visualizzare le modifiche ad esso apportate dal browser
> / dispositivo B.
>
> In queste condizioni dunque sul browser / dispositivo A, in carrello,
> verranno ancora visualizzati i prodotti PROD01, PROD02 e PROD03.
> Passando però al checkout verranno recepite le modifiche apportate al
> carrello dal browser / dispositivo B e quindi si procederà a
> concludere l'ordine con i prodotti PROD01, PROD02 e PROD04 che, di
> fatto, non erano quelli precedentemente visualizzati alla pagina
> Carrello.
>
> Ora è chiaro che nel momento in cui l'utente dovesse utilizzare le
> proprie credenziali in maniera esclusiva sarebbe consapevole, prima di
> concludere l'ordine sul browser / dispositivo A di aver apportato
> delle modifiche al carrello dal browser / dispositivo B e quindi del
> fatto che passando dal carrello al checkout i prodotti effettivamente
> in ordine potrebbero anche cambiare.
>
> Al contrario, in un processo non standard in cui due persone diverse
> dovessero utilizzare le credenziali di uno stesso utente per
> effettuare contemporaneamente due ordini su due dispositivi / browser
> diversi, uno dei due potrebbe anche non accorgersi del fatto che
> passando dal carrello al checkout sia cambiato qualcosa in termini di
> articoli o quantità in ordine e potrebbe quindi portare a termine il
> checkout con un insieme di prodotti che non sono esattamente quelli
> che intendeva acquistare.
>
> Infine, per quel che riguarda il comportamento dell'applicativo in un
> sito B2B nel momento in cui dovessero entrare in gioco anche gli
> Agenti, è bene sottolineare che, nelle condizioni in esame, **si andrà
> a lavorare sempre e comunque in maniera diretta sull'ultimo carrello
> associato al cliente per cui viene fatta l'autenticazione** (e non su
> di una sua copia) **e questo indipendentemente dal fatto che tale
> carrello sia stato creato, in precedenza, dal cliente stesso o, per
> suo consto, da un Agente opportunamente abilitato**
>
> Ciò significa dunque che nel caso in cui l'Agente X dovesse
> valorizzare un carrello per il Cliente Y, l'applicazione si comporterà
> come di seguito indicato:

- Se ad autenticarsi sul sito è direttamente il Cliente Y, una volta
  effettuato il login, troverà in carrello gli articoli precedentemente
  inseriti dall'Agente X

- Se ad autenticarsi sul sito è l'Agente X per conto del Cliente Y, una
  volta effettuato il login, troverà in carrello gli articoli da lui
  stesso precedentemente inseriti

- Se ad autenticarsi sul sito è l'Agente Z per conto del Cliente Y, una
  volta effettuato il login, anch'esso troverà in carrello gli articoli
  precedentemente inseriti dall'Agente X

> **ATTENZIONE!** Il comportamento sarà del tutto analogo nel momento in
> cui a valorizzare il primo carrello dovesse essere direttamente il
> Cliente Y
>
> Ovviamente, tenendo conto del fatto che, nelle condizioni indicate, si
> andrà a lavorare direttamente sull'ultimo carrello del cliente, nel
> caso in cui su quello stesso cliente possano lavorare due diversi
> agenti, sarebbe estremamente alto il rischio che questi finiscano col
> "pestarsi i piedi" effettuando ciascuno delle modifiche sullo stesso
> carrello che potrebbero essere corrette per lui ma non per l'altro
> Agente
>
> **In definitiva dunque, nel momento in cui si dovesse decidere di
> adottare questa impostazione, trovandosi comunque nelle condizioni in
> cui più persone diverse possono lavorare contemporaneamente sulla
> stessa utenza, occorrerà anche tenere sempre bene presente che il
> rischio di vedersi sovrascritte le modifiche apportate ad un
> determinato carrello potrebbe essere molto elevato.**

- **RILEVA CARRELLO UTENTE/AGENTE -- GESTIONE UNIFICATA (ECOMMERCE
  MEXAL)**

> Selezionando questa opzione (disponibile solo per siti Ecommerce
> collegati a Mexal) si avrà, sostanzialmente, lo stesso comportamento
> descritto per l'opzione precedente (Rileva Carrello Utente / Agente --
> Gestione Unificata).
>
> Anche in questo caso dunque nel momento in cui un utente dovesse
> effettuare l'autenticazione al sito **senza aver aggiunto ( durante la
> stessa sessione) nessun articolo in carrello** verrà effettuata una
> ricerca per rilevare l'ultimo carrello eventualmente associato a
> quello stesso utente e, nel caso in cui tale ricerca dovesse dare
> esito positivo Passweb caricherà sul front end del sito direttamente
> quello stesso carrello **senza effettuarne una copia**, con tutto ciò
> che ne consegue.
>
> **ATTENZIONE!** Anche in questo caso l'attivazione di eventuali mail
> di recupero dei carrelli abbandonati non avrebbero molto senso.
>
> Quello che cambia impostando il parametro "Gestione Carrello al Login"
> sull'opzione "Rileva Carrello Utente / Agente -- Gestione Unificata",
> è il comportamento dell'applicativo in relazione al fatto che l'ultimo
> carrello associato ad un determinato cliente sia stato creato dal
> cliente stesso o da uno degli Agenti abilitati a gestirlo.
>
> In particolare dunque, in queste condizioni, nel caso in cui l'ultimo
> carrello associato, ad esempio, al Cliente Y dovesse essere stato
> creato direttamente da lui allora:

- Se ad autenticarsi sul sito è lo stesso Cliente Y, una volta
  effettuato il login, troverà in carrello gli articoli da lui stesso
  inseriti

- Se ad autenticarsi sul sito dovesse essere invece l'Agente X o
  l'Agente Z per conto del Cliente Y, una volta effettuato il login,
  troverà il carrello vuoto

> Nel caso in cui, invece, l'ultimo carrello associato al Cliente Y
> dovesse essere stato creato per suo conto dall'Agente X allora:

- Se ad autenticarsi sul sito è direttamente il Cliente Y, una volta
  effettuato il login, troverà il carrello vuoto

- Se ad autenticarsi sul sito è l'Agente Z per conto del Cliente Y, una
  volta effettuato il login, troverà il carrello vuoto

- Se ad autenticarsi sul sito è l'Agente X per conto del Cliente Y, una
  volta effettuato il login, troverà in carrello gli articoli da lui
  stesso inseriti

> In sostanza dunque, nelle condizioni indicate, si andrà sempre e
> comunque a lavorare direttamente sull'ultimo carrello associato ad un
> determinato utente ma quale sia quest'ultimo carrello dipenderà anche
> da chi lo ha effettivamente creato.

**ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
effettuare dei test per verificare il comportamento dell'applicativo
nelle diverse configurazioni del parametro "Gestione Carrello al Login"
è sempre bene, una volta variate queste impostazioni, eliminare i cookie
dei browser / dispositivi su cui vengono effettuati i test

In ogni caso i cookie che possono influenzare il comportamento del
carrello, in relazione al parametro in oggetto, sono sempre cookie di
sessione per cui, una volta scaduta la sessione in essere l'applicativo
recepirà correttamente le nuove impostazioni del parametro "Gestione
Carrello al Login"

**ATTENZIONE! le impostazioni settate per il parametro "Gestione
Carrello al login" valgono non solo per il carrello ma anche per la
Wishlist corrente e per il Comparatore**

**Gestione Carrello al Logout:** consente di definire come dovrà essere
gestito, al logout, il carrello utente

E' possibile selezionare uno dei seguenti valori:

- **MANTIENI**

> Selezionando questa opzione (che è anche l'impostazione di default)
> effettuando il logout dal sito verranno mantenuti in carrello gli
> stessi articoli presenti prima del logout (il tutto ovviamente sempre
> nell'ambito della stessa sessione di lavoro e all'interno dello stesso
> browser)
>
> **ATTENZIONE!** In queste condizioni se, dopo aver effettuato il
> logout, si dovesse effettuare (utilizzando ovviamente sempre lo stesso
> browser) il login per un altro cliente questo si ritroverà in carrello
> esattamente gli stessi articoli presenti prima di aver effettuato il
> logout per il cliente precedente.

- **ANNULLA**

> Selezionando questa opzione effettuando il logout dal sito verranno
> automaticamente eliminati dal carrello tutti gli articoli in esso
> presenti prima del logout.
>
> In queste condizioni dunque nel caso in cui, dopo il logout, venisse
> effettuato il login con un altro utente, utilizzando ovviamente sempre
> lo stesso browser e senza inserire altri articoli prima del login, il
> carrello che verrà caricato dipenderà dalle impostazione settate per
> il precedente parametro "Gestione Carrello al Login"

**ATTENZIONE!** In ogni caso se l'esigenza dovesse essere quella di
salvare una determinata lista di articoli per un dato utente, anziché
lasciarli in carrello si consiglia sempre di salvarli all'interno di
un'apposita Wishlist

**Messaggio Carrello al Logout**: consente di attivare la
visualizzazione, sul front end del sito, di un apposito messaggio nel
momento in cui l'utente dovesse tentare di effettuare il logout **avendo
ancora articoli in carrello**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_logout_carrello.bmp](./assets/media/image10.png)

Il messaggio in esame potrà essere personalizzato alla pagina "**Testi
Messaggi Sito**" del Wizard agendo in corrispondenza dell'elemento
"**Richiesta Conferma Logout**" presente tra i "**Testi Generici**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_conferma_logout.bmp](./assets/media/image11.png)

e, nello specifico, verrà visualizzato nel momento in cui, pur avendo
ancora articoli in carrello l'utente dovesse:

- tentare di effettuare il logout sul front end del sito utilizzando
  l'apposito pulsante presente all'interno del componente "Barra Utente"

- tentare di effettuare il logout dall'Area Riservata

- cliccare, sempre in Area Riservata, sul pulsante "Nuovo Ordine
  Cliente" effettuando, di fatto, il logout per l'utente precedentemente
  impersonificato

Va da sé, ovviamente, che il logout verrà poi effettuato solo nel caso
in cui l'utente dovesse effettivamente confermare l'operazione.

**Gestione articoli in carrello / wishlist:** consente di impostare la
specifica modalità di inserimento articoli in carrello / wishlist.

E' possibile selezionare uno dei seguenti valori:

- **Modifica riga articolo:** nel caso in cui l'articolo aggiunto sia
  già presente in carrello, verrà modificata la quantità della relativa
  riga articolo

- **Nuova riga articolo:** verrà sempre creata una nuova riga articolo,
  anche nel caso in cui l'articolo aggiunto fosse già presente in
  Carrello.

- **Modifica riga articolo se Cliente, nuova riga articolo se Agente
  (solo Ecommerce Mexal):** nel caso in cui ad effettuare l'ordine sia
  un Cliente e l'articolo inserito fosse già presente in Carrello, verrà
  modificata la quantità della relativa riga articolo. Nel caso in cui
  ad effettuare l'ordine dovesse invece essere un Agente verrà sempre
  creata una nuova riga articolo anche nel caso in cui l'articolo
  aggiunto fosse già presente in Carrello.

- **Nuova riga articolo se Cliente, modifica riga articolo se Agente
  (solo Ecommerce Mexal):** nel caso in cui ad effettuare l'ordine sia
  un Cliente verrà sempre creata una nuova riga articolo anche nel caso
  in cui l'articolo aggiunto fosse già presente in Carrello. Nel caso in
  cui ad effettuare l'ordine dovesse invece essere un Agente e
  l'articolo inserito fosse già presente in Carrello, verrà modificata
  la quantità della relativa riga articolo.

**ATTENZIONE!** Le impostazioni settate per il parametro in oggetto
possono influire anche sui contenuti (quantità e subtotale) di eventuali
pop up di aggiunta in carrello / wishlist.

In particolare nel caso di creazione di una nuova riga quantità e
subtotale presenti nel pop up di aggiunta in carrello / wishlist saranno
sempre riferite alla quantità del prodotto che è stato effettivamente
aggiunto indipendentemente dal fatto che in carrello siano già presenti
o meno altre righe dello stesso prodotto

Nel caso invece di modifica della riga prodotto già presente in
carrello, quantità e subtotale presenti nel pop up di aggiunta faranno
sempre riferimento alle condizioni di questa stessa riga.

Per maggiori informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Componenti Ecommerce -- Componenti interni ai
componenti ecommerce -- Aggiunta al carrello*" di questo manuale

**ATTENZIONE! Per ordini originati a partire da Liste Regalo
indipendentemente da quanto impostato per il parametro in oggetto verrà
sempre modificata la quantità dell'eventuale riga articolo già presente
in carrello**

Per maggiori informazioni relativamente alla gestione delle Liste Regalo
si veda anche la corrispondente sezione di questo manuale "*Varianti
Sito Responsive -- Lista Componenti Ecommerce -- Componente Lista
Regalo*"

**Gestione articoli Box**: consente di impostare la modalità di gestione
degli articoli Campionario in relazione ad eventuali Filtri Articolo
impostati in fase di configurazione di:

- Promozioni

- Buoni Sconto

- Gift Card

- Raccolta Punti

- Regole di Raccolta Punti (Assegna X Punti per ogni Y del totale merce)

- Pagamenti

- Metodi di Trasporto

- Costi di Spese Accessorie

E' possibile selezionare una delle seguenti opzioni:

- **Considera il Box -- opzione di default**: in queste condizioni la
  validazione del filtro verrà fatta prendendo in considerazione
  unicamente l'articolo Campionario, indipendentemente dai suoi
  componenti, che non verranno quindi considerati in alcun modo

- **Considera i componenti del Box:** in queste condizioni la
  validazione del filtro verrà fatta prendendo in considerazione i
  singoli componenti del Campionario ma non l'articolo Campionario in
  sé, articoli questo che potrebbe quindi anche non soddisfare il filtro
  impostato senza che questo pregiudichi in qualche modo l'applicazione
  della Promozione, del Buono Sconto, del Pagamento ....

**Relativamente alle Promozioni e/o ai Buoni Sconto, l'impostazione di
questo parametro potrà impattare, ovviamente, non solo sulle loro
condizioni di applicabilità, ma anche su come verrà poi effettivamente
applicata la Promozione o il Buono Sconto in esame.**

Supponendo di avere a che fare, ad esempio, con una Promozione del tipo
"Sconto ogni X articoli in Carrello", se il parametro in esame dovesse
essere impostato sull'opzione "Considera il Box", nel valutare
l'articolo X verrà considerato solo ed esclusivamente l'articolo
Campionario (i singoli componenti non verranno considerati in alcun
modo)

Nel momento in cui per il parametro in esame dovesse invece essere stata
impostata l'opzione "Considera i componenti del Box", nel valutare
l'articolo X in carrello verranno considerati singolarmente tutti i
componenti del Campionario (in questo caso non verrà invece considerata
in alcun modo la riga del carrello relativa all'articolo Campionario in
sé).

Per maggiori informazioni in merito si rimanda a quanto indicato
all'interno di questo manuale in relazione alla singola Promozione /
Buono Sconto.

**ATTENZIONE!** Il parametro "**Gestione Articoli Box**" non ha alcun
effetto sulle promozioni Ho.Re.Ca. (definite direttamente all'interno
del gestionale)

**Le promozioni definite all'interno di gestionali Ho.Re.Ca. infatti,
non considerano mai gli articoli presenti all'interno del Composto ma
sono tarate sempre e soltanto sul Composto stesso**

