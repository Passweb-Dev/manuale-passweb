# INFORMAZIONI GENERALI



All'interno della sezione "**Informazioni Generali**" presente nella
maschera di configurazione di ogni pagamento sarà possibile indicare un
valore per i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamento_mexal_configurazione.bmp](./assets/media/image8.png)

**Tipo di Pagamento:** consente di definire la tipologia del pagamento
attualmente selezionato. E' possibile scegliere tra il valore "Pagamento
di Mexal / Ho.Re.Ca.", da utilizzare per pagamenti quali "Contrassegno"
"Bonifico" ecc... completamente gestiti e configurati all'interno del
gestionale, e una delle diverse possibili modalità di pagamento mediante
carta di credito.

**NOTA BENE:** selezionando come tipologia del pagamento una delle
diverse possibili modalità mediante carta di credito, verranno
successivamente richiesti altri parametri, strettamente legati alla
specifica tipologia considerata, e necessari per completare la
configurazione del pagamento on line.

**Stato del Pagamento:** permette di Abilitare/Disabilitare lo specifico
pagamento, facendolo quindi comparire o meno tra quelli che il cliente
potrà poi selezionare all'interno del sito web (allo stesso modo di
quanto avviene con i pulsanti "Abilita Pagamento" e "Disabilita
Pagamento" precedentemente esaminati)

**Ordinamento:** consente di assegnare al pagamento in esame uno
specifico numero che verrà poi utilizzato per ordinare l'elenco dei
pagamenti disponibili, elenco questo visualizzato, sul front end del
sito, in fase di checkout piuttosto che all'interno del relativo modulo
per il preventivo sui pagamenti presente in carrello.

**ATTENZIONE!** i pagamenti attivi per i quali non è stato specificato
un numero d'ordine verranno visualizzati per primi

Inoltre:

- a parità di ordinamento i pagamenti attivi presenti in elenco verranno
  ordinati per descrizione

- nel caso in cui sia gestito il "pagamento abituale", questo verrà
  visualizzato sempre e comunque come primo elemento in elenco
  (indipendentemente dal fatto di avergli assegnato o meno uno specifico
  numero d'ordine)

**Descrizione:** etichetta identificativa della modalità di pagamento
selezionata. A default verrà proposta la stessa descrizione utilizzata,
per lo specifico pagamento, all'interno del gestionale.

**Dettaglio:** consente di inserire ulteriori informazioni relativamente
al pagamento attualmente selezionato.

Grazie a questo campo è quindi possibile, ad esempio, per pagamenti
mediante Bonifico indicare le coordinate bancarie da utilizzare per
effettuare il versamento.

Il pulsante "**Aggiungi un segnaposto**" presente immediatamente al di
sotto del campo in questione consente di utilizzare anche il seguente
segnaposto:

- **Codice Contratto Nexi**: consente di inserire all'interno del
  dettaglio un segnaposto che verrà poi sostituito in maniera dinamica
  con il valore del codice contratto creato su Nexi a seguito di un
  pagamento ricorrente (per maggiori informazioni sui pagamenti
  ricorrenti si veda quanto indicato nel successivo capitolo "*Nexi Xpay
  Pro -- Pagamenti ricorrenti"* di questo manuale).

**Visualizza dettaglio:** consente di decidere se, e dove visualizzare
le informazioni aggiuntive sul pagamento. E' possibile selezionare uno
dei seguenti valori:

- **Non visualizzare:** in queste condizioni non verrà, ovviamente,
  visualizzata nessuna informazione aggiuntiva sul pagamento,
  indipendentemente da quanto inserito all'interno del campo "Dettaglio"

- **In fase di Checkout:** in queste condizioni una volta inserite,
  all'interno del campo "Dettaglio", le informazioni aggiuntive sul
  pagamento, verrà visualizzato sul sito, in fase di checkout e accanto
  alla descrizione del pagamento in esame, un pulsante "**Dettagli**"
  mediante il quale l'utente potrà visualizzare le informazioni
  aggiuntive precedentemente inserite.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamento_configurazione_dettagli.bmp](./assets/media/image9.png)

- **Nel Dettaglio dell'Ordine:** in queste condizioni le informazioni
  aggiuntive sul dettaglio del pagamento verranno visualizzate nel
  dettaglio dell'Ordine che l'utente si appresta a confermare. Inoltre
  queste stesse informazioni verranno inserite anche in tutte le mail
  inviate dall'applicativo all'interno delle quali compare il dettaglio
  dell'ordine effettuato dal cliente.

- **In fase di Checkout e nel Dettaglio dell'Ordine:** in queste
  condizioni le informazioni aggiuntive sul pagamento verranno
  visualizzate in fase di checkout (mediante l'apposito pulsante
  "Dettagli"), nel riepilogo dell'ordine che l'utente si appresta a
  confermare e anche in tutte le mail inviate dall'applicativo e che
  contengono il dettaglio dell'ordine effettuato dal cliente.

- **Nel carrello:** in queste condizioni le informazioni aggiuntive sul
  pagamento verranno visualizzate, in Carrello, all'interno
  dell'apposito modulo per la "Stima dei Costi di Pagamento"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettagli_pagamento_carrello.bmp](./assets/media/image10.png)

- **Nel Carrello ed in fase di Checkout:** in queste condizioni le
  informazioni aggiuntive sul pagamento verranno visualizzate, in
  Carrello, all'interno dell'apposito modulo per la "Stima dei Costi di
  Pagamento", e in fase di conferma ordine nella corrispondente sezione
  di selezione del pagamento

- **Nel Carrello e nel Dettaglio dell'Ordine:** in queste condizioni le
  informazioni aggiuntive sul pagamento verranno visualizzate, in
  Carrello, all'interno dell'apposito modulo per la "Stima dei Costi di
  Pagamento" e nel dettaglio dell'Ordine che l'utente si appresta a
  confermare

- **Sempre:** in queste condizioni le informazioni aggiuntive sul
  pagamento verranno sempre visualizzate sia che ci si trovi all'interno
  della pagina Carrello (posto ovviamente di aver impostato la
  visualizzazione del modulo per la "Stima dei costi di Pagamento"),
  così come in fase di Conferma o di Dettaglio Ordine.

**Indicazione Abilitazione:** consente di impostare, in ciascuna delle
lingue attualmente gestite all'interno del sito, un testo personalizzato
mediante il quale poter indicare all'utente come comportarsi per
abilitare il pagamento in esame nel caso in cui questo non dovesse
essere selezionabile.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\msg_pagamenti_non_selezionabili.bmp](./assets/media/image11.png)

Il testo indicato all'interno di questo campo verrà poi inserito:

- Nella sezione del Checkout relativa ai Pagamenti

- Nel pop up visualizzato, sempre in Checkout, nel caso in cui sia stato
  selezionato il parametro "Mostra popup se non ci sono Pagamenti\"
  presente nella maschera di configurazione del componente Checkout

- In Carrello in fase di preventivo sui pagamenti

e soprattutto **verrà effettivamente visualizzato solo nel caso in cui
risulti valida almeno una delle seguenti condizioni**:

- non ci sono pagamenti selezionabili

- non è possibile procedere con l\'ordine senza selezionare una
  pagamento (parametro "Procedi se non ci sono pagamenti" nella maschera
  di configurazione del componente Checkout deselezionato)

- risultano essere presenti pagamenti che non vengono però mostrati a
  causa di uno o più dei seguenti parametri:

  - Filtro articoli: alcuni articoli in ordine non soddisfano il filtro
    impostato sul relativo pagamento (se nessuno degli articoli in
    ordine dovesse soddisfare il filtro, il pagamento non verrebbe
    considerato)

  - Limite minimo: il totale merce in ordine non raggiunge il limite
    minimo impostato sul relativo pagamento

  - Limite massimo: il totale merce in ordine supera limite massimo
    impostato sul relativo pagamento

Va de sé quindi che un messaggio di questo tipo dovrebbe essere
impostato solo nel caso in cui per il pagamento in esame si dovesse
effettivamente decidere di impostare uno dei limiti sopra indicati.

Il pulsante "**Aggiungi un segnaposto**" presente immediatamente al di
sotto del campo in questione consente di comporre il messaggio
utilizzando anche uno dei segnaposto presenti in elenco, segnaposto
questi che consentono di gestire:

- **Limite Minimo / Massimo**: consente di inserire all'interno del
  messaggio un segnaposto che verrà poi sostituito in maniera dinamica
  con il valore del Limite Minimo / Massimo eventualmente impostato per
  il pagamento in esame

- **Articoli Esclusi**: consente di inserire all'interno del messaggio
  un segnaposto che verrà poi sostituito in maniera dinamica con l'
  elenco degli articoli presenti in ordine che non soddisfano
  l'eventuale Filtro Articolo impostato sul pagamento in esame

- **Se Limite Minimo / Massimo**: consente di inserire all'interno del
  messaggio un' istruzione condizionale per visualizzare quanto inserito
  al suo interno solo nel caso in cui il totale merce in ordine non
  dovesse soddisfare il Limite Minimo / Massimo eventualmente impostata
  sul pagamento in esame

- **Se Articoli Esclusi**: consente di inserire all'interno del
  messaggio un' istruzione condizionale per visualizzare l' elenco di
  articoli presenti in ordine che non soddisfano l'eventuale Filtro
  Articolo impostato sul pagamento in esame

Grazie a questi segnaposto sarà quindi possibile impostare messaggi del
tipo

- *\$if(min_limit)\$Puoi usufruire del pagamento in Contrassegno se
  raggiungi un minimo di \$min_limit\$.\$endif\$*

> che verrà visualizzato solo nel caso in cui il totale merce in ordine
> non dovesse superare il limite minimo impostato e indicherà all'utente
> anche l'effettivo valore che il totale merce dovrà raggiungere per
> abilitare il metodo di pagamento in questione.

- *\$if(excluded_items)\$Puoi usufruire del pagamento in Contrassegno se
  rimuovi dal carrello i seguenti articoli:\<br
  /\>\$excluded_items\$\$endif\$*

> che verrà visualizzato solo nel caso in cui ci siano articoli in
> carrello che non soddisfano il filtro (esclusivo) eventualmente
> impostato sul pagamento in questione

- ...

**ATTENZIONE!** Nel caso in cui per il pagamento in esame dovesse essere
impostato contemporaneamente un limite minimo, un limite massimo e anche
un filtro articoli verrà visualizzato prima di tutto l'eventuale
messaggio relativo al filtro articoli, poi quello relativo al limite
minimo e, infine, quello relativo al limite massimo (posto ovviamente di
aver composto il messaggio utilizzando tutte le apposite istruzioni
condizionali)

**Filtro Articoli:** consente di impostare uno specifico filtro mediante
il quale poter condizionare la visibilità del pagamento in esame alla
presenza in carrello di determinati articoli.

In questo senso poi occorre sottolineare che, **relativamente agli
articoli di tipo Campionario**, la validazione del filtro impostato
verrà fatta prendendo in considerazione l'articolo Campionario in sé
piuttosto che i singoli Componenti dipendentemente da come è stato
impostato il parametro "**Gestione Articoli Box**" alla pagina
"**Configurazione Catalogo**" del Wizard.

In particolare nel caso in cui il parametro in questione dovesse essere
impostato sul valore:

- **Considera il Box** -- **opzione di default**: verrà preso in
  considerazione soltanto l'articolo Campionario.

> In questo caso dunque, la visibilità del pagamento sarà condizionata
> alla presenza in carrello dell'articolo Campionario in sé,
> indipendentemente da quelli che potranno essere i suoi componenti

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, per valutare la visibilità o meno del pagamento
> verranno presi in considerazione i componenti del Campionario ma non
> l'articolo Campionario in sé che, quindi, potrebbe anche non
> soddisfare il filtro impostato.

**ATTENZIONE! Il filtro definito mediante il campo in esame non è un
filtro esclusivo** per cui il relativo metodo di pagamento verrà
visualizzato sul front end del sito **anche se uno solo degli articoli
presenti in carrello** dovesse effettivamente soddisfare il filtro
impostato

Nel momento in cui l'esigenza dovesse essere invece quella di
visualizzare il pagamento solo se tutti gli articoli effettivamente
presenti in carrello dovessero soddisfare il filtro impostato, non sarà
più sufficiente definire il solo "Filtro articoli" ma occorrerà
impostare anche un ben preciso "**Filtro carrello**"

**Filtro carrello:** consente di impostare un filtro mediante il quale
poter condizionare la visibilità del pagamento in esame alla quantità /
numero di articoli presenti in ordine, a livello globale o di singola
riga e/o sulla base del fatto che gli articoli in carrello abbiano o
meno uno sconto già applicato. Di base quindi lavorando sul "Filtro
carrello" sarà possibile:

- decidere se il pagamento dovrà essere visualizzato solo nel momento in
  cui tutte le righe articolo presenti in carrello dovessero soddisfare
  un eventuale "Filtro Articoli" o anche se solo una certa percentuale
  di esse dovesse essere effettivamente sufficiente per fare scattare la
  promozione.

- decidere se la condizione di visibilità del pagamento dovrà essere
  validata considerando tutti gli articoli presenti in carrello che
  soddisfano un eventuale "Filtro Articoli", oppure solo quelli che,
  oltre a soddisfare un eventuale "Filtro Articoli", risultino anche
  privi di eventuali altri sconti già applicati.

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_filtro_quantità.bmp](./assets/media/image12.png)

- **Quantità in carrello:** permette di definire una condizione di
  visibilità del pagamento basata sulla **quantità complessiva di
  articoli presenti in carrello**.

> Supponendo dunque di impostare un filtro del tipo "**Quantità in
> carrello maggiore di 5**" il pagamento in esame verrà visualizzato
> solo ed esclusivamente nel caso in cui la quantità complessiva di
> articoli in carrello dovesse essere effettivamente maggiore di 5. Tale
> condizione potrebbe quindi essere soddisfatta inserendo in carrello un
> solo articolo in quantità 6 o, ad esempio, due distinti articoli
> ciascuno in quantità 3.

- **Elementi in carrello:** permette di definire una condizione di
  visibilità del pagamento basta sul **numero complessivo di articoli
  presenti in carrello** (e quindi effettivamente in ordine).

> Supponendo quindi di impostare un filtro del tipo "**Elementi in
> Carrello maggiore di 2**" il pagamento in esame verrà visualizzato
> solo ed esclusivamente nel caso in cui siano stati inseriti in
> carrello almeno 3 distinti articoli indipendentemente dalla quantità
> acquistata per ognuno di essi.
>
> **ATTENZIONE!** **Nel caso in cui, per il pagamento in esame, dovesse
> essere impostato anche un Filtro Articoli, nella valutazione della
> condizione sul numero di articoli presenti in carrello verranno
> considerati solo ed esclusivamente gli articoli che soddisfano il
> filtro impostato.**
>
> Di base dunque se dovessimo trovarci in una situazione mista in cui
> sono presenti in carrello sia prodotti che soddisfano un eventuale
> Filtro Articoli sia prodotti che non lo soddisfano, nel momento in cui
> quelli che lo soddisfano dovessero soddisfare anche eventuali
> condizioni impostate sul numero di elementi, allora la promozione
> verrebbe correttamente applicata.
>
> Diversamente se l'esigenza dovesse essere quella di non applicare la
> promozione in una situazione mista, in cui ci ritroviamo in carrello
> prodotti che soddisfano il Filtro Articoli ma anche prodotti che non
> lo soddisfano, sarà necessario utilizzare allora per il Filtro
> carrello l'opzione "Percentuale Elementi in Carrello"

- **Elementi distinti in Carrello**: stesso funzionamento della
  condizione "Elementi in carrello" con la particolarità però di
  considerare eventuali righe che fanno riferimento allo stesso articolo
  come un unico elemento in carrello.

> Supponendo dunque di impostare un filtro del tipo "Elementi distinti
> in carrello maggiore di 2" il pagamento in esame verrà visualizzato
> solo nel caso in cui dovessero essere presenti in carrello almeno 3
> righe di articoli questa volta **tutti diversi tra loro.**

- **Percentuale Elementi in Carrello**: permette di indicare la
  percentuale di articoli presenti in carrello che dovranno soddisfare
  un eventuale condizione di Filtro Articoli affinché il pagamento in
  esame possa effettivamente essere visualizzato.

> Nel momento in cui l'esigenza dovesse essere dunque quella di non
> visualizzare il pagamento sul front end del sito in una situazione
> mista, mostrandolo invece solo ed esclusivamente nel caso in cui tutti
> gli articoli presenti in carrello dovessero soddisfare un'eventuale
> condizioni di Filtro Articoli, sarà allora necessario impostare un
> Filtro Quantità del tipo "**Percentuale elementi in carrello = 100**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_percentuale_articoli.bmp](./assets/media/image13.png)

> In queste condizioni se dovessimo avere in carrello anche un solo
> articolo che non soddisfa la condizione impostata all'interno del
> campo "Filtro Articoli" il pagamento, indipendentemente da tutto il
> resto, non verrà visualizzato.
>
> Allo stesso modo se l'esigenza dovesse essere quella di visualizzare
> il pagamento quando almeno il 50% delle righe articolo presenti in
> carrello dovessero soddisfare la condizione di Filtro Articoli, sarà
> allora necessario impostare un "Filtro carrello" del tipo
> "**Percentuale elementi in carrello maggiore o uguale 50**"
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere impostato nessun
> Filtro Articoli la "Percentuale elementi in carrello" sarà ovviamente
> sempre uguale a 100

- **Percentuale Quantità in Carrello**: permette di indicare quanti
  articoli in percentuale, rispetto alla quantità totale di prodotti
  presenti in carrello, dovranno soddisfare un eventuale condizione di
  Filtro Articoli, affinché il pagamento in esame possa effettivamente
  essere visualizzato

> Supponendo dunque che l'esigenza sia quella di visualizzare il
> pagamento in esame solo nel momento in cui almeno il 30% della
> quantità complessiva di articoli presenti in carrello appartenga alla
> categoria 24 ("Outlet Uomo"), dovremmo configurare una condizione di
> applicabilità del tipo di quella rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamento_percentuale_quantita.bmp](./assets/media/image14.png)

> In questo modo infatti se dovessimo trovarci ad avere in carrello una
> quantità complessiva di 5 prodotti di cui 4 (quindi 80% del totale)
> appartenenti ad una categoria diversa dalla 24 ed uno solo (quindi il
> 20% del totale) appartenente alla categoria 24, la condizione
> impostata non risulterebbe soddisfatta e la promozione, di
> conseguenza, non verrebbe applicata.
>
> Se invece, in queste stesse condizioni, dovessimo trovarci ad avere in
> carrello una quantità complessiva di 6 prodotti di cui sempre 4 (ossia
> il 67% del totale) appartenenti ad una categoria diversa dalla 24 e i
> restanti 2 (quindi il 33% del totale) appartenenti invece alla
> categoria 24, la condizione impostata sarebbe verificata e, di
> conseguenza, la promozione verrebbe applicata

- **Quantità in Riga:** permette di definire una condizione di
  visibilità del pagamento basata sulla quantità di articoli presenti
  nelle singole righe dell'ordine.

> Nello specifico, in questo caso, verrà valutata la quantità di riga
> per ogni singolo prodotto che dovesse effettivamente soddisfare
> un'eventuale filtro articoli impostato mediante il relativo parametro.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_quantita_riga.bmp](./assets/media/image15.png)

> il pagamento verrà effettivamente visualizzato sul front end del sito
> solo nel momento in cui in ordine dovessimo avere almeno un articolo
> il cui codice inizia con AGLIANIC e la sua quantità di riga dovesse
> essere maggiore o uguale a 2
>
> Nelle condizioni indicate dunque, supponendo di avere anche i seguenti
> articoli in ordine

  -------------------------------------------------------------
  PRODOTTO                        QUANTITA' IN CARRELLO
  ------------------------------- -----------------------------
  AGLIANICVULDON99                1

  AGLIANICVULROI01                1

  BARBARESASILI_00                2
  -------------------------------------------------------------

> il pagamento in questione non verrà visualizzato e questo perché i
> prodotti che soddisfano il filtro articoli impostato sono i primi due
> ma nessuno di essi ha in riga una quantità maggiore o uguale a 2
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere in
> ordine i seguenti articoli

  -------------------------------------------------------------
  PRODOTTO                        QUANTITA' IN CARRELLO
  ------------------------------- -----------------------------
  AGLIANICVULDON99                2

  AGLIANICVULROI01                1

  BARBARESASILI_00                2
  -------------------------------------------------------------

> il pagamento verrebbe correttamente visualizzato e questo perché uno
> dei due prodotti che soddisfano il filtro articoli impostato
> (AGLIANICVULDON99) ha effettivamente una quantità di riga uguale a 2

- **Quantità Massima in Riga:** permette di definire una condizione di
  visibilità del pagamento basata sulla quantità di articoli presenti
  nelle singole righe dell'ordine.

> Nello specifico, in questo caso, verranno valutati tutti i prodotti
> che dovessero soddisfare un'eventuale filtro articoli impostato
> mediante il relativo parametro e, tra questi, verrà poi preso in
> considerazione solo quello con la quantità in riga più alta. Se la
> quantità di riga di questo articolo dovesse soddisfare la condizione
> impostata, il pagamento verrebbe correttamente visualizzato altrimenti
> no.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_quantita_massima_riga.bmp](./assets/media/image16.png)

> e supponendo anche di avere i seguenti articoli in ordine

  -------------------------------------------------------------
  PRODOTTO                        QUANTITA' IN CARRELLO
  ------------------------------- -----------------------------
  AGLIANICVULDON99                2

  AGLIANICVULROI01                1

  BARBARESASILI_00                3
  -------------------------------------------------------------

> il pagamento non verrà visualizzato e questo perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il primo ma tale quantità
> (2) non soddisfa comunque la condizione impostata (maggiore o uguale a
> 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere in
> ordine i seguenti articoli

  -------------------------------------------------------------
  PRODOTTO                        QUANTITA' IN CARRELLO
  ------------------------------- -----------------------------
  AGLIANICVULDON99                2

  AGLIANICVULROI01                4

  BARBARESASILI_00                3
  -------------------------------------------------------------

> il pagamento verrebbe correttamente visualizzato perché i prodotti che
> soddisfano il filtro articoli impostato sono sempre i primi due; tra
> questi quello con la quantità in riga più alta è il secondo
> (AGLIANICVULROI01) e tale quantità (4) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Quantità Minima in Riga:** permette di definire una condizione di
  visibilità del pagamento basata sulla quantità di articoli presenti
  nelle singole righe dell'ordine.

> Nello specifico, in questo caso, verranno valutati tutti i prodotti
> che dovessero soddisfare un'eventuale filtro articoli impostato
> mediante il relativo parametro e, tra questi, verrà poi preso in
> considerazione solo quello con la quantità in riga più bassa. Se la
> quantità di riga di questo articolo dovesse soddisfare la condizione
> impostata, il pagamento verrebbe correttamente visualizzato altrimenti
> no.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_quantita_minima_riga.bmp](./assets/media/image17.png)

> e supponendo anche di avere i seguenti articoli in ordine

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il pagamento non verrà visualizzato e questo perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) ma tale quantità (1) non soddisfa comunque la
> condizione impostata (maggiore o uguale a 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in ordine

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   3

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il pagamento verrebbe correttamente visualizzato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) e tale quantità (3) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Sconto in Riga**: permette di definire una condizione di visibilità
  del pagamento che tenga conto di tutti gli articoli presenti in ordine
  che soddisfano un eventuale "Filtro Articoli", o solo di quelli che,
  oltre a soddisfare un eventuale "Filtro Articoli", risultino anche
  privi di eventuali altri sconti già applicati.

> **ATTENZIONE! l'opzione "Sconto in Riga" è di tipo Stringa**
>
> In conseguenza di ciò per creare una condizione che verrà validata
> solo nel caso in cui i prodotti in ordine che soddisfano un eventuale
> "Filtro Articoli" risultino essere anche privi di altri sconti già
> applicati, **il campo "Valore" della condizione "Sconto in Riga" dovrà
> essere lasciato vuoto (**Valore = Stringa vuota).
>
> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_sconto_in_riga.bmp](./assets/media/image18.png)

> la condizione in esame verrà validata e il relativo pagamento
> visualizzato solo nel caso in cui tutti gli articoli presenti in
> ordine (**Percentuale Elementi in Carrello = 100**) appartengano alla
> categoria 24 e siano tutti privi di sconto (**Sconto in Riga = stringa
> vuota**)
>
> Al contrario, se anche tutti gli articoli presenti in ordine
> appartenessero effettivamente alla categoria 24 ma anche uno solo di
> essi avesse già uno sconto applicato (perché ad esempio importato dal
> gestionale) la condizione non verrebbe validata e, di conseguenza, il
> relativo pagamento non verrebbe visualizzato.
>
> **ATTENZIONE!** **si ricorda che nel caso di articoli box (campionari
> standard e configurabili) il prezzo del box stesso viene determinato
> sommando il prezzo dei singoli componenti al netto di eventuali sconti
> ad essi applicati**
>
> In sostanza dunque ad articoli Campionario non verrà mai applicato
> direttamente un determinato sconto.
>
> Nel momento in cui l'esigenza dovesse essere quindi quella di
> considerare non lo sconto dell'articolo campionario in sé ma quello
> eventualmente applicato ai suoi componenti sarà necessario verificare
> di aver correttamente impostato il parametro "**Gestione Articoli
> Box**" presente alla pagina "**Configurazione Catalogo**" del Wizard
> sul valore "**Considera i componenti del Box**".
>
> Per maggiori informazioni in merito a questo parametro si veda anche
> quanto indicato nel relativo capitolo di questo manuale ("*Catalogo --
> Configurazione Parametri Catalogo - Catalogo Mexal / Ho.Re.Ca. --
> Gestione Carrello*")

**Selezionato:** selezionando questo parametro, la corrispondente
modalità di pagamento sarà quella selezionata a default all'interno del
modulo di Checkout Ordine. I metodi di pagamento "selezionati a default"
verranno evidenziati in blu tra quelli presenti in elenco

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamento_default.bmp](./assets/media/image19.png)

**ATTENZIONE!** **E' possibile impostare come "selezionate a default"
due o più modalità di pagamento contemporaneamente**, in maniera tale
che, ad esempio, due utenti appartenenti a due gruppi differenti con
differenti modalità di pagamento abilitate si trovino sempre selezionata
a default una specifica modalità di pagamento.

Nel caso in cui un dato utente sia abilitato a visualizzare tutti i
pagamenti impostati sul Wizard come "selezionati a default" sul front
end del sito, in fase di checkout, si troverà effettivamente selezionato
a default solamente il primo di quelli presenti in elenco.

**NOTA BENE:** il pagamento abituale del cliente è sempre prioritario
rispetto a quella che dovrebbe essere, secondo il parametro appena
considerato, la modalità di pagamento selezionata a default.

Ciò significa dunque che, nel caso in cui alla pagina "Configurazione
Ordini" del Wizard il parametro "Gestione del Pagamento Abituale" sia
stato impostato sul valore "Abilitato", e nel caso in cui per il cliente
che sta effettuando l'ordine sia stato definito, all'interno del
gestionale, un pagamento abituale, quest'ultimo sarà sempre quello
selezionato a default.

**Gestisci:** consente di decidere se il pagamento in esame dovrà o meno
essere visualizzato in relazione a determinate tipologie di documento.
Ovviamente l'effettiva visibilità del pagamento dipenderà poi anche
dagli altri parametri di configurazione.

E' possibile selezionare uno dei seguenti valori:

- **Sempre:** selezionando questa opzione il pagamento in esame verrà
  sempre visualizzato indipendentemente dalla particolare tipologia di
  documento creato

- **Escludi Preventivi:** selezionando questa opzione il pagamento in
  esame non verrà visualizzato nel momento in cui il documento generato
  dovesse essere un preventivo.

- **Escludi Ordini:** selezionando questa opzione il pagamento in esame
  non verrà visualizzato nel momento in cui il documento generato
  dovesse essere un ordine

**ATTENZIONE!** il parametro in esame ha effetto solo ed esclusivamente
in fase di Checkout

In conseguenza di ciò all'interno del modulo per la "Stima dei Costi di
Pagamento" (pagina Carrello) verranno mostrati tutti i metodi di
pagamento abilitati indipendentemente dalle impostazioni settate per il
parametro in questione.

**Stato della Riga Ordine -- visibile solo per siti collegati a Mexal:**
consente di specificare lo stato in cui dovranno essere poste, in Mexal,
le varie righe dell'ordine nel momento in cui questo dovesse essere
concluso selezionando il pagamento in oggetto.

E' possibile indicare uno dei seguenti valori:

- **Evadibile**: in queste condizioni ogni riga dell'ordine nascerà,
  all'interno del gestionale, con stato impostato ad E (Evadibile),
  indipendentemente dalla effettiva disponibilità dei singoli articoli

- **Sospesa**: in queste condizioni ogni riga dell'ordine nascerà,
  all'interno del gestionale, con stato impostato ad S (Sospesa),
  indipendentemente dalla effettiva disponibilità dei singoli articoli

- **Bloccata**: in queste condizioni ogni riga dell'ordine nascerà,
  all'interno del gestionale, con stato impostato ad B (Bloccata),
  indipendentemente dalla effettiva disponibilità dei singoli articoli

- **Sospesa o Evadibile in base alla Disponibilità**: in queste
  condizioni, in fase di inserimento dell'ordine all'interno del
  gestionale verrà effettuato un controllo per ogni singolo articolo
  presente all'interno del documento; se la disponibilità dell'articolo
  dovesse essere superiore alla quantità inserita in ordine per quello
  stesso articolo, allora la relativa riga del documento verrà posta
  nello stato E (Evadibile); in caso contrario lo stato della riga verrà
  posto a S (Sospesa)

- **Bloccata o Evadibile in base alla Disponibilità**: in queste
  condizioni, in fase di inserimento dell'ordine all'interno del
  gestionale verrà effettuato un controllo per ogni singolo articolo
  presente all'interno del documento; se la disponibilità dell'articolo
  dovesse essere superiore alla quantità inserita in ordine per quello
  stesso articolo, allora la relativa riga del documento verrà posta
  nello stato E (Evadibile); in caso contrario lo stato della riga verrà
  posto a B (Bloccata)

**ATTENZIONE!** il tipo di disponibilità (Netta, Lorda, Esistenza
ecc...) che verrà valuta nei due casi sopra evidenziati, ed in base alla
quale dunque l'applicazione dovrà decidere se far nascere le righe
dell'ordine nello stato E piuttosto che nello stato S o B, è quello
impostato all'interno del campo "**Disponibilità**" presente
nell'omonima sezione della pagina "**Catalogo -- Configurazione
Parametri Catalogo**" del Wizard.

**ATTENZIONE! Quanto impostato per il parametro "Stato della Riga
Ordine" a livello di singolo pagamento è prioritario rispetto a quanto
impostato per lo stesso parametro a livello di "Configurazione Ordini"**

Ciò significa dunque che supponendo di essere nelle seguenti condizioni:

- parametro **"Stato della Riga Ordine"** presente alla pagina
  "**Configurazione Ordini**" del Wizard impostato sul valore
  "**Sospesa**"

- parametro **"Stato della Riga Ordine"** presente nella maschera di
  configurazione del pagamento "**PayPal**" impostato sul valore
  "**Evadibile**"

nel momento in cui l'utente dovesse concludere un ordine selezionando
come metodo di pagamento "PayPal" questo stesso ordine verrà inserito
sul gestionale con tutte le righe nello stato E (Evadibile)

Ovviamente se, nelle stesse condizioni, non dovesse essere stato
indicato nessun valore in fase di configurazione del pagamento "PayPal"
per il parametro in oggetto, farà fede quanto indicato alla pagina
"Configurazione Ordini" del Wizard e l'ordine verrà quindi inserito sul
gestionale con le righe a S (Sospese)

**Abilita pagamento per prenotazioni -- visibile solo per siti collegati
al gestionale Beauty:** consente, se selezionato, di visualizzare il
pagamento in questione anche in fase di conferma prenotazione (posto
ovviamente di aver abilitato lo step dei pagamenti).

Per maggiori informazioni relativamente alla gestione dei pagamenti
nell'ambito di prenotazioni da inserire all'interno del gestionale
Beauty, si veda anche quanto indicato all'interno del capitolo
"*Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componente
Prenotazione Custom Ecommerce Beauty*" di questo manuale.

##### OPZIONI DEL METODO DI PAGAMENTO

All'interno della sezione "**Opzioni del metodo di Pagamento**" è
possibile impostare le condizioni in corrispondenza delle quali il
pagamento in esame potrà effettivamente essere selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opzioni_metodo_pagamento.bmp](./assets/media/image20.png)

Nello specifico il parametro:

- **Codice Pagamento sul Gestionale (campo di sola lettura):**consente
  di visualizzare il codice corrispondente al pagamento attualmente
  selezionato all'interno della tabella pagamenti del gestionale

<!-- -->

- **Articolo Spesa del costo aggiuntivo:** codice dell'articolo di tipo
  S (spesa) che verrà utilizzato, lato gestionale, per gestire eventuali
  costi aggiuntivi sul pagamento in esame.

> **Per poter associare ad uno specifico pagamento eventuali costi
> aggiuntivi è necessario ricorrere ad un articolo di tipo Spesa
> opportunamente codificato ed abilitato per essere esportato e gestito
> anche all'interno del sito. Questo articolo verrà quindi aggiunto e
> visualizzato, a seguito della selezione della specifica modalità di
> pagamento, nel corpo del documento (non esistono infatti in Mexal,
> piuttosto che in uno dei gestionali Ho.Re.Ca., specifici campi nel
> piede del documento per gestire questi costi addizionali).**
>
> **NOTA BENE:**. gli articoli di tipo spesa utilizzati per gestire
> costi accessori sui pagamenti verranno automaticamente considerati
> come non visualizzabili in negozio, indipendentemente da quanto
> impostato per essi in relazione alla funzionalità "Visualizza in
> Negozio".
>
> Per maggiori informazioni relativamente alla codifica e alla gestione
> di articoli di tipo Spesa nei siti collegati ad uno dei gestionali
> Ho.Re.Ca. si veda anche la sezione "Configurazione Gestionale --
> Ho.Re.Ca. Parametri Configurazione Gestionale -- Funzionalità di
> Gestione Articoli -- Articoli di tipo Spesa" di questo manuale.

- **Costo aggiuntivo nel paese di default / nei paesi esteri:** consente
  di specificare quello che dovrà essere il valore del costo aggiuntivo
  da considerare nel momento in cui l'utente dovesse selezionare la
  modalità di pagamento in esame, oltre ad un indirizzo di spedizione
  merce appartenente / non appartenente al paese definito, nella
  corrispondente sezione del Wizard, come paese di default.

> Sono accettati i seguenti valori:

- **Valori numerici positivi -- es. 20:** in queste condizioni nel
  momento in cui l'utente dovesse selezionare la modalità di pagamento
  in esame dovrà poi sostenere un costo ulteriore di 20€

- **Valori percentuali positivi -- es. 20%:** in queste condizioni nel
  momento in cui l'utente dovesse selezionare la modalità di pagamento
  in esame dovrà sostenere un costo ulteriore pari al 20% **del Totale
  Merce comprensivo di IVA**

- **Valori numerici negativi -- es. -20:** in queste condizioni la
  selezione della modalità di pagamento in esame non andrà ad aumentare
  il totale del documento ma, al contrario, andrà a diminuire di 20€
  tale importo

- **Valori percentuali negativi -- es. -20%:** in queste condizioni la
  selezione della modalità di pagamento in esame non andrà ad aumentare
  il totale del documento ma, al contrario, andrà a diminuire tale
  importo di un valore pari al 20% **del Totale Merce comprensivo di
  IVA**

> **ATTENZIONE!** L'utilizzo di valori negativi per i costi aggiuntivi
> sui pagamenti potrebbe quindi rivelarsi particolarmente utile nel
> momento in cui l'esigenza dovesse essere, ad esempio, quella di
> applicare un certo sconto nel caso in cui l'utente dovesse selezionare
> una specifica modalità di pagamento.

- **Formula:** è possibile definire esattamente la formula da utilizzare
  per determinare il valore del costo aggiuntivo che dovrà poi essere
  applicato al pagamento.

> Nella definizione della formula è possibile utilizzare:

- **gli operatori standard (+-\*/)**

- **elevatore a potenza (Pow)**

> [Esempio]{.underline}: supponendo di voler calcolare il valore
> dell'espressione "due alla terza" la formula da utilizzare dovrà
> essere:
>
> **Pow(2,3)**

- **radice quadrata (Sqrt)**

> [Esempio]{.underline}: supponendo di voler calcolare il valore
> dell'espressione "radice quadrata di 16" la formula da utilizzare
> dovrà essere:
>
> **Sqrt(16)**

- **modulo (%)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma:
>
> **10%3**
>
> e consentirà di dividere il primo argomento per il secondo,
> restituendo come risultato solo il resto (nell'esempio indicato il
> risultato ottenuto sarà 1)

- **valore assoluto (Abs)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Abs(-5)**
>
> e consentirà di ottenere come risultato il valore assoluto del numero
> indicato tra parentesi (nell'esempio indicato il risultato ottenuto
> sarà 5)

- **valore intero (Truncate)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Truncate(5.2)**
>
> e consentirà di ottenere come risultato il valore intero del numero
> indicato tra parenesi (nell'esempio considerato il risultato ottenuto
> sarà 5)

- **valore intero superiore (Ceiling)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Ceiling(5.2)**
>
> e consentirà di ottenere come risultato il valore intero
> immediatamente superiore al numero indicato tra parentesi
> (nell'esempio indicato il risultato ottenuto sarà 6)

- **parentesi tonde**

- **la variabile x che rappresenta il valore del Totale Merce Ivato +
  eventuali spese presenti nel documento**

- **la variabile y che rappresenta il valore del Totale Merce NON
  ivato**

- **la variabile z che rappresenta il valore del Totale Merce Ivato**

- **istruzione condizionale "if"**

> All'interno della formula è possibile utilizzare anche l'istruzione
> condizionale "if" come operatore ternario quindi nel formato
>
> **if(condizione, valore da applicare se condizione verificata, valore
> da applicare se condizione non verificata)**
>
> **ATTENZIONE!** E' fondamentale che come separatore dei decimali venga
> utilizzato sempre e soltanto il "." (punto).
>
> Nel caso in cui si dovesse utilizzare come separatore la "," (virgola)
> la formula non risulterà essere corretta e il risultato ottenuto non
> sarà quindi quello desiderato.
>
> Il pulsante **"Aggiungi segnaposto"** presente immediatamente al di
> sotto di questi campi consente di inserire, nella eventuale formula
> utilizzata per determinare il costo aggiuntivo del pagamento in
> questione, gli elementi "Totale merce Ivato" e "Totale merce non
> Ivato" corrispondenti rispettivamente alle variabili y e z

- **Tipo Costo Aggiuntivo:** consente di specificare se l'importo del
  costo aggiuntivo che si sta codificando (e che è stato inserito nei
  due precedenti campi) dovrà essere considerato o meno comprensivo di
  iva. Sarà quindi possibile selezionare uno dei seguenti valori:

  - **Non Ivato:** in questo caso l'importo indicato nei precedenti
    campi "Costo aggiuntivo nel paese di default/nei paesi esteri", sarà
    considerato **iva esclusa**.

> In conseguenza di ciò se ad effettuare l'ordine sul sito dovesse
> essere un privato (generando quindi un OX) su tali importi verrà
> calcolata l'iva. L'importo del costo aggiuntivo sul pagamento,
> presente nel riepilogo dell'ordine alla voce "Spese" (quello
> evidenziato in figura)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\iva_spese_pagamento_1.bmp](./assets/media/image21.png)

> sarà dunque quello indicato all'interno dei due precedenti campi
> maggiorato dell'iva, calcolata secondo l'aliquota in uso all'interno
> del gestionale (iva cliente, particolarità iva, iva articolo, iva
> ripartita ...).
>
> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo del costo
> aggiuntivo sul pagamento, presente nel riepilogo dell'ordine alla voce
> "Spese", coinciderà esattamente con quanto inserito all'interno dei
> due precedenti campi. L'iva sul costo aggiuntivo verrà comunque
> calcolata e andrà ad influire sul totale della relativa voce presente
> nel piede del documento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\iva_spese_pagamento_2.bmp](./assets/media/image22.png)

- **Ivato:** in questo caso l'importo indicato nei precedenti campi
  "Costo aggiuntivo nel paese di default/nei paesi esteri", sarà
  considerato **iva compresa**. In conseguenza di ciò se ad effettuare
  l'ordine sul sito dovesse essere un privato (generando quindi un OX)
  l'importo del costo aggiuntivo sul pagamento, presente nel riepilogo
  dell'ordine, coinciderà esattamente con quello indicato all'interno
  dei precedenti campi.

> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo del costo
> aggiuntivo sul pagamento, presente nel riepilogo dell'ordine,
> coinciderà con quello inserito nei precedenti campi scorporato
> dell'iva, secondo l'aliquota in uso all'interno del gestionale (iva
> cliente, particolarità iva, iva articolo, iva ripartita ...). L'iva
> così calcolata andrà poi ad influire sul totale della relativa voce
> presente nel piede del documento.
>
> **ATTENZIONE!!** per quel che riguarda gli importi eventualmente
> indicati a fianco dei singoli metodi di pagamento presenti, in
> checkout, nel relativo step

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\iva_spese_pagamento_3.bmp](./assets/media/image23.png)

> questi potranno essere ivati o non ivati (con la relativa etichetta)
> dipendentemente da come è stato impostato il parametro "**Prezzo**"
> presente alla pagina "**Configurazione Catalogo**" del Wizard. Il
> consiglio, in questo senso è, ovviamente, quello di gestire questo
> valore coerentemente con la tipologia di documento generata e quindi
> con il valore che verrà poi indicato anche nel riepilogo dell'ordine.

- **Tipologia di totale dei limiti**: consente di specificare se gli
  importi indicati all'interno dei successivi campi "Limite Minimo /
  Massimo" dovranno essere considerati relativi al solo "Totale Merce"
  oppure al "Totale Merce Ivato + Spese + Trasporto".

> **ATTENZIONE!** nel momento in cui il parametro in questione dovesse
> essere impostato su "**Totale Merce**" sarà necessario considerare
> anche che l'importo effettivo sulla base del quale decidere di
> visualizzare o meno il pagamento in oggetto, verrà considerato
> comprensivo o meno anche di eventuali articoli spesa inserti in
> carrello (a seguito dell'applicazione di determinate promozioni o
> buoni sconto) dipendentemente dall'impostazione scelta per il
> parametro "**Gestione Totale Merce**" presente nella sezione
> "*Catalogo -- Configurazione Parametri Catalogo*" del Wizard

- **Gestione Limite:** consente di specificare se gli importi indicati
  all'interno dei successivi campi "Limite Minimo / Massimo" dovranno
  essere considerati o meno comprensivi di iva.

> **ATTENZIONE!** Per ovvie ragioni nel momento in cui il parametro
> "**Tipologia di totale dei limiti**" dovesse essere impostato su
> "**Totale Ordine**" l'unica opzione disponibile per il parametro
> "**Gestione Limite**" sarà "**Ivato**"

- **Limite Minimo / Massimo:** importo al di sotto / al di sopra del
  quale non abilitare la modalità di pagamento in esame.

> Nel caso in cui dunque il totale merce / ordine dovesse essere minore
> / maggiore del valore indicato all'interno di questo campo, la
> corrispondente modalità di pagamento non verrà visualizzata tra le
> possibili opzioni di scelta dell'utente **(indipendentemente dal fatto
> di aver impostato il parametro "Stato del Pagamento" su
> "Abilitato").**
>
> Occorre inoltre ricordare che l'importo indicato all'interno di questi
> campi:

- verrà considerato comprensivo o meno di iva a seconda di quanto
  impostato per il precedente parametro "**Gestione Limite**"

- sarà riferito al Totale merce o al Totale Ordine a seconda di quanto
  impostato per il precedente parametro "**Tipologia di totale dei
  limiti**"

- non tiene in considerazione eventuali Sconti/Abbuoni impostati, lato
  gestionale, sul relativo pagamento

> **NOTA BENE:** nel caso in cui i due parametri "Limite Minimo/Massimo
> del totale merce" vengano lasciati entrambi a 0 il corrispondente
> pagamento, se abilitato, comparirà sempre tra le possibili opzioni di
> scelta dell'utente.
>
> **NOTA BENE:** nel caso in cui il parametro "Limite Massimo del totale
> merce" sia lasciato a 0 il range di valori del totale merce in
> corrispondenza del quale visualizzare il pagamento in esame, andrà dal
> valore minimo all'infinito.

##### METODI DI TRASPORTO NON CONSENTITI

All'interno della sezione "**Metodi di trasporto non consentiti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opzioni_metodo_pagamento_2.bmp](./assets/media/image24.png)

è possibile specificare, selezionandoli dall'elenco presente nel box di
sinistra ed inserendoli nel box di destra, i metodi di trasporto in
corrispondenza dei quali il pagamento in esame non dovrà essere
visualizzato come possibile opzione di scelta per l'utente
**(indipendentemente dal fatto di aver impostato il parametro "Stato del
Pagamento" su "Abilitato")**.

##### LINEE ARTICOLO

La sezione "**Linee Articolo**" consente di associare il metodo di
pagamento in esame ad una o più linee articolo.

In questo modo dunque, il metodo di pagamento in oggetto verrà poi
proposto all\'utente in fase di acquisto, **solo ed esclusivamente nel
caso di ordini contenenti articoli appartenenti alla linea/linee
indicate.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_linee_articolo.bmp](./assets/media/image25.png)

Per creare un'associazione "Linea Articolo -- Pagamento" è sufficiente
selezionare la Linea desiderata dall'elenco presente nel box di
sinistra, ed inserirla nel box di destra cliccando sull'apposita
freccia.

Allo stesso modo per eliminare l'associazione "Linea Articolo --
Pagamento", sarà sufficiente selezionare la linea desiderata dall'elenco
di destra ed inserirla in quello di sinistra cliccando sull'apposita
freccia

**NOTA BENE:** per maggiori informazioni in merito alla gestione delle
linee articolo si vedano anche le sezioni "Configurazione Gestionale --
Mexal Parametri Configurazione Gestionale -- Mexal Attivazione Passweb
-- Funzionalità Mexal Articoli -- Gestione Linee Articolo" e
"Configurazione Gestionale -- Ho.Re.Ca. Parametri Configurazione
Gestionale -- Funzionalità di Gestione Articoli -- Gestione Linee
Articolo" di questo manuale.

##### GRUPPI

La sezione **"Gruppi"** consente infine di associare la modalità di
pagamento in esame ad uno o più gruppi di utenti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_gruppi_utente.bmp](./assets/media/image26.png)

Per creare un'associazione "Gruppo Utenti - Pagamento" è sufficiente
selezionare il Gruppo desiderato dall'elenco presente nel box di
sinistra, ed inserirlo nel box di destra cliccando sul pulsante
raffigurante una piccola freccia verde. Allo stesso modo per eliminare
l'associazione "Gruppo Utenti - Pagamento", sarà sufficiente selezionare
il Gruppo desiderato dall'elenco di destra ed inserirlo in quello di
sinistra cliccando sul pulsante raffigurante una piccola freccia rossa.

Una volta creata un'associazione "Gruppo Utenti -- Pagamento", il
pagamento in oggetto potrà essere utilizzato solo ed esclusivamente
dagli utenti appartenenti allo specifico gruppo.

**ATTENZIONE:** **Nel caso in cui ad effettuare l'ordine sia un Agente
(Ecommerce Mexal) per conto dei suoi clienti verranno considerati i
pagamenti associati all'eventuale gruppo di appartenenza dell'Agente**

**NOTA BENE:** per maggiori informazioni in merito alla gestione Gruppi
Utente si veda la sezione "Utenti -- Gruppi Utenti Sito" di questo
manuale.

##### QAPLA'

La sezione "**Qaplà**", visualizzabile solo nel momento in cui sia stata
attivata in maniera corretta l'integrazione tra Passweb e la relativa
piattaforma terza, consente di impostare determinate opzioni di gestione
della spedizione (es. Consegna al piano, Consegna al sabato ecc...) che
verranno poi passate a Qaplà nel momento in cui l'utente dovesse
selezionare in fase di checkout il metodo di pagamento in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_qapla.bmp](./assets/media/image27.png)

**ATTENZIONE!** la sezione Qaplà è visibile solo nel momento in cui
siano state inserite le relative chiavi di configurazione in
corrispondenza dei campi "**Qaplà API Key Privata**" e "**Qaplà API Key
Pubblica**" presenti nella sezione "**Logistica -- Qaplà**" alla pagina
"**Sito -- Preferenze**" del Wizard (tab "**Integrazioni**")

I parametri presenti all'interno di questa sezione consentono
rispettivamente di:

- **Opzioni di spedizione**: sono legate allo specifico corriere e,
  attualmente, sono disponibili solo per i corrieri Bartolini (BRT) e
  GLS.

> **Lato** **Qaplà l'effettiva gestione di queste informazioni dipende
> quindi dal corriere che verrà poi utilizzato per gestire la
> corrispondente spedizione**.
>
> In sostanza dunque, nel momento in cui il cliente dovesse selezionare,
> in fase di checkout, un metodo di pagamento configurato per inviare a
> Qaplà determinate opzioni di spedizione (es. la consegna al piano),
> Passweb invierà alla piattaforma terza, assieme ai dati dell'ordine,
> anche queste informazioni aggiuntive su come gestire la spedizione.
> Lato Qaplà tali informazioni diventeranno però visibili solo nel
> momento in cui l'utente dovesse decidere di gestire la spedizione con
> il corriere corretto.
>
> Supponendo dunque di configurare un metodo di pagamento con l'opzione
> "Servizio al Sabato" questa informazione sarà effettivamente visibile
> su Qaplà solo nel momento in cui la relativa spedizione dovesse poi
> essere gestita con GLS.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_opzioni_corriere.bmp](./assets/media/image28.png)

> **Un'altra cosa di fondamentale importanza da tenere in considerazione
> è che le opzioni di spedizione sono definite in fase di configurazione
> del metodo di pagamento e non possono quindi essere selezionate
> direttamente dall'utente sul front end del sito.**
>
> Nel momento in cui l'esigenza dovesse dunque essere quella di offrire
> all'utente, ad esempio, la possibilità di selezionare tra la "Consegna
> su appuntamento" o la "Consegna al piano" di Bartolini sarà necessario
> codificare due diversi metodi di pagamento, con descrizioni
> differenti, magari anche con due costi aggiuntivi differenti e
> comunque, ciascuno, con la relativa opzione di spedizione Qaplà
> selezionata.
>
> Ovviamente non è possibile selezionare in fase di checkout,
> contemporaneamente, due diversi metodi di pagamento, per cui se
> l'esigenza dovesse essere quella di permettere all'utente di decidere
> se selezionare, ad esempio, sia la consegna al piano che la consegna
> al sabato le opzioni di spedizione Qaplà non dovranno essere gestite
> sul metodo di pagamento ma attraverso apposite Spese Accessorie. Per
> maggiori informazioni in merito alla gestione delle Spese Accessorie
> si veda anche quanto indicato nel corrispondente capitolo di questo
> manuale ("*Ordini -- Spese Accessorie*")

- **Custom Label**: campi che possono esseri utilizzati per passare a
  Qaplà informazioni personalizzate di tipo testuale.

> A differenza delle opzioni di spedizione, non sono legate su Qaplà, ad
> uno specifico corriere.
>
> Anche le etichette personalizzate vanno comunque definite in fase di
> configurazione dello specifico metodo di pagamento e non potranno
> quindi essere inserite direttamente dagli utenti sul front end del
> sito.
>
> Come detto però su Qaplà questi dati sono indipendenti dal corriere
> effettivamente utilizzato per gestire la spedizione e potranno quindi
> essere sempre visualizzati all'interno dei campi "Custom 1 / 2 / 3"
> aprendo il dettaglio dell'ordine inviato da Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_custom_label_1.bmp](./assets/media/image29.png)

- **Tipologia di assicurazione:** consente di definire la metodologia di
  calcolo dell'importo da assicurare che dovrà poi essere passato a
  Qaplà nel momento in cui l'utente dovesse selezionare, in fase di
  checkout, il metodo di pagamento in esame.

> E' possibile selezionare una delle seguenti opzioni:

- **Disabilitato:** selezionando questa opzione non verrà trasmesso a
  Qaplà nessun importo da assicurare

- **Solo Merce**: in queste condizioni l'importo da assicurare passato a
  Qaplà coinciderà con il **Totale Merce Ivato**

- **Merce + Trasporto**: in queste condizioni l'importo da assicurare
  passato a Qaplà coinciderà con il Totale Merce Ivato + eventuali spese
  di trasporto (anch'esse ivate)

- **Totale ordine**: in queste condizioni l'importo da assicurare
  passato a Qaplà coinciderà con il Totale Ordine

> **ATTENZIONE!** lato Qaplà il valore dell'importo da assicurare verrà
> visualizzato nel dettaglio del documento a patto che la relativa
> spedizione sia gestita mediante uno specifico corriere (es. BRT, GLS
> ...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_importo_assicurazione.bmp](./assets/media/image30.png)

- **Contrassegno:** se selezionato, nel momento in cui l'utente dovesse
  selezionare in fase di checkout il pagamento in esame, verrà passata a
  Qaplà, assieme a tutti gli altri dati dell'ordine, anche
  l'informazione necessaria alla piattaforma terza per marcare quello
  specifico ordine come pagato in contrassegno.

> Al pari delle custom label anche questa informazione non è ovviamente
> dipendente dallo specifico corriere che verrà poi utilizzato per
> gestire la spedizione e potrà quindi essere visualizzata su Qaplà
> stessa sia a livello di elenco ordini che aprendo il dettaglio del
> relativo documento, come evidenziato nelle figure di seguito riportate

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_qapla_2.bmp](./assets/media/image31.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_qapla_3.bmp](./assets/media/image32.png)

Un' ultima considerazione di fondamentale importanza da fare è che, lato
Passweb, le "Opzioni di spedizione per Qaplà" possono essere associate,
a seconda delle esigenze, a:

- Metodi di Trasporto

- Spese Accessorie

- Pagamenti

Nel momento in cui si dovesse dunque decidere, per una qualsiasi
ragione, di configurare queste opzioni di spedizione contemporaneamente
per due o più dei suddetti elementi, sarà necessario prestare
particolare attenzione, in fase di configurazione, a non creare delle
possibili situazioni di conflitto come potrebbe essere ad esempio, un
metodo di trasporto con associata l'opzioni di consegna al piano per
Bartolini e un pagamento con associata invece, sempre per Bartolini,
l'opzione di consegna al sabato.

In queste condizioni infatti verranno passate a Qaplà entrambe le
opzioni di spedizione solo nel momento in cui l'utente dovesse
effettivamente selezionare quello specifico metodo di trasporto e anche
quello specifico pagamento.

Allo stesso modo, in caso di conflitti, verrà fatto un merge delle
informazioni da passare a Qaplà, anche per quel che riguarda eventuali
valori settati per le Custom Label.

Supponendo dunque di aver impostato per un determinato metodo di
trasporto la "Custom Label 1" di Qaplà con la stringa "Trasporto X" e la
"Custom Label 2" di un pagamento con la stringa "Pagamento Y", nel
momento in cui l'utente dovesse selezionare in fase di checkout quello
specifico metodo di trasporto e quello specifico pagamento verrà passato
a Qaplà sia il valore della "Custom Label 1" (determinato dalla
selezione del metodo di trasporto) che quello della "Custom Label 2"
(determinato invece dalla selezione del pagamento)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_custom_label_2.bmp](./assets/media/image33.png)

Nel momento in cui invece, sia per il metodo di trasporto che per il
pagamento selezionato dall'utente in fase di checkout dovesse essere
stato impostato un valore per la stessa Custom Label, verranno passate a
Qaplà ed inserite nello stesso campo entrambe queste informazioni
separate da un ;

Supponendo dunque di aver impostato la "Custom Label 1" per il metodo di
trasporto selezionato in fase di checkout sul valore "opzione A" e la
stessa "Custom Label 1" per il pagamento selezionato in fase di checkout
sul valore "opzione B" ci ritroveremo poi su Qaplà una situazione del
tipo di quella rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_custom_label_3.bmp](./assets/media/image34.png)

Infine, se conflitto dovesse verificarsi a livello di "Tipologia di
assicurazione" verrà utilizzato il seguente livello di priorità:

- Totale ordine

- Merce + trasporto

- Merce

- Disabilitata

Ciò significa dunque che nel momento in cui l'utente dovesse selezionare
in fase di checkout ad esempio, un metodo di trasporto configurato per
passare a Qaplà come importo da assicurare il Totale Merce + le spese di
trasporto e un pagamento configurato invece per passare a Qaplà come
importo da assicurare il solo Totale Ordine, seguendo l'ordine di
priorità sopra indicato l'importo da assicurare effettivamente passato a
Qaplà per quel determinato documento sarà proprio il Totale Ordine.

