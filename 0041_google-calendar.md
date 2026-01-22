# GOOGLE CALENDAR



La sezione **Google Calendar** presente alla voce "*Sito -- Preferenze
-- Integrazioni*" del Wizard consente di impostare i parametri necessari
per l'integrazione tra l'Agenda, presente nell'Area Riservata del
proprio sito, e Google Calendar

![](./assets/media/image95.png)

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

![](./assets/media/image70.png)

2.  Aprire il menu a tendina posizionato nella parte alta della pagina e
    creare poi un nuovo progetto cliccando sulla relativa voce

![](./assets/media/image71.png)

3.  Una volta avviata la creazione di un nuovo progetto sarà necessario
    assegnargli un nome (es. Google Calendar) e cliccare poi sul
    pulsante **Crea**

![](./assets/media/image72.png)

4.  Completata la creazione del progetto accedere alla sezione
    "**Libreria**" cliccando per questo sulla relativa voce di menu
    presente sulla sinistra della pagina

![](./assets/media/image73.png)

5.  Selezionare quindi, tra quelle presenti in Libreria, le api relative
    a **Google Calendar** (cercandole eventualmente mediante l'apposito
    campo di ricerca)

![](./assets/media/image96.png)

> e successivamente cliccare sul pulsante "**Abilita**"

![](./assets/media/image97.png)

6.  Una volta abilitate le API di cui al punto precedente, aprire il
    menu di navigazione cliccando sul relativo pulsante presente nella
    parte alta della pagina e selezionare la voce "**API e servizi -
    Credenziali**"

![](./assets/media/image76.png)

7.  Verificare innanzitutto di aver configurato correttamente la
    schermata di consenso e, se questo non fosse già stato fatto,
    cliccare sul relativo pulsante "**Configura Schermata di Consenso**"

![](./assets/media/image98.png)

8.  In fase di configurazione della schermata di consenso impostare il
    parametro "**User Type**" sul valore "**Esterno**" e cliccare poi
    sul pulsante "**Crea**"

![](./assets/media/image99.png)

9.  Completare il successivo form inserendo i dati richiesti (nome
    dell'applicazione, email per assistenza, domini autorizzati ...) e
    cliccare poi sul pulsante "**Salva e Continua**"

![](./assets/media/image100.png)

> **ATTENZIONE!** l'inserimento di alcuni dati (es. logo
> dell'applicazione) potrebbe poi richiedere, prima di passare in
> produzione, la validazione dell'App da parte di Google.

10. Nel successivo step ("**Ambiti**") cliccare sul pulsante "**Salva e
    Continua**" posto nella parte bassa della pagina senza aggiungere
    altro

![](./assets/media/image101.png)

> **ATTENZIONE!** E' comunque necessario aver attivato correttamente le
> API di Google Calendar come descritto al punto 5

11. Nello step relativo alla creazione degli utenti di prova aggiungere,
    se necessario, l'account Google di eventuali utenti che potranno
    provare l'integrazione tra l'Agenda dell'Area Riservata e il loro
    Google Calendar nel momento in cui lo stato dell'app che stiamo
    realizzando dovesse essere ancora "**Test in corso**"

![](./assets/media/image102.png)

> **ATTENZIONE!** Per consentire a tutti gli utenti del sito di
> sfruttare l'integrazione tra l'Agenda in Area Riservata e il loro
> Google Calendar senza visualizzare eventuali messaggi di sicurezza,
> sarà necessario ovviamente portare l'App in produzione sottoponendola,
> se richiesto, alla verifica da parte di Google
>
> Una volta aggiunti gli eventuali utenti di prova cliccare ancora una
> volta sul pulsante "**Salva e Continua**" e successivamente nella
> maschera di riepilogo cliccare su "**Torna alla Dashboard**"

![](./assets/media/image103.png)

12. Completata la creazione della schermata di consenso la nostra App
    sarà ancora nello stato "**Test in corso**" per cui, in queste
    condizioni solo eventuali utenti di test appositamente creati
    potranno effettivamente testare l'integrazione tra l'Agenda del sito
    e il loro calendario google.

> Per modificare lo stato dell'App sarà sufficiente cliccare sul
> pulsante "**Pubblica l'App**" evidenziato in figura

![](./assets/media/image104.png)

> **ATTENZIONE!** Dipendentemente dai dati inseriti la pubblicazione
> dell'App potrebbe essere soggetta a verifica da parte di Google.
>
> In ogni caso, portando l'App in produzione senza sottoporla alla
> verifica da parte di Google, nel momento in cui l'utente dovesse poi
> tentare di attivare, sul front end del sito, il salvataggio delle
> attività in Agenda anche sul calendario di Google, verrà avvisato,
> attraverso un apposito messaggio, che l'App in esame non è ancora
> stata verificata.

![](./assets/media/image105.png)

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

![](./assets/media/image106.png)

14. Cliccare quindi sulla voce "**Crea Credenziali**" e successivamente
    sulla voce "**ID client OAuth**" evidenziata in figura

![](./assets/media/image107.png)

15. Compilare la successiva maschera di creazione delle credenziali come
    di seguito indicato

![](./assets/media/image108.png)

- **Tipo di applicazione**: selezionare "**Applicazione web**"

- **Nome**: nome descrittivo del client Oauth2 che stiamo configurando

16. Cliccare sul pulsante "**Aggiungi URI**" presente in corrispondenza
    della sezione "**URI di reindirizzamento autorizzati**"

![](./assets/media/image109.png)

> successivamente, inserire nel relativo campo di input il seguente
> indirizzo
>
> <https://www.dominiosito.it/AreaRiservata/Strumenti/Profilo/CallbackOAuthGoogle>
>
> e cliccare, infine sul pulsante "**Crea**"

17. Terminata la creazione del client OAuth verrà visualizzata una
    maschera contenente le due chiavi di configurazione da inserire
    all'interno del proprio sito Passweb

![](./assets/media/image110.png)

> Copiare quindi il contenuto dei campi "**Il tuo ID client**" e "**Il
> tuo client secret**" ed inserirlo rispettivamente all'interno dei
> campi "**ID Client Google Calendar**" e "**Client Secret Google
> Calendar**" presenti alla pagina "*Sito -- Preferenze --
> Integrazioni*" del Wizard (sezione Google Calendar).

![](./assets/media/image95.png)

A questo punto, nel momento in cui un utente del sito abilitato ad
accedere in Area Riservata, dovesse andare nella pagina di gestione del
suo profilo troverà, all'interno della sezione "**Opzioni Agenda**", il
pulsante "**Sign in with Google"** con l'indicazione relativa al fatto
che l'integrazione con il calendario di Google non è ancora stata
attivata

![](./assets/media/image111.png)

**ATTENZIONE!** il pulsante "**Sign in with Google"** verrà visualizzato
solo dopo aver inserito correttamente, nel Wizard di Passweb, le chiavi
di configurazione relative a Google Calendar

Cliccando sul pulsante evidenziato in figura verrà chiesto all'utente di
autenticarsi con il proprio account Google

![](./assets/media/image112.png)

Posto quindi che l'app di integrazione sia stata creata in maniera
corretta e che si stata anche appositamente verificata da parte di
Google, una volta inserite le credenziali del proprio account verrà
mostrata la schermata di consenso che l'utente dovrà approvare (pulsante
"**Conferma**") per poter così attivare l'integrazione tra le due
piattaforme

![](./assets/media/image113.png)

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

![](./assets/media/image114.png)

- Nel caso in cui l'app di integrazione pur essendo posta nello stato
  "**In Produzione**" non sia stata ancora inviata a Google per la
  verifica, verrà visualizzato un apposito messaggio di warning per
  informare l'utente di questo fatto

![](./assets/media/image105.png)

> In queste condizioni l'utente potrebbe comunque procedere cliccando su
> "**Avanzate**" e successivamente su "**Apri
> [www.urlsito.it](http://www.urlsito.it)**"

![](./assets/media/image115.png)

> in maniera tale da accedere comunque alla schermata di consenso che
> dovrà essere correttamente approvata (pulsante "**Continua**") per
> garantire l'integrazione tra le due piattaforme

![](./assets/media/image116.png)

Una volta pubblicata l'app di integrazione e concesse tutte le
autorizzazioni del caso l'integrazione tra l'Agenda Passweb e i
Calendari Google dello specifico utente sarà terminata.

Tornando quindi nella pagina di profilo dell'utente troveremo ora
l'indicazione di avvenuta connessione ed il pulsante "**Disconnetti**"
da utilizzare nel momento in cui si dovesse decidere di non utilizzare
più questa integrazione e di limitare il salvataggio di nuove attività
sulla propria Agenda Passweb

![](./assets/media/image117.png)

Da questo momento in avanti in fase di creazione di nuovi calendari
all'interno della propria Agenda Passweb, sarà possibile indicare anche
l'id del calendario google su cui sincronizzare le nuove attività che
verranno inserite su quello stesso calendario

![](./assets/media/image118.png)

Per maggiori informazioni relativamente all'utilizzo dell'Agenda
disponibile in Area Riservata Passweb e alla sua integrazione con Google
Calendar si veda anche quanto indicato nel relativo capitolo di questo
manuale ("*Siti Ecommerce -- Area Riservata e B2B -- Agenda*")

