# T.P@Y.SM



La modalità di pagamento etichettata a default come **T.P@Y.SM** viene
riconosciuta e gestita da tutte le banche che utilizzano il relativo
gateway di pagamento online.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione
    **T.P@Y.SM**

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_tpay.bmp](./assets/media/image246.png){width="5.545138888888889in"
height="3.265972222222222in"}

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Terminal ID:** codice terminale assegnato all\'esercente;

- **Chiave per firma digitale:** codice alfanumerico assegnato
  all\'esercente;

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

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del sistema "T.P@Y.SM"
potrebbe non essere allineato con la corrente versione di tale software.
Si consiglia quindi di utilizzare la specifica manualistica.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o all' applicazione di Back Office, occorre
rivolgersi alla relativa assistenza.

Le informazioni da inserire nei campi sopra indicati non sono reperibili
sul gestionale ma vengono fornite direttamente all'esercente dalla
banca, al momento della sua registrazione sul sito e/o della sua
adesione al servizio offerto.

Tali informazioni sono di fondamentale importanza in quanto saranno poi
quelle che consentiranno di accedere al gateway di pagamento e di poter
così portare a termine il pagamento tramite carta di credito.

**NOTA BENE**: un'eventuale discordanza tra i dati inseriti nei campi
sopra indicati e quelli forniti all'esercente dalla banca, renderà
impossibile agli utenti del sito utilizzare questa modalità di
pagamento.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame,
l'ordine sarà memorizzato nel database di Passweb, e l'utente verrà
reindirizzato alla specifica pagina di accesso del gateway di pagamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tpay_1.bmp](./assets/media/image247.png){width="4.7340277777777775in"
height="2.83125in"}

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"**Annulla**") oppure di portare a termine l'acquisto e completare la
transazione.

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

Nel secondo caso (conferma della transazione), dopo aver inserito i dati
richiesti, l'ordine verrà preso in carico e gestito, da questo momento
in avanti, dall'applicazione della banca.

Il numero ordine che viene riportato nella mail o visualizzato nel Back
Office rappresenta l'identificativo dell'ordine sul database di Passweb.
Per determinare la sigla ordine gestionale corrispondente
all'identificativo è necessario utilizzare la pagina Gestione Ordini del
Wizard. Effettuando infatti una ricerca per identificativo, verrà
visualizzato il record indicante la sigla dell'ordine utilizzata sul
gestionale (se l'ordine è già stato registrato, se l'ordine non è stato
ancora inserito sul gestionale campo sarà invece vuoto).

**NOTA BENE**: eventuali mail di notifica di avvenuta transazione, così
come accrediti e addebiti sui relativi c/c sono gestiti totalmente
dall'applicazione della banca.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta una risposta positiva
dall'applicazione di pagamento on line.

**ATTENZIONE!** **T.P@Y.SM supporta la modalità Server to Server**. In
tale modalità l'applicazione di back office della banca invierà una
notifica al sito per gestire l'esito della transazione anche nel caso in
cui l'acquirente non dovesse fare ritorno sul sito dell'esercente (ad
esempio perché a transazione conclusa chiude semplicemente il browser).

In ogni caso nel momento in cui dovessero essere effettuati ordini a
seguito dei quali l'applicazione di Back Office non ha restituito alcuna
risposta (ad esempio perché è stato chiuso il browser prima di
completare il pagamento) , come nel caso di annullamento della procedura
di pagamento, tali ordini resteranno unicamente all'interno del database
di Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

