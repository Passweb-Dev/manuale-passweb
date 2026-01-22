# IMPOSTAZIONI GENERALI



All'interno della sezione "**Impostazioni Generali**" è possibile
impostare i parametri di configurazione della carta regalo che si
desidera creare.

**ATTENZIONE!** I parametri presenti all'interno di questa sezione
possono variare in relazione alla specifica tipologia di Gift Card

In particolare il campo:

- **Nome**: consente di impostare il nome identificativo della Gift Card
  in esame, in maniera tale da poterla poi distinguere tra tutte le
  altre presenti in elenco

- **Formato Codice**: consente di impostare il template che dovrà essere
  utilizzato per la generazione automatica dei codici da associare alle
  varie Gift Card.

> Sono ammessi caratteri alfabetici maiuscoli, numerici, il trattino ( -
> ), l'underscore ( \_ ) e i seguenti segnaposto:

- **{L}**: in fase di generazione del codice verrà sostituito con una
  lettera maiuscola

- **{D}**: in fase di generazione del codice verrà sostituito con
  carattere numerico

> Supponendo quindi di impostare un template del tipo di quello qui di
> seguito indicato
>
> GFT-{L}{L}{L}-{D}{D}{D}-GFT
>
> i codici Gift Card generati in automatico dal programma potrebbero
> essere:
>
> GFT-SUY-857-GFT
>
> GFT-LOI-584-GFT
>
> GFT-KJH-123-GFT
>
> ...
>
> Per maggiori informazioni relativamente alla generazione dei codici da
> associare alle varie Gift Card gestite all'interno del sito si veda
> anche il successivo capitolo di questo manuale

- **Tipologia:** consente di impostare la Tipologia di Gift Card che si
  intende realizzare e, conseguentemente, anche il modo in cui essa
  verrà poi gestita all'interno del sito.

> E' possibile selezionare uno dei seguenti valori:

- **Fisica:** è la classica carta regalo su cui dovrà essere stampato il
  relativo codice di attivazione (quello per essa generato all'interno
  della sezione "*Gift Card -- Codici*" del Wizard).

> Una Gift Card di questo tipo è, a tutti gli effetti, un vero e proprio
> prodotto fisico per cui la sua gestione, dalla generazione del codice
> all' attivazione dovrà essere fatta in maniera manuale.
>
> Per la stessa ragione, ovviamente, la consegna della carta regalo
> all'acquirente avverrà mediante uno dei metodi di spedizioni gestiti
> all'interno del sito. Sarà poi cura dell'acquirente stesso consegnarla
> all'effettivo beneficiario come meglio crede.

- **Virtuale**: a differenza delle carte fisiche le Gift Card Virtuali
  non verranno considerate come dei veri e propri prodotti fisici per
  cui il loro processo di gestione e attivazione sarà fondamentalmente
  diverso da quello appena analizzato. Ciò non toglie ovviamente che per
  poter essere venduta sullo store online anche una Gift Card Virtuale
  dovrà comunque essere associata ad un normale articolo codificato
  all'interno del gestionale e correttamente gestito anche all'interno
  del sito

> Per maggiori informazioni relativamente alle procedure di gestione
> delle Gift Card Fisiche o Virtuali si veda anche quanto indicato nel
> precedente capitolo di questo manuale.

- **Ho.Re.Ca. -- disponibile solo per i siti Ecommerce collegati al
  gestionale Beauty**: questa particolare tipologia di Gift Card verrà
  utilizzata per gestire l'acquisto di Voucher (Buoni Regalo) che
  potranno poi essere spesi in fase di prenotazione / pagamento di uno o
  più trattamenti sia all'interno del sito che direttamente nel punto
  vendita.

> **E' possibile gestire solamente una Gift Card di tipo Ho.Re.Ca.** e,
> a differenza delle Gift Card di Fisiche o Virtuali, non sarà
> necessario associarla a determinati articoli operando direttamente dal
> Wizard di Passweb. Nel momento in cui per un sito collegato a Beauty
> dovesse, infatti, essere attivato **il modulo aggiuntivo delle Gift
> Card**, tutti gli articoli di tipo "**Trattamento**" e/o "**Ricarica
> promozione**", correttamente esportati e gestiti all'interno del sito,
> verranno considerati automaticamente come delle Gift Card di tipo
> Ho.Re.Ca.
>
> In conseguenza di ciò ogni singolo trattamento presente all'interno
> del sito potrà non solo essere prenotato ma anche acquistato sotto
> forma di Voucher (Buono Regalo), Voucher questo che potrà poi essere
> utilizzato in un momento successivo (e comunque coerente con il suo
> periodo di validità) per pagare quello stesso trattamento.
>
> Anche gli articoli di tipo "Ricarica Promozione" potranno essere
> acquistati come un qualsiasi altro prodotto presente all'interno del
> sito ma, a differenza dei Voucher generati dall'acquisto di uno
> specifico trattamento, il loro importo potrà essere utilizzato per
> pagare interamente o solo in parte uno qualsiasi dei trattamenti
> gestiti all'interno di Beauty.
>
> In ogni caso l'acquisto di un "Trattamento" o di un articolo di tipo
> "Ricarica promozione", se portato a termine, e quindi pagato, in
> maniera corretta porterà sempre alla creazione, in Beauty, di un
> corrispondente "Buono Sconto" il cui codice (generato anche sulla base
> delle impostazioni settate in fase di configurazione, su Passweb,
> della Gift Card di tipo Ho.Re.Ca.) sarà quello che l'utente dovrà poi
> effettivamente utilizzare all'interno del sito in fase di pagamento di
> un determinato trattamento.
>
> Per maggiori informazioni relativamente alle procedure di gestione
> delle Gift Card di tipo Ho.Re.Ca. si veda anche quanto indicato nel
> successivo capitolo (*'Gift Card Ho.Re.Ca.'*) di questo manuale

- **Articolo Utilizzo -- solo per Gift Card fisiche o Virtuali**:
  consente di impostare l'articolo spesa da inserire nel relativo
  documento gestionale nel momento in cui un utente in fase di acquisto
  dovesse decidere di utilizzare il saldo di eventuali Gift Card da lui
  riscattate.

> **Generalmente, l'articolo spesa utilizzato per gestire la Gift Card
> sul documento dovrebbe essere iva esente**.
>
> Se poi per determinate ragioni si volesse comunque gestire l'iva su
> questo particolare articolo è necessario ricordare che:

- non dovrà mai essere utilizzata un'iva ripartita

- nel caso in cui il saldo della Gift Card venga applicato al Totale
  dell'ordine dovrà necessariamente essere utilizzato un articolo spesa
  iva esente

> In caso contrario i totali del documento gestionale potrebbero non
> coincidere con quelli del corrispondente ordine web.

- **Applicazione Utilizzo -- solo per Gift Card fisiche o Virtuali**:
  consente di decidere a cosa dovrà essere applicato il saldo della Gift
  Card. E' possibile selezionare una delle seguenti opzioni.

  - **Articoli**: selezionando questa opzione il saldo della Gift Card
    verrà applicato al (e contribuirà quindi ad abbattere e/o azzerare
    il) totale merce ivato **dei soli articoli che soddisfano le
    condizioni di applicabilità della Gift Card in esame** In queste
    condizioni non verranno quindi abbattuti importi relativi a
    eventuali costi aggiuntivi sulle spedizioni e/o sui pagamenti.

> **ATTENZIONE!** Impostando il parametro "Applicazione Utilizzo" sul
> valore "Articoli" le condizioni di applicabilità della Gift Card
> determineranno esattamente gli articoli per i quali la Gift Card può e
> non può essere utilizzata andando quindi a definire esattamente
> l'importo complessivo da poter abbattere con l'uso della carta regalo

- **Merce**: selezionando questa opzione il saldo della Gift Card verrà
  sempre applicato al (e contribuirà quindi ad abbattere e/o azzerare
  il) totale merce ivato dell'intero documento.

> Anche in questo caso non verranno quindi abbattuti importi relativi a
> eventuali costi aggiuntivi sulle spedizioni e/o sui pagamenti.
>
> **ATTENZIONE!** Impostando il parametro "Applicazione Utilizzo" sul
> valore "Merce" le condizioni di applicabilità della Gift Card non
> verranno considerate per determinare l'importo complessivo da poter
> abbattere **che sarà sempre e comunque il totale merce ivato
> dell'intero documento**. In questo caso quindi, le condizioni di
> applicabilità della Gift Card vengono valutate solo ed esclusivamente
> per capire se la carta regalo può o non può essere applicata
> all'intero totale merce
>
> Per comprendere meglio supponiamo di avere in ordine un articolo A con
> totale riga (ivato) pari a 10€ e un articolo B con totale riga (ivato)
> pari a 20€.
>
> Supponiamo anche di aver impostato una condizione di applicabilità
> della Gift Card che sarà soddisfatta solo se in carrello è presente
> esattamente l'articolo A.
>
> In queste condizioni la Gift Card verrà correttamente applicata perché
> in carrello è effettivamente presente l' articolo A e l' applicazione
> sarà sull\'intero totale merce ivato, cioè 30€.
>
> Se, nelle stesse condizioni, il parametro "Applicazione Utilizzo"
> fosse stato impostato invece sul valore "Articoli" la Gift Card
> avrebbe comunque potuto essere applicata ma l'importo da poter
> abbatter in questo caso sarebbe stato il solo totale di riga relativo
> all'articolo A ossia 10€.

- **Ordine**: selezionando questa opzione il saldo della Gift Card verrà
  applicato al (e contribuirà quindi ad abbattere e/o azzerare il)
  Totale Ordine comprensivo di eventuali spese di trasporto e di
  eventuali spese aggiuntive ad eccezione di quelle relative ai
  pagamenti (che non potranno quindi essere abbattute dal saldo della
  Gift Card)

> **ATTENZIONE!** Nel momento in cui il parametro "Applicazione
> Utilizzo" dovesse essere impostato sul valore "Ordine" l'articolo
> spesa utilizzato per gestire la Gift Card **dovrà necessariamente
> essere iva esente**. In caso contrario, come precedentemente
> evidenziato i totali documento all'interno del gestionale potrebbero
> non coincidere con quelli del corrispondente ordine web.

- **Durata (giorni) -- solo per Gift Card Virtuali o di tipo Ho.Re.Ca**.
  Consente di impostare il numero di giorni, a partire dalla data di
  attivazione (determinata dalla data di esportazione sul sito della
  relativa fattura / corrispettivo di acquisto), entro i quali la Gift
  Card potrà essere riscattata ed utilizzata.

> **ATTENZIONE**! nel caso di Gift Card Fisiche generalmente i codici ad
> esse associati vengono già attivati prima ancora di stamparli sulla
> singola carta regalo (in maniera tale da evitare che l'amministratore
> del sito debba fare manualmente questa attivazione ogni volta che
> riceve un ordine di acquisto della Gift Card).
>
> In queste condizioni non è quindi possibile impostare un numero di
> giorni di scadenza perché si correrebbe il rischio di vendere una Gift
> Card Fisica con codici già scaduti.
>
> Come indicato nei successivi capitoli di questo manuale, è comunque
> possibile assegnare una scadenza anche alla Gift Card Fisiche
> lavorando sul parametro "**Data di scadenza**" presente nella maschera
> di configurazione dei singoli codici associati alla carta fisica

- **Notifica scadenza (giorni) -- solo per Gift Card fisiche o
  Virtuali**: consente di definire a quanti giorni dalla data di
  scadenza della Gift Card dovrà essere inviata la mail di "Notifica
  Scadenza".

> Nel caso in cui il campo dovesse essere impostato sul valore 0, la
> mail di notifica verrà inviata il giorno stesso della scadenza
>
> **ATTENZIONE!** Affinchè la mail di "Notifica Scadenza" possa essere
> inviata correttamente non è sufficiente settare il parametro in esame
> ma occorre anche configurare correttamente la relativa mail
> impostandone il testo e soprattutto l'oggetto ( che determina
> l'effettiva attivazione della mail)

La sezione "**Condizioni**" (disponibile solo per **Gift Card fisiche o
Virtuali )** consente invece di definire le condizioni di applicabilità
della Gift Card in esame.

**ATTENZIONE!** prima di poter definire le condizioni di applicabilità
di una Gift Card è necessario effettuare almeno un salvataggio dei
parametri di configurazione.

Una volta salvata la Gift Card si attiverà infatti, come mostrato in
figura, un nuovo pulsante mediante il quale poter gestire, attraverso
l'apposita maschera, l'inserimento di una nuova condizione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_condizione_giftcard.bmp](./assets/media/image304.png){width="5.636111111111111in"
height="3.3048611111111112in"}

Per ogni condizione è possibile impostare un valore per i seguenti
parametri:

**Nome:** nome identificativo della condizione che si sta impostando

**Filtro Articoli:** consente di impostare un determinato filtro
articoli. Per maggiori informazioni in merito alla creazione di un
filtro articoli si veda anche la sezione "*Utenti -- Gruppi Utenti Sito
-- Filtri Utente e Filtri Articolo -- Filtri Articolo*" di questo
manuale.

Impostando, sulla condizione in esame, un filtro articoli il saldo della
relativa Gift Card potrà essere utilizzato solo nel caso in cui tra gli
articoli in ordine **ce** **ne sia almeno uno che soddisfi tale
filtro**.

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

> In questo caso dunque, la condizione di applicabilità della Gift Card
> verrà validata, se l'articolo Campionario in sé dovesse effettivamente
> soddisfare il filtro impostato, indipendentemente dal fatto che i suoi
> componenti possano poi soddisfare o meno lo stesso filtro

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, la condizione di applicabilità della Gift Card
> verrà eventualmente validata prendendo in considerazione i componenti
> del Campionario ma non l'articolo Campionario in sé che, quindi,
> potrebbe anche non soddisfare il filtro impostato
>
> Il fatto poi di utilizzare il saldo della Gift Card solo per gli
> stessi articoli definiti dalla condizione piuttosto che per tutto il
> totale merce / ordine dipenderà da come è stato settato il parametro
> "Applicazione Utilizzo"

**Filtro Carrello:** consente di impostare un filtro sulla quantità /
numero di articoli presenti in carrello e/o sulla base del fatto che gli
articoli in carrello abbiano o meno uno sconto già applicato.

Di base quindi lavorando sul "Filtro Carrello" sarà possibile:

- decidere se la Gift Card dovrà essere applicata solo nel momento in
  cui tutte le righe articolo presenti in carrello dovessero soddisfare
  un eventuale "Filtro Articoli" o anche se solo una certa percentuale
  di esse dovesse essere effettivamente sufficiente per fare scattare la
  promozione.

- decidere se la condizione di applicabilità della Gift Card dovrà
  essere validata considerando tutti gli articoli presenti in carrello
  che soddisfano un eventuale "Filtro Articoli", oppure solo quelli che,
  oltre a soddisfare un eventuale "Filtro Articoli", risultino anche
  privi di eventuali altri sconti già applicati.

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_condizione_gc.bmp](./assets/media/image305.png){width="5.7340277777777775in"
height="3.2270833333333333in"}

- **Quantità in carrello:** permette di definire una condizione sulla
  **quantità complessiva di articoli presenti in carrello**. Supponendo
  quindi di impostare un filtro del tipo "Quantità in carrello maggiore
  di 5" la Gift Card in esame, con il relativo saldo, potrà essere
  utilizzata solo ed esclusivamente nel caso in cui la quantità
  complessiva di articoli in carrello dovesse essere maggiore di 5. Tale
  condizione potrebbe quindi essere soddisfatta inserendo in carrello un
  solo articolo in quantità 6 o, ad esempio, due distinti articoli
  ciascuno in quantità 3.

- **Elementi in carrello**: permette di definire una condizione sul
  numero complessivo di articoli presenti in carrello. Supponendo quindi
  di impostare un filtro del tipo "Elementi in Carrello maggiore di 2"
  la Gift Card in esame potrà essere utilizzata solo ed esclusivamente
  nel caso in cui siano stati inseriti in carrello almeno 3 distinti
  articoli indipendentemente dalla quantità acquistata per ognuno di
  essi.

> **ATTENZIONE!** **Nel caso in cui, sulla condizione in esame, sia
> stato impostato anche un Filtro Articoli, nella valutazione del filtro
> sulle quantità e/o sul numero di articoli presenti in carrello
> verranno considerati solo ed esclusivamente gli articoli che
> soddisfano il filtro impostato.**
>
> Di base dunque se dovessimo trovarci in una situazione mista in cui
> sono presenti in carrello sia prodotti che soddisfano un eventuale
> Filtro Articoli sia prodotti che non lo soddisfano, nel momento in cui
> quelli che lo soddisfano dovessero soddisfare anche eventuali
> condizioni impostate sulla quantità o sul numero di elementi, allora
> la Gift Card potrà essere utilizzata.
>
> Diversamente se l'esigenza dovesse essere quella di rendere la Gift
> Card non valida in una situazione mista, in cui ci ritroviamo in
> carrello prodotti che soddisfano il Filtro Articoli ma anche prodotti
> che non lo soddisfano, sarà necessario utilizzare allora per il Filtro
> Quantità l'opzione "Percentuale Elementi in Carrello"

- **Elementi distinti in Carrello**: stesso funzionamento della
  condizione "Elementi in carrello" con la particolarità però di
  considerare eventuali righe che fanno riferimento allo stesso articolo
  come un unico elemento in carrello.

> Supponendo dunque di impostare un filtro del tipo "Elementi distinti
> in carrello maggiore di 2" la Gift Card in esame potrà essere
> utilizzata solo nel caso in cui dovessero essere presenti in carrello
> almeno 3 righe di articoli questa volta **tutti diversi tra loro.**

- **Percentuale Elementi in Carrello**: permette di indicare la
  percentuale di articoli presenti in carrello che dovranno soddisfare
  un eventuale condizione di Filtro Articoli affinché la Gift Card in
  esame possa effettivamente essere utilizzata.

> Nel momento in cui l'esigenza dovesse essere dunque quella di bloccare
> l'utilizzo della Gift Card in una situazione mista e applicarla solo
> ed esclusivamente nel caso in cui tutti gli articoli presenti in
> carrello dovessero soddisfare un'eventuale condizioni di Filtro
> Articoli, sarà allora necessario impostare un Filtro Carrello del tipo
> "**Percentuale elementi in carrello = 100**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gc_percentuale_articoli.bmp](./assets/media/image306.png){width="4.538888888888889in"
height="2.5131944444444443in"}

> In queste condizioni se dovessimo avere in carrello anche un solo
> articolo che non soddisfa la condizione impostata all'interno del
> campo "Filtro Articoli" la Gift Card, indipendentemente da tutto il
> resto, non potrà essere utilizzata.
>
> Allo stesso modo se l'esigenza dovesse essere quella di poter
> utilizzare la Gift Card quando almeno il 50% delle righe articolo
> presenti in carrello dovesse soddisfare la condizione di Filtro
> Articoli, sarà allora necessario impostare un Filtro Carrello del tipo
> "**Percentuale elementi in carrello maggiore o uguale 50**"
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere impostato nessun
> Filtro Articoli la "Percentuale elementi in carrello" sarà ovviamente
> sempre uguale a 100

- **Percentuale Quantità in Carrello**: permette di indicare quanti
  articoli in percentuale, rispetto alla quantità totale di prodotti
  presenti in carrello, dovranno soddisfare un eventuale condizione di
  Filtro Articoli, affinché la Gift Card possa effettivamente essere
  utilizzata

> Supponendo dunque che l'esigenza sia quella di dover utilizzare la
> Gift Card solo nel momento in cui almeno il 30% della quantità
> complessiva di articoli presenti in carrello appartenga alla categoria
> 24 ("Outlet Uomo"), dovremmo configurare una condizione di
> applicabilità del tipo di quella rappresentata in figura
>
> ![Videate\\gc_percentuale_quantita.bmp](./assets/media/image307.png){width="3.285416666666667in"
> height="1.9868055555555555in"}
>
> In questo modo infatti se dovessimo trovarci ad avere in carrello una
> quantità complessiva di 5 prodotti di cui 4 (quindi 80% del totale)
> appartenenti ad una categoria diversa dalla 24 ed uno solo (quindi il
> 20% del totale) appartenente alla categoria 24, la condizione
> impostata non risulterebbe soddisfatta e la Gift Card, di conseguenza,
> non potrebbe essere utilizzata
>
> Se invece, in queste stesse condizioni, dovessimo trovarci ad avere in
> carrello una quantità complessiva di 6 prodotti di cui sempre 4 (ossia
> il 67% del totale) appartenenti ad una categoria diversa dalla 24 e i
> restanti 2 (quindi il 33% del totale) appartenenti invece alla
> categoria 24, la condizione impostata sarebbe verificata e, di
> conseguenza, la Gift Card potrebbe essere utilizzata

- **Quantità in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verrà valutata la quantità di riga per ogni
  singolo prodotto che soddisfa l'eventuale filtro impostato. Supponendo
  dunque di considerare una configurazione del tipo di quella
  rappresentata in figura

![Videate\\nuova_condizione_gc_3.bmp](./assets/media/image308.png){width="4.2340277777777775in"
height="2.5909722222222222in"}

> la Gift Card potrà essere utilizzata solo nel momento in cui in
> carrello dovessimo avere almeno un articolo il cui codice inizia con
> AGLIANIC e la sua quantità di riga dovesse essere maggiore o uguale a
> 2
>
> Nelle condizioni indicate con i seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   1

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> la Gift Card non potrà essere utilizzata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due e nessuno di
> essi ha in riga una quantità maggiore o uguale a 2
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> la Gift Card potrà essere utilizzata perché uno dei due prodotti che
> soddisfano il filtro articoli impostato (AGLIANICVULDON99) ha
> effettivamente una quantità di riga uguale a 2

- **Quantità Massima in Riga:** permette di definire una condizione
  sulla quantità di articoli presenti nelle singole righe del carrello.
  Nello specifico, in questo caso, verranno valutati tutti i prodotti
  che soddisfano l'eventuale filtro impostato e tra questi verrà preso
  in considerazione solo quello con la quantità in riga più alta. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata la Gift Card potrà essere utilizzata altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\nuova_condizione_gc_4.bmp](./assets/media/image309.png){width="4.175in"
height="2.6104166666666666in"}

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Gift Card non potrà essere utilizzata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il primo ma tale quantità
> (2) non soddisfa comunque la condizione impostata (maggiore o uguale a
> 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   4

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Gift Card potrà essere utilizzata perché i prodotti che soddisfano
> il filtro articoli impostato sono i primi due; tra questi quello con
> la quantità in riga più alta è il secondo (AGLIANICVULROI01) e tale
> quantità (4) soddisfa correttamente la condizione impostata (maggiore
> o uguale a 3)

- **Quantità Minima in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verranno valutati tutti i prodotti che
  soddisfano l'eventuale filtro impostato e tra questi verrà preso in
  considerazione solo quello con la quantità in riga più bassa. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata Gift Card potrà essere utilizzata altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\nuova_condizione_gc_5.bmp](./assets/media/image310.png){width="4.220833333333333in"
height="2.6104166666666666in"}

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Gift Card non potrà essere utilizzta perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il primo (AGLIANICVULDON99)
> ma tale quantità (1) non soddisfa comunque la condizione impostata
> (maggiore o uguale a 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   3

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Gift Card potrà essere utilizzata perché i prodotti che soddisfano
> il filtro articoli impostato sono i primi due; tra questi quello con
> la quantità in riga più bassa è il secondo (AGLIANICVULROI01) e tale
> quantità (3) soddisfa correttamente la condizione impostata (maggiore
> o uguale a 3)

- **Sconto in Riga**: permette di definire una condizione di
  applicabilità della Gift Card che tenga conto di tutti gli articoli
  presenti in carrello che soddisfano un eventuale "Filtro Articoli", o
  solo di quelli che, oltre a soddisfare un eventuale "Filtro Articoli",
  risultino anche privi di eventuali altri sconti già applicati.

> **ATTENZIONE! l'opzione "Sconto in Riga" è di tipo Stringa**
>
> In conseguenza di ciò per creare una condizione che verrà validata
> solo nel caso in cui i prodotti in carrello che soddisfano un
> eventuale "Filtro Articoli" risultino essere anche privi di altri
> sconti già applicati, **il campo "Valore" della condizione "Sconto in
> Riga" dovrà essere lasciato vuoto (**Valore = Stringa vuota).
>
> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gc_sconto_in_riga.bmp](./assets/media/image311.png){width="3.3048611111111112in"
height="2.1881944444444446in"}

> la condizione in esame verrà validata e la relativa Gift Card potrà
> essere applicata solo nel caso in cui tutti gli articoli presenti in
> carrello (**Percentuale Elementi in Carrello = 100**) appartengano
> alla categoria 24 e siano tutti privi di sconto (**Sconto in Riga =
> stringa vuota**)
>
> Al contrario, se anche tutti gli articoli presenti in carrello
> appartenessero effettivamente alla categoria 24 ma anche uno solo di
> essi avesse già uno sconto applicato (perché ad esempio importato dal
> gestionale) la condizione non verrebbe validata e, di conseguenza, la
> relativa Gift Card non potrebbe essere utilizzata.
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

Il parametro "**Gestione Condizioni**" permette, infine, di decidere se
la Gift Card in esame, con il relativo saldo, potrà essere utilizzata
solo ed esclusivamente nel momento in cui tutte le condizioni impostate
siano state soddisfatte oppure se è sufficiente che ne siano verificate
solamente un certo numero.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_condizione_gc_8.bmp](./assets/media/image312.png){width="5.616666666666666in"
height="3.298611111111111in"}

In particolare dunque impostando questo parametro sul valore:

- **Tutte le condizioni devono essere soddisfatte**: la Gift Card in
  esame, con il relativo saldo, potrà essere utilizzata solo ed
  esclusivamente nel momento in cui tutte le condizioni impostate siano
  state soddisfatte

- **Almeno X condizioni devono essere soddisfatte**: per poter
  utilizzare la Gift Card in esame, con il relativo saldo, è sufficiente
  è sufficiente che siano soddisfatte almeno X condizioni di quelle
  indicate, dove X sarà esattamente il numero specificato in
  corrispondenza del successivo campo "**Numero condizioni (X)**"

