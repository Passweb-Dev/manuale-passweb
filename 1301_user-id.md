# USER-ID



GA4 può identificare i visitatori del sito in tre modi differenti. Nello
specifico gli utenti del sito possono essere identificati mediante:

- **Client ID** (Device): questo tipo di identificazione fa uso,
  essenzialmente, di "1st party cookie" (cookie di prima parte). Se un
  visitatore svuota i cookie del proprio browser o naviga il sito
  utilizzando un browser o un dispositivo differente, questo verrà
  considerato come un nuovo dispositivo e quindi anche la visita verrà
  conteggiata a tutti gli effetti come quella di un nuovo visitatore

- **Google Signals:** questo tipo di identificazione riconosce gli
  utenti in base al fatto che abbiano o meno effettuato l'accesso al
  loro Account Google e in base al fatto che abbiano o meno acconsentito
  alla condivisione dei dati a fini pubblicitari.

> **ATTENZIONE!** Google Signals è lo strumento che Google utilizza per
> personalizzare gli annunci pubblicitari quindi è a tutti gli effetti
> uno strumento di identificazione e profilazione degli utenti. Non è
> attivo a default sulle proprietà GA4 e nel momento in cui si dovesse
> decidere di attivarlo occorre accertarsi di aver correttamente
> informato gli utenti nell'informativa di gestione dei cookie e della
> privacy, di rispettare tutte le norme previste dal GDPR e di
> richiedere quindi agli utenti del sito tutti i consensi del caso

- **User ID:** questo metodo di identificazione consente di associare i
  visitatori del sito ad un identificatore univoco che deve essere
  assegnato agli utenti stessi direttamente dall'applicativo,
  tipicamente, mediante il processo di login. E' sicuramente il metodo
  di identificazione più accurato dei tre inquanto consente di
  riconoscere l'utente in maniera cross device e cross platform (posto
  ovviamente che abbia effettuato l'accesso al sito e che il sistema gli
  associ effettivamente sempre lo stesso identificativo).

Relativamente all'utilizzo o meno dello User ID vanno fatte poi altre
considerazioni di fondamentale importanza.

- Come dovrebbe essere chiaro l'utilizzo di questo metodo di
  identificazione ci consente indubbiamente di ottenere dati più precisi
  e soprattutto di capire meglio quello che è il comportamento globale
  (su vari dispositivi) di uno stesso utente. Nel momento in cui si
  dovesse decidere di attivare e gestire lo User Id, proprio per il
  principio su cui si basa, occorre anche considerare che si potrebbe
  verificare una diminuzione nel conteggio del numero di visite perché
  quelle che prima erano considerate come visite di nuovi utenti (perché
  provenienti ad esempio da dispositivi differenti) ora potrebbero
  essere effettivamente considerate come visite dello stesso utente.

- E' necessario avere sempre ben presente che i termini e le condizioni
  di servizio di Google Analytics non consentono il monitoraggio di
  informazioni di identificazione personale (PII) come possono essere ad
  esempio l'indirizzo mail, il codice fiscale ... e lo stesso principio
  vale anche per lo User ID.

> **ATTENZIONE!** attivando il tracciamento mediante User ID si ha anche
> la responsabilità di garantire che l\'utilizzo dell' ID utente sia
> conforme ai Termini di servizio di Google Analytics. Non vanno quindi
> utilizzate informazioni che consentono l'identificazione personale e,
> allo stesso modo, sarà necessario, da una parte, fornire nelle Norme
> sulla gestione della privacy del proprio sito un'informativa adeguata
> circa l'utilizzo degli identificatori e, dall'altra parte, verificare
> di aver gestito in maniera adeguata la richiesta di consenso
> preventivo per il tracciamento.
>
> In ogni caso **Lo User ID non deve contenere in alcun modo
> informazioni che una terza parte potrebbe utilizzare per determinare
> l'identità di un utente**.

- Lo User ID non viene applicato ai dati storici che esulano dall'ambito
  della stessa sessione. Quando un nuovo visitatore atterra sul sito GA4
  memorizza un cookie con un ID generato casualmente (questo è il Client
  ID e NON lo User ID). Se dopo diverse sessioni lo stesso utente decide
  di registrarsi, e gli viene quindi assegnato uno specifico User ID
  questo non verrà applicato automaticamente anche ai dati di tutte le
  sessioni precedenti. Se invece l'utente decide di registrarsi
  nell'ambito della stessa sessione di navigazione allora lo User ID
  verrà attribuito anche a tutti gli eventi che si sono verificati
  (sempre nell'ambito della stessa sessione) prima dell'assegnazione
  dello User ID.

- Lo User ID non può essere unito tra diverse proprietà

- Nel momento in cui si dovesse decidere di attivare il tracciamento
  mediante User ID questo andrà poi passato a GA4 come parametro
  aggiuntivo dello specifico evento che si intende tracciare, oppure
  come parametro aggiuntivo del tag di configurazione e, in quest'ultimo
  caso verrà automaticamente associato anche a tutti gli eventi gestiti.

Fatte queste importanti considerazioni va ora detto che per attivare il
monitoraggio mediante User ID è necessario verificare alcune
configurazioni sia lato Passweb che lato GA4. Nello specifico:

- Lato Passweb è possibile decidere di attivare o meno il tracciamento
  mediante User ID attraverso l'apposito flag "**Utilizza User ID**"
  presente alla pagina "**Sito -- Preferenze**" del Wizard (tab
  "**Tracciamento Dati**") dopo aver selezionato come metodo di
  tracciamento **Google Analytics 4**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_58.bmp](./assets/media/image4.png)

> In questo senso è anche bene sottolineare che, come richiesto da
> Google, una volta attivato il parametro in questione:

- lo User ID inviato ad Analytics coinciderà esattamente con l'Id utente
  in uso al sito Passweb e sarà quindi un semplice codice numerico che
  non consente a strumenti di terze parti di risalire all'effettiva
  identità dell'utente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_59.bmp](./assets/media/image5.png)

- lo User ID verrà impostato a livello di tag di configurazione e verrà
  quindi inviato assieme a tutti gli eventi gestiti dal proprio sito
  Passweb

<!-- -->

- Lato GA4 la raccolta dei dati mediante User ID dipende invece dal
  metodo utilizzato da Analytics stesso per associare gli eventi agli
  utenti, metodo questo che può essere impostato all'interno della
  sezione "**Data Display -- Reporting Identity**" presente
  nell'interfaccia di amministrazione della relativa proprietà GA4

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_60.bmp](./assets/media/image6.png)

**ATTENZIONE!** GA4 imposta a default l'Identificazione nei report
sull'opzione "**Blended**" il che significa che verranno valutati,
nell'ordine, i seguenti metodi di identificazione degli utenti: prima di
tutto lo User ID poi i Google Signals, l'ID Dispositivo (Client ID) e
infine i Modelli automatici

In queste condizioni dunque, nel momento in cui lo User ID dovesse
essere effettivamente disponibile questo verrà utilizzato come metodo di
identificazione degli utenti per tutti i rapporti di GA4. Se non
presente verranno invece utilizzati i Google Signals e a seguire Client
ID e Modelli Automatici

**In considerazione di ciò** **prima di attivare, lato Passweb, il
tracciamento mediante User ID è necessario accertarsi bene di gestire in
maniera corretta la richiesta agli utenti di tutti i consensi necessari,
di aver sistemato in maniera adeguata l'informativa privacy in uso sul
sito e, in generale, di soddisfare tutto quanto richiesto dal GDPR in
merito di trattamento dei dati**

Di seguito alcuni indirizzi dove poter trovare documentazione ufficiale
di Google relativamente all'utilizzo dello User-ID

<https://support.google.com/analytics/answer/9213390?hl=it>

<https://support.google.com/analytics/answer/10976610?hl=it&ref_topic=9303474>

<https://support.google.com/analytics/answer/6366371?hl=it>

