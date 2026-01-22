# ATTIVAZIONE IN GOOGLE ADS DELLE CONVERSIONI AVANZATE



Di seguito viene indicata la procedura da seguire per poter attivare la
gestione delle **conversioni avanzate per il web** all'interno del
proprio account di Google Ads

1.  Accedere al proprio account Google Ads, portarsi nella sezione
    "**Obiettivi -- Impostazioni**" e espandere la sezione
    "**Conversioni Avanzate**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_1.bmp](./assets/media/image2.png){width="5.406944444444444in"
height="3.3465277777777778in"}

2.  Selezionare il parametro "**Attiva le conversioni avanzate**" (può
    essere necessario accettare i "Termini per il trattamento dei dati
    degli annunci su Google)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_2.bmp](./assets/media/image3.png){width="5.406944444444444in"
height="3.3465277777777778in"}

3.  Abilitando il parametro "Attiva le conversioni avanzate" verrà
    visualizzato un ulteriore campo all'interno del quale dovremo andare
    ad indicare il metodo utilizzato per gestire e configurare i dati
    forniti dagli utenti.

> In sostanza dovremo indicare esattamente, selezionandolo dal relativo
> menu a tendina, il metodo adottato nel nostro sistema di tracciamento
> per inviare a Google Ads i dati utente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_3.bmp](./assets/media/image4.png){width="5.406944444444444in"
height="3.3465277777777778in"}

> Come evidenziato in figura le opzioni possibili sono 3:

- Tag Google

- Google Tag Manager

- API Google Ads

> Passweb gestisce 2 delle 3 opzioni indicate, nello specifico dovremo
> quindi selezionare:

- **Tag Google** se in fase di configurazione del sito abbiamo optato
  per un tracciamento diretto **Sito Passweb -- Google Ads**

- **Google Tag Manager** se in fase di configurazione del sito abbiamo
  invece optato per l'implementazione di un sistema di tracciamento
  mediante l'utilizzo di Google Tag Manager

> **ATTENZIONE!** **E' fondamentale selezionare esattamente l'opzione
> corrispondente al metodo di tracciamento che abbiamo deciso di
> implementare all'interno del nostro sito Passweb**
>
> Nel momento in cui dovessimo infatti indicare, all'interno di questo
> campo, un valore non corrispondente a quello che poi andremo
> effettivamente ad utilizzare per inviare i dati utente a Google Ads,
> questi stessi dati non verranno mail elaborati.
>
> Tanto per intenderci se, all'interno di questo campo, dovessimo
> selezionare l'opzione Google Tag, ma lato Passweb dovessimo poi
> decidere di implementare l'invio dei dati utente a Google Ads mediante
> Google Tag Manager quello indicato all'interno di Google Ads non
> corrisponderà a quello che effettivamente facciamo all'interno del
> sito Passweb per cui i dati utente non potranno mai essere elaborati e
> le conversioni avanzate non potranno mai funzionare in maniera
> corretta.
>
> Ora indipendentemente dal fatto di aver indicato a Google Ads che i
> dati utente gli saranno inviati mediante Google Tag (quindi con il
> tracciamento diretto Sito -- Google Ads) oppure mediante Tag Manager,
> avremo sempre a disposizione 3 diverse modalità con cui poter
> raccogliere questi dati:

- Automatica

- Mediante indicazione di selettori CSS o variabili Javascript da
  utilizzare per ricavare i dati utente direttamente dalla pagina web

- Mediante l'inserimento nelle pagine web del nostro sito di un
  determinato snippet di codice.

> **In questo senso, dovremo sempre fare molta attenzione a non
> utilizzare mail la raccolta dati automatica di Google**
>
> Il modo di procede sarà dunque diverso a seconda del fatto di aver
> selezionato, in questa fase, l'opzione Tag Google (in questo caso si
> veda quanto indicato al punto 4) oppure mediante Google Tag Manager
> (in questo caso si veda quanto indicato al punto 5)

4.  Se nel punto 3 di questa procedura abbiamo indicato a Google Ads che
    l'invio dei dati utente avviene mediante Google Tag e quindi in fase
    di configurazione del sito abbiamo optato per il tracciamento
    diretto Sito Passweb -- Googla Ads, l'impostazione del metodo
    utilizzato per la raccolta dei dati utente **deve essere fatta a
    livello di Tag Google**.

> In questo caso dovremo quindi cliccare sul pulsante "**Dettagli Tag**"
> evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_4.bmp](./assets/media/image5.png){width="5.406944444444444in"
height="3.3465277777777778in"}

> e, nella successiva maschera, accertarci di aver **deselezionato**
> entrambe le opzioni "**Rileva automaticamente i dati forniti dagli
> utenti**" (che, attenzione, è selezionato di default) e "**Specifica i
> selettori CSS o le variabili Javascript**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_5.bmp](./assets/media/image6.png){width="5.406944444444444in"
height="3.3465277777777778in"}

> In questo modo i dati utente raccolti e inviati a Google Ads saranno
> esattamente quelli gestiti dallo snippet di codice presente nella
> relativa pagina del sito e generato direttamente da Passweb
>
> **ATTENZIONE! si ricorda che Passweb gestisce il tracciamento diretto
> Sito -- Google Ads solo ed esclusivamente in merito a conversioni
> legate ad eventi di Purchase**
>
> Nel momento in cui l'esigenza dovesse essere quella di gestire
> conversioni legate anche ad altri eventi (es. add_to_cart,
> begin_checkout ...) sarà quindi necessario implementare il sistema di
> tracciamento utilizzando Google Tag Manager
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Sito -- Preferenze -- Tracciamento Dati --
> Google -- Google Ads*" di questo manuale

5.  Se nel punto 3 di questa procedura abbiamo indicato a Google Ads che
    l'invio dei dati utente avviene mediante Google Tag Manager, e
    quindi in fase di configurazione del sito abbiamo optato per il
    tracciamento mediante GTM, l'impostazione del metodo utilizzato per
    la raccolta dei dati utente **dovrà essere fatta direttamente
    all'interno di Google Tag Manager in fase di configurazione della
    variabile di tipo "User Provided Data"**, variabile questa che dovrà
    essere configurata impostando il parametro "**Type**" sull'opzione
    "**Manual configuration**" secondo quanto indicato all'interno del
    capitolo "*Google Tag manager -- User Provided Data e conversioni
    avanzate -- Creazione delle variabili per la gestione dei dati
    utente -- Variabile PWB User Provided Data*" di questo manuale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_6.bmp](./assets/media/image7.png){width="5.406944444444444in"
height="3.3465277777777778in"}

6.  Una volta settato tutto correttamente il pulsante "**Salva**"
    presente nella parte bassa della maschera ci consente di salvare le
    modifiche apportate e di attivare così per il nostro account Ads la
    gestione delle conversioni avanzate per il web.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_attivazione_ec_7.bmp](./assets/media/image8.png){width="5.406944444444444in"
height="3.3465277777777778in"}

**ATTENZIONE! l'attivazione della funzionalità "Conversioni avanzate per
il web" all'interno di Google Ads di fatto prepara solo il sistema alla
ricezione dei dati utente, dati questi che devono poi essere
effettivamente inviati ad Ads implementando in maniera corretta il
proprio sistema di tracciamento**

Per maggiori informazioni in merito si veda ad esempio quanto indicato
all'interno del capitolo "*Google Tag manager -- User Provided Data e
conversioni avanzate"* di questo manuale

