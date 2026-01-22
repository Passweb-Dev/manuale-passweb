# LINKEDIN



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e **Linkedin** al fine di
consentire agli utenti del sito di effettuare la registrazione e/o
l'autenticazione utilizzando il proprio profilo social.

**ATTENZIONE! Per poter realizzare questo tipo di integrazione è
necessario, ovviamente, che l'amministratore del sito disponga di un
proprio account Linkedin regolarmente funzionante**

1.  Accedere all'indirizzo <https://developer.linkedin.com>,
    autenticarsi con il proprio account LinkedIn e cliccare sulla voce
    **My Apps** presente nel menu principale e da qui selezionare la
    voce "**Create app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login39.bmp](./assets/media/image276.png)

> In alternativa cliccare direttamente sul pulsante "**Create app**"
> presente nella pagina

2.  Completare la creazione della nuova App inserendo i dati richiesti
    all'interno del relativo Form (i campi evidenziati con un piccolo
    asterisco sono obbligatori) e cliccare quindi sul pulsante "**Create
    app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login43.bmp](./assets/media/image277.png)

> **ATTENZIONE!** la creazione di una nuova app richiede anche la
> presenza o la creazione di una propria pagina LinkedIn (campo
> **LinkedIn Page**)

3.  Una volta completata il form sopra evidenziato con tutti i dati
    obbligatori, cliccando sul pulsante **Invia** verremo
    automaticamente ricondotti alla sezione **Setting** della nuova App

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login43a.bmp](./assets/media/image278.png)

> Portarsi quindi all'interno della sezione **Auth** cliccando sulla
> corrispondente voce di menu presente nella parte alta della pagina

4.  All'interno di questa sezione potremo visualizzare e prelevare le
    API Key da inserire poi in Passweb in maniera tale da poter
    completare l'integrazione tra le due piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login44.bmp](./assets/media/image279.png)

> copiare il codice presente all'interno del campo "**Client ID"** ed
> inserirlo alla pagina "*Sito -- Preferenze -- Social Media*" del
> Wizard nel campo **ID** **client** presente nella sezione LinkedIn
>
> Allo stesso modo copiare il codice presente all'interno del campo
> **Client Secret** e incollarlo all'interno del campo **Secret**
> **client** del Wizard di Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45c.bmp](./assets/media/image280.png)

> Una volta inseriti in Passweb i due parametri di configurazione
> richiesti cliccare sul pulsante "**Salva**" presente nella parte bassa
> della maschera.
>
> Per completare la configurazione dovremo ora impostare l'URL di
> ritorno per consentire agli utenti di essere correttamente ridiretti
> sul sito Passweb una volta effettuata l'autenticazione con il proprio
> account LinkedIn e, ovviamente, settare i vari permessi necessari per
> stabilire quali dati dovranno essere passati, previa autorizzazione
> del utente, dall'account LinkedIn al sito Passweb

5.  **Autorizzare l'URL di reindirizzamento**.

> Per questo è necessario inserire nel campo "**Authorized redirect URLs
> for your app**" presente all'interno della sezione **OAuth 2.0
> settings**, l'indirizzo del proprio sito Passweb seguito dalla stringa
> **/callbackSocial/LinkedIn**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45.bmp](./assets/media/image281.png)

6.  **Selezionare il tipo di app che si intende creare**.

> Per questo è necessario portarsi all'interno della sezione
> **Products** cliccando sulla relativa voce di menu presente nella
> parte alta della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45a.bmp](./assets/media/image282.png)

> Selezionare quindi l'opzione "**Sign In with Linkedin**", accettare i
> termini e le condizioni d'uso e cliccare sul pulsante "**Add
> product**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45b.bmp](./assets/media/image283.png)

> **ATTENZIONE!** A seguito di questa fase l'app potrebbe andare in
> revisione a LinkedIn. Sarà quindi necessario attendere l'approvazione
> dell'app per poter procedere
>
> Una volta approvata l'app da parte di Linkedin dovremo vedere il
> prodotto "**Sign In with Linkedin**" all'interno della sezione
> "**Added products**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45d.bmp](./assets/media/image284.png)

7.  Una volta approvata l'app da parte di Linkedin e verificato che il
    prodotto "**Sign In with Linkedin**" sia stato correttamente
    aggiunto all'interno della sezione "**Added products**", portarsi
    nuovamente all'interno della sezione **Auth** cliccando per questo
    sulla corrispondente voce di menu e verificare che nella sotto
    sezione "**OAuth 2.0 scopes**" siano stati correttamente aggiunti i
    permessi **r_emailaddress** e **r_liteprofile**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login45e.bmp](./assets/media/image285.png)

A questo punto l'integrazione tra le due piattaforme sarà completata e
gli utenti del sito Passweb potranno quindi autenticarsi utilizzando il
proprio profilo LinkedIn

Completato il processo di integrazione dunque, l'App sarà subito on line
e sarà possibile verificarne il corretto funzionamento utilizzando un
qualsiasi account LinkedIn regolarmente registrato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login50.bmp](./assets/media/image286.png)

Nel momento in cui l'utente dovesse cliccare sul relativo pulsante
presente all'interno del pannello di login, verrà ridiretto su una
pagina di accesso di Linkedin all'interno della quale dovrà inserire le
credenziali del proprio account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login67.bmp](./assets/media/image287.png)

Una volta inserite le credenziali del proprio account verrà visualizzata
un ulteriore maschera di consenso al trasferimento dei dati indicati dal
proprio account LinkedIn al sito Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login67a.bmp](./assets/media/image288.png)

**ATTENZIONE**! Nel caso in cui l'utente fosse già autenticato al Social
Network non gli sarà richiesto di inserire nuovamente le sue credenziali
ma soltanto di autorizzare il trasferimento dei dati.

Una volta concessa l'autorizzazione l'utente verrà quindi
automaticamente ridiretto al sito Passweb dove risulterà essere
autenticato in modo tale da poter procedere al suo primo ordine e/o
all'integrazione dei suoi dati attraverso l'apposita pagina "Profilo
Utente".

Per maggiori informazioni relativamente al componente "Login Utente" e a
come configurarlo per abilitare agli utenti la possibilità di accedere
al sito mediante il proprio profilo social si veda anche la sezione
"*Live Editing -- Lista Componenti Interazione Utente -- Componenti
Interni ai componenti interazione utente -- Social Login*" di questo
manuale.

