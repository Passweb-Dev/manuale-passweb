# TRACCIAMENTO SITO



Il "**Monitoraggio del sito**" in ActiveCampaign è una funzionalità che
consente di collegare i processi di marketing alle attività e alle
interazioni degli utenti sul sito web.

Una volta implementato in maniera corretta questo sistema di consente di
sviluppare processi di vendita e di marketing in grado di sfruttare il
targeting comportamentale degli utenti piuttosto che la segmentazione
avanzata, strumenti questi che hanno dimostrato di migliorare
l'esperienza utente e di aumentare le conversioni.

Alcuni esempi di utilizzo in questo senso possono essere:

- Attivazione di un messaggio con un codice coupon da inviare 30 minuti
  dopo che un contatto visualizza una pagina del prodotto del sito ma
  non senza però concludere un acquisto

- Applicazione di un tag per indicare l\'interesse di un contatto e
  iniziare una sequenza di follow-up mirata dopo due o più visite a una
  categoria specifica di prodotti

- Creare automazioni basate sulle pagine visitate.

- Attivare email specifiche quando un contatto visita una pagina chiave

- Aumentare o ridurre il punteggio del contatto o il punteggio del lead
  in base alle visite e alle visualizzazioni di pagine specifiche.

- Personalizzazione del contenuto delle campagne in base alle categorie
  del sito che un contatto ha visualizzato ripetutamente utilizzando il
  contenuto condizionale

- ...

Dal punto di vista tecnico il sistema di tracciamento utilizzato da
ActiveCampaign si sviluppa sia lato client (tracciamento delle pagine
visitate dagli utenti) che lato server (tracciamento di eventi custom)

Nello specifico, il tracciamento lato client viene effettuato via
Javascript, in modo molto simile a quello che avviene anche con Google
Analytics, utilizzando lo snippet di codice presente all'interno del
backend di ActiveCampaign (sezione "**Sito Web -- Monitoraggio del
sito**")

![](./assets/media/image15.png)

**ATTENZIONE! Il tracciamento lato client prende in considerazione solo
ed esclusivamente la visita alle pagine del sito**

In queste condizioni dunque, una volta inserito il codice di
tracciamento in tutte le pagine del sito, l'utente che si collega e
naviga verrà inserito in una sessione collegata a dei cookie e lo
snippet di tracciamento si preoccuperà di inviare ad ActiveCampaign
informazioni relative alle pagine visitate dall'utente durante quella
specifica sessione di navigazione.

Va da sé, ovviamente, che come avviene anche per altri strumenti di
tracciamento (es. Google Analytics), nel momento in cui un utente
dovesse decidere di rifiutare i cookie o di disabilitare javascript
risulterà poi impossibile tracciarlo in maniera corretta.

Un'ulteriore considerazione di fondamentale importanza da fare è quella
che riguarda poi l'effettiva visualizzazione dei dati inviati ad
ActiveCampaign. In questo senso infatti occorre sottolineare che il
sistema di tracciamento messo in piedi da ActiveCampaign è volto
principalmente a gestire specifiche azioni di marketing automation e, in
conseguenza di ciò, **ogni evento tracciato all'interno del sito** (es.
pageview) **dovrà necessariamente essere legato su ad uno specifico
utente dotato di un indirizzo mail valido**

In sostanza dunque i dati inviati ad ActiveCampaign potranno essere
visualizzati solo nel momento in cui sarà anche possibile associarli ad
uno specifico contatto e, in queste condizioni, verranno visualizzati
proprio nell'anagrafica di quello stesso contatto (sezione "**Attività
Recenti**")

![](./assets/media/image16.png)

Un punto fondamentale in tutto il processo, quindi, sarà proprio quello
di riuscire ad identificare i vari contatti a cui associare gli eventi
registrati dal sistema di tracciamento (per maggiori informazioni in
merito si vedano anche i successivi capitoli di questo manuale)

Per quel che riguarda invece il tracciamento lato server, questo
riguarda più nel dettaglio la possibilità di monitorare eventi custom.
Deve essere attivato in maniera specifica operando sempre dalla pagina
"**Sito Web -- Monitoraggio del sito**"

![](./assets/media/image17.png)

e, soprattutto, richiede di interagire con le API messe a disposizione
da ActiveCampaign utilizzando un linguaggio lato server

**ATTENZIONE! attualmente questo tipo di tracciamento NON è implementato
nativamente all'interno dei siti Passweb**

