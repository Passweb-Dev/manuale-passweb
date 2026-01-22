# GESTIONE ORDINI



All'interno della sezione **"Catalogo -- Amazon - Ordini"** è possibile
visualizzare e gestire tutti gli ordini acquisiti direttamente dal
Marketplace a seguito di sincronizzazioni manuali e/o automatiche

![](./assets/media/image296.png)

I pulsanti presenti nella barra degli strumenti della maschera "**Lista
Ordini**" consentono rispettivamente di:

**Sincro Ordini** (
![](./assets/media/image45.png) ): consente, di effettuare la
sincronizzazione tra le due piattaforme importando quini in Passweb
eventuali nuovi ordini, e relativi clienti, acquisiti direttamente sul
marketplace Amazon.

**ATTENZIONE!** la sincronizzazione tra Passweb a Amazon, con la
conseguente eventuale importazione di nuovi ordini, **avverrà anche, in
maniera completamente automatica, a seguito di ogni "Sincronizzazione
Totale"** (manuale o schedulata) tra il Sito ed il gestionale
Passepartout

Per maggiori informazioni in merito si veda anche il capitolo "*Acquisto
articoli su Amazon e sincronizzazione Ordini sul gestionale*" di questo
manuale.

**Parametri Ordine** (
![](./assets/media/image168.png) ): consente di impostare una o più
causali, opportunamente definite all' interno del gestionale, ed
utilizzate per marcare come "**Annullati**" gli ordini provenienti dal
Marketplace.

**ATTENZIONE! le causali impostate all'interno di questa sezione sono
valide a livello generale per tutti gli ordini presenti in elenco.**

E' possibile annullare un ordine indicando diverse motivazioni,
corrispondenti ciascuna ad una delle causali impostate all'interno delle
relative tabelle gestionali **(tutti campi sono obbligatori**)

![](./assets/media/image297.png)

- **Buyer Canceled:** consente di definire la causale di annullamento
  utilizzata all'interno del gestionale per marcare il relativo ordine
  come Annullato in conseguenza del fatto che l'acquirente ha richiesto
  di annullare l'ordine

- **Carrier Coverage Failure:** consente di definire la causale di
  annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza di una mancata copertura
  del Vettore

- **Carrier Credit Decision:** consente di definire la causale di
  annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza di problemi sul
  pagamento

- **Customer Exchange:** consente di definire la causale di annullamento
  utilizzata all'interno del gestionale per marcare il relativo ordine
  come Annullato a seguito di uno scambio di acquirenti

- **Customer Return:** consente di definire la causale di annullamento
  utilizzata all'interno del gestionale per marcare il relativo ordine
  come Annullato in conseguenza di un reso cliente

- **Generale Adjustment:** consente di definire la causale di
  annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza di generici problemi

- **Merchandise notrecived** consente di definire la causale di
  annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza di merce non ricevuta

- **No Inventory** consente di definire la causale di annullamento
  utilizzata all'interno del gestionale per marcare il relativo ordine
  come Annullato in conseguenza della non disponibilità del prodotto da
  spedire

- **Risk Assessment information not vaild:** consente di definire la
  causale di annullamento utilizzata all'interno del gestionale per
  marcare il relativo ordine come Annullato in conseguenza di
  informazioni sulla valutazione dei rischi non valide

- **Shipping Adress Undeliverable:** consente di definire la causale di
  annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza di un indirizzo di
  spedizione non corretto

**ATTENZIONE!** Nel caso di **siti Ecommerce collegati a Mexal** è
necessario indicare, nei campi sopra evidenziati, il codice delle
relative Causali. Nel caso invece di **siti Ecommerce collegati ad uno
dei gestionali Ho.Re.Ca**. il nome di queste stesse causali.

Annullando un ordine all'interno del gestionale e utilizzando, allo
stesso tempo, una delle causali sopra indicate, sarà quindi possibile
comunicare automaticamente, in fase di sincronizzazione Sito --
Gestionale, il cambio di stato anche al relativo Marketplace.

**Annulla** (
![](./assets/media/image170.png) ): consente di porre l'ordine attualmente
selezionato in elenco nello stato di "**In Attesa di Annullo**"
indicando anche la motivazione per cui l'ordine in esame è stato
annullato

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Annulla"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà visualizzata la maschera "**Parametri
di Annullamento dell'Ordine**" all'interno della quale poter indicare,
selezionandola dall'apposito menu a tendina (campo **Motivo di
Annullamento**), la motivazione per cui si desidera annullare quello
specifico ordine.

![](./assets/media/image298.png)

**ATTENZIONE!** Una volta impostato un "Motivo di Annullamento" l'ordine
sarà posto, come detto, nello stato di "**In Attesa di Annullo**" ma non
verrà comunicato nulla al relativo marketplace dove l'ordine manterrà,
quindi, il suo stato originario.

In queste condizioni per completare l'annullamento dell'ordine sarà
necessario eseguire manualmente la procedura di "Aggiornamento Ordini"
sul Marketplace (pulsante **Aggiorna Ordini**) oppure attendere la
prossima sincronizzazione "Sito -- Gestionale".

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Annullato**" anche all'interno del proprio sito Passweb. Lato
gestionale l'ordine manterrà invece il suo stato originale (essendo
l'annullamento partito dal sito Passweb) e sarà quindi necessaria una
sincronizzazione per allineare lo stato del documento anche sul
gestionale.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Annullo**" e provvederà ad effettuare il cambio di stato sia verso il
marketplace che verso il gestionale in maniera del tutto automatica.

In entrambi i casi dunque al termine della sincronizzazione l'ordine
sarà in stato "**Annullato**" sul gestionale, sul sito Passweb e sul
relativo Marketplace.

**ATTENZIONE!** Per maggiori informazioni sulle procedure di
annullamento di un ordine Amazon si veda anche il successivo capitolo di
questo manuale (*Stati Ordine Amazon*)

**Spedizione** (
![](./assets/media/image172.png) ): consente di porre l'ordine attualmente selezionato
in elenco nello stato di "**In Attesa di Spedizione**"

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Spedizione"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Parametri della Spedizione**"

![](./assets/media/image299.png)

all'interno della quale poter impostare:

- **Vettore:** consente di impostare, selezionandolo dal relativo menu a
  tendina, il Vettore Amazon utilizzato per effettuare la spedizione
  relativamente all'ordine in questione.

> **ATTENZIONE!** All'interno del campo "Vettore" verranno visualizzati
> solo ed esclusivamente quei metodi di trasporto configurati come
> Vettori Amazon e per i quali è stato quindi valorizzato, in fase di
> configurazione, il relativo campo "**Vettore Amazon**"

![](./assets/media/image300.png)

> Per maggiori informazioni in merito si veda anche la sezione "*Ordini
> -- Configurazione Metodi di trasporto*" di questo manuale.

- **Data di Inizio Trasporto:** consente di impostare la data di inizio
  trasporto relativamente all'ordine in questione.

- **Number Tracking:** consente di impostare il Number Tracking
  assegnato dallo spedizioniere alla spedizione che si sta effettuando.

**ATTENZIONE!** Nel caso in cui **il processo di spedizione parta dal
gestionale** mediante la valorizzazione dei relativi campi, tutti e tre
i parametri presenti all'interno di questa maschera saranno in sola
visualizzazione.

Una volta impostati questi parametri cliccando sul pulsante "Salva"
l'ordine passerà in stato di "**In Attesa di Spedizione**" ma non verrà
comunicato nulla al relativo marketplace dove l'ordine manterrà, quindi,
il suo stato originario.

In queste condizioni per completare il processo di spedizione
dell'ordine sarà necessario eseguire manualmente la procedura di
"Aggiornamento Ordini" sul Marketplace (pulsante **Aggiorna Ordini**)
oppure attendere la prossima sincronizzazione "Sito -- Gestionale".

**ATTENZIONE!** Per effettuare il cambio di stato da "In Attesa di
Spedizione" a "Spedito" è necessario che tutti e tre i campi "Vettore",
"Data Inizio Trasporto" e "Number Tracking" siano stati correttamente
valorizzati. **Nel caso in cui anche uno soltanto di questi non dovesse
essere valorizzato l'ordine rimarrà sempre nello stato di "In Attesa di
Spedizione"**

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Spedito**" anche all'interno del proprio sito Passweb. Lato
gestionale non verrà apportata ancora nessuna modifica all'ordine e sarà
quindi necessaria una sincronizzazione per allineare lo stato del
documento anche sul gestionale.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Spedizione**", provvederà ad effettuare il cambio di stato (che passerà
quindi a "**Spedito**") anche verso il marketplace e inserirà lato
gestionale il vettore la data di inizio trasporto e, dove possibile,
anche il Number Tracking impostati all'interno del sito.

Nello specifico **Vettore, Data di Inizio Trasporto** e **Number
Tracking** verranno inseriti nei relativi campi presenti nel piede del
documento

![](./assets/media/image301.png)

![](./assets/media/image302.png)

Per i siti Ecommerce collegati a Mexal, nel momento in cui il Number
Tracking dovesse essere gestito con un Attributo Ordine, il codice di
spedizione verrà ovviamente inserito all'interno dell'apposito campo
della videata riportabile utente utilizzata per gestire l'attributo in
esame.

Per maggiori informazioni relativamente alla gestione del Number
Tracking si veda anche quanto indicato alla sezione *"Ordini --
Configurazione Ordini -- Impostazioni generali"* di questo manuale

In tutti i casi, comunque, al termine della sincronizzazione l'ordine
sarà in stato "**Spedito**" sul marketplace a all'interno del proprio
sito Passweb mentre all'interno del gestionale saranno stati valorizzati
i campi del Vettore, della Data di Inizio Trasporto e del Number
Tracking.

**ATTENZIONE!** Affinchè i valori inseriti da Passweb siano
correttamente visibili nel piede dei documenti Mexal, è necessario che
il parametro di magazzino "**Memorizza data e ora inizio trasporto**"
sia stato correttamente selezionato

![](./assets/media/image177.png)

Nel caso in cui il parametro in oggetto non fosse stato selezionato,
Data e ora di inizio trasporto impostate da Passweb potranno essere
visibili all'interno di bolle e/o fatture ma non all'interno di ordini.

Per maggiori informazioni sulle procedure di spedizione di un ordine
Amazon si veda anche il successivo capitolo di questo manuale (*Stati
Ordine Amazon*)

**Rimborso** (
![](./assets/media/image303.png) ): consente di porre l'ordine
attualmente selezionato in elenco nello stato di "**In Attesa di
Rimborso**"

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Rimborso"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà visualizzata la maschera "**Parametri
di Rimborso Ordine**"

![](./assets/media/image304.png)

all'interno della quale l'utente avrà la possibilità di selezionare, tra
quelli proposti in elenco, lo specifico motivo a seguito del quale viene
effettuato il rimborso dell'ordine (le motivazioni selezionabili sono
fornite direttamente da Amazon e non possono essere modificate in alcun
modo)

Una volta selezionata la specifica motivazione, cliccando sul pulsante
"Salva" l'ordine passerà, come detto, in stato di "**In Attesa di
Rimborso**"; per completare il processo di rimborso dell'ordine sarà
necessario quindi eseguire manualmente la procedura di "Aggiornamento
Ordini" sul Marketplace (pulsante **Aggiorna Ordini**) oppure attendere
la prossima sincronizzazione "Sito -- Gestionale".

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Rimborsato**" anche all'interno del proprio sito Passweb.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Rimborso**" e provvederà ad effettuare il cambio di stato (che passerà
quindi a "**Rimborsato**") anche verso il marketplace.

**ATTENZIONE**! **Gli stati "In Attesa di Rimborso" e "Rimborsato" non
hanno un corrispettivo gestionale per cui possono essere gestiti solo
all'interno di questa sezione del Wizard di Passweb oltre a poter essere
comunicati anche al relativo Marketplace Amazon.**

**Aggiorna Ordini** (
![](./assets/media/image180.png) ): consente di eseguire, in maniera
manuale, la procedura di aggiornamento dello stato ordini dal proprio
sito Passweb verso i relativi Marketplace Amazon.

**ATTENZIONE!** La procedura "Aggiorna Ordini" eseguita da questa
sezione del Wizard funziona esclusivamente dal sito Passweb verso i
Marketplace e non ha alcuna influenza sul gestionale.

Per maggiori informazioni relativamente ai vari cambi di stato e a come
poter comunicare tali informazioni ai relativi marketplace si veda anche
il successivo capitolo ("*Stati Ordine Amazon*") di questo manuale.

