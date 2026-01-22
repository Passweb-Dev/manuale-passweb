# SCONTO ARTICOLO O PREZZO FISSO



Utilizzando questo tipo di promozione è possibile configurare, per gli
articoli coinvolti e indipendentemente da quello che è il particolare
listino ad essi associato:

- uno sconto in percentuale

- uno sconto a valore

- un prezzo fisso

- un prezzo come sconto.

E' possibile mettere in promozione singoli articoli (Tabella "**Articoli
in Promozione**") oppure intere categorie (Tabella **"Articoli
appartenenti alle categorie"**) definendo tanto per il singolo articolo,
quanto per l'intera Categoria lo sconto (a valore o in percentuale) o il
prezzo che dovrà poi essere applicato.

![](./assets/media/image534.png)

Il campo "**Tipo Sconto**" presente all'interno della scheda "**Opzioni
Sconto articolo**" permette, in questo senso, di definire come dovrà
effettivamente comportarsi la Promozione (**all'interno del gestionale e
anche sul sito**).

E' possibile selezionare uno dei seguenti valori:

- **Percentuale:** selezionando questa opzione ad ogni
  articolo/categoria di articoli coinvolti nella Promozione verrà
  applicata la percentuale di sconto indicata all'interno della relativa
  tabella

- **Valore:** selezionando questa opzione ad ogni articolo/categoria di
  articoli coinvolti nella Promozione verrà applicato lo sconto in
  valore indicato all'interno della relativa tabella

- **Prezzo:** selezionando questa opzione per ogni articolo/categoria di
  articoli coinvolti nella Promozione verrà utilizzato il prezzo
  indicato all'interno della relativa tabella indipendentemente da
  quello che è lo specifico listino associato all'articolo stesso.

- **Prezzo come sconto:** selezionando questa opzione per ogni
  articolo/categoria di articoli coinvolti nella Promozione verrà
  utilizzato il prezzo indicato all'interno della relativa tabella
  indipendentemente da quello che è lo specifico listino associato
  all'articolo stesso. In queste condizioni inoltre, sul front end del
  sito, verrà visualizzato anche uno sconto a valore pari alla
  differenza tra il prezzo di listino dell'articolo e quello impostato
  tramite la promozione

**ATTENZIONE!** nel caso in cui sia stato selezionato il parametro
"**Applica Sconto come prezzo**" (visibile solo nel caso in cui il
precedente parametro "Tipo Sconto" sia stato impostato sul valore
"Percentuale" o "Valore".), **tanto in fase di conto all'interno del
gestionale quanto sul sito, non verranno mai visualizzati eventuali
sconti dovuti all'applicazione della Promozione ma verrà visualizzato ed
utilizzato direttamente il prezzo degli articoli al netto di tali
sconti**.

**Inoltre i prezzi presenti all'interno del sito saranno arrotondati a 2
decimali** per cui potrebbe non esserci un'esatta corrispondenza con i
relativi totali di un documento analogo generato però a partire dal
gestionale.

![](./assets/media/image535.png)

Per maggiori informazioni relativamente alla configurazione, lato
gestionale, di questa particolare tipologia di promozione si rimanda
all'apposito manuale di prodotto.

Una volta codificata ed esportata, questo tipo di Promozione potrà poi
essere utilizzata all'interno del sito in due modi differenti,
dipendentemente dal fatto di aver valorizzato o meno il campo "**Applica
solo ai primi articoli**" (scheda "**Opzioni Sconto articolo**").

**[CASO A -- APPLICA SOLO AI PRIMI ARTICOLI 🡪 NON
VALORIZZATO]{.underline}**

![](./assets/media/image536.png)

In queste condizioni sarà possibile decidere, in fase di attivazione e
configurazione della Promozione all'interno del sito, come questa dovrà
effettivamente comportarsi.

Selezionando, all'interno della maschera "Lista delle Promozioni"
precedentemente esaminata, la Promozione in esame, e cliccando sul
pulsante **Modifica Promozione**
(![](./assets/media/image479.png) ) si avrà accesso alla maschera di
configurazione della Promozione stessa

![](./assets/media/image530.png)

all'interno della quale il campo:

**Attivo:** consente di attivare la Promozione e di poterla quindi
utilizzare all'interno del sito

**Gestione:** permette di stabilire come la Promozione in esame dovrà
essere applicata all'interno del sito. E' possibile selezionare una
delle seguenti opzioni:

- **Ho.Re.Ca.:** in queste condizioni la Promozione verrà applicata
  utilizzando esattamente le stesse logiche definite all'interno del
  gestionale.

> In particolare nel caso in cui

- L'articolo coinvolto nella Promozione sia gestito con **unità di
  misura = pz** e la **Promozione sia stata configurata per applicare
  degli sconti in percentuale o a valore**, tali sconti verranno
  applicati direttamente a livello di listino.

> In queste condizioni sarà quindi possibile visualizzare lo sconto
> dovuto alla promozione tanto in Catalogo quanto nella relativa scheda
> prodotto.

![](./assets/media/image537.png)

- L'articolo coinvolto nella Promozione sia gestito con **unità di
  misura diversa da pz** e la **Promozione sia stata configurata per
  applicare degli sconti in percentuale**, tali sconti verranno
  applicati direttamente a livello di listino.

> Come nel caso precedente, anche in queste condizioni sarà quindi
> possibile visualizzare lo sconto dovuto alla promozione tanto in
> Catalogo quanto nella relativa scheda prodotto.

- L'articolo coinvolto nella Promozione sia gestito con **unità di
  misura diversa da pz** e la **Promozione sia stata configurata per
  applicare degli sconti a valore,** tali sconti verranno applicati in
  Carrello mediante l'inserimento di un apposito **Abbuono**

![](./assets/media/image538.png)

> A differenza dei casi precedenti, in queste condizioni non sarà quindi
> possibile visualizzare lo sconto dovuto alla promozione ne in Catalogo
> ne tanto meno all'interno della relativa scheda prodotto.
>
> L'Abbuono dovuto all'applicazione di queste promozioni verrà infatti
> visualizzato soltanto in Carrello oltre che, ovviamente, in fase di
> Checkout ordine.

- Nel caso in cui la **Promozione sia stata configurata per applicare
  dei Prezzi fissi,** indipendentemente dal fatto di considerare
  articoli con unità di misura uguale o diversa da pz, i prezzi
  impostati all'interno della Promozione verranno visualizzati ed
  utilizzati allo stesso modo anche all'interno del sito, tanto in
  Catalogo quanto nelle relative schede prodotto.

> In queste condizioni, dunque, non verranno visualizzati sconti di
> alcun tipo ne tanto meno verranno utilizzati degli Abbuoni (la
> promozione agisce infatti direttamente sul prezzo degli articoli)

- **Listino:** selezionando questa opzione il Prezzo e/o lo Sconto (in
  percentuale o a valore) dovuti all'applicazione di questa promozione
  verranno applicati **sempre e comunque a livello di listino,
  indipendentemente dal fatto di considerare articoli con unità di
  misura uguale o diversa da pz.**

> In queste condizioni sarà quindi possibile visualizzare eventuali
> sconti dovuti alla promozione tanto in Catalogo quanto nella relativa
> scheda prodotto.

**[CASO B -- APPLICA SOLO AI PRIMI ARTICOLI 🡪 VALORIZZATO]{.underline}**

![](./assets/media/image539.png)

In queste condizioni eventuali sconti dovuti alla Promozione verranno
applicati **sempre e comunque a livello di Carrello mediante
l'inserimento di un relativo Abbuono.**

![](./assets/media/image540.png)

Selezionando, all'interno della maschera "Lista delle Promozioni"
precedentemente esaminata, la Promozione in esame, e cliccando sul
pulsante **Modifica Promozione**
(![](./assets/media/image479.png) ) si avrà sempre accesso alla maschera di
configurazione della Promozione stessa dove, questa volta però, non sarà
più possibile decidere come questa dovrà comportarsi all'interno del
sito ma solamente se attivarla o meno (parametro "**Attivo**").

In relazione a questa particolare configurazione della Promozione va
sottolineato inoltre che questa verrà effettivamente applicata solo ai
primi N articoli presenti in ordine che rientrano, ovviamente, nella
promozione dove, il numero N indicato all'interno del campo "**Applica
solo ai primi Articoli**", verrà valutato in maniera diversa a seconda
del fatto che l'articolo abbia un'unità di misura uguale o diversa da
pz.

In particolare:

- **Nel caso in cui l'articolo in ordine sia gestito con unità di misura
  uguale a pz**, verrà considerata **la quantità in ordine** di quello
  stesso articolo

- **Nel caso in cui l'articolo in ordine sia gestito con unità di misura
  diversa da pz**, verrà considerato **l'articolo in ordine**
  **indipendentemente dalla quantità acquistata**.

**[ESEMPIO]{.underline}**

Supponiamo di aver impostato, all'interno del gestionale, il campo
"**Applica solo ai primi Articoli**" sul valore **4** e di aver inserito
in carrello i seguenti articoli:

- ARTICOLO 1 -- Unità di misura pz -- Quantità in ordine = 2

- ARTICOLO 2 -- Unità di misura diversa da pz -- Quantità in ordine = 2

- ARTICOLO 3 -- Unità di misura diversa da pz -- Quantità in ordine = 1

- ARTICOLO 4 -- Unità di misura diversa da pz -- Quantità in ordine = 4

- ARTICOLO 5 -- Unità di misura pz -- Quantità in ordine = 3

Supponiamo inoltre che la Promozione in oggetto possa essere applicata
solo ai seguenti articoli: ARTICOLO 1, ARTICOLO 2, ARTICOLO 4 e ARTICOLO
5

Per capire a quanti e a quali degli articoli in ordine verrà
effettivamente applicata la Promozione in esame, occorre capire,
innanzitutto, in che modo ciascuno di essi concorre al raggiungimento
del valore precedentemente impostato all'interno del campo "**Applica
solo ai primi Articoli**".

In questo senso, per il primo articolo (ARTICOLO 1), essendo esso
gestito con unità di misura uguale a pz, verrà considerata la sua
quantità in ordine e, pertanto, esso avrà un'incidenza pari a 2.

Per quel che riguarda invece il secondo articolo, essendo esso gestito
con unità di misura diversa da pz, verrà considerata la sola presenza
dell'articolo in ordine, indipendentemente da quella che possa poi
essere la quantità acquistata. In queste condizioni dunque l'incidenza
dell' "ARTICOLO 2" sarà pari a 1.

Il terzo articolo (ARTICOLO 3) in ordine non è coinvolto nella
Promozione, non verrà quindi valutato e non avrà alcuna incidenza nel
raggiungimento del valore N=4

Infine per le stesse ragioni appena evidenziate, gli ultimi due articoli
in ordine (entrambi coinvolti nella Promozione) avranno rispettivamente
un'incidenza pari a 1 e a 3.

**In queste condizioni la Promozione verrà quindi applicata solo ed
esclusivamente ai seguenti articoli: ARTICOLO 1 (incidenza 2), ARTICOLO
2 (incidenza 1) ARTICOLO 4 (incidenza 1) 🡪 N=2+1+1=4.**

Lato gestionale, infine, nel momento in cui si andrà a caricare, in
cassa, l'ordine nato all'interno del sito web si avrà che:

- eventuali **sconti sui singoli articoli** dovuti all'applicazione
  della promozione verranno riportati **all'interno delle relative righe
  articolo**.

![](./assets/media/image541.png)

- eventuali sconti, dovuti alla promozione e **applicati sul sito a
  livello di Carrello** mediante **Abbuoni,** verranno riportati
  all'interno del campo **Sconto**

![](./assets/media/image542.png)

**ATTENZIONE!** Le Promozioni di tipo **Sconto Articolo / Prezzo Fisso**
non sono considerate tra l'elenco delle Promozioni da poter escludere
nel caso di applicazione di eventuali Buoni Sconto.

Ciò significa dunque che nel momento in cui un dato utente dovesse
trovarsi applicata questo tipo di promozione, e fosse anche in possesso
di un Codice Sconto ancora valido, potrebbe tranquillamente utilizzarlo
usufruendo quindi di un ulteriore sconto oltre a quello previsto dalla
Promozione.

Per maggiori informazioni sull'utilizzo dei Buoni Sconto e sulla
possibilità di escludere determinate promozioni all'applicazione dei
Buoni Sconto si veda anche il capitolo "*Ordini -- Configurazione
Promozioni -- Buoni Sconto*" di questo manuale.

