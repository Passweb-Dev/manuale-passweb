# VISITATORI



All'interno di questa sezione è possibile ottenere informazioni
dettagliate relativamente a quelli che sono gli accessi al front end del
sito effettuati da parte di normali visitatori (autenticati e non)
nell'intervallo di tempo indicato e in relazione alla Variante Sito
selezionata mediante il relativo controllo

**ATTENZIONE!** Sono esclusi da questa sezione gli accessi effettuati da
Crawlers, Bot o Tool di vario genere.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_visitatori_1.bmp](./assets/media/image39.png){width="5.98125in"
height="3.515277777777778in"}

Nello specifico all'interno del box "**Visitatori online**" verranno
visualizzati gli utenti attualmente online sul front end del sito.

In questo senso è bene chiarire che con il termine **utenti online** si
intende identificare tutti quegli utenti che hanno interagito in qualche
modo con le pagine web del nostro sito nel corso degli ultimi 30 minuti

In conseguenza di ciò nel momento in cui un utente dovesse visitare una
qualsiasi pagina del nostro sito, verrà considerato immediatamente come
un "Utente online" e verrà quindi visualizzato all'interno del box in
esame (oltre che nel relativo indicatore presente sulla Dashboard del
sito).

Fintantoché continuerà ad interagire con il sito, navigando tra le varie
pagine, aggiungendo articoli in carrello ecc... continuerà ad essere
considerato e conteggiato tra gli Utenti online. Nel momento in cui
dovesse invece smettere di interagire verrà considerato ancora come un
utente online per i primi 30 minuti dopodiché trascorsi **30 minuti di
inattività** verrà considerato come un **utente non attivo** e, in
conseguenza di ciò, non sarà più conteggiato tra gli utenti online.

**ATTENZIONE!** potrebbero anche verificarsi casi in cui, durante il suo
periodo di inattività, l'utente lasci comunque aperte una o più pagine
del sito. In queste condizioni, dipendentemente dalla pagina aperta,
potrebbero innescarsi meccanismi di refresh automatico dei componenti
presenti all'interno della pagina web che porterebbero Passweb a
considerare l'utente come attivo e a conteggiarlo quindi tra gli utenti
online anche se, di fatto, non sta interagendo più in maniera diretta
con il sito.

Per ciascuno degli utenti presenti all'interno di questa sezione
verranno visualizzate le seguenti informazioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visitatori_online.bmp](./assets/media/image40.png){width="3.220833333333333in"
height="1.3868055555555556in"}

**Browser utilizzato (1)**: icona identificativa del browser che
l'utente sta utilizzando per navigare il sito.

**Data della visita (2)**: indicazione relativa a quando è iniziata la
sessione di navigazione del relativo utente

**Id di sessione (3)**: numero identificativo della sessione di
navigazione dell'utente.

Di per se questo dato, legato principalmente a logiche di programmazione
dell'applicativo, potrebbe sembrare non particolarmente interessante. In
realtà è molto importante perché **consente di tracciare il dettaglio di
ogni singola sessione di navigazione effettuata dall'utente**.

Cliccando infatti su questo numero verrà visualizzata infatti la
maschera **"Attività per Sessione -- id della sessione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attivita_per_sessione.bmp](./assets/media/image41.png){width="6.067361111111111in"
height="3.564583333333333in"}

all'interno della quale sarà possibile ottenere informazioni più
dettagliate relativamente alla sessione di navigazione selezionata e
alle pagine effettivamente consultate dall'utente durante questa stessa
sessione (per maggiori informazioni relativamente ai dettagli di
navigazione di ogni singola sessione utente si rimanda a quanto indicato
nel successivo capitolo di questo manuale "*Attività per Sessione*")

La tabella presente nella parte bassa della maschera consente invece
visualizzare lo storico delle visite ricevute dal sito, storico che fa
riferimento, ovviamente, all'intervallo temporale selezionato mediante
il relativo controllo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_storico_visite.bmp](./assets/media/image42.png){width="6.067361111111111in"
height="3.564583333333333in"}

All'interno di questa tabella sarà quindi possibile visualizzare e
monitorare gli accessi al sito da parte di due diverse tipologie di
utenti:

- **Visitatori:** sono i tradizionali utenti web che navigano i
  contenuti del sito senza effettuare l'autenticazione..

- **Visitatori Autenticati:** un normale visitatore diventerà un
  "**Visitatore Autenticato**" nel momento stesso in cui effettuerà il
  login al sito. Per questa specifica tipologia di utenti sarà possibile
  visualizzare, oltre alle informazioni presenti per i "normali"
  visitatori, anche il Nome e il Cognome (o Rag. Sociale) inseriti
  dall'utente stesso all'atto della registrazione sul sito e quindi
  presenti nelle relative anagrafiche Passweb e/o Gestionali

Il pannello di ricerca presente nella parte alta della maschera consente
di filtrare i dati in base alla:

- tipologia del visitatore -- check "**Solo Visitatori Autenticati**"

- identificativo della sessione di visita -- campo **Id**

- indirizzo IP -- campo **Ip**

- Nome/Ragione Sociale/Email dell'utente che ha effettuato la visita
  (ovviamente solo per i visitatori autenticati) -- campo **Nome/Ragione
  Sociale/Email**

Il pulsante "**Esporta**" presente all'interno di questa stessa sezione
consente invece di esportare i dati attualmente presenti in griglia (e
quindi eventualmente filtrati rispetto al totale dei dati stessi)
all'interno di un apposito file .csv.

Per ogni singolo elemento presente in griglia, e quindi per ogni singolo
accesso al sito, sono riportate le seguenti informazioni:

- **Id:** identificativo della sessione di visita dell'utente.

> Come già indicato per i "Visitatori Online" anche in questo caso
> cliccando sull'identificativo di una specifica sessione verrà
> visualizzata la maschera "**Attività per sessione**" all'interno della
> quale poter ottenere informazioni dettagliate sulla relativa sessione
> di navigazione (per maggiori informazioni relativamente ai dettagli di
> navigazione di ogni singola sessione utente si rimanda a quanto
> indicato nel successivo capitolo di questo manuale "*Attività per
> Sessione*")

- **Data Inizio:** data di inizio della corrispondente sessione di
  lavoro, ossia **la data di accesso al sito da parte del relativo
  utente**

- **IP:** indirizzo IP della macchina client dell'utente che ha visitato
  il sito nella data indicata

- **Durata:** durata della sessione di lavoro, ossia il tempo di
  permanenza sul sito da parte dello specifico utente durante l'accesso
  considerato.

- **Utente (solo per Visitatori Autenticati):** Nome/Cognome/Ragione
  Sociale del Visitatore che, durante la sessione in esame, ha
  effettuato l'autenticazione al sito.

> Cliccando sul Nome del Visitatore Autenticato verrà visualizzata la
> maschera "**Attività per Utente**" all'interno della quale poter
> visualizzare il dettaglio delle pagine visitate e delle attività
> effettuate da quello stesso utente **durante TUTTE LE SUE SESSIONI DI
> LAVORO**

![Videate\\statistiche_attivita_per_utente.bmp](./assets/media/image43.png){width="5.98125in"
height="3.515277777777778in"}

> Per maggiori informazioni relativamente alla maschera "Attività
> Utente" si rimanda a quando indicato nel successivo capitolo di questo
> manuale ("*Attività Utente*")

- **Pagine:** consente di visualizzare il numero complessivo di pagine
  viste dall'utente in questione durante la sessione e dunque durante
  l'accesso considerato (il dettaglio di queste pagine può essere
  visualizzato all'interno della sezione "**Attività per utente**")

- **Browser:** consente di visualizzare il browser, con relativa
  versione, utilizzato dall'utente in questione durante la sessione di
  lavoro e quindi durante l'accesso considerato.

