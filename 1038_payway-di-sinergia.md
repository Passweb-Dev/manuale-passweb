# PAYWAY DI SINERGIA



La modalità di pagamento etichettata a default come **PayWay di
Sinergia** viene riconosciuta e gestita da tutte le banche che
utilizzano il relativo gateway di pagamento online.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione **Sinergia
    PayWay**

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_sinergia.bmp](./assets/media/image186.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Terminal ID:** codice identificativo del negozio assegnato
  all\'esercente dalla banca;

- **Chiave per firma digitale:** chiave segreta fornita dalla Banca
  all'esercente all'atto della sottoscrizione del servizio.

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
>
> La modalità di autorizzazione immediata prevede che durante la fase di
> pagamento online venga immediatamente inviata la richiesta di
> autorizzazione ai circuiti internazionali. Una volta conclusa la
> transazione in modo positivo l'esercente ha la certezza che quanto
> dovuto dal cliente è stato "prenotato" dal suo plafond.
>
> La modalità di autorizzazione differita prevede che durante la fase di
> pagamento online le transazioni siano prese in carico ma non inoltrate
> ai circuiti.
>
> L'esercente che utilizza questa modalità di accettazione dei pagamenti
> è in grado, in un secondo tempo, di far elaborare le richieste di
> autorizzazione pendenti che lo riguardano.

**NOTA BENE**: Sinergia gestisce solamente importi in euro; per
eventuali ordini in valuta il totale del documento verrà quindi
opportunamente convertito in euro e passato alla banca.

Per maggiori dettagli relativi alla Contabilizzazione o
all'Autorizzazione Immediata o Differita, così come per maggiori
dettagli relativi alla specifica applicazione di BackOffice della banca
si rimanda ai relativi manuali.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del sistema \@POS potrebbe
non essere allineato con la corrente versione di tale software. Si
consiglia quindi di utilizzare la specifica manualistica.

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

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (link
"Annulla e Torna al sito ...") oppure di portare a termine l'acquisto e
completare la transazione.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine già confermato
e non avrà modo di modificarlo. Come detto, infatti l'ordine viene
memorizzato nel database di Passweb prima che l'utente venga ricondotto
al sito della banca.

In queste condizioni però l'utente non ha ancora effettuato il pagamento
per cui l'ordine, memorizzato nel database di Passweb, assumerà lo stato
di "Pagamento Non Confermato" e, conseguentemente, alla sincronizzazione
non verrà inserito in maniera automatica all'interno del gestionale.

In queste stesse condizioni, nel caso in cui l'utente volesse effettuare
comunque l'ordine utilizzando però una diversa modalità di pagamento,
dovrà ripartire da zero inserendo gli articoli in carrello ed
effettuando nuovamente la procedura di checkout.

Nel secondo caso (conferma della transazione) l'ordine verrà preso in
carico e gestito, da questo momento in avanti, dall'applicazione della
banca.

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

Nel caso in cui siano stati effettuati ordini a seguito dei quali
l'applicazione di Back Office non ha restituito alcuna risposta (ad
esempio perché è stato chiuso il browser prima di completare il
pagamento) , come nel caso di annullamento della procedura di pagamento,
tali ordini resteranno unicamente all'interno del database di Passweb
nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

