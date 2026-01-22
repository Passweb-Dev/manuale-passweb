# OPT OUT UTENTI



Come indicato nei precedenti capitoli di questo manuale nel momento in
cui si dovesse gestire il tracciamento classico di Matomo (via
javascript con l'installazione di cookie sul browser dell'utente)
diventa di fondamentale importanza, per ottemperare a quanto previsto
dal GDPR, inserire nelle varie informative (Privacy Policy, Cookie
Policy ...) il fatto che il sito utilizza Matomo come sistema di web
analytics con la conseguente installazione dei relativi cookie e,
soprattutto, diventa di fondamentale importanza gestire le richieste di
consenso preventivo assicurandosi che i cookie vengano installati e i
dati raccolti solo dopo che l'utente abbia effettivamente dato il suo
esplicito consenso.

**ATTENZIONE!** sotto questo aspetto Matomo è sottoposto esattamente
agli stessi vincoli cui è sottoposto anche Google Analytics

In questo senso la soluzione più semplice potrebbe essere, come per
Google Analytics, quella di ricorrere all'utilizzo di apposite
piattaforme CMP (es. Iubenda, Cookiebot ...) facendo attenzione al fatto
di:

- inserire nelle informative da esse generate l'utilizzo di Matomo come
  piattaforma di web analytics

- classificare i cookie utilizzati da Matomo come cookie
  analitici/statistici o marketing/profilazione in base alla tipologia
  di dati che andremo effettivamente a raccogliere

- configurare il blocco preventivo dello script di Matomo per essere
  certi di attivare il tracciamento e iniziare a raccogliere i dati solo
  dopo che l'utente abbia effettivamente prestato il proprio consenso
  all'utilizzo di quella specifica tipologia di cookie

Ai seguenti indirizzi è possibile trovare informazioni più dettagliate
relativamente a come poter utilizzare Matomo assieme a:

- Iubenda --
  <https://www.iubenda.com/it/help/3592-full-piwik-integration-guide>

- Cookiebot --
  <https://support.cookiebot.com/hc/en-us/articles/360017539960-Matomo-installation>
  (installazione e gestione di Cookiebot mediante il sistema Tag Manager
  di Matomo)

Oltre all'utilizzo di piattaforme CMP esterne (comunque indispensabili
nel momento in cui il sito dovesse utilizzare anche altri strumenti di
tracciamento diversi da Matomo), un'altra possibile soluzione potrebbe
essere quella di implementare le richieste di consenso ai cookie
utilizzando direttamente il client di monitoraggio javascript di Matomo
e il relativo form di Opt Out.

Tra i vari strumenti di gestione della Privacy messi a disposizione da
Matomo troviamo infatti anche un form di Opt Out gestito tramite un
iframe che può essere inserito in una qualsiasi pagina del nostro sito

Per prelevare il codice di questo iframe è sufficiente accedere alla
sezione "**Opt-out Utenti**" presente all'interno del menu "**Privacy**"
nella pagina di **Amministrazione** della propria installazione Matomo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_9.bmp](./assets/media/image9.png)

Una volta inserito l'iframe in questione all'interno del nostro sito,
mediante un apposito componente HTML, nelle relative pagine comparirà lo
stesso messaggio visualizzato in anteprima anche all'interno di Matomo
con un check che l'utente potrà deselezionare per negare il proprio
consenso evitando quindi di essere tracciato.

Ora, riguardo l'utilizzo del form di Opt Out gestito in questo modo
(quindi mediante l'inserimento sul sito del relativo iframe) vanno fatte
alcune considerazioni di fondamentale importanza.

Innanzitutto occorre considerare che **nell'implementazione standard di
Matomo, a default, tutti i visitatori del sito saranno tracciati**.
Questo significa quindi che nel momento in cui l'utente dovesse accedere
per la prima volta al sito (e, ovviamente, non siano stati implementati
specifici controlli mediante apposite piattaforme CMP) la sua visita
verrà tracciata e i suoi dati verranno correttamente raccolti.

A questo punto, se sul sito è stato inserito il from di opt out,
l'utente potrà negare il proprio consenso deselezionando l'apposito flag
e da questo momento in avanti non verrà più tracciato.

Tecnicamente nel momento in cui l'utente dovesse deselezionare il flag
verrà installato sul suo browser un cookie 'pwik_ignore' (le visite di
utenti con questo cookie installato non verranno tracciate).

Come è semplice comprendere, sebbene la gestione di questo form sia
estremamente semplice (si tratta infatti di inserire un semplice iframe
nelle pagine del sito) non è esattamente corretta e conforme al GDPR
inquanto **non soddisfa il concetto di consenso preventivo**. Prima che
venga installato il cookie che impedisce il tracciamento l'utente deve
infatti accedere al sito almeno una volta senza che questo stesso cookie
sia presente nel suo browser e quindi i dati della sua prima visita
verranno comunque registrati.

Inoltre il cookie 'pwik_ignore' che impedisce il tracciamento potrebbe
anche essere trattato (dipendentemente dalle modalità di installazione
di Matomo) come un cookie di terze parti e se l'utente dovesse avere
attivi dei sistemi di blocco su questo tipo di cookie questo non potrà
essere installato e, di fatto, anche deselezionando il flag l'utente
continuerebbe ad essere tracciato.

Infine, anche se questo aspetto è sicuramente meno importante dei
precedenti, l'iframe non è molto personalizzabile, è possibile
modificare font e colori operando direttamente a Matomo ma ad, esempio,
non è possibile modificare il testo del messaggio.

In virtù di tutto quanto detto quindi la soluzione migliore, in ottica
di conformità al GDPR e nell'ipotesi di non voler ricorrere all'utilizzo
di piattaforme CMP, è indubbiamente quella di implementare le richieste
di consenso al tracciamento e/o all'utilizzo dei cookie utilizzando il
client di monitoraggio javascript di Matomo e un form di Opt Out
customizzato seguendo rispettivamente le indicazioni presenti ai
seguenti link

- <https://developer.matomo.org/guides/tracking-consent>

- <https://developer.matomo.org/guides/tracking-javascript-guide#optional-creating-a-custom-opt-out-form>

Nel primo dei due link sopra indicati viene spiegato come modificare il
codice di tracciamento di Matomo per implementare un sistema di
richiesta di consenso preventivo (analogo, sotto certi aspetti, alla
Google Consent Mode) mentre nel secondo viene spiegato come poter
costruire un form di Opt Out completamente personalizzabile e come
operare per fare in modo che le scelte fatte dall'utente all'interno di
questo form si riflettano esattamente sul tracciamento e sulla raccolta
dei suoi dati.

Per maggiori informazioni in merito a questo tipo di operazioni è
possibile consultare anche il successivo capitolo di questo manuale.

In ogni caso un altro adempimento di fondamentale importanza imposto dal
GDPR è quello di poter mostrare una prova del consenso fornito dagli
utenti, per cui oltre ad implementare eventualmente tutto il meccanismo
di richiesta preventiva con Matomo andrebbe poi implementato anche un
sistema per registrare i consensi forniti dagli utenti.

Tenendo conto di questo e del fatto che questo tipo di soluzione è
comunque limitata solamente all'utilizzo di Matomo (il consenso
preventivo all'utilizzo di strumenti quali il pixel di facebook, google
ads ... andrebbe gestito in maniera diversa) **in definitiva la
soluzione migliore è più sicura in ottica GDPR potrebbe essere
effettivamente la prima indicata ossia quella di utilizzare apposite
piattaforme CMP come Iubenda o Cookiebot demandando direttamente a loro
tutta la gestione del consenso preventivo e della registrazione dei
consensi forniti dagli utenti**

