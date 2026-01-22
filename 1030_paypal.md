# PAYPAL



Per poter abilitare questa particolare modalità di pagamento è
necessario disporre di un Account Business o Premiere all'interno del
sistema PayPal.

**ATTENZIONE**: **nel caso in cui il sito venga richiamato all'interno
di un iframe il pagamento tramite PayPal potrebbe non funzionare in
maniera corretta. Tali malfunzionamenti non sono da ricondurre a Passweb
ma a PayPal stesso i cui moduli di pagamento non possono essere inseriti
all'interno di iframe**

Soddisfatta questa condizione indispensabile, per poter poi attivare
questa specifica modalità di pagamento in Passweb sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione PAYPAL

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

![](./assets/media/image159.png)

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

- **Email conto PayPal:** Email inserita dall'utente in fase di
  attivazione del proprio account PayPal

<!-- -->

- **Nome del Carrello:** stringa descrittiva che verrà visualizzata
  all'interno dell'applicazione di Back Office di PayPal in
  corrispondenza dell'importo relativo alla transazione effettuata
  (identificativa del sito o del venditore da cui il cliente ha
  effettuato l'acquisto)

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate dovrà avvenire in maniera **"Immediata"**
  o **"Differita"**. Una contabilizzazione immediata, ad esempio,
  permetterà all'esercente di rendere automaticamente contabili tutte le
  transazione autorizzate, senza un suo specifico intervento dall'
  applicazione di Back Office.

> Una contabilizzazione differita richiederà invece che le operazioni
> autorizzate siano esplicitamente rese contabili dall'esercente
> attraverso la relativa applicazione di Back Office.

- **Client ID / Secret Stringa** -- **dati non obbligatori** -- chiavi
  di configurazione dell'App PayPal utilizzata per gestire al meglio
  l'integrazione tra il proprio sito e la modalità di pagamento PayPal
  in esame.

> **ATTENZIONE!** i valori da inserire all'interno dei campi Client ID e
> Secret Stringa dovranno essere prelevati dall'APP appositamente creata
> nell'ambiente developer di PayPal. Per maggiori informazioni in merito
> si veda anche il successivo capitolo ("*PayPal Checkout -- Creazione
> App*") di questo manuale

- **Sovrascrivi indirizzo**: consente, se selezionato, di sovrascrivere
  (limitatamente alla transazione in esame) l'indirizzo eventualmente
  presente su PayPal con l'indirizzo di spedizione indicato dall'utente
  in fase di ordine

**Le informazioni presenti all'interno di questa sezione sono di
fondamentale importanza in quanto saranno poi quelle che consentiranno
di accedere all'applicazione di Back Office di PayPal e di poter così
portare a termine correttamente il pagamento on-line tramite carta di
credito.**

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame,
verrà reindirizzato alla specifica pagina di accesso del gateway di
PayPal dove potrà scegliere se pagare con carta di credito (pulsante
"**Paga con una carta**") oppure utilizzando il proprio account PayPal
(pulsante "**Accedi**" dopo aver inserito le credenziali del proprio
account)

![](./assets/media/image160.png)

**A questo punto però l'ordine non è ancora stato preso in carico da
PayPal e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"Annulla" nella parte bassa della pagina) oppure di portare a termine
l'acquisto e completare la transazione.

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

Nel secondo caso, una volta scelta la modalità di pagamento (Carta o
Account PayPal ) verrà presentata all'utente una pagina web con il
riassunto dei dati relativi alla transazione in essere.

![](./assets/media/image161.png)

Cliccando sul pulsante "**Paga Adesso**" verrà completata la relativa
transazione verrà mostrato all'utente una maschera di ringraziamento con
all'interno un pulsante per poter tornare al sito Ecommerce di
provenienza (pulsante "**Torna sul sito del venditore**"), e
contestualmente, verrà comunque ritornata al sito Ecommerce risposta
positiva (**implementazione "Server to Server"**).

![](./assets/media/image162.png)

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**ATTENZIONE!** **PayPal supporta la modalità Server to Server**. In
tale modalità il gateway di PayPal invierà una notifica al sito per
gestire l'esito della transazione anche nel caso in cui l'acquirente non
dovesse fare ritorno sul sito dell'esercente (ad esempio perché a
transazione conclusa chiude semplicemente il browser).

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali la piattaforma di finanziamento non ha restituito alcuna
risposta tali ordini resteranno unicamente all'interno del database di
Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

Nel successivo capitolo verranno illustrati i principali punti della
procedura di attivazione di un account PayPal di test (Sandbox), account
questo che potrà poi essere utilizzato, prima di passare all'ambiente di
produzione, per verificare che tutto funzioni in maniera corretta.

