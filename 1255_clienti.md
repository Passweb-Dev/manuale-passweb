# CLIENTI



All'interno di questa sezione è possibile configurare e gestire l'invio
al corrispondente Store Mailchimp, dei clienti presenti all'interno del
proprio sito Ecommerce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp-ecommerce_7.bmp](./assets/media/image127.png){width="5.809722222222222in"
height="3.5215277777777776in"}

Per comprendere il funzionamento dei parametri presenti all'interno di
questa sezione del Wizard è necessario chiarire, innanzitutto, un
concetto di fondamentale importanza.

MailChimp consente di inviare due diverse tipologie di Email:

- **Email Cumulative (Bulk Email)** come ad esempio Newsletter Mensili,
  Email Promozionali ecc...(una stessa mail inviata a più destinatari)

- **Email Transazionali** (**Transactional Email**) come ad esempio
  Email successive alla creazione di un account, alla creazione di un
  carrello abbandonato, a un cambio di stato di alcuni ordini
  ecc...(email inviate a singoli utenti)

Le **Email cumulative** potranno essere inviate solo ed esclusivamente a
quegli utenti che hanno acconsentito in maniera esplicita ad iscriversi
ad una determinata Lista e che sono quindi stati inseriti all'interno di
questa stessa lista nello stato di "**Subscribed**".

Generalmente questi sono gli utenti che, in fase di registrazione o in
un qualsiasi altro momento hanno deciso di iscriversi, mediante
l'apposito componente Passweb, alla Newsletter del sito acconsentendo
quindi anche a ricevere comunicazioni di carattere commerciale.

Le **Email transazionali** sono invece Email più mirate, rivolte
generalmente ad uno specifico utente ed inviate a seguito di una
determinata azione, come ad esempio il cambio di stato di un ordine o la
creazione di un carrello abbandonato. Tali mail potranno essere inviate
a tutti gli utenti presenti all'interno di una Lista indipendentemente
dal fatto che questi stessi utenti abbiano acconsentito o meno, in
maniera esplicita, a far parte di quella stessa lista e quindi
indipendentemente dal fatto che siano stati inseriti o meno all'interno
della Lista nello stato di Subscribed. Anche utenti in stato
"Unsubscribed" o "Non-Subscribed" potranno quindi ricevere email
transazionali.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp-ecommerce_11.bmp](./assets/media/image128.png){width="6.705555555555556in"
height="3.675in"}

Ovviamente utenti in grado di poter ricevere mail cumulative potranno
tranquillamente ricevere anche ogni tipo di mail transazionali.

Al contrario utenti abilitati alla ricezione di mail transazionali non
potranno mai ricevere mail cumulative.

Per maggiori informazioni in merito a stati e tipologie di utenti in
MailChimp si rimanda alla specifica documentazione di prodotto
(<https://mailchimp.com/help/about-your-contacts>).

Chiarito questo concetto di fondamentale importanza, veniamo ora ai
parametri di configurazione presenti all'interno di questa sezione:

**Tipo di sottoscrizione su MailChimp**: consente di decidere, tra tutti
i clienti del proprio sito Ecommerce, quali e in che condizioni dovranno
essere inviati alla Lista collegata allo Store Passweb creato su
MailChimp.

E' possibile selezionare uno dei seguenti valori:

- **Tutti gli utenti:** selezionando questa opzione mediante
  l'operazione di sincronizzazione manuale verranno inviati, ed iscritti
  alla Lista collegata allo Store MailChimp, **nello stato di
  Subscribed**, tutti i clienti già presenti all'interno del proprio
  sito Ecommerce indipendentemente dal fatto che essi abbiano o meno
  acconsentito esplicitamente a ricevere comunicazioni di carattere
  commerciale.

> Allo stesso modo, in queste condizioni, tutti i nuovi clienti del sito
> (utenti che si registrano e / o che effettuano ordini) verranno
> automaticamente inseriti nella Lista collegata allo Store MailChimp
> **sempre nello stato di Subscribed** indipendentemente, ancora una
> volta, dal fatto di aver acconsentito o meno a ricevere comunicazioni
> di carattere commerciale.
>
> **ATTENZIONE!** Questa opzione abilitando, di fatto, ogni utente del
> sito alla ricezione di mail di carattere commerciale indipendentemente
> da quella che è stata, in tal senso, la sua specifica scelta, potrebbe
> violare le norme di Privacy richieste dal GDPR

- **Tutti gli utenti (in base all'iscrizione a MailChimp):**
  selezionando questa opzione mediante l'operazione di sincronizzazione
  manuale verranno inviati, ed iscritti alla Lista collegata allo Store
  MailChimp tutti i clienti già presenti all'interno del proprio sito
  Ecommerce.

> In questo caso però se il cliente dovesse già essere presente nella
> Lista collegata allo Store il suo stato (Subscribed o Non-Subscribed)
> resterà invariato. Nel caso in cui, invece il cliente non dovesse
> essere presente nella Lista verrà aggiunto nello stato di
> Non-Subscribed (e sarà quindi abilitato alla ricezione delle sole mail
> transazionali)
>
> I nuovi clienti del sito verranno iscritti alla Lista collegata allo
> Store Mailchimp e lo stato di Subscribed verrà assegnato loro solo ed
> esclusivamente nel caso in cui abbiano acconsentito, esplicitamente, a
> ricevere anche comunicazioni di carattere commerciale. In caso
> contrario verranno iscritti alla Lista nello stato di Non-Subscribed
> (e saranno quindi abilitati alla ricezione delle sole mail
> transazionali)
>
> In queste condizioni sarà quindi di fondamentale importanza accertarsi
> di aver inserito tanto nel form di registrazione al sito quanto nel
> modulo di One Step Checkout il form di iscrizione a Mailchimp con
> all'interno un campo mediante il quale poter consentire agli utenti
> del sito di accettare o rifiutare la ricezione di mail di carattere
> commerciale.
>
> **ATTENZIONE!** Questa opzione è quella che meglio soddisfa le norme
> in materia di privacy richieste dal GDPR in quanto, da una parte
> lascia agli utenti del sito la possibilità di decidere se ricevere o
> meno comunicazioni di carattere commerciale e dall'altra abilita
> comunque MailChimp ad inviare a tutti gli utenti del sito mail
> transazionali.

- **Solo gli utenti iscritti a MailChimp:** selezionando questa opzione
  l'operazione di sincronizzazione manuale non altererà in alcun modo il
  numero o lo stato degli iscritti alla Lista collegata allo Store.

> In queste condizioni infatti, se il cliente dovesse essere già
> presente nella Lista collegata allo Store il suo stato (Subscribed o
> Non-Subscribed) resterà invariato. Nel caso in cui, invece il cliente
> non dovesse essere già presente nella Lista NON verrà mai inserito.
>
> I nuovi clienti del sito potranno essere iscritti alla Lista collegata
> allo Store Mailchimp solo ed esclusivamente nel momento in cui avranno
> acconsentito, esplicitamente, a ricevere comunicazioni di carattere
> commerciale.
>
> Come nel caso precedente, anche questa volta diventa di fondamentale
> importanza accertarsi di aver inserito tanto nel form di registrazione
> al sito quanto nel modulo di One Step Checkout il form di iscrizione a
> Mailchimp con all'interno un campo mediante il quale poter consentire
> agli utenti del sito di accettare o rifiutare la ricezione di mail di
> carattere commerciale.
>
> **ATTENZIONE!** In queste condizioni, ovviamente, all'interno della
> Lista collegata allo Store Mailchimp avremo solo ed esclusivamente
> utenti nello stato di Subscribed mentre non saranno mai presenti
> utenti in grado di ricevere solo mail transazionali

**Data**: consente di impostare una specifica data che verrà poi
considerata come data di registrazione al sito e che verrà utilizzata
come filtro per individuare gli utenti che dovranno effettivamente
essere trasferiti nella corrispondente Lista MailChimp

Impostando una specifica data, la procedura di importazione clienti
prenderà quini in considerazione solo ed esclusivamente quei clienti del
sito la cui data di registrazione è successiva a quella impostata

Nel caso in cui il campo in esame dovesse invece essere lasciato vuoto,
la procedura di importazione clienti su MailChimp, lanciata mediante il
corrispondente pulsante presente nella barra degli strumenti prenderà in
considerazione tutti i clienti attualmente presenti all'interno del
proprio sito Ecommerce, indipendentemente da quella che è la loro data
di registrazione al sito.

**ATTENZIONE!** Nel caso in cui si dovesse impostare una specifica data,
in relazione alla quale effettuare la sincronizzazione dei Clienti, e/o
variare una data precedentemente impostata, **è indispensabile, prima di
effettuare la sincronizzazione cliccare sul pulsante** **"Salva"**

**Filtro Utenti:** consente di impostare un determinato Filtro Utenti
che verrà poi utilizzato per individuare, tra tutti gli utenti del sito,
quelli che dovranno effettivamente essere trasferiti nella
corrispondente Lista MailChimp.

**ATTENZIONE!** Il filtro impostato all'interno di questo campo andrà in
AND con l'eventuale data di registrazione settata in corrispondenza del
precedente parametro "Data"

Per maggiori informazioni relativamente a come poter costruire un filtro
utenti si veda anche quanto indicato all'interno del capitolo "*Utenti
-- Siti Ecommerce -- Gruppi Utenti Sito -- Filtri Utente e Filtri
Articolo -- Filtri Utente*" di questo manuale

Il pulsante "**Sincro Clienti**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sincro_clienti.bmp](./assets/media/image124.png){width="0.5090277777777777in"
height="0.17777777777777778in"} ) presente nella barra degli strumenti
di uno Store correttamente connesso, consente di avviare manualmente la
procedura di importazione sulla Lista collegata allo Store MailChimp
attualmente selezionato, dei clienti presenti all'interno del proprio
sito Ecommerce.

**ATTENZIONE!** Oltre ai clienti, verranno importati sullo Store
MailChimp in esame, anche tutti gli ordini attualmente presenti sul sito
Passweb e relativi, ovviamente, a questi stessi clienti

Una volta lanciata la procedura di importazione clienti sullo Store
Mailchimp l'esito verrà notificato via mail all'indirizzo indicato
all'interno della sezione "Posta/SMS" del Wizard (campo E-mail).

La procedura di importazione clienti nella Lista collegata allo Store
MailChimp, prenderà in considerazione, ovviamente i **soli clienti che
soddisfano le condizioni impostate mediante i parametri precedentemente
esaminati e che hanno anche un indirizzo mail correttamente impostato
all'interno della loro anagrafica**.

Inoltre nel caso in cui, per siti multilingua, si sia deciso di gestire
uno Store MailChimp diverso per ogni singola lingua del sito, la
procedura di sincronizzazione di un determinato Store prenderà
inconsiderazione solamente i clienti la cui lingua coinciderà con la
lingua associata allo Store stesso.

**ATTENZIONE!** La lingua di un utente è determinata sulla base della
sua Nazione di appartenenza

Supponendo dunque di sincronizzare i clienti dello Store Italiano,
verranno processati, di base, i soli clienti Italiani

**L'unica eccezione in tal senso è rappresentata dallo Store di
Default** (marcato come tale attraverso l'apposito parametro). Nella
procedura di sincronizzazione clienti dello Store di default infatti,
oltre ai clienti la cui lingua coincide con quella dello Store, verranno
processati e presi in considerazione anche tutti quegli utenti la cui
lingua non coincide con nessuna delle lingue associate agli Store
MailChimp attualmente gestiti.

Come per la sincronizzazione articoli, anche la procedura di
sincronizzazione clienti, dovrebbe essere eseguita solo la prima volta o
al massimo nel momento in cui si dovesse rendere necessario, per qualche
ragione, allineare la base dati del proprio sito (a livello di clienti)
con quella presente all'interno dello Store MailChimp.

A regime, infatti, l'invio di nuovi clienti allo Store MailChimp avverrà
in maniera del tutto automatica seguendo la normale operatività del sito
e le impostazioni settate per il parametro "**Tipo di sottoscrizione su
MailChimp**".

Inoltre al termine di ogni sincronizzazione "Sito -- Gestionale" Passweb
si preoccuperà anche di eseguire, in maniera del tutto automatica e
secondo la stessa logica descritta fino ad ora, la sincronizzazione
clienti verso tutti gli Store MailChimp correttamente connessi

**ATTENZIONE!** I dati inviati a MailChimp, relativamente ai clienti,
del sito possono variare, ovviamente, in relazione a come è stato
costruito il form di iscrizione a MailChimp.

**In ogni caso, per ovvie ragioni, la mail dell'utente sarà l'unico dato
trasmesso in qualsiasi condizione.**

