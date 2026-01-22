# NUMERA NPGW



La modalità di pagamento etichettata a default come **Numera NPGW**
viene riconosciuta e gestita da tutte le banche che utilizzano il
relativo gateway di pagamento online.

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione **Numera
    NPGW**

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_numera.bmp](./assets/media/image138.png){width="5.545138888888889in"
height="3.2729166666666667in"}

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Codice Negozio:** codice del negozio assegnato all\'esercente;

- **TermId:** codice terminale assegnato all\'esercente;

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del sistema "Numera NPGW"
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

Numera NPGW, fornirà all'esercente un modulo di avviamento al servizio
che dovrà essere compilato come di seguito indicato:

  -----------------------------------------------------------------------------------------
  Indirizzo script1 test (001)        http://urlsito/store/cart/checkout/numerascript/001
  ----------------------------------- -----------------------------------------------------
  Indirizzo script2 test (002)        http://urlsito/store/cart/checkout/numerascript/002

  Indirizzo script3 test (003)        http://urlsito/store/cart/checkout/numerascript/003

  Indirizzo script4 test (004)        

  Indirizzo script di ritorno al      http://urlsito/store/cart/checkout/numerascript/999
  negozio test (999)                  

  Indirizzo script1 produzione (001)  http://urlsito/store/cart/checkout/numerascript/001

  Indirizzo script2 produzione (002)  http://urlsito/store/cart/checkout/numerascript/002

  Indirizzo script3 produzione (003)  http://urlsito/store/cart/checkout/numerascript/003

  Indirizzo script4 produzione (004)  

  Indirizzo script di ritorno al      http://urlsito/store/cart/checkout/numerascript/999
  negozio produzione (999)            
  -----------------------------------------------------------------------------------------

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame,
l'ordine sarà memorizzato nel database di Passweb, e l'utente verrà
reindirizzato alla specifica pagina di accesso del gateway di pagamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\numera_1.bmp](./assets/media/image139.png){width="4.980555555555555in"
height="2.8895833333333334in"}

**A questo punto però l'ordine non è ancora stato preso in carico dalla
banca e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (link
"Annulla") oppure di portare a termine l'acquisto e completare la
transazione.

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

Verranno quindi presentate all'utente una serie di maschere all'interno
delle quali inserire tutti i dati necessari per il pagamento (numero
carta, scadenza ecc...).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\numera_2.bmp](./assets/media/image140.png){width="4.9743055555555555in"
height="2.7534722222222223in"}

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

