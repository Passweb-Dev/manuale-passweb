# GOOGLE



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e **Google** al fine di
consentire agli utenti del sito di effettuare la registrazione e/o
l'autenticazione utilizzando il proprio profilo social.

**ATTENZIONE! Per poter realizzare questo tipo di integrazione è
necessario, ovviamente, che l'amministratore del sito disponga di un
proprio account Google regolarmente funzionante**

1.  Accedere all'indirizzo <https://console.developers.google.com>
    utilizzando il proprio account Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login23.bmp](./assets/media/image70.png)

2.  Una volta effettuato l'accesso alla Google Developers Console aprire
    il menu a tendina posizionato nella parte alta della pagina e creare
    poi un nuovo progetto cliccando sulla relativa voce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login71.bmp](./assets/media/image71.png)

3.  Una volta avviata la creazione di un nuovo progetto sarà necessario
    assegnargli un nome e cliccare poi sul pulsante **Crea**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login25.bmp](./assets/media/image72.png)

4.  Terminata la creazione del nuovo progetto accedere, alla sua
    Dashboard e da qui cliccare sulla voce di menu "**Credenziali**"
    presente nella parte sinistra della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login27.bmp](./assets/media/image265.png)

5.  Cliccare quindi sul pulsante "**Crea Credenziali**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login28.bmp](./assets/media/image266.png)

> e selezionare dal contestuale menu a tendina la voce "**ID client
> OAuth**"

6.  Arrivati a questo punto sarà ora necessario configurare
    correttamente la schermata di consenso che verrà visualizzata agli
    utenti del sito nel momento in cui tenteranno di effettuare
    l'autenticazione mediante il loro account Google.

> Cliccare quindi sul pulsante "**Configura Schermata di consenso**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login72.bmp](./assets/media/image267.png)

7.  Nella maschera di configurazione della tipologia di utenti
    selezionare l'opzione "**Esterno**" e cliccare sul pulsante
    "**Crea**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login72a.bmp](./assets/media/image268.png)

8.  Impostare quindi un nome per l'applicazione (campo "**Nome
    Applicazione**), un logo (campo "**Logo dell'Applicazione**"), i
    domini autorizzati (campo "**Domini autorizzati**") e i link alle
    pagine del proprio sito contenenti le condizioni di privacy e i
    termini di servizio

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login31.bmp](./assets/media/image269.png)

> Una volta inseriti i dati richiesti cliccare sul pulsante "**Salva**"
> posto nella parte bassa della maschera

9.  Terminata la configurazione della Schermata di Consenso dovremo ora
    selezionare il tipo di applicazione che si intende realizzare.

> Tornare quindi alla sezione "**Credenziali**" mediante l'apposita voce
> presente sulla sinistra della pagina, cliccare nuovamente sul pulsante
> "**Crea Credenziali**" e selezionare ancora una volta la voce "**ID
> client OAuth**"

10. Nella successiva maschera selezionare la voce "**Applicazione web**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login72b.bmp](./assets/media/image270.png)

> e inserire poi nei successivi campi i seguenti valori:

- **Nome:** consente di assegnare uno specifico nome al client Web che
  si sta realizzando

- **Origini javascript autorizzate:** inserire l'indirizzo del proprio
  sito Passweb

- **URI di reindirizzamento autorizzati:** inserire l'indirizzo del
  proprio sito Passweb seguito da **/callbackSocial/GooglePlus**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login74.bmp](./assets/media/image271.png)

> Cliccare quindi sul pulsante **Crea** per avviare la creazione delle
> credenziali
>
> A questo punto verranno immediatamente visualizzate le due Api Key da
> inserire poi in Passweb in maniera tale da poter completare
> l'integrazione tra le due piattaforme e consentire agli utenti del
> nostro sito di effettuare l'autenticazione utilizzando il proprio
> account Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login75.bmp](./assets/media/image272.png)

> Le due API Key sopra visualizzate saranno comunque sempre visibili
> all'interno della sezione C**redenziali** relativa al progetto appena
> creato

11. Copiare quindi il codice presente all'interno del campo **ID**
    **Client** sopra evidenziato ed inserirlo alla pagina "*Sito --
    Preferenze -- Social Media*" del Wizard nel campo **Client ID**
    presente nella sezione Google

> Allo stesso modo copiare il codice presente all'interno del campo
> **Client Secret** dell'App di Google e incollarlo all'interno del
> campo **Client Secret** del Wizard di Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login75a.bmp](./assets/media/image273.png)

> Una volta inseriti in Passweb i due parametri di configurazione
> richiesti cliccare sul pulsante "**Salva**" presente nella parte bassa
> della maschera.

A questo punto l'integrazione tra le due piattaforme sarà completata e
gli utenti del sito Passweb potranno quindi autenticarsi utilizzando il
proprio account Google

**ATTENZIONE!** Potrebbe essere necessario sottomettere la propria App e
la propria "Consent Screen" all'approvazione di Google prima di poterle
effettivamente utilizzare per consentire agli utente l'accesso al sito
mediante account Google

Completato il processo di integrazione dunque sarà possibile verificarne
il corretto funzionamento utilizzando un qualsiasi account Google
regolarmente registrato. Nel momento in cui l'utente dovesse infatti
cliccare sul relativo pulsante presente all'interno del pannello di
login,

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login38.bmp](./assets/media/image274.png)

verrà ridiretto su una pagina di accesso di Google all'interno della
quale dovrà inserire le credenziali del proprio account Google.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login70.bmp](./assets/media/image275.png)

Nel caso in cui l'utente fosse già autenticato non gli sarà richiesto di
inserire nuovamente le sue credenziali ma soltanto di autorizzare il
trasferimento dei dati.

Concessa l'autorizzazione ad accedere ai dati del proprio profilo
l'utente verrà automaticamente ridiretto al sito Passweb dove risulterà
essere perfettamente autenticato in modo tale da poter procedere al suo
primo ordine e/o all'integrazione dei suoi dati attraverso l'apposita
pagina "Profilo Utente".

Per maggiori informazioni relativamente al componente "Login Utente" e a
come configurarlo per abilitare agli utenti la possibilità di accedere
al sito mediante il proprio profilo social si veda anche la sezione
"*Live Editing -- Lista Componenti Interazione Utente -- Componenti
Interni ai componenti interazione utente -- Social Login*" di questo
manuale.

