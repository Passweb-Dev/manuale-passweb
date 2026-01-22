# ISCRIZIONE ALLA NEWSLETTER ACTIVECAMPAIGN IN FASE DI REGISTRAZIONE AL SITO



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui l'esigenza dovesse essere quella di consentire agli utenti del
sito di iscriversi alla newsletter direttamente in fase di registrazione
al sito, sarà necessario utilizzare il componente "**Newsletter**"
inserendolo all'interno del Componente di primo livello **Registrazione
Utente** e impostando, in fase di configurazione, il campo "**Tipo di
Integrazione**" sul valore "**ActiveCampaign**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_activecampaign.bmp](./assets/media/image157.png)

**ATTENZIONE! l'iscrizione alla Newsletter ActiveCampaign dal form di
registrazione utente non prevede il double opt-in**

Ciò significa dunque che nel caso in cui l'utente dovesse decidere, in
fase di registrazione al sito, di iscriversi anche alla Newsletter il
suo inserimento nella relativa Lista di ActiveCampaign sarà immediato e
non richiederà nessun altro tipo di conferma

Nel momento in cui l'esigenza dovesse essere quella di gestire
l'iscrizione alla Newsletter con il double opt-in (richiedendo quindi
all'utente un ulteriore conferma prima di iscriverlo effettivamente al
servizio) sarà necessario gestire l'iscrizione al di fuori del form di
registrazione utilizzando uno dei moduli messi a disposizione
direttamente da ActiveCampaign (per maggiori informazioni relativamente
a come poter abilitare / disabilitare il double opt-in su di un modulo
ActiveCampaign si rimanda alla relativa documentazione di prodotto)

In considerazione di quanto appena detto e di quanto indicato anche
nella documentazione ufficiale di ActiveCampaign
(<https://www.activecampaign.com/learn/guides/preparing-for-the-gdpr-collecting-consent>),
per poter gestire l'iscrizione alla Newsletter all'interno del form di
registrazione utente in maniera GDPR compliance, il consiglio è quello
di:

- utilizzare appositi checkbox (realizzati con campi contatto custom di
  ActiveCampaign), ovviamente non preselezionati e che esprimano in
  maniera chiara quali informazioni l'utente può aspettarsi di ricevere
  una volta iscritto al servizio

- utilizzare un checkbox specifico (non preselezionato) per ogni tipo di
  consenso che si vuole raccogliere (consenso alla comunicazioni
  marketing via email, consenso all'invio di sms, consenso alle
  telefonate ...)

- includere nel form di registrazione utente, mediante il campo Privacy,
  un link ai termini di servizio e all'informativa privacy in uso sul
  sito e un checkbox che l'utente deve selezionare per poterli accettare
  in maniera esplicita

**ATTENZIONE!** Prima di adottare questo tipo di soluzione si consiglia
comunque di verificare sempre con chi di dovere (il proprio legale
piuttosto che il proprio DPO) l'effettiva adesione della soluzione
stessa alle normative GDPR in materia di Privacy e trattamento dei dati

Una volta completata la configurazione del componente, al salvataggio,
l'applicazione si preoccuperà di contattare ActiveCampaign, utilizzando
la relativa API Key inserita in fase di configurazione del sito (pagina
"*Sito -- Gestione Newsletter -- Email Marketing*"), **preleverà tutti i
campi Contatto Custom definiti sulla piattaforma terza e li inserirà,
assieme ai campi Contatto Standard anch'essi presenti su ActiveCampaign
(Nome, Cognome, Email ...), all'interno del form di Registrazione
Utente** (per maggiori informazioni relativamente a come creare e
gestire i campi Contatto Custom all'interno di ActiveCampaign si rimanda
alla relativa documentazione di prodotto)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_campi_contatto.bmp](./assets/media/image158.png)

A questo punto dovremo quindi decidere, tra tutti i campi importati da
ActiveCampaign, quali visualizzare all'interno del form di registrazione
nel momento in cui l'utente dovesse decidere di iscriversi al servizio,
quali nascondere e quali mappare con campi già presenti nello stesso
form di registrazione evitando così all'utente di inserire la stessa
informazione due volte.

In questo senso per nascondere uno dei campi importati da ActiveCampaign
e non visualizzarlo nel momento in cui l'utente dovesse decidere di
iscriversi alla Newsletter, sarà sufficiente aprire la sua maschera di
configurazione e deselezionare il parametro "**Pubblica**"

Per quel che riguarda invece la possibilità di mappare i campi importati
con altri campi già presenti nel form di registrazione sarà necessario,
anche in questo caso, aprire la maschera di configurazione del relativo
campo e agire sul parametro "**Tipo di dato da rilevare**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_mappa_campo_contatto.bmp](./assets/media/image159.png)

**ATTENZIONE!** Il parametro "**Tipo di dato da rilevare**" è
visualizzato tra i parametri di configurazione dei componenti interni al
form di iscrizione alla newsletter solo ed esclusivamente nel caso in
cui tale form sia inserito all'interno del componente di Registrazione
e/o di Profilo Utente.

**Tipo di dato da rilevare:** consente di decidere se il valore del
relativo campo di iscrizione alla Newsletter dovrà essere inserito
dall'utente o se dovrà essere prelevato automaticamente dal valore di un
altro campo del form di registrazione/profilo. E' possibile selezionare
uno dei seguenti valori:

- **Nessuno**: selezionando questa opzione il relativo campo del form di
  iscrizione alla newsletter verrà visualizzato e dovrà quindi essere
  compilato dall'utente nel momento in cui questo dovesse decidere di
  iscriversi anche alla Newsletter

- **Campo Cliente**: in queste condizioni il relativo campo del form di
  iscrizione alla newsletter non verrà mai visualizzato, per cui se
  l'utente dovesse decidere di iscriversi anche alla Newsletter
  l'informazione da inviare a ActiveCampaign, in relazione a questo
  specifico campo, verrà prelevata direttamente da quanto inserito
  dall'utente stesso all'interno di un altro campo del form di
  registrazione.

> Il successivo parametro **Campo di Origine** consente di indicare lo
> specifico Campo Cliente da cui dover prelevare questa informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_mappa_campo_contatto_2.bmp](./assets/media/image160.png)

- **Attributo Cliente**: come nel caso precedente, anche in queste
  condizioni il relativo campo del form di iscrizione alla newsletter
  non verrà mai visualizzato e l'informazione da inviare a
  ActiveCampaign verrà quindi prelevata direttamente da quanto inserito
  dall'utente stesso all'interno di un altro campo del form di
  registrazione

> Il successivo parametro **Attributo di Origine** consente di indicare
> lo specifico Attributo Utente da cui dover prelevare questa
> informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_mappa_campo_contatto_3.bmp](./assets/media/image161.png)

**ATTENZIONE!** La mail di registrazione inviata all'utente a seguito
della conferma di registrazione al sito conterrà anche i campi relativi
a ActiveCampaign solo nel caso in cui l'utente abbia effettivamente
deciso di iscriversi alla Newsletter.

Sul front end del sito, il funzionamento sarà analogo a quanto già visto
per le altre piattaforme.

Anche in questo caso dunque, all'interno del form di registrazione verrà
visualizzato **un Radio Button con le due opzioni Si, No mediante il
quale l'utente potrà decidere se iscriversi o meno anche alla
Newsletter**

![Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image149.png)

Nel caso in cui l'utente dovesse decidere di registrarsi al sito senza
iscriversi alla Newsletter (opzione **No**) non verrà visualizzato
nessuno dei campi importati da ActiveCampaign e, ovviamente, non verrà
inviata alla piattaforma terza nessun tipo di informazione.

**ATTENZIONE!** l'anagrafica dell'utente potrebbe comunque essere già
presente su ActiveCampaign (senza però alcun tipo di consenso marketing)
perché è stata abilitata, in relazione ad ActiveCampaign, la gestione
degli ordini e dei carrelli abbandonati e l'utente ha effettivamente
creato sul sito un Carrello Abbandonato o ha completato un ordine

Nel momento in cui l'utente dovesse invece decidere di iscriversi anche
alla Newsletter (opzione **Si**) verranno visualizzati **i campi
importati da ActiveCampaign** che si è deciso, in fase di
configurazione, di voler effettivamente visualizzare.

![Videate\\newsletter_registrazione3.bmp](./assets/media/image162.png)

In queste condizioni, una volta completata la registrazione al sito
verrà creata, ovviamente la relativa anagrafica Passweb e,
contestualmente, verranno inviati ad ActiveCampaign i dati necessari per
creare anche qui (o eventualmente aggiornare, ricordando che il campo
chiave è chiaramente il campo Email) la relativa anagrafica utente.

