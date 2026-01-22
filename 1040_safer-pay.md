# SAFER PAY



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche che offrono il servizio **"SaferPay"**.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione SAFER PAY

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_safer_pay.bmp](./assets/media/image188.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Numero del Cliente:** numero identificativo del cliente fornito
  dalla banca all'atto dell'adesione al servizio

- **Terminale:** codice terminale fornito dalla banca all'atto
  dell'adesione al servizio

- **Nome Utente API:** nome utente associato all'API utilizzata per
  l'integrazione con il servizio

- **Password API:** password utente associata all'API utilizzata per
  l'integrazione con il servizio

**NOTA BENE**: le informazioni da inserire nei campi Numero del Cliente,
Terminale, Nome Utente API e Password API non sono reperibili sul
gestionale ma vengono fornite direttamente all'esercente dalla banca, al
momento della sua adesione al servizio offerto oppure devono essere
reperite nelle apposite sezione dell'applicazione di Back Office della
banca. Un'eventuale discordanza tra i dati inseriti e quelli forniti
all'esercente dalla banca, renderà impossibile agli utenti del sito
utilizzare questa modalità di pagamento.

In particolare per quel che riguarda il "**Nome Utente API"** e la
"**Password API**" tali dati dovranno essere opportunamente generati
all'interno della relativa applicazione di Back Office accedendo alla
sezione "**Impostazioni -- JSON API Basic Authentication**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\safer_pay_backoffice.bmp](./assets/media/image189.png)

**NOTA BENE**: Safer Pay consente di gestire anche pagamenti in valuta.

Per maggiori dettagli relativi alla specifica applicazione di BackOffice
si rimanda ai relativi manuali.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office di Safer Pay potrebbe non
essere allineato con la corrente versione di tale software. Si consiglia
quindi di utilizzare la specifica manualistica reperibile dal sito della
banca.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà di Safer Pay occorre rivolgersi alla relativa assistenza.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame,
l'ordine sarà memorizzato nel database di Passweb, e l'utente verrà
reindirizzato alla specifica pagina di accesso del gateway di pagamento:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\saferpay_1.bmp](./assets/media/image190.png)

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"Interrompi") oppure di portare a termine l'acquisto e completare la
transazione.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine ancora da
confermare. Volendo potrà dunque decidere di ripartire dalla situazione
attuale, modificando se necessario l'ordine in essere con l'aggiunta o
l'eliminazione di determinati articoli, selezionando altre tipologie di
trasporto e /o altri pagamenti ecc... per poi passare nuovamente a
concludere l'ordine.

In queste condizioni dunque non essendo concluso, l'ordine non verrà
ovviamente memorizzato nel database di Passweb né tanto meno verrà
inserito in Mexal

Nel secondo caso, cliccando sul pulsante "**Acquistare**" potrà essere
mostrata un'ulteriore per la gestione del 3D Secure

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\saferpay_4.bmp](./assets/media/image191.png)

Completato anche questo passaggio l'ordine verrà definitivamente preso
in carico dalla banca

Il numero ordine riportato nella mail o visualizzato nel Back Office
rappresenta l'identificativo dell'ordine sul database di Passweb. Per
determinare la sigla ordine gestionale corrispondente all'identificativo
è necessario utilizzare la pagina Gestione Ordini del Wizard.
Effettuando infatti una ricerca per identificativo, verrà visualizzato
il record indicante la sigla dell'ordine utilizzata sul gestionale (se
l'ordine è già stato registrato, se l'ordine non è stato ancora inserito
sul gestionale il campo sarà invece vuoto).

**NOTA BENE**: eventuali mail di notifica di avvenuta transazione, così
come accrediti e addebiti sui relativi c/c sono gestiti totalmente
dall'applicazione di Back Office della Banca.

Nel caso in cui siano stati effettuati ordini a seguito dei quali
l'applicazione di Back Office non ha restituito alcuna risposta (ad
esempio perché è stato chiuso il browser prima del ritorno al sito di
e-commerce), come nel caso di annullamento della procedura di pagamento,
tali ordini resteranno unicamente all'interno del database di Passweb
nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

