# PARAMETRI GENERALI



Per ciascun Metodo di trasporto di tipo Passweb è possibile impostare un
valore per i seguenti parametri:

![](./assets/media/image264.png)

**Stato del Metodo di Trasporto:** permette di Abilitare/Disabilitare la
specifica spesa di trasporto, facendola quindi comparire o meno tra
quelle che il cliente potrà poi selezionare all'interno del sito web
(allo stesso modo di quanto avviene con i pulsanti "Attiva Trasporto" e
"Disattiva Trasporto" precedentemente esaminati)

**Ordinamento:** consente di assegnare alla modalità di spedizione in
esame uno specifico numero che verrà poi utilizzato per ordinare
l'elenco delle spedizioni disponibili, elenco questo visualizzato, sul
front end del sito, in fase di checkout piuttosto che all'interno del
relativo modulo per il preventivo sulle spese di spedizione presente in
carrello.

**ATTEZNIONE!** Le spedizioni attive per le quali non è stato
specificato un numero d'ordine verranno visualizzate per prime

Inoltre:

- a parità di ordinamento le spedizioni attive presenti in elenco
  verranno ordinate per descrizione

- nel caso in cui sia gestito il "vettore abituale", questo verrà
  visualizzato sempre e comunque come primo elemento in elenco
  (indipendentemente dal fatto di avergli assegnato o meno uno specifico
  numero d'ordine)

**Descrizione**: etichetta identificativa della modalità di spedizione
utilizzata

**Dettaglio**: consente di inserire ulteriori informazioni relativamente
al metodo di trasporto in esame.

**Visualizza dettaglio**: consente di decidere se, e dove visualizzare
le informazioni aggiuntive sulla spesa di trasporto in oggetto. E'
possibile selezionare uno dei seguenti valori:

- **Non visualizzare**: in queste condizioni non verrà, ovviamente,
  visualizzata nessuna informazione aggiuntiva sulla spesa di trasporto,
  indipendentemente da quanto inserito all'interno del campo "Dettaglio"

- **In fase di Checkout**: in queste condizioni una volta inserite,
  all'interno del campo "Dettaglio", le informazioni aggiuntive sulla
  spesa di trasporto, verrà visualizzato sul sito, in fase di checkout e
  accanto alla descrizione della spesa in esame, un pulsante
  "**Dettagli**" mediante il quale l'utente potrà visualizzare le
  informazioni aggiuntive precedentemente inserite.

![](./assets/media/image265.png)

- **Nel Dettaglio dell'Ordine:** in queste condizioni le informazioni
  aggiuntive sulla spesa di trasporto verranno visualizzate nel
  dettaglio dell'Ordine. Inoltre queste stesse informazioni verranno
  inserite anche in tutte le mail inviate dall'applicativo all'interno
  delle quali compare il dettaglio dell'ordine effettuato dal cliente.

![](./assets/media/image266.png)

- **In fase di Checkout e nel Dettaglio dell'Ordine:** in queste
  condizioni le informazioni aggiuntive sulla spesa di trasporto
  verranno visualizzate in fase di checkout (mediante l'apposito
  pulsante "Dettagli"), nel riepilogo dell'ordine che l'utente si
  appresta a confermare e anche in tutte le mail inviate
  dall'applicativo e che contengono il dettaglio dell'ordine effettuato
  dal cliente.

**Indicazione Abilitazione:** consente di impostare, in ciascuna delle
lingue attualmente gestite all'interno del sito, un testo personalizzato
mediante il quale poter indicare all'utente come comportarsi per
abilitare il trasporto in esame nel caso in cui questo non dovesse
essere selezionabile.

![](./assets/media/image267.png)

Il testo indicato all'interno di questo campo verrà poi inserito:

- Nella sezione del Checkout relativa alle Spedizioni

- Nel pop up visualizzato, sempre in Checkout, nel caso in cui sia stato
  selezionato il parametro "Mostra popup se non ci sono Spedizioni\"
  presente nella maschera di configurazione del componente Checkout

- In Carrello in fase di preventivo delle spese di spedizione

e soprattutto **verrà effettivamente visualizzato solo nel caso in cui
risulti valida almeno una delle seguenti condizioni**:

- non ci sono spedizioni selezionabili

- non è possibile procedere con l\'ordine senza selezionare una
  spedizione (parametro "Procedi se non ci sono spedizioni" nella
  maschera di configurazione del componente Checkout deselezionato)

- risultano essere presenti trasporti per la zona di spedizione indicata
  dall'utente che non vengono però mostrati a causa di uno o più dei
  seguenti parametri:

  - Filtro articoli: alcuni articoli in carrello non soddisfano il
    filtro impostato sul relativo metodo di trasporto (se nessuno degli
    articoli in ordine dovesse soddisfare il filtro, la spedizione non
    verrebbe considerata)

  - Limite minimo: il totale merce in carrello non raggiunge il limite
    minimo impostato sul relativo metodo di trasporto

  - Limite massimo: il totale merce in carrello supera limite massimo
    impostato sul relativo metodo di trasporto

Va de sé quindi che un messaggio di questo tipo dovrebbe essere
impostato solo nel caso in cui per il trasporto in esame si dovesse
effettivamente decidere di impostare uno dei limiti sopra indicati.

Il pulsante "**Aggiungi un segnaposto**" presente immediatamente al di
sotto del campo in questione consente di comporre il messaggio
utilizzando anche uno dei segnaposto presenti in elenco, segnaposto
questi che consentono di gestire:

- **Limite Minimo / Massimo**: consente di inserire all'interno del
  messaggio un segnaposto che verrà poi sostituito in maniera dinamica
  con il valore del Limite Minimo / Massimo eventualmente impostato per
  il trasporto in esame

- **Articoli Esclusi**: consente di inserire all'interno del messaggio
  un segnaposto che verrà poi sostituito in maniera dinamica con l'
  elenco degli articoli presenti in carrello che non soddisfano
  l'eventuale Filtro Articolo impostato sul trasporto in esame

- **Se Limite Minimo / Massimo**: consente di inserire all'interno del
  messaggio un' istruzione condizionale per visualizzare quanto inserito
  al suo interno solo nel caso in cui il totale merce in carrello non
  dovesse soddisfare il Limite Minimo / Massimo eventualmente impostata
  sul trasporto in esame

- **Se Articoli Esclusi**: consente di inserire all'interno del
  messaggio un' istruzione condizionale per visualizzare l' elenco di
  articoli presenti in carrello che non soddisfano l'eventuale Filtro
  Articolo impostato sul trasporto in esame

Grazie a questi segnaposto sarà quindi possibile impostare messaggi del
tipo

- *\$if(min_limit)\$Puoi usufruire della spedizione in Italia se
  raggiungi un minimo di \$min_limit\$.\$endif\$*

> che verrà visualizzato solo nel caso in cui il totale merce in
> carrello non dovesse superare il limite minimo impostato e indicherà
> all'utente anche l'effettivo valore che il totale merce dovrà
> raggiungere per abilitare il metodo di trasporto in questione.

- *\$if(excluded_items)\$Puoi usufruire della spedizione in Italia se
  rimuovi dal carrello i seguenti articoli:\<br
  /\>\$excluded_items\$\$endif\$*

> che verrà visualizzato solo nel caso in cui ci siano articoli in
> carrello che non soddisfano il filtro (esclusivo) eventualmente
> impostato sul trasporto in questione

- ...

**ATTENZIONE!** Nel caso in cui per il trasporto in esame dovesse essere
impostato contemporaneamente un limite minimo, un limite massimo e anche
un filtro articoli verrà visualizzato prima di tutto l'eventuale
messaggio relativo al filtro articoli, poi quello relativo al limite
minimo e, infine, quello relativo al limite massimo (posto ovviamente di
aver composto il messaggio utilizzando tutte le apposite istruzioni
condizionali)

**Filtro Articoli:** consente di impostare uno specifico filtro mediante
il quale poter condizionare la visibilità del metodo di trasporto in
esame alla presenza in carrello di determinati articoli.

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

> In questo caso dunque, la visibilità del metodo di trasporto sarà
> condizionata alla presenza in carrello dell'articolo Campionario in
> sé, indipendentemente da quelli che potranno essere i suoi componenti

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, per valutare la visibilità o meno del metodo di
> trasporto verranno presi in considerazione i componenti del
> Campionario ma non l'articolo Campionario in sé che, quindi, potrebbe
> anche non soddisfare il filtro impostato.

**ATTENZIONE! Il filtro definito mediante il campo in esame non è un
filtro esclusivo** per cui il relativo metodo di trasporto verrà
visualizzato sul front end del sito **anche se uno solo degli articoli
presenti in carrello** dovesse effettivamente soddisfare il filtro
impostato

Nel momento in cui l'esigenza dovesse essere invece quella di
visualizzare il metodo di trasporto solo se tutti gli articoli
effettivamente presenti in carrello dovessero soddisfare il filtro
impostato, non sarà più sufficiente definire il solo "Filtro articoli"
ma occorrerà impostare anche un ben preciso "**Filtro carrello**"

**Filtro carrello:** consente di impostare un filtro mediante il quale
poter condizionare la visibilità del metodo di trasporto in esame alla
quantità / numero di articoli presenti in ordine, a livello globale o di
singola riga e/o sulla base del fatto che gli articoli in carrello
abbiano o meno uno sconto già applicato. Di base quindi lavorando sul
"Filtro carrello" sarà possibile:

- decidere se il metodo di trasporto dovrà essere visualizzato solo nel
  momento in cui tutte le righe articolo presenti in carrello dovessero
  soddisfare un eventuale "Filtro Articoli" o anche se solo una certa
  percentuale di esse dovesse essere effettivamente sufficiente per fare
  scattare la promozione.

- decidere se la condizione di visibilità del metodo di trasporto dovrà
  essere validata considerando tutti gli articoli presenti in carrello
  che soddisfano un eventuale "Filtro Articoli", oppure solo quelli che,
  oltre a soddisfare un eventuale "Filtro Articoli", risultino anche
  privi di eventuali altri sconti già applicati.

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

![](./assets/media/image268.png)

- **Quantità in carrello:** permette di definire una condizione sulla
  **quantità complessiva di articoli presenti in carrello** (e quindi
  effettivamente in ordine).

> Supponendo dunque di impostare un filtro del tipo "**Quantità in
> carrello maggiore di 5**" il metodo di trasporto in esame verrà
> visualizzato solo ed esclusivamente nel caso in cui la quantità
> complessiva di articoli in carrello dovesse essere effettivamente
> maggiore di 5. Tale condizione potrebbe quindi essere soddisfatta
> inserendo in carrello un solo articolo in quantità 6 o, ad esempio,
> due distinti articoli ciascuno in quantità 3.

- **Elementi in carrello:** permette di definire una condizione sul
  **numero complessivo di articoli presenti in carrello** (e quindi
  effettivamente in ordine).

> Supponendo quindi di impostare un filtro del tipo "**Elementi in
> Carrello maggiore di 2**" il metodo di trasporto in esame verrà
> visualizzato solo ed esclusivamente nel caso in cui siano stati
> inseriti in carrello almeno 3 distinti articoli indipendentemente
> dalla quantità acquistata per ognuno di essi.
>
> **ATTENZIONE!** **Nel caso in cui, per il metodo di trasporto in
> esame, dovesse essere impostato anche un Filtro Articoli, nella
> valutazione della condizione sul numero di articoli presenti in
> carrello verranno considerati solo ed esclusivamente gli articoli che
> soddisfano il filtro impostato.**
>
> Di base dunque se dovessimo trovarci in una situazione mista in cui
> sono presenti in carrello sia prodotti che soddisfano un eventuale
> Filtro Articoli sia prodotti che non lo soddisfano, nel momento in cui
> quelli che lo soddisfano dovessero soddisfare anche eventuali
> condizioni impostate sul numero di elementi, allora il metodo di
> trasporto verrebbe correttamente applicata.
>
> Diversamente se l'esigenza dovesse essere quella di non applicare
> metodo di trasporto in una situazione mista, in cui ci ritroviamo in
> carrello prodotti che soddisfano il Filtro Articoli ma anche prodotti
> che non lo soddisfano, sarà necessario utilizzare allora per il Filtro
> Carrello l'opzione "Percentuale Elementi in Carrello"

- **Elementi distinti in Carrello**: stesso funzionamento della
  condizione "Elementi in carrello" con la particolarità però di
  considerare eventuali righe che fanno riferimento allo stesso articolo
  come un unico elemento in carrello.

> Supponendo dunque di impostare un filtro del tipo "Elementi distinti
> in carrello maggiore di 2" il metodo di trasporto in esame verrà
> visualizzato solo nel caso in cui dovessero essere presenti in
> carrello almeno 3 righe di articoli questa volta **tutti diversi tra
> loro.**

- **Percentuale Elementi in Carrello**: permette di indicare la
  percentuale di articoli presenti in carrello che dovranno soddisfare
  un eventuale condizione di Filtro Articoli affinché il metodo di
  trasporto in esame possa effettivamente essere visualizzato.

> Nel momento in cui l'esigenza dovesse essere dunque quella di non
> visualizzare il metodo di trasporto sul front end del sito in una
> situazione mista, mostrandolo invece solo ed esclusivamente nel caso
> in cui tutti gli articoli presenti in carrello dovessero soddisfare
> un'eventuale condizioni di Filtro Articoli, sarà allora necessario
> impostare un Filtro Carrello del tipo "**Percentuale elementi in
> carrello = 100**"

![](./assets/media/image13.png)

> In queste condizioni se dovessimo avere in carrello anche un solo
> articolo che non soddisfa la condizione impostata all'interno del
> campo "Filtro Articoli" il metodo di trasporto, indipendentemente da
> tutto il resto, non verrà visualizzato.
>
> Allo stesso modo se l'esigenza dovesse essere quella di visualizzare
> il metodo di trasporto quando almeno il 50% delle righe articolo
> presenti in carrello dovessero soddisfare la condizione di Filtro
> Articoli, sarà allora necessario impostare un Filtro Quantità del tipo
> "**Percentuale elementi in carrello maggiore o uguale 50**"
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere impostato nessun
> Filtro Articoli la "Percentuale elementi in carrello" sarà ovviamente
> sempre uguale a 100

- **Percentuale Quantità in Carrello**: permette di indicare quanti
  articoli in percentuale, rispetto alla quantità totale di prodotti
  presenti in carrello, dovranno soddisfare un eventuale condizione di
  Filtro Articoli, affinché il metodo di trasporto in esame possa
  effettivamente essere visualizzato

> Supponendo dunque che l'esigenza sia quella di visualizzare il
> trasporto in esame solo nel momento in cui almeno il 30% della
> quantità complessiva di articoli presenti in carrello appartenga alla
> categoria 24 ("Outlet Uomo"), dovremmo configurare una condizione di
> applicabilità del tipo di quella rappresentata in figura

![](./assets/media/image14.png)

> In questo modo infatti se dovessimo trovarci ad avere in carrello una
> quantità complessiva di 5 prodotti di cui 4 (quindi 80% del totale)
> appartenenti ad una categoria diversa dalla 24 ed uno solo (quindi il
> 20% del totale) appartenente alla categoria 24, la condizione
> impostata non risulterebbe soddisfatta e il metodo di trasporto, di
> conseguenza, non verrebbe visualizzato.
>
> Se invece, in queste stesse condizioni, dovessimo trovarci ad avere in
> carrello una quantità complessiva di 6 prodotti di cui sempre 4 (ossia
> il 67% del totale) appartenenti ad una categoria diversa dalla 24 e i
> restanti 2 (quindi il 33% del totale) appartenenti invece alla
> categoria 24, la condizione impostata sarebbe verificata e, di
> conseguenza, il relativo metodo di trasporto verrebbe correttamente
> visualizzato

- **Quantità in Riga:** permette di definire una condizione di
  visibilità del metodo di trasporto basata sulla quantità di articoli
  presenti nelle singole righe dell'ordine.

> Nello specifico, in questo caso, verrà valutata la quantità di riga
> per ogni singolo prodotto che dovesse effettivamente soddisfare
> un'eventuale filtro articoli impostato mediante il relativo parametro.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![](./assets/media/image15.png)

> il metodo di trasporto verrà effettivamente visualizzato sul front end
> del sito solo nel momento in cui in ordine dovessimo avere almeno un
> articolo il cui codice inizia con AGLIANIC e la sua quantità di riga
> dovesse essere maggiore o uguale a 2
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

> il metodo di trasporto in questione non verrà visualizzato e questo
> perché i prodotti che soddisfano il filtro articoli impostato sono i
> primi due ma nessuno di essi ha in riga una quantità maggiore o uguale
> a 2
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

> il metodo di trasporto verrebbe correttamente visualizzato e questo
> perché uno dei due prodotti che soddisfano il filtro articoli
> impostato (AGLIANICVULDON99) ha effettivamente una quantità di riga
> uguale a 2

- **Quantità Massima in Riga:** permette di definire una condizione di
  visibilità del pagamento basata sulla quantità di articoli presenti
  nelle singole righe dell'ordine.

> Nello specifico, in questo caso, verranno valutati tutti i prodotti
> che dovessero soddisfare un'eventuale filtro articoli impostato
> mediante il relativo parametro e, tra questi, verrà poi preso in
> considerazione solo quello con la quantità in riga più alta. Se la
> quantità di riga di questo articolo dovesse soddisfare la condizione
> impostata, il metodo di trasporto verrebbe correttamente visualizzato
> altrimenti no.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![](./assets/media/image16.png)

> e supponendo anche di avere i seguenti articoli in ordine

  -------------------------------------------------------------
  PRODOTTO                        QUANTITA' IN CARRELLO
  ------------------------------- -----------------------------
  AGLIANICVULDON99                2

  AGLIANICVULROI01                1

  BARBARESASILI_00                3
  -------------------------------------------------------------

> il metodo di trasporto non verrà visualizzato e questo perché i
> prodotti che soddisfano il filtro articoli impostato sono i primi due;
> tra questi quello con la quantità in riga più alta è il primo ma tale
> quantità (2) non soddisfa comunque la condizione impostata (maggiore o
> uguale a 3)
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
> impostata, il metodo di trasporto verrebbe correttamente visualizzato
> altrimenti no.
>
> Supponendo dunque di considerare una configurazione del tipo di quella
> rappresentata in figura

![](./assets/media/image17.png)

> e supponendo anche di avere i seguenti articoli in ordine

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il metodo di trasporto non verrà visualizzato e questo perché i
> prodotti che soddisfano il filtro articoli impostato sono i primi due;
> tra questi quello con la quantità in riga più bassa è il secondo
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

> il metodo di trasporto verrebbe correttamente visualizzato perché i
> prodotti che soddisfano il filtro articoli impostato sono i primi due;
> tra questi quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) e tale quantità (3) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Sconto in Riga**: permette di definire una condizione di visibilità
  del metodo di trasporto che tenga conto di tutti gli articoli presenti
  in ordine che soddisfano un eventuale "Filtro Articoli", o solo di
  quelli che, oltre a soddisfare un eventuale "Filtro Articoli",
  risultino anche privi di eventuali altri sconti già applicati.

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

![](./assets/media/image18.png)

> la condizione in esame verrà validata e il relativo trasporto
> visualizzato solo nel caso in cui tutti gli articoli presenti in
> ordine (**Percentuale Elementi in Carrello = 100**) appartengano alla
> categoria 24 e siano tutti privi di sconto (**Sconto in Riga = stringa
> vuota**)
>
> Al contrario, se anche tutti gli articoli presenti in ordine
> appartenessero effettivamente alla categoria 24 ma anche uno solo di
> essi avesse già uno sconto applicato (perché ad esempio importato dal
> gestionale) la condizione non verrebbe validata e, di conseguenza, il
> relativo metodo di trasporto non verrebbe visualizzato.
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

**Selezionato:** selezionando questo parametro, il corrispondente metodo
di trasporto sarà quello selezionato a default all'interno del modulo di
Checkout Ordine. I metodi di trasporto "selezionati a default" sono
evidenziati in blu tra quelli presenti in elenco

![](./assets/media/image269.png)

**ATTENZIONE!** E' possibile impostare come "selezionati a default" due
o più metodi di trasporto contemporaneamente, in maniera tale che, ad
esempio, due utenti appartenenti a due gruppi differenti con differenti
metodi di trasporto abilitati si trovino sempre selezionato a default
uno specifico metodo di trasporto.

Nel caso in cui un dato utente sia abilitato a visualizzare tutti i
metodi di trasporto impostati sul Wizard come "selezionati a default"
sul front end del sito, in fase di checkout, si troverà effettivamente
selezionato a default solamente il primo di quelli presenti in elenco.

**ATTENZIONE: nel caso di siti Ecommerce collegati a Mexal** il
trasporto abituale del cliente è sempre prioritario rispetto a quello
che dovrebbe essere, secondo il parametro appena considerato, il metodo
di trasporto selezionato a default.

Ciò significa dunque che, per la tipologia di siti in oggetto, nel caso
in cui alla pagina "Configurazione Ordini" del Wizard il parametro
"**Gestione del Trasporto Abituale**" sia stato impostato sul valore
"**Abilitato**", e nel caso in cui per il cliente che sta effettuando
l'ordine sia stato definito, in Mexal, un vettore abituale, quest'ultimo
sarà sempre quello selezionato a default.

**Valuta di riferimento:** permette di selezionare, tra le valute
gestite all'interno del sito, la specifica valuta in cui dovranno essere
considerati gli importi relativi alla modalità di spedizione in oggetto.

**Scaglioni e Calcolo Percentuale:** permette di specificare l'unità di
misura sulla base della quale verranno definiti i vari scaglioni nel
caso di **Spese di Trasporto di Tipo Tabellare** e la base di calcolo
(**Totale Merce o Imponibile**) da utilizzare per la determinazione dei
valori in percentuale.

Nello specifico poi, per quel che riguarda i valori di Totale Merce e
Imponibile utilizzati per determinare in quale scaglione si ricade, ed
eventualmente anche l'importo dello scaglione stesso occorre sempre
ricordare che:

- Totale Merce ed Imponibile verranno considerati comprensivi o meno di
  eventuali articoli spesa inserti in carrello (a seguito
  dell'applicazione di determinate promozioni o buoni sconto)
  dipendentemente dall'impostazione scelta per il parametro "**Gestione
  Totale Merce**" presente nella sezione "*Catalogo -- Configurazione
  Parametri Catalogo*" del Wizard

- Totale Merce ed Imponibile verranno considerati **sempre al netto di
  eventuali articoli di tipo "Gift Card" inseriti in ordine**. In
  conseguenza di ciò possiamo quindi affermare che eventuali Gift Card
  (sia Fisiche che Virtuali) presenti in ordine non avranno alcun
  impatto né sulla determinazione dello scaglione di applicazione della
  spesa di trasporto, né tanto meno su quello che potrebbe essere
  l'importo assegnato a quel determinato scaglione (nel caso ovviamente
  di calcolo in percentuale)

E' possibile selezionare uno dei seguenti valori:

- **Scaglioni in base al Prezzo con Costo Fisso o Calcolo Percentuale
  sul Totale Merce**: in questo caso gli scaglioni della spesa di
  trasporto verranno definiti in base al Totale Merce. Il passaggio
  quindi da uno scaglione ad un altro e conseguentemente l'applicazione
  di uno specifico importo per la spesa in esame dipenderà dal Totale
  Merce (comprensivo di IVA).

> Allo stesso modo, in queste condizioni, nel caso in cui dovessero
> essere indicati dei valori in percentuale, questa verrà calcolata
> sempre sul Totale Merce (comprensivo di IVA)

- **Scaglioni in base all'Imponibile con Costo Fisso o Calcolo
  Percentuale sull'Imponibile:** in questo caso gli scaglioni della
  spesa di trasporto verranno definiti in base all'Imponibile (Totale
  Merce **NON** comprensivo di IVA). Il passaggio dunque da uno
  scaglione all\'altro, e conseguentemente l\'applicazione di uno
  specifico importo per la spesa in esame, dipenderà dal valore
  dell'Imponibile (Totale Merce **NON** comprensivo di IVA).

> In queste condizioni, nel caso in cui dovessero essere indicati dei
> valori in percentuale questa verrà calcolata sempre sull'Imponibile
> (Totale merce **NON** comprensivo di IVA)

- **Scaglioni in base al numero di Articoli con Costo Fisso o Calcolo
  Percentuale sul Totale Merce:** in questo caso gli scaglioni della
  spesa di trasporto verranno definiti in base al numero di articoli
  presenti in ordine. Il passaggio dunque da uno scaglione all\'altro, e
  conseguentemente l\'applicazione di uno specifico importo per la spesa
  in esame, dipenderà dal numero di articoli acquistati.

> **ATTENZIONE!** Nel calcolo del numero di articoli in ordine non
> verranno considerati articoli di tipo Gift Card
>
> In queste condizioni, ovviamente, nel momento in cui dovessero essere
> indicati dei valori in percentuale, la percentuale specificata verrà
> calcolata sempre sul Totale Merce (comprensivo di IVA)

- **Scaglioni in base al numero di Articoli con Costo Fisso o Calcolo
  Percentuale sull'Imponibile:** in questo caso gli scaglioni della
  spesa di trasporto verranno definiti in base al numero di articoli
  presenti in ordine. Il passaggio dunque da uno scaglione all\'altro, e
  conseguentemente l\'applicazione di uno specifico importo per la spesa
  in esame, dipenderà dal numero di articoli acquistati.

> **ATTENZIONE!** Nel calcolo del numero di articoli in ordine non
> verranno considerati articoli di tipo Gift Card
>
> In queste condizioni, ovviamente, nel momento in cui dovessero essere
> indicati dei valori in percentuale, la percentuale specificata verrà
> calcolata sempre sull'Imponibile (Totale merce **NON** comprensivo di
> IVA)

- **Scaglioni in base al campo Personalizzato con Costo Fisso o Calcolo
  Percentuale sul Totale Merce:** in questo caso gli scaglioni della
  spesa di trasporto che si sta codificando potranno essere definiti,
  **per siti Ecommerce collegati a Mexal:**

  - sulla base di quanto indicato all'interno dello specifico campo
    gestionale collegato alla funzionalità Mexal **"Spese di trasporto a
    Scaglioni"**

  - sulla base del Peso indicato all'interno del relativo campo presente
    nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

  - sulla base di quanto indicato all'interno di un Attributo Articolo
    Passweb appositamente realizzato

> Nel caso invece di **siti Ecommerce collegati ad uno dei gestionali
> Ho.Re.Ca.** gli scaglioni della spesa di trasporto potranno essere
> definiti:

- sulla base di quanto impostato per il campo **"Misuratore Trasporto a
  Scaglioni"** nell'Anagrafica Passweb degli articoli presenti in ordine
  (sezione **Informazioni Generali**)

- sulla base del Peso indicato all'interno del relativo campo presente
  nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

- sulla base di quanto indicato all'interno di un Attributo Articolo
  Passweb appositamente realizzato.

> **ATTENZIONE!** In queste condizioni nel caso in cui dovessero essere
> indicati dei valori in percentuale, la percentuale indicata verrà
> calcolata sempre **sul Totale Merce** (comprensivo di IVA).

- **Scaglioni in base al campo Personalizzato con Costo Fisso o Calcolo
  Percentuale sull'Imponibile:** come nel caso precedente, anche in
  queste condizioni, gli scaglioni della spesa di trasporto che si sta
  codificando potranno essere definiti, **per siti Ecommerce collegati a
  Mexal:**

  - sulla base di quanto indicato all'interno dello specifico campo
    gestionale collegato alla funzionalità Mexal **"Spese di trasporto a
    Scaglioni"**

  - sulla base del Peso indicato all'interno del relativo campo presente
    nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

  - sulla base di quanto indicato all'interno di un Attributo Articolo
    Passweb appositamente realizzato

> Nel caso invece di **siti Ecommerce collegati ad uno dei gestionali
> Ho.Re.Ca.** gli scaglioni della spesa di trasporto potranno essere
> definiti:

- sulla base di quanto impostato per il campo **"Misuratore Trasporto a
  Scaglioni"** nell'Anagrafica Passweb degli articoli presenti in ordine
  (sezione **Informazioni Generali**)

- sulla base del Peso indicato all'interno del relativo campo presente
  nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

- sulla base di quanto indicato all'interno di un Attributo Articolo
  Passweb appositamente realizzato.

> **ATTENZIONE!** A differenza del caso precedente in queste condizioni,
> nel momento in cui dovessero essere indicati dei valori in
> percentuale, la percentuale indicata verrà calcolata **sempre
> sull'Imponibile** (Totale merce NON comprensivo di IVA).

**NOTA BENE:** Per maggiori informazioni relativamente alla gestione
delle spese di trasporto a scaglioni sulla base di un campo
personalizzato, si veda anche il successivo capitolo di questo manuale
("Mexal / Ho.Re.Ca. Spese di trasporto a scaglioni")

**Tipo di campo:** visualizzato solo nel caso in cui il precedente
parametro "**Scaglioni e Calcolo percentuale**" sia stato impostato su
uno dei seguenti valori: **Scaglioni in base al campo Personalizzato con
Costo Fisso** o **Calcolo Percentuale sul Totale Merce** oppure
**Scaglioni in base al campo Personalizzato con Costo Fisso** o
**Calcolo Percentuale sull'Imponibile**.

Consente di stabilire la tipologia del campo da utilizzare nel calcolo
dello scaglione in cui ricade la spesa di trasporto in oggetto.

E' possibile selezionare uno dei seguenti valori:

- **Campo Articolo:** in queste condizioni sarà possibile decidere di
  utilizzare come campo per il calcolo dello scaglione, selezionandolo
  dal menu a tendina presente in corrispondenza del successivo parametro
  (**Campo**), il Peso definito per l'articolo all'interno del
  corrispondente campo dell'Anagrafica Passweb (sezione
  "**Spedizione**"), oppure il campo gestionale collegato alla
  funzionalità Mexal **"Spese di trasporto a Scaglioni" (**opzione
  "**Misuratore**")

![](./assets/media/image270.png)

- **Attributo Articolo:** in queste condizioni sarà possibile decidere
  di utilizzare come campo per il calcolo dello scaglione,
  selezionandolo dal menu a tendina presente in corrispondenza del
  successivo parametro (**Attributo**), uno degli Attributi articolo
  Passweb appositamente creati per questo scopo

![](./assets/media/image271.png)

> **ATTENZIONE!** All'interno del menu a tendina verranno visualizzati
> solo ed esclusivamente Attributi Articolo di tipo "**Testo**" o
> "**Numero**"

**Gestione Limite:** consente di indicare se i successivi valori
impostati all'interno dei campi "Limite Minimo / Massimo del totale
merce" dovranno essere considerati o meno privi di iva

**Limite Minimo del totale merce:** valore del totale merce al di sotto
del quale la modalità di spedizione in esame non dovrà essere attivata.

Nel caso in cui dunque il totale merce del documento dovesse essere
minore del valore indicato all'interno di questo campo, la
corrispondente modalità di spedizione non verrà visualizzata tra le
possibili opzioni di scelta dell'utente **(indipendentemente dal fatto
di aver impostato il parametro "Stato del Metodo di Trasporto" su
"Abilitato").**

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**Limite Massimo del totale merce:** valore del totale merce al di sopra
del quale la modalità di spedizione in esame non dovrà essere attivata.

Nel caso in cui dunque il totale merce del documento dovesse essere
maggiore o uguale al valore indicato all'interno di questo campo, la
corrispondente modalità di spedizione non verrà visualizzata tra le
possibili opzioni di scelta dell'utente **(indipendentemente dal fatto
di aver impostato il parametro "Stato del Metodo di Trasporto" su
"Abilitato").**

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**NOTA BENE:** nel caso in cui l'utente che effettua l'ordine abbia una
valuta diversa da quella specificata all'interno del campo "Valuta di
riferimento" gli importi dei limiti minimo e massimo specificati in fase
di configurazione della spesa di trasporto verranno convertiti nella
valuta in uso dal cliente.

**ATTENZIONE!** anche in questo caso il Totale Merce, sarà considerato
comprensivo o meno di eventuali articoli spesa inserti in carrello (a
seguito dell'applicazione di determinate promozioni o buoni sconto)
dipendentemente dall'impostazione scelta per il parametro "**Gestione
Totale Merce**" presente nella sezione "*Catalogo -- Configurazione
Parametri Catalogo*" del Wizard

**Larghezza massima imballo (cm):** consente di indicare la larghezza
massima che potrà assumere uno degli imballi coinvolti nella spedizione.
Nel momento in cui uno degli articoli in ordine dovesse avere una
larghezza superiore a quella indicata all'interno di questo campo, la
modalità di spedizione in esame non verrà proposta tra quelle
selezionabili dall'utente

**Altezza massima imballo (cm):** consente di indicare l'altezza massima
che potrà assumere uno degli imballi coinvolti nella spedizione. Nel
momento in cui uno degli articoli in ordine dovesse avere un'altezza
superiore a quella indicata all'interno di questo campo, la modalità di
spedizione in esame non verrà proposta tra quelle selezionabili
dall'utente

**Profondità massima imballo (cm):** consente di indicare la profondità
massima che potrà assumere uno degli imballi coinvolti nella spedizione.
Nel momento in cui uno degli articoli in ordine dovesse avere una
profondità superiore a quella indicata all'interno di questo campo, la
modalità di spedizione in esame non verrà proposta tra quelle
selezionabili dall'utente

**Volume massimo (cm^3^):** consente di indicare il volume che potranno
assumere gli articoli coinvolti nella spedizione. Nel momento in cui il
volume calcolato **(Larghezza x Altezza x Profondità x Quantità articolo
in ordine**) dovesse essere superiore a quello indicato all'interno di
questo campo, la modalità di spedizione in esame non verrà proposta tra
quelle selezionabili dall'utente

**Peso massimo (kg):** consente di indicare il peso massimo che potranno
assumere gli articoli coinvolti nella spedizione. Nel momento in cui il
peso calcolato **(Peso Singolo articolo x Quantità articolo in ordine**)
dovesse essere superiore a quello indicato all'interno di questo campo,
la modalità di spedizione in esame non verrà proposta tra quelle
selezionabili dall'utente

**ATTENZIONE!** Per maggiori informazioni relativamente a come poter
gestire le dimensioni dei singoli articoli si rimanda a quanto indicato
all'interno del relativo capitolo di questo manuale ("*Catalogo --
Gestione Articoli -- Articoli -- Anagrafica Articolo / Servizio --
Anagrafica Passweb -- Spedizione*")

**Tipo Costo:** consente di indicare se l'importo definito per la
specifica zona di consegna merce dovrà essere considerato o meno
comprensivo di iva. E' possibile selezionare uno dei seguenti valori:

- **Non Ivato:** in questo caso l'importo specificato per la spesa di
  trasporto sarà considerato **iva esclusa**. In conseguenza di ciò se
  ad effettuare l'ordine sul sito dovesse essere un privato (generando
  quindi un OX) su tali importi verrà calcolata l'iva. L'importo della
  spesa di trasporto, presente nel riepilogo dell'ordine (quello
  evidenziato in figura)

![](./assets/media/image272.png)

> sarà dunque quello definito in fase di configurazione del trasporto
> stesso maggiorato dell'iva.
>
> L'aliquota utilizzata per il calcolo dell'IVA potrà variare in
> relazione al fatto di gestire le spese di trasporto mediante
> l'apposita voce presente nel piede del documento oppure mediante un
> articolo spesa che verrà inserito nel corpo del documento stesso.
>
> In particolare nel primo caso (**Spese di trasporto gestite nel piede
> del documento**) l'aliquota utilizzata sarà esattamente quella
> impostata, per siti **Ecommerce collegati a Mexal,** all'interno del
> campo "**Aliquota Iva Spese Trasporto**" della tabella gestionale
> "**Bolli e Spese Banca**"

![](./assets/media/image273.png)

> per i siti **Ecommerce collegati ad uno dei gestionali Ho.Re.Ca**.,
> invece, verrà considerata l'aliquota impostata sul Wizard di Passweb
> all'interno del campo "**Aliquota iva Spese trasporto**" della
> maschera di "**Configurazione Parametri dell'ordine**".

![](./assets/media/image274.png)

> **ATTENZIONE!** nel momento in cui si dovesse decidere di gestire le
> spese di trasporto nel piede del documento e i due campi sopra
> evidenziati non dovessero avere una specifica aliquota impostata,
> l'iva verrà ripartita (allo stesso modo di quanto avviene anche nel
> gestionale) sulla base delle singole aliquote degli articoli in
> ordine. In questo caso inoltre (iva ripartita) se l'utente che
> effettua l'ordine dovesse avere la fatturazione elettronica abilitata
> verrà comunque considerata l'aliquota iva maggiore tra quelle in uso
> agli articoli presenti in ordine
>
> Nel secondo caso (spese di trasporto gestite mediante apposito
> articolo spesa inserito nel corpo del documenti) l'aliquota utilizzata
> sarà invece quella applicata sul gestionale all'articolo di tipo Spesa
> indicato nel successivo campo "Articolo".
>
> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo della spesa di
> trasporto, presente nel riepilogo dell'ordine, coinciderà esattamente
> con quello definito in fase di configurazione del trasporto stesso.
>
> **L'iva sulla spesa di trasporto verrà comunque calcolata, come sopra
> indicato**, e andrà quindi ad influire sul totale della relativa voce
> presente nel piede del documento.

![](./assets/media/image275.png)

> **ATTENZIONE!** in caso di iva ripartita gli arrotondamenti utilizzati
> (anche all'interno del gestionale) potrebbero portare ad avere valori
> differenti a seconda del fatto di gestire le spese di trasporto nel
> piede del documento oppure mediante un articolo spesa inserito nel
> corpo del documento stesso.
>
> Nel primo caso infatti (spese nel piede del documento) i calcoli
> verranno effettuati considerando sempre due decimali (come del resto
> avviene anche nel gestionale).
>
> Nel secondo caso invece (spese nel corpo del documento mediante un
> apposito articolo spesa) i calcoli verranno effettuati considerando lo
> stesso numero di decimali impostati ed utilizzati per il prezzo
> (parametro "Visualizzazione decimali sui Prezzi" in Configurazione
> Catalogo)

- **Ivato:** in questo caso l'importo specificato per la spesa di
  trasporto sarà considerato **iva compresa**. In conseguenza di ciò se
  ad effettuare l'ordine sul sito dovesse essere un privato (generando
  quindi un OX) l'importo della spesa di trasporto, presente nel
  riepilogo dell'ordine, coinciderà esattamente con quello definito in
  fase di configurazione del trasporto stesso.

> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo della spesa di
> trasporto, presente nel riepilogo dell'ordine, sarà quello definito in
> fase di configurazione del trasporto stesso scorporato dell'iva.
>
> Anche in questo caso l'aliquota utilizzata per il calcolo dell'Iva
> potrà variare in relazione al fatto di gestire le spese di trasporto
> mediante l'apposita voce presente nel piede del documento oppure
> mediante un articolo spesa che verrà inserito nel corpo del documento
> stesso, oltre ovviamente al fatto di gestire un' aliquota fissa o
> ripartita e al fatto di avere o meno la fatturazione elettronica
> abilitata (secondo la stessa logica indicata al punto precedente)

- **Iva Documento:** in questo caso l'importo specificato per la spesa
  di trasporto sarà considerato:

<!-- -->

- iva esclusa nel caso in cui venga generato un documento di tipo OC
  (verrà quindi applicata la stessa gestione del caso in cui Tipo Costo
  = Non Ivato)

- iva inclusa nel caso in cui venga generato un documento di tipo OX
  (verrà quindi applicata la stessa gestione del caso in cui Tipo Costo
  = Ivato)

**ATTENZIONE!!** per quel che riguarda gli importi indicati a fianco dei
singoli metodi di trasporto presenti, in checkout, nel relativo step

![](./assets/media/image276.png)

questi potranno essere ivati o non ivati (con la relativa etichetta)
dipendentemente da come è stato impostato il parametro "**Prezzo**"
presente alla pagina "**Configurazione Catalogo**" del Wizard. Il
consiglio, in questo senso è, ovviamente, quello di gestire questo
valore coerentemente con la tipologia di documento generata e quindi con
il valore che verrà poi indicato anche nel riepilogo dell'ordine.

**Articolo:** consente, se indicato, di gestire le spese di trasporto
mediante un articolo di tipo spesa che verrà poi inserito nel corpo del
documento.

Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca., la
scelta di gestire le spese di trasporto mediante un articolo di tipo
spesa oppure nella relativa voce presente nel piede del documento,
dipende essenzialmente da come il documento stesso dovrà poi essere
gestito all'interno del gestionale.

Nel caso in cui tutta la gestione rimanga all'interno del menu Magazzino
(es. Retail Configuratore) è possibile scegliere di gestire le spese di
trasporto tanto con l'articolo spesa quanto con la relativa voce
presente nel piede del documento.

Nel caso in cui invece la gestione del documento passi dalla cassa, sarà
necessario gestire le spese di trasporto mediante un articolo di tipo
Spesa.

**ATTENZIONE!** Per maggiori informazioni relativamente alla gestione,
sui siti Ho.Re.Ca., degli articoli di tipo spesa si veda anche la
sezione *"Configurazione gestionale -- Ho.Re.Ca. Parametri
Configurazione Gestionale -- Funzionalità di gestione articoli --
Articoli di tipo Spesa"* di questo manuale.

**Costo spedizione 0€**: consente di impostare, in ciascuna delle lingue
attualmente gestite all'interno del sito, un testo personalizzato che
verrà visualizzato in corrispondenza del relativo metodo di spedizione
nel momento in cui l'importo ad esso associato sia pari a 0.

Sia in fase di checkout che all'interno del modulo di preventivo delle
spese di spedizione presente in carrello, in corrispondenza del singolo
metodo di trasporto potrà quindi essere visualizzato:

- l'importo esatto della spesa di spedizione (determinato dai vari
  parametri di configurazione oltre che dalle specifiche condizioni
  d'ordine) nel momento in cui tale importo dovesse risultare maggiore
  di zero

- il testo inserito all'interno del campo in esame (es. "Gratuito") nel
  momento in cui l'importo associato alla spesa di spedizione dovesse
  risultare pari a zero

![](./assets/media/image277.png)

**ATTENZIONE!** Nel momento in cui il parametro in esame non dovesse
essere valorizzato in corrispondenza del singolo metodo di spedizione
verrà sempre visualizzato l'importo ad esso associato anche nel caso in
cui tale importo dovesse essere pari a 0

Una volta impostati tutti i parametri generali, sarà poi necessario
definire anche:

- il tipo di trasporto che dovrà essere utilizzato per il metodo di
  spedizione che si sta configurando -- sezione **Parametri del
  Trasporto**

- eventuali linee articoli o gruppi utente ad esso associati -- sezione
  **Linee Articolo** e **Gruppi**

- la specifica modalità di calcolo da applicare alla spesa di trasporto
  in questione in relazione anche alla zona geografica in cui dovrà
  essere poi spedita la merce -- sezione **Zone di spedizione**

