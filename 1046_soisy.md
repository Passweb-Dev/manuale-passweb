# SOISY



La modalità etichettata a default come **Soisy** offre agli utenti del
sito la possibilità di concludere i loro acquisti **mediante la
richiesta di un finanziamento online**.

**ATTENZIONE! Il finanziamento viene richiesto e gestito sulla
piattaforma Soisy (<https://www.soisy.it/>).**

Nel momento in cui si dovesse decidere di attivare questa modalità di
pagamento, Passweb offre anche la possibilità di inserire, direttamente
nella scheda prodotto, il relativo widget per mostrare all'utente una
possibile simulazione di rateizzazione, collegata ovviamente al prezzo
di quello specifico articolo (per maggiori informazioni in merito si
veda anche quanto indicato all'interno del capitolo "*Varianti Sito
Responsive -- Lista Componenti Ecommerce -- Componenti interni ai
componenti Ecommerce -- Componente Simulatore del Pagamento*" di questo
manuale)

Una volta selezionata questa particolare modalità di pagamento l'utente
verrà quindi portato su questa piattaforma dove dovrà fornire tutta la
documentazione necessaria per l'approvazione del finanziamento e per
poter concludere correttamente il proprio ordine.

Per poter attivare questa particolare modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione **Soisy**

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_soisy.bmp](./assets/media/image214.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Shop ID:** codice identificativo del negozio assegnato
  all\'esercente direttamente da Soisy all'atto della sottoscrizione del
  servizio;

- **API Key:** chiave segreta fornita direttamente da Soisy all'atto
  della sottoscrizione del servizio e indispensabile per poter
  realizzare correttamente l'integrazione tra la piattaforma di
  finanziamento ed il proprio sito Ecommerce.

**Occorre considerare, inoltre, che la richiesta del finanziamento
online potrà avvenire solo ed esclusivamente per ordini di un certo
importo (generalmente compresi tra i 250 e i 15000 euro).**

Nel caso in cui il totale ordine non dovesse rientrare entro questi
limiti, nel momento in cui l'utente dovesse comunque scegliere questa
particolare modalità di pagamento, verrà visualizzato, alla conferma,
un' apposito messaggio d'errore per informarlo che, in relazione a
quello specifico importo, non è possibile richiedere un finanziamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\soisy_2.bmp](./assets/media/image215.png)

**ATTENZIONE! Una volta verificato, direttamente con Soisy, il range
entro cui poter avviare la richiesta di finanziamento, si consiglia
quindi di impostare i relativi limiti all'interno dei campi "Limite
minimo / massimo" presenti nella maschera di configurazione del
pagamento stesso**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\soisy_3.bmp](./assets/media/image95.png)

In questo modo saremo quindi sicuri che questa specifica modalità di
pagamento verrà proposta al cliente solo ed esclusivamente nel caso in
cui l'importo del suo ordine (o del solo totale merce) sia tale da poter
effettivamente avviare la richiesta di finanziamento.

Per maggiori dettagli relativamente alla configurazione e
all'attivazione del servizio oltre che agli importi per i quali poter
effettivamente richiedere dei finanziamenti si rimanda alla specifica
documentazione di prodotto **(<https://www.soisy.it/>).**

In ogni caso le informazioni da inserire in fase di configurazione del
pagamento non sono reperibili sul gestionale ma vengono fornite
all'esercente direttamente da Soisy, al momento della sua adesione al
servizio offerto.

Tali informazioni sono di fondamentale importanza in quanto saranno poi
quelle che consentiranno di realizzare correttamente l'integrazione tra
la piattaforma di finanziamento ed il proprio sito Ecommerce.

**NOTA BENE**: un'eventuale discordanza tra i dati inseriti nei campi di
configurazione e quelli forniti all'esercente, renderà impossibile agli
utenti del sito utilizzare questa modalità di pagamento.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", se l'utente dovesse, alla
conferma dell'ordine, selezionare la modalità di pagamento in esame, e
se l'importo dell'ordine dovesse rientrare effettivamente nei limiti
richiesti per l'avvio della procedura di finanziamento, l'ordine sarà
memorizzato nel database di Passweb, e l'utente verrà reindirizzato
automaticamente sulla piattaforma Soisy dove potrà completare la propria
richiesta.

**A questo punto però l'ordine non è ancora concluso in maniera corretta
e, conseguentemente, non è ancora avvenuto alcun pagamento**. L'utente
potrà ancora decidere di annullare tutto (link "Torna al carrello")
oppure di proseguire nella sua richiesta di finanziamento.

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

Nel secondo caso l'utente dovrà invece seguire tutti i passi e fornire
tutta la documentazione necessaria (direttamente sul sito di Soisy) per
portare a termine correttamente la propria richiesta di finanziamento.

Una volta conclusa la procedura per la richiesta del finanziamento
l'utente verrà automaticamente riportato sul sito Ecommerce dove
l'ordine risulterà ora concluso in maniera corretta.

**NOTA BENE**: verranno inseriti all'interno del gestionale solo ed
esclusivamente gli ordini per i quali è stata ricevuta dalla piattaforma
Soisy, relativamente alla richiesta di finanziamento, una risposta
positiva.

Nel caso in cui siano stati effettuati ordini con richieste di
finanziamento a seguito delle quali la piattaforma Soisy non ha
restituito alcuna risposta (ad esempio perché è stato chiuso il browser
prima di completare la procedura), tali ordini resteranno unicamente
all'interno del database di Passweb nello stato di **"Pagamento Non
Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

