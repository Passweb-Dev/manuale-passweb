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

![Videate\\facebook_tracciamento_client_1.bmp](./assets/media/image1.png){width="5.2340277777777775in"
height="3.532638888888889in"}

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

![Videate\\facebook_tracciamento_client_2.bmp](./assets/media/image2.png){width="5.2340277777777775in"
height="3.532638888888889in"}

> Selezionare quindi l' opzione "**Web**" e cliccare sul pulsante
> "**Collega**"

![Videate\\tracking-facebook-3.bmp](./assets/media/image9.png){width="5.590972222222222in"
height="3.33125in"}

> Successivamente selezionare l'opzione "**API Conversion**" e cliccare
> ancora una volta sul pulsante "**Collega**"

![Videate\\tracking-facebook-4.bmp](./assets/media/image10.png){width="5.590972222222222in"
height="3.33125in"}

- Nella successiva maschera assegnare un nome al Pixel (campo "**Assegna
  un nome al tuo pixel**") e cliccare poi sul pulsante "**Continua**"

![Videate\\tracking-facebook-5.bmp](./assets/media/image11.png){width="5.590972222222222in"
height="3.33125in"}

- A questo punto si apriranno una serie di pop up di presentazione della
  Conversion API. Saltarli tutti (pulsante "**Avanti**") fino ad
  arrivare alla maschera "**Collega l'attività del sito web usando l'API
  Conversions**" di seguito evidenziata

![Videate\\tracking-facebook-6.bmp](./assets/media/image12.png){width="5.590972222222222in"
height="3.33125in"}

> Cliccare quindi sul pulsante "**Installa codice manualmente**"

- Nella schermata successiva cliccare sul pulsante "**Continua**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-7.bmp](./assets/media/image13.png){width="5.2340277777777775in"
height="3.532638888888889in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-8.bmp](./assets/media/image14.png){width="5.2340277777777775in"
height="3.532638888888889in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-8a.bmp](./assets/media/image15.png){width="5.2340277777777775in"
height="3.532638888888889in"}

> Cliccare quindi sul pulsante "**Continua**"

- A questo punto, come detto, sarà necessario impostare, **per ciascuno
  degli eventi indicati**, le informazioni che verranno inviate a
  Facebook dal sito Passweb.

> Selezionare quindi, uno alla volta, lo specifico evento presente sulla
> sinistra della sezione "**Seleziona parametri**" e flaggare in
> corrispondenza della sotto sezione di destra i parametri dell'evento
> secondo lo schema di seguito indicato:

![Videate\\tracking-facebook-evento-pagamento.bmp](./assets/media/image16.png){width="5.558333333333334in"
height="3.201388888888889in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-aggiunta_carrello.bmp](./assets/media/image17.png){width="5.66875in"
height="3.129861111111111in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-aggiunta_wish.bmp](./assets/media/image18.png){width="5.66875in"
height="3.123611111111111in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-inizio-acquisto.bmp](./assets/media/image19.png){width="5.675in"
height="3.1166666666666667in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-acquisizione-contatto.bmp](./assets/media/image20.png){width="5.675in"
height="3.1104166666666666in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-acquisto.bmp](./assets/media/image21.png){width="5.6819444444444445in"
height="3.1166666666666667in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-ricerca.bmp](./assets/media/image22.png){width="5.6819444444444445in"
height="3.1166666666666667in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-evento-visualizzazione-contenuti.bmp](./assets/media/image23.png){width="5.675in"
height="3.1166666666666667in"}

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

![Videate\\tracking-facebook-10.bmp](./assets/media/image24.png){width="5.590972222222222in"
height="3.33125in"}

> in maniera tale da accedere all'ultimo step della configurazione

- Una volta effettuato l'accesso alla maschera "Vedi le istruzioni"
  cliccare sul link "**Apri la guida all'implementazione**" evidenziato
  in figura

![Videate\\tracking-facebook-11.bmp](./assets/media/image25.png){width="5.590972222222222in"
height="3.33125in"}

- Cliccare quindi su "**Inizia**"

![Videate\\tracking-facebook-12.bmp](./assets/media/image26.png){width="5.590972222222222in"
height="3.33125in"}

> e successivamente su "**Genera un token di accesso**"

![Videate\\tracking-facebook-13.bmp](./assets/media/image27.png){width="5.590972222222222in"
height="3.33125in"}

![Videate\\tracking-facebook-15.bmp](./assets/media/image28.png){width="5.590972222222222in"
height="3.33125in"}

- Copiare il token appena generato e incollarlo in corrispondenza del
  parametro "**Access Token**" presente all'interno della sezione
  "**Facebook Pixel -- Conversion API**" della pagina "**Sito --
  Preferenze**" (tab **"Tracciamento Dati**") del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracking-facebook-14.bmp](./assets/media/image29.png){width="5.792361111111111in"
height="3.50625in"}

> **ATTENZIONE! come indicato sul Business Manager di Facebook il token
> generato al punto precedente non sarà memorizzato su Facebook per cui
> una volta creato è consigliabile copiarlo e salvarlo anche in un luogo
> sicuro cui poter accedere in caso di bisogno**

- Una volta generato e copiato il token di accesso scorrere in fondo
  alla pagina e cliccare sul pulsante "**Fine**"

![Videate\\tracking-facebook-16.bmp](./assets/media/image30.png){width="5.590972222222222in"
height="3.33125in"}

- A questo punto verremo ricondotti automaticamente alla Panoramica del
  Pixel di Facebook appena creato e identificato dal nome ad esso
  assegnato nei primi step del processo.

![Videate\\tracking-facebook-17.bmp](./assets/media/image31.png){width="5.590972222222222in"
height="3.33125in"}

- Cliccare quindi sulla voce "**Impostazioni**" evidenziata in figura

![Videate\\tracking-facebook-18.bmp](./assets/media/image32.png){width="5.590972222222222in"
height="3.33125in"}

- Copiare l'identificativo del pixel (campo **ID del pixel**)

![Videate\\tracking-facebook-19.bmp](./assets/media/image33.png){width="5.590972222222222in"
height="3.33125in"}

> e inserirlo in corrispondenza del parametro "**Pixel ID**" presente
> all'interno della sezione "**Facebook Pixel -- Conversion API**" della
> pagina "**Sito -- Preferenze**" (tab **"Tracciamento Dati**") del
> Wizard

![Videate\\facebook_tracciamento_client_6.bmp](./assets/media/image34.png){width="5.792361111111111in"
height="3.50625in"}

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

