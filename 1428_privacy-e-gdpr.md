# PRIVACY E GDPR



**ATTENZIONE! Passepartout non è in alcun modo responsabile in merito
all'utilizzo o meno, in maniera conforme a quanto previsto dal GDPR, di
strumenti di terze parti come possono essere ActiveCampaign, Google
Analytics, Matomo, Facebook**

Il sistema di monitoraggio implementato da ActiveCampaign deve essere
considerato a tutti gli effetti un sistema di tracciamento e
profilazione degli utenti al pari, tanto per capirci, di Google
Analytics. Tale sistema consente infatti, grazie all'utilizzo di
appositi cookie, di raccogliere dati sulle visite effettuate al sito
identificando gli utenti in base al loro indirizzo mail, raccogliendo
tra l'altro anche l'indirizzo IP e associando questi dati ad una
specifica anagrafica presente sulla piattaforma.

Indirizzo mail e indirizzo IP sono considerati ai sensi del GDPR dati
personali perché consentono di fatto di identificare univocamente un
contatto e, in conseguenza di ciò, anche il sistema di monitoraggio di
ActiveCampaign deve sottostare alla vigente normativa in maniera di
Privacy, Cookie e GDPR.

In questo senso i punti chiave da gestire sono sempre gli stessi vale a
dire:

- Collocazione dei dati raccolti

- Informativa chiara ed esplicita agli utenti del sito relativamente
  all'utilizzo della piattaforma e al tipo di dati che verranno raccolti

- Richiesta di consenso preventivo prima di effettuare il tracciamento

Per quel che riguarda il primo punto va detto che la configurazione
multisede dalla piattaforma offre ai clienti dell'Unione Europea la
possibilità di archiviare i dati in modo sicuro in un data center
Europeo

Per quel che riguarda la necessità di informare gli utenti del sito
relativamente al tipo di dati raccolti andrà integrata la Privacy policy
e la Cookie Policy in uso al sito per indicare in maniera esplicita agli
utenti che il sito utilizza la piattaforma di ActiveCampaign e che in
conseguenza di ciò verranno installati determinati cookie e verranno
raccolti determinati dati.

Infine per quel che riguarda la richiesta di consenso preventivo sarà di
fondamentale importanza accertarsi del fatto che i cookie di
profilazione utilizzati dal sistema di monitoraggio lato client di
ActiveCampaign vengano installati nel browser dell'utente e inizino a
raccogliere i dati solo dopo che l'utente stesso abbia fornito in
maniera esplicita l'apposito consenso.

In definitiva dunque nel momento in cui dovessimo inviare dati di
tracciamento ad ActiveCampaign senza prima richiedere il consenso agli
utenti e senza portarli a conoscenza, nelle varie informative presenti
sul sito, dei dati che verranno raccolti e dell'utilizzo che ne faremo,
**saremmo in palese violazione di quanto previsto e richiesto dal
GDPR**.

Compreso ciò il punto fondamentale diventa, al solito, quello di capire
come poter gestire, anche nel caso di ActiveCampaign, le richieste di
consenso preventivo e, in questo senso, le cose non sono poi così
diverse da Google Analytics, Matomo o Facebook.

Anche in questo caso infatti la soluzione migliore è indubbiamente
quella di ricorrere all'utilizzo di apposite piattaforme CMP (es.
Iubenda, Cookiebot ...) facendo attenzione al fatto di:

- inserire nelle informative da esse generate l'utilizzo di
  ActiveCampaign come piattaforma di marketing automation

- classificare i cookie utilizzati da ActiveCampaign come cookie
  marketing/profilazione

- configurare il blocco preventivo dello script di tracciamento di
  ActiveCampaign per essere certi di attivare il tracciamento e iniziare
  a raccogliere i dati solo dopo che l'utente ha effettivamente prestato
  il proprio consenso all'utilizzo di quella specifica tipologia di
  cookie

In merito a quest'ultimo punto è bene ricordare alcune cose di
fondamentale importanza, ossia:

- lo snippet di tracciamento prelevato dal backend del proprio account
  ActiveCampaign **ha attiva l'opzione "Traccia per impostazione
  predefinita"** esemplificata dall'istruzione
  '*vgo('setTrackByDefault', true);*'

> Ciò significa che una volta caricata la pagina del sito in cui è stato
> inserito, lo script di tracciamento verrà immediatamente attivato e
> indipendentemente dal fatto che l'utente abbia o no prestato i
> consensi del caso, inizierà a tracciare e ad inviare dati ad
> ActiveCampaign e questa, come ormai dovrebbe essere chiaro, è una cosa
> assolutamente da evitare

- lo snippet di tracciamento di ActiveCampaign non è gestito nativamente
  da Passweb ma va inserito in maniera manuale, ad esempio, all'interno
  del campo "**Code Snippet -- FOOTER**" presente alla pagina "**Sito --
  Preferenze**" del Wizard (sezione "**Integrazioni**").

> In conseguenza di ciò Passweb non potrà bloccare preventivamente
> questo script (come fa invece per altri che gestisce in maniera
> nativa) e dovrà essere cura dell'amministratore del sito accertarsi di
> inserirlo in maniera corretta, ossia in modo tale che venga
> effettivamente eseguito dopo che l'utente ha prestato il relativo
> consenso e potendo anche, nel caso, fornire prova di tale
> accettazione.

Per risolvere questo problema è possibile procedere in maniera diversa
ma, come già detto, la soluzione più semplice è sicuramente quella di
utilizzare una piattaforma CMP, come può essere Iubenda o CookieBot
utilizzando uno dei metodi messi a disposizione da queste stesse
piattaforma per bloccare in maniera preventiva gli script di
tracciamento presenti sul sito.

In questo senso, ad esempio, tutte le piattaforme CMP mettono a
disposizione delle funzioni di callback che possono essere utilizzate
per implementare la soluzione indicata anche nella documentazione
ufficiale di ActiveCampaign
<https://help.activecampaign.com/hc/it/articles/360000872064-Monitoraggio-del-sito-e-GDPR#monitoraggio-del-sito-e-gdpr-0-0>

Nello specifico si potrebbe quindi pensare di:

- modificare lo snippet di tracciamento di ActiveCampaign disattivando
  l'opzione "Traccia per impostazione predefinita" e sostituendo quindi
  la riga di codice *vgo('setTrackByDefault', true);* con
  ***vgo('setTrackByDefault', false);***

- utilizzare le funzioni di callback messe a disposizione dalla
  piattaforma CMP per attivare il tracciamento solo dopo che l'utente ha
  prestato il consenso richiamando l'istruzione
  *vgo('process','allowtracking');*

- testare al caricamento della pagina il valore dei cookie installati
  dalla piattaforma CMP per capire se l'utente ha prestato il consenso e
  nel caso attivare lo snippet di tracciamento

Un alternativa, sicuramente più semplice di quella appena descritta,
potrebbe essere invece quella di utilizzare il tagging manuale dei vari
script, posto ovviamente che la piattaforma CMP utilizzata offra questa
possibilità.

Nel caso di Iubenda, ad esempio, si potrebbe inserire lo snippet di
tracciamento di ActiveCampaign nel campo "**Code Snippet -- FOOTER**"
presente alla pagina "**Sito -- Preferenze**" del Wizard, modificandolo
come di seguito indicato

***\<script type=\"text/plain\" class=\"\_iub_cs_activate \"
data-iub-purposes=\"4,5\"\>***

*(function(e,t,o,n,p,r,i){e.visitorGlobalObjectAlias=n;e\[e.visitorGlobalObjectAlias\]=e\[e.visitorGlobalObjectAlias\]\|\|function(){(e\[e.visitorGlobalObjectAlias\].q=e\[e.visitorGlobalObjectAlias\].q\|\|\[\]).push(arguments)};e\[e.visitorGlobalObjectAlias\].l=(new
Date).getTime();r=t.createElement(\"script\");r.src=o;r.async=true;i=t.getElementsByTagName(\"script\")\[0\];i.parentNode.insertBefore(r,i)})(window,document,\"https://diffuser-cdn.app-us1.com/diffuser/diffuser.js\",\"vgo\");*

*vgo(\'setAccount\', \'800260471\');*

*vgo(\'setTrackByDefault\', true);*

*vgo(\'process\');*

*\</script\>*

dove:

- **type="text-plain"** evita che lo script venga trattato come tale e
  quindi eseguito al caricamento della pagina

- **class="\_iub_cs_activate"** è la classe che iubenda utilizza nelle
  sue procedure di tagging manuale per identificare gli script inline
  che dovranno poi essere attivati nel momento in cui l'utente avrà
  prestato i relativi consensi

- **data-iub-purposes="4,5"** consente di gestire il consenso per
  categoria di Iubenda e, nello specifico, di attivare lo script nel
  momento in cui l'utente avrà prestato il consenso 3 e 4 ovvero
  consenso statistico e marketing

In questo modo dunque, sarà Iubenda stesso in maniera completamente
automatica a preoccuparsi di modificare lo script in maniera tale che
possa effettivamente essere eseguito e possa quindi iniziare a tracciare
solo dopo che l'utente ha prestato il giusti consensi per il
tracciamento.

Allo stesso modo sarà sempre Iubenda a preoccuparsi, ancora una volta in
maniera completamente automatica, di disabilitare questo stesso script
(riportandolo esattamente nelle condizioni in cui lo abbiamo inserito)
nel momento in cui un utente che aveva precedentemente prestato il
consenso dovesse, ad un certo punto, cambiare idea e modificare quindi
le sue preferenze agendo ovviamente dal banner dei consensi messo a
disposizione da Iubenda

**ATTENZIONE!** per maggiori informazioni in merito alle opzioni di
tagging manuale si veda anche quanto indicato nel capitolo *"GDPR
Gestione e blocco preventivo dei cookie -- Blocco Preventivo --
Iubenda*" di questo manuale o, meglio ancora, alla relativa
documentazione della piattaforma CMP utilizzata (es.
<https://www.iubenda.com/it/help/674-tagging-manuale-blocco-cookie> )
