# ISCRIZIONE ALLA NEWSLETTER BRAINLEAD IN FASE DI REGISTRAZIONE AL SITO



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui l'esigenza dovesse essere quella di consentire agli utenti del
sito di iscriversi alla newsletter direttamente in fase di registrazione
al sito, sarà necessario utilizzare il componente "**Newsletter
(MailChimp o BrainLead)**" inserendolo all'interno del Componente di
primo livello **Registrazione Utente** e impostando, in fase di
configurazione, il campo "**Tipo di Integrazione**" sul valore
"**Brainlead**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_brainlead.bmp](./assets/media/image156.png)

**ATTENZIONE!** a differenza di quanto avviene con MailChimp nel caso di
Brainlead il Double Opt-in, di base, non è gestito, per cui in tutti
casi una volta inserita la propria mail e confermata l'adesione al
servizio l'utente verrà immediatamente iscritto.

Una volta completata la configurazione del componente, al salvataggio,
l'applicazione si preoccuperà di contattare Brainlead, utilizzando la
relativa API Key inserita in fase di configurazione del sito,
**preleverà tutti i campi custom definiti sulla piattaforma terza e li
inserirà, assieme al campo Email, all'interno del form di Registrazione
Utente**

**ATTENZIONE!** L'unico campo custom definito su BrainLead che non verrà
inserito in maniera esplicita all'interno del form di Registrazione
Utente sarà quello dichiarato in corrispondenza del parametro di
configurazione "**Custom Field per consenso Marketing**"

Come precedentemente evidenziato tale campo sarà infatti quello
collegato al Radio Button "**Iscrizione alla Newsletter Si / No**" e, in
conseguenza di ciò, verrà utilizzato per registrare il consenso
all'iscrizione al servizio di Newsletter e alla ricezione delle mail di
carattere commerciale.

Tutti gli altri campi Custom verranno invece correttamente riportati
all'interno del form di registrazione e per ciascuno di essi sarà poi
possibile decidere se visualizzarlo o meno anche sul front end del sito.

In questo senso dunque il funzionamento è leggermente diverso rispetto a
quello che avviene per MailChimp.

Come indicato nel precedente capitolo di questo manuale infatti, nel
caso di MailChimp vengono prelevati ed inseriti all'interno del
componente Newsletter tutti e solo i campi dello specifico form di
iscrizione (**Singup form**) creato su MailChimp stesso (questo perché
le API messe a disposizione da MailChimp consentono di prelevare i campi
di uno specifico form).

In fase di configurazione su Passweb c'è poi la possibilità, come visto,
di decidere quali di questi campi visualizzare o meno sul sito e quali
eventualmente mappare con altri campi già presenti nel form di
registrazione per evitare all'utente di dover inserire la stessa
informazione due volte.

Le API messe a disposizione da Brainlead invece non consentono di
prelevare solamente i campi di uno specifico form per cui, in questo
caso, la gestione dovrà essere per forza di cose differente.

Nello specifico, verranno prelevati ed inseriti all'interno del
componente Newsletter **tutti i campi custom creati su Brainlead** e su
Passweb ci sarà come al solito la possibilità, di nascondere tali campi
(perché ad esempio non utilizzati nel form di iscrizione) o di mapparli
con eventuali altri campi già presenti nel form di registrazione per
evitare all'utente di dover inserire la stessa informazione due volte.

Per quel che riguarda **i campi "Standard" invece l'unico ad essere
inserito all'interno del componente Newsletter sarà il campo Mail**.
Tale campo potrà poi essere mappato con il campo mail già presente nel
form di registrazione oppure, volendo, si potrebbe non effettuare questa
mappatura consentendo così all'utente di indicare, in fase di iscrizione
al servizio, un indirizzo mail diverso da quello utilizzato per la
registrazione al sito.

**Tutti gli altri campi "Standard" presenti su Brainlead (es. Nome,
Cognome, Indirizzo ...) e che possono o meno essere inseriti all'interno
di qualsiasi form, verranno gestiti automaticamente da Passweb.**

Ciò significa dunque che indipendentemente dal fatto di aver inserito o
meno nel form di iscrizione costruito su Brainlead, ad esempio, il campo
Nome e il campo Cognome, questi non verranno comunque visualizzati
all'interno del componente "Newsletter", verranno però gestiti da
Passweb e collegati in automatico ai campi analoghi presenti nel form di
registrazione utente. In altri termini dunque se, all'interno del form
di registrazione utente dovessero essere presenti anche i campi Nome e
Cognome e l'utente li dovesse aver valorizzati in fase di registrazione
al sito, le relative informazioni verranno correttamente passate anche a
Brainlead

Di seguito l'elenco dei campi che, se inseriti nel form di
registrazione, verranno sempre passati anche a Brainlead (posto
ovviamente che l'utente che si registra li abbia correttamente
valorizzati):

- Nome

- Cognome

- Telefono

- Fax

- Indirizzo

- CAP

- Città

- Stato

Relativamente poi alla possibilità di mappare i campi custom di
Brainlead e/o il campo Mail con altri campi già presenti nel form di
registrazione il discorso è analogo a quello che avviene per MailChimp

Per poter effettuare questo tipo di operazione sarà quindi necessario
agire sul parametro "**Tipo di dato da rilevare**" presente nella
maschera di configurazione dei componenti interni al form di iscrizione
alla Newsletter.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione4_res.bmp](./assets/media/image153.png)

**ATTENZIONE!** Il parametro "**Tipo di dato da rilevare**" è
visualizzato tra i parametri di configurazione dei componenti interni al
form di iscrizione alla newsletter solo ed esclusivamente nel caso in
cui tale form sia inserito all'interno del componente di Registrazione
e/o di Profilo Utente.

**Tipo di dato da rilevare:** consente di decidere se il valore del
relativo campo di iscrizione alla Newsletter dovrà essere inserito
dall'utente o se dovrà essere prelevato automaticamente dal valore di un
altro campo del form di registrazione/profilo. E' possibile selezionare
uno dei seguenti valori:

- **Nessuno**: selezionando questa opzione il relativo campo del form di
  iscrizione alla newsletter verrà visualizzato e dovrà quindi essere
  compilato dall'utente nel momento in cui questo dovesse decidere di
  iscriversi anche alla Newsletter

- **Campo Cliente**: in queste condizioni il relativo campo del form di
  iscrizione alla newsletter non verrà mai visualizzato, per cui se
  l'utente dovesse decidere di iscriversi anche alla Newsletter
  l'informazione da inviare a Brainlead, in relazione a questo specifico
  campo, verrà prelevata direttamente da quanto inserito dall'utente
  stesso all'interno di un altro campo del form di registrazione.

> Il successivo parametro **Campo di Origine** consente di indicare lo
> specifico Campo Cliente da cui dover prelevare questa informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione5_res.bmp](./assets/media/image154.png)

- **Attributo Cliente**: in queste condizioni il relativo campo del form
  di iscrizione alla newsletter non verrà mai visualizzato, per cui se
  l'utente dovesse decidere di iscriversi anche alla Newsletter
  l'informazione da inviare a Brainlead, in relazione a questo specifico
  campo, verrà prelevata direttamente da quanto inserito dall'utente
  stesso all'interno di un altro campo del form di registrazione

> Il successivo parametro **Attributo di Origine** consente di indicare
> lo specifico Attributo Utente da cui dover prelevare questa
> informazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione6_res.bmp](./assets/media/image155.png)

**ATTENZIONE!** La mail di registrazione inviata all'utente a seguito
della conferma di registrazione al sito conterrà anche i campi relativi
a BrainLead solo nel caso in cui l'utente abbia effettivamente deciso di
iscriversi alla Newsletter.

Sul front end del sito, il funzionamento sarà analogo a quanto già visto
e spiegato per MailChimp.

Anche in questo caso dunque, all'interno del form di registrazione verrà
visualizzato **un Radio Button con le due opzioni Si, No mediante il
quale l'utente potrà decidere se iscriversi o meno anche alla
Newsletter**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image151.png)

Nel caso in cui l'utente dovesse decidere di registrarsi al sito senza
iscriversi alla Newsletter (opzione **No**) il campo Custom dichiarato
in corrispondenza del parametro "Custom Field per consenso Marketing"
verrà valorizzato di conseguenza (quindi a No) anche su BrainLead, e
eventuali altri campi del form di iscrizione definiti su Brainlead non
verranno mai visualizzati.

Nel momento in cui l'utente dovesse invece decidere di iscriversi anche
alla Newsletter (opzione **Si**) il campo Custom dichiarato in
corrispondenza del parametro "Custom Field per consenso Marketing" verrà
valorizzato di conseguenza (quindi a Si) anche sui BrainLead e, inoltre,
verranno anche visualizzati **i campi custom (ed eventualmente il campo
mail)** che si è deciso, in fase di configurazione, di voler
effettivamente visualizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione3.bmp](./assets/media/image152.png)

