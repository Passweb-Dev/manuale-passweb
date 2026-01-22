# KLARNA



**ATTENZIONE! Per poter attivare il pagamento rateale mediante
piattaforma Klarna è necessario acquistare il relativo modulo**

La modalità di pagamento etichettata a default come **Klarna** offre
agli utenti del sito la possibilità di effettuare acquisti suddividendo
il pagamento in 3 comode rate pagabili, senza interessi, direttamente
con la propria carta di credito.

**ATTENZIONE! Il finanziamento viene richiesto e gestito direttamente
sulla piattaforma Klarna ( <https://www.klarna.com/it/> ).**

![](./assets/media/image110.png)

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
verrà quindi ricondotto su questa piattaforma dove dovrà fornire tutta
la documentazione e i dati richiesti per l'approvazione del
finanziamento e per poter quindi concludere correttamente il proprio
ordine.

Per attivare questa particolare modalità di pagamento in Passweb sarà
necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione **Klarna**

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

![](./assets/media/image111.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Username / Password**: credenziali di accesso alle API della
  piattaforma di pagamento. Indispensabili per poter realizzare
  correttamente l'integrazione tra la piattaforma di pagamento ed il
  proprio sito Ecommerce.

> Per maggiori informazioni relativamente a dove poter reperire queste
> informazioni si veda anche quanto indicato nel successivo capitolo
> ("*Parametri di integrazione*") di questo manuale

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate mediante il sistema di pagamento in esame
  dovrà avvenire con **"Addebito Immediata"** o mediante
  **"Autorizzazione"**.

> L'impostazione del parametro sul valore "Addebito Immediato"
> permetterà all'esercente di rendere automaticamente contabili tutte le
> transazione, senza un suo specifico intervento dall' applicazione di
> Back Office.
>
> L'impostazione del parametro sul valore "Autorizzazione" richiederà
> invece che le operazioni autorizzate siano esplicitamente rese
> contabili dall'esercente attraverso la relativa applicazione di Back
> Office fornita da Klarna.

- **Tema del simulatore:** tema grafico del simulatore di finanziamento
  che verrà visualizzato direttamente nella pagina di checkout del
  proprio sito oppure nelle singole pagine prodotto.

- **ID Simulatore**: consente di specificare l'identificativo del
  simulatore di finanziamento che verrà visualizzato direttamente nella
  pagina di checkout del proprio sito oppure nelle singole pagine
  prodotto.

> **ATTENZIONE!** Nel momento in cui il parametro in questione non
> dovesse essere valorizzato in maniera corretta il simulatore potrebbe
> non essere visualizzato né in fase di checkout né tanto meno nelle
> singole pagine prodotto

- **Metodi di Pagamento**: consente di selezionare tra quelli proposti,
  i metodi di pagamento che dovranno poi essere mostrati all'utente nel
  momento in cui verrà ricondotto sulla pagina di pagamento di Klarna.

**ATTENZIONE!** la richiesta di rateizzazione del pagamento potrebbe
essere accettata solo ed esclusivamente per ordini con importo compreso
tra un determinato valore minimo e massimo. **Tali valori non sono
impostabili da Passweb**. Per maggiori informazioni in merito è
necessario fare riferimento direttamente al contratto sottoscritto con
la piattaforma di pagamento.

Nel caso in cui il totale ordine non dovesse rientrare entro eventuali
limiti imposti dalla piattaforma terza, nel momento in cui l'utente
dovesse comunque scegliere questa particolare modalità di pagamento,
verrà visualizzato, alla conferma, un' apposito messaggio per informarlo
che, in relazione a quello specifico ordine, non è possibile richiedere
una rateizzazione del pagamento

![](./assets/media/image112.png)

**ATTENZIONE! Una volta verificato, direttamente con Klarna, il range
entro cui poter avviare la richiesta di rateizzazione, si consiglia
quindi di impostare i relativi limiti all'interno dei campi "Limite
minimo / massimo" presenti nella maschera di configurazione del
pagamento stesso**

![](./assets/media/image95.png)

In questo modo saremo quindi sicuri che questa specifica modalità di
pagamento verrà proposta al cliente solo ed esclusivamente nel caso in
cui l'importo del suo ordine (o del solo totale merce) sia tale da poter
effettivamente avviare la richiesta di rateizzazione.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", e posto ovviamente di
soddisfare eventuali condizioni di applicabilità impostate per il
pagamento in esame, in fase di checkout comparirà anche l'opzione
relativa a questo stesso pagamento con l'indicazione delle possibili
rate.

![](./assets/media/image113.png)

Nel momento in cui l'utente dovesse decidere di utilizzare questo tipo
di pagamento, alla conferma dell'ordine, il documento sarà memorizzato
nel database di Passweb, e l'utente verrà reindirizzato automaticamente
sulla piattaforma Klarna dove potrà completare la propria richiesta.

L'utente dovrà quindi inserire i dati necessari per creare un proprio
account sulla piattaforma di Klarna, dopo di che gli verranno richiesti
i dati della carta di credito da utilizzare per effettuare i pagamenti
rateizzati e, una volta inseriti anche questi dati gli verranno proposte
le diverse possibili modalità di pagamento.

![](./assets/media/image114.png)

**A questo punto però l'ordine non è ancora concluso in maniera corretta
e, conseguentemente, non è ancora avvenuto alcun pagamento**. L'utente
potrà ancora decidere di annullare tutto oppure di proseguire nella sua
richiesta di finanziamento.

Nel primo caso, annullamento della transazione l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine ancora da
confermare. Volendo potrà dunque decidere di ripartire dalla situazione
attuale, modificando se necessario l'ordine in essere con l'aggiunta o
l'eliminazione di determinati articoli, selezionando altre tipologie di
trasporto e /o altri pagamenti ecc... per poi passare nuovamente a
concludere l'ordine.

Nel secondo caso l'utente dovrà invece seguire tutti i passi e fornire
(direttamente sul sito di Klarna) tutti i dati necessaria per portare a
termine correttamente la propria richiesta di rateizzazione del
pagamento.

Una volta conclusa la procedura per la richiesta di rateizzazione
l'utente verrà automaticamente riportato sul sito Ecommerce dove
l'ordine risulterà ora concluso in maniera corretta.

**NOTA BENE**: verranno inseriti all'interno del gestionale solo ed
esclusivamente gli ordini per i quali è stata ricevuta dalla piattaforma
Klarna, relativamente alla richiesta di finanziamento, una risposta
positiva.

**ATTENZIONE! Klarna supporta la modalità Server to Server**. In tale
modalità l'applicazione di back office del gateway, una volta acquisito
il pagamento, invierà una notifica al sito per gestire l'esito della
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

