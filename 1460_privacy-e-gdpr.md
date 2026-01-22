# PRIVACY E GDPR



Come indicato nei precedenti capitoli di questo manuale WA Smart
Business è a tutti gli effetti una piattaforma Marketing che, volendo,
potrebbe anche essere assimilata alle più comuni piattaforme di
Newsletter.

Come MailChimp o ActiveCampaign infatti, anche WA Smart Business (pur
utilizzando un canale differente che è appunto quello di Whatsapp)
consente di inviare da una parte campagne marketing per la promozione
dei prodotti presenti all'interno del proprio sito Ecommerce e
dall'altra parte i cosiddetti messaggi di servizio (o utility) per
informare l'utente relativamente ad un cambio di stato del proprio
ordine, per ricordargli un carrello abbandonato ...

In ogni caso, indipendentemente dalla tipologia di messaggio inviato, si
tratta pur sempre dell'integrazione con una piattaforma terza con cui
verranno scambiati dei dati (nello specifico, ad esempio, il numero di
cellulare degli utenti) per cui il tutto dovrà essere implementato
sempre in maniera conforme a quanto richiesto dal GDPR.

Sarà quindi necessario, da una parte verificare di aver inserito
all'interno del sito un'informativa adeguata circa l'utilizzo della
piattaforma in esame e dei dati che con essa vengono raccolti e,
dall'altra parte, occorrerà verificare di aver gestito in maniera
corretta eventuali richieste di consenso preventivo necessarie per
l'invio di campagne di marketing.

**ATTENZIONE! in ogni caso Passepartout non è in alcun modo responsabile
in merito all'utilizzo, in maniera conforme a quanto previsto dal GDPR,
di strumenti di terze parti come può essere WA Smart Business, per cui
il consiglio è sempre quello di verificare direttamente con il relativo
supporto piuttosto che con il proprio DPO se la soluzione che si è
scelto di adottare è o meno conforme a quanto richiesto dalla
normativa**

Relativamente al tema della gestione dei consensi occorre poi fare
alcune considerazioni di fondamentale importanza legate proprio alla
diversa tipologia di messaggi che potranno essere inviati con questa
piattaforma utilizzando o meno l'integrazione con Passweb.

I messaggi di carattere commerciale (es. promozione prodotti) dovranno
infatti essere gestiti direttamente dal back end di WA Smart Business e,
prima di poterli inviare, sarà necessario raccogliere il consenso
preventivo da parte dei singoli utenti.

**Tale consenso dovrà essere raccolto utilizzando gli strumenti messi a
disposizione dalla piattaforma terza e verrà registrato direttamente su
WA Smart Business**.

In questo senso si potrebbe pensare, ad esempio, di utilizzare il
classico QR Code o un pulsante Whatsapp da inserire all'interno di
un'apposita pagina del sito

![](./assets/media/image18.png)

Scansionano il QR Code o cliccando sul pulsante, l'utente potrà avviare
la comunicazione con l'azienda e ricevere automaticamente un primo
messaggio di benvenuto all'interno del quale potrebbero già essere
inseriti, oltre ai link all'informativa del caso, anche i pulsanti per
la richiesta del consenso marketing.

Gli stessi pulsanti potrebbero essere inseriti anche all'interno dei
messaggi di servizio, il QR Code potrebbe essere spedito via mail a
tutti gli utenti iscritti al servizio di newsletter, potrebbe essere
stampato e mostrato direttamente alla cassa in negozio ....

**ATTENZIONE!** per maggiori informazioni sulle diverse modalità e
possibilità di raccolta del consenso preventivo per l'invio di
comunicazioni marketing e sui diversi strumenti messi a disposizione, in
questo senso dalla piattaforma terza (QR Code, Pulsanti, Messaggi di
benvenuto ...), si consiglia di fare riferimento sempre alla relativa
documentazione di prodotto

I messaggi relativi al cambio di stato di un ordine, alla notifica di un
carrello abbandonato, alla notifica dell'inserimento di un'attività in
agenda, di un nuovo documento in area riservata ... possono invece
essere considerati effettivamente come messaggi di utility (a patto
chiaramente di non inserire al loro interno delle informazioni di
carattere marketing, come da esempio il codice di una promo).

**L'invio di questi messaggi sarà gestito direttamente da Passweb e,
oltre ad avere un costo differente rispetto ai messaggi marketing, non
sarà soggetto alla richiesta di alcun tipo di consenso**.

Ciò significa dunque che l'utente potrà ricevere su Whatsapp, ad
esempio, la notifica di spedizione del suo ordine senza dover rilasciare
nessun consenso preventivo. L' unico vincolo in questo senso, oltre
ovviamente al fatto di aver inserito in fase di registrazione al sito il
proprio numero di cellulare, sarà la presa visione delle informative
pubblicate sul sito stesso e l'accettazione dei termini e delle
condizioni di servizio (cosa questa di per sé già obbligatoria in fase
di checkout)

In ogni caso, anche in queste condizioni, il consiglio è comunque quello
di gestire sul sito un'opzione di Opt-Out che, se esercitata, metta
l'utente nelle condizioni di non ricevere più neppure i messaggi di
servizio.

Per poter implementare questa opzione sarà sufficiente inserire nei form
di Registrazione e Profilo Utente un componente "**Campo Checkbox**"
mappato sul Campo Cliente "**Opt Out Whatsapp**" come in figura

![](./assets/media/image19.png)

![](./assets/media/image20.png)

In questo modo gli utenti che non avranno esercitato questa specifica
opzione, continueranno a ricevere su Whatsapp i messaggi di servizio.
Una volta esercitata l'opzione invece, l'utente non riceverà più nessun
tipo di comunicazione Whatsapp (per lo meno quelle inviate in automatico
dall'applicativo).

Ovviamente sarà cura dell'amministratore del sito, accertarsi del fatto
che questi utenti siano stati eliminati anche da eventuali liste di
campagne marketing gestite direttamente dalla piattaforma di WA Smart
Business
