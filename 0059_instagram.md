# INSTAGRAM



Di seguito è indicata la procedura da seguire per realizzare
l'integrazione tra il proprio sito Passweb e **Instagram** al fine di
consentire agli utenti del sito di effettuare la registrazione e/o
l'autenticazione utilizzando il proprio profilo social.

**ATTENZIONE!** Per poter realizzare questo tipo di integrazione è
necessario che l'amministratore del sito disponga:

- **di un account sviluppatore Facebook regolarmente funzionante**

- **di un account Instagram con contenuti multimediali**

1.  Accedere al sito Facebook per sviluppatori
    (<https://developers.facebook.com> ) con il proprio account e
    selezionare la voce "**Le mie app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login3.bmp](./assets/media/image209.jpeg)

2.  Una volta effettuato l'accesso alla sezione delle App crearne una
    nuova cliccando per questo sul pulsante "**Crea un' app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login4.bmp](./assets/media/image210.png)

3.  All'interno della maschera di selezione della tipologia di App da
    realizzare selezionare la voce **"Creazione di funzioni collegate"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login5.bmp](./assets/media/image211.png)

4.  Compilare la maschera relativa ai dati anagrafici dell'App che si
    sta realizzando (Nome App, Indirizzo Mail, Account Business Manager
    collegato) e cliccare sul pulsante "**Crea app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login6.bmp](./assets/media/image212.png)

5.  Una volta creata l'app selezionare dal menu presente sulla sinistra
    della pagina la voce "**Impostazioni -- Di Base**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_2.bmp](./assets/media/image229.png)

> e completare l'anagrafica dell'app inserendo tutti i dati richiesti,
> facendo attenzione, in particolare, ad inserire le seguenti
> informazioni (necessarie poi per poter mandare l'app in validazione):

- **URL della Normativa sulla privacy:** url della pagina del proprio
  sito web in cui sono indicate le condizioni di gestione della privacy

- **Icona dell'app:** icona identificativa dell'app (dimensione comprese
  tra 512x512px e 1024x1024px)

- **Categoria:** indicare tra le categorie proposte quella della propria
  app (es. Utility e Produttività)

- **Scopo dell'app:** selezionare l'opzione "**Tuo o della tua
  azienda**"

> Una volta inseriti i dati richiesti cliccare sul pulsante "**Salva le
> modifiche**" posto nella parte bassa della pagina.

6.  Rimanendo sempre all'interno della stessa sezione scorrere ora fino
    al fondo della pagina cliccare sul pulsante "**Aggiungi
    piattaforma**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_3.bmp](./assets/media/image230.png)

> Nella successiva maschera, selezionare l'opzione "**Sito Web**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_4.bmp](./assets/media/image231.png)

> Aggiungere quindi l'indirizzo del proprio sito all'interno del campo
> "**URL del sito**" e cliccare su "**Salva le Modifiche**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_5.bmp](./assets/media/image232.png)

7.  Una volta aggiunto il tipo di piattaforma su cui dovrà essere
    utilizzata l'app, cliccare sulla voce "**Prodotti**" presente nel
    menu posto sulla sinistra della pagina, selezionare "**Instagram
    Basic Display**" e cliccare sul pulsante "**Configura**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_1.bmp](./assets/media/image233.png)

> Scorrere quindi in fondo alla pagina e cliccare sul pulsante "**Create
> New App**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_6.bmp](./assets/media/image234.png)

8.  Nella successiva maschera (Create a New Instagram App ID) inserire,
    all'interno del campo "**Nome visualizzato"** il nome della propria
    app e cliccare quindi sul pulsante "**Crea un' app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_7.bmp](./assets/media/image235.png)

9.  Una volta terminata la creazione dell'app verremo automaticamente
    ricondotti all'interno della sezione "**Basic Display**" evidenziata
    in figura dove dovremo inserire altri dati di fondamentale
    importanza per poter completare la nostra integrazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_8.bmp](./assets/media/image236.png)

10. Portarsi quindi in corrispondenza della sezione "**Impostazioni del
    client OAuth**" e inserire all'interno del campo "**URI di
    reindirizzamento OAuth validi**", l'indirizzo del proprio sito web
    seguito dalla stringa **/callbackSocial/Instagram** come evidenziato
    in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_9.bmp](./assets/media/image237.png)

> Allo stesso modo inserire l'indirizzo del proprio sito web anche
> all'interno dei successivi campi "**URL di callback per la rimozione
> dell\'autorizzazione**" e "**URL per la richiesta di eliminazione dei
> dati**"
>
> Cliccare quindi sul pulsante "**Salva le modifiche** " posto nella
> parte bassa della pagina

11. Sempre all'interno della pagina "Basic Display" portarsi ora in
    corrispondenza della sezione "**Analisi dell'app per Instagram Basic
    Display**" e aggiungere l'opzione relativa al permesso
    "**instagram_graph_user_profile**" cliccando sul corrispondente
    pulsante "**Aggiungi alla richiesta**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_10.bmp](./assets/media/image238.png)

12. Restando ancora all'interno della pagina "Basic Display" sarà
    necessario, arrivati a questo punto, prelevare i dati da inserire
    poi in Passweb per completare l'integrazione tra le due piattaforme.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_11.bmp](./assets/media/image239.png)

> Nello specifico i dati richiesti saranno quelli presenti all'interno
> dei campi "**ID app Instagram**" e "**Chiave Segreta di Instagram**"
> sopra evidenziati
>
> Copiare quindi il codice presente all'interno del campo "**ID app
> Instagram**" ed inserirlo alla pagina "*Sito -- Preferenze -- Social
> Media*" del Wizard nel campo **App ID** presente nella sezione
> **Instagram**
>
> Allo stesso modo copiare il codice presente all'interno del campo
> "**Chiave Segreta di Instagram**" e incollarlo nel campo **Client
> Secret**
>
> **ATTENZIONE!** Per visualizzare il codice presente all'Interno del
> campo "Chiave Segreta di Instagram" è necessario cliccare sul pulsante
> "Mostra" ed inserire la password del proprio account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_12.bmp](./assets/media/image240.png)

> Una volta inseriti in Passweb i due parametri di configurazione
> richiesti cliccare sul pulsante "**Salva**" presente nella parte bassa
> della maschera.

13. Arrivati a questo punto e completata l'integrazione tra le due
    piattaforme per terminare il processo sarà necessario effettuare
    altre piccole configurazioni all'interno della propria App dovute,
    essenzialmente, al fatto che, appena creta, questa sarà in modalità
    di sviluppo e per renderla effettivamente utilizzabile dovremo poi
    pubblicarla.

> Tornare quindi all'interno della sezione "**Impostazioni -- Di Base**"
> e verificare di aver inserito correttamente tutti i dati richiesti
> (punto 5)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_2.bmp](./assets/media/image229.png)

14. Per poter pubblicare l'app sarà necessario per prima cosa sottoporla
    alla validazione da parte di Facebook. Per questo sarà necessario
    portarsi all'interno della pagina "**Basic Display**" e cliccare sul
    pulsante "**Invia per l'analisi**" posto all'interno della sezione
    "Analisi dell'App per Instagram Basic Display" precedentemente
    analizzata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_13.bmp](./assets/media/image241.png)

> **ATTENZIONE!** Il pulsante "Invia per l'analisi" si abiliterà solo
> nel momento in cui tutti i dati richiesti (tra cui anche un video che
> mostra il funzionamento dell'app e l'utilizzo dei relativi permessi di
> login) saranno stati correttamente inseriti
>
> Ottenuta la validazione da parte di Facebook, per pubblicare l'app
> sarà poi sufficiente agire mediante l'apposito pulsante di switch
> posto nella parte alta della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_14.bmp](./assets/media/image242.png)

Prima di pubblicare definitivamente la nostra App potrebbe essere utile
effettuare anche alcuni test di corretto funzionamento in maniera tale
da verificare la possibilità di accedere al nostro sito Passweb
utilizzando un profilo Instagram

Per far questo è necessario:

1.  Accedere alla pagina "**Basic Display**" dell'app appena creata,
    portarsi all'interno della sezione "**User Token Generator**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_15.bmp](./assets/media/image243.png)

> e cliccare sul pulsante "**Add or Remove Instagram Testers**". In
> questo modo verremo infatti ricondotti automaticamente all'interno
> della pagina Ruoli dove avremo la possibilità di creare gli utenti di
> test di cui abbiamo bisogno

2.  All'interno della pagina "**Ruoli**" portarsi quindi in
    corrispondenza della sezione "**Tester di Instagram**" (parte bassa
    della pagina)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_16.bmp](./assets/media/image244.png)

> cliccare sul pulsante "**Aggiungi Tester di Instagram**" e inserire
> nella successiva maschera lo username dell'utente Instagram che si
> vuole invitare come utente di test della nostra app

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_17.bmp](./assets/media/image245.png)

3.  L'utente Instagram invitato come tester potrà gestire e accettare
    l'invito all'interno della sezione "**App e siti web**" del proprio
    profilo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_18.bmp](./assets/media/image246.png)

4.  Una volta approvato l'invito l'utente comparirà all'interno della
    sezione Tester di Instagram

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_19.bmp](./assets/media/image247.png)

> e potrà quindi provare ad effettuare l'autenticazione al nostro sito
> Ecommerce con il proprio account anche se l' App è ancora in modalità
> di sviluppo

5.  A questo punto potremo quindi aprire il sito Passweb e scegliere di
    effettuare l'autenticazione utilizzando il profilo Instagram

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_20.bmp](./assets/media/image248.png)

6.  Cliccando sul relativo pulsante presente in corrispondenza del
    pannello di Login l'utente verrà quindi ricondotto alla pagina di
    accesso al social network dove dovrà ovviamente inserire le
    credenziali del proprio account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_21.bmp](./assets/media/image249.png)

> Volendo è anche possibile effettuare prima l'accesso ad Instagram,
> aprire poi in un altro tab del browser il sito Passweb ed effettuare
> l'autenticazione mediante Instagram; in questo caso non verrà
> richiesto di inserire nuovamente le credenziali di accesso alla
> piattaforma social.

7.  In ogni caso una volta inserite le credenziali verrà richiesto il
    permesso di accedere alle informazioni del proprio account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login_instagram_22.bmp](./assets/media/image250.png)

> Cliccando quindi sul pulsante "**Autorizza**" verremo automaticamente
> ricondotti al sito Passweb dove potremo verificare l'avvenuto accesso
> (e conseguentemente l'avvenuta registrazione) del nuovo utente di
> test.

**ATTENZIONE!** **Lasciando l'App in modalità Test i soli utenti
abilitati ad accedere al sito Passweb mediante il loro profilo Instagram
saranno i tester appositamente creati**

Per maggiori informazioni relativamente al componente "Login Utente" e a
come configurarlo per abilitare agli utenti la possibilità di accedere
al sito mediante il proprio profilo social si veda anche la sezione
"*Live Editing -- Lista Componenti Interazione Utente -- Componenti
Interni ai componenti interazione utente -- Social Login*" di questo
manuale.

