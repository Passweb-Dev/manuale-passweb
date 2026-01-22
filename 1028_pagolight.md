# PAGOLIGHT



**ATTENZIONE! Per poter attivare il pagamento rateale mediante la
piattaforma di PagoLight (heidipay) è necessario acquistare il relativo
modulo**

La modalità di pagamento etichettata a default come **PagoLight** offre
agli utenti del sito la possibilità di concludere i loro acquisti
**mediante la richiesta di un finanziamento online**.

Una volta approvata la richiesta di finanziamento sarà poi possibile
suddividere il totale dell' ordine in comode rate pagabili direttamente
con la propria carta di credito.

**ATTENZIONE! Il finanziamento viene richiesto e gestito sulla
piattaforma PagoLight** **(heidipay) ( <https://pagolight.it> ).**

![](./assets/media/image141.png)

Nel momento in cui si dovesse decidere di attivare questa modalità di
pagamento, Passweb offre anche la possibilità di inserire, direttamente
nella scheda prodotto, il relativo widget per mostrare all'utente una
possibile simulazione di rateizzazione, collegata ovviamente al prezzo
di quello specifico articolo (per maggiori informazioni in merito si
veda anche quanto indicato all'interno del capitolo "*Componenti
Ecommerce -- Componenti interni ai componenti Ecommerce -- Componente
Simulatore del Pagamento*" di questo manuale)

Una volta selezionata questa particolare modalità di pagamento l'utente
verrà quindi ricondotto sulla relativa piattaforma dove dovrà fornire
tutta la documentazione e i dati richiesti per l'approvazione del
finanziamento e per poter quindi concludere correttamente il proprio
ordine.

Per attivare questa particolare modalità di pagamento in Passweb sarà
necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione
    **PagoLight**

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **"Lista dei Metodi di Pagamento"**
    precedentemente esaminata.

3.  Attivare questa nuova modalità di pagamento secondo quanto descritto
    nel capitolo *"Configurazione Modalità di Pagamento"* di questo
    manuale.

4.  Impostare in maniera corretta i parametri specifici per questa
    particolare modalità di pagamento.

In particolare per poter eseguire quest'ultimo passaggio sarà necessario
selezionare il pagamento in oggetto all'interno della maschera **"Lista
dei Metodi di Pagamento"** e cliccare sul pulsante "**Modifica
Pagamento**", presente nella barra degli strumenti.

Verrà quindi visualizzata la maschera di configurazione e
personalizzazione del pagamento, all'interno della quale sarà necessario
impostare, oltre ai parametri classici di configurazione del pagamento,
anche quelli specifici del gateway attualmente considerato e presenti
all'interno della sezione "**Parametri Gateway**"

![](./assets/media/image142.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Merchant Key:** chiave segreta. Indispensabile per poter realizzare
  correttamente l'integrazione tra la piattaforma di finanziamento ed il
  proprio sito Ecommerce.

- **Codice tabella:** opzionale e solo per contratti **PagoLight Pro**.
  Consente di indicare il codice tabella abilitato e collegato al
  proprio contratto PagoLight Pro

> **ATTENZIONE!** Merchant Key e Codice tabella dovranno essere forniti
> all'esercente al momento della sottoscrizione del relativo contratto
> con la piattaforma di PagoLight.
>
> Un'eventuale discordanza tra i dati inseriti nei campi di
> configurazione e quelli forniti all'esercente da PagoLight renderà
> impossibile agli utenti del sito utilizzare questa modalità di
> pagamento.

- **Numero di rate:** consente di inserire il numero di rate (separate
  dal carattere ,) che dovranno poi essere considerate dal simulatore di
  pagamento per mostrare una simulazione delle diverse possibili opzioni
  di rateizzazione che la piattaforma terza offrirà all'utente.

> **ATTENZIONE!** Ovviamente le diverse possibili rate inserite
> all'interno di questo campo (e utilizzate poi dal simulatore) dovranno
> essere coerenti con quelle che verranno effettivamente mostrate
> all'utente in fase di pagamento sul gateway della piattaforma terza.
> **Si consiglia quindi di rivolgersi direttamente a Pago Light per
> sapere quali configurazioni di rate sono effettivamente accettate
> dalla piattaforma**

- **Script simulatore di pagamento:** consente di inserire e gestire il
  codice necessario per visualizzare all'interno del sito (pagina
  Prodotto e pagina Checkout) il simulatore di pagamento.

> Per maggiori informazioni relativamente a come poter configurare e
> utilizzare il simulatore di pagamento messo a disposizione
> direttamente da Pagolight si rimanda a quanto indicato nel successivo
> capitolo di questo manuale.

**ATTENZIONE!** in fase di configurazione di questo pagamento occorre
considerare **che la richiesta del finanziamento con rateizzazione
online potrà avvenire solo ed esclusivamente per ordini di un certo
importo**

Altra cosa di fondamentale importanza da tenere sempre in considerazione
è che nel momento in cui si dovesse tentare di utilizzare il pagamento
in questione per importi inferiori all'importo minimo effettivamente
utilizzato dalla piattaforma terza, **non verrà visualizzato il relativo
simulatore e confermando l'ordine questo verrà comunque acquisito da
Passweb restando però in stato di "Pagamento non confermato"** (la
piattaforma terza non ritorna infatti uno specifico messaggio di errore
necessario per poter gestire questo tipo di casistica)

**Per evitare questo tipo di errori diventa quindi indispensabile agire
mediante i campi "Limite minimo / massimo" presenti nella sezione
"Informazioni generali" della maschera di configurazione del pagamento
stesso**

![Videate\\soisy_3.bmp](./assets/media/image95.png)

In questo modo saremo quindi sicuri che questa specifica modalità di
pagamento verrà proposta al cliente solo ed esclusivamente nel caso in
cui l'importo del suo ordine sia tale da poter effettivamente avviare la
richiesta di rateizzazione.

**ATTENZIONE!** Gli importi settati all'interno dei campi "Limite Minimo
/ Massimo" determineranno anche la visualizzazione o meno del relativo
simulatore di pagamento eventualmente inserito nelle varie pagine
prodotto.

**Si consiglia di rivolgersi direttamente a Pago Light per informazioni
sempre aggiornate relativamente agli importi minimi/massimi accettai per
questo tipo di pagamento, importi questi che andranno poi inseriti nei
capi spora evidenziati.**

Una volta settati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", e posto, ovviamente, di
soddisfare eventuali condizioni di applicabilità impostate per il
pagamento in esame, in fase di checkout comparirà anche l'opzione
relativa a Pagolight.

![](./assets/media/image143.png)

Nel momento in cui l'utente dovesse poi decidere di utilizzare
effettivamente questo tipo di pagamento, alla conferma dell'ordine, il
documento sarà memorizzato nel database di Passweb, e l'utente verrà
reindirizzato automaticamente sulla piattaforma di PagoLight dove potrà
completare la propria richiesta.

![](./assets/media/image144.png)

Una volta selezionato il numero di rate desiderato l'utente dovrà
inserire i dati necessari per completare la richiesta di finanziamento,
compresi quelli relativi alla carta di credito

![](./assets/media/image145.png)

Durante i vari step di inserimento dati sulla piattaforma di PagoLight
si avrà sempre la possibilità di annullare la richiesta in essere
cliccando sul relativo link presente nella parte bassa della pagina

![](./assets/media/image146.png)

In questo caso l'utente verrà reindirizzato al sito ecommerce dove si
troverà l'ordine iniziale in stato di "**Pagamento non confermato**".

**Nel momento in cui dovesse decidere di confermare l'acquisto con un
altro metodo di pagamento dovrà quindi procedere alla creazione di un
nuovo ordine**

Nel caso in cui, invece, siano stati inseriti tutti i dati richiesti da
PagoLight portando a termine correttamente la richiesta di
finanziamento, l'utente verrà automaticamente riportato sul sito
Ecommerce dove l'ordine risulterà ora concluso in maniera corretta.

**NOTA BENE**: all'interno del gestionale verranno inseriti solo ed
esclusivamente gli ordini per i quali è stata ricevuta dalla piattaforma
PagoLight, relativamente alla richiesta di finanziamento in essere, una
risposta positiva.

**ATTENZIONE!** **Pago Light supporta la modalità Server to Server**. In
tale modalità l'applicazione di back office del gateway di pagamento
invierà una notifica al sito per gestire l'esito della transazione anche
nel caso in cui l'acquirente non dovesse fare ritorno sul sito
dell'esercente (ad esempio perché a transazione conclusa chiude
semplicemente il browser).

In ogni caso se, per qualsiasi ragione, il sito Ecommerce non dovesse
ricevere risposta dalla piattaforma terza Passweb non potrà sapere se la
transazione è stata o meno conclusa correttamente per cui il relativo
ordine resterà unicamente all'interno del database del sito nello stato
di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

