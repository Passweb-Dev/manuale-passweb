# PASSWEB E WA SMART BUSINESS



WA Smart Business (<https://www.wasmartbusiness.com/>) è una piattaforma
che offre strumenti per la gestione di messaggistica su WhatsApp con
funzioni di marketing, automazione, invio campagne, assistenza clienti,
notifiche ... ed è basata sull'utilizzo delle API ufficiali di WhatsApp
Business Platform, un servizio fornito da Meta per consentire alle
aziende di comunicare con i propri utenti in modo scalabile, sicuro e
conforme alle normative sulla privacy e sull'antispam.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\wa_smart_business_1.bmp](./assets/media/image1.png){width="5.6625in"
height="3.5194444444444444in"}

Prima di passare ad analizzare nel dettaglio come poter integrare questa
piattaforma all'interno del proprio sito Passweb e cosa sarà
effettivamente possibile fare o non fare con questo tipo di
integrazione, è bene chiarire subito alcuni concetti fondamentali
relativamente al modo in cui questo tipo di piattaforme andranno poi a
lavorare.

In questo senso, la prima cosa da mettere in evidenza è che Meta
gestisce di fatto due diverse modalità per l'invio dei messaggi a
seconda di chi inizia per primo la comunicazione:

- **Conversazioni iniziate dall'utente**: avvengono quanto è il cliente
  che scrive per primo all'azienda.

> In questo caso l'azienda può rispondere liberamente entro una finestra
> temporale di 24 ore senza costi aggiuntivi e soprattutto senza
> restrizioni sul contenuto del messaggio

- **Conversazioni iniziate dall'azienda**: avvengono quando è l'azienda
  a voler contattare il cliente per prima, oppure dopo che sono
  trascorse più di 24 ore dall'ultimo messaggio scambiato con il
  cliente.

> In questo caso Meta impone regole più rigide sulla comunicazione per
> prevenire abusi generati dall'invio di spam, di comunicazioni
> commerciali non richieste ... e, in questo caso, richiede l'utilizzo
> esclusivo di **template di messaggi pre approvati**.
>
> In sostanza dunque, se è l'azienda a voler contattare il cliente, in
> determinate circostanze, potrebbe anche farlo a patto però di
> utilizzare solo ed esclusivamente dei template di messaggio il cui
> testo è stato preventivamente approvato da Meta stesso. In questo modo
> Meta può tutelare l'esperienza degli utenti impedendo che le aziende
> inviino comunicazioni indesiderate o eccessivamente promozionali.

In questo sistema dunque i Template di messaggio sono chiaramente un
elemento di fondamentale importanza perché di fatto sono gli unici
messaggi che l'azienda potrà inviare per iniziare la comunicazione con
un cliente, comunicazione questa che, una volta accettata dall'utente
potrà poi proseguire (per una durata massima di 24 ore) senza ulteriori
restrizioni né a livello di contenuti né a livello di costi (l'azienda
pagherà solamente il primo messaggio inviato mediante template).

Ogni Template dunque altro non è se non un messaggio strutturato
approvato in anticipo da Meta che può contenere

- **Testo fisso** (non modificabile dopo l'approvazione)

- **Segnaposto variabili** (placeholder), indicati come {{1}}, {{2}},
  ecc. che potranno poi essere sostituiti dinamicamente in fase di
  costruzione del singolo messaggio con valori specifici come ad esempio
  nome utente, codice ordine, data consegna ecc...

- **Componenti opzionali** come pulsanti (es. "Chiama ora", "Visita
  sito"), immagini, video, documenti, link di approfondimento ...

che una volta approvato potrà essere riutilizzato in maniera illimitata
a patto però di non modificarlo (se si vuole cambiare anche solo una
parola sarà necessario creare un nuovo template o comunque rimandare in
approvazione quello modificato e attendere nuovamente la sua validazione
da parte di Meta) e che dovrà anche essere associato ad una ben
determinata categorie (tra quelle ufficiali di meta) categoria questa
che determinerà come il template stesso potrà essere utilizzato e quali
costi avrà.

In questo senso le categorie gestite da Meta sono: **Marketing**,
**Utility (o Transazionali)** e **Autenticazione** e, dipendentemente
dalla categoria cui verranno associati, i Template potranno poi essere
utilizzati rispettivamente per:

- **Marketing**: invio di messaggi promozionali, commerciali, offerte,
  sconti ecc....

> Questo tipo di messaggi, inoltre, potranno essere inviati solo nel
> caso in cui l'utente abbia fornito esplicito consenso

- **Utility (o transazionali)**: invio di messaggi di aggiornamento
  sullo stato degli ordini, carrelli abbandonati, notifiche di
  appuntamenti ...

> A differenza dei messaggi marketing, i messaggi di utility o
> transazionali potranno invece essere inviati anche senza aver raccolto
> un consenso preventivo da parte dell'utente

- **Autenticazione**: invio di codici OTP o link di verifica

> Come per i messaggi di utility anche quelli gestiti dai Template di
> Autenticazione potranno essere inviati senza aver raccolto un consenso
> preventivo da parte dell'utente

**ATTENZIONE!** il costo dei messaggi potrà variare in relazione alla
categoria cui appartiene il template che verrà utilizzato (tipicamente i
messaggi dal costo più elevato sono quelli che utilizzano Template della
categoria Marketing)

Chiariti questi concetti di fondamentale importanza è bene sottolineare
ora che l'integrazione Passweb -- WA Smart Business prevede che:

- I Template di messaggio vengano creati direttamente sulla piattaforma
  terza e da qui dovranno essere inviati in approvazione a Meta

- All'interno di Passweb sarà possibile utilizzare esclusivamente
  Template definiti sulla piattaforma terza (e approvati da Meta)
  associandoli a determinati eventi (es. creazione di un carrello
  abbandonato, cambio di stato di un ordine, notifica di un messaggio in
  area riservata ...).

> In questo senso sarà possibile gestire l'invio automatico di messaggi
> Whatsapp in relazione ai seguenti eventi:

- **Notifica Stato Ordine**: messaggio inviato, all'intestatario del
  documento nel momento in cui l'ordine dovesse entrate in uno degli
  stati gestiti.

- **Notifica carrello abbandonato**: messaggio inviato a seguito della
  creazione di un carrello abbandonato all'utente cui risulta associato
  il carrello

- **Notifica invio messaggio**: notifica dell'inserimento di un nuovo
  messaggio in Area Riservata inviata al destinatario del messaggio
  stesso

- **Notifica lettura messaggio**: notifica di lettura di un messaggio
  inserito in Area Riservata inviata al mittente del messaggio

- **Notifica cambio stato attività**: notifica del cambio di stato di
  un'attività inserita in Area Riservata (sezione Agenda) inviata al
  creatore dell'attività stessa

- **Notifica presa visione attività**: la notifica di presa visione, da
  parte del relativo destinatario, di un'attività ad esso assegnata
  (sezione Agenda). Il destinatario della notifica sarà ovviamente il
  creatore dell'attività stessa

- **Promemoria attività**: notifica della scadenza di un attività
  assegnata ad un determinato utente in Area Riservata (sezione Agenda)

- **Notifica Upload File**: notifica di upload di un file nella sezione
  "Documenti" di Area Riservata inviata all'amministratore associato
  alla cartella in cui viene caricato il file

- **Notifica Download File / Presa visione File**: notifica di download
  (pulsante "Scarica") / presa visione (pulsante "Anteprima) di un nuovo
  file precedentemente caricato nella sezione Documenti dell'Area
  Riservata. Anche in questo caso il destinatario della notifica sarà
  l'amministratore associato alla cartella in cui si trova il file

> Nel momento in cui si dovesse verificare uno degli eventi sopra
> indicati Passweb potrà scatenare l'invio del corrispondente Template
> di Messaggio, invio questo che avverrà comunque sempre e soltanto
> dalla piattaforma di WA Smart Business.

- Per ogni Template potranno essere utilizzate variabili dinamiche (es.
  Nome Utente, Stato Ordine, Totale Ordine ...) che verranno poi
  valorizzate correttamente da Passweb e passate a WA Smart Business in
  maniera tale da personalizzare il relativo messaggio con i dati
  dell'evento che lo ha generato

- I messaggi di carattere commerciale dovranno essere inviati,
  utilizzando i relativi Template, operando direttamente all'interno
  della piattaforma di WA Smart Business

- Non è possibile utilizzare Passweb per inviare agli utenti messaggi a
  "testo libero". Una volta avviata la comunicazione con un utente i
  successivi messaggi dovranno quindi essere inviati e gestiti operando
  direttamente all'interno della piattaforma di WA Smart Business
  attraverso il relativo sistema di Chat

Va da sé, ovviamente, che nel momento in cui si dovesse decidere di
attivare questa integrazione sarà di fondamentale importanza richiede
agli utenti del sito, in fase di registrazione, il proprio numero di
cellulare.

