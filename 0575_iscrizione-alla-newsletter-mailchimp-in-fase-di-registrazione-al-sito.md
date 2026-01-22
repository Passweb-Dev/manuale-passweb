# ISCRIZIONE ALLA NEWSLETTER MAILCHIMP IN FASE DI REGISTRAZIONE AL SITO



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui l'esigenza dovesse essere quella di consentire agli utenti del
sito di iscriversi alla newsletter direttamente in fase di registrazione
al sito, sarà necessario utilizzare il componente "**Newsletter
(MailChimp o BrainLead)**" inserendolo all'interno del Componente di
primo livello **Registrazione Utente** e impostando, in fase di
configurazione, il campo "**Tipo di Integrazione**" sul valore
"**MailChimp**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp.bmp](./assets/media/image150.png){width="5.097222222222222in"
height="3.071527777777778in"}

**ATTENZIONE! In queste condizioni il processo di iscrizione alla
Newsletter MailChimp è leggermente diverso rispetto a quanto potrebbe
verificarsi nel momento in cui l'iscrizione dovesse essere gestita con
un form specifico esterno al componente di Registrazione Utente**

A tal proposito è bene evidenziare per prima cosa che, come indicato
anche nei precedenti capitoli di questo manuale, per poter completare
l'iscrizione alla Newsletter MailChimp un utente dovrà, generalmente,
cliccare anche su di un apposito link di "Conferma Iscrizione" presente
all'interno di una mail inviata direttamente da MailChimp all'indirizzo
indicato dall'utente stesso in fase di iscrizione.

Solo a questo punto l'iscrizione sarà completa e l'utente potrà
effettivamente ricevere le Newsletter a lui dedicate.

**Nel momento in cui, invece, l'iscrizione al servizio dovesse avvenire
direttamente dal form di Registrazione / Profilo Utente, avendo anche
acconsentito espressamente al trattamento dei dati personali (gestito
mediante il campo Privacy), l'iscrizione alla Newsletter sarà immediata
e non richiederà nessun altro tipo di conferma da parte dell'utente.**

In sostanza dunque nel caso in cui l'esigenza dovesse essere quella di
iscrivere utenti alla newsletter senza che MailChimp invii loro un
ulteriore mail di Conferma Iscrizione, sarà necessario inserire
all'interno del Form di Registrazione / Profilo Utente anche un
componente "Campo Privacy".

**ATTENZIONE!** Prima di adottare questo tipo di soluzione si consiglia
comunque di verificare con chi di dovere l'effettiva adesione della
soluzione stessa alle nuove normative GDPR in materia di Privacy e
trattamento dei dati

**ATTENZIONE!** per ovvie ragioni, il parametro "**Invia Indirizzo**"
non sarà presente per componenti di iscrizione alla newsletter gestiti
esternamente al form di Registrazione e/o a quello di Profilo Utente

Una volta completata la configurazione del componente al salvataggio (in
maniera totalmente analoga a quello che avviene anche per il componente
"Iscrizione Newsletter") l'applicazione si preoccuperà di contattare
MailChimp, utilizzando la relativa API Key inserita in fase di
configurazione del sito, di prelevare il form di iscrizione impostato
sulla specifica piattaforma e di inserire i relativi campi all'interno
del form di Registrazione Utente.

In queste condizioni, oltre ai campi definiti sulla piattaforma terza,
verrà però visualizzato, come primo elemento del form di iscrizione alla
Newsletter, **un Radio Button con le due opzioni Si, No** **mediante il
quale l'utente potrà decidere se iscriversi o meno anche alla
Newsletter**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image151.png){width="5.604166666666667in"
height="3.4743055555555555in"}

Nel caso in cui l'utente dovesse decidere di registrarsi al sito senza
iscriversi alla Newsletter (opzione **No**) i campi del form di
iscrizione alla newsletter non verranno mai visualizzati.

Nel momento in cui l'utente dovesse invece decidere di iscriversi anche
alla Newsletter (opzione **Si**) verranno visualizzati a default tutti i
campi presenti nel relativo form di iscrizione definito su MailChimp.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione3.bmp](./assets/media/image152.png){width="5.604166666666667in"
height="3.4743055555555555in"}

In queste condizioni potrebbero anche verificarsi situazioni in cui
alcuni dei dati necessari per l'iscrizione alla Newsletter siano già
stati inseriti dall'utente in analoghi campi del form di registrazione
(es. indirizzo mail).

In conseguenza di ciò, **nel momento in cui non si volesse costringere
l'utente ad inserire le stesse informazioni due volte, sarà necessario
mappare i campi del form di iscrizione alla Newsletter con altri campi
già presenti all'interno del form di Registrazione Utente.**

Per poter effettuare questo tipo di operazione è necessario agire sul
parametro "**Tipo di dato da rilevare**" presente nella maschera di
configurazione dei campi interni al form di iscrizione alla Newsletter.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione4_res.bmp](./assets/media/image153.png){width="4.597222222222222in"
height="2.922222222222222in"}

**ATTENZIONE!** Il parametro "**Tipo di dato da rilevare**" è
visualizzato tra i parametri di configurazione dei campi interni al form
di iscrizione alla newsletter solo ed esclusivamente nel caso in cui
tale form sia inserito all'interno del componente di Registrazione e/o
di Profilo Utente.

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
  l'informazione da inviare a MailChimp, in relazione a questo specifico
  campo, verrà prelevata direttamente da quanto inserito dall'utente
  stesso all'interno di un altro campo del form di registrazione.

> Il successivo parametro **Campo di Origine** consente di indicare lo
> specifico Campo Cliente da cui dover prelevare questa informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione5_res.bmp](./assets/media/image154.png){width="4.597222222222222in"
height="2.922222222222222in"}

- **Attributo Cliente**: in queste condizioni il relativo campo del form
  di iscrizione alla newsletter non verrà mai visualizzato, per cui se
  l'utente dovesse decidere di iscriversi anche alla Newsletter
  l'informazione da inviare a MailChimp, in relazione a questo specifico
  campo, verrà prelevata direttamente da quanto inserito dall'utente
  stesso all'interno di un altro campo del form di registrazione

> Il successivo parametro **Attributo di Origine** consente di indicare
> lo specifico Attributo Utente da cui dover prelevare questa
> informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione6_res.bmp](./assets/media/image155.png){width="4.610416666666667in"
height="2.9347222222222222in"}

**ATTENZIONE!** La mail di registrazione inviata all'utente a seguito
della conferma di registrazione al sito conterrà anche i campi relativi
a MailChimp solo nel caso in cui l'utente abbia deciso di iscriversi
alla Newsletter.

