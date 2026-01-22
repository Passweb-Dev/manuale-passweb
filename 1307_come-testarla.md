# COME TESTARLA



Una volta attivata la Google Consent Mode l'ultimo passaggio da fare
potrebbe essere quello di verificare che il tutto funzioni in maniera
corretta come effettivamente descritto nei precedenti capitoli di questo
manuale.

In questo senso è possibile, ad esempio, utilizzare gli strumenti per
sviluppatori di Chrome per verificare:

- Che i valori impostati a default per i vari consensi siano stati
  registrati correttamente

- Che i dati trasmessi ai server di Google siano coerenti con le scelte
  effettuate dagli utenti in merito alla gestione dei cookie

Per quel che riguarda il primo punto a questo indirizzo
<https://support.cookiebot.com/hc/en-us/articles/360018413380-Checking-if-Consent-Mode-is-properly-implemented>
è indicato un semplice snippet di codice (sezione "Checking the Consent
Mode Setting") da copiare, incollare ed eseguire nella Console degli
strumenti per sviluppatori del proprio browser.

Eseguendo questo snippet di codice prima di effettuare qualsiasi tipo di
scelta in merito alla gestione dei consensi dovremo avere come risultato
i valori impostati a default per ogni singolo consenso

![](./assets/media/image15.png)

Eseguendo lo stesso snippet di codice dopo aver impostato qualche
consenso dovremo invece vedere oltre al valore di default anche l'update
effettuato direttamente dalla CMP sulla base dei consensi forniti
dall'utente

![](./assets/media/image16.png)

Per quel che riguarda invece la possibilità di verificare che i dati
trasmessi ai server di Google siano coerenti con le scelte effettuate
dagli utenti in merito alla gestione dei cookie, è possibile utilizzare
ancora una volta gli "Strumenti per sviluppatori" del proprio browser
controllando, questa volta dal tab "Network", il dettaglio delle
richieste inviate ai server di Google.

Nello specifico sarà necessario controllare il valore del parametro
"**gcs**" presente nell'hit inviato a Google. Tale parametro avrà
infatti un valore del tipo

**gcs=G1XX**

dove G1 è una parte invariante del valore di questo parametro mentre i
successivi due digit potranno assumere un valore di 0 o 1 a seconda del
fatto che i due consensi obbligatori, ad_storage e analytics_storage,
siano in stato 'denied' o 'granted'. Nello specifico sarà quindi
possibile fare riferimento alla seguente tabella

+-----------------------------------+-----------------------------------+
| **VALORE PARAMETRO gcs**          | **SIGNIFICATO**                   |
+===================================+===================================+
| G100                              | **ad_storage = denied;            |
|                                   | analytics_storage = denied**      |
|                                   |                                   |
|                                   | Consenso negato sia per i cookie  |
|                                   | statistici che per i cookie di    |
|                                   | marketing                         |
+-----------------------------------+-----------------------------------+
| G101                              | **ad_storage = denied;            |
|                                   | analytics_storage = granted**     |
|                                   |                                   |
|                                   | Consenso negato per i cookie di   |
|                                   | marketing e approvato invece per  |
|                                   | i cookie statistici               |
+-----------------------------------+-----------------------------------+
| G110                              | **ad_storage = granted;           |
|                                   | analytics_storage = denied**      |
|                                   |                                   |
|                                   | Consenso negato per i cookie di   |
|                                   | statistici e approvato invece per |
|                                   | i cookie marketing                |
+-----------------------------------+-----------------------------------+
| G111                              | **ad_storage = granted;           |
|                                   | analytics_storage = granted**     |
|                                   |                                   |
|                                   | Consenso approvato sia per i      |
|                                   | cookie statistici che per i       |
|                                   | cookie di marketing               |
+-----------------------------------+-----------------------------------+

In considerazione di ciò se apriamo il tab Network degli "Strumenti per
sviluppatori" ed effettuiamo una visita al sito con la Consent Mode
implementata, prima di aver fornito qualsiasi tipo di consenso e, nel
pannello di ricerca presente sulla sinistra, filtriamo per gcs, dovremmo
trovare le richieste effettivamente inviate ai server di Google da parte
del nostro sito, in tali richieste (sulla base della tabella sopra
riportata) il valore del parametro gcs dovrebbe, generalmente, essere
esattamente G100

![](./assets/media/image17.png)

In queste condizioni inoltre non dovremmo registrare su Analytics nessun
tipo di visita né nella Debug View né tanto meno nei report in tempo
reale.

Facendo la stessa operazione, questa volta però dopo aver fornito il
consenso ad esempio sia per i cookie statistici che per quelli marketing
nel dettaglio delle hit inviate ai server di Google dovremo ora avere un
valore del parametro gcs pari a G111

![](./assets/media/image18.png)

Come ulteriore verifica, in queste condizioni dovremmo ora registrare
correttamente visita e relativi eventi anche in tutti i rapporti di GA4

