# WISHLIST PERSONALI



Come evidenziato nei precedenti capitoli di questo manuale, il
componente Wishlist Custom si comporterà in maniera diversa a seconda
del fatto che l'utente abbia o meno effettuato l'autenticazione al sito
e, soprattutto, a seconda del fatto che sia stato configurato per
consentire all'utente stesso di creare unicamente delle Wishlist
Personali oppure anche delle vere e proprie Liste Regalo

Nello specifico, **se l'esigenza dovesse essere quella di far creare e
gestire all'utente unicamente delle** **Wishlist Personali**, dove per
Wishlist Personali si intende, come precedentemente evidenziato, delle
liste di articoli gestibili unicamente dallo stesso utente che le ha
create e salvate, sarà allora necessario assicurarsi di **NON**
selezionare, in fase di configurazione del componente stesso, il
parametro "**Gestione Liste Regalo**"

![](./assets/media/image195.png)

In queste condizioni:

- **Nel caso in cui non sia stata ancora effettuata l'autenticazione al
  sito**, l'utente avrà unicamente la possibilità di inserire articoli
  nella Wishlist corrente senza poter comunque effettuare nessun tipo di
  salvataggio relativamente a questa particolare lista di articoli

> All'interno del componente verrà quindi visualizzata solo ed
> esclusivamente la "Wishlist Corrente", ossia la lista di articoli
> inseriti dall'utente durante la specifica sessione di navigazione, con
> la possibilità di inserire uno o tutti gli articoli presenti in lista
> all'interno del carrello.

![](./assets/media/image196.png)

- **Nel caso in cui l'utente abbia già effettuato l'autenticazione al
  sito,** oltre a poter inserire articoli nella Wishlist corrente, avrà
  anche, da una parte la possibilità di salvare tale lista assegnandole
  uno specifico nome, e dall'altra parte, la possibilità di richiamare e
  visualizzare eventuali Wishlist salvate in momento precedente.

In quest'ultimo caso (autenticazione effettuata) all'interno del
componente saranno presenti due distinti elementi, la Wishlist Corrente
e l'elenco di tutte le Wishlist precedentemente salvate:

**[WISHLIST CORRENTE]{.underline}**

E la stessa Wishlist visualizzata anche nel caso in cui non fosse stata
effettuata l'autenticazione al sito

![](./assets/media/image197.png)

Come per il Componente Carrello, anche in questo caso la lista degli
articoli presenti nella Wishlist è strutturata all'interno di una
griglia perfettamente responsiva le cui colonne possono essere definite
direttamente all'interno della sezione "**Gestione Contenuti**" presente
nella maschera di gestione e configurazione del componente stesso.

Inoltre, come sempre, il comportamento responsivo della griglia è tale
per cui indipendentemente dalla larghezza impostata per ogni singola
colonna, in corrispondenza di risoluzioni inferiori ai 992 px la griglia
stessa si linearizzerà disponendo le varie colonne una sotto l'altra.

A differenza di ciò che avveniva nel caso in cui l'utente non avesse
ancora effettuato l'autenticazione, in queste condizioni al di sotto
della Wishlist corrente comparirà anche, come evidenziato in figura, un
piccolo form costituito da un unico campo di input (che l'utente potrà
utilizzare per assegnare un nome alla Wishlist in esame) e da un
apposito pulsante di salvataggio.

Alla pressione del pulsante "**Salva**" la Wishlist Corrente verrà
salvata con lo specifico nome indicato all'interno del corrispondente
campo di input, inserita nell'elenco delle Wishlist Salvate e, infine,
svuotata.

**ATTENZIONE! Gli articoli presenti nella Wishlist Corrente, potranno
variare a seconda del fatto che l'utente abbia già inserito degli
articoli in Wishlist durante la stessa sessione di navigazione e/o a
seconda del fatto di aver effettuato l'autenticazione al sito.**

I pulsanti "**Aggiungi in Carrello**" e "**Rimuovi**", presenti in
corrispondenza di ogni singolo articolo in Wishlist consentono
rispettivamente di:

![](./assets/media/image198.png)

- **Aggiungi in Carrello:** consente di inserire in Carrello la
  corrispondente riga articolo.

> **ATTENZIONE!** Non è possibile aggiungere in Carrello articoli per i
> quali è stata abilitata la funzionalità di "Prezzo a Richiesta"

- **Rimuovi:** consente di eliminare la corrispondente riga dalla
  Wishlist corrente.

Per quel che riguarda invece i pulsanti presenti nella parte bassa della
Wishlist Corrente, e relativi quindi all'intera lista articoli, questi
consentiranno rispettivamente di:

- **Aggiungi tutto al Carrello:** consente di aggiungere in carrello
  tutti gli articoli presenti nella Wishlist corrente, ad eccezione di
  quelli per i quali è stata attivata la funzionalità di "Prezzo a
  Richiesta".

> Nello specifico poi, cliccando su questo pulsante verranno proposte
> all'utente due diverse possibili opzioni di scelta:

![](./assets/media/image199.png)

- **Rimuovi gli articoli dalla wishlist:** selezionando questa opzione
  tutti gli articoli presenti nella Wishlist attualmente visualizzata
  verranno aggiunti in carrello e, contestualmente, verranno anche
  rimossi dalla Wishlist stessa.

> **ATTENZIONE! nelle condizioni indicate la Wishlist verrà svuotata ma
> NON eliminata.** In conseguenza di ciò volendo, sarà comunque
> possibile aggiungere in un secondo momento nuovi articoli a questa
> stessa Wishlist
>
> Nel momento in cui l'esigenza dovesse essere non solo quella di
> svuotare automaticamente la Wishlist dopo aver aggiunto tutti gli
> articoli in carrello, ma anche quella di eliminarla in maniera
> definitiva, sarà necessario agire manualmente cliccando sul
> corrispondente pulsante di "Rimozione Wishlist"

- **Mantieni gli articoli nella wishlist**: selezionando questa opzione
  tutti gli articoli presenti nella Wishlist attualmente visualizzata
  verranno aggiunti in carrello senza però essere eliminati dalla
  Wishlist stessa

<!-- -->

- **Aggiorna Wishlist:** visibile solo nel caso in cui il parametro
  "**Aggiornamento Dati Articoli**", presente nella maschera di
  configurazione del componente, sia stato impostato sul valore
  "**Intera Wishlist**".

> Consente di aggiornare la Wishlist Corrente salvando eventuali
> modifiche apportate alle quantità degli articoli presenti in elenco.
> In relazione a tali quantità, modificabili direttamente da questo
> stesso componente, va poi sottolineato che, come già avviene per il
> carrello, anche in questo caso **è possibile inserire quantità intere
> o decimali** in perfetto accordo con le relative impostazioni del
> gestionale.
>
> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> in Mexal o su uno dei gestionali Ho.Re.Ca. i decimali sulle quantità
> dei singoli articoli si rimanda allo specifico manuale.

- **Svuota Wishlist:** consente all'utente di svuotare la Wishlist
  attualmente visualizzata eliminando in un colpo solo tutti gli
  articoli presenti al suo interno.

> **ATTENZIONE!** Anche in questo caso la Wishlist verrà svuotata ma NON
> eliminata

**[ELENCO DI TUTTE LE WISHLIST SALVATE]{.underline}**

E' un elenco di tutte le Wishlist salvate, in momenti precedenti, dall'
utente attualmente loggato

![](./assets/media/image200.png)

Nelle condizioni in esame (Wishlist Personali), per ciascuna lista
presente in elenco verranno visualizzati due pulsanti "**Rimuovi**" e
"**Visualizza**" attraverso cui poter rispettivamente:

- **Rimuovi:** consente all'utente di eliminare dall'elenco la
  corrispondente Lista dei Desideri.

- **Visualizza:** consente all'utente di visualizzare il dettaglio della
  corrispondente Lista dei Desideri, sostituendolo a quello della
  Wishlist Corrente.

![](./assets/media/image201.png)

> Nell'intestazione di questa lista verrà inoltre visualizzato:

- il nome assegnato alla lista stessa e la sua data di creazione

- un pulsante "**Torna alla Wishlist corrente"** che l'utente potrà
  utilizzare per tornare a visualizzare all'interno del componente il
  dettaglio della Wishlist Corrente

- un pulsante di "**Stampa**" per consentire al creatore della lista di
  effettuare una stampa della Wishlist in questione

> **ATTENZIONE!** Il pulsante di Stampa verrà visualizzato solo nel
> momento in cui sia stato correttamente definito il relativo Template
> (per maggiori informazioni in merito si veda anche quanto indicato
> all'interno della sezione "*Utenti -- Wishlist -- Tipologia*" di
> questo manuale)

**ATTENZIONE! in fase di visualizzazione del dettaglio di una Wishlist i
vari articoli verranno filtrati in base alla proprietà di pubblicazione
e ad eventuali filtri articolo associati al cliente in questione.**

Questo perché dal momento in cui la Wishlist è stata creata al momento
in cui viene visualizzato il suo dettaglio, potrebbero essere cambiate
alcune condizioni e quindi alcuni dei suoi articoli potrebbero, ad
esempio, non essere più gestiti all'interno del sito oppure potrebbero
non essere più acquistabili dallo specifico cliente sulla base di nuovi
filtri articolo a lui stesso associati.

