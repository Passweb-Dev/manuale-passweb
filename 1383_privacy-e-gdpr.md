# PRIVACY E GDPR



**ATTENZIONE**! quanto indicato all'interno di questo manuale in merito
all'utilizzo e alla configurazione di Matomo non costituisce un parere
legalmente valido per cui prima di attivare o disattivare determinate
funzionalità e per essere sicuri di operare in maniera conforme a quanto
previsto dal GDPR, **si consiglia di fare sempre riferimento a quanto
espressamente indicato dal Garante e/o dalle figure deputate (DPO), per
il proprio sito, alla gestione della Privacy e di tutto ciò che le ruota
attorno**

**ATTENZIONE! Passepartout non è in alcun modo responsabile in merito
all'utilizzo o meno, in maniera conforme a quanto previsto dal GDPR, di
strumenti di terze parti come possono essere Googla Analytics, Matomo,
Facebook ...**

Come già evidenziato nei precedenti capitoli di questo manuale il
principale vantaggio di Matomo rispetto a Google Analytics (almeno allo
stato attuale delle cose) è indubbiamente quello di poter utilizzare
questo strumento in maniera conforme a quanto previsto dal GDPR. Questo
non vuol dire però che Matomo può, a prescindere, essere non soggetto a
tutto quanto richiesto dal GDPR.

**Anche Matomo dovrà infatti essere pur sempre configurato e settato in
un certo modo per poter essere effettivamente conforme a tutto quanto
previsto dal GDPR**

In questo senso i punti chiave da prendere in considerazione sono
essenzialmente due:

- la proprietà dei dati raccolti con Matomo

- la richiesta di consenso agli utenti prima di attivare la raccolta dei
  dati e la tipologia di dati raccolti

Per quel che riguarda il primo punto (al momento non risolvibile con
GA4) non ci sono grossi problemi nel senso che con **Matomo la proprietà
e l'accesso ai dati resta sotto l'esclusivo controllo di chi li
raccoglie** **e questo indipendentemente dal fatto di utilizzare
un'istallazione Matomo in Cloud oppure On Premise.**

In particolare, nel momento in cui si dovesse optare per
un'installazione di **Matomo in Cloud** i server utilizzati per
memorizzare i dati sarebbero quelli dell'azienda stessa, localizzati in
Europa (nello specifico in Francia) e quindi in tutto e per tutto
conformi a quanto previsto dal GDPR Europeo. Considerando inoltre che
l'azienda che sviluppa Matomo non è in alcun modo partecipata da società
Americane non c'è neppure il rischio di dover trasferire i dati raccolti
negli Stati Uniti o comunque in un paese in cui la gestione della
privacy non è in linea con quanto effettivamente richiesto dall'Europa
(a differenza invece di quello che avviene con Google Analytics che pur
raccogliendo i dati in server Europei si troverebbe comunque costretta,
dietro specifica richiesta del governo americano, a trasferire i dati
negli Stati Uniti)

Nel momento in cui si dovesse optare invece per un'installazione di
**Matomo On Premise** il tutto dipenderà ovviamente da dove sarà
localizzato il server utilizzato per installare Matomo e quindi per
raccogliere i dati. Va da se che, in queste condizioni, se anche
dovessimo raccogliere dati in Europa ma il server utilizzato per
installare Matomo dovesse essere localizzato in USA ci ritroveremmo
esattamente nelle stesse condizioni di Google Analytics andando quindi
incontro ad una violazione del GDPR perché i dati raccolti verrebbero
effettivamente trasferiti negli Stati Uniti.

In definitiva raccogliendo dati in Europa e installando Matomo su di un
server Europeo potremo essere sicuri, almeno sotto questo aspetto, di
essere conformi a quanto previsto dal GDPR.

Sotto questo aspetto, in realtà, i problemi da prendere in
considerazione sarebbero poi altri e riguarderebbero principalmente
l'assunzione di responsabilità legale in merito ad eventuali data breach
sul server utilizzato per installare Matomo e contenente quindi i dati
degli utenti.

Per quel che riguarda il secondo punto, ossia la richiesta di consenso
agli utenti prima di attivare la raccolta dei dati e la tipologia di
dati raccolti, occorre invece fare riferimento alle modalità di
funzionamento di Matomo.

Come evidenziato anche nei precedenti capitoli di questo manuale
infatti, di base, il tracciamento di quello che succede all'interno del
sito con Matomo viene effettuato lato client (via Javascript) con
l'installazione nel browser dei visitatori di appositi cookie che,
dipendentemente dalla tipologia di dati raccolti, potranno poi essere
classificati come cookie analitici/statistici oppure come cookie di
marketing/profilazione

**ATTENZIONE!** Ai seguenti indirizzi
<https://matomo.org/blog/2020/02/web-analytics-cookies-gdpr/>
<https://matomo.org/faq/general/faq_146/> è possibile trovare maggiori
informazioni in merito ai cookie utilizzati da Matomo

Sotto questo aspetto dunque anche Matomo è soggetto esattamente agli
stessi vincoli e agli stessi obblighi imposti dal GDPR, in merito alla
gestione dei cookie, cui è sottoposto lo stesso Google Analytics e
quindi possiamo giustamente affermare **che non è assolutamente legale
installare cookie Matomo sul browser degli utenti prima che questi
abbiano prestato il loro consenso**.

Come noto infatti la sentenza della Corte di giustizia del 2019 (Az.:
C-673/17) prevede che venga richiesto un consenso esplicito all'utente
prima di poter effettivamente installare sul suo browser un qualsiasi
tipo di cookie che non sia tecnicamente obbligatorio e quindi
indispensabile per un corretto funzionamento del sito. Tutto ciò che va
oltre il funzionamento essenziale del sito (quindi cookie analitici,
cookie di marketing ...) richiede un consenso **esplicito e preventivo**
da parte dell'utente.

In definitiva dunque nel momento in cui dovessimo utilizzare Matomo per
attivare una raccolta di dati (indipendentemente dal fatto che siano o
meno dati personali degli utenti) basata sull'utilizzo dei cookie senza
prima richiedere il consenso agli utenti e senza portarli a conoscenza,
nelle varie informative presenti sul sito, dei dati che verranno
raccolti e dell'utilizzo che ne faremo, **saremmo in palese violazione
di quanto previsto e richiesto dal GDPR**.

Compreso ciò il punto fondamentale diventa ora quello di capire come
poter gestire, anche nel caso di Matomo, le richieste di consenso
preventivo e, in questo senso, le cose non sono poi così diverse da
Google Analytics.

Anche in questo caso infatti una possibile soluzione potrebbe essere
quella di ricorrere all'utilizzo di apposite piattaforme CMP (es.
Iubenda, Cookiebot ...) facendo attenzione al fatto di:

- inserire nelle informative da esse generate l'utilizzo di Matomo come
  piattaforma di web analytics

- classificare i cookie utilizzati da Matomo come cookie
  analitici/statistici o marketing/profilazione in base alla tipologia
  di dati che andremo effettivamente a raccogliere

- configurare il blocco preventivo dello script di Matomo per essere
  certi di attivare il tracciamento e iniziare a raccogliere i dati solo
  dopo che l'utente abbia effettivamente prestato il proprio consenso
  all'utilizzo di quella specifica tipologia di cookie

Un'altra possibile soluzione, limitata però al solo utilizzo di Matomo,
potrebbe anche essere quella di utilizzare il form di Opt Out (standard
o customizzato) disponibile tra i vari strumenti di gestione della
Privacy messi a disposizione da Matomo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_9.bmp](./assets/media/image9.png)

e le relative chiamate API per una corretta gestione delle richieste di
consenso

**ATTENZIONE! Questo tipo di soluzione è limitata esclusivamente
all'utilizzo di Matomo e ai cookie da esso installati.**

Ciò significa che nel momento in cui all'interno del sito dovessero
essere utilizzati anche altri strumenti di tracciamento che fanno uso di
cookie (es. Facebook, Google Ads ...) questi dovranno necessariamente
essere bloccati in maniera preventiva mediante strumenti appositi
(piattaforme CMP) che nulla hanno a che vedere con il form di Opt Out di
Matomo

Per maggiori informazioni in merito alla gestione del form di Opt Out di
Matomo si veda anche quanto indicato nel relativo capitolo ("*Matomo --
Privacy e GDPR -- Opt Out Utenti*") di questo manuale

Infine, un'ultima considerazione molto interessante da fare, in merito
sempre all'utilizzo dei cookie, è che volendo gestire questo tipo di
tracciamento, dal punto di vista delle modalità di installazione di
Matomo, la soluzione migliore è indubbiamente quella On Premise. In
questo modo infatti, associando all'installazione Matomo un sottodominio
del dominio principale in uso al sito, sarà possibile far sì che i
cookie installati da Matomo siano trattati come cookie di prima parte
con tutti i vantaggi del caso (allo stesso modo di quello che avviene ad
esempio per il tracciamento server side di GTM)

In generale comunque il problema relativo all'utilizzo dei banner di
consenso è rappresentato, ovviamente, da tutti quegli utenti che
potrebbero negare il proprio consenso all'utilizzo dei cookie privando
dunque gli amministratori del sito di tutta una serie di dati che
fondamentali per avere sempre un quadro chiaro di quello che è il reale
andamento del sito e dei relativi obiettivi di business.

Da questo punto di vista le cose andavano decisamente meglio quando era
consentito tracciare gli utenti senza la necessità di richiedere un
consenso preventivo e sotto questo aspetto Matomo può aiutare gli
amministratori del sito in maniera indubbiamente maggiore di quanto non
riesca a fare Google Analytics.

Matomo dispone infatti di tutta una serie di parametri di configurazione
grazie ai quali poter attivare ad esempio un tracciamento cookieless
(senza cioè l'utilizzo di cookie) e un anonimizzazione dei dati che, in
determinate condizioni, potrebbero anche portare a tracciare gli utenti
senza richiedere il consenso e restando comunque conformi a quanto
richiesto dal GDPR

Nei successivi capitoli di questo manuale verranno analizzati
rapidamente i principali parametri di configurazioni e le impostazioni
disponibili per rendere la propria installazione di Matomo conforme al
GDPR nelle diverse possibili situazioni.

**ATTENZIONE!** Per maggiori informazioni in merito alla gestione della
privacy in Matomo si consiglia di fare sempre riferimento alla
documentazione ufficiale disponibile, ad esempio, al seguente link
<https://matomo.org/faq/general/configure-privacy-settings-in-matomo/>

