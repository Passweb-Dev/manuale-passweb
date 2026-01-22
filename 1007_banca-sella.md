# BANCA SELLA



Questa modalità di pagamento online viene attualmente riconosciuta e
gestita da tutte le banche che aderiscono al circuito **"Banca Sella"**.

**NOTA BENE**: attualmente, lato Passweb, è stata sviluppata, in questo
senso, l'integrazione con architettura basata su crittografia. All'atto
della sottoscrizione del contratto l'esercente dovrà quindi richiedere
l'attivazione di questa precisa modalità di pagamento.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione BANCA
    SELLA -- CRITTOGRAFIA

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_banca_sella.bmp](./assets/media/image46.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

> **ATTENZIONE! Gli url che andranno poi impostati nel back-end della
> banca per configurare correttamente il metodo di pagamento saranno
> diversi a seconda del fatto di lavorare in ambiente di test o di
> produzione**

- **Codice Esercente:** codice che identifica l'esercente, fornito da
  Banca Sella;

- **Versione:** consente di selezionare dal relativo menu a tendina la
  specifica versione (Basic, Advanced, Professional) della modalità di
  pagamento indicata dall'esercente all'atto della sottoscrizione del
  contratto con la banca.

**NOTA BENE**: le informazioni da inserire nei campi Codice Esercente e
Versione non sono reperibili sul gestionale ma vengono fornite
direttamente all'esercente da Banca Sella, al momento della sua della
sua adesione al servizio offerto.

Occorre poi considerare che la modalità di pagamento in esame identifica
(lato server Banca Sella) l\'esercente che richiede il servizio di
cifratura, confrontando l\'indirizzo IP del server chiamante con gli
indirizzi IP configurati dall\'esercente nell'apposita sezione
dell\'ambiente di BackOffice.

**Al fine di garantire il corretto funzionamento del pagamento on line
sarà quindi necessario accedere all'applicazione di Back Office della
banca con le credenziali fornite dalla banca stessa all'atto della
sottoscrizione del contratto, portarsi nella sezione**
"**Configurazione" e cliccare sulla voce "Indirizzi IP" in maniera tale
da accedere alla maschera di inserimento degli indirizzi IP abilitati
alle transazioni**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\banca_sella_indirizzi_ip.bmp](./assets/media/image47.png)

All'interno di questa maschera andranno quindi specificati i due
indirizzi IP di seguito riportati:

**89.186.34.\***

**89.186.36.\***

**NOTA BENE**: nel caso in cui tali indirizzi IP non vengano inseriti
correttamente, l'applicazione di BancaSella non sarà in grado di
riconoscere i server su cui risiede il sito Passweb. In queste
condizioni l'elaborazione della transazione terminerà restituendo uno
specifico messaggio di errore.

Una volta impostati gli indirizzi IP indicati sarà poi necessario
portarsi all'interno della sezione "**Sicurezza**", cliccare sulla voce
"**Livello Sicurezza**" e, nella relativa maschera, selezionare
l'opzione "**Verifica correttezza di almeno uno tra indirizzo IP e API
Key**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\banca_sella_indirizzi_ip_2.bmp](./assets/media/image48.png)

Infine, sempre all'interno dell'applicazione di Back Office di Banca
Sella sarà necessario impostare anche gli url cui la stessa applicazione
dovrà ritornare una risposta, sia essa positiva (transazione conclusa
correttamente) o negativa (transazione che per diverse ragioni non è
stata conclusa correttamente) oltre all' url per la gestione della
comunicazione server to server.

Per inserire queste informazioni sarà quindi necessario accedere ancora
una volta all'applicazione di back office della banca, portarsi nella
sezione **"*Configurazione"*** e cliccare questa volta "**Indirizzi
Risposte**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\banca_sella_8.bmp](./assets/media/image49.png)

All'interno della relativa maschera "Indirizzi Risposte" andranno quindi
inserite le seguenti informazioni:

- **E-mail informazioni:** indirizzo cui l'applicazione di Back Office
  di Banca Sella invierà tutte le eventuali mail di informazione;

- **E-mail per risposta positiva:** indirizzo cui l'applicazione di Back
  Office di Banca Sella invierà una mail in caso di esito positivo della
  transazione;

- **E-mail per risposta negativa:** indirizzo cui l'applicazione di Back
  Office di Banca Sella invierà una mail in caso di esito negativo della
  transazione.

- **URL per risposta positiva:** url cui l'applicazione di Back Office
  di Banca Sella dovrà ritornare una risposta positiva.

> Inserire all'interno di questo campo i seguenti indirizzi:

- **https://www.\[dominio
  sito\]/store/cart/checkout/bancasellatestcreditok --** da utilizzare
  nel caso in cui si stia lavorando in ambiente di test

- **https://www.\[dominio sito\]/store/cart/checkout/creditok --** da
  utilizzare nel caso in cui si stia lavorando in ambiente di produzione

<!-- -->

- **URL per risposta negativa:** url cui l'applicazione di Back Office
  di Banca Sella dovrà ritornare una risposta negativa.

> Inserire all'interno di questo campo i seguenti indirizzi:

- **https://www.\[dominio
  sito\]/store/cart/checkout/bancasellatestcreditko --** da utilizzare
  nel caso in cui si stia lavorando in ambiente di test

- **https://www.\[dominio sito\]/store/cart/checkout/creditko --** da
  utilizzare nel caso in cui si stia lavorando in ambiente di produzione

<!-- -->

- **URL Server to Server:** url utilizzato dall'applicazione di Banca
  Sella per la comunicazione Server to Server

> Inserire all'interno di questo campo i seguenti indirizzi:

- **https://www.\[dominio sito\]/store/cart/checkout/bancasellatests2s
  --** da utilizzare nel caso in cui si stia lavorando in ambiente di
  test

- **https://www.\[dominio sito\]/store/cart/checkout/server2server --**
  da utilizzare nel caso in cui si stia lavorando in ambiente di
  produzione

**ATTENZIONE!** Nella comunicazione Server to Server l'applicazione di
back office di Banca Sella invierà una notifica al sito per gestire
l'esito della transazione anche nel caso in cui l'acquirente non dovesse
fare ritorno sul sito dell'esercente (ad esempio perché a transazione
conclusa chiude semplicemente il browser). Per gestire correttamente
questo tipo di comunicazione evitando quindi di dover gestire, lato
Passweb, ordini nello stato di "Pagamento non confermato", si consiglia
di impostare sempre in maniera corretta anche l'URL Server to Server

Una volta impostati correttamente i parametri di configurazione presenti
sia lato Passweb che lato applicazione di Back office di Banca Sella,
nel momento in cui l'utente dovesse, alla conferma dell'ordine,
selezionare la modalità di pagamento in esame, l'ordine sarà memorizzato
nel database di Passweb, e l'utente verrà reindirizzato alla specifica
pagina di accesso del gateway GestPay in cui dovrà inserire i dati
relativi al pagamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\banca_sella_10.bmp](./assets/media/image50.png)

Prima di reindirizzare l\'utente al sito Banca Sella l\'ordine viene
sempre salvato all\'interno del database di Passweb e vengono
conseguentemente inviate (se è stata attivata la gestione delle mail) le
corrispondenti E-mail di Invio Ordine e di Informazione.

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"Torna al Negozio") oppure di portare a termine l'acquisto e completare
la transazione (pulsante "Procedi").

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine ancora da
confermare. Volendo potrà dunque decidere di ripartire dalla situazione
attuale, modificando se necessario l'ordine in essere con l'aggiunta o
l'eliminazione di determinati articoli, selezionando altre tipologie di
trasporto e /o altri pagamenti ecc... per poi passare nuovamente a
concludere l'ordine.

Nel momento in cui l'utente, una volta ritornato al sito, dovesse
comunque decidere di non chiudere l'ordine, questo resterebbe
memorizzato nel database di Passweb in stato di "**Pagamento non
confermato**"

Nel secondo caso (conferma della transazione) l\'ordine verrà preso in
carico e gestito, da questo momento in avanti, da Banca Sella. Verrà
quindi presentata all\'utente una pagina web (ricevuta digitale)
contenente i dati della transazione e gli verrà inviata una mail di
notifica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\banca_sella_11.bmp](./assets/media/image51.png)

Il numero ordine che viene riportato nella mail o visualizzato nel Back
Office rappresenta l\'identificativo dell\'ordine sul database di
Passweb. Per determinare la sigla ordine gestionale corrispondente
all\'identificativo è necessario utilizzare la pagina Gestione Ordini
del Wizard. Infatti, effettuando una ricerca per identificativo, verrà
visualizzato il record indicante la sigla dell\'ordine utilizzata sul
gestionale (se l\'ordine è già stato registrato, se l\'ordine non è
stato ancora inserito sul gestionale il campo sarà invece vuoto).

All\'esercente verranno notificate via mail tutte le transazioni
completate con successo.

**NOTA BENE**: le mail di notifica di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente
dall'applicazione di Banca Sella.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta una risposta positiva
dall'applicazione di Back Office di Banca Sella.

Nel caso in cui siano stati effettuati ordini a seguito dei quali
l'applicazione di Back Office non ha restituito alcuna risposta (ad
esempio perché è stato chiuso il browser prima del ritorno al sito di
e-commerce) , come nel caso di annullamento della procedura di
pagamento, tali ordini resteranno unicamente all'interno del database di
Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

**NOTA BENE**: Banca Sella gestisce solamente importi in euro; per
eventuali ordini in valuta il totale del documento verrà quindi
opportunamente convertito in euro e passato alla banca.

**ATTENZIONE! Per non dover gestire ordini in stato di "Pagamento non
Confermato" è necessario aver configurato correttamente la gestione
Server to Server**

Per informazioni più dettagliate relative alla gestione di addebiti e
accrediti sui rispettivi c/c e alla conseguente gestione dell'ordine da
parte di Banca Sella all'interno della sua applicazione di Back Office
rimandiamo alla relativa manualistica.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office di Banca Sella potrebbe
non essere allineato con la corrente versione di tale software. Si
consiglia quindi di utilizzare la specifica manualistica reperibile dal
sito della banca.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà di Banca Sella occorre rivolgersi alla relativa assistenza.

