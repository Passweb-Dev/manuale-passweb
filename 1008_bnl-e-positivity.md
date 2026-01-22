# BNL E-POSITIVITY



La modalità di pagamento etichettata a default come BNL e-POSitivity
viene riconosciuta e gestita da tutte le banche che utilizzano il
relativo gateway di pagamento.

e--POSitivity Connect è la soluzione di pagamento più semplice che BNL
POSitivity offre per collegare il vostro negozio online alla piattaforma
per pagamenti via Internet di e--POSitivity. BNL POSitivity, una volta
ricevuti i dati tramite Connect, si preoccuperà di gestire tutte le
interazioni necessarie con i circuiti di credito per elaborare la
transazione in modo corretto.

e--POSitivity consente di accettare una vasta gamma di circuiti:

- L'accettazione delle carte Visa, Visa Electron, MasterCard e Maestro è
  compresa nel contratto di convenzionamento stipulato con BNL
  POSitivity. Per alcune categorie merceologiche è possibile che vi
  siano delle restrizioni nell'accettazione delle carte MasterCard e
  Maestro: in tali casi BNL POSitivity fornisce un avviso preventivo in
  fase di definizione del contratto.

- Le carte Maestro sono accettate esclusivamente in modalità Connect e
  solo se sulla carta è attivo il servizio di sicurezza 3D Secure
  SecureCode. Per informazioni visitare:
  http://www.maestrocard.com/it/esercizicommerciali/index.html

- Per i circuiti American Express, Diners e JCB è necessario
  sottoscrivere gli appositi moduli di convenzione con i rispettivi
  circuiti; la modulistica è disponibile contattando la propria Agenzia
  BNL, il proprio Agente BNL POSitivity o il Servizio Esercenti BNL
  POSitivity. BNL POSitivity provvederà ad inoltrare il contratto e ad
  attivare il circuito automaticamente al momento della ricezione del
  codice di convenzione assegnato.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione BNL
    e-POSitivity

<!-- -->

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

![](./assets/media/image52.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Store ID:** codice esercente che identifica il negozio sui sistemi
  di BNL POSitivity

- **Shared Secret:** codice segreto fornito all'esercente dalla banca
  all'adesione del servizio

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate dovrà avvenire in maniera **"Immediata"**
  o **"Differita"**. Una contabilizzazione immediata, ad esempio,
  permetterà all'esercente di rendere automaticamente contabili tutte le
  transazione autorizzate, senza un suo specifico intervento dall'
  applicazione di Back Office della banca.

> Una contabilizzazione differita richiederà invece che le operazioni
> autorizzate siano esplicitamente rese contabili dall'esercente
> attraverso la relativa applicazione di Back Office fornita dalla
> banca.

**NOTA BENE**: BNL e-POSitivity gestisce solamente importi in euro; per
eventuali ordini in valuta il totale del documento verrà quindi
opportunamente convertito in euro e passato alla banca

- **Modalità:** consente di selezionare la specifica modalità di
  funzionamento che dovrà essere adottata da questo sistema di
  pagamento. Abilitando una modalità piuttosto che un'altra potranno
  variare le informazioni richieste dalla banca stessa ai fini di una
  corretta acquisizione dell'ordine e della relativa transazione.
  Attualmente è gestita la sola modalità **PayOnly**:

Le informazioni da inserire nei campi sopra indicati sono di
fondamentale importanza in quanto saranno poi quelle che consentiranno
di accedere al gateway di pagamento e di poter così portare a termine il
pagamento tramite carta di credito.

**NOTA BENE**: un'eventuale discordanza tra i dati inseriti nei campi
sopra indicati e quelli forniti all'esercente dalla banca, renderà
impossibile agli utenti del sito utilizzare questa modalità di
pagamento.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame,
l'ordine sarà memorizzato nel database di Passweb, e l'utente verrà
reindirizzato alla specifica pagina di accesso del gateway "BNL
e-POSitivity" dove, per completare il pagamento, gli verranno richieste
diverse informazioni.

![](./assets/media/image53.png)

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (link
"Annulla e Torna al sito ...") oppure di portare a termine l'acquisto e
completare la transazione.

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

Nel secondo caso (conferma della transazione), dopo aver inserito i dati
necessari per completare il pagamento (carta di credito, codice di
sicurezza ecc...), l'ordine verrà preso in carico e gestito direttamente
dall'applicazione della banca.

Completato il pagamento in maniera corretta l'ordine verrà inserito
nell'applicazione di Back Office della banca e il cliente verrà
automaticamente ricondotto alla pagina di "Ordine Confermato" del sito
e-commerce.

Il numero ordine che viene riportato nella mail o visualizzato nel Back
Office rappresenta l'identificativo dell'ordine sul database di Passweb.
Per determinare la sigla ordine gestionale corrispondente
all'identificativo è necessario utilizzare la pagina Gestione Ordini del
Wizard. Effettuando infatti una ricerca per identificativo, verrà
visualizzato il record indicante la sigla dell'ordine utilizzata sul
gestionale (se l'ordine è già stato registrato, se l'ordine non è stato
ancora inserito sul gestionale il campo sarà invece vuoto).

**NOTA BENE**: eventuali mail di notifica di avvenuta transazione, così
come accrediti e addebiti sui relativi c/c sono gestiti totalmente
dall'applicazione della banca.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta una risposta positiva
dall'applicazione della banca.

**ATTENZIONE!** **BNL e-POSitivity supporta la modalità Server to
Server**. In tale modalità l'applicazione di back office della banca
invierà una notifica al sito per gestire l'esito della transazione anche
nel caso in cui l'acquirente non dovesse fare ritorno sul sito
dell'esercente (ad esempio perché a transazione conclusa chiude
semplicemente il browser).

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali l'applicazione di Back Office non ha restituito alcuna
risposta tali ordini resteranno unicamente all'interno del database di
Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office della banca potrebbe non
essere allineato con la corrente versione di tale software. Si consiglia
quindi di utilizzare la specifica manualistica.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o all' applicazione di Back Office, occorre
rivolgersi alla relativa assistenza.

