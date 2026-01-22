# SCALAPAY



**ATTENZIONE! Per poter attivare il pagamento rateale mediante la
piattaforma di Scalapay è necessario acquistare il relativo modulo**

La modalità di pagamento etichettata a default come **Scalapay** offre
agli utenti del sito la possibilità di effettuare acquisti suddividendo
il pagamento in 3 o 4 comode rate pagabili, senza interessi,
direttamente con la propria carta di credito.

**ATTENZIONE! Il finanziamento viene richiesto e gestito direttamente
sulla piattaforma Scalapay ( <https://www.scalapay.com/it> ).**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_0.bmp](./assets/media/image199.png)

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
    line in oggetto assegnandogli, ad esempio, la descrizione
    **Scalapay**

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_scalapay.bmp](./assets/media/image200.png)

Nel caso specifico il parametro:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Versione Script:** consente di impostare la versione del widget di
  Scalapay utilizzato per gestire il simulatore che verrà poi mostrato
  all'interno del sito (nella pagina prodotto, nella pagina carrello e
  nella pagina di checkout) per consentire all'utente di verificare la
  relativa rateizzazione del pagamento prima di concludere
  effettivamente l'ordine.

> E' possibile selezionare una delle seguenti opzioni:

- **v4:** in queste condizioni verrà utilizzato il vecchio widget di
  Scalapay che mostrerà sempre e comunque un numero di rate predefinito
  (3 o 4) in base a quanto impostato all'interno del successivo
  parametro "**Numero Rate**"

- **v5 -- consigliata --** in queste condizioni verrà visualizzato il
  nuovo widget di Scalapay che offre la possibilità di effettuare una
  simulazione del pagamento sia in 3 che in 4 rate

> **ATTENZIONE!** l'utilizzo di questo script richiede anche
> l'inserimento di un nuovo parametro "Merchant Token" prelevabile
> direttamente dal back-end del proprio account Scalapay
>
> **ATTENZIONE!** quanto impostato in corrispondenza del parametro
> "Versione Script" ha effetto unicamente sulla gestione del simulatore
> di pagamento. L'effettiva possibilità di suddividere il pagamento in 3
> o 4 rate verrà poi effettuata direttamente sul gateway e dipenderà
> dallo specifico prodotto Scalapay attivato in fase di sottoscrizione
> del relativo contratto (e conseguentemente dalla chiave API di
> integrazione utilizzata)

- **Secret API Key:** chiave segreta. Indispensabile per poter
  realizzare correttamente l'integrazione tra la piattaforma di
  pagamento ed il proprio sito Ecommerce.

> **ATTENZIONE!** All'interno di questa chiave, prelevabile direttamente
> dal back end del proprio account Scalapay, sono mappati i prodotti
> attivati in fase di sottoscrizione del relativo contratto ed è da
> questa chiave dunque che dipende l'effettiva possibilità, da parte del
> cliente, di suddividere poi il pagamento in 3 o in 4 rate

- **Merchant Token -- obbligatorio per "Versione Script = v5" --**
  Consente di impostare il Merchant Token necessario per il corretto
  funzionamento del nuovo widget di Scalapay (quello che consente la
  simulazione contemporanea della rateizzazione del pagamento in 3 o 4
  soluzioni)

> **ATTENZIONE**! Per maggiori informazioni relativamente a dove e a
> come poter reperire "Secret Api Key" e "Merchant Token" si veda anche
> quanto indicato nel successivo capitolo ("*Parametri di
> integrazione*") di questo manuale

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
> Office fornita da Scalapay.

- **Frase Checkout:** consente di indicare, selezionandola dall'apposito
  menu a tendina, la frase che dovrà essere visualizzata in checkout in
  corrispondenza del radio button di selezione del pagamento in oggetto

> **ATTENZIONE!** Le frasi selezionabili sono fornite direttamente dal
> widget di Scalapay e non possono essere modificate. Inoltre per i siti
> multilingua attualmente Scalapay fornisce descrizioni solamente in
> Italiano, Francese, .... In conseguenza di ciò nel momento in cui
> dovesse essere in uso una lingua diversa da quelle indicate il testo
> della "Frase Checkout" verrà visualizzato in Italiano

- **Numero Rate -- solo per "Versione Script = v4" --** consente di
  decidere se il vecchio simulatore di Scalapay dovrà mostrare una
  possibilità di rateizzazione in 3 oppure in 4 rate.

> **ATTENZIONE!** l'impostazione settata in corrispondenza di questo
> parametro, e il conseguente funzionamento del simulatore Scalapay,
> dovrà essere coerente con quello che è il prodotto Scalapay attivato
> in fase di sottoscrizione del contratto e quindi con quello che è
> effettivamente il numero di rate che l'utente si troverà poi a dover
> gestire sul relativo gateway per concludere il pagamento
>
> Per maggiori informazioni in merito si consiglia di fare riferimento
> direttamente all'assistenza Scalapay

- **Importo minimo / massimo:** campo in sola lettura visualizzato solo
  dopo aver effettuato un primo salvataggio del pagamento in esame.

> Consente di visualizzare il range di valori entro cui deve ricadere il
> totale dell'ordine affinché il pagamento in questione possa
> effettivamente essere applicato. Tali valori non sono impostabili da
> Passweb.
>
> **ATTENZIONE!** in fase di configurazione di questo pagamento occorre
> quindi considerare **che la richiesta del finanziamento con
> rateizzazione online potrà avvenire solo ed esclusivamente per ordini
> di un certo importo**
>
> In queste condizioni inoltre nel momento in cui l'utente dovesse
> comunque scegliere questa particolare modalità di pagamento, verrà
> visualizzato, alla conferma, un' apposito messaggio d'errore per
> informarlo che, in relazione a quello specifico importo, non è
> possibile richiedere un finanziamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_1.bmp](./assets/media/image201.png)

> **ATTENZIONE! Una volta verificato il range entro gli utenti potranno
> effettuare la richiesta di rateizzazione dell'importo da pagare, si
> consiglia quindi di impostare i relativi limiti all'interno dei campi
> "Limite minimo / massimo" presenti nella maschera di configurazione
> del pagamento stesso**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\soisy_3.bmp](./assets/media/image95.png)

> In questo infatti la modalità di pagamento in questione verrà proposta
> al cliente solo ed esclusivamente nel caso in cui l'importo dell'
> ordine o del solo totale merce (dipendentemente dalle impostazioni
> settate per i parametri di configurazione) sia tale da poter
> effettivamente avviare la richiesta di rateizzazione.

Una volta impostati correttamente i parametri presenti all'interno della
sezione "Configurazione Parametri Gateway", e posto ovviamente di
soddisfare eventuali condizioni di applicabilità impostate per il
pagamento in esame, in fase di checkout comparirà anche l'opzione
relativa a questo stesso pagamento con l'indicazione delle possibili
rate (dipendentemente da quanto impostato per il parametro "Frase
Checkout" precedentemente esaminato)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_2.bmp](./assets/media/image202.png)

**ATTENZIONE!** Se si dovesse decidere di visualizzare, in checkout o in
carrello, eventuali "Dettagli" sul pagamento in oggetto, il testo
visualizzato verrà fornito direttamente da Scalapay e non potrà essere
modificato in alcun modo

Nel momento in cui l'utente dovesse decidere di utilizzare questo tipo
di pagamento, alla conferma dell'ordine, il documento sarà memorizzato
nel database di Passweb, e l'utente verrà reindirizzato automaticamente
sulla piattaforma Scalapay dove potrà completare la propria richiesta.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_3.bmp](./assets/media/image203.png)

L'utente dovrà quindi inserire i dati necessari per creare un proprio
account sulla piattaforma di Scalapay, dopo di che gli verranno
richiesti i dati della carta di credito da utilizzare per effettuare i
pagamenti rateizzati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_4.bmp](./assets/media/image204.png)

**ATTENZIONE!** la possibilità di decidere, in questa fase, se pagare in
3 (opzione "Pay in 3") o in 4 (opzione "Pay in 4") rate dipende dal
prodotto Scalapay attivato in fase di sottoscrizione del relativo
contratto

**A questo punto però l'ordine non è ancora concluso in maniera corretta
e, conseguentemente, non è ancora avvenuto alcun pagamento**. L'utente
potrà ancora decidere di annullare tutto oppure di proseguire nella sua
richiesta di finanziamento.

Nel primo caso, annullamento della transazione (link "Ritorna a Scalapay
online store"), l'utente verrà reindirizzato al sito ecommerce dove si
troverà l'ordine ancora da confermare. Volendo potrà dunque decidere di
ripartire dalla situazione attuale, modificando se necessario l'ordine
in essere con l'aggiunta o l'eliminazione di determinati articoli,
selezionando altre tipologie di trasporto e /o altri pagamenti ecc...
per poi passare nuovamente a concludere l'ordine.

Nel momento in cui l'utente, una volta ritornato al sito, dovesse
comunque decidere di non chiudere l'ordine, questo resterebbe
memorizzato nel database di Passweb in stato di "**Pagamento non
confermato**"

Nel secondo caso l'utente dovrà invece seguire tutti i passi e fornire
(direttamente sul sito di Scalapay) tutti i dati necessaria per portare
a termine correttamente la propria richiesta di rateizzazione del
pagamento.

Una volta conclusa la procedura per la richiesta di rateizzazione
l'utente verrà automaticamente riportato sul sito Ecommerce dove
l'ordine risulterà ora concluso in maniera corretta.

**NOTA BENE**: verranno inseriti all'interno del gestionale solo ed
esclusivamente gli ordini per i quali è stata ricevuta dalla piattaforma
di pagamento, relativamente alla richiesta di finanziamento, una
risposta positiva.

**ATTENZIONE!** **Scalapay supporta la modalità Server to Server**. In
tale modalità l'applicazione di back office del gateway di pagamento
invierà una notifica al sito per gestire l'esito della transazione anche
nel caso in cui l'acquirente non dovesse fare ritorno sul sito
dell'esercente (ad esempio perché a transazione conclusa chiude
semplicemente il browser).

Per attivare correttamente la modalità Server to Server è necessario
però aver configurato correttamente il Webhook all'interno del
backoffice di Scalapay (per maggiori informazioni in merito si veda
anche quanto indicato all'interno del successivo capitolo di questo
manuale ("*Parametri di integrazione*")

Nel caso in cui la modalità Server to Server non sia stata configurata e
attivata in maniera corretta, se l'utente dovesse ad esempio chiudere il
browser prima di essere ridiretto sul sito Ecommerce, Passweb non potrà
sapere se la transazione è stata o meno conclusa correttamente per cui
il relativo ordine resterà unicamente all'interno del database del sito
nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

