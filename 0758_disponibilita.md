# DISPONIBILITA'



La sezione "**Disponibilità**", presente all'interno della maschera
"**Configurazione Catalogo Mexal / Ho.Re.Ca.**" consente di impostare la
modalità di acquisto degli articoli in catalogo in relazione a quella
che è la loro attuale disponibilità all'interno di Passweb.

All'interno di questa sezione è inoltre possibile attivare il componente
"**Notifica Disponibilità**" e abilitare quindi il sistema di gestione
delle notifiche relative alla richiesta di disponibilità dei vari
prodotti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_catalogo_mexal_disponibilita.bmp](./assets/media/image20.png){width="5.980555555555555in"
height="3.545138888888889in"}

In particolare il campo:

**Disponibilità del magazzino:** consente di specificare il/i Magazzini
del gestionale che dovranno essere considerati nel calcolo dei valori
delle disponibilità che verranno poi memorizzate, per ogni singolo
articolo, nel database di Passweb. E' possibile selezionare uno dei
seguenti valori:

- **Magazzino dell'ordine:** selezionando questo valore nel calcolo
  della disponibilità verrà considerato solo ed esclusivamente il
  magazzino indicato all'interno del campo "**Magazzino**" presente
  nella maschera di "**Configurazione Ordini**" del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\disponibilita_mexal_magazzino_1.bmp](./assets/media/image21.png){width="5.772916666666666in"
height="3.50625in"}

- **Tutti i Magazzini:** selezionando questo valore nel calcolo della
  disponibilità verranno considerati tutti i magazzini del gestionale
  attualmente gestiti.

- **Personalizzato:** selezionando questo valore verrà visualizzato
  l'elenco dei magazzini attualmente gestiti. A fianco di ciascun
  magazzino comparirà un apposito check di selezione. Il calcolo della
  disponibilità verrà quindi effettuato considerando l'insieme dei
  magazzini appositamente selezionati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\catalogo_mexal_disponibilita_personalizzata.bmp](./assets/media/image22.png){width="5.785416666666666in"
height="3.5256944444444445in"}

**Disponibilità:** consente di impostare, selezionandola tra le opzioni
disponibili, la specifica formula che dovrà essere utilizzata per il
calcolo delle disponibilità che verranno poi memorizzate, per ogni
singolo articolo, nel database di Passweb.

**ATTENZIONE!** Modificando le impostazioni dei parametri
"**Disponibilità** del magazzino" e "**Disponibilità**" verrà
automaticamente avviata la procedura di calcolo delle disponibilità dei
vari articoli. **Tale** **procedura non effettua un accesso al
gestionale per reperire le disponibilità in tempo reale ma rielabora
semplicemente, sulla base delle nuove impostazioni, i valori attualmente
presenti, per le disponibilità dei vari articoli, nel database di
Passweb**

**Scorta Minima:** consente di impostare il valore della scorta minima,
valore questo che verrà poi considerato, per il calcolo delle
disponibilità da memorizzare, per ogni singolo articolo, nel database di
Passweb.

E' possibile indicare un valore fisso (es. 10) oppure un valore in
percentuale (es. 10%). In quest'ultimo caso la percentuale indicata
verrà calcolata sul valore determinato in base alla formula impostata e
sarà, eventualmente, arrotondato per difetto.

Supponendo quindi di aver impostato come formula per il calcolo della
disponibilità l'Esistenza (Inventario + Carico -- Scarico) e come Scorta
minima il valore 10%, nel momento in cui per un determinato articolo
dovessimo avere dal gestionale un' Esistenza pari a 38 unità, il valore
della scorta minima arrotondato per difetto sarà esattamente di (38 x
10)/100 = 3 unità.

In queste condizioni dunque l'effettiva disponibilità, su Passweb,
dell'articolo in esame sarà esattamente di 38-3=35 unità

**ATTENZIONE!** Nel caso in cui la Scorta Minima sia impostata a 0 il
valore della disponibilità calcolata e memorizzata, per ogni singolo
articolo, all'interno di Passweb coinciderà, ovviamente, con il valore
della disponibilità calcolata in quello stesso momento all'interno del
gestionale.

**Nel momento in cui la "Scorta Minima" fosse impostata invece su di un
valore diverso da 0,** il valore effettivo della disponibilità
all'interno di Passweb sarà dato dalla differenza tra la disponibilità
gestionale e il valore della scorta minima.

**ATTENZIONE! La Scorta Minima indicata all'interno di questo campo si
intende definita per magazzino e per taglia**

Questo significa dunque che, nel momento in cui per il calcolo della
disponibilità dovessero essere considerati, ad esempio, due magazzini
(Mag1 e Mag2), supponendo di avere impostato una scorta minima di 2 per
l\'articolo X, si avrà una situazione di questo tipo

  ---------------------------------------------------------------------
  **MAGAZZINO**   **DISPONIBILITA'**   **DISPONIBILITA' EFFETIVA
                                       (DISPONIBILITA' -- SCORTA
                                       MINIMA)**
  --------------- -------------------- --------------------------------
  Mag1            10                   8

  Mag2            6                    4
  ---------------------------------------------------------------------

e la disponibilità risultante sarà quindi di 8 + 4 = 12 unità (contro
una disponibilità gestionale pari a 16).

Allo stesso modo se l\'articolo X fosse stato un articolo a taglie nelle
condizioni in tabella

+---------------+--------------------+--------------------------------+
| **MAGAZZINO** | **DISPONIBILITA'** | **DISPONIBILITA' EFFETIVA      |
|               |                    | (DISPONIBILITA' -- SCORTA      |
|               |                    | MINIMA)**                      |
+===============+====================+================================+
| Mag1          | T1 -- 3            | T1 -- 1                        |
|               |                    |                                |
|               | T2 - 5             | T2 -- 3                        |
+---------------+--------------------+--------------------------------+

si otterrebbe, lato Passweb, una disponibilità complessiva di 4 unità, 1
sulla taglia T1 e 3 sulla taglia T2 (contro una disponibilità gestionale
pari a 8 unità)

**ATTENZIONE! Il valore della scorta minima per gli articoli in Catalogo
può essere impostato anche articolo per articolo, agendo direttamente
dalla relativa Anagrafica Passweb mediante l'apposito parametro "Scorta
Minima"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scorta_minima_articolo.bmp](./assets/media/image23.png){width="5.785416666666666in"
height="3.33125in"}

Ovviamente i valori impostati sul singolo articolo avranno priorità
rispetto a quelli impostati a livello generale all'interno della sezione
"Configurazione Catalogo" del Wizard.

In questo senso è bene ricordare però che un'eventuale variazione del
parametro "Scorta Minima" presente all'interno della maschera
"Configurazione Catalogo" del Wizard, comporterà il ricalcolo e
l'aggiornamento delle scorte minime di tutti gli articoli gestiti sul
sito andando quindi a sovrascrivere eventuali impostazioni
precedentemente settate a livello di singolo prodotto.

**ATTENZIONE!** In generale nel valutare quella che per Passweb è la
quantità effettiva di un certo articolo su di un determinato magazzino,
occorre sempre tener conto di quanto impostato all'interno di questa
sezione del Wizard **in termini sia di formula utilizzata per il calcolo
della disponibilità che di Scorta Minima**

**Soglia Disponibilità:** consente di impostare un valore di soglia per
la disponibilità che potrà poi essere utilizzato in fase di definizione
degli scaglioni impostabili all'interno del componente "Disponibilità
Articolo". Tale valore deve necessariamente essere **un valore intero**
e può rivelarsi particolarmente utile nel momento in cui l'esigenza
dovesse essere quella di gestire degli scaglioni di disponibilità del
tipo:

- **Quantità articolo = 0** 🡪 Articolo non disponibile (pallino rosso)

- **Quantità articolo maggiore di 0 e minore del Valore di Soglia** 🡪
  Articolo a disponibilità bassa (pallino arancione)

- **Quantità articolo maggiore del Valore di Soglia** 🡪 Articolo a
  disponibilità elevata (pallino verde)

dove, ovviamente, il "Valore di Soglia" potrà essere un numero diverso
per i diversi prodotti gestiti all'interno del sito

**In questo senso una cosa di fondamentale importanza da tenere sempre
in considerazione è che il Valore di Soglia impostato all'interno di
questo campo verrà utilizzato esclusivamente come valore di default per
tutti i nuovi articoli importati all'interno del sito.**

Nel momento in cui l'esigenza dovesse essere quindi quella di impostare
un Valore di Soglia per articoli già gestiti all'interno del sito sarà
necessario agire direttamente dall'omonimo campo presente
nell'anagrafica Passweb del singolo prodotto, oppure in maniera massiva
mediante importazione via csv (per maggiori informazioni in merito si
veda anche quanto indicato nei relativi capitoli di questo manuale
*"Catalogo -- Gestione Articoli -- Articoli - Anagrafica Articolo /
Servizio"* e "*Catalogo -- Gestione Articoli -- Articoli - Anagrafica
Articolo / Servizio -- Importazione / Esportazione dei dati articolo
tramite file"*)

Sulla base di quanto appena detto è semplice comprendere anche che
eventuali modifiche apportate al valore impostato all'interno del campo
in esame verranno applicate solo ai nuovi articoli e non si
rifletteranno in alcun modo sui prodotti già presenti all'interno del
sito.

**ATTENZIONE!** Una volta impostato il Valore di Soglia questo potrà poi
essere utilizzato in fase di definizione degli scaglioni di
disponibilità mediante il segnaposto **"x"**

Supponendo dunque di aver impostato per due diversi prodotti "PROD01" e
"PROD02" un valore di soglia rispettivamente di 5 e 10 e che tali
prodotti siano presenti sul sito in quantità rispettivamente di 6 e 8
unità, andando poi ad impostare una disponibilità a fasce del tipo:

- Da 0 A 1 🡪 Disponibilità Bassa

- Da 1 a x 🡪 Disponibilità Media

- Da x in poi 🡪 Disponibilità Alta

nel momento in cui l'utente dovesse richiedere la disponibilità
dell'articolo "PROD01" otterrebbe come risultato una "Disponibilità
Alta" (la quantità 6 di tale prodotto ricade infatti nella fascia "Da x
in poi" essendo per questo prodotto x=5).

Nel momento in cui l'utente dovesse richiedere invece la disponibilità
dell'articolo "PROD02" otterrebbe come risultato una "Disponibilità
Media" (la quantità 8 di tale prodotto ricade infatti nella fascia "Da 1
a x" essendo per questo prodotto x=10).

**Gestione Acquisto:** consente di impostare quella che dovrà essere la
modalità di acquisto di default per gli articoli presenti in catalogo,
in relazione alla **loro attuale disponibilità all'interno del database
di Passweb**.

E' possibile selezionare uno dei seguenti valori:

- **Acquista sempre:** selezionando questa opzione sarà sempre possibile
  acquistare i vari articoli presenti in catalogo (a meno ovviamente di
  ulteriori specifiche limitazioni) indipendentemente, dunque, da quella
  che è la loro attuale disponibilità all'interno del database di
  Passweb.

- **Acquista solo se disponibile:** selezionando questa opzione sarà
  possibile acquistare i vari articoli presenti in catalogo solo ed
  esclusivamente nel caso in cui la loro attuale disponibilità
  (**calcolata al netto di un eventuale Scorta Minima**) sia maggiore di
  zero e comunque superiore alla quantità che l'utente desidera
  effettivamente acquistare.

> In particolare nel caso in cui la disponibilità memorizzata nel
> database di Passweb per un certo articolo **sia minore o uguale a 0**,
> verrà visualizzato per questo stesso articolo, al posto del pulsante
> "Aggiungi in Carrello", l'etichetta "**Articolo Esaurito**"
> (personalizzabile all'interno della sezione "Gestione Testi/Messaggi
> del sito") impedendone di fatto l'acquisto.
>
> **Nel caso di articoli a taglie (Ecommerce Mexal)**, qualora
> l'articolo risulti disponibile solo per determinate taglie, le taglie
> non disponibili non verranno mostrate nelle diverse possibili opzioni
> di selezione.
>
> **Per quel che riguarda invece gli articoli strutturati**, nel caso in
> cui per la corrispondente struttura sia stato impostato il parametro
> "Tipologia di Visualizzazione" sul valore "Vincolante al precedente
> livello", le opzioni di selezione relative a configurazioni di
> articoli figlio non disponibili verranno comunque visualizzate
> all'interno del configuratore di prodotto ma potranno essere
> stilizzate in maniera diversa dalle altre in modo tale da evidenziare
> chiaramente che quella specifica configurazione porterà ad ottenere un
> articolo al momento non disponibile e quindi non acquistabile.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\configuratore_articoli_non_disponibili_1.bmp](./assets/media/image24.png){width="5.227083333333334in"
height="3.50625in"}

> Per stilizzare in maniera diversa dalle altre le opzioni di selezione
> relative a configurazioni di articoli figlio non disponibili è
> sufficiente agire dallo style editor del componente "Configuratore"
> selezionando uno degli elementi evidenziati in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\configuratore_articoli_non_disponibili_2.bmp](./assets/media/image25.png){width="4.675in"
height="2.0972222222222223in"}

> Ovviamente gli articoli corrispondenti a configurazioni attualmente
> non disponibili non potranno essere acquistati per cui selezionando
> una configurazione di prodotto finito che contiene un'opzione non
> disponibile al posto del pulsante di Aggiunta in Carrello verrà
> visualizzata, anche in questo caso, l'etichetta di "Articolo
> Esaurito".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\configuratore_articoli_non_disponibili_3.bmp](./assets/media/image26.png){width="5.227083333333334in"
height="3.1104166666666666in"}

> **ATTENZIONE!** Il fatto di ammettere, in queste condizioni, anche la
> configurazione di articoli figli attualmente non disponibili potrebbe
> comunque rivelarsi utile nel momento in cui l'utente volesse, ad
> esempio, aggiungere quello specifico articolo in Wishlist o magari
> richiedere per esso la notifica mail nel momento in cui dovesse
> ritornare disponibile (cosa questa ovviamente non possibile
> escludendolo a priori dalle possibili opzioni di scelta presenti
> all'interno del configuratore)
>
> Infine nel caso in cui invece l'utente tenti di acquistare un articolo
> in quantità superiore a quella che è la sua attuale disponibilità
> all'interno di Passweb, l'articolo verrà effettivamente aggiunto in
> carrello ma **in quantità uguale a quella che è la sua attuale
> disponibilità** e l'utente verrà avvisato di ciò con un apposito
> messaggio (personalizzabile all'interno della sezione "Gestione
> Testi/Messaggi" del Wizard).
>
> **ATTENZIONE!** Impostando il parametro "**Gestione Acquisto**" sul
> valore "**Acquista solo se disponibile**", passando dalla pagina
> Carrello alla pagina Checkout sul front end del sito, verrà attivato
> un controllo per verificare le disponibilità attuali degli articoli
> presenti in carrello. Nel momento in cui per alcuni di essi la
> disponibilità Passweb dovesse essere minore o uguale a 0 o comunque
> inferiore alla quantità presente in carrello per lo specifico
> articolo, verrà visualizzato un apposito messaggio per notificare
> all'utente l'impossibilità di acquistare il relativo prodotto

**NOTA BENE:** le disponibilità dei vari articoli presenti all'interno
del database di Passweb e calcolate sulla base dei parametri appena
esaminati, **NON SONO DISPONIBILITA' AGGIORNATE IN TEMPO REALE**. I dati
utilizzati per il calcolo di questi valori vengono prelevati dal
gestionale e sono aggiornati all'ultima sincronizzazione utile.

**Eccezioni:** consente di impostare un'eventuale filtro articoli in
relazione al quale poter impostare una "Gestione dell' acquisto" diversa
da quella definita mediante il precedente parametro **"Gestione
Acquisto"**

In sostanza dunque, nel caso in cui il precedente parametro "Gestione
Acquisto" sia stato impostato sul valore "Acquista Sempre" gli articoli
che dovessero soddisfare il filtro impostato all'interno del campo
"Eccezioni" potranno essere acquistati solo se disponibili.

Allo stesso modo nel caso in cui il precedente parametro "Gestione
Acquisto" sia stato impostato sul valore "Acquista solo se disponibile"
gli articoli che dovessero soddisfare il filtro impostato all'interno
del campo "Eccezioni" potranno essere acquistati sempre,
indipendentemente da quella che è la loro attuale disponibilità
all'interno del database di Passweb.

**NOTA BENE:** per maggiori informazioni relativamente alla creazione di
un filtro articoli si veda anche la sezione "Utenti -- Gruppi Utenti
Sito -- Filtri Utenti e Filtri Articolo" di questo manuale.

**ATTENZIONE!** **La modalità di acquisto degli articoli in Catalogo può
essere impostata anche articolo per articolo, agendo direttamente dalla
relativa Anagrafica Passweb mediante l'apposito parametro "Gestione
Acquisto"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_acquisto.bmp](./assets/media/image27.png){width="5.804861111111111in"
height="3.33125in"}

**In questo senso però è bene sottolineare come in fase di
sincronizzazione verrà valutato, per ogni articolo coinvolto nella
sincronizzazione stessa, il filtro impostato all'interno del campo
"Eccezioni" e, nel caso in cui alcuni di essi dovessero soddisfare tale
filtro, verrà modificato di conseguenza il valore impostato, nella loro
Anagrafica Passweb, per il campo "Gestione Acquisto".**

In definitiva dunque, nel caso in cui si desideri impostare la Gestione
dell'Acquisto direttamente dall'Anagrafica Passweb di ogni singolo
articolo è consigliabile non impostare nessun filtro articoli
all'interno del campo "Eccezioni" (evitando così di correre il rischio
che eventuali impostazioni settate per lo specifico articolo possano
essere sovrascritte alla sincronizzazione).

Allo stesso modo nel caso in cui si desideri impostare la Gestione
dell'Acquisto a livello generale, lavorando per questo con i parametri
"Gestione Acquisto" e "Eccezioni" presenti nella maschera
"Configurazione Catalogo Mexal / Ho.Re.Ca.", è consigliabile non andare
poi a variare le impostazioni agendo direttamente nell'Anagrafica
Passweb dello specifico articolo (creando cioè eccezioni alle
eccezioni).

**Gestione Disponibilità DBA**: consente di indicare come dovrà essere
calcolata la disponibilità degli articoli di tipo DBA presenti
all'interno del sito. E' possibile selezionare uno dei seguenti valori:

- **Gestisci la disponibilità della DBA** -- opzione di default: in
  queste condizioni la disponibilità di un articolo di tipo DBA verrà
  valutata prendendo in considerazione i progressivi dell'articolo
  stesso

- **Calcola la disponibilità della DBA sulla base delle disponibilità
  dei componenti**: selezionando questa opzione la disponibilità di un
  articolo di tipo DBA verrà valutata sulla base delle disponibilità dei
  singoli componenti della DBA stessa (esattamente allo stesso modo di
  quanto avviene per un articolo di tipo Campionario)

**ATTENZIONE! Il parametro in esame ha effetto a livello generale per
tutti gli articoli di tipo DBA gestiti all'interno del sito**

Nel momento in cui l'esigenza dovesse invece essere quella di modificare
la metodologia di calcolo della disponibilità di un singolo articolo di
tipo DBA sarà possibile agire dall'analogo parametro presente
nell'Anagrafica Passweb dell'articolo stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\anagrafica_passweb_disponibilita_DBA.bmp](./assets/media/image28.png){width="5.804861111111111in"
height="3.5256944444444445in"}

In ogni caso occorre sempre tenere in considerazione che un'eventuale
variazione del parametro "**Gestione Disponibilità DBA"** presente
all'interno della maschera "Configurazione Catalogo" del Wizard,
comporterà il ricalcolo e l'aggiornamento delle impostazioni dello
stesso campo per tutti gli articoli gestiti sul sito **andando quindi a
sovrascrivere eventuali impostazioni precedentemente settate a livello
di singolo prodotto**.

Inoltre nel momento in cui si dovesse gestire sul sito una disponibilità
sempre visualizzata con i valori aggiornati all'ultima sincronizzazione
e si dovesse decidere per qualche ragione di modificare il parametro in
questione (a livello generale o di singolo articolo) si consiglia sempre
di effettuare anche una nuova sincronizzazione in maniera tale da essere
certi che il valore della disponibilità visualizzato per l'articolo di
tipo DBA sia effettivamente coerente con il tipo di gestione per esso
adottata

A differenza degli articoli di tipo DBA la cui disponibilità può essere
valutata, come appena visto, ragionando sia sulle disponibilità dei
singoli componenti che sulle disponibilità dell'articolo DBA stesso
(ovviamente un'opzione è alternativa all'altra), per gli **articoli di
tipo Campionario** è invece possibile ragionare in un modo soltanto.

In questo senso infatti occorre considerare che in Mexal un articolo di
tipo Campionario è solo un contenitore logico di tanti singoli articoli
e sono proprio questi singoli articoli ad essere venduti per cui questa
particolare tipologia di prodotti non hanno, ovviamente, progressivi
propri e non potranno quindi avere neppure una specifica disponibilità.

**In considerazione di ciò per gli articoli Campionario verranno quindi
valutate le disponibilità dei singoli articoli componenti il Campionario
stesso (tenendo conto, per questo, anche di eventuali formule definite
sui singoli componenti del campionario).**

Supponendo dunque di avere a che fare con un articolo Campionario
composto da:

  ---------------------------------------------------------------------
     **COMPONENTE          **QUANTITA'**           **DISPONIBILITA'
     CAMPIONARIO**                                    PASSWEB**
  ------------------- ------------------------ ------------------------
      ARTICOLO 1                 2                        10

      ARTICOLO 2                 1                        3

      ARTICOLO 3                 1                        6
  ---------------------------------------------------------------------

e supponendo di aver impostato il parametro "Gestione Acquisto" sul
valore "Acquista solo se disponibile", il massimo numero di articoli di
questo tipo acquistabili all'interno del sito sarebbe 3.

Nel caso in cui si tentasse di acquistare questo articolo in quantità
maggiore o uguale a 4 infatti, ci si scontrerebbe con il fatto di dover
acquistare per l'articolo "ARTICOLO 2" una quantità superiore a quella
che è la sua effettiva disponibilità attualmente memorizzata nel
database di Passweb (3).

Per quel che riguarda invece **gli articoli a Taglie**, gestiti in Mexal
attraverso l'apposita tabella, verrà calcolata, tenendo conto di quanto
impostato per i parametri appena esaminati, e memorizzata nel database
di Passweb, la disponibilità di ogni singola taglia della serie cui
appartiene lo specifico articolo.

Infine, un'ultima cosa da tenere sempre in considerazione è che **in
caso di acquisto di un determinato articolo, il numero di elementi
acquistati verrà sottratto al valore della disponibilità memorizzata in
Passweb per quello stesso articolo, solo ed esclusivamente dopo
l'inserimento nel gestionale del relativo ordine.**

Dopo aver inserito l'ordine all'interno del gestionale l'applicazione
andrà dunque a rileggere dal gestionale stesso tutti i dati necessari
per ricalcolare la disponibilità degli articoli appena ordinati, secondo
la formula di calcolo selezionata all'interno di questa sezione del
Wizard, e andrà poi ad aggiornare quelli che sono i corrispondenti
valori presenti nel database di Passweb.

**NOTA BENE:** l'aggiornamento delle disponibilità memorizzate nel
database di Passweb a seguito dell'inserimento di un nuovo ordine
riguarda solo ed esclusivamente gli articoli presenti all'interno
dell'ordine stesso.

