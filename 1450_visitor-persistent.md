# VISITOR: 'PERSISTENT'



Utilizzando questa impostazione (*visitor: 'persistent'*) i visitatori
del sito verranno tracciati attraverso ID di sessione anonimi generati
sempre da Clerk utilizzando esattamente lo stesso algoritmo del caso
precedente.

**A differenza però dell'impostazione visitor:'auto', in questo caso
l'ID di sessione verrà salvato anche in local storage nel browser
dell'utente** (con la chiave "clerk-visitor-id") e questo porterà
ovviamente ad alcune conseguenze, sia positive che negative, che
dovranno per forza di cose essere tenute in debita considerazione nel
momento in cui si dovesse decidere di utilizzare questa impostazione.

**In questo senso, innanzitutto, il fatto di salvare dei dati nel
browser dell'utente fa scattare, oltre a tutto il resto (informativa
chiara ed esplicita sull'utilizzo della piattaforma, catalogazione dei
cookie utilizzati ...), anche la necessità di un consenso preventivo.**

Relativamente al GDPR infatti il salvataggio di dati in local storage è
accomunabile all'utilizzo dei cookie di terza parte per cui potrà
avvenire solo dopo che l'utente ha prestato l'apposito consenso.

Dal punto di vista tecnico questo significa quindi che **lo script di
configurazione di Clerk, e di conseguenza tutto il funzionamento dei
relativi moduli implementati all'interno del sito (ricerca,
raccomandazioni, chat ...) dovrà essere sottoposto allo stesso blocco
preventivo che va applicato, ad esempio a sistemi come Google Analytics,
MailChimp, Active Campaign...**

Ora, considerando che tale script non è gestito nativamente da Passweb
ma deve essere inserito direttamente dall'amministratore del sito
all'interno del campo "**Codice di tracciamento**" (sezione "**Parametri
Store**" nel tab "**Configurazione**" della maschera "**Dati Account**")

![](./assets/media/image69.png)

dovrà essere cura dell'amministratore stesso fare in modo che la sua
attivazione sia effettivamente condizionata all'accettazione dei cookie
da parte dell'utente che sta navigando il sito.

In questo senso, come già visto per servizi analoghi, la soluzione
migliore è indubbiamente quella di ricorrere all'utilizzo di apposite
piattaforme CMP (es. Iubenda, Cookiebot ...) e, nello specifico, alla
loro opzione di tagging manuale per vari script presenti all'interno del
sito (posto ovviamente che la piattaforma CMP utilizzata offra
effettivamente questa possibilità).

Nel caso di Iubenda, ad esempio, si potrebbe inserire lo script di
configurazione di Clerk modificandolo come di seguito indicato

*\<!\-- Start of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

*\<script **type= "text/plain" class="\_iub_cs_activate"**
**data-iub-purposes="4"**\>*

*(function(w,d){*

*var
e=d.createElement(\'script\');e.type=\'text/javascript\';e.async=true;*

*e.src=\'https://cdn.clerk.io/clerk.js\';*

*var
s=d.getElementsByTagName(\'script\')\[0\];s.parentNode.insertBefore(e,s);*

*w.\_\_clerk_q=w.\_\_clerk_q\|\|\[\];w.Clerk=w.Clerk\|\|function(){w.\_\_clerk_q.push(arguments)};*

*})(window,document);*

*Clerk(\'config\', {*

*key: '{clerk_public_key}',*

***visitor:'persistent'**,*

*collect_email:true*

*});*

*\</script\>*

*\<!\-- End of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

dove

- **type="text-plain"** evita che lo script venga trattato come tale e
  quindi eseguito al caricamento della pagina

- **class="\_iub_cs_activate"** è la classe che iubenda utilizza nelle
  sue procedure di tagging manuale per identificare gli script inline
  che dovranno poi essere attivati nel momento in cui l'utente avrà
  prestato i relativi consensi

- **data-iub-purposes="4"** consente di gestire il consenso per
  categoria di Iubenda e, nello specifico, di attivare lo script nel
  momento in cui l'utente avrà prestato il consenso 4 ovvero consenso
  statistico

In questo modo dunque, sarà Iubenda stesso in maniera completamente
automatica a preoccuparsi di modificare lo script in maniera tale che
possa effettivamente essere eseguito e possa quindi iniziare a
funzionare solo dopo che l'utente abbia prestato i giusti consensi.

Allo stesso modo sarà sempre Iubenda a preoccuparsi, ancora una volta in
maniera completamente automatica, di disabilitare questo stesso script
(riportandolo esattamente nelle condizioni in cui lo abbiamo inserito)
nel momento in cui un utente che aveva precedentemente prestato il
consenso dovesse, ad un certo punto, cambiare idea e modificare quindi
le sue preferenze agendo ovviamente dal banner dei consensi messo a
disposizione da Iubenda

Per maggiori informazioni in merito alle opzioni di tagging manuale si
veda anche quanto indicato nel capitolo "GDPR Gestione e blocco
preventivo dei cookie -- Blocco Preventivo -- Iubenda" di questo manuale
o, meglio ancora, alla relativa documentazione della piattaforma CMP
effettivamente utilizzata (es.
<https://www.iubenda.com/it/help/674-tagging-manuale-blocco-cookie> )

**ATTENZIONE!** in queste condizioni, nel momento in cui l'utente
dovesse decidere, per una qualsiasi ragione, di non prestare l'apposito
consenso, lo script di configurazione di Clerk non verrà attivato e, di
conseguenza, non verranno attivati neppure eventuali moduli (ricerca,
raccomandazioni, chat ...) implementati all'interno del sito

In conseguenza di ciò, ovviamente, si può anche evitare di inserire
l'opzione di Opt-out nel modulo di Registrazione / Profilo Utente
inquanto la volontà di non essere tracciati da Clerk può già essere
espressa mediante il Cookie Banner.

Oltre al fatto di dover condizionare l'utilizzo dei moduli Clerk
all'accettazione dei cookie un altro aspetto "negativo" legato
all'utilizzo dell'opzione *visitor: 'persistent'* è rappresentato dal
fatto che, come detto, l'algoritmo utilizzato per la generazione dell'id
di sessione è lo stesso utilizzato anche nel caso di *visitor: 'auto'*.

Come nel caso precedente quindi, anche questa volta, **qualsiasi
visitatore che dovesse navigare sullo stesso sito, dalla stessa rete,
con lo stesso tipo di dispositivo e utilizzando anche lo stesso browser,
si troverà di fatto a condividere lo stesso ID di sessione già
utilizzata da un altro utente** (con tutto ciò che ne consegue).

Per quel che riguarda invece i vantaggi che si possono ottenere con
l'impostazione *visitor: 'persistent'* va evidenziato, da una parte, il
fatto di poter implementare un tracciamento di lunga durata. In queste
condizioni infatti il valore del visitor id salvato in local storage
avrà una durata superiore ai 30 giorni previsti dall'opzione 'auto' per
cui sarà effettivamente possibile tracciare il comportamento dell'utente
(posto che utilizzi ovviamente lo stesso dispositivo, lo stesso browser
e che abbia prestato i relativi consensi) su di un arco temporale più
lungo.

Dall'altra parte il fatto di poter accedere al valore del visitor id
salvato in local storage fa si che questo stesso valore possa essere
riutilizzato anche nelle chiamate server effettuate alle API di Clerk.

In questo senso infatti nel momento in cui l'utente dovesse prestare i
relativi consensi, Passweb si preoccuperà di creare un apposito cookie
di prima parte denominato anch'esso '*clerk-visitor-id*' e settato sul
valore dell'omonima chiave presente in local storage.

Il valore presente all'interno di questo cookie, corrispondente di fatto
al visitor id utilizzato nelle chiamate lato client di Clerk, potrà
quindi essere utilizzato anche nelle chiamate server alle API delle
Raccomandazioni incentrate sul visitatore permettendoci di implementare
queste stesse Raccomandazioni utilizzando, a differenza di quanto
avveniva nel caso di *visitor: 'auto'*, il componente "Popolarità
Prodotto" ed essendo sicuri che gli articoli presenti al suo interno
siano effettivamente coerenti con i dati di navigazione dello specifico
utente.

**ATTENZIONE! anche in questo caso il consiglio è sempre quello di
verificare direttamente con il supporto Clerk o con il proprio DPO che
la soluzione adottata sia effettivamente conforme a quanto richiesto dal
GDPR**

