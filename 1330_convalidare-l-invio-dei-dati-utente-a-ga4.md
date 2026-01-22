# CONVALIDARE L' INVIO DEI DATI UTENTE A GA4



I dati utente inviati a GA4 seguendo la procedura indicata nel
precedente capitolo di questo manuale potranno poi essere utilizzati da
Google Analytics per creare ad esempio delle audience di pubblico da
condividere con Google Ads oppure potranno anche essere inviati
direttamente a Google Ads nel momento in cui si dovesse decidere di
gestire, su questa piattaforma, le conversioni avanzate mediante
l'import dei dati necessari proprio da Google Analytics.

In ogni caso tali dati, per ragioni di privacy, saranno sempre dati
crittati, non decodificabili e non potranno mai essere visualizzati
utilizzando una qualche metrica o un qualche report disponibile su
Google Analytics.

In conseguenza di ciò, nel momento in cui l'esigenza dovesse essere
quella di verificare che i dati utente siano effettivamente inviati in
maniera corretta dal nostro sito a Google Analytics potremmo procedere
in due modi diversi: utilizzando gli Strumenti per Sviluppatori di
Chrome per analizzare il dettaglio delle chiamate effettuate dal browser
verso Google Analytics, oppure utilizzando Tag Assistant.

Vediamo più nel dettaglio come procedere in entrambi i casi.

**[STRUMENTI PER SVILUPPATORI DI CHROME]{.underline}**

In questo caso per verificare che i dati utente vengano inviati
correttamente a Google Analytics dovremo:

- Aprire gli strumenti per sviluppatori di Chrome (tasto funzione F12) e
  accedere alla sezione **Network** (o Rete dipendentemente da quella
  che è la lingua di utilizzo del browser)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_1.bmp](./assets/media/image27.png)

> dove potremo esaminare il dettaglio di tutte le chiamate effettuate
> dal browser.

- Una volta effettuato l'accesso a questa sezione degli Strumenti per
  Sviluppatori dovremo cliccare sul piccolo segnale di divieto posto in
  alto a sinistra nella barra degli strumenti in maniera tale da
  eliminare lo storico di eventuali precedenti chiamate e dovremo anche
  verificare di aver selezionato l'opzione All presente sempre nella
  barra degli strumenti di questa sezione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_2.bmp](./assets/media/image28.png)

- A questo punto, dopo aver verificato ovviamente di aver prestato tutti
  i consensi necessari per consentire di attivare il sistema di
  tracciamento, sarà sufficiente ricaricare la pagina web per vedere la
  scheda Network popolarsi con tutte le chiamate effettuate dal nostro
  browser per costruire la pagina web e per gestire anche eventuali
  interazioni e scambio di dati con strumenti di terze parti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_3.bmp](./assets/media/image29.png)

- Tra tutte le chiamate effettuate dal browser dovremo ora isolare
  quelle effettuate verso Google Analytics e per far questo sarà
  sufficiente inserire nel pannello di ricerca presente nella barra
  degli strumenti di questa sezione la stringa "collect" (le chiamate
  effettuate verso google analytics hanno infatti un endpoint di
  destinazione del tipo https://www.google-analytics.com/g/collect\....)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_4.bmp](./assets/media/image30.png)

- Una volta isolate le chiamate effettuate dal browser verso Google
  Analytics potremo esaminarne il dettaglio semplicemente cliccandoci
  sopra e portandoci poi nella scheda "Payload" cliccando sull'apposito
  pulsante presente nella parte destra della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_5.bmp](./assets/media/image31.png)

- Arrivati a questo punto per verificare che i dati utente siano stati
  inviati correttamente a Google Analytics dovremo semplicemente
  cercare, tra quelli presenti all'interno della scheda Payload
  evidenziata in figura, il **parametro em che è per l'appunto quello
  deputato alla gestione dei dati utente.** La presenza e il valore di
  questo parametro ci dirà dunque se, nell'ambito della chiamata
  esaminata, i dati utente sono stati inviati o meno a Google Analytics
  e, in caso positivo se tale invio ha presentato o meno degli errori

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_6.bmp](./assets/media/image32.png)

> Nello specifico:

- **Se il parametro em manca** completamente, significa che i dati
  utente, necessari per la gestione delle conversioni avanzate, non sono
  stati inviati.

- **Se è presente il parametro em**, ma è simile a "**tv.1\~em.**",
  significa che il parametro delle conversioni avanzate viene inviato,
  ma è vuoto e quindi, anche in questo caso, che i dati utente non sono
  stati inviati

- **Se è presente il parametro em**, ma è simile a "**tv.1\~em.e1**",
  significa che il parametro delle conversioni avanzate è stato inviato
  correttamente, ma si è verificato un problema nei dati inviati.

- **Se il parametro em è presente** ed è simile a **"tv.1\~em." seguito
  da una lunga stringa di caratteri** (come nel caso evidenziato in
  figura), significa che il parametro delle conversioni avanzate è stato
  inviato senza errori e la lunga stringa di caratteri rappresenta
  proprio il valore dei dati utente hashati passato dal browser a Google
  Analytics

**[TAG ASSISTANT]{.underline}**

Un altro modo, forse più semplice, per verificare il corretto invio a
Google Analytics dei dati utente è quello di utilizzare Tag Assistant
andando quindi a debuggare il nostro sistema di tracciamento.

Per far questo sarà necessario:

- Accedere alla proprietà di Google Analytics collegata al sito,
  portarsi nella sezione "Admin" e cliccare sulla voce "Data streams"
  presente all'interno del riquadro "Data collection and modification"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_7.bmp](./assets/media/image33.png)

- Dovremo quindi entrare nel dettaglio del Data Stream utilizzato per il
  sito (semplicemente cliccandoci sopra)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_8.bmp](./assets/media/image34.png)

> accedere poi alla sezione "**Configure tag settings**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_9.bmp](./assets/media/image35.png)

> e da qui una volta entrati nella sezione "**Admin**" cliccare sul
> pulsante "**Launch Tag Assistant**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_10.bmp](./assets/media/image36.png)

- In questo modo verrà aperto lo strumento disponibile su Google
  Analytics per poter effettuare il debug del proprio sistema di
  tracciamento. Dovremo quindi digitare l'url del nostro sito e cliccare
  sul pulsante "**Connect**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_11.bmp](./assets/media/image37.png)

- Su di un nuovo tab del browser verrà quindi aperto il nostro sito
  mentre nel tab attuale avremo la possibilità di vedere ed esaminare
  nel dettaglio tutti i tag e gli hit inviati dal browser a Google
  Analytics

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_12.bmp](./assets/media/image38.png)

- Dovremo quindi cliccare sul Tag corrispondente ad uno degli eventi
  tracciati sul sito (es. quello relativo all'evento di View Item List
  evidenziato in figura)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_13.bmp](./assets/media/image39.png)

> in maniera tale da accedere al dettaglio del relativo hit inviato dal
> sito a Google Analytics

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_14.bmp](./assets/media/image40.png)

- A questo punto potremo, per semplicità, cliccare sulle due piccole
  parentesi graffe poste in alto a destra nella tabella contenente tutti
  i parametri della hit inviata a Google Analytics

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_15.bmp](./assets/media/image41.png)

> e, come nel caso precedente, potremo a questo punto andare a ricercare
> tra tutti i parametri presenti in questa maschera di dettaglio il
> parametro em che sappiamo essere quello deputato alla gestione dei
> dati utente

- Se tutto è andato nella maniera corretta dovremo quindi trovare questo
  parametro e potremo vedere anche il dettaglio di ogni singolo dato
  utente che è stato passato a Google Analytics con la chiamata in
  oggetto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\verifica_upd_16.bmp](./assets/media/image42.png)

> Alcuni di questi dati potranno essere visualizzati in chiaro (es.
> City, Postal Code, Country ...) perché non essendo dati sensibili
> Google non richiede di hasharli, altri invece come la mail, il numero
> di telefono o il nome non saranno ovviamente in chiaro ma il fatto di
> vedere come valore una lunga stringa di caratteri ci dice già che il
> dato è presente ed è stato correttamente hashato e quindi che tutto è
> andato in maniera corretta.
>
> Diversamente se il parametro em non fosse presente o se alcuni dei
> campi da esso gestiti fossero vuoti ci sarebbe qualcosa da rivedere
> nell'implementazione del nostro sistema di tracciamento
