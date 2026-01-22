# AFONE PAIMENT



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche appoggiate al gateway di pagamento **Afone Paiment**
(https://www.afonepaiement.com).

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione Afone
    Paiment

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **" Lista dei Metodi di Pagamento"**
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
all'interno della sezione "**Parametri Gateway**

![](./assets/media/image39.png)

Nello specifico all'interno della sezione "**Configurazione Parametri
del Gateway**" sarà possibile indicare se utilizzare l'ambiente di test
oppure l'ambiente reale di produzione

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Virtual POS Terminal ID:** codice identificativo dell'esercente

- **Private Key:** codice fornito all'esercente direttamente dalla banca
  all'atto della sua adesione al servizio

**NOTA BENE**: le informazioni da inserire nei campi Virtual POS
Terminal ID e Private Key **sono obbligatorie** e non sono reperibili
sul gestionale ma vengono fornite direttamente all'esercente, al momento
della sua adesione al servizio offerto. Una eventuale discordanza tra i
dati inseriti in questi campi e quelli forniti all'esercente dalla
banca, renderà impossibile agli utenti del sito utilizzare questa
modalità di pagamento

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate dovrà avvenire in maniera **"Immediata"**
  o **"Differita"**. Una contabilizzazione immediata, ad esempio,
  permetterà all'esercente di rendere automaticamente contabili tutte le
  transazione autorizzate, senza un suo specifico intervento dall'
  applicazione di Back Office della banca.

> Una contabilizzazione differita (Pre-autorizzazione) richiederà invece
> che le operazioni autorizzate siano esplicitamente rese contabili
> dall'esercente attraverso la relativa applicazione di Back Office
> fornita dalla banca.

Una volta impostati correttamente i parametri presenti all'interno delle
due sezioni appena analizzate, se l'utente dovesse, alla conferma
dell'ordine, selezionare la modalità di pagamento in esame, l'ordine
sarà memorizzato nel database di Passweb, e l'utente verrà reindirizzato
sul sito del gateway di pagamento dove dovrà inserire i relativi dati.

![](./assets/media/image40.png)

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"**Annulla**") oppure di portare a termine l'acquisto e completare la
transazione.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine già confermato
e non avrà modo di modificarlo. Come detto, infatti l'ordine viene
memorizzato nel database di Passweb prima che l'utente venga ricondotto
al sito della banca.

In queste condizioni però l'utente non ha ancora effettuato il pagamento
per cui l'ordine, memorizzato nel database di Passweb, assumerà lo stato
di "**Pagamento Non Confermato**" e, conseguentemente, alla
sincronizzazione non verrà inserito in maniera automatica all'interno
del gestionale.

**In queste stesse condizioni, nel caso in cui l'utente volesse
effettuare comunque l'ordine utilizzando però una diversa modalità di
pagamento, dovrà ripartire da zero inserendo gli articoli in carrello ed
effettuando nuovamente la procedura di checkout.**

Nel secondo caso, una volta confermata la transazione ed inserito
eventualmente anche il codice per il 3D secure verrà presentata
all'utente una pagina web con il riassunto dei dati relativi alla
transazione in essere.

![](./assets/media/image41.png)

Cliccando sul pulsante "**Torna la negozio**" l'utente sarà ricondotto
automaticamente al sito Ecommerce, l'ordine verrà considerato valido ed
inserito quindi all'interno del gestionale

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **Afone Paiment supporta la modalità Server to Server**.
In tale modalità l'applicazione di back office della banca invierà una
notifica al sito per gestire l'esito della transazione anche nel caso in
cui l'acquirente non dovesse fare ritorno sul sito dell'esercente (ad
esempio perché a transazione conclusa chiude semplicemente il browser).

Per abilitare la modalità server to server è però necessario accedere al
back end del proprio account esercente Afone, portarsi all'interno della
sezione "**Configuiration -- MyURLs**" e inserire il dominio del proprio
sito all'interno del box "**Allow domain for IPN**"

![](./assets/media/image42.png)

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali l'applicazione di Back Office non ha restituito alcuna
risposta tali ordini resteranno unicamente all'interno del database di
Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di utilizzare la specifica
manualistica.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà del Gateway di paramento occorre rivolgersi alla relativa
assistenza.

