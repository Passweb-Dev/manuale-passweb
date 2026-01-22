# SUMUP



**ATTENZIONE! Per poter gestire i pagamenti mediante il gateway di SumUp
è necessario attivare prima cosa il relativo modulo su Passstore**

SumUp (<https://sumup.it> ) è una piattaforma per la gestione dei
pagamenti online che offre alle piccole imprese e ai professionisti un
nuovo modo di accettare pagamenti con carte di credito utilizzando
dispositivi prodotti da questa stessa società, smartphone o tablet e che
dispone anche di un proprio gateway di pagamento online

E' un sistema sicuro che risponde ai requisiti più severi in fatto di
sicurezza ed è certificato come provider di servizi conforme allo
standard PCI (<https://developer.sumup.com/docs/widgets-card/>)

Non ha canoni mensili o costi fissi ma, come altri servizi simili,
trattiene una percentuale sulle transazioni effettuate mediante il suo
gateway di pagamento. Per maggiori informazioni sui prezze e sui
requisiti di sicurezza offerti da questa piattaforma si consiglia di
fare riferimento alle relative sezioni del portale SumUp

Per poter attivare sul proprio sito Ecommerce i pagamenti mediate il
gateway di SumUp occorre soddisfare due prerequisiti di fondamentale
importanza. Nello specifico è necessario:

- **Disporre di un account SumUp valido e correttamente funzionante**.

> Nel caso in cui non si disponga di questo account sarà possibile
> crearlo a partire dal seguente link <https://me.sumup.com/login>
>
> Sarà poi necessario creare all'interno del portale di sviluppo di
> SumUp un'apposita app (analogamente a quanto avviene ad esempio per le
> integrazioni social) necessaria per garantire l'integrazione tra il
> proprio sito Ecommerce e la piattaforma di pagamento (per maggiori
> informazioni in merito si veda anche il successivo capitolo di questo
> manuale "*SumUp Parametri di Integrazione*")

- **Aver attivato per il proprio sito ecommerce un certificato SSL.**

> Dal punto di vista della sicurezza, come precedentemente evidenziato,
> SumUp è certificato come provider di servizi conforme allo standard
> PCI che è attualmente il più rigoroso in ambito di pagamenti on line.
> Utilizzando il widget messo a disposizione dalla piattaforma per
> completare il pagamento, anche il sito Ecommerce sarà compliance agli
> stessi standard PCI.
>
> Grazie a questo widget infatti non sarà lo shop online a gestire i
> dati sensibili delle carte, dati questi che verranno invece traferiti
> al server sicuro di SumUp senza "passaggi" intermedi. In tutto questo
> per garantire uno standard di sicurezza elevato è chiaro che la
> comunicazione con il server di SumUp debba essere quanto meno criptata
> e che il sito debba quindi disporre di un proprio certificato SSL. Per
> maggiori informazioni si consiglia comunque di consultare la relativa
> sezione sicurezza sul sito di SumUp
> (<https://developer.sumup.com/docs/widgets-card/> )

Una volta soddisfatti i due prerequisiti appena evidenziati sarà poi
necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale una
    specifica entry alla quale poter agganciare il pagamento on line in
    oggetto assegnandogli, ad esempio, la descrizione "SumUp".

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

![](./assets/media/image229.png)

Nello specifico all'interno di questa sezione sarà possibile indicare un
valore per i seguenti parametri:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

> Per maggiori informazioni relativamente a come poter passare, su
> Stripe, dall'ambiente di test a quello di produzione si veda anche
> quanto indicato nel successivo capitolo ("*Stripe Parametri di
> integrazione*") di questo manuale o comunque si faccia riferimento
> alla documentazione della specifica piattaforma

- **Merchant Code:** identificativo merchant del proprio account SumUp.
  Per maggiori informazioni relativamente a dove e come poter reperire
  questa informazione si veda quanto indicato nel successivo capitolo
  ("*Stripe Parametri di integrazione*") di questo manuale

- **Client Id / secret:** all'interno di questi campi andranno impostate
  le chiavi di configurazione necessarie per poter garantire
  l'integrazione tra il proprio sito Ecommerce e il gateway di SumUp.
  Per maggiori informazioni relativamente a dove e a come poter reperire
  queste informazioni si veda anche quanto indicato nel successivo
  capitolo ("*SumUp Parametri di integrazione*") di questo manuale

Una volta impostati correttamente i parametri di configurazione, se
l'utente dovesse, alla conferma dell'ordine, selezionare la modalità di
pagamento in esame, l'ordine sarà memorizzato nel database di Passweb, e
l'utente verrà reindirizzato su di una specifica pagina del sito
Ecommerce in cui troverà il widget fornito da SumUp per poter completare
il pagamento

![](./assets/media/image230.png)

**ATTENZIONE!** La pagina utilizzata per contenere il widget di SumUp e
per completare il pagamento è una pagina cablata che non può essere
modificata graficamente. L'unica personalizzazione possibile è quella
che riguarda il logo dell'azienda. In questo senso il logo visualizzato
all'interno di questa pagina sarà esattamente quello indicato in
corrispondenza del campo "**Logo Area Riservata e Sito in Lavorazione**"
presente alla pagina "**Preferenze Sito**" del Wizard

**A questo punto l'ordine non è ancora stato preso in carico da SumUp e,
conseguentemente, non è ancora avvenuto alcun pagamento**. L'utente
potrà ancora decidere, quindi, di annullare tutto (pulsante "**Back to
Checkout**") oppure di portare a termine l'acquisto e completare la
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

Nel secondo caso (conferma della transazione) dopo aver inserito i dati
richiesti, sarà sufficiente cliccare sul pulsante "**Paga**" per potare
a termine l'rodine.

![](./assets/media/image231.png)

Una volta elaborato il pagamento e completata la transazione l'utente
sarà ricondotto automaticamente al sito Ecommerce e l'ordine, se
possibile, verrà immediatamente inserito all'interno del gestionale.

**NOTA BENE**: le mail di notifica di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **SumUp supporta la modalità Server to Server in maniera
nativa**. L'attivazione di questa modalità non richiede quindi alcun
tipo di configurazione lato back end

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali, per qualsiasi motivo, il gateway di pagamento non ha
restituito alcuna risposta, tali ordini resteranno unicamente
all'interno del database di Passweb nello stato di **"Pagamento Non
Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà del Gateway di paramento occorre rivolgersi alla relativa
assistenza.

