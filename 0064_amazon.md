# AMAZON



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e la piattaforma **Amazon
Seller** al fine di consentire agli utenti del sito di effettuare la
registrazione e/o l'autenticazione utilizzando direttamente il loro
account Amazon.

**[ATTENZIONE!]{.underline}**

Per poter realizzare questo tipo di integrazione è necessario

- **disporre di un Account Amazon Developer**

- **aver attivato sul proprio sito Passweb un certificato SSL**

1.  Accedere con il proprio account developer al seguente indirizzo
    <https://developer.amazon.com/it/apps-and-games/login-with-amazon>

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_1a.bmp](./assets/media/image301.png)

> Nel caso in cui non si disponga ancora di un account developer sulla
> piattaforma Amazon sarà possibile crearlo in questo momento partendo
> ad esempio dal link "**Sign up for a developer account**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_1b.bmp](./assets/media/image302.png)

2.  Una volta effettuato l'accesso con il proprio account sviluppatore,
    cliccare sulla voce "**Developer Console**" presente nella parte
    alta della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_1c.bmp](./assets/media/image303.png)

> e successivamente sulla voce di menu "**Login with Amazon**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_1d.bmp](./assets/media/image304.png)

3.  Come indicato nella seguente schermata, per poter implementare il
    login con Amazon sarà necessario per prima cosa creare un apposito
    profilo di sicurezza (posto ovviamente che non si disponga già, per
    altre ragioni, di un profilo di sicurezza utilizzabile anche in
    queste condizioni)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_2a.bmp](./assets/media/image305.png)

> Cliccare quindi sul pulsante "**Crea un nuovo profilo di sicurezza**"
> presente all'interno della pagina

4.  Completare la creazione del profilo indicando un **Nome**, una
    **Descrizione** e l' url della pagina del proprio sito utilizzata
    per gestire **l'informativa sulla privacy**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_3a.bmp](./assets/media/image306.png)

> Cliccare quindi sul pulsante "**Salva**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_3b.bmp](./assets/media/image307.png)

5.  Una volta creato il profilo di sicurezza passare con il mouse
    sull'icona raffigurante una piccola rotellina e selezionare, dal
    contestuale menu a tendina, la voce "**Impostazioni Web**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_4a.bmp](./assets/media/image308.png)

6.  All'interno della sezione "**Impostazioni Web**" della maschera di
    gestione del profilo di sicurezza sarà ora possibile prelevare i due
    parametri **Client ID** e **Client Secret,** necessari per poter
    realizzare l'integrazione e consentire agli utenti del nostro sito
    di effettuare l'autenticazione utilizzando il proprio account Amazon

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_5a.bmp](./assets/media/image309.png)

> Copiare quindi i codici evidenziati in figura ed inserirli alla pagina
> "*Sito -- Preferenze -- Social Media*" del Wizard nei relativi campi
> della sezione "Amazon"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_7.bmp](./assets/media/image310.png)

7.  Restando sempre all'interno della della sezione "**Impostazioni
    Web**" della maschera di gestione del profilo di sicurezza, cliccare
    sul pulsante "**Modifica**" e inserire all'interno del campo

    - **Origini consentite:** indirizzo del proprio sito web

    - **URL di ritorno consentiti:** indirizzo del proprio sito seguito
      dal path **/callbackSocial/Amazon**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_6a.bmp](./assets/media/image311.png)

> Cliccare quindi sul pulsante "**Salva**" in modo da aggiornare il
> proprio profilo di sicurezza

A questo punto l'integrazione tra le due piattaforme sarà completata e
gli utenti del sito Passweb potranno quindi autenticarsi utilizzando il
proprio account Amazon.

Nel momento in cui l'utente dovesse cliccare sul relativo pulsante
presente all'interno del pannello di login

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_7a.bmp](./assets/media/image312.png)

verrà infatti ridiretto su una pagina di accesso ad Amazon all'interno
della quale dovrà inserire le credenziali del proprio account.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_9.bmp](./assets/media/image313.png)

Una volta inserite tali credenziali verrà visualizzata la maschera di
consenso attraverso la quale autorizzare la trasmissione dei dati dal
account Amazon al sito Passweb.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_amazon_8a.bmp](./assets/media/image314.png)

Nel caso in cui l'utente fosse già autenticato ad Amazon non gli sarà
richiesto di inserire nuovamente le sue credenziali ma soltanto di
autorizzare il trasferimento dei dati.

Una volta concessa l'autorizzazione l'utente verrà automaticamente
ridiretto al sito Passweb dove risulterà essere perfettamente
autenticato in modo tale da poter procedere al suo primo ordine e/o
all'integrazione dei suoi dati attraverso l'apposita pagina "Profilo
Utente".

Per maggiori informazioni relativamente al componente "Login Utente" e a
come configurarlo per abilitare agli utenti la possibilità di accedere
al sito mediante il proprio profilo social si veda anche la sezione
"*Live Editing -- Lista Componenti Interazione Utente -- Componenti
Interni ai componenti interazione utente -- Social Login*" di questo
manuale.

