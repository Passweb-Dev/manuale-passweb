# SARDEXNET



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche appoggiate al gateway di pagamento **Sardex.net**
(<https://www.sardex.net>).

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione Axepta

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
all'interno della sezione "**Parametri Gateway**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_sardexnet.bmp](./assets/media/image192.png)

Nello specifico all'interno di questa sezione il campo:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Username / Password:** credenziali di accesso al servizio (fornite
  all'esercente direttamente dal gateway di pagamento)

**NOTA BENE**: le informazioni da inserire nei campi Username e Password
**sono obbligatorie** e non sono reperibili sul gestionale ma vengono
fornite direttamente all'esercente, al momento della sua adesione al
servizio offerto. Una eventuale discordanza tra i dati inseriti in
questi campi e quelli forniti all'esercente, renderà impossibile agli
utenti del sito utilizzare questa modalità di pagamento

Una volta impostati correttamente i parametri presenti all'interno delle
due sezioni appena analizzate, se l'utente dovesse, alla conferma
dell'ordine, selezionare la modalità di pagamento in esame, l'ordine
sarà memorizzato nel database di Passweb, e l'utente verrà reindirizzato
sul sito del gateway di pagamento dove dovrà inserire i relativi dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sardexnet_1.bmp](./assets/media/image193.png)

**ATTENZIONE! Per poter concludere una transazione l'utente dovrà
accedere al gateway di pagamento con il proprio account. Nel caso in cui
non disponga di questo account dovrà quindi crearlo preventivamente**

Una volta effettuato l'accesso al gateway **l'ordine non è ancora stato
preso in carico dalla banca e, conseguentemente, non è ancora avvenuto
alcun pagamento**. L'utente potrà ancora decidere, quindi, di annullare
tutto oppure di portare a termine l'acquisto e completare la
transazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sardexnet_2.bmp](./assets/media/image194.png)

Nel primo caso (pulsante **Annulla**) l'utente verrà reindirizzato al
sito ecommerce dove si troverà l'ordine ancora da confermare. Volendo
potrà dunque decidere di ripartire dalla situazione attuale, modificando
se necessario l'ordine in essere con l'aggiunta o l'eliminazione di
determinati articoli, selezionando altre tipologie di trasporto e /o
altri pagamenti ecc... per poi passare nuovamente a concludere l'ordine.

Nel secondo caso (pulsante **Paga**), una volta confermata la
transazione verrà presentata all'utente una pagina con la conferma del
pagamento appena effettuato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sardexnet_3.bmp](./assets/media/image195.png)

e, dopo pochi secondi, sarà automaticamente ricondotto al sito
Ecommerce. L'ordine verrà considerato valido ed inserito quindi
all'interno del gestionale

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **Sardexnet supporta la modalità Server to Server**. In
tale modalità l'applicazione di back office della banca invierà una
notifica al sito per gestire l'esito della transazione anche nel caso in
cui l'acquirente non dovesse fare ritorno sul sito dell'esercente (ad
esempio perché a transazione conclusa chiude semplicemente il browser).

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

