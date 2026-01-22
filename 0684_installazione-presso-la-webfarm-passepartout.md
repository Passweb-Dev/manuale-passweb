# INSTALLAZIONE PRESSO LA WEBFARM PASSEPARTOUT



Nel caso di installazioni Passcom presso la server farm di Passepartout
sarà necessario, per prima cosa, impostare il radio button presente
nella parte alta della maschera sul valore **"Installazione Web Farm"**
in maniera tale da poter visualizzare tutti i parametri necessari per
realizzare l'integrazione sito-gestionale in questa specifica
configurazione di prodotto.

![](./assets/media/image143.png)

In queste condizioni, dunque, sarà necessario specificare un valore per
i seguenti parametri:

- **Dominio:** dominio dell'installazione gestionale all'interno della
  web Farm Passepartout a cui collegare il sito web.

- **Sigla Azienda:** : sigla dell'azienda utilizzata dallo studio
  (tipicamente STD). L'azienda indicata all'interno di questo campo sarà
  poi quella utilizzata per gestire l'integrazione tra sito e
  gestionale. A differenza di tutte le altre aziende presenti
  nell'installazione gestionale dunque, l'azienda qui indicata non avrà
  mai la possibilità di essere esportata e gestita all'interno del sito
  web come una normale azienda cliente.

**NOTA BENE**: l'azienda indicata all'interno del campo **Sigla
Azienda** non avrà mai la possibilità di essere esportata e gestita
all'interno del sito web come una normale azienda cliente. Per questa
ragione si consiglia di indicare all'interno di questo campo la sigla
dell'azienda tipicamente utilizzata dal commercialista per effettuare le
sue elaborazioni (es. STD) e mai una sua azienda cliente.

- **Login Server:** login dell'utente amministratore del gestionale (la
  stessa login utilizzata dall'amministratore di Passcom per connettersi
  al gestionale tramite Predesk).

- **Password Server:** password utilizzata dell'utente amministratore
  del gestionale (la stessa password utilizzata dall'amministratore di
  Passcom per connettersi al gestionale tramite Predesk).

- **Sottodominio Predesk:** codice identificativo dell'installazione
  gestionale all'interno della web Farm Passepartout a cui collegare il
  sito web

- **Gruppo del gestionale dei Commercialisti:** nome del gruppo creato
  in Passcom e i cui utenti avranno accesso all'area riservata del sito
  come utenti di tipo COMMERCIALISTA

- **Crea Gerarchia Utenti del Gestionale:** consente, se selezionato, di
  generare alla sincronizzazione, relativamente agli utenti Passcom, la
  gerarchia creata in automatico da Passweb (vedi anche sezione "UTENTI
  -- UTENTI AREA RISERVATA -- GESTIONE UTENTI -- GERARCHIA UTENTI
  PASSCOM" di questo manuale).

> In particolare, selezionando tale parametro, alla successiva
> sincronizzazione verrà automaticamente creata in Passweb la gerarchia
> utenti descritta alla pagina "Utenti -- Gerarchie -- Gerarchia Utenti
> Passcom" di questo manuale e al suo interno verranno collocati, nei
> rispettivi gruppi, gli utenti di tipo COMMERCIALISTA, DIPENDENTE e
> AZIENDA.
>
> Non selezionando il parametro sopra indicato invece, alla successiva
> sincronizzazione non verrà creata in automatico nessuna gerarchia
> utenti e nessun gruppo, lasciando quindi libero l'amministratore del
> sito di crearsi, attraverso il menu **"Utenti"** del Wizard tutti i
> gruppi che desidera, e di inserire al loro interno anche utenti di
> tipo COMMERCIALISTA, DIPENDENTE e AZIENDA esportati e prelevati
> direttamente da Passcom.

**NOTA BENE**: per poter eliminare la gerarchia degli utenti Passcom
eventualmente creata in automatico da Passweb alla sincronizzazione, non
è sufficiente deselezionare il parametro "Crea Gerarchia Utenti del
Gestionale", ma occorre anche eliminare manualmente la relativa
gerarchia agendo dal menu "Utenti - Gruppi" del Wizard.

La sezione "Docuvision" consente invece di settare i parametri relativi
all'integrazione tra il proprio sito commercialista e Docuvision.

Nello specifico il parametro:

- **Gestione Pagine:** consente di decidere se attivare la gestione del
  documentale Passepartout a Pagine oppure quella a Revisioni.

> In particolare, selezionando questo parametro, Passweb considererà
> attiva la gestione di Docuvision a Pagine.
>
> Nel caso in cui il parametro in oggetto non venga selezionato, Passweb
> considererà invece attiva la gestione di Docuvision a Revisioni.
>
> **Come indicato nella relativa etichetta il parametro "Gestione
> Pagine" ha effetto solo ed esclusivamente nel caso in cui la versione
> del gestionale sia inferiore alla 2011B**
>
> **Nel caso in cui la versione del gestionale sia maggiore o uguale
> alla 2011B sarà possibile impostare, per ogni singolo documento, la
> sua gestione a pagine o a revisioni direttamente all'interno di
> Passcom**

**NOTA BENE**: per maggiori informazioni su come impostare, direttamente
all'interno del gestionale, uno specifico documento Docuvision a Pagine
o a Revisioni si rimanda all'apposito manuale

- **Notifiche SMS per nuovi documenti** -- visualizzato solo nel caso in
  cui sia stato correttamente configurato un account su SMS Hosting

> Consente, se abilitato, di inviare alle varie aziende esportate e
> gestite all'interno del sito notifiche SMS relative all'inserimento,
> in Docuvision, di nuovi documenti

- **Notifiche Whatsapp per nuovi documenti** -- visualizzato solo nel
  caso in cui sia stata correttamente configurata l'integrazione tra il
  proprio sito e WA Smart Business

> Consente, se abilitato, di inviare alle varie aziende esportate e
> gestite all'interno del sito notifiche Whatsapp relative
> all'inserimento, in Docuvision, di nuovi documenti
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Passweb e WA Smart Business*" di questo
> manuale

- **Notifiche Telegram per nuovi documenti** -- visualizzato solo nel
  caso in cui sia stata correttamente configurata l'integrazione tra il
  proprio sito e Telegram

> Consente, se abilitato, di inviare alle varie aziende esportate e
> gestite all'interno del sito notifiche Telegram relative
> all'inserimento, in Docuvision, di nuovi documenti
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Passweb e Telegram*" di questo manuale

**ATTENZIONE!** per inviare notifiche SMS, Telegram e/o Whatsapp, oltre
all'attivazione dei parametri in esame e al fatto di aver configurato in
maniera corretta l'integrazione tra il proprio Sito Commercialista e le
relative piattaforme Marketing, sarà necessario, ovviamente, aver
assegnato ad ogni azienda gestita un numero di telefono valido e aver
pubblicato correttamente dei documenti all'interno delle Classi
Docuvision gestite sul sito

Per maggior informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Siti Commercialista Area Riservata --
Documenti -- Ricerca Documenti Passcom -- Notifiche*" di questo manuale

Infine, all'interno della sezione "**Web API**" è possibile impostare le
credenziali di un utente Passcom appositamente abilitato alla gestione
delle relative API

![](./assets/media/image144.png)

**ATTENZIONE!** l'utilizzo delle Web Api Passcom è indispensabile per
poter attivare e gestire le notifiche via mail e/o sms relative alla
pubblicazione di nuovi documenti in una delle Classi Docuvision
pubblicate all'interno del sito. Per maggiori informazioni in merito si
veda anche quanto indicato nel relativo capitolo di questo manuale
("*Siti Commercialista Area Riservata -- Documenti -- Ricerca Documenti
Passcom -- Notifiche*")

Per maggiori informazioni relativamente a come poter invece effettuare
generiche chiamate alle Web API di Passcom si rimanda a quanto indicato
nel relativo capitolo di questo manuale ("*Configurazione -- Passcom
Configurazione Gestionale -- Web API Passcom*") e, soprattutto, alla
relativa documentazione di prodotto.

