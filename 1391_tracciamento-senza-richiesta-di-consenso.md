# TRACCIAMENTO SENZA RICHIESTA DI CONSENSO



Come più volte indicato all'interno di questo manuale, in base a quanto
previsto dal GDPR nel momento in cui si dovessero raccogliere dati di
identificazione personale e / o si dovesse utilizzare un sistema di
tracciamento che prevede l'installazione di cookie nel browser degli
utenti diventa obbligatorio, prima di raccogliere qualsiasi tipo di
informazione, richiedere un consenso esplicito e preventivo.

Il problema di queste richieste consiste essenzialmente nel fatto che
molti utenti potrebbero anche non acconsentire ad essere tracciati
privando quindi gli amministratori del sito di informazioni fondamentali
per avere un quadro chiaro di quello che è l'andamento del sito e dei
relativi obiettivi di business.

Ora, a differenza di quanto avviene con Google Analytics, grazie alle
funzioni di anonimizzazione e di gestione della Privacy messe a
disposizione da Matomo, volendo, potrebbe anche essere possibile porsi
in una situazione tale per cui il sistema di tracciamento attivo sul
sito possa anche non ricadere nel perimetro GDPR e possa quindi essere
implementato senza la richiesta di consenso agli utenti

**ATTENZIONE!** Per maggiori informazioni in merito a come poter
effettivamente implementare con Matomo un sistema di tracciamento senza
la richiesta di consenso si consiglia di fare riferimento alla
documentazione ufficiale della piattaforma disponibile ai seguenti link

<https://matomo.org/faq/new-to-piwik/how-do-i-use-matomo-analytics-without-consent-or-cookie-banner/>

<https://matomo.org/faq/new-to-piwik/how-can-i-still-track-a-visitor-without-cookies-even-if-they-decline-the-cookie-consent/>

In sostanza si tratterà di dover soddisfare due condizioni fondamentali:

- Implementare un sistema di tracciamento cookieless, che non fa uso
  cioè di cookie di tracciamento

- Assicurarsi di non tracciare nessuna informazione di identificazione
  personale (PII)

Nello specifico poi per quel che riguarda l'attivazione di un sistema
cookieless sarà necessario:

- implementare la gestione del consenso all'utilizzo dei cookie secondo
  quanto descritto nel relativo capitolo di questo manuale
  ("*Implementazione del consenso al tracciamento o all'uso dei cookie
  con il Matomo javascript tracking client*" ) e inserendo quindi, nel
  codice di monitoraggio di Matomo, la seguente istruzione

> **\_paq.push(\[\'requireCookieConsent\'\]);**

- implementare in maniera corretta il form di Opt Out per consentire
  agli utenti di gestire in autonomia questo consenso

> Per maggiori informazioni in merito si consiglia di fare sempre
> riferimento alla documentazione ufficiale Matomo
> (<https://developer.matomo.org/guides/tracking-javascript-guide#optional-creating-a-custom-opt-out-form>)

In alternativa se non dovessimo prevedere neppure di chiedere il
consenso all'utilizzo dei cookie potremmo anche, in maniera più
drastica, disabilitare completamente tutti i cookie analitici impostati
da Matomo agendo per questo mediante il parametro "**Forza il
tracciamento senza cookie**" presente alla pagina "**Privacy -- Rendi
anonimi i tuoi dati**" del pannello di **Amministrazione** della propria
installazione Matomo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_17.bmp](./assets/media/image20.png)

Operando in questo modo ci troveremo quindi in condizione tali per cui:

- non verranno utilizzati cookie di tracciamento

- i dati raccolti non verranno utilizzati per scopi diversi
  dall\'analisi (a differenza di quello che avviene con Google Analytics
  che utilizza i dati raccolti anche per altri scopi e quindi richiede
  sempre il consenso)

- i visitatori non potranno essere tracciati su diversi siti web (anche
  in questo caso diversamente da quello che avviene con Google Analytics
  che tiene traccia dei visitatori su più siti)

- un utente non potrà essere tracciato per più giorni all'interno dello
  stesso sito (in Matomo non è possibile generare profili utente quando
  i cookie sono disabilitati)

**ATTENZIONE!** anche disabilitando completamente l'utilizzo dei cookie
di tracciamento, in determinate circostanze, Matomo potrebbe comunque
installare nel browser dell'utente specifici cookie (come indicato nelle
documentazione ufficiale <https://matomo.org/faq/general/faq_157/> ) che
comunque, non essendo cookie di profilazione, potranno essere
giustamente considerati come cookie essenziali per i quali non è
prevista la possibilità di opt out

Per quel che riguarda invece il fatto di non tracciare nessuna
informazione di identificazione personale sarà necessario:

- Assicurarsi che gli indirizzi IP siano resi anonimi (mascheramento di
  2 o 3 byte)

- Assicurarsi che gli URL e i titoli delle pagine tracciate non
  contengano dati personali

- Assicurarsi che gli URL dei referrer delle pagine visitate non
  includano dati personali è possibile agire mediante il parametro
  "Rendi anonimo il referrer").

- Assicurarsi, se si utilizzano funzionalità come Dimensioni
  personalizzate, Variabili personalizzate, Monitoraggio eventi che i
  dati raccolti non includano dati personali.

- Assicurarsi, se utilizzano funzionalità come Registrazione delle
  sessioni o Heatmap, di ignorare qualsiasi elemento nella pagina che
  includa dati personali

- **Se si utilizzano funzionalità come il monitoraggio Ecommerce o lo
  User ID, è fortemente consigliato chiedere il consenso al tracciamento
  oltre che sistemare in maniera adeguata tutte le informative privacy
  presenti sul sito**. Questo perché dati quali l'Id Ordine o lo User
  Id, essendo ricollegabili allo specifico utente, possono essere
  considerate come informazioni di identificazione personale (anche se
  eventualmente sostituiti con uno pseudonimo)

- Assicurarsi che i dati raccolti in Matomo vengano utilizzati solo per
  la misurazione dell\'audience e la valutazione delle prestazioni del
  sito Web e non per altri scopi.

- Assicurarsi di non monitorare lo stesso utente su siti diversi.

**ATTENZIONE! Tutti i dati raccolti con Matomo senza il consenso
dell'utente devono assolutamente essere dati anonimi**

Al seguente indirizzo
<https://matomo.org/blog/2018/04/how-to-not-process-any-personal-data-with-matomo-and-what-it-means-for-you/#user-id>
è possibile trovare informazioni utili relativamente a come poter
operare in maniera tale da non processare nessun dato di identificazione
personale (PII)

**ATTENZIONE!** anche al verificarsi di tutte queste condizioni rimane
comunque l'obbligo di menzionare nell'informativa privacy presente sul
sito il fatto che viene utilizzato Matomo come sistema di Web Analytics

Una volta appurato che al verificarsi di tutto quanto sopra indicato
potremmo effettivamente evitare di richiedere agli utenti il consenso al
tracciamento, rimanendo comunque conformi a quanto previsto dal GDPR, va
considerato ora anche l'altro lato della medaglia.

Se da una parte, infatti, la possibilità di non richiedere il consenso
evita il rischio di perdere tutti i dati di quegli utenti che lo
avrebbero negato, dall'altra parte occorre anche sottolineare che il
fatto di non utilizzare più cookie di tracciamento avrà un impatto di
non poco conto sui dati raccolti (
<https://matomo.org/faq/general/faq_156/> ), dati questi che alle fine
si riveleranno essere per forza di cose poco accurati

In definitiva dunque valutando attentamente tutti gli aspetti ossia il
fatto che per evitare di chiedere il consenso è necessario essere certi
al 100% che non vengano raccolti dati di identificazione personale, il
fatto che eliminando i cookie otterremo comunque dati molto meno
accurati, il fatto che nel momento in cui dovessimo implementare anche
il **tracciamento ecommerce comunque sarebbe fortemente consigliato
richiedere il consenso in virtù del fatto che l'ID Ordine può essere
considerato un dato di identificazione personale**, il fatto che
comunque Matomo potrebbe anche non essere il solo sistema di
tracciamento in uso al sito ... si potrebbe arrivare facilmente alla
conclusione che, tutto sommato, la soluzione migliore sia ancora una
volta quella di gestire le richieste di consenso esattamente allo stesso
modo di quanto avviene con Google Analytics.

