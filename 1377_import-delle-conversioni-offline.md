# IMPORT DELLE CONVERSIONI OFFLINE



Come già evidenziato in altri capitoli di questo manuale, uno dei
principali problemi in cui si potrebbe incorrere nella gestione del
tracciamento delle conversioni di acquisto su Google Ads è quello che
potrebbe verificarsi nel momento in cui l'utente dovesse decidere di
pagare l'ordine online.

In queste condizioni, infatti, una volta confermato l'ordine l'utente
uscirà dal sito e verrà ricondotto sul gateway di pagamento della banca
dove potrà completare la transazione inserendo, in maniera sicura, tutti
i dati della carta di credito.

Fatto questo, dipendentemente dal metodo di pagamento utilizzato,
l'utente potrebbe anche decidere di non tornare al sito chiudendo
semplicemente il browser.

**In queste condizioni quindi non essendo caricata la pagina di conferma
ordine del sito Passweb, non potrà essere eseguito lo snippet di codice
necessario per inviare a Google Ads i dati della transazione e, di
conseguenza, non potrà essere registrata neppure la relativa
conversione.**

Per gestire queste casistiche Google Analytics offre la possibilità di
utilizzare delle chiamate lato server, mediante Measurement Protocol,
che consentono a Passweb, una volta ricevuta la chiamata server 2 server
di ritorno dal gateway di pagamento (chiamata questa che conferma che
tutto è andato effettivamente a buon fine), di inviare comunque i dati
della transazione a Google Analytics.

Impostando quindi il parametro "**Google Analytics -- Eventi checkout**"
presente alla pagina "**Sito -- Preferenze**" del wizard (tab
"**Tracciamento Dati**" sezione "**Eventi Ecommerce per Google Analytics
e Google Tag Manager**") sul valore "Server"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\import_conversioni_offline_1.bmp](./assets/media/image27.png){width="5.813194444444444in"
height="3.3333333333333335in"}

potremmo avere, sostanzialmente, la certezza che l'evento di purchase
venga comunque registrato su Google Analytics anche nel momento in cui
l'utente, dopo aver pagato, dovesse decidere di chiudere il browser
senza tornare sulla pagina Passweb di conferma ordine (e senza quindi
far scattare l'evento client di registrazione delle purchase)

**A differenza di Analytics, purtroppo, Google Ads non mette a
disposizione delle chiamate lato server da poter utilizzare per inviare
i dati di conversione ad Ads anche nel momento in cui l'utente dovesse
decidere di chiudere il browser sul gateway di pagamento senza poi
tornare al sito, per cui, in queste condizioni, la conversione andrebbe,
ovviamente, persa.**

Passweb offre comunque la possibilità di recuperare anche questo tipo di
conversioni mettendo a disposizione dell'utente i dati di questa
particolare tipologia di ordini (conclusi correttamente sul gateway di
pagamento e senza ritorno al sito Ecommerce) nel formato richiesto da
Google Ads per poter poi essere uplodati all'interno di questa stessa
piattaforma grazie alle procedure di **Import delle conversioni offline
(**quindi esternamente al sito e in un momento successivo a quello in
cui è stato effettivamente registrato l'ordine) o meglio ancora, come
richiesto dallo stesso Google Ads, utilizzando le "**Conversioni
avanzate per i lead**"

Detto che lo scopo di questo manuale non è assolutamente quello di
fornire una descrizione esaustiva di come funziona in Ads l'import delle
conversioni offline e/o la gestione delle conversioni avanzate per i
leads, dei vantaggi che queste potrebbero portare o delle casistiche in
cui andrebbero effettivamente utilizzate, e che per ottenere questo tipo
di informazioni il consiglio è sempre quello di fare riferimento alla
relativa documentazione Google Ads
(<https://support.google.com/google-ads/answer/2998031> ,
<https://support.google.com/google-ads/answer/9888656#leads> ), il
flusso attivabile all'interno del proprio sito Ecommerce per gestire
questo tipo di conversioni, di base, è il seguente:

- L'utente arriva una prima volta sul nostro sito cliccando su di un
  annuncio pubblicitario di Google Ads

- All'arrivo sul sito l'url di atterraggio conterrà il parametro gclid
  (creato grazie al tagging automatico di Ads che è sempre bene
  attivare) della relativa campagna e, posto che lo stesso utente abbia
  prestato tutti i relativi consensi (in ambito GDPR) verranno salvati
  sul suo browser tutti i cookie di tracciamento

- In questa prima fase però l'utente abbandona il sito senza concludere
  l'ordine e quindi senza convertire. In questa fase non viene quindi
  inviata ad Ads nessun tipo di informazione

- Lo stesso utente decide poi in un momento successivo di tornare sul
  nostro sito utilizzando ovviamente lo stesso dispositivo e lo stesso
  browser in cui è ancora presente il cookie di Ads salvato durante la
  sua prima visita

- Questa volta si registra, effettua il login e conclude l'ordine
  decidendo di pagare con carta di credito

- Selezionato quindi il metodo di pagamento, cliccando sul pulsante di
  conferma l'utente verrà ricondotto sulla pagina del gateway di
  pagamento. In questo momento inoltre, prima di uscire dal sito
  Ecommerce verranno eseguite le due istruzioni seguenti:

> *gtag(\'set\', \'user_data\', {*
>
> *\"**sha256_email_address\":* *valore hashato della mail utente*
>
> *\"**sha256_phone_number\":* *valore hashato del telefono utente,*
>
> *\"address\": {*
>
> *\"**sha256_first_name\":* *valore hashato del nome utente,*
>
> *\"**sha256_last_name\":* *valore hashato del cognome / ragione
> sociale utente,*
>
> *\"street\":* *indirizzo utente (via),*
>
> *\"city\":* *indirizzo utente (città),*
>
> *\"postal_code\":* *indirizzo utente (CAP),*
>
> *\"country\":* *indirizzo utente (Nazione)*
>
> *}*
>
> *});*
>
> *gtag(\'event\', \'set_user_data_passweb\', { \'send_to\': AW-XXXXX
> })*
>
> che di fatto consentono di inviare ad Ads i dati dell'utente che ha
> effettuato l'ordine.
>
> **ATTENZIONE!** affinché le due istruzioni appena evidenziate possano
> essere eseguite in maniera corretta è necessario che siano soddisfatti
> tutti i requisiti di seguito indicati:

- la mail del cliente deve essere uno dei dati obbligatori richiesti in
  fase di registrazione al sito

- il parametro "**ID Conversioni Google Ads**" presente alla pagina
  "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento Dati**"
  sezione "**Google Ads**") deve essere correttamente valorizzato con
  l'identificatore univoco delle conversioni associate al proprio
  account Google Ads

- in fase di configurazione del sito deve essere stato attivato il
  parametro "**Raccolta Dati Utente Google Ads**" presente anch'esso
  alla pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento
  Dati**" sezione "**Google Ads**")

> A questo punto possono verificarsi due diverse situazioni.

- **Caso 1** -- L'utente conclude il pagamento e decide anche di tornare
  sul sito Ecommerce visitando quindi la pagina Passweb di "Conferma
  Ordine".

> In questo caso, posto di aver implementato in maniera corretta tutto
> il sistema di tracciamento, visitando la pagina di conferma ordine
> verrà eseguito lo snippet di codice deputato all'invio dei dati
> dell'ordine verso Google Ads dove verrà quindi registrata in maniera
> corretta la relativa conversione.
>
> Allo stesso modo a seguito della visita della pagina di conferma
> ordine il relativo documento Passweb verrà automaticamente marcato
> come "**Esportato su Google Ads**"

![Videate\\ordine_esportato_su_ads.bmp](./assets/media/image28.png){width="5.766666666666667in"
height="3.3in"}

> assumendo per l'appunto che i dati della conversione siano già stati
> inviati correttamente alla relativa piattaforma

- **Caso 2** -- L'utente conclude il pagamento ma questa volta decide di
  non tornare sul sito Ecommerce chiudendo semplicemente il browser dopo
  aver completato la transazione.

> In questo caso non potrà essere eseguito lo snippet di codice deputato
> all'invio dei dati dell'ordine verso Google Ads dove non verrà quindi
> registrata nessuna conversione.
>
> Per questa ragione il relativo documento Passweb verrà automaticamente
> marcato come "**Non ancora esportato su Google Ads**"

![Videate\\ordine_non_esportato_su_ads.bmp](./assets/media/image29.png){width="5.766666666666667in"
height="3.3in"}

- I documenti marcati come "**Non ancora esportati su Google Ads**"
  potranno essere inseriti, in un secondo momento, in un file prodotto
  in automatico da Passweb che potrà essere caricato su Ads a seguito di
  una schedulazione automatica oppure di un semplice upload manuale.

- Tra i dati presenti all'interno di questo file ci sarà sicuramente la
  mail (hashata) dell'utente che ha effettuato il relativo ordine (la
  stessa che il sito ha inviato ad Ads nel momento in cui l'utente ha
  abbandonato il sito ecommerce per essere ridiretto al gateway di
  pagamento) e, volendo, anche il valore del gclid eventualmente
  presente nel browser dell'utente nel momento in cui è stato effettuato
  l'ordine.

- La mail (hashata) dell'utente, ed eventualmente il valore del gclid,
  presenti nel file di importazione verranno utilizzati come campi
  chiave e consentiranno a Google Ads, di registrare la conversione (che
  non era stata registrata al momento della conclusione dell'ordine)
  legandola, secondo i suoi modelli di attribuzione, alla corretta
  campagna e al relativo utente.

Ora per fare in modo che tutto questo flusso possa effettivamente essere
implementato in maniera corretta è necessario operare in un certo modo
sia all'interno di Passweb che all'interno del proprio account Google
Ads.

