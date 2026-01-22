# FLAGPAY



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche appoggiate al gateway di pagamento **FlagPay**.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione FlagPay

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_flagpay.bmp](./assets/media/image102.png)

Nello specifico all'interno di questa sezione il campo:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **PSPID:** Codice identificativo dell'account FlagPay assegnato
  all'esercente in fase di attivazione del servizio

- **Chiave di sicurezza:** chiave di sicurezza dell'account assegnata
  all'esercente in fase di attivazione del servizio

**NOTA BENE**: le informazioni da inserire nei campi PSPID e Chiave di
sicurezza **sono obbligatorie** e non sono reperibili sul gestionale ma
vengono fornite direttamente all'esercente, al momento della sua
adesione al servizio offerto. Una eventuale discordanza tra i dati
inseriti in questi campi e quelli forniti all'esercente, renderà
impossibile agli utenti del sito utilizzare questa modalità di pagamento

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate dovrà avvenire in maniera **"Immediata"**
  (Vendita) o **"Differita"** (Autorizzazione). Una contabilizzazione
  immediata, ad esempio, permetterà all'esercente di rendere
  automaticamente contabili tutte le transazione autorizzate, senza un
  suo specifico intervento dall' applicazione di Back Office della
  banca.

> Una contabilizzazione differita richiederà invece che le operazioni
> autorizzate siano esplicitamente rese contabili dall'esercente
> attraverso la relativa applicazione di Back Office fornita dalla
> banca.

Oltre a questo, per consentire una corretta integrazione tra il proprio
sito Passweb e il gateway di pagamento, occorrerà configurare
correttamente anche la relativa applicazione di backoffice.

Nello specifico sarà quindi necessario:

- Accedere, nell'applicazione di backoffice della banca, alla sezione
  "**Configurazione -- Informazioni Tecniche -- Parametri Globali di
  sicurezza**" e selezionare, in corrispondenza del parametro "**Metodo
  di hashing**" l'opzione "**SHA-512**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_1.bmp](./assets/media/image103.png)

- Accedere alla sezione "**Configurazione -- Informazioni Tecniche --
  Ritorno d'informazione della transazione**" e selezionare l'opzione
  "**Desidero ricevere i parametri di ritorno delle transazioni sugli
  URL di redirezione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_2.bmp](./assets/media/image104.png)

- Rimanendo all'interno della sezione "**Configurazione -- Informazioni
  Tecniche -- Ritorno d'informazione della transazione**" selezionare,
  all'interno della sezione "**Richiesta server-to-server via diretta
  HTTP**" l'opzione "**Sempre differita (non immediatamente dopo il
  pagamento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_3.bmp](./assets/media/image105.png)

> e successivamente inserire all'interno dei campi "**Se lo statuto del
> pagamento è accettato, in attesa o incerto"** e **"Se lo statuto del
> pagamento è annullato dal cliente o troppi rigetti dell' acquirente**"
> il seguente url
>
> **https://www.miosito.it/store/cart/checkout/flagpay/s2s**
>
> dove al posto di www.miosito.it andrà inserito, ovviamente,
> l'indirizzo del proprio sito web

- Verificare, infine, che all'interno della sezione "**Parametri
  ecommerce dinamici**" siano correttamente inseriti all'interno del box
  "**Selezionato**" i campi **ORDERID, STATUS, NCERROR e PAYID**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_4.bmp](./assets/media/image106.png)

**ATTENZIONE!** Gli ultimi due punti sono di fondamentale importanza per
poter abilitare le chiamate server to server consentendo quindi al
gateway di pagamento di comunicare al sito Passweb se la transazione è
andata o meno a buon fine anche nel momento in cui l'utente dovesse
chiudere il browser prima di fare ritorno al sito Ecommerce.

Una volta impostati correttamente tutti i parametri di configurazione
(sia quelli presenti su Passweb che quelli indicati in riferimento
all'applicazione di back office del gateway di pagamento), se l'utente
dovesse, alla conferma dell'ordine, selezionare la modalità di pagamento
in esame, l'ordine sarà memorizzato nel database di Passweb, e l'utente
verrà reindirizzato sul sito del gateway di pagamento dove dovrà
inserire i dati necessari per concludere la transazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_5.bmp](./assets/media/image107.png)

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto oppure di
portare a termine l'acquisto e completare la transazione.

Nel primo caso l'utente verrà reindirizzato al sito ecommerce dove si
troverà l'ordine ancora da confermare. Volendo potrà dunque decidere di
ripartire dalla situazione attuale, modificando se necessario l'ordine
in essere con l'aggiunta o l'eliminazione di determinati articoli,
selezionando altre tipologie di trasporto e /o altri pagamenti ecc...
per poi passare nuovamente a concludere l'ordine.

Nel secondo caso, una volta confermata la transazione verrà presentata
all'utente una pagina con la conferma del pagamento appena effettuato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flagpay_6.bmp](./assets/media/image108.png)

e, dopo pochi secondi, sarà automaticamente ricondotto al sito
Ecommerce. L'ordine verrà considerato valido ed inserito quindi
all'interno del gestionale

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **FlagPay supporta la modalità Server to Server**
(necessita configurazione all'interno dell'applicazione di backoffice
della banca secondo quanto precedentemente indicato).

In tale modalità l'applicazione di back office della banca invierà una
notifica al sito per gestire l'esito della transazione anche nel caso in
cui l'acquirente non dovesse fare ritorno sul sito dell'esercente (ad
esempio perché a transazione conclusa chiude semplicemente il browser).

Per attivare questa modalità è però necessario configurare correttamente
l'applicazione di back office del gateway di pagamento

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

