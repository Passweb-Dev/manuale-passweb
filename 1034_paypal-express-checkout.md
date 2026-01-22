# PAYPAL EXPRESS CHECKOUT



La procedura di pagamento rapido messa a disposizione da PayPal, e
marcata all'interno di Passweb come **PayPal Express Checkout,**
consente ai clienti di completare la transazione in poche semplici fasi.
Utilizzando questa modalità di pagamento infatti i clienti avranno la
possibilità di accedere ai dati di spedizione e di fatturazione
memorizzati in modo sicuro all'interno di PayPal, dati questi che
verranno poi ritrasmessi da PayPal al sito Ecommerce dove il cliente
potrà completare immediatamente il proprio acquisto.

Per poter utilizzare questa modalità di pagamento è necessario disporre
di un account PayPal Business

**ATTENZIONE**: **nel caso in cui il sito venga richiamato all'interno
di un iframe il pagamento tramite PayPal potrebbe non funzionare in
maniera corretta. Tali malfunzionamenti non sono da ricondurre a Passweb
ma a PayPal stesso i cui moduli di pagamento non possono essere inseriti
all'interno di iframe**

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione PAYPAL
    EXPRESS CHECKOUT

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **"Lista dei Metodi di Pagamento"**
    precedentemente esaminata.

<!-- -->

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_paypal_express.bmp](./assets/media/image180.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

> E' sempre consigliabile verificare per prima cosa la corretta
> integrazione tra il sistema di pagamento ed il proprio sito web in un
> ambiente di test per poi passare solo successivamente all'ambiente
> Live di produzione. Per maggiori informazioni su come creare una
> account PayPal di test si veda anche il successivo capitolo di questo
> manuale.

- **API Username:** nome utente generato direttamente da PayPal e
  associato quindi al profilo di test (sandbox) o di produzione di
  PayPal stesso cui si vuole collegare il proprio sito e-commerce

- **API Password:** password utente generata direttamente da PayPal e
  associata quindi al profilo di test (sandbox) o di produzione di
  PayPal stesso cui si vuole collegare il proprio sito e-commerce

- **Signature:** firma digitale univoca generata direttamente da PayPal
  come riga di testo o simboli hash e associata al profilo di test
  (sandbox) o di produzione di PayPal stesso cui si vuole collegare il
  proprio sito e-commerce

- **Contabilizzazione:** permette di specificare se la transazione è un
  pagamento per una vendita definitiva (Vendita) o un\'autorizzazione
  per una vendita definitiva da riscuotere in seguito (Autorizzazione).

- **Client ID / Secret Stringa** -- **dati non obbligatori** -- chiavi
  di configurazione dell'App PayPal utilizzata per gestire al meglio
  l'integrazione tra il proprio sito e la modalità di pagamento PayPal
  in esame.

> **ATTENZIONE!** i valori da inserire all'interno dei campi Client ID e
> Secret Stringa dovranno essere prelevati dall'APP appositamente creata
> nell'ambiente developer di PayPal. Per maggiori informazioni in merito
> si veda anche il successivo capitolo ("*PayPal Checkout -- Creazione
> App*") di questo manuale

**Le informazioni presenti all'interno di questa sezione sono di
fondamentale importanza in quanto saranno poi quelle che garantiranno la
corretta integrazione tra Passweb e il sistema di pagamento PayPal
Express Checkout mettendo così l'utente nelle condizioni di poter
portare a termine il proprio acquisto.**

**NOTA BENE**: per maggiori informazioni relativamente alle modalità di
creazione di un account PayPal e/o allo specifico funzionamento della
modalità Express Checkout si rimanda alla specifica documentazione
reperibile in rete.

Di seguito verranno illustrati i principali punti della procedura di
attivazione di un account PayPal di test (Sandbox) e/o di produzione cui
poter poi collegare, in maniera corretta, il metodo di pagamento in
esame, oltre ovviamente alle specifiche modalità di utilizzo di questa
stessa modalità di pagamento all'interno del proprio sito Passweb.

