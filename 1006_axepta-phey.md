# AXEPTA PHEY



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche appoggiate al gateway di pagamento **Axepta pHey**
(gruppo **BNP PARIBAS**).

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_axepta.bmp](./assets/media/image43.png)

Nello specifico all'interno di questa sezione il campo:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Access Token:** consente di indicare il token di accesso necessario
  per l'integrazione con il gateway di pagamento

- **License Key Server / License Key Easy Checkout:** consente di
  indicare le due chiavi di configurazione necessarie per poter
  integrare correttamente il proprio sito con il gateway di pagamento

**NOTA BENE**: le informazioni da inserire nei campi Access Token,
License Key Server, License Key Easy Checkout **sono obbligatorie** e
non sono reperibili sul gestionale ma vengono fornite direttamente
all'esercente, al momento della sua adesione al servizio offerto. In
alternativa tali dati potrebbero essere reperiti all'interno
dell'apposito back office fornito dalla banca.

Una eventuale discordanza tra i dati inseriti in questi campi e quelli
forniti all'esercente, renderà impossibile agli utenti del sito
utilizzare questa modalità di pagamento

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

- **Gestisci Wallet Utente:** se selezionato, consente di valorizzare
  nella chiamata al gateway di Axepta il parametro "payInstrToken" con
  l'identificativo dell'utente Passweb in modo che vengano poi
  visualizzate le carte utente già salvate e si possa effettuare il
  "pagamento in un click".

Una volta impostati correttamente i parametri presenti all'interno delle
due sezioni appena analizzate, se l'utente dovesse, alla conferma
dell'ordine, selezionare la modalità di pagamento in esame, l'ordine
sarà memorizzato nel database di Passweb, e l'utente verrà reindirizzato
sul sito del gateway di pagamento dove dovrà inserire i relativi dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_axepta_2.bmp](./assets/media/image44.png)

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto oppure di
portare a termine l'acquisto e completare la transazione.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine già confermato
e non avrà modo di modificarlo. Come detto, infatti l'ordine viene
memorizzato nel database di Passweb prima che l'utente venga ricondotto
al sito della banca.

In queste condizioni però l'utente non ha ancora effettuato il pagamento
per cui l'ordine, memorizzato nel database di Passweb, assumerà lo stato
di "Pagamento Non Confermato" e, conseguentemente, alla sincronizzazione
non verrà inserito in maniera automatica all'interno del gestionale.

**In queste stesse condizioni, nel caso in cui l'utente volesse
effettuare comunque l'ordine utilizzando però una diversa modalità di
pagamento, dovrà ripartire da zero inserendo gli articoli in carrello ed
effettuando nuovamente la procedura di checkout.**

Nel secondo caso, una volta confermata la transazione verrà presentata
all'utente una pagina web con l'esito del pagamento appena effettuato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_axepta_3.bmp](./assets/media/image45.png)

e, dopo pochi secondi, sarà automaticamente ricondotto al sito
Ecommerce, l'ordine verrà considerato valido ed inserito quindi
all'interno del gestionale

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **Axepta pHey supporta la modalità Server to Server**
(non sono necessarie ulteriori configurazioni nell'applicazione di
backoffice della banca). In tale modalità l'applicazione di back office
della banca invierà una notifica al sito per gestire l'esito della
transazione anche nel caso in cui l'acquirente non dovesse fare ritorno
sul sito dell'esercente (ad esempio perché a transazione conclusa chiude
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
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di utilizzare la specifica
manualistica.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà del Gateway di paramento occorre rivolgersi alla relativa
assistenza.

