# PAYPAL



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e **PayPal** al fine di
consentire agli utenti del sito di effettuare la registrazione e/o
l'autenticazione utilizzando i dati presenti sul proprio profilo PayPal.

**ATTENZIONE! Per poter realizzare questo tipo di integrazione è
necessario, ovviamente, che l'amministratore del sito disponga di un
proprio account PayPal regolarmente funzionante**

1.  Accedere all'indirizzo <https://developer.paypal.com> ed effettuare
    l'accesso con il proprio account PayPal.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login51.bmp](./assets/media/image289.png){width="5.00625in"
height="3.454861111111111in"}

2.  Una volta effettuato l'accesso verremo ricondotti nella
    **Dashboard** all'interno della sezione "**My apps and
    Credentials**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login53.bmp](./assets/media/image290.png){width="5.519444444444445in"
height="3.376388888888889in"}

> dove avremo la possibilità di creare App sia nell'ambiente **Sandbox**
> di test che in quello **Live** di produzione
>
> **ATTENZIONE! Passweb gestisce attualmente le App PayPal solamente in
> modalità Live**

3.  Selezionare quindi, mediante l'apposito controllo l'ambiente
    **Live** e cliccare poi sul pulsante "**Create app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login53a.bmp](./assets/media/image291.png){width="5.00625in"
height="3.454861111111111in"}

4.  Assegnare un nome all'app e cliccare sul pulsante "**Create app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login53b.bmp](./assets/media/image292.png){width="5.00625in"
height="3.454861111111111in"}

5.  Una volta terminata la creazione dell'App accedere alla pagina di
    dettaglio dell'app

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login56.bmp](./assets/media/image293.png){width="5.00625in"
height="3.454861111111111in"}

> dove potremo trovare i due parametri da inserire poi in Passweb per
> completare l'integrazione tra le due piattaforme e consentire agli
> utenti del nostro sito di effettuare l'autenticazione utilizzando il
> proprio account PayPal
>
> Copiare quindi il codice presente all'interno del campo **Client** ed
> inserirlo alla pagina "Sito -- Preferenze -- Social Media" del Wizard
> nel campo **Client ID** presente nella sezione PayPal.
>
> Allo stesso modo copiare il codice presente all'interno del campo
> **Secret** e incollarlo all'interno del campo **Secret** del Wizard di
> Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login56a.bmp](./assets/media/image294.png){width="5.811805555555556in"
height="3.545138888888889in"}

6.  Per completare la configurazione dovremo ora impostare l'URL di
    ritorno per consentire agli utenti di essere correttamente ridiretti
    sul sito Passweb una volta effettuata l'autenticazione con l'account
    PayPal e, ovviamente, settare i vari permessi necessari per
    stabilire quali dati dovranno essere passati, previa autorizzazione
    del utente, dall'account PayPal al sito Passweb.

> Nella pagina di dettaglio dell'app portarsi quindi all'interno della
> sezione **Live App Settings** e inserire all'interno del campo
> **Return URL** l'indirizzo del proprio sito Passweb seguito dalla
> stringa **/callbackSocial/PayPal**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login58.bmp](./assets/media/image295.png){width="5.00625in"
height="3.454861111111111in"}

> Considerando inoltre che la nostra App dovrà essere utilizzata per
> consentire agli utenti del sito di effettuare l'autenticazione
> utilizzando il loro Account PayPal sarà necessario assicurarsi di aver
> selezionato all'interno della sezione **App feature options** la voce
> **Connect with PayPal (formerly Log In with PayPal)**, come
> evidenziato in figura.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login58a.bmp](./assets/media/image296.png){width="5.00625in"
height="3.454861111111111in"}

> Una volta impostati i parametri di configurazione come descritto
> cliccare sul pulsante **Save**

7.  Cliccare quindi sul pulsante **Advanced Options** presente in
    corrispondenza della voce **Login with PayPal**

> In questo modo verrà evidenziata un'ulteriore sezione dei parametri di
> configurazione in cui poter decidere, nello specifico, quali dati
> dovranno essere trasmessi dall'account PayPal al sito Passweb per
> poter poi effettuare la registrazione del nuovo utente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login60.bmp](./assets/media/image297.png){width="5.00625in"
height="3.454861111111111in"}

> **Verificare di aver selezionato i dati relativi al nome utente, alla
> mail e all'indirizzo.**
>
> **ATTENZIONE! Come evidenziato nel relativo messaggio prima di poter
> selezionare i dati relativi a mail ed indirizzo (obbligatori per il
> corretto funzionamento dell'integrazione) sarà necessario sottomettere
> l'app ad un processo di approvazione seguendo per questo la procedura
> indicata nel messaggio stesso**
>
> Inserire inoltre all'interno dei campi **Privacy policy URL** e **User
> agreement URL**, rispettivamente, gli indirizzi delle pagine del sito
> Passweb utilizzate per descrivere le proprie condizioni di Privacy
> Policy e di User Agreement
>
> Verificare infine di aver selezionato l'opzione "**Enable customers
> who haven\'t yet confirmed their email address with PayPal, to log in
> to your app**" in modo tale da consentire agli utenti che non hanno
> ancora confermato in PayPal il loro indirizzo email, di poter comunque
> effettuare l'autenticazione al sito Passweb.
>
> Una volta impostati i parametri di configurazione come descritto
> cliccare sul pulsante **Save**

A questo punto l'integrazione tra le due piattaforme sarà completata e
gli utenti del sito Passweb potranno quindi autenticarsi utilizzando il
proprio account PayPal

Completato il processo di integrazione, l'App sarà subito on line e sarà
possibile verificarne il corretto funzionamento utilizzando un qualsiasi
account PayPal regolarmente registrato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login64.bmp](./assets/media/image298.png){width="5.1625in"
height="3.5256944444444445in"}

Nel momento in cui l'utente dovesse cliccare sul relativo pulsante
presente all'interno del pannello di login, verrà ridiretto su una
pagina di accesso di PayPal all'interno della quale dovrà inserire le
credenziali del proprio account.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login68.bmp](./assets/media/image299.png){width="5.1625in"
height="3.5256944444444445in"}

Una volta inserite tali credenziali verrà visualizzata la maschera di
consenso attraverso la quale autorizzare la trasmissione dei dati dal
account PayPal al sito Passweb.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login69.bmp](./assets/media/image300.png){width="5.155555555555556in"
height="2.9090277777777778in"}

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

