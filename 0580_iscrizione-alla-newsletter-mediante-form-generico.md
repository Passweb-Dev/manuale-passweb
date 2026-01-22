# ISCRIZIONE ALLA NEWSLETTER MEDIANTE FORM GENERICO



Nel caso in cui l'esigenza dovesse essere quella di consentire agli
utenti del sito di gestire l'iscrizione alla newsletter all'interno di
un Form generico sarà necessario utilizzare il componente
"**Newsletter**" inserendolo all'interno del Componente di primo livello
**Form** e impostando, in fase di configurazione, il campo "**Tipo di
Integrazione**" sul valore "**MailChimp**", "**ActiveCampaign**" o
"**Brainlead**" a seconda della piattaforma utilizzata.

In queste condizioni configurazione, gestione e funzionamento del
componente sono del tutto analoghi a quanto descritto all'interno del
precedente capitolo "Iscrizione alla Newsletter MailChimp / Brainlead /
ActiveCampaign in fase di registrazione al sito".

Le uniche differenze saranno relative al fatto che non si farà più
riferimento, ovviamente, al form di registrazione al sito, ma allo
specifico form preso in considerazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione_form_generico2_res.bmp](./assets/media/image166.png)

Anche in questo caso poi potrebbero verificarsi situazioni in cui alcuni
dei dati necessari per l'iscrizione alla Newsletter siano già stati
inseriti dall'utente in analoghi campi del form (es. indirizzo mail).

Per non costringere l'utente ad inserire le stesse informazioni due
volte sarà quindi necessario, come nei casi precedenti, **mappare i
campi del form di iscrizione alla Newsletter con altri campi già
presenti all'interno dello stesso form Passweb.**

Nel caso specifico, per poter effettuare questo tipo di operazione è
necessario:

- Assegnare uno specifico valore al parametro "**Id/Name**" presente
  nella maschera di configurazione dello specifico controllo del form
  Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione_form_generico4_res.bmp](./assets/media/image167.png)

- Impostare il parametro "**Tipo di dato da rilevare**" presente nella
  maschera di configurazione del campo interno al form di iscrizione
  alla Newsletter sul valore "**Campo Form**" e valorizzare il
  successivo parametro "**Campo di Origine Id/Name**" con lo stesso dato
  indicato al punto precedente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione_form_generico5_res.bmp](./assets/media/image168.png)

Nel caso in cui il parametro "**Tipo di dato da rilevare**" dovesse
essere invece impostato sull'opzione "Nessuno" il corrispondente campo
verrà sempre visualizzato all'interno del form Passweb e dovrà quindi
essere compilato dall'utente nel momento in cui questo dovesse decidere
di iscriversi alla Newsletter

**ATTENZIONE!** Nel caso in cui si sia deciso di utilizzare BrainLead
come sistema di gestione delle Newsletter e il componente "Form"
generico di Passweb per gestire il form di iscrizione al servizio, gli
unici dati passati a BrainLead al momento dell'iscrizione, potranno
essere soltanto l'indirizzo mail ed eventuali campi custom.

Per tale ragione, nel momento in cui si dovesse decidere di utilizzare
BrainLead, è sempre consigliabile gestire il processo di iscrizione alla
Newsletter contestualmente a quello di registrazione al sito.

