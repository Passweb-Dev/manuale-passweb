# APPLE



Di seguito è indicata la procedura da seguire per consentire agli utenti
del sito di effettuare la registrazione e/o l'autenticazione utilizzando
il loro Apple ID

**ATTENZIONE!** Per poter realizzare questo tipo di integrazione è
necessario disporre di:

- **un certificato SSL** correttamente associato al proprio sito web

- **un account Apple Developer** regolarmente funzionante

- **l'iscrizione al Apple Developer Program**

In assenza di uno qualsiasi di questi prerequisiti non sarà possibile
prelevare dal portale per sviluppatori di Apple tutte le risorse
necessarie per creare l'app di integrazione tra le due piattaforme.

Una volta soddisfatti i prerequisiti sarà poi necessario:

1.  Accedere con il proprio account al Portale per sviluppatori di Apple
    (<https://developer.apple.com> ) e cliccare sulla voce
    "**Certificates, Identifiers & Profiles**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_1.bmp](./assets/media/image315.png)

2.  Una volta effettuato l'accesso alla sezione di gestione dei
    certificati cliccare sulla voce "**Identifiers**" presente nel menu
    posto sulla sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_2.bmp](./assets/media/image316.png)

> e, successivamente, cliccare sull'icona blu raffigurante un piccolo +
> per aggiungere un nuovo identificatore

3.  Selezionare quindi "**App IDs**", cliccare sul pulsante
    "**Continue**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_3.bmp](./assets/media/image317.png)

> selezionare come tipologia del nuovo identificatore l'opzione "App" e
> cliccare ancora una volta sul pulsante "**Continue"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_4.bmp](./assets/media/image318.png)

4.  Nella successiva schermata sarà necessario impostare una
    **Descrizione** e un **Bundle ID** per l'App ID che andremo a creare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_5.bmp](./assets/media/image319.png)

> Inserire quindi all'interno del campo "**Description**" una stringa
> identificativa della nostra App (es. "Login Passweb") mentre per quel
> che riguarda il Bundle ID è consigliato inserire una stringa in stile
> reverse dns. Supponendo quindi che il sito su cui andremo ad
> implementare l'autenticazione tramite Apple ID risponda al dominio
> clobis.passepartout.net potremo inserire all'interno del campo "Bundle
> ID" la stringa **net.passepartout.clobis**

5.  Restando sempre all'interno della stessa pagina scorrere l'elenco
    delle funzionalità presenti all'interno della sezione
    "**Capabilities**" e selezionare l'opzione "**Sign in with Apple**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_6.bmp](./assets/media/image320.png)

> Cliccare quindi sul pulsante "**Continue**" e successivamente sul
> pulsante "**Register**" posto nella parte alta della pagina. In questo
> modo verrà confermata la creazione del nostro App ID e verremo
> automaticamente ricondotti alla pagina di gestione dei certificati
> degli identificatori e dei profili

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_7.bmp](./assets/media/image321.png)

6.  Una volta creato l'App ID dovremo ora creare un nuovo Service ID.
    Restando quindi all'interno della pagina "Certificates, Identifiers
    & Profiles" cliccare ancora una volta sull'icona blu raffigurante un
    piccolo +

> Nella successiva schermata selezionare questa volta l'opzione
> "**Services ID**" e cliccare sul pulsante "**Continue**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_8.bmp](./assets/media/image322.png)

7.  Nella successiva schermata dovremo inserire all'interno del campo
    "**Description**" il nome dell'App che vedranno poi gli utenti
    durante il flusso di autenticazione al nostro sito con il loro Apple
    ID.

> All'interno del campo "**Identifier**" andrà invece inserito, sempre
> in notazione dns reverse l'identificatore del Service ID che stiamo
> registrando e che diventerà poi l'id del client OAuth utilizzato per
> l'autenticazione. Considerando dunque che nei passaggi precedenti come
> Bundle ID dell'App avevamo utilizzato la stringa
> net.passepartout.clobis ora all'interno del campo Identifier potremo
> inserire la stringa net.passepartout.clobisClient

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_9.bmp](./assets/media/image323.png)

> Una volta inseriti i dati richiesti cliccare sul pulsante
> "**Continue**" e successivamente sul pulsante "**Register**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_10.bmp](./assets/media/image324.png)

> In questo modo verrà confermata la creazione del nostro Service ID e
> verremo nuovamente ricondotti alla pagina di gestione dei certificati
> degli identificatori e dei profili, questa volta però nella sezione
> relativa ai Service IDs

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_11.bmp](./assets/media/image325.png)

8.  Cliccare quindi tra quelli presenti in elenco il Service ID appena
    creato in maniera tale da poter tornare ad editarne i dettagli

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_12.bmp](./assets/media/image326.png)

> Nella maschera di dettaglio del Service ID selezionare quindi
> l'opzione "**Sign In with Apple**" e cliccare sul pulsante
> "**Configure**" in maniera tale da poter accedere alla sezione in cui
> inserire il domino del sito su cui andrà poi in esecuzione la nostra
> App e gli url di reindirizzamento utilizzati durante il flusso di
> autenticazione OAuth

9.  Verificare quindi che all'interno del campo "**Primary App ID**" sia
    impostata l'App precedentemente creata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_13.bmp](./assets/media/image327.png)

> Compilare inoltre i due campi "Domains and Subdomains" e "Return
> URLSs" come di seguito indicato:

- **Domains and Subdomains:** dominio del nostro sito

- **Return URLSs**: dominio del nostro sito seguito dalla stringa
  **/callbackSocial/Apple**

> Cliccare quindi sul pulsante "**Next**" successivamente sul pulsante
> "**Done**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_14.bmp](./assets/media/image328.png)

> e infine sul pulsante "**Continue**" e "**Save**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_15.bmp](./assets/media/image329.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_16.bmp](./assets/media/image330.png)

10. Arrivati a questo punto lo step successivo sarà quello relativo alla
    generazione della chiave da utilizzare poi in fase di autenticazione

> Dalla pagina "Certificates, Identifiers & Profiles" cliccare quindi
> sulla voce **Keys** presente nel menu posto sulla sinistra della
> pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_17.bmp](./assets/media/image331.png)

> e, successivamente, cliccare sull'icona blu raffigurante un piccolo +
> per aggiungere una nuova chiave

11. Assegnare quindi un nome alla chiave (campo Key Name), selezionare
    l'opzione "**Sign in with Apple**" e cliccare sul relativo pulsante
    "**Configure**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_18.bmp](./assets/media/image332.png)

12. Nella successiva maschera impostare all'interno del campo "**Primary
    App ID**" l'App ID creato nei precedenti passaggi di questa guida

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_19.bmp](./assets/media/image333.png)

> Cliccare quindi sul pulsante "**Save**" e successivamente sui pulsanti
> "**Continue**" e "**Register**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_20.bmp](./assets/media/image334.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_21.bmp](./assets/media/image335.png)

13. Arrivati a questo punto dovremo effettuare il download della chiave
    generata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_22.bmp](./assets/media/image336.png)

> Cliccare quindi sul pulsante **Download** e salvare il file in una
> cartella locale del nostro pc
>
> **ATTENZIONE!** Come indicato dal relativo messaggio di avvertimento
> una volta effettuato il download della chiave questa verrà eliminata
> dai server Apple e non sarà più possibile scaricarla per cui è
> altamente consigliato conservare questa chiave con attenzione ed
> effettuare magari anche una copia di backup della stessa da conservare
> in locale sul proprio pc

14. Una volta creata la chiave l'ultimo passaggio è quello che prevede
    di andare riprendere l'identificatore del Service Id creato al punto
    7 e inserirlo tra i parametri di configurazione del nostro sito.

> Tornare quindi all'interno della pagina "**Certificates, Identifiers &
> Profiles**" cliccare sulla voce di menu "**Identifiers**" e accedere,
> utilizzando il menu a tendina evidenziato in figura alla sezione
> relativa ai Services IDs

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_23.bmp](./assets/media/image337.png)

15. Selezionare quindi il Service Id precedentemente creato in maniera
    tale da accedere alla sua maschera di dettaglio

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_24.bmp](./assets/media/image338.png)

> Copiare quindi la stringa presente in corrispondenza del campo
> "**Identifier**" ed inserirla alla pagina "*Sito -- Preferenze --
> Social Media*" del Wizard nel campo **Service ID** presente
> all'interno della sezione Apple

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_25.bmp](./assets/media/image339.png)

Completata la configurazione potremo quindi aprire il sito Passweb e
scegliere di effettuare l'autenticazione utilizzando il nostro Apple ID

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_26.bmp](./assets/media/image340.png)

Cliccando sul relativo pulsante presente in corrispondenza del pannello
di Login l'utente verrà quindi ricondotto ad una pagina di accesso in
cui dovrà inserire il proprio Apple ID

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_28.bmp](./assets/media/image341.png)

Una volta inserito il proprio Apple ID potrà essere richiesto, se attiva
sul proprio Apple ID la verifica in due fasi, un codice di accesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_29.bmp](./assets/media/image342.png)

Inserito il codice verrà chiesto all'utente di condividere o meno la
propria mail con il sito su cui sta effettuando l'accesso (opzione
selezionata a default).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\login_apple_30.bmp](./assets/media/image343.png)

Cliccando quindi sul pulsante "**Continua**" l'utente verrà
automaticamente ricondotto e autenticato al sito Passweb

**ATTENZIONE!** Nel momento in cui l'utente dovesse decidere di non
condividere l'indirizzo mail, per portare a termine correttamente un
ordine all'interno del sito Passweb dovrebbe prima completare il suo
profilo inserendo oltre all'indirizzo di spedizione anche il proprio
indirizzo mail

Per maggiori informazioni relativamente al componente "Login Utente" e a
come configurarlo per abilitare agli utenti la possibilità di accedere
al sito mediante il proprio Apple ID si veda anche la sezione "*Live
Editing -- Lista Componenti Interazione Utente -- Componenti Interni ai
componenti interazione utente -- Social Login*" di questo manuale.

