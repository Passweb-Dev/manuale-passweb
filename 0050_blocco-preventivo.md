# BLOCCO PREVENTIVO



La sezione "**Blocco Preventivo**" consente di decidere come dovrà
essere gestito il blocco preventivo dei cookie, anche in relazione
all'utilizzo della Consent Mode e ovviamente alla specifica piattaforma
CMP che si è deciso di utilizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_integrazioni_blocco_cookie_1.bmp](./assets/media/image175.png){width="5.740277777777778in"
height="3.623611111111111in"}

In questo senso è bene sottolineare che, al momento, è possibile
integrare con il proprio sito Passweb una delle seguenti piattaforme
CMP:

- Iubenda

- CookieBot

- One Trust

I parametri presenti all'interno di questa sezione consentono quindi di:

**Blocco Preventivo dei Cookie:** consente di decidere se ed
eventualmente come gestire il blocco preventivo dei cookie in relazione
all'utilizzo della Consent Mode e relativamente anche ai componenti
nativi di Passweb (per i quali l'utente non ha modo di intervenire sul
relativo codice sorgente) che potrebbero effettivamente rilasciare
cookie di profilazione o di terze parti prima che l'utente abbia
espresso il relativo consenso.

È possibile selezionare una delle seguenti opzioni:

- **No**: selezionando questa opzione non verrà attivato nessun blocco
  preventivo dei cookie e, conseguentemente, non verrà attivata neppure
  la gestione della Consent Mode.

> In queste condizioni quindi eventuali script di tracciamento verranno
> eseguiti sempre e comunque rilasciando tutti i cookie di cui hanno
> bisogno
>
> **ATTENZIONE! questa opzione rende il sito non compliance con quanto
> richiesto dal GDPR**

- **Iubenda + Consent Mode (v2 Avanzata):** selezionando questa opzione
  verrà attivata la Consent Mode di Iubenda in modalità Avanzata e sarà
  quindi necessario inserire lo snippet di codice fornito da Iubenda
  stessa all'interno del successivo campo "**Code Snippet Cookie**" e
  impostare anche un valore di default per i vari consensi (sezione
  "**Valori Consent Default**")

> Per maggiori informazioni su quello che è il funzionamento della
> Consent Mode in modalità Avanzata e su cosa comporta questa scelta si
> faccia riferimento a quanto indicato anche nel relativo capitolo di
> questo manuale ("*Google Analytics -- Consent Mode -- Tipologie di
> Consent Mode -- Consent Mode Avanzata*")
>
> In queste condizioni sarà inoltre di fondamentale importanza:

- **Accertarsi di non avere attivato su Iubenda l'autoblocking.** In
  caso contrario infatti lo snippet di codice fornito da Iubenda
  andrebbe a bloccare tutti gli script presenti sul sito compresi quelli
  indispensabili per il corretto funzionamento del sito stesso

- **Eliminare dallo snippet di codice fornito da Iubenda, prima di
  inserirlo all'interno del relativo campo Passweb (Code Snippet
  Cookie), il seguente scritp**

> *\<script type=\"text/javascript\"
> src=\"//cs.iubenda.com/sync/XXXX.js\"\>\</script\>*
>
> Dove XXXX è un numero identificato del proprio account Iubenda.
>
> Tale script, se inserito in Passweb, demanderebbe infatti la gestione
> del valore di default dei vari consensi direttamente a Iubenda andando
> quindi a sovrascrivere eventuali impostazioni settate in questo senso
> direttamente all'interno di Passweb (per maggiori informazioni in
> merito all'integrazione "Passweb -- Iubenda" si veda anche quanto
> indicato all'interno del capitolo "*GDPR Gestione e blocco preventivo
> dei cookie -- Blocco Preventivo -- Iubenda*" di questo manuale)

- **Iubenda + Consent Mode (v2 Base):** selezionando questa opzione
  verrà attivata la Consent Mode di Iubenda in modalità Base e sarà
  quindi necessario inserire lo snippet di codice fornito da Iubenda
  stessa all'interno del successivo campo "**Code Snippet Cookie**"

> Per maggiori informazioni su quello che è il funzionamento della
> Consent Mode in modalità Base e su cosa comporta questa scelta si
> faccia riferimento a quanto indicato anche nel relativo capitolo di
> questo manuale ("*Google Analytics -- Consent Mode -- Tipologie di
> Consent Mode -- Consent Mode Avanzata*")
>
> In queste condizioni sarà inoltre di fondamentale importanza:

- **Accertarsi di non avere attivato su Iubenda l'autoblocking.** In
  caso contrario infatti lo snippet di codice fornito da Iubenda
  andrebbe a bloccare tutti gli script presenti sul sito compresi quelli
  indispensabili per il corretto funzionamento del sito stesso

- **Eliminare dallo snippet di codice fornito da Iubenda, prima di
  inserirlo all'interno del relativo campo Passweb (Code Snippet
  Cookie), il seguente scritp**

> *\< script type=\"text/javascript\"
> src=\"//cs.iubenda.com/sync/XXXX.js\"\>\</script\>*
>
> Dove XXXX è un numero identificato del proprio account Iubenda.
>
> Tale script, se inserito in Passweb, demanderebbe infatti la gestione
> del valore di default dei vari consensi direttamente a Iubenda andando
> quindi a sovrascrivere il valore di default impostato da Passweb per i
> vari consensi, valore questo che come precedentemente indicato, in
> queste condizioni sarà sempre "Denied" e non potrà essere modificato
> (per maggiori informazioni in merito all'integrazione "Passweb --
> Iubenda" si veda anche quanto indicato all'interno del capitolo "*GDPR
> Gestione e blocco preventivo dei cookie -- Blocco Preventivo --
> Iubenda*" di questo manuale).

- **Cookiebot:** selezionando questa opzione il blocco preventivo dei
  cookie verrà demandato interamente a Cookiebot
  (<https://www.cookiebot.com> )

> Per maggiori informazioni in merito a quelle che sono le operazioni da
> effettuare per consentire a Cookiebot di bloccare correttamente cookie
> di profilazione o di terze parti prima che l'utente abbia espresso il
> proprio consenso si rimanda a quanto indicato all'interno del capitolo
> "*GDPR Gestione e blocco preventivo dei cookie -- Blocco Preventivo --
> Cookiebot*" di questo manuale

- **Cookiebot + Consent Mode (v2):** consente di attivare la gestione
  della Google Consent Mode in collaborazione con i servizi offerti
  dalla piattaforma di Cookiebot. Tale opzione va quindi selezionata
  solo ed esclusivamente nel momento in cui si sia effettivamente deciso
  di utilizzare, oltre a CookieBot, anche la Google Consent Mode

> **ATTENZIONE!** Per maggiori informazioni relativamente alla Consent
> Mode, a come funziona, a quelli che sono i vantaggi a cui potrebbe
> portare una sua corretta implementazione e a come poterla
> effettivamente implementare sfruttando l'integrazione diretta tra
> Passweb, Analytics e CookieBot si rimanda anche a quanto indicato
> nella sezione "*Google Analytics -- Consent Mode*" di questo manuale.

- **OneTrust**: selezionando questa opzione il blocco preventivo dei
  cookie verrà demandato interamente alla piattaforma OneTrust
  (<https://www.onetrust.it/> )

> Per maggiori informazioni in merito a quelle che sono le operazioni da
> effettuare per consentire a OneTrust di bloccare correttamente cookie
> di profilazione o di terze parti prima che l'utente abbia espresso il
> proprio consenso si rimanda a quanto indicato all'interno del capitolo
> "*GDPR Gestione e blocco preventivo dei cookie -- Blocco Preventivo --
> OneTrust*" di questo manuale

**ATTENZIONE! indipendentemente dal fatto di demandare il blocco
preventivo ad un servizio terzo piuttosto che ad un altro l'impostazione
di questo parametro, da sola, potrebbe non bastare a bloccare
effettivamente tutti i cookie rilasciati dal proprio sito.**

Nel momento in cui si dovesse decidere infatti di implementare
l'integrazione con un qualunque altro servizio di terze parti che
dovesse far uso di cookie non strettamente tecnici (es. Hotjar, Pulsanti
social, live chat ...), l'amministratore del sito dovrà preoccuparsi di
attivare, anche in merito a questi stessi servizi, il blocco preventivo
dei cookie effettuando, ad esempio, apposite operazioni di tagging
manuale

In questo senso una cosa di fondamentale importanza da tenere sempre in
considerazione è il fatto che quasi tutte le piattaforme CMP offrono, in
fase di configurazione, due diverse modalità di blocco dei cookie:

- **Autoblocking** (Blocco automatico): in questo caso la piattaforma
  terza andrà a scansionare il sito web per individuare eventuali script
  o elementi presenti all'interno delle varie pagine che potrebbero
  rilasciare dei cookie e, in relazione ad essi, attiverà
  automaticamente il blocco preventivo (disabilitando, ad esempio, i
  relativi script fino a che l'utente non abbia prestato i relativi
  consensi)

- **Blocco (tagging) manuale**: in questo caso è l'amministratore del
  sito che dovrà sapere esattamente quali script, plugin o elementi
  installati all'interno delle varie pagine possano effettivamente
  rilasciare dei cookie non tecnici e che dovrà quindi preoccuparsi di
  bloccarli in maniera preventiva configurandoli secondo quanto
  indicato, relativamente alle operazioni di tagging manuale, nella
  documentazione della specifica piattaforma CMP utilizzata

Ovviamente il blocco automatico potrebbe sembrare l'opzione più
semplice, ma allo stesso tempo è anche la più pericolosa inquanto in
queste condizioni la piattaforma terza potrebbe andare a bloccare dei
javascript, fondamentali per il corretto funzionamento del sito, che non
rilasciano in alcun modo cookie di profilazione e che non dovrebbero
quindi essere bloccati in alcun modo (pena il non corretto funzionamento
del sito)

In conseguenza di ciò **si consiglia di non attivare mai il blocco
automatico e di gestire, consapevolmente, il tagging manuale degli
elementi che dovranno effettivamente essere bloccati in maniera
preventiva.**

**ATTENZIONE! Passweb non può sapere a priori quali servizi di terze
parti l'utente ha deciso di attivare. Sarà compito dell'amministratore
del sito, dunque, verificare se il servizio in questione utilizzi
effettivamente dei cookie non tecnici, quali siano ed eventualmente
gestirne il blocco preventivo.**

Per maggiori informazioni relativamente a come poter gestire i cookie e
a come comportarsi per essere in regola con la vigente normativa in
materia di GDPR si veda anche quanto indicato all'interno del relativo
capitolo di questo manuale ("*GDPR -- Gestione e blocco preventivo dei
cookie*")

**Code Snippet Cookie:** consente di inserire e gestire lo script di
attivazione della piattaforma CMP (Iubenda, Cookiebot ecc ...) che si è
deciso di utilizzare e integrare all'interno del proprio sito Passweb

Lo script di integrazione dovrà essere prelevato direttamente dal
backend della specifica piattaforma CMP. Per maggiori informazioni in
merito si veda anche quanto indicato all'interno del capitolo "*GDPR
Gestione e blocco preventivo dei cookie -- Blocco Preventivo"* di questo
manuale

**ATTENZIONE!** in relazione all'utilizzo della Consent Mode in un
sistema di tracciamento diretto Sito -- Analytics (che non prevede
quindi utilizzo di Tag Manager) è di fondamentale importanza inserire lo
snippet di codice fornito dalla specifica piattaforma CMP direttamente
all'interno di questo campo. In caso contrario infatti potrebbe non
essere garantito il corretto ordine di esecuzione dei vari script cosa
questa indispensabile per fare in modo che la Consent Mode Base o
Avanzata possa operare effettivamente come deve.

**Valori Consent Default** -- visibile solo nel caso in cui si sia
deciso di implementare la Consent Mode in modalità Avanzata e quindi
solo se:

- **Blocco Preventivo dei Cookie = Iubenda + Consent Mode (v2
  Avanzata)**

- **Blocco Preventivo dei Cookie = CookieBot + Consent Mode (v2)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\analytics_valori_consent_default.bmp](./assets/media/image176.png){width="5.740277777777778in"
height="3.3506944444444446in"}

I parametri presenti all'interno di questa sezione consentono di
impostare il valore di default (Denied o Granted) per le diverse
tipologie di consenso gestite dalla Consent Mode.

Nello specifico dunque il parametro:

- **AdStorage:** consente di impostare il valore di default relativo al
  consenso **ad_storage**

- **AnalyticsStorage:** consente di impostare il valore di default
  relativo al consenso **analytics_storage**

- **FunctionalityStorage:** consente di impostare il valore di default
  relativo al consenso **functionality_storage**

- **PersonalizationStorage:** consente di impostare il valore di default
  relativo al consenso **personalization_storage**

- **AdUserData:** consente di impostare il valore di default relativo al
  consenso **ad_user_data**

- **AdPersonalization:** consente di impostare il valore di default
  relativo al consenso **ad_personalization**

- **SecurityStorage:** consente di impostare il valore di default
  relativo al consenso **security_storage**

Di base nell'implementazione della Consent Mode Avanzata tutti i
consensi sopra evidenziati dovrebbero avere il valore di default
impostato su "**Denied**" (negato). Questo garantisce infatti che gli
script di tracciamento non salvino cookie né registrino dati
identificabili salvo esplicito consenso da parte dell'utente. In queste
condizioni verranno comunque inviati a Google dei cosiddetti
**cookieless pings** ossia richieste anonime che non contengono
identificatori personali, ma forniscono informazioni di base come
l'evento avvenuto, il tipo di pagina visitata, e lo stato di consenso.

In determinate condizioni, si potrebbe anche pensare di applicare una
configurazione "forzata" dei valori di default che prevede di impostare
su "**Granted**" (consentito) il default dei consensi di
**analytics_storage** e di **security_storage**, cosa questa che
consentirebbe di raccogliere ancora più dati.

**ATTENZIONE!** in ogni caso **prima di applicare la configurazione che
prevede di impostare su "Granted" il valore di default di determinati
consensi (es. analytics_storage) è sempre bene confrontarsi con il
proprio DPO e/o con chi si occupa della questione privacy del sito in
modo tale da essere certi di rimanere comunque compliance con quanto
richiesto dal GDPR.**

Inoltre nel caso in cui si dovesse decidere di implementare la Consent
Mode Avanzata settando direttamente su Passweb il valore di default dei
vari consensi sarà fondamentale accertarsi del fatto che tali valori non
siano poi eventualmente sovrascritti dalla stessa piattaforma CMP.

**ATTENZIONE!** nel momento in cui si dovesse invece decidere di
implementare la Consent Mode in modalità Base, la sezione "Valori
Consent Default" non verrà visualizzata, il valore di default dei vari
consensi verrà impostato automaticamente da Passweb su "Denied" e non
potrà essere modificato

Per maggiori informazioni relativamente al significato di ciascuno dei
consensi sopra indicati e a cosa comporti effettivamente il fatto di
impostarli a default su "Denied" piuttosto che su "Granted" in relazione
all'utilizzo della Consent Mode Avanzata o Base si veda anche quanto
indicato all'interno del capitolo "*Google Analytics -- Consent Mode*"
di questo manuale.

