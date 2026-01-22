# WISHLIST PER LISTE REGALO



Nel caso in cui **l'esigenza dovesse essere quella di far creare e
gestire ad un utente autenticato oltre a Wishlist Personali anche delle
vere e proprie Liste Regalo** sarà allora necessario assicurarsi di
**aver selezionato**, in fase di configurazione del componente stesso,
il parametro "**Gestione Liste Regalo**"

![](./assets/media/image202.png)

**ATTENZIONE!** Per Lista Regalo si intende essenzialmente una
particolare lista di articoli, selezionati da un determinato utente (il
creatore della lista), e che altri utenti opportunamente abilitati (con
i quali è stata cioè condivisa la lista stessa) potranno acquistare,
fino ad esaurimento della lista stessa, accedendo all'apposita sezione
del sito.

In queste condizioni:

- **Nel caso in cui non sia stata ancora effettuata l'autenticazione al
  sito**, come già avveniva per le Wishlist Personali, l'utente avrà
  unicamente la possibilità di inserire articoli nella Wishlist corrente
  senza poter comunque effettuare nessun tipo di salvataggio
  relativamente a questa particolare lista di articoli ne a livello di
  "Wishlist Personale" ne tanto meno a livello di "Lista Regalo"

- **Nel caso in cui sia già stata effettuata l'autenticazione al sito,**
  oltre a poter inserire articoli nella Wishlist Corrente, l'utente avrà
  la possibilità di salvare la lista in esame selezionando anche la
  tipologia che dovrà assumere tale lista potendo quindi decidere se
  creare una Wishlist Personale oppure una Lista Regalo. Come nel caso
  precedente, inoltre, l'utente avrà sempre la possibilità di richiamare
  e visualizzare eventuali Wishlist Personale e/o Liste Regalo salvate
  in momento precedente.

In quest'ultimo caso (autenticazione effettuata) all'interno del
componente saranno presenti due distinti elementi, la **Wishlist
Corrente** e **l'elenco di tutte le Wishlist / Liste Regalo
precedentemente salvate**:

**[WISHLIST CORRENTE]{.underline}**

E' la stessa visualizzata anche nel caso in cui non fosse stata
effettuata l'autenticazione al sito

![](./assets/media/image203.png)

Anche in questo caso la lista degli articoli presenti nella Wishlist è
strutturata all'interno di una griglia perfettamente responsiva le cui
colonne possono essere definite direttamente all'interno della sezione
"**Gestione Contenuti**" presente nella maschera di gestione e
configurazione del componente stesso.

Inoltre, come sempre, il comportamento responsivo della griglia è tale
per cui indipendentemente dalla larghezza impostata per ogni singola
colonna, in corrispondenza di risoluzioni inferiori ai 992 px la griglia
stessa si linearizzerà disponendo le varie colonne una sotto l'altra.

A differenza di ciò che avveniva nel caso in cui l'utente non avesse
ancora effettuato l'autenticazione, in queste condizioni al di sotto
della Wishlist corrente comparirà anche, come evidenziato in figura, un
form costituito, inizialmente dai campi Nome e Tipologia mediante i
quali poter indicare rispettivamente:

**Nome**: consente di assegnare un nome alla lista di articoli che si
intende salvare

**Tipologia**: consente di definire la tipologia da assegnare alla lista
di articoli che si intende salvare. E' possibile selezionare uno dei
seguenti valor:

- **Personale:** selezionando questa opzione al salvataggio verrà creata
  una Wishlist Personale. Per maggiori informazioni in merito a questa
  specifica tipologia di Wishlist si veda il precedente capitolo di
  questo manuale

- **Lista Regalo:** selezionando questa opzione al salvataggio verrà
  creata una vera e propria Lista Regalo. In queste condizioni sarà
  inoltre necessario definire un valore per i seguenti campi:

![](./assets/media/image204.png)

- **Titolo Evento:** consente di assegnare un titolo all'evento in
  relazione al quale verrà poi creata la Lista Regalo

- **Organizzatore Evento:** consente di indicare l'organizzatore
  dell'evento in relazione al quale verrà poi creata la Lista Regalo

- **Luogo Evento:** consente di indicare il luogo dell'evento in
  relazione al quale verrà poi creata la Lista Regalo

- **Descrizione Evento:** consente di assegnare descrizione all'evento
  in relazione al quale verrà poi creata la Lista Regalo

- **Data Evento (obbligatorio):** consente di indicare la data
  dell'evento in relazione al quale verrà poi creata la Lista Regalo

- **Immagine Evento:** consente di assegnare un'immagine all'evento in
  relazione al quale verrà poi creata la Lista Regalo

- **Indirizzo di spedizione (obbligatorio se presente all'interno del
  form):** consente di impostare l'indirizzo di spedizione cui dovranno
  essere inviati gli articoli acquistati mediante la Lista Regalo in
  oggetto.

> E' possibile selezionare uno qualsiasi degli indirizzi di spedizione
> gestiti per l'utente in esame. Nel caso in cui l'indirizzo selezionato
> non dovesse essere disponibile tra quelli presenti in elenco sarà
> necessario, per prima cosa aggiungerlo al proprio profilo.
>
> **ATTENZIONE!** Il campo "**Indirizzo di spedizione**" verrà
> visualizzato solo ed esclusivamente nel caso in cui in fase di
> configurazione della Tipologia di Wishlist sia stato selezionato il
> flag **"Indirizzo Spedizione"**

![](./assets/media/image205.png)

> Per maggiori informazioni in merito si veda anche la sezione "*Utenti
> -- Wishlist -- Tipologia*" di questo manuale

Alla pressione del pulsante "**Salva**" la Wishlist Corrente verrà
salvata come "**Lista Regalo**", gli verranno associati tutti i dati
inseriti mediante l'apposito form di creazione (Titolo Evento, Data
Evento, Organizzatore ecc...), verrà inserita nell'elenco delle Wishlist
Salvate e, infine, verrà svuotata.

**ATTENZIONE! Gli articoli presenti nella Wishlist Corrente, potranno
variare a seconda del fatto che l'utente abbia già inserito degli
articoli in Wishlist durante la stessa sessione di navigazione e/o a
seconda del fatto di aver effettuato l'autenticazione al sito.**

Anche in questo caso i pulsanti "**Aggiungi in Carrello**" e
"**Rimuovi**", presenti in corrispondenza di ogni singolo articolo in
Wishlist consentono rispettivamente di:

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

**[ELENCO DELLE WISHLIST / LISTE REGALO SALVATE IN MOMENTI PRECEDENTI
DALL' UTENTE ATTUALMENTE LOGGATO]{.underline}**

![](./assets/media/image206.png)

Per ciascuna "Lista Regalo" presente in elenco verranno visualizzati
anche i seguenti pulsanti:

- **Rimuovi:** consente all'utente di eliminare dall'elenco la
  corrispondente Lista Regalo.

- **Visualizza:** consente all'utente di visualizzare il dettaglio della
  corrispondente Lista Regalo, sostituendolo a quello della Wishlist
  Corrente.

![](./assets/media/image207.png)

> Nell'intestazione di questa lista verrà inoltre visualizzato:

- il nome assegnato alla lista stessa e la sua data di creazione

- un pulsante "**Torna alla Wishlist corrente"** che l'utente potrà
  utilizzare per tornare a visualizzare all'interno del componente il
  dettaglio della Wishlist Corrente

- un pulsante di "**Stampa**" per consentire al creatore della lista di
  effettuare una stampa della Lista Regalo in questione

> **ATTENZIONE!** Il pulsante di Stampa verrà visualizzato solo nel
> momento in cui sia stato correttamente definito il relativo Template
> (per maggiori informazioni in merito si veda anche quanto indicato
> all'interno della sezione "*Utenti -- Wishlist -- Tipologia*" di
> questo manuale)

- **Modifica:** consente di modificare le informazioni aggiuntive (es.
  Organizzatore dell'evento, Data dell'Evento ecc...) associate alla
  Lista Regalo in esame

- **Anteprima:** consente di visualizzare, mediante collegamento alla
  relativa pagina, la Lista Regalo in esame così come apparirà agli
  utenti che ne dovranno poi acquistare i singoli articoli.

> **ATTENZIONE! Per poter visualizzare un anteprima della Lista Regalo è
> necessario aver inserito e configurato correttamente all'interno della
> pagina "Lista Regalo" l'omonimo componente.**
>
> Per maggiori informazioni in merito si veda anche la sezione
> "*Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componente
> Lista Regalo*" di questo manuale

- **Condividi:** consente di condividere la corrispondente Lista Regalo.

> Cliccando su questo pulsante verrà infatti visualizzata un ulteriore
> sezione all'interno della quale l'utente avrà la possibilità di
> condividere la Lista Regalo in oggetto via social (Facebook, Twitter
> e/o Google +) oppure via mail

![Videate\\wl_lista_regalo_5.bmp](./assets/media/image208.png)

> Per maggiori informazioni relativamente alle modalità di condivisione
> di una Lista Regalo si veda anche la sezione "*Varianti Sito
> Responsive -- Lista Componenti Ecommerce -- Componente Lista Regalo --
> Condivisione Lista Regalo*" di questo manuale

**ATTENZIONE! in fase di visualizzazione di una Lista Regalo (o della
sua Anteprima) i vari articoli verranno filtrati in base alle loro
proprietà di pubblicazione.**

Questo perché dal momento in cui la Lista Regalo è stata creata al
momento in cui viene visualizzato il suo dettaglio, potrebbero essere
cambiate alcune condizioni e quindi alcuni dei suoi articoli potrebbero,
ad esempio, non essere più gestiti all'interno del sito.

