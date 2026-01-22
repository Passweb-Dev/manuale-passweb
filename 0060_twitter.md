# TWITTER



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e **Twitter** al fine di
consentire agli utenti del sito di effettuare la registrazione e/o
l'autenticazione utilizzando il proprio profilo social.

**ATTENZIONE! Per poter realizzare questo tipo di integrazione è
necessario, che l'amministratore del sito disponga sia di un proprio
account Twitter sia di un account developer all'interno della stessa
piattaforma social (account questo che potrà essere creato
contestualmente all'attivazione della prima app)**

Nel caso in cui si disponga già di un account sviluppatore per Twitter
passare direttamente al punto 3

1.  Accedere alla piattaforma di sviluppo di Twitter al seguente link:
    <https://developer.twitter.com> e cliccare sulla voce **Apps**
    presente nel menu

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter1.bmp](./assets/media/image251.png){width="4.9222222222222225in"
height="3.3569444444444443in"}

2.  Cliccare quindi sul pulsante "**Create an App**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter3.bmp](./assets/media/image252.png){width="4.9222222222222225in"
height="3.3569444444444443in"}

> e completare, fornendo tutti i dati richiesti dalla piattaforma, i
> passaggi necessari per portare a termine correttamente la creazione
> del proprio account sviluppatore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter3a.bmp](./assets/media/image253.png){width="4.9222222222222225in"
height="3.545138888888889in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter3b.bmp](./assets/media/image254.png){width="4.9222222222222225in"
height="3.545138888888889in"}

> Una volta completata la creazione del proprio account sviluppatore
> verremo ridiretti automaticamente all'interno del "**Developer
> Portal**" di Twitter dove potremo creare la nostra app

3.  Nel caso in cui dovessimo già disporre di un account developer
    all'interno della piattaforma social, sarà necessario per prima cosa
    effettuare l'accesso a Twitter con il proprio account e
    successivamente, a login effettuata, accedere all'indirizzo
    <https://developer.twitter.com>

> A questo punto sarà necessario selezionare, dal menu presente nella
> parte alta della pagina, la voce **Apps**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter3c.bmp](./assets/media/image255.png){width="4.9222222222222225in"
height="2.9090277777777778in"}

> in maniera tale da poter accedere alla sezione del portale di sviluppo
> in cui poter creare la nostra nuova app

4.  Una volta effettuato l'accesso alla sezione del portale di sviluppo
    deputata alla creazione delle app cliccare sul pulsante "**Create
    App**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter3d.bmp](./assets/media/image256.png){width="4.9222222222222225in"
height="3.50625in"}

5.  Assegnare quindi un nome all'App e cliccare sul pulsante
    "**Complete**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter4.bmp](./assets/media/image257.png){width="4.9222222222222225in"
height="3.5131944444444443in"}

6.  Completata la creazione dell'App verrà visualizzata una maschera
    contenente i dati da inserire all'interno del proprio sito Passweb
    per realizzare l'integrazione tra le due piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter4a.bmp](./assets/media/image258.png){width="4.9222222222222225in"
height="3.5131944444444443in"}

> Copiare quindi il contenuto del campo "**Api Key**" ed inserirlo
> all'interno del campo "**Consumer Key (API Key)** presente alla pagina
> "*Sito -- Preferenze -- Social Media*" del Wizard nella sezione
> relativa a Twitter.
>
> Allo stesso modo copiare il contenuto del campo "**API secret Key**"
> ed inserirlo all'interno del campo "**Consumer Secret (API Secret)**"
> presente sempre alla pagina"*Sito -- Preferenze -- Social Media*" del
> Wizard

7.  Cliccare sul pulsante "**App Setting**" in maniera tale da essere
    ridiretti sulla pagina di gestione delle impostazioni della propria
    App, pagina questa da cui potremo eventualmente prelevare (sezione
    "Keys and tokens") i parametri di configurazione "Api Key" e "Api
    secret key") indicati al punto precedente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter4b.bmp](./assets/media/image259.png){width="4.9222222222222225in"
height="3.5131944444444443in"}

8.  Nella pagina di gestione delle impostazioni della propria app,
    cliccare sul pulsante "**Edit**" presente in corrispondenza della
    sezione "**Authentication settings**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter5.bmp](./assets/media/image260.png){width="4.9222222222222225in"
height="3.5131944444444443in"}

> e compilare i campi richiesti come di seguito indicato:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter5a.bmp](./assets/media/image261.png){width="4.9222222222222225in"
height="3.5131944444444443in"}

- Abilitare il check "**Enable 3rd party authentication**"

- Abilitare il check "**Request email address from users**"

- Impostare all'interno del campo "**Callback URLs**" l'indirizzo del
  proprio sito web seguito dalla stringa **/callbackSocial/Twitter**

- Impostare all'interno del campo "**Website URL**" l'indirizzo del
  proprio sito web

- Impostare all'interno dei campi "**Terms of service**" e "**Privacy
  policy**" gli indirizzi delle pagine del proprio sito relative
  rispettivamente alla gestione dei "Termini e Condizioni" e alla
  "Privacy Policy"

A questo punto l'integrazione tra le due piattaforme sarà completata e
gli utenti del sito Passweb potranno quindi autenticarsi utilizzando il
proprio profilo Twitter

**ATTENZIONE! Twitter non offre, a differenza di Facebook, la
possibilità di mettere la propria App in modalità Test e/o di utilizzare
utenti fittizi per verificare il corretto funzionamento
dell'integrazione.**

Completato il processo di integrazione dunque, l'App sarà subito on line
e sarà possibile verificarne il corretto funzionamento utilizzando un
qualsiasi account LinkedIn regolarmente registrato.

Nel momento in cui l'utente dovesse cliccare sul relativo pulsante
presente all'interno del pannello di login

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter13.bmp](./assets/media/image262.png){width="5.00625in"
height="3.214583333333333in"}

verrà ridiretto su una pagina di accesso di Twitter all'interno della
quale dovrà inserire le credenziali del proprio account, oltre ad
autorizzare la trasmissione dei dati dal proprio profilo Twitter al sito
Passweb.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_twitter14.bmp](./assets/media/image263.png){width="5.415277777777778in"
height="3.5909722222222222in"}

Nel caso in cui l'utente fosse già autenticato al Social Network non gli
sarà richiesto di inserire nuovamente le sue credenziali ma soltanto di
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

Il campo **Account Twitter** presente alla pagina "*Sito -- Preferenze
-- Social Media*" del Wizard consente infine di

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_twitter.bmp](./assets/media/image264.png){width="5.811805555555556in"
height="3.545138888888889in"}

**Account Twitter:** consente di specificare il proprio account Twitter.
E' necessario per valorizzare il Meta Tag "**twitter:site**" nel momento
in cui si dovesse decidere di abilitare, per il proprio sito, il
protocollo Opengraph in maniera tale da poter indicare in maniera più
precisa quali informazioni di una pagina web dovranno essere condivise
sui vari social.

