# CONSENT MODE AVANZATA



La modalità **Avanzata** rappresenta l'opzione più sofisticata di
implementazione della Consent Mode ed è pensata, essenzialmente, per chi
vuole mantenere un certo livello di analisi e modellazione anche in
assenza di consenso ed è quindi particolarmente indicata per contesti
che richiedono **ottimizzazione delle campagne, modellazione accurata e
dati più robusti**, pur mantenendo un framework conforme alla privacy

In questo caso, i tag e gli script di tracciamento di Google **vengono
caricati immediatamente al caricamento della pagina**, ma iniziano a
operare in uno stato di consenso predefinito che, di solito, è
**denied** (negato).

Questo significa che, pur essendo attivi, gli script di tracciamento non
impostano cookie né registrano dati identificabili. In queste condizioni
inviano comunque a Google dei cosiddetti **cookieless pings** ossia
richieste anonime che non contengono identificatori personali, ma
forniscono informazioni di base come l'evento avvenuto, il tipo di
pagina visitata, e lo stato di consenso.

Quando poi l'utente esprime la propria scelta tramite il cookie banner,
lo stato di consenso verrà aggiornato dinamicamente e i tag e gli script
di tracciamento modificheranno di conseguenza il loro comportamento: se
l'utente accetta, inizieranno a raccogliere dati completi con cookie e
identificatori. Se rifiuta, continueranno invece ad inviare solo segnali
anonimi.

Questo approccio ha due vantaggi principali:

- **Continuità nella raccolta dati** -- anche senza consenso, Google
  riceve informazioni aggregate che possono essere utilizzate per la
  **modellazione delle conversioni** e per l'analisi del traffico.

- **Maggiore precisione** -- i modelli di conversione sono più accurati
  perché tengono conto anche del comportamento degli utenti che non
  hanno accettato i cookie, pur rispettando la loro privacy.

Dal punto di vista tecnico questo tipo di implementazione richiede
maggiore attenzione. Occorre infatti configurare correttamente gli stati
di consenso di default, collegare la piattaforma CMP per aggiornare
dinamicamente lo stato quando l'utente effettua le sue scelte, e occorre
assicurarsi anche che i tag e gli script di tracciamento vengano
eseguiti correttamente sin dal primo caricamento della pagina.

Nel caso in cui si dovesse decidere di implementare la Consent Mode
Avanzata, dunque, il primo script ad essere eseguito al caricamento
della pagina sarà esattamente quello che consente di importare la
libreria Google per l'utilizzo dei vari comandi "gtag" e per
l'inizializzazione dello script di tracciamento

*\< script type=\"text/javascript\" async=\"\"
src=https://www.googletagmanager.com/gtag/js?id=G-XXXXXXX \>\< / script
\>*

Successivamente verrà poi eseguito lo script di seguito riportato che,
di base, si occuperà di impostare il valore di default dei vari consensi

> *\<script\>*
>
> *// Parte 1 -- Inizializzazione del dataLayer*
>
> *window.dataLayer = window.dataLayer \|\| \[\];*
>
> *function gtag() {*
>
> *dataLayer.push(arguments);*
>
> *}*
>
> *// Parte 2 -- Impostazione del valore di default per i vari consensi*
>
> *gtag(\"consent\", \"default\", {*
>
> *ad_storage: \"denied\",*
>
> *ad_user_data: \"denied\",*
>
> *ad_personalization: \"denied\",*
>
> *analytics_storage: \"denied\",*
>
> *functionality_storage: \"denied\", // optional*
>
> *personalization_storage: \"denied\", // optional*
>
> *security_storage: \"granted\", // optional*
>
> *wait_for_update: 2000 // milliseconds*
>
> *});*
>
> *// Parte 3 -- Ottimizzazione della qualità dei click*
>
> *gtag(\'set\', \'url_passthrough\', true);*
>
> *gtag(\"set\", \"ads_data_redaction\", true);*
>
> *\</script\>*

Nel primo blocco di questo snippet di codice ("*Parte 1 --
Inizializzazione del dataLayer")* viene semplicemente inizializzato il
Data Layer in uso al sito in modo tale da preparalo per l'inserimento
dei valori di default che dovranno essere assegnati ai vari consensi

Nel secondo blocco ("*Parte 2 -- Impostazione del valore di default per
i vari consensi*") vengono invece settati i valori di default che
dovranno assumere i diversi tipi di consenso, valori questi che potranno
essere impostati mediante i relativi parametri presenti all'interno del
Wizard del proprio sito Passweb (menu "**Sito -- Preferenze**", tab
"**Tracciamento Dati**", sezione "**Valori Consent Default**")

![](./assets/media/image13.png)

Sotto questo punto di vista è bene sottolineare che, come
precedentemente evidenziato, generalmente il valore di default dei vari
consensi dovrebbe essere impostato su "**Denied**" (negato) in modo tale
da gestire una sorta di blocco preventivo impendo a Google di installare
sia i cookie marketing che quelli analitici.

In queste condizioni tali cookie verranno quindi installati solo dopo
che l'utente avrà interagito con il banner della CMP fornendo in maniera
esplicita i relativi consensi. Prima dell'interazione con il cookie
banner e nel caso in cui l'utente dovesse negare il consenso al
tracciamento a Google verranno inviati solo ed esclusivamente i
cosiddetti **cookieless pings.**

Il fatto comunque di poter impostare direttamente da Passweb un valore
di default per ogni singolo consenso mette l'amministratore del sito
nelle condizioni, volendo, di abilitare anche una configurazione
"forzata" dei valori di default che prevede di impostare su
"**Granted**" (consentito) il valore di default dei consensi di
**analytics_storage** e di **security_storage.**

Ora, a parte il valore di **security_storage** che di per sé potrebbe
anche essere impostato sempre su "Granted" non avendo particolari
implicazioni dal punto di vista della privacy, il fatto di impostare, in
questa configurazione, anche analytics_storage su "Granted" fa sì che,
sulla base di quanto indicato nei precedenti capitoli di questo manuale,
al caricamento della pagina venga immediatamente salvato sul browser
dell'utente il cookie analitico (non quello di marketing) di Analytics,
inviando quindi a Google non più dei semplici ping anonimi ma veri e
propri dati di tracciamento relativi alla vista della pagina web.

Tale configurazione consente, ovviamente, di ottenere dati ancora più
precisi ma per poterla effettivamente applicare bisognerebbe, da una
parte, accertarsi di anonimizzare correttamente i dati inviati ad
Analytics prima dell'esplicito consenso al tracciamento, e dall'altra
parte, ricorrere al "Legittimo interesse" dichiarando esplicitamente
tutto ciò che serve (compreso il fatto che il sito raccoglie dati di
visite alle pagine prima che l'utente abbia fornito il consenso) nelle
varie informative presenti sul sito

**ATTENZIONE!** **prima di applicare la configurazione che prevede di
impostare su "Granted" il valore di default di analytics_storage è
sempre bene confrontarsi con il proprio DPO e/o con chi si occupa della
questione privacy del sito in modo tale da essere certi di rimanere
comunque compliance con quanto richiesto dal GDPR.**

Infine, nel terzo blocco dello script ("*Parte 3 -- Ottimizzazione della
qualità dei click*") consente di eseguire delle istruzioni che di per sé
non sono obbligatorie ma che consentono comunque di attivare e gestire
correttamente due ulteriori funzionalità "avanzate" della Consent Mode.

In particolare per quel che riguarda il primo dei due comandi
("*gtag(\'set\', \'url_passthrough\', true);*") la cosa importante da
sottolineare è che i tag di Google di solito memorizzano le informazioni
sull'annuncio che un utente ha seguito per arrivare sul sito nei cookie
di prima parte, al fine di migliorare l'accuratezza della conversione.
Il problema in questo senso è che quando ad_storage è settato a denied,
i tag di Google non salvano queste informazioni localmente.

In queste condizioni per migliorare la qualità della misurazione dei
click degli annunci, è possibile scegliere di passare le informazioni
attraverso i parametri dell'URL utilizzando, per l'appunto il comando in
esame

**ATTENZIONE!** Utilizzando questa funzione potrebbero essere aggiunti
ai link sul sito alcuni parametri di query string (gclid, dclid, gclsrc,
\_gl).

Per quel che riguarda invece il secondo comando occorre ricordare che di
base quando ad_storage è denied, non verranno impostati nuovi cookie per
scopi pubblicitari. Inoltre, i cookie di terze parti precedentemente
impostati su google.com e doubleclick.net non verranno utilizzati se non
per scopi di spam e frode. In queste condizioni i dati inviati a Google
includeranno comunque l'URL della pagina intera, comprese le
informazioni sui click sugli annunci nei parametri dell'URL.

Volendo è comunque possibile ridurre ulteriormente i dati degli annunci
quando ad_storage è 'denied' utilizzando, per l'appunto il comando
*gtag(\"set\", \"ads_data_redaction\", true);*

Quando ads_data_redaction è true e ad_storage è denied infatti, gli
identificatori di clic sugli annunci inviati nelle richieste di rete da
Google Ads e dai tag Floodlight verranno oscurati. Le richieste di rete
verranno inviate inoltre anche tramite un dominio senza cookie.

**ATTENZIONE!** In assenza di questo comando facoltativo, alcuni cookie
potrebbero comunque essere installati.

Una volta impostato il valore di default dei vari consensi, verrà poi
eseguito lo script di inizializzazione e configurazione del sistema di
tracciamento di Google Analytics, cosa questa che, assieme ai valori di
default precedentemente impostati per i vari consensi, permetterà al
sito di iniziare ad inviare a Google i vari cookiless pings ancora prima
che compaia il banner della CMP in uso al sito e quindi ancora prima che
l'utente abbia prestato i relativi consensi (oltre che ovviamente nel
momento in cui l'utente dovesse poi negare il consenso al tracciamento)
permettendo quindi a Google stesso mediante il suo sistema di
modellazione dei dati di recuperare statistiche e conversioni che
altrimenti andrebbero sicuramente perse

A questo punto, l'ultimo step nel flusso di attivazione e di gestione
della Consent Mode Avanzata, sarà quello che prevede di inserire,
successivamente allo script di tracciamento di GA4, lo snippet di codice
per l'attivazione e la gestione del cookie banner della CMP in uso al
sito (es. Iubenda) che da questo momento in avanti si occuperà di
bloccare, salvo esplicito consenso, eventuali altri script presenti sul
sito che dovessero rilasciare cookie e/o profilare gli utenti, oltre che
ovviamente di aggiornare in tempo reale i vari consensi sulla base delle
scelte effettuate in maniera esplicita dall'utente stesso

**ATTENZIONE!** **per poter garantire il corretto ordine di esecuzione
dei vari script, e quindi la corretta implementazione della Consent Mode
Avanzata, è indispensabile che tutti i vari snippet di codice siano
inseriti nei rispettivi campi presenti all'interno della sezione
"Tracciamento Dati" presente alla pagina "Sito -- Preferenze" del
Wizard**

Ciò significa dunque che nel momento in cui lo script di tracciamento di
Google o lo script di gestione della CMP (es. Iubenda) dovesse essere
inserito in maniera manuale all'interno di campi come "Code Snippet --
Head / Footer" o in altre sezioni del sito diverse da quelle presenti
all'interno della sezione "Tracciamento Dati", l'ordine di esecuzione
dei vari script potrebbe non essere quello corretto e, di conseguenza,
la Consent Mode potrebbe non funzionare come deve.

