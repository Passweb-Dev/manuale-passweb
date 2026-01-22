# FINDOMESTIC



La modalità etichettata a default come **Findomestic** offre agli utenti
del sito la possibilità di concludere i loro acquisti **mediante la
richiesta di un finanziamento online**.

**ATTENZIONE! Per poter utilizzare questa specifica modalità di
pagamento è necessario attivare per prima cosa il relativo modulo su
Passstore**

In questo senso occorre anche sottolineare che all'interno del proprio
sito Passweb sarà possibile gestire, in relazione alla piattaforma di
Findomestic, due diverse tipologie di finanziamento:

- **Finanziamento semplice, con rateizzazione dell'importo da pagare**

- **Finanziamento con utilizzo di incentivi statali e rateizzazione
  dell'importo da pagare**

In ogni caso per attivare una delle due modalità di finanziamento
gestite sarà necessario:

- Stipulare con Findomestic il contratto corretto in relazione alla
  tipologia di servizio che si vuole fornire

- Attivare su Passstore il modulo Findomestic coerente con la tipologia
  di servizio da offrire (su Passstore sono infatti presenti due moduli
  Findomestic, uno per gestire il finanziamento semplice e l'altro per
  gestire il finanziamento con utilizzo di incentivi statali).

**ATTENZIONE! Il finanziamento verrà richiesto e gestito, assieme a
tutta la relativa documentazione, direttamente sulla piattaforma di
Findomestic**

Nel momento in cui si dovesse decidere di attivare questa modalità di
pagamento, Passweb offre anche la possibilità di inserire, direttamente
nella scheda prodotto, il relativo widget per mostrare all'utente una
possibile simulazione di rateizzazione, collegata ovviamente al prezzo
di quello specifico articolo (per maggiori informazioni in merito si
veda anche quanto indicato all'interno del capitolo "*Varianti Sito
Responsive -- Lista Componenti Ecommerce -- Componenti interni ai
componenti Ecommerce -- Componente Simulatore del Pagamento*" di questo
manuale)

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale una
    specifica entry alla quale poter agganciare il pagamento on line in
    oggetto assegnandogli, ad esempio, la descrizione "Findomestic"

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_findomestic.bmp](./assets/media/image94.png)

Nel caso specifico i parametri presenti all'interno di questa sezione
potranno variare in relazione al fatto di aver attivato il modulo di
Findomestic standard oppure quello che prevede la possibilità di
utilizzare anche gli incentivi statali.

Per maggiori informazioni in merito ai parametri da settare nelle due
diverse casistiche si veda quanto indicato nei successivi capitoli di
questo manuale ("*Findomestic Standard*" e "*Findomestic con incentivi
statali*")

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
abilitare la possibilità di attivare un finanziamento solo in
corrispondenza di certi importi, sarà sufficiente agire mediante i campi
"Limite minimo / massimo" presenti nella maschera di configurazione del
pagamento stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\soisy_3.bmp](./assets/media/image95.png)

In questo modo saremo quindi sicuri che questa specifica modalità di
pagamento verrà proposta al cliente solo ed esclusivamente nel caso in
cui l'importo del suo ordine (o del solo totale merce) sia tale da poter
effettivamente avviare la richiesta di finanziamento.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Parametri Gateway", se l'utente dovesse, alla conferma
dell'ordine, selezionare la modalità di pagamento in esame, l'ordine
sarà memorizzato nel database di Passweb, e l'utente verrà reindirizzato
automaticamente sulla piattaforma di Findomestic dove potrà completare
la propria richiesta.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_1.bmp](./assets/media/image96.png)

**A questo punto però l'ordine non è ancora concluso in maniera corretta
e, conseguentemente, non è ancora avvenuto alcun pagamento**. L'utente
potrà ancora decidere di annullare tutto oppure di proseguire nella sua
richiesta di finanziamento.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine già confermato
e non avrà modo di modificarlo. Come detto, infatti l'ordine viene
memorizzato nel database di Passweb prima che l'utente venga ricondotto
sulla piattaforma per la richiesta del finanziamento.

In queste condizioni però l'utente non ha ancora effettuato il pagamento
per cui l'ordine, memorizzato nel database di Passweb, assumerà lo stato
di "Pagamento Non Confermato" e, conseguentemente, alla sincronizzazione
non verrà inserito in maniera automatica all'interno del gestionale.

In queste stesse condizioni, nel caso in cui l'utente volesse effettuare
comunque l'ordine utilizzando però una diversa modalità di pagamento,
dovrà ripartire da zero inserendo gli articoli in carrello ed
effettuando nuovamente la procedura di checkout.

Nel secondo caso l'utente dovrà invece seguire tutti i passi **e fornire
tutta la documentazione necessaria (direttamente sul sito di
Findomestic) per portare a termine correttamente la propria richiesta di
finanziamento.**

Una volta conclusa la procedura per la richiesta del finanziamento
l'utente potrà tornare sul sito Ecommerce dove l'ordine risulterà ora
concluso in maniera corretta.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_2.bmp](./assets/media/image97.png)

**ATTENZIONE!** **Findomestic supporta la modalità Server to Server**.
In tale modalità la piattaforma di finanziamento invierà una notifica al
sito per gestire l'esito della transazione anche nel caso in cui
l'acquirente non dovesse fare ritorno sul sito dell'esercente (ad
esempio perché a transazione conclusa chiude semplicemente il browser).

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali, per qualsiasi ragione, la piattaforma di finanziamento non ha
restituito alcuna risposta tali, ordini resteranno unicamente
all'interno del database di Passweb nello stato di **"Pagamento Non
Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

