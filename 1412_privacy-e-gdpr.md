# PRIVACY E GDPR



Come già evidenziato nei precedenti capitoli di questo manuale anche
Brainlead (così come Google Analytics, Matomo o Facebook) deve essere
considerato a tutti gli effetti come un sistema di tracciamento e
profilazione degli utenti e, come tale, deve quindi sottostare alla
normativa vigente in materia di Privacy e GDPR.

Anche in questo caso dunque i punti chiave da prendere in considerazione
sono sempre due:

- La collocazione dei dati

- La richiesta di consenso agli utenti prima di attivare effettivamente
  la raccolta dei dati

Per quel che riguarda il primo punto non ci sono grossi problemi, nel
senso che Brainlead è una società con sede in Italia (i dati non escono
quindi dalla Comunità Europea) in tutto e per tutto conforme a quanto
richiesto e previsto dal GDPR Europeo.

Per quel che riguarda il secondo punto, ossia la richiesta di consenso
agli utenti prima di attivare la raccolta dei dati, occorre invece fare
riferimento alle modalità di funzionamento di Brainlead.

In questo senso, come evidenziato nel precedente capitolo di questo
manuale, il sistema di tracciamento messo in piedi da Brainlead funziona
sia lato client (via Javascript) con l'installazione nel browser dei
visitatori di appositi cookie (che dovranno essere classificati come
cookie di marketing / profilazione), che lato server mediante apposite
chiamate API controllate e validate dall'utilizzo di una specifica API
Key

Per quel che riguarda il tracciamento lato client dunque anche Brainlead
è soggetto esattamente agli stessi vincoli e agli stessi obblighi GDPR,
cui è sottoposto, ad esempio, anche lo stesso Google Analytics. In
conseguenza di ciò possiamo giustamente affermare **che non è
assolutamente legale installare cookie Brainlead sul browser degli
utenti prima che questi abbiano prestato il loro esplicito consenso**

Come noto infatti la sentenza della Corte di giustizia del 2019 (Az.:
C-673/17) prevede che venga richiesto un consenso esplicito all'utente
prima di poter effettivamente installare sul suo browser un qualsiasi
tipo di cookie che non sia tecnicamente obbligatorio e quindi
indispensabile per un corretto funzionamento del sito. Tutto ciò che va
oltre il funzionamento essenziale del sito (quindi cookie analitici,
cookie di marketing ...) richiede un consenso **esplicito e preventivo**
da parte dell'utente.

In definitiva dunque nel momento in cui dovessimo inviare dei dati a
Brainlead senza prima richiedere il consenso agli utenti e senza
portarli a conoscenza, nelle varie informative presenti sul sito, dei
dati che verranno raccolti e dell'utilizzo che ne faremo, **saremmo in
palese violazione di quanto previsto e richiesto dal GDPR**.

Compreso ciò il punto fondamentale diventa, al solito, quello di capire
come poter gestire, anche nel caso di Brainlead, le richieste di
consenso preventivo e, in questo senso, le cose non sono poi così
diverse da Google Analytics, Matomo o Facebook.

Anche in questo caso infatti la soluzione migliore è indubbiamente
quella di ricorrere all'utilizzo di apposite piattaforme CMP (es.
Iubenda, Cookiebot ...) facendo attenzione al fatto di:

- inserire nelle informative da esse generate l'utilizzo di Brainlead
  come piattaforma di marketing automation

- classificare i cookie utilizzati da Brainlead come cookie
  marketing/profilazione

- configurare il blocco preventivo dello script di Brainlead per essere
  certi di attivare il tracciamento e iniziare a raccogliere i dati solo
  dopo che l'utente abbia effettivamente prestato il proprio consenso
  all'utilizzo di quella specifica tipologia di cookie

In merito a quest'ultimo punto è bene ricordare che lo script di
tracciamento richiesto da Brainlead è gestito nativamente in Passweb e
quindi come altri script analoghi (Google Analytics, Facebook ...) è
controllato dal parametro "**Blocco preventivo dei cookie**" presente
alla pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento
Dati**", sezione "**Blocco Preventivo**").

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\brainlead_blocco_preventivo.bmp](./assets/media/image6.png)

Per maggiori informazioni in merito al parametro in oggetto si veda
anche quanto indicato all'interno dei relativi capitoli di questo
manuale ("*Sito -- Preferenze -- Tracciamento Dati -- Blocco
Preventivo*" e "*GDPR Gestione e blocco preventivo dei cookie*")

**ATTENZIONE!** nel momento in cui si dovesse decidere di gestire il
blocco preventivo dei cookie con una piattaforma CMP diversa da quelle
integrabili con Passweb, potrebbe poi essere necessario modificare
manualmente lo script di tracciamento di Brainlead per applicare in
maniera corretta il blocco preventivo. In tal senso si consiglia sempre
di fare riferimento alla documentazione della specifica piattaforma CMP
che si è deciso di utilizzare

Per quel che riguarda invece il tracciamento lato server, rientriamo
anche in questo caso, in un discorso più che altro di tipo etico.

Considerando infatti che, dal punto di vista tecnico il tracciamento
lato server non richiede né l'installazione di cookie sul browser
dell'utente né tanto meno l'esecuzione, sempre sul browser dell'utente,
di determinate istruzioni javascript quello che si ottiene implementando
un tracciamento di questo tipo è, da un parte, che l'utente non ha modo
di verificare di essere tracciato, perché di fatto sul suo browser non
avviene nulla, e per la stessa ragione, dall'altra parte che piattaforme
CMP come Iubenda o Cookiebot non potendo, ovviamente, intervenire sul
codice server dell'applicativo utilizzato per realizzare il sito, non
avranno modo di condizionare automaticamente il tracciamento al consenso
fornito dall'utente.

Il risultato che si ottiene dunque è che potrebbero facilmente
verificarsi situazioni in cui l'utente nega il consenso al tracciamento,
verificando anche che quanto da lui espresso sia stato effettivamente
rispettato perché non riscontra né l'installazione di cookie né tanto
meno la presenza di istruzioni atte ad inviare dati a piattaforme
esterne, poi però viene comunque tracciato a sua insaputa perché il sito
implementa anche un sistema di tracciamento lato server in maniera
"eticamente" non corretta.

Posto infatti che l'utente di per se non ha modo di verificare se è o
meno tracciato a livello server, è chiaro che se ha negato il consenso
al tracciamento, tale preferenza dovrebbe essere rispettata sotto tutti
i punti di vista per cui, in queste condizioni, dovrebbe essere
disabilitato anche un eventuale tracciamento a livello server.

In questo senso le diverse piattaforme CMP mettono a disposizione
apposite funzioni di callback da poter utilizzare per capire se e quando
l'utente ha negato il consenso al tracciamento e per bloccare di
conseguenza anche eventuali tracciamenti lato server.

Sta quindi all'applicativo utilizzato per realizzare il sito dare la
possibilità di sfruttare queste funzioni di callback per bloccare anche
un eventuale tracciamento lato server e all'etica di chi lo realizza e
lo configura fare in modo di rispettare le preferenze espresse dagli
utenti sotto tutti i punti di vista.

Detto ciò in Passweb, il parametro "**Disabilita Tracciamento Server
senza consenso**" presente alla pagina "Sito -- Preferenze" del Wizard
(tab "Tracciamento Dati", sezione "Blocco Preventivo") serve proprio ad
esplicitare quanto appena indicato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\brainlead_blocco_preventivo_server.bmp](./assets/media/image7.png)

Per maggiori informazioni in merito al parametro in oggetto si veda
anche quanto indicato all'interno del relativo capitolo di questo
manuale ("*Sito -- Preferenze -- Tracciamento Dati -- Blocco
Preventivo*")

**ATTENZIONE! Passepartout non è in alcun modo responsabile in merito
all'utilizzo o meno, in maniera conforme a quanto previsto dal GDPR, di
strumenti di terze parti come possono essere Brainlead, Google
Analytics, Matomo, Facebook ...**

