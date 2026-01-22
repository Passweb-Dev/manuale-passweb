# CONFIGURAZIONE -- PARAMETRI STORE



La sezione "**Parametri Store**" presente all'interno del tab
"**Configurazione**", visualizzata solo dopo aver inserito e salvato le
chiavi di configurazione necessarie per l'integrazione Passweb -- Clerk,
consente di impostare alcuni parametri di fondamentale importanza per il
corretto funzionamento di quelli che saranno poi i moduli Clerk
(Ricerca, Raccomandazioni, Chat ...) implementati all'interno del
proprio sito Ecommerce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_parametri_store.bmp](./assets/media/image8.png){width="5.409027777777778in"
height="3.584722222222222in"}

Nello specifico il campo:

**Codice di tracciamento**: consente di inserire lo snippet di codice
necessario per inizializzare e configurare Clerk.js la libreria
javascript di Clerk utilizzata per

- Caricare i moduli di Clerk (Search, Recommendations, Email, Audience)

- Tracciare il comportamento utente in tempo reale (click,
  visualizzazioni, ricerche ...)

- Inviare eventi a Clerk.io per la personalizzazione dinamica

- ...

**ATTENZIONE!** Considerando che un buon 90% dell'integrazione tra
Passweb e Clerk avviene lato client, la libreria **Clerk.js è di fatto
il cuore di tutta l'integrazione**. In conseguenza di ciò **se, per una
qualsiasi ragione, lo script inserito all'interno di questo campo non
dovesse essere caricato ed eseguito in maniera corretta** (perché ad
esempio genera degli errori, o semplicemente perché è stato sottoposto a
consenso preventivo e l'utente non ha accettato i relativi cookie) la
libreria Clerk.js non potrà essere caricata e, di conseguenza, i moduli
Clerk (Ricerca, Raccomandazioni, Chat ...) eventualmente presenti
all'interno non potranno più funzionare

Il pulsante "**Seleziona un segnaposto**" presente immediatamente al di
sopra dell'editor di codice consente di personalizzare lo script di
configurazione utilizzando uno dei segnaposto messi a disposizione da
Passweb. Nello specifico:

- **Chiave Pubblica** -- consente di inserire il segnaposto
  **{clerk_public_key}** che verrà poi sostituito a runtime con il
  valore della chiave pubblica inserita in corrispondenza del campo "Api
  Key" precedentemente analizzato

- **Visitor_pwb** -- consente di inserire il segnaposto
  **{clerk_visitor_type}** che verrà poi sostituito a runtime con il
  valore *visitor: null* oppure con *visitor: 'xxxxxxxxxxxxxxxx'* (dove
  'xxxxxxxxxxxxxxxx' è una stringa univoca di 16 caratteri generata da
  Passweb) a seconda del fatto che l'utente abbia o meno prestato il
  consenso per l'utilizzo dei cookie analitici.

Lo snippet di codice da inserire all'interno di questo campo può essere
prelevato direttamente dal proprio account Clerk all'interno della
sezione "**Developers -- Tracking Code**" dello store con cui si
desidera effettuare l'integrazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_tracking_code.bmp](./assets/media/image9.png){width="5.370138888888889in"
height="3.33125in"}

Va detto però che lo script prelevabile dalla sezione sopra evidenziata,
viene fornito da Clerk in una versione "base" dove cioè l'unico
parametro di configurazione indicato in maniera esplicita è la chiave
pubblica, come si può effettivamente notare dall'istruzione

*Clerk(\'config\', {*

*key: \'xxxxxxxxxxxxxxxxxxx\'*

*});*

In questo senso la prima cosa da sottolineare è che tale chiave potrebbe
essere inserita nello script di configurazione anche utilizzando il
segnaposto "Chiave Pubblica" precedentemente analizzato e quindi nel
formato

*Clerk(\'config\', {*

***key: \'{clerk_public_key}\'***

*});*

In questo modo se, per una qualsiasi ragione, dovesse essere necessario
cambiare la chiave pubblica sarebbe sufficiente inserire la nuova
all'interno del campo "Api Key" della sezione "Credenziali" e il nuovo
valore verrebbe automaticamente inserito poi anche nello script di
configurazione di Clerk.js

Oltre al parametro **key** è possibile utilizzare, in maniera esplicita,
anche altri parametri di configurazione, alcuni dei quali molto
importanti e che possono modificare il funzionamento della libreria
Clerk.js e di conseguenza anche il funzionamento di tutta l'integrazione
tra Passweb e Clerk.

Tra questi, due parametri particolarmente importanti da prendere in
considerazione, soprattutto in ottica GDPR, sono indubbiamente il
parametro **visitor** e il parametro **collect_email**

- **visitor**: determina il modo in cui verrà generato memorizzato e
  utilizzato l'identificativo di ogni visitatore influenzando, di
  conseguenza, il sistema di tracciamento messo in atto da Clerk e
  quello che dovrà o non dovrà essere indicato nelle varie informative
  Privacy e Cookie Policy del sito.

> Clerk gestisce 4 diverse possibili opzioni per il parametro visitor:

- *visitor: 'auto'* -- opzione di default

> **ATTENZIONE!** nel momento in cui lo script di configurazione di
> Clerk dovesse essere inserito senza un impostazione esplicita per il
> parametro visitor, verrà automaticamente attivata l'opzione *visitor:
> 'auto'*

- *visitor: 'persistent'*

- *visitor: null*

- *visitor: Custom*

<!-- -->

- **collect_email**: consente di decidere se Clerk dovrà o meno
  raccogliere in maniera automatica, durante la sessione di navigazione,
  l'indirizzo e-mail dell'utente. Nello specifico l'impostazione:

  - **collect_email**: false -- opzione di default

> Impedisce a Clerk di raccogliere in maniera automatica l'indirizzo
> email dell'utente
>
> **ATTENZIONE!** nel momento in cui lo script di configurazione di
> Clerk dovesse essere inserito senza un impostazione esplicita per il
> parametro collect_email, verrà automaticamente attivata l'opzione
> *collect_email: false*

- **collect_email**: true

> Consente a Clerk di raccogliere in maniera automatica l'indirizzo
> email dell'utente

Nell'ipotesi di voler utilizzare la modalità Custom per il parametro
visitor e di voler consentire a Clerk di raccogliere in maniera
automatica la mail dell'utente durante la sua sessione di navigazione
(opzioni queste che possono essere assolutamente consigliate) lo script
di configurazione da inserire all'interno del campo "Codice di
tracciamento" dovrà dunque essere il seguente

*\<!\-- Start of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

*\<script type=\"text/javascript\"\>*

*(function(w,d){*

*var
e=d.createElement(\'script\');e.type=\'text/javascript\';e.async=true;*

*e.src=\'https://cdn.clerk.io/clerk.js\';*

*var
s=d.getElementsByTagName(\'script\')\[0\];s.parentNode.insertBefore(e,s);*

*w.\_\_clerk_q=w.\_\_clerk_q\|\|\[\];w.Clerk=w.Clerk\|\|function(){w.\_\_clerk_q.push(arguments)};*

*})(window,document);*

*Clerk(\'config\', {*

***key: \'{clerk_public_key}\'**,*

***collect_email: true,***

***{clerk_visitor_type}***

*});*

*\</script\>*

*\<!\-- End of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

Per maggior informazioni relativamente a tutti i possibili parametri di
configurazione di Clerk.js si consiglia di fare sempre riferimento alla
specifica documentazione di prodotto disponibile, ad esempio, ai
seguenti link
<https://help.clerk.io/it/integrations/any-webshop/clerkjs/> -
<https://docs.clerk.io/docs/clerkjs-configuration>

Per maggiori informazioni invece relativamente a come le diverse
impostazioni dei parametri *visitor* e *collect_email* andranno ad
impattare effettivamente sul funzionamento dell'integrazione Passweb --
Clerk e sul GDPR, si rimanda anche a quanto indicato nel successivo
capitolo "*Passweb Clerk -- Privacy e GDPR*" di questo manuale

**ATTENZIONE!** il fatto di poter inserire liberamente lo script di
configurazione di Clerk.js all'interno del campo "**Codice di
tracciamento**" offre piena libertà all'amministratore del sito che, di
fatto, può personalizzare questo stesso script attivando o disattivando
specifiche funzionalità dell'integrazione, secondo quelle che sono le
sue specifiche esigenze

D'altra parte questa libertà richiede anche una certa consapevolezza
relativamente al funzionamento di Clerk oltre che specifiche conoscenze
tecniche (si ricorda infatti che eventuali errori nello script di
configurazione andranno a pregiudicare il corretto funzionamento di
tutta l'integrazione). In caso di dubbi relativamente alla
configurazione di Clerk.js il consiglio è quindi sempre quello di
rivolgersi direttamente all'assistenza Clerk (e nel caso poi anche
all'assistenza Passweb).

**Valuta**: consente di indicare, selezionandola tra quelle gestite
all'interno del sito, la specifica valuta da utilizzare per il calcolo
dei prezzi degli articoli che verranno poi inseriti all'interno del
relativo feed e pubblicati quindi anche all'interno di Clerk

**Lingua**: consente di indicare, selezionandola tra quelle gestite
all'interno del sito, la lingua di riferimento per la lettura dei valori
dei campi articolo che verranno poi inseriti all'interno del relativo
feed. A seconda dunque della lingua indicata all'interno di questo campo
nel feed articoli verranno inserite informazioni in italiano o in
lingua.

Ovviamente la lingua indicata all'interno di questo campo dovrà
corrispondere a quella dello store Clerk con cui si sta effettuando
l'integrazione

**ATTENZIONE!** È possibile creare un solo account per ogni lingua
gestita

Per maggiori informazioni relativamente all'integrazione Passweb --
Clerk nel caso di siti multilingua si veda anche quanto indicato nel
relativo capitolo ("*Passweb e Clerk -- Integrazione -- Multilingua*")
di questo manuale

**Categoria Sconto Cliente**: consente di indicare la specifica
"Categoria Sconto Cliente" (selezionandola tra quelle definite
all'interno del gestionale) che dovrà essere presa in considerazione
nella determinazione del prezzo degli articoli che verranno poi inseriti
all'interno del relativo feed e pubblicati quindi anche all'interno di
Clerk

**Pulisci Chat al Logout Utente**: consente, se selezionato, di azzerare
la Chat Clerk eventualmente implementata all'interno del sito
(eliminando quindi tutti i messaggi in essa presenti) nel momento in cui
l'utente dovesse effettuare il log out

**ATTENZIONE!** considerando che la Chat di Clerk, se attivata, salva un
"id conversazione" in session storage del browser, nel caso in cui si
dovesse decidere di non selezionare questo parametro i messaggi
eventualmente presenti in chat resteranno sempre visibili fintanto che
non verrà chiuso il browser o i singoli tab utilizzati dall'utente per
navigare il sito

**Account di default**: consente di impostare l'account in esame come
Account di default. Tale parametro è collegato, essenzialmente, alla
gestione dei siti multilingua. In questo caso, infatti, il consiglio
(come indicato anche da Clerk stesso nella sua documentazione) è quello
di creare uno store per ogni lingua del sito e, conseguentemente, anche
un Account Clerk per singola lingua all'interno di Passweb.

In questo modo ordini e clienti condivisi con Clerk verranno smistati,
in base alla loro lingua, sul relativo store e, nel caso in cui
dovessero esserci ordini o clienti con associata una lingua diversa da
quelle gestite (per cui dunque non è stato impostato né uno store Clerk
né il corrispondente account all'interno di Passweb) questi verranno
automaticamente assegnati allo store di default

Per maggiori informazioni relativamente all'integrazione Passweb --
Clerk nel caso di siti multilingua si veda anche quanto indicato nel
relativo capitolo ("*Passweb e Clerk -- Integrazione -- Multilingua*")
di questo manuale

**Attributo Opt-Out**: consente di indicare, selezionandolo da un
apposito menu a tendina, quello che dovrà poi essere utilizzato come
attributo di Opt-Out per Clerk.

L'attributo indicato dovrà essere un attributo cliente di tipo Testo e
dovrà poi essere inserito anche sul front end del sito, all'interno dei
moduli di Registrazione / Profilo Utente mediante l'utilizzo di un
componente "**Campo Checkbox**"

**ATTENZIONE!** il parametro in esame non è obbligatorio ma è comunque
vivamente consigliato gestirlo in maniera corretta

Per maggiori informazioni in merito alla gestione dell'Opt-Out di Clerk
si veda anche quanto indicato all'interno del capitolo "*Passweb e Clerk
-- Privacy e GDPR -- Gestione del Visitor Id -- Opzione di Opt-Out*" di
questo manuale

