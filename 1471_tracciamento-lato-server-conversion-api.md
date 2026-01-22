# TRACCIAMENTO LATO SERVER -- CONVERSION API



La modalità di tracciamento lato server è stata introdotta (e di fatto
resa obbligatoria) da Facebook parallelamente all'uscita di iOS 14.5.

A partire da questa versione del suo sistema operativo Apple ha infatti
modificato in maniera sostanziale la modalità di acquisizione dei dati
degli utenti rendendo obbligatoria, per tutte le App, la richiesta
esplicita, agli utenti, del consenso per raccoglierne e condividerne i
dati.

In queste condizioni solo se, e dopo che l'utente acconsente al
tracciamento dei dati sarà effettivamente possibile raggiungerlo a fini
pubblicitari sul suo dispositivo.

In conseguenza di ciò, da una parte Facebook si è visto costretto a
modificare il suo sistema di tracciamento sia lato web che lato app in
maniera tale da limitare, per quanto possibile, eventuali perdite nella
capacità di tracciamento.

Dall'altra parte chi vorrà utilizzare il sistema di tracciamento e di
advertising messo a disposizione dal social network dovrà
essenzialmente:

- impostare la **Conversion API** in maniera tale da attivare
  correttamente il sistema di tracciamento lato server

- impostare **gli eventi aggregati** per continuare a tracciare e
  ottimizzare le campagne per gli eventi di conversione più importanti.
  In questo senso occorre sottolineare che:

  - possono essere impostati un **massimo di 8 eventi per dominio**

  - inizialmente questi eventi possono essere preassegnati direttamente
    da Facebook secondo l'ordine che ritiene più rilevante e sulla base
    della spesa pubblicitaria più recente prodotta da tutti gli account
    pubblicitari che pubblicano inserzioni sul dominio in esame

  - gli eventi aggregati possono comunque essere modificati in un
    qualsiasi momento operando direttamente dal Business Manager di
    Facebook

Nello specifico poi per quel che riguarda la Conversion API occorre
sottolineare che:

- **è un sistema di tracciamento lato Server**, si tratta quindi di uno
  strumento che permette di condividere direttamente dai server del sito
  a quelli di Facebook (mediante un apposito token di accesso) le azioni
  dei clienti e i principali eventi web

- **è uno strumento complementare al Facebook Pixel (e quindi al
  tracciamento lato client).**

> Ciò significa che, volendo, sarà possibile (ma non obbligatorio)
> utilizzare assieme questi due strumenti (Pixel e Conversion API).
>
> **ATTENZIONE!** Nel momento in cui si dovesse decidere di utilizzare
> contemporaneamente sia il tracciamento lato server (Conversion API)
> che quello lato client (Pixel) sarà poi necessario affidarsi al
> sistema di deduplica degli eventi di Facebook in maniera tale da non
> avere lo stesso evento tracciato due volte

- per poter essere implementata all'interno del proprio sito dovranno
  essere soddisfatti **determinati prerequisiti**. Nello specifico, ad
  esempio sarà necessario:

  - disporre di un Account Business Manager

  - implementare correttamente sul proprio sito anche il Pixel di
    Facebook

  - generare uno specifico Access Token

  - verificare, sempre tramite Business Manager, il dominio del proprio
    sito

  - ...

In questo tipo di tracciamento non dovrà essere inserito nessun codice
javascript all'interno del sito ma ci si dovrà preoccupare solamente di
configurare in maniera corretta l'applicazione.

Di seguito viene quindi descritta la procedura necessaria per attivare
correttamente, all'interno del proprio sito Passweb, il tracciamento di
Facebook mediante Conversion API.

- Accedere al proprio Account **Business Manager**, aprire il menu
  "**Tutti gli Strumenti**" e selezionare la voce "**Gestione Eventi**"

![Videate\\facebook_tracciamento_client_1.bmp](./assets/media/image1.png)

> **ATTENZIONE!** l'Accesso Token necessario per attivare le Conversion
> API, così come il Pixel di Facebook, può essere generato unicamente
> all'interno del Business Manager di Facebook. Il fatto dunque di
> disporre di un proprio Business Manager è un prerequisito
> indispensabile per attivare sia il tracciamento lato client che quello
> lato server
>
> Per maggiori informazioni relativamente a come attivare un proprio
> Business Manager creando il relativo account si consiglia di fare
> riferimento alla documentazione ufficiale presente sui siti di
> Facebook

- Una volta effettuato l'accesso alla sezione "Gestione Eventi" cliccare
  sul pulsante verde raffigurante un piccolo + (**Collega origini dei
  dati**)

![Videate\\facebook_tracciamento_client_2.bmp](./assets/media/image2.png)

> Selezionare quindi l' opzione "**Web**" e cliccare sul pulsante
> "**Collega**"

![Videate\\tracking-facebook-3.bmp](./assets/media/image9.png)

> Successivamente selezionare l'opzione "**API Conversion**" e cliccare
> ancora una volta sul pulsante "**Collega**"

![Videate\\tracking-facebook-4.bmp](./assets/media/image10.png)

- Nella successiva maschera assegnare un nome al Pixel (campo "**Assegna
  un nome al tuo pixel**") e cliccare poi sul pulsante "**Continua**"

![Videate\\tracking-facebook-5.bmp](./assets/media/image11.png)

- A questo punto si apriranno una serie di pop up di presentazione della
  Conversion API. Saltarli tutti (pulsante "**Avanti**") fino ad
  arrivare alla maschera "**Collega l'attività del sito web usando l'API
  Conversions**" di seguito evidenziata

![Videate\\tracking-facebook-6.bmp](./assets/media/image12.png)

> Cliccare quindi sul pulsante "**Installa codice manualmente**"

- Nella schermata successiva cliccare sul pulsante "**Continua**"

![](./assets/media/image13.png)

> in maniera tale da accedere alla maschera di "**Selezione eventi**"
> all'interno della quale poter selezionare gli eventi aggregati che
> dovranno poi essere tracciati mediante Conversion API.
>
> **ATTENZIONE!** si ricorda che, come precedentemente evidenziato e
> come indicato anche dalla documentazione ufficiale di Facebook, sarà
> poi possibile attivare **massimo di 8 eventi per dominio**

- A questo punto sarà quindi necessario selezionare tra quelli gestiti
  da Passweb 8 eventi (tra standard e custom) e indicare per ciascuno di
  essi le informazioni che verranno passate a Facebook (per maggiori
  informazioni relativamente agli eventi gestiti da Passweb si veda
  anche quanto indicato nel successivo capitolo "*Eventi e Parametri*"
  di questo manuale)

> Si potrebbe pensare, ad esempio, di selezionare tra gli eventi
> ecommerce consigliati l'evento di **Acquisto**, **Aggiunta al
> carrello, Visualizzazione dei contenuti, Aggiunta delle informazioni
> di pagamento**, **Aggiunta alla lista dei desideri, Inizio di
> acquisto** e **Ricerca** e l'evento aggiuntivo "**Acquisizione
> Contatto**" (Altra categoria aziendale)

![](./assets/media/image14.png)

![](./assets/media/image15.png)

> Cliccare quindi sul pulsante "**Continua**"

- A questo punto, come detto, sarà necessario impostare, **per ciascuno
  degli eventi indicati**, le informazioni che verranno inviate a
  Facebook dal sito Passweb.

> Selezionare quindi, uno alla volta, lo specifico evento presente sulla
> sinistra della sezione "**Seleziona parametri**" e flaggare in
> corrispondenza della sotto sezione di destra i parametri dell'evento
> secondo lo schema di seguito indicato:

![Videate\\tracking-facebook-evento-pagamento.bmp](./assets/media/image16.png)

> **[AGGIUNTA DELLE INFORMAZIONI DI PAGAMENTO]{.underline}**
>
> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- Categoria del contenuto

- Valuta

- Valore

- Id dei contenuti

- Contenuti

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[AGGIUNTA AL CARRELLO]{.underline}**

![](./assets/media/image17.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- ID dei contenuti

- Categoria del contenuto

- Nome del contenuto

- Contenuti

- Valuta

- Valore

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[AGGIUNTA ALLA LISTA DEI DESIDERI]{.underline}**

![](./assets/media/image18.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- ID dei contenuti

- Categoria del contenuto

- Nome del contenuto

- Contenuti

- Valuta

- Valore

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[INIZIO DI ACQUISTO]{.underline}**

![](./assets/media/image19.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- Categoria del contenuto

- Nome del contenuto

- Numero di elementi

- Valuta

- Valore

- Id dei contenuti

- Contenuti

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[ACQUISIZIONE CONTATTO]{.underline}**

![](./assets/media/image20.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Categoria del contenuto

- Nome del contenuto

- Stato

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[ACQUISTO]{.underline}**

![](./assets/media/image21.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- Categoria del contenuto

- Nome del contenuto

- Numero di elementi

- Valuta

- Valore

- Id dei contenuti

- Contenuti

- ID dell'ordine

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[RICERCA]{.underline}**

![](./assets/media/image22.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Valore

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.
>
> **[VISUALIZZAZIONE DI CONTENUTI]{.underline}**

![](./assets/media/image23.png)

> **Parametri dei dettagli degli eventi**:

- ID dell'evento

- Tipo di contenuto

- Categoria del contenuto

- Nome del contenuto

- Valuta

- Valore

- Id dei contenuti

- Contenuti

> **Parametri delle informazioni dei clienti:**

- Indirizzo IP client

- Paese

- Agente utente client

- Città

- Email

- ID esterno

- Cookie dell'ID del click (fbc)

- Cookie dell'ID del browser (fbp)

- Nome

- Cognome

- Telefono

- Stato

> **ATTENZIONE!** alcuni dei parametri delle informazioni dei clienti
> sopra indicati verranno effettivamente inviati solo se disponibili.
> Nello specifico, ad esempio, Email, Nome, Cognome ecc... dell'utente
> che naviga il sito potranno essere eventualmente inviati solo dopo che
> l'utente stesso avrà effettuato l'autenticazione.

- Nella successiva maschera di controllo della configurazione cliccare
  sul pulsante "**Conferma la configurazione**" posto in basso a destra

![Videate\\tracking-facebook-10.bmp](./assets/media/image24.png)

> in maniera tale da accedere all'ultimo step della configurazione

- Una volta effettuato l'accesso alla maschera "Vedi le istruzioni"
  cliccare sul link "**Apri la guida all'implementazione**" evidenziato
  in figura

![Videate\\tracking-facebook-11.bmp](./assets/media/image25.png)

- Cliccare quindi su "**Inizia**"

![Videate\\tracking-facebook-12.bmp](./assets/media/image26.png)

> e successivamente su "**Genera un token di accesso**"

![Videate\\tracking-facebook-13.bmp](./assets/media/image27.png)

![Videate\\tracking-facebook-15.bmp](./assets/media/image28.png)

- Copiare il token appena generato e incollarlo in corrispondenza del
  parametro "**Access Token**" presente all'interno della sezione
  "**Facebook Pixel -- Conversion API**" della pagina "**Sito --
  Preferenze**" (tab **"Tracciamento Dati**") del Wizard

![](./assets/media/image29.png)

> **ATTENZIONE! come indicato sul Business Manager di Facebook il token
> generato al punto precedente non sarà memorizzato su Facebook per cui
> una volta creato è consigliabile copiarlo e salvarlo anche in un luogo
> sicuro cui poter accedere in caso di bisogno**

- Una volta generato e copiato il token di accesso scorrere in fondo
  alla pagina e cliccare sul pulsante "**Fine**"

![Videate\\tracking-facebook-16.bmp](./assets/media/image30.png)

- A questo punto verremo ricondotti automaticamente alla Panoramica del
  Pixel di Facebook appena creato e identificato dal nome ad esso
  assegnato nei primi step del processo.

![Videate\\tracking-facebook-17.bmp](./assets/media/image31.png)

- Cliccare quindi sulla voce "**Impostazioni**" evidenziata in figura

![Videate\\tracking-facebook-18.bmp](./assets/media/image32.png)

- Copiare l'identificativo del pixel (campo **ID del pixel**)

![Videate\\tracking-facebook-19.bmp](./assets/media/image33.png)

> e inserirlo in corrispondenza del parametro "**Pixel ID**" presente
> all'interno della sezione "**Facebook Pixel -- Conversion API**" della
> pagina "**Sito -- Preferenze**" (tab **"Tracciamento Dati**") del
> Wizard

![Videate\\facebook_tracciamento_client_6.bmp](./assets/media/image34.png)

Arrivati a questo punto avremo completato la configurazione e
l'attivazione delle Conversion API e potremo quindi testare il corretto
funzionamento del tracciamento lato Server. In questo senso ci tornerà
particolarmente utile il campo "**Codice di Test**" all'interno del
quale poter inserire il "**test_event_code**" prelevabile direttamente
dal Business Manager di Facebook e indispensabile per poter
effettivamente testare il corretto tracciamento degli eventi server (per
maggiori informazioni in merito si veda anche quanto indicato nel
successivo capitolo "*Verifica del tracciamento*" di questo manuale)

Infine per quel che riguarda il parametro "**Abilita eventi custom**"
possiamo evidenziare che, come già per il tracciamento lato client,
anche in questo caso tale parametro consente, se selezionato, di
attivare il tracciamento dei seguenti eventi personalizzati: SelectItem,
ViewItemList, ViewCart, RemoveFromCart, AddShippingInfo

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
**attivare solamente il tracciamento lato Server** (Conversion API) sarà
sufficiente compilare correttamente (seguendo quanto precedentemente
descritto) i due campi "**Access Token**" e "**Pixel ID**"

Nel caso in cui si dovesse invece decidere di **utilizzare
contemporaneamente il tracciamento lato server e quello lato client,**
sarà necessario verificare di aver correttamente selezionato anche il
parametro "Tracciamento Client".

In queste condizioni inoltre, **sarà poi necessario affidarsi al sistema
di deduplica degli eventi di Facebook** in maniera tale da non avere lo
stesso evento tracciato due volte

In questo senso, coerentemente con quanto indicato nella documentazione
ufficiale di Facebook (
<https://www.facebook.com/business/help/823677331451951?id=1205376682832142>
), Passweb si preoccuperà di inviare, per ogni evento, il parametro
"**event**" del tracciamento client, uguale al parametro
"**event_name**" della Conversions API e il parametro "**eventID**"
(tracciamento client) uguale al parametro "**event_id**" (tracciamento
server).

Nello specifico, per i parametri "event" e "event_name" verrà utilizzato
un nome identificativo dell' evento da tracciare (Purchase, AddToCart,
AddPaymentInfo ...).

Per i parametri "eventID" e "event_id" verrà invece utilizzato un
identificativo univoco costituito dal nome dell'evento da tracciare più
un timestamp di ora, minuti e secondi in cui si è verificato l'evento
più un ulteriore codice univoco (es. "Purchase-20211124164437-779")

