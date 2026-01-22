# INVIO DEI DATI A BRAINLEAD



Sulla base di quanto evidenziato nei precedenti capitoli di questo
manuale, dovrebbe ormai essere abbastanza chiaro che una volta
configurato tutto in maniera corretta, la discriminante principale che
regola l'invio dei dati da Passweb a Brainlead sarà sempre
l'accettazione da parte dell'utente ad essere tracciato, accettazione
questa che dovrebbe essere gestita da un'apposita piattaforma CMP (es.
Iubenda, Cookiebot ...)

Nel caso in cui l'utente dovesse negare il consenso al tracciamento, i
blocchi attivabili su Passweb potranno evitare l'attivazione sia del
tracciamento lato client che di quello lato server, per cui in queste
condizioni a Brainlead (come a qualsiasi altro servizio analogo) non
verrà passata alcuna informazione.

Nel momento in cui l'utente dovesse invece decidere di fornire il
proprio consenso verranno correttamente attivati sia il tracciamento
lato client che quello lato server.

Il primo (tracciamento client) si preoccuperà di registrare e
trasmettere a Brainlead informazioni relative alle pagine visitate
dall'utente che sta navigando il sito (pageview).

Il secondo (tracciamento server) si preoccuperà invece di inviare a
Brainlead informazioni relative agli eventi di **aggiunta articoli in
carrello**, **creazione di nuovi ordini** e **registrazione di nuovi
utenti**.

In particolare, contestualmente all'**aggiunta di un articolo in
carrello** verranno inviati a Brainlead i seguenti dati:

- **Codice**

- **Categoria Merceologica** (comprese eventuali categorie padre della
  categoria di appartenenza dello specifico prodotto)

- **Titolo**

- **Descrizione**

- **Url Immagine negozio**

- **Url prodotto**

- **Quantità**

- **Prezzo** (del singolo articolo)

Contestualmente alla registrazione di un nuovo utente potranno essere
inviati a Brainlead i seguenti dati:

- **Nome**

- **Cognome**

- **Email**

- **Telefono**

- **Fax**

- **Indirizzo**

- **CAP**

- **Città**

- **Stato**

- **Eventuali campi custom** definiti su Brainlead ed inseriti anche nel
  form di registrazione

Infine contestualmente alla conferma di un nuovo ordine verranno inviati
a Brainlead le seguenti informazioni:

- **Email dell'utente intestatario dell'ordine**

<!-- -->

- **Data di invio dell'ordine a Brainlead**

- **Nome** (utente intestatario)

- **Cognome** (utente intestatario)

- **Data ordine**

- **Numero Ordine**

- **Valuta**

- **Stato Ordine** (relativo agli stati gestiti su Passweb)

- **Indirizzo Spedizione**

- **Città Spedizione**

- **CAP Spedizione**

- **Stato Spedizione**

- **Nazione Spedizione**

- **Indirizzo Fatturazione**

- **Città Fatturazione**

- **CAP Fatturazione**

- **Stato Fatturazione**

- **Nazione Fatturazione**

- **Totale Merce**

- **Tasse totali (IVA)**

- **Totale spese di spedizione**

- **Modalità di Pagamento**

- **Modalità di spedizione**

- **Codici Coupon**

Per quel che riguarda l'effettiva visualizzazione di questi dati
all'interno di Brainlead occorre fare una considerazione di fondamentale
importanza.

Come già evidenziato nei precedenti capitoli di questo manuale infatti,
il sistema di tracciamento messo in piedi da Brainlead è volto
principalmente a gestire specifiche azioni di marketing automation e, in
conseguenza di ciò, **ogni evento tracciato all'interno del sito**
(pageview, aggiunta / rimozione articoli in carrello, creazione /
aggiornamento del carrello abbandonato ...) **dovrà necessariamente
essere legato, su Brainlead, ad uno specifico utente dotato di un
indirizzo mail valido** (oltre che di un numero di cellulare nel momento
in cui si dovesse decidere di attivare e gestire su Brainlead anche il
canale degli SMS).

**I dati inviati verranno quindi effettivamente visualizzati sulla
Timeline di Brainlead solo nel momento in cui i diversi eventi potranno
essere effettivamente associati ad uno specifico utente, e soltanto nel
momento in cui si sia verificato almeno uno degli eventi server
tracciati.**

In altre parole se un utente dovesse navigare il sito da anonimo (senza
aver effettuato cioè la registrazione e l'autenticazione al sito)
Passweb invierà comunque i dati di tracciamento a Brainlead (posto
chiaramente che lo stesso utente abbia dato esplicito consenso) ma, non
avendo a disposizione un indirizzo mail cui associarli, questi non
potranno essere assegnanti a nessuno degli utenti effettivamente
presenti su Brainlead e, pertanto, non verranno visualizzati.

Nel momento in cui lo stesso utente, nell'ambito della stessa sessione
di navigazione dovesse effettuare la registrazione al sito
(registrazione che è uno degli eventi server tracciati da Passweb verso
Brainlead) oppure dovesse effettuare l'autenticazione (perché già
registrato) e successivamente l'aggiunta di un articolo in carrello
(aggiunta in carrello che è un altro degli eventi tracciati) allora, da
questo momento in avanti, sarà effettivamente possibile assegnare tutti
i dati di tracciamento ad uno specifico utente Brainlead e sarà proprio
a partire da questo momento che verranno visualizzati, sulla Timeline di
quello stesso utente, tutti i dati inviati da Passweb in quella
specifica sessione di navigazione (anche quelli relativi a prima della
registrazione e/o del login e dell'aggiunta di almeno un articolo in
carrello).

![](./assets/media/image4.png)

Sulla base dei dati ricevuti, infine, sarà possibile attivare e
configurare, direttamente in Brainlead, determinate tipologie di
automazioni.

**ATTENZIONE!** per maggiori informazioni su come poter attivare e
configurare le automazioni (es. carrelli abbandonati) in Brainlead è
necessario fare riferimento alla relativa documentazione e/o al relativo
supporto tecnico.
