# COMPONENTI E-COMMERCE -- NOTIFICA DISPONIBILITA'



Il Componente **"Notifica Disponibilità"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_notifica_disponibilita_res.bmp](./assets/media/image584.png)

**può essere inserito unicamente all'interno dei componenti Ecommerce di
primo livello "Scheda Prodotto" e "Catalogo Ecommerce" o simili** (es.
"Offerte / Novità", "Abbinati" ecc...)**.**

Grazie a questo componente, in particolare, sarà possibile inserire
all'interno del sito un modulo mediante il quale gli utenti potranno
richiedere di essere avvisati via mail nel momento in cui determinati
articoli, attualmente non disponibili, dovessero tornare ad essere
nuovamente acquistabili.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_tutti.bmp](./assets/media/image585.png)

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata la sua maschera di gestione e
configurazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\notifica_disponibilita_configurazione_res.bmp](./assets/media/image586.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito

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

- **Label:** consente di impostare una stringa di testo che verrà poi
  visualizzata all'interno del sito come intestazione del componente

- **Posizionamento dei Campi della notifica:** consente di posizionare
  gli elementi principali del componente secondo uno schema
  prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- Il pulsante per la richiesta di notifica

- Il campo di input per l'inserimento dell'indirizzo mail

- L'eventuale informazione relativa alle taglie / colori gestiti
  sull'articolo

> E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame, permettendo dunque, già in fase di
> configurazione del componente stesso di decidere quale elemento dovrà
> essere visualizzato prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

- **Pagina di destinazione per l'autenticazione:** consente di indicare,
  selezionandola dal sottostante albero delle pagine, la specifica
  pagina cui dovrà essere ridiretto un utente non autenticato nel
  momento in cui il componente stesso fosse configurato per poter essere
  utilizzato dai soli utenti registrati e l'utente dovesse cliccare
  sull'apposito messaggio presente all'interno del componente

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

**ATTENZIONE! Il componente Notifica Disponibilità, pur essendo
configurato in maniera corretta, potrà essere effettivamente attivato
solo ed esclusivamente nel momento in cui il parametro "Gestione
Disponibilità", presente alla pagina "*Catalogo -- Configurazione
Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca.*" del Wizard, sia stato
impostato sul valore "Ai soli utenti registri" o "A tutti"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\notifica_disponibilita.bmp](./assets/media/image587.png)

Dipendentemente dal valore assunto dal parametro evidenziato in figura
infatti, il componente Notifica Disponibilità potrà comportarsi in un
modo oppure in un altro.

Nello specifico nel caso in cui il parametro "**Gestione Notifica
Disponibilità**" sia stato impostato sul valore:

- **No: il componente "Notifica Disponibilità" non verrà attivato** e,
  di fatto, non sarà quindi possibile abilitare il sistema di gestione
  delle notifiche relative alle disponibilità dei vari prodotti.

> In queste condizioni, inserendo il componente "Notifica Disponibilità"
> all'interno del sito e configurandolo in maniera corretta, verrà
> comunque visualizzato un apposito messaggio di avviso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_no.bmp](./assets/media/image588.png)

- **Ai soli utenti Registrati:** il componente "Notifica Disponibilità"
  verrà correttamente attivato ma sarà disponibile ai soli utenti
  registrati.

> In queste condizioni, dunque, nel momento in cui un utente dovesse
> visitare, ad esempio, la pagina prodotto di un articolo attualmente
> non disponibile in cui è stato inserito il componente "Notifica
> Disponibilità", senza aver ancora effettuato l'autenticazione, in
> corrispondenza di questo stesso componente verrà visualizzato un
> apposito messaggio (personalizzabile alla sezione "Gestione Testi /
> Messaggi Sito" del Wizard) per informarlo relativamente alla necessità
> di effettuare l'autenticazione al sito prima di poter richiedere di
> essere avvisato quando il prodotto dovesse tornare ad essere
> disponibile.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_utenti_registrati.bmp](./assets/media/image589.png)

> Il messaggio in questione sarà inoltre un link che ricondurrà l'utente
> direttamente alla pagina impostata all' intero del campo "**Pagina di
> destinazione per l'autenticazione**" presente tra i parametri di
> configurazione del componente "Notifica Disponibilità".
>
> Una volta effettuata l'autenticazione, l'utente sarà automaticamente
> ricondotto alla precedente pagina prodotto dove il componente
> "Notifica Disponibilità" visualizzerà ora un messaggio diverso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_utenti_registrati2.bmp](./assets/media/image590.png)

> Cliccando su questo messaggio, e richiedendo espressamente di essere
> avvisato nel momento in cui l'articolo dovesse tornare disponibile,
> l'utente riceverà una mail non appena la disponibilità (**memorizzata
> in Passweb**) dell'articolo in esame torni ad essere maggiore di zero.
>
> L'indirizzo mail cui verrà inviata tale notifica sarà ovviamente
> quello inserito dall'utente stesso in fase di registrazione al sito.

- **A tutti:** il componente "Notifica Disponibilità" verrà
  correttamente attivato e sarà disponibile per tutti gli utenti del
  sito, registrati e non.

> In queste condizioni dunque nel momento in cui un utente autenticato
> dovesse visitare, ad esempio, la pagina prodotto di un articolo
> attualmente non disponibile in cui è stato inserito il componente
> "Notifica Disponibilità", visualizzerà esattamente lo stesso messaggio
> del caso precedente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_utenti_registrati2.bmp](./assets/media/image590.png)

> La mail cui verrà inviata la notifica, sarà anche in questo caso
> quella inserita dall'utente stesso in fase di registrazione al sito.
>
> A differenza del caso precedente però, nel momento in cui a visitare
> la pagina dovesse essere ora un utente **non autenticato**, il
> componente "Notifica Disponibilità" visualizzerà un apposito campo di
> input all'interno del quale l'utente, pur non essendo ancora
> registrato al sito, potrà comunque inserire la mail cui dovrà essere
> inviata la notifica di "prodotto nuovamente disponibile"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_tutti.bmp](./assets/media/image585.png)

Per articoli gestiti a taglie/colori prima del pulsante "Avvisami" o del
link per richiedere la notifica di disponibilità, verrà visualizzato
anche un apposito menu a tendina mediante il quale l'utente potrà
indicare la specifica taglia/colore del prodotto per cui desidera
effettivamente ricevere la notifica di disponibilità.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_taglie.bmp](./assets/media/image591.png)

**ATTENZIONE! All' interno del menu a tendina verranno ovviamente
visualizzate le sole taglie/colori attualmente non disponibili**

Per maggiori informazione relativamente all'attivazione e alla gestione
del sistema di notifiche sulle disponibilità prodotto si veda anche la
sezione *"MailChimp -- Notifiche Disponibilità -- Passweb e MailChimp"*
di questo manuale

**ATTENZIONE! Si ricorda che il sistema di gestione delle notifiche di
disponibilità dei prodotti può essere attivato solo ed esclusivamente
nel momento in cui il parametro "Gestione Acquisto" sia stato impostato
sul valore "Acquista solo se disponibile" e l'effettiva disponibilità
degli articoli sia quindi demandata interamente ai valori memorizzati
nel database del sito e aggiornati all'ultima sincronizzazione utile.**

