# BRAINTREE



Braintree Payments ( <https://www.braintreepayments.com/> ) è un'azienda
con sede a Chicago che offre una delle piattaforme di pagamento
full-stack più popolari sul mercato degli ecommerce. Attualmente è
presente in più di 40 nazioni nel mondo, tra cui i paesi appartenenti
all'Unione Europea, USA, Australia, Canada, Hong Kong, Singapore, con
oltre 100 valute messe a disposizione.

Dal 2013 è entrata a far parte della galassia di PayPal e tra le sue
caratteristiche principali vi è quella di accettare numerosi sistemi per
i pagamenti, tra cui ovviamente PayPal, Visa, MasterPass, fino anche ad
Apple Pay e Google Pay.

**ATTENZIONE! Per poter attivare questa tipologia di pagamento è
necessario acquistare il relativo modulo all'interno di Passstore.**

**Inoltre, considerando la modalità di integrazione messa a disposizione
dalla piattaforma in oggetto, per poter gestire correttamente questo
tipo di pagamento sarà necessario utilizzare un checkout a step**

Una volta acquistato il relativo modulo per poter poi abilitare
effettivamente il pagamento in oggetto all'interno del proprio sito
Passweb sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione BRAINTREE

<!-- -->

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **"Lista dei Metodi di Pagamento"**
    precedentemente esaminata.

<!-- -->

3.  Attivare questa nuova modalità di pagamento secondo quanto descritto
    nel capitolo *"Configurazione Modalità di Pagamento"* di questo
    manuale.

4.  Impostare in maniera corretta i parametri di configurazione
    specifici per questa particolare modalità di pagamento.

In particolare per poter eseguire quest'ultimo passaggio sarà necessario
selezionare il pagamento in oggetto all'interno della maschera **"Lista
dei Metodi di Pagamento"** e cliccare sul pulsante "**Modifica
Pagamento**", presente nella barra degli strumenti.

Verrà quindi visualizzata la maschera di configurazione e
personalizzazione del pagamento, all'interno della quale sarà necessario
impostare, oltre ai parametri classici di configurazione del pagamento,
anche quelli specifici del gateway attualmente considerato e presenti
all'interno della sezione "**Parametri Gateway**"

![](./assets/media/image54.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

> E' sempre consigliabile verificare per prima cosa la corretta
> integrazione tra il sistema di pagamento ed il proprio sito web in un
> ambiente di test per poi passare solo successivamente all'ambiente
> Live di produzione. Per maggiori informazioni su come creare una
> account Sandbox di Braintree si veda anche il successivo capitolo di
> questo manuale.
>
> **Considerando che gli ambienti Braintree di Sandbox e di produzione
> sono comunque ambienti diversi e separati, è sempre consigliabile
> effettuare appositi test anche in ambiente di produzione**

- **Merchant ID:** stringa identificativa del proprio account
  commerciante di Braintree. Può essere trovata nel Backoffice di
  Braintree, nella pagina Home oppure all'interno della sezione
  "**Business**" accessibile dal menu presente in testata (icona
  raffigurante una piccola rotellina)

![](./assets/media/image55.png)

![](./assets/media/image56.png)

- **Public Key / Private Key:** chiave pubblica / privata necessarie per
  il corretto funzionamento dell'integrazione tra Braintree ed il
  proprio sito ecommerce. Come già il Merchant ID anche la chiave
  pubblica e quella privata da utilizzare in fase di integrazione
  saranno indicate all'interno del Backoffice di Braintree alla pagina
  Home oppure all'interno della sezione "**API**" accessibile dal menu
  presente in testata (icona raffigurante una piccola rotellina)

![](./assets/media/image57.png)

![](./assets/media/image58.png)

- **Pagamenti Abilitati:** consente di decidere quali pagamenti dovranno
  effettivamente essere abilitati e resi quindi disponibili agli utenti
  del sito che selezioneranno Braintree in fase di checkout

> E' possibile attivare e gestire i seguenti pagamenti:

- **Card**: pagamento mediante carta di credito.

> Attivando questo pagamento sarà poi possibile decidere, direttamente
> dal backoffice di Braintree, se richiedere o meno, in fase di
> checkout, anche il CVV della carta di credito come ulteriore misura di
> sicurezza.
>
> **ATTENZIONE!** la richiesta del CVV è un'opzione che va attivata e
> configurata direttamente all'interno di Braintree
>
> Per maggiori informazioni in merito si veda anche quanto indicato nei
> successivi capitoli di questo manuale o, meglio ancora, nella
> documentazione ufficiale di Braintree
> (<https://developer.paypal.com/braintree/articles/guides/fraud-tools/basic/avs-cvv-rules>)

- **PayPal:** pagamento mediante PayPal

> Come precedentemente evidenziato, Braintree è una società entrata a
> far parte dal 2013 della galassia PayPal e non poteva pertanto mancare
> la gestione di questa tipologia di pagamento.
>
> **ATTENZIONE!** Per dare agli utenti che selezionano Braintree in fase
> di checkout la possibilità di pagare mediante PayPal non è sufficiente
> flaggare all'interno di Passweb il parametro in questione ma
> **affinché tutto possa funzionare in maniera corretta sarà necessario
> configurare anche il pagamento PayPal all'interno del backoffice di
> Braintree**
>
> Per maggiori informazioni in merito si veda anche quanto indicato nei
> successivi capitoli di questo manuale o, meglio ancora, nella
> documentazione ufficiale di Braintree
> (<https://developer.paypal.com/braintree/docs/guides/paypal/testing-go-live/dotnet>)

- **Apple Pay:** pagamento mediante Apple Pay.

> **ATTENZIONE!** per fare in modo che l'opzione Apple Pay compaia
> effettivamente tra le possibili opzioni di pagamento messe a
> disposizione da Braintree è necessario che il sito sia protetto da un
> certificato SSL e risponda dunque ad un indirizzo del tipo
> https://\...
>
> E' bene ricordare inoltre che Apple Pay è disponibile solamente in
> Safari su iOS versione 10+ e su macOS versione 10.12+
>
> Nel momento in cui Apple Pay non dovesse essere supportata dal browser
> utilizzato (ad esempio perché l'utente sta navigando con Chrome su
> dispositivo Windows) l'opzione "Apple Pay" come possibile pagamento
> messo a disposizione da Braintree non verrà ovviamente visualizzata
>
> **ATTENZIONE!** Come per PayPal anche in questo caso non è sufficiente
> attivare su Passweb il relativo check ma questo tipo di pagamento
> dovrà necessariamente essere configurato in maniera adeguata anche
> all'interno del backoffice di Braintree
>
> Per maggiori informazioni in merito si veda anche quanto indicato nei
> successivi capitoli di questo manuale o, meglio ancora, nella
> documentazione ufficiale di Braintree
> (<https://developer.paypal.com/braintree/docs/guides/apple-pay/configuration/javascript/v3>)

- **Google Pay**: pagamento mediante Google Pay.

> **ATTENZIONE!** per fare in modo che l'opzione Google Pay compaia
> effettivamente tra le possibili opzioni di pagamento messe a
> disposizione da Braintree è necessario che il sito sia protetto da un
> certificato SSL e risponda dunque ad un indirizzo del tipo
> https://\...
>
> E' bene ricordare inoltre che Google Pay è disponibile solamente in
> Google Chrome v61 o versioni successive su Android
>
> Nel momento in cui Google Pay non dovesse essere supportata dal
> browser l'opzione "Google Pay" come possibile pagamento messo a
> disposizione da Braintree non verrà ovviamente visualizzata
>
> **ATTENZIONE!** Come per PayPal e Apple Pay anche in questo caso non è
> sufficiente attivare su Passweb il relativo check ma questo tipo di
> pagamento dovrà necessariamente essere configurato in maniera adeguata
> anche all'interno del backoffice di Braintree
>
> Per maggiori informazioni in merito si veda anche quanto indicato nei
> successivi capitoli di questo manuale o, meglio ancora, nella
> documentazione ufficiale di Braintree
> (<https://developer.paypal.com/braintree/docs/guides/google-pay/configuration/javascript/v3>)
>
> **ATTENZIONE!** Non sono gestiti i pagamenti **PayPal Credit**
> (disponibile solo per i commercianti che vendono a clienti negli Stati
> Uniti o nel Regno Unito) e **Venmo** (attualmente non disponibile in
> Italia)

- **Nome Negozio (Apple Pay):** nome del negozio che verrà visualizzato
  all'utente nel momento in cui dovesse scegliere Apple Pay, come
  effettiva modalità di pagamento tra quelle messe a disposizione da
  Braintree,

- **Google Merchan ID (Google Pay):** ID Google relativo all'account di
  produzione, su cui verranno poi dirottati i pagamenti

> **ATTENZIONE! Il parametro in esame è indispensabile per la corretta
> elaborazione delle transazioni che utilizzando questa metodologia di
> pagamento ma soltanto in ambiente di produzione**
>
> In fase di test con account Sandbox non è quindi necessario
> specificarlo e il corrispondente campo può anche essere lasciato
> vuoto.

- **3d Secure Verification:** consente se attivato, di abilitare, per i
  clienti che dovessero scegliere il pagamento mediante carta di
  credito, lo step di verifica mediante 3d Secure

> **ATTENZIONE!** la verifica 3d Secure sarà disponibile ovviamente solo
> per i clienti che decideranno di pagare con carta di credito e, nello
> specifico, solo per i clienti che utilizzeranno carte di credito
> iscritte ad un programma di verifica come "Verified by VISA"
>
> Per verificare se il 3d Secure è gestito o meno all'intero del proprio
> account Braintree è sufficiente accedere al Backoffice, aprire il menu
> di navigazione cliccando sull'icona raffigurante una piccola rotellina
> posta in testata e selezionare la voce "Business"

![](./assets/media/image59.png)

> Cliccare quindi sul link posto in corrispondenza della colonna
> "**Merchant Account ID**"

![](./assets/media/image60.png)

> e verificare che per la voce "**3D Secure**" sia indicata l'opzione
> "**Enrolled**"

![](./assets/media/image61.png)

**Le informazioni presenti all'interno di questa sezione sono di
fondamentale importanza in quanto saranno poi quelle che garantiranno la
corretta integrazione tra Passweb e i sistemi di pagamento messi a
disposizione dalla piattaforma Braintree mettendo così l'utente nelle
condizioni di poter portare a termine il proprio acquisto.**

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", nel momento in cui l'utente
dovesse, in fase di checkout, selezionare Braintree verranno poi
visualizzate le diverse opzioni di pagamento effettivamente disponibili
sulla base di quanto configurato tanto in Passweb quanto in Braintree e
in base anche a quanto effettivamente supportato dal browser che
l'utente sta utilizzando (in relazione soprattutto all'opzione relativa
ad Apple Pay).

![](./assets/media/image62.png)

Dipendentemente dalla modalità di pagamento effettivamente selezionata
sarà poi necessario fornire i dati richiesti per completare il
pagamento.

**[PAGAMENTO CON CARTA DI CREDITO]{.underline}**

Nel caso in cui dovesse essere selezionato il pagamento mediante carta
di credito per completare il processo sarà necessario inserire,
all'interno dell'apposito form i dati della carta

![](./assets/media/image63.png)

In fase di test è possibile utilizzare una delle carte indicate al
seguente link

<https://developer.paypal.com/braintree/docs/reference/general/testing/dotnet#avs-and-cvv/cid-responses>

**ATTENZIONE! a differenza di quanto avviene con le altre modalità di
pagamento disponibili in Passweb, nel caso di Braintree non si verrà
ridiretti sulla pagina di uno specifico gateway di pagamento e il
processo potrà quindi essere concluso restando sempre all'interno del
proprio sito ecommerce**

In ogni caso, anche in queste condizioni i dati della carta di credito
saranno criptati ed elaborati direttamente dal gateway di Braintree
generando un token (ossia un dato criptato) che verrà poi utilizzato per
concludere la transazione.

**Nessuna delle informazioni inserite verrà quindi memorizzata nel
database del sito Passweb**

Nello specifico durante la transazione a Braintree verranno passati i
seguenti dati:

- payment_method_nonce: token restituito da Braintree con le
  informazioni sul pagamento

- amount: ammontare dell\'ordine

- order_id: identificativo dell\'ordine su Passweb

- currency_iso_code: valuta dell\'ordine

- customer_details:

  - email: email dell\'utente

  - first_name: nome

  - last_name: cognome

**[PAGAMENTO CON PAYPAL]{.underline}**

Nel momento in cui si dovesse selezionare PayPal come modalità di
pagamento verrà visualizzato il pulsante "**Paga Adesso**" di PayPal

![](./assets/media/image64.png)

In queste condizioni per completare la transazione sarà quindi
necessario cliccare sul pulsante evidenziato in figura e inserire, nella
successiva maschera, le credenziali dell'account PayPal da utilizzare
per il pagamento

![](./assets/media/image65.png)

Effettuato l'accesso all'account PayPal sarà quindi possibile scegliere
se completare il pagamento con una delle carte registrate sull'account
PayPal oppure utilizzando il saldo caricato su questo stesso account

![](./assets/media/image66.png)

**ATTENZIONE!** anche in questo caso come per il pagamento con carta,
tutto il processo avverrà senza uscire dal sito Ecommerce. Gli eventuali
dati della carta di credito verranno però inseriti all'interno di una
finestra gestita direttamente da PayPal e verranno quindi processati
direttamente da PayPal stesso.

**Anche in questo caso sul database di Passweb non verrà in alcun modo
memorizzata nessuna informazione relativa alla carta di credito
utilizzata dall'utente**

Cliccando sul pulsante "**Continua a rivedere l'ordine**" verrà chiusa
la finestra relativa a PayPal e sarà quindi possibile concludere
l'ordine

![](./assets/media/image67.png)

**[PAGAMENTO CON GOOGLE PAY]{.underline}**

Infine nel caso in cui si dovesse selezionare come modalità di pagamento
Google Pay verrà visualizzato il classico pulsante "**Gpay**"

![](./assets/media/image68.png)

Cliccando sul pulsante evidenziato in figura verranno richieste le
credenziali dell'Account Google cui dovrà, ovviamente, essere associata
almeno una carta di credito

![](./assets/media/image69.png)

Analogamente a quanto avveniva per PayPal sarà quindi sufficiente
inserire le credenziali del proprio account google, selezionare la carta
di credito desiderata (oppure registrarne una nuova) e concludere poi
l'ordine

**ATTENZIONE!** come nei casi precedenti tutto il processo avverrà senza
lasciare il sito Ecommerce. I dati di eventuali carte di credito
verranno in questo caso registrati e processati direttamente da Google

**Anche in questo caso, dunque, sul database di Passweb non verrà in
alcun modo memorizzata nessuna informazione relativa alla carta di
credito utilizzata dall'utente**

