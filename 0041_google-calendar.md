# GOOGLE CALENDAR



La sezione **Google Calendar** presente alla voce "*Sito -- Preferenze
-- Integrazioni*" del Wizard consente di impostare i parametri necessari
per l'integrazione tra l'Agenda, presente nell'Area Riservata del
proprio sito, e Google Calendar

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_configurazione_1.bmp](./assets/media/image95.png){width="5.532638888888889in"
height="3.584722222222222in"}

Una volta impostati correttamente questi parametri di configurazione,
gli utenti abilitati ad accedere all'Area Riservata del sito potranno
poi decidere (mediante l'attivazione di un apposito parametro) di fare
in modo che, da quel momento in avanti, ogni attività gestita nella
propria agenda venga riportata automaticamente anche all'interno del
loro calendario Google.

**ATTENZIONE!** L'integrazione è **monodirezionale**, **dal Sito Passweb
verso il Calendario di Google**. Eventuali modifiche apportate ad
attività direttamente dal calendario di Google non verranno quindi
riportate nell'Agenda dell'Area Riservata

Per maggiori informazioni relativamente alla gestione dell'Agenda in
Area Riservata e a come abilitare il trasferimento delle attività sui
calendari di Google si veda anche quanto indicato all'interno del
relativo capitolo di questo manuale ("*Siti Ecommerce Area Riservata e
B2B -- Agenda*")

Per ottenere le chiavi da inserire all'interno dei campi evidenziati in
figura è necessario invece seguire passo passo la procedura qui di
seguito indicata:

1.  Accedere all'indirizzo <https://console.developers.google.com>
    utilizzando il proprio account Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login23.bmp](./assets/media/image70.png){width="5.013194444444444in"
height="2.8375in"}

2.  Aprire il menu a tendina posizionato nella parte alta della pagina e
    creare poi un nuovo progetto cliccando sulla relativa voce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login71.bmp](./assets/media/image71.png){width="5.220833333333333in"
height="2.8569444444444443in"}

3.  Una volta avviata la creazione di un nuovo progetto sarà necessario
    assegnargli un nome (es. Google Calendar) e cliccare poi sul
    pulsante **Crea**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login25.bmp](./assets/media/image72.png){width="5.090972222222222in"
height="2.714583333333333in"}

4.  Completata la creazione del progetto accedere alla sezione
    "**Libreria**" cliccando per questo sulla relativa voce di menu
    presente sulla sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_gmap_6.bmp](./assets/media/image73.png){width="5.00625in"
height="3.1819444444444445in"}

5.  Selezionare quindi, tra quelle presenti in Libreria, le api relative
    a **Google Calendar** (cercandole eventualmente mediante l'apposito
    campo di ricerca)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_1.bmp](./assets/media/image96.png){width="5.311805555555556in"
height="3.0194444444444444in"}

> e successivamente cliccare sul pulsante "**Abilita**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_2.bmp](./assets/media/image97.png){width="5.090972222222222in"
height="2.714583333333333in"}

6.  Una volta abilitate le API di cui al punto precedente, aprire il
    menu di navigazione cliccando sul relativo pulsante presente nella
    parte alta della pagina e selezionare la voce "**API e servizi -
    Credenziali**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_gmap_6c.bmp](./assets/media/image76.png){width="5.00625in"
height="3.1819444444444445in"}

7.  Verificare innanzitutto di aver configurato correttamente la
    schermata di consenso e, se questo non fosse già stato fatto,
    cliccare sul relativo pulsante "**Configura Schermata di Consenso**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_3.bmp](./assets/media/image98.png){width="5.090972222222222in"
height="2.714583333333333in"}

8.  In fase di configurazione della schermata di consenso impostare il
    parametro "**User Type**" sul valore "**Esterno**" e cliccare poi
    sul pulsante "**Crea**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_4.bmp](./assets/media/image99.png){width="5.090972222222222in"
height="2.714583333333333in"}

9.  Completare il successivo form inserendo i dati richiesti (nome
    dell'applicazione, email per assistenza, domini autorizzati ...) e
    cliccare poi sul pulsante "**Salva e Continua**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_5.bmp](./assets/media/image100.png){width="5.090972222222222in"
height="3.467361111111111in"}

> **ATTENZIONE!** l'inserimento di alcuni dati (es. logo
> dell'applicazione) potrebbe poi richiedere, prima di passare in
> produzione, la validazione dell'App da parte di Google.

10. Nel successivo step ("**Ambiti**") cliccare sul pulsante "**Salva e
    Continua**" posto nella parte bassa della pagina senza aggiungere
    altro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_6.bmp](./assets/media/image101.png){width="5.090972222222222in"
height="3.545138888888889in"}

> **ATTENZIONE!** E' comunque necessario aver attivato correttamente le
> API di Google Calendar come descritto al punto 5

11. Nello step relativo alla creazione degli utenti di prova aggiungere,
    se necessario, l'account Google di eventuali utenti che potranno
    provare l'integrazione tra l'Agenda dell'Area Riservata e il loro
    Google Calendar nel momento in cui lo stato dell'app che stiamo
    realizzando dovesse essere ancora "**Test in corso**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_7.bmp](./assets/media/image102.png){width="5.090972222222222in"
height="3.545138888888889in"}

> **ATTENZIONE!** Per consentire a tutti gli utenti del sito di
> sfruttare l'integrazione tra l'Agenda in Area Riservata e il loro
> Google Calendar senza visualizzare eventuali messaggi di sicurezza,
> sarà necessario ovviamente portare l'App in produzione sottoponendola,
> se richiesto, alla verifica da parte di Google
>
> Una volta aggiunti gli eventuali utenti di prova cliccare ancora una
> volta sul pulsante "**Salva e Continua**" e successivamente nella
> maschera di riepilogo cliccare su "**Torna alla Dashboard**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_8.bmp](./assets/media/image103.png){width="5.090972222222222in"
height="3.545138888888889in"}

12. Completata la creazione della schermata di consenso la nostra App
    sarà ancora nello stato "**Test in corso**" per cui, in queste
    condizioni solo eventuali utenti di test appositamente creati
    potranno effettivamente testare l'integrazione tra l'Agenda del sito
    e il loro calendario google.

> Per modificare lo stato dell'App sarà sufficiente cliccare sul
> pulsante "**Pubblica l'App**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_9.bmp](./assets/media/image104.png){width="5.325in"
height="3.545138888888889in"}

> **ATTENZIONE!** Dipendentemente dai dati inseriti la pubblicazione
> dell'App potrebbe essere soggetta a verifica da parte di Google.
>
> In ogni caso, portando l'App in produzione senza sottoporla alla
> verifica da parte di Google, nel momento in cui l'utente dovesse poi
> tentare di attivare, sul front end del sito, il salvataggio delle
> attività in Agenda anche sul calendario di Google, verrà avvisato,
> attraverso un apposito messaggio, che l'App in esame non è ancora
> stata verificata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_18.bmp](./assets/media/image105.png){width="5.49375in"
height="3.2597222222222224in"}

> In queste condizioni è comunque possibile procedere attivando
> l'integrazione in maniera tale che il messaggio evidenziato non sia
> più visualizzato.
>
> **E' comunque consigliato, per ovvie ragioni, di inserire sempre tutti
> i dati richiesti dalla schermata di consenso dell'App e di mandare
> questa stessa App in revisione a Google in maniera tale da evitare la
> visualizzazione di messaggi che potrebbero spaventare gli utenti del
> sito**.

13. Arrivati a questo punto è possibile passare alla creazione delle
    chiavi di integrazione da inserire poi nei relativi campi del Wizard
    di Passweb.

> Portarsi quindi all'interno della sezione "Credenziali" cliccando per
> questo sulla relativa voce di menu posta sulla sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_10.bmp](./assets/media/image106.png){width="5.325in"
height="3.545138888888889in"}

14. Cliccare quindi sulla voce "**Crea Credenziali**" e successivamente
    sulla voce "**ID client OAuth**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_11.bmp](./assets/media/image107.png){width="5.325in"
height="3.545138888888889in"}

15. Compilare la successiva maschera di creazione delle credenziali come
    di seguito indicato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_12.bmp](./assets/media/image108.png){width="5.325in"
height="3.545138888888889in"}

- **Tipo di applicazione**: selezionare "**Applicazione web**"

- **Nome**: nome descrittivo del client Oauth2 che stiamo configurando

16. Cliccare sul pulsante "**Aggiungi URI**" presente in corrispondenza
    della sezione "**URI di reindirizzamento autorizzati**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_13.bmp](./assets/media/image109.png){width="5.325in"
height="3.545138888888889in"}

> successivamente, inserire nel relativo campo di input il seguente
> indirizzo
>
> <https://www.dominiosito.it/AreaRiservata/Strumenti/Profilo/CallbackOAuthGoogle>
>
> e cliccare, infine sul pulsante "**Crea**"

17. Terminata la creazione del client OAuth verrà visualizzata una
    maschera contenente le due chiavi di configurazione da inserire
    all'interno del proprio sito Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_14.bmp](./assets/media/image110.png){width="5.325in"
height="3.545138888888889in"}

> Copiare quindi il contenuto dei campi "**Il tuo ID client**" e "**Il
> tuo client secret**" ed inserirlo rispettivamente all'interno dei
> campi "**ID Client Google Calendar**" e "**Client Secret Google
> Calendar**" presenti alla pagina "*Sito -- Preferenze --
> Integrazioni*" del Wizard (sezione Google Calendar).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_configurazione_1.bmp](./assets/media/image95.png){width="5.532638888888889in"
height="3.584722222222222in"}

A questo punto, nel momento in cui un utente del sito abilitato ad
accedere in Area Riservata, dovesse andare nella pagina di gestione del
suo profilo troverà, all'interno della sezione "**Opzioni Agenda**", il
pulsante "**Sign in with Google"** con l'indicazione relativa al fatto
che l'integrazione con il calendario di Google non è ancora stata
attivata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_15.bmp](./assets/media/image111.png){width="5.701388888888889in"
height="3.5in"}

**ATTENZIONE!** il pulsante "**Sign in with Google"** verrà visualizzato
solo dopo aver inserito correttamente, nel Wizard di Passweb, le chiavi
di configurazione relative a Google Calendar

Cliccando sul pulsante evidenziato in figura verrà chiesto all'utente di
autenticarsi con il proprio account Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_16.bmp](./assets/media/image112.png){width="5.597222222222222in"
height="3.4090277777777778in"}

Posto quindi che l'app di integrazione sia stata creata in maniera
corretta e che si stata anche appositamente verificata da parte di
Google, una volta inserite le credenziali del proprio account verrà
mostrata la schermata di consenso che l'utente dovrà approvare (pulsante
"**Conferma**") per poter così attivare l'integrazione tra le due
piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_20.bmp](./assets/media/image113.png){width="5.49375in"
height="3.2597222222222224in"}

**ATTENZIONE!** Nel caso in cui l'app di integrazione su Google dovesse
essere ancora nello stato di "**Test in corso**" o, pur essendo "**In
Produzione**" non dovesse ancora essere stata verificata da Google
potrebbero essere visualizzati specifici messaggi di errore e/o di
avviso

In particolare, nel caso in cui:

- L'app di integrazione dovesse essere ancora nello stato di "**Test in
  Corso**" (si veda il punto 12 della procedura precedentemente
  descritta) verrà visualizzato un messaggio di errore e, di fatto, sarà
  impossibile per l'utente salvare le attività in agenda nel relativo
  calendario di google (a meno che non sia uno degli utenti di test
  appositamente creati)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_17.bmp](./assets/media/image114.png){width="5.434722222222222in"
height="3.2597222222222224in"}

- Nel caso in cui l'app di integrazione pur essendo posta nello stato
  "**In Produzione**" non sia stata ancora inviata a Google per la
  verifica, verrà visualizzato un apposito messaggio di warning per
  informare l'utente di questo fatto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_18.bmp](./assets/media/image105.png){width="5.49375in"
height="3.2597222222222224in"}

> In queste condizioni l'utente potrebbe comunque procedere cliccando su
> "**Avanzate**" e successivamente su "**Apri
> [www.urlsito.it](http://www.urlsito.it)**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_19.bmp](./assets/media/image115.png){width="5.49375in"
height="3.2597222222222224in"}

> in maniera tale da accedere comunque alla schermata di consenso che
> dovrà essere correttamente approvata (pulsante "**Continua**") per
> garantire l'integrazione tra le due piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_19b.bmp](./assets/media/image116.png){width="5.597222222222222in"
height="3.4090277777777778in"}

Una volta pubblicata l'app di integrazione e concesse tutte le
autorizzazioni del caso l'integrazione tra l'Agenda Passweb e i
Calendari Google dello specifico utente sarà terminata.

Tornando quindi nella pagina di profilo dell'utente troveremo ora
l'indicazione di avvenuta connessione ed il pulsante "**Disconnetti**"
da utilizzare nel momento in cui si dovesse decidere di non utilizzare
più questa integrazione e di limitare il salvataggio di nuove attività
sulla propria Agenda Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_calendar_connesso.bmp](./assets/media/image117.png){width="5.701388888888889in"
height="3.5in"}

Da questo momento in avanti in fase di creazione di nuovi calendari
all'interno della propria Agenda Passweb, sarà possibile indicare anche
l'id del calendario google su cui sincronizzare le nuove attività che
verranno inserite su quello stesso calendario

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_calendario_id_google_calendar.bmp](./assets/media/image118.png){width="2.9611111111111112in"
height="1.792361111111111in"}

Per maggiori informazioni relativamente all'utilizzo dell'Agenda
disponibile in Area Riservata Passweb e alla sua integrazione con Google
Calendar si veda anche quanto indicato nel relativo capitolo di questo
manuale ("*Siti Ecommerce -- Area Riservata e B2B -- Agenda*")

