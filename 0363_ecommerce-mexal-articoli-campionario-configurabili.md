# ECOMMERCE MEXAL -- ARTICOLI CAMPIONARIO CONFIGURABILI



Come evidenziato nel precedente capitolo di questo manuale, nel caso in
cui l'esigenza dovesse essere quella di gestire dei Box configurabili
dando quindi all'utente la possibilità di decidere, direttamente in fase
di acquisto all'interno del sito, come comporre il suo Box, scegliendo
tra una lista di articoli preconfigurata, quali andare effettivamente ad
inserire all'interno del Box, ed eventualmente in che quantità, e quali
no si dovrà ricorrere per forza di cose ad un **Campionario
Configurabile**.

Per gestire questo tipo di articoli sarà quindi necessario, per prima
cosa, rendere configurabile il Campionario definito all'interno del
gestionale e impostare i limiti entro i quali l'utente potrà poi
muoversi in fase di composizione del suo Box.

In questo senso dovremo quindi agire dalla sezione "**Dati Articolo**"
(accessibile sul Wizard alla voce di menu "*Catalogo -- Gestione
Articoli*") selezionando il Campionario in esame, attivando il check
"**Abilita Configurazione**" (scheda "Box") e impostando le quantità
minime e massime tra cui l'utente potrà muoversi per ogni singolo
componente del Campionario.

![](./assets/media/image71.png)

**ATTENZIONE!** Per maggiori informazioni relativamente a come rendere
configurabile un articolo di tipo Campionario e come poter impostare per
ogni singolo componente le quantità minime e massime tra cui scegliere
si veda anche la sezione "*Catalogo -- Gestione Articoli -- Articoli --
Anagrafica Articolo/Servizio -- Anagrafica Passweb -- Box*" di questo
manuale

In queste condizioni il Componente **"Campionario E-commerce"** inserito
all'interno della Scheda Prodotto consentirà non solo di visualizzare
l'elenco dei singoli Componenti del Campionario (come avveniva per i
Campionari Semplici), ma offrirà all'utente anche la possibilità di
decidere come comporre il suo Box scegliendo quali articoli inserire, ed
eventualmente in che quantità, e quali no, il tutto ovviamente sempre
nei limiti impostati in fase di abilitazione del Campionario
Configurabile.

![](./assets/media/image72.png)

Per ogni singolo componente del Campionario potrà quindi essere
visualizzato:

- **Il configuratore di prodotto**, nel caso in cui il componente in
  questione fosse un articolo strutturato.

> Sarà ovviamente necessario aver inserito, in fase di creazione della
> scheda prodotto, all'interno del componente "Campionario Ecommerce"
> anche il relativo componente "Configuratore".
>
> **ATTENZIONE!** Nel caso in cui sia stata indicata, per l'articolo in
> questione, una quantità minima superiore a 0, sarà ovviamente
> necessario che l'utente configuri l'articolo prima di poter
> effettivamente inserire l'intero box in carrello.

- **Un campo di input con relativi pulsanti incrementali (+/-)**
  mediante il quale l'utente potrà impostare, per ogni singolo
  componente del campionario la quantità con cui quello stesso articolo
  dovrà essere inserito nel Box.

![](./assets/media/image73.png)

> **ATTENZIONE!** Per visualizzare tale campo sarà necessario inserire,
> in fase di creazione della scheda prodotto, all'interno del componente
> "Campionario Ecommerce" anche il componente "**Aggiungi in Carrello**"
>
> Nel caso in cui l'articolo in esame fosse un articolo a Taglie /
> Colori verrà visualizzata la configurazione estesa delle taglie.

![](./assets/media/image74.png)

> Inoltre, dipendentemente dal fatto di aver selezionato o meno in fase
> di configurazione dello specifico componente il parametro "**Solo
> Taglie Indicate**", potranno essere visualizzate le sole taglie per le
> quali è stata effettivamente inserita, lato gestionale, una quantità
> o, in alternativa, tutte le taglie/colori gestite.

![](./assets/media/image75.png)

> Immediatamente al di sopra del campo di input verrà visualizzata anche
> un'etichetta (personalizzabile alla sezione "Testi / Messaggi" del
> Sito agendo sull'elemento "Range" del componente "Aggiungi al
> Carrello") con **l'indicazione delle quantità minima e massima
> impostabili per lo specifico componente.**

![](./assets/media/image76.png)

> Il valore minimo indicato coincide con quello impostato all'interno
> del campo "**Quantità Minima**" e definito, lato Passweb, in fase di
> abilitazione del singolo componente del Campionario

![](./assets/media/image77.png)

> **ATTENZIONE! Se l'esigenza dovesse essere quella di rendere un
> componente del Box non obbligatorio sarà sufficiente:**

- **selezionare per esso il parametro "Abilita Configurazione"**

- **impostare la sua "Quantità Minima" sul valore 0 (o al limite
  lasciare vuoto il campo)**

- **impostare il parametro "Predefinito" sul valore NO**

> In queste condizioni infatti il componente in oggetto verrà
> inizialmente visualizzato all'interno del box configurabile con
> quantità pari a 0 (indipendentemente da quella che è la quantità
> settata all'interno del gestionale in fase di configurazione del
> relativo Campionario) e l'utente, volendo, potrebbe anche decidere di
> non inserirlo all'interno del Box**.**
>
> **ATTENZIONE!** Per maggiori informazioni sui parametri "Quantità
> minima" e "Predefinito", si veda anche la sezione *Catalogo --
> Gestione Articoli -- Articoli - Anagrafica Articolo / Servizio --
> Anagrafica Passweb -- Box* di questo manuale
>
> Il valore massimo coincide invece con la quantità con cui il relativo
> articolo è stato inserito, lato gestionale, all'interno del
> Campionario

![](./assets/media/image78.png)

> Infine **nel caso in cui lo specifico componente del Campionario fosse
> stato impostato come "non configurabile" (parametro "Abilita
> Configurazione" non selezionato), il campo di input per l'impostazione
> delle quantità sarà disabilitato e non verranno visualizzati neppure i
> relativi pulsanti incrementali**

![](./assets/media/image79.png)

> In queste condizioni dunque l'utente non potrà apportare nessun tipo
> di variazione al componente che verrà quindi inserito nel Box così
> come stabilito all'interno del gestionale.

Oltre alle etichette con l'indicazione delle quantità minima e massima
impostabili per lo specifico componente, è possibile visualizzare,
immediatamente al di sotto del componente Campionario, anche un testo
riepilogativo con l'indicazione delle quantità minima e massima globali
effettivamente gestibili per l'intero Box.

![](./assets/media/image80.png)

In questo caso il numero minimo di elementi (inteso come quantità
complessive) che dovranno essere necessariamente presenti all'interno
del Box prima di poterlo inserire in carrello, coincide con il valore
impostato, lato Passweb, in corrispondenza del parametro "**Numero
Minimo Componenti**"

![](./assets/media/image81.png)

**ATTENZIONE! Il valore di questo parametro dovrà essere, ovviamente,
minore o uguale alla somma delle quantità minime dei singoli componenti
del Campionario**

Il numero massimo (intesto sempre come quantità complessive) di articoli
che potranno essere inseriti all'interno di un Box configurabile può
essere gestito in maniera diversa dipendentemente dal fatto di
considerare siti Ecommerce collegati a Mexal oppure ad uno dei
gestionali Ho.Re.Ca..

In particolare nel caso di **siti Ecommerce collegati ad uno dei
gestionali Ho.Re.Ca.** il valore in esame è impostato direttamente
all'interno del gestionale mediante il parametro "**N° massimo
complessivo**" presente nella scheda di configurazione del Composto che
si sta considerando

![](./assets/media/image82.png)

In questo caso inoltre il campo "**Numero massimo di componenti**"
presente nell'anagrafica Passweb dello specifico articolo sarà in sola
visualizzazione e non potrà quindi essere variato in alcun modo se non
agendo, come detto, all'interno del gestionale stesso.

Nel caso invece di **siti Ecommerce collegati a Mexal**, il numero
massimo di componenti potrà essere specificato direttamente
nell'Anagrafica Passweb dell'articolo mediante il campo in "**Numero
massimo di componenti**" indicato in figura.

![](./assets/media/image83.png)

**ATTENZIONE! Nel momento in cui questo campo non dovesse essere
valorizzato, il numero massimo di articoli che potranno essere inseriti
all'interno di un Box configurabile sarà dato dalla somma delle quantità
impostate per ogni singolo componente, direttamente su Mexal, in fase di
configurazione del relativo articolo Campionario.**

Nel momento in cui un utente dovesse apportare delle variazioni alle
quantità dei singoli componenti del Box:

- verranno avviati dei controlli per garantire che siano sempre
  rispettati i limiti massimi e minimi impostati tanto sul singolo
  componente quanto complessivamente sull'intero Box.

> Nel caso in cui a seguito della variazione apportata si dovesse
> superare la quantità complessiva di articoli acquistabili con
> l'interno box verrà visualizzato un apposito popup di notifica

- verrà ricalcolato, sulla base delle quantità attualmente impostate, il
  prezzo complessivo del Box.

> **ATTEZIONE! Il prezzo complessivo di un Campionario Configurabile è
> dato dalla somma dei prezzi dei singoli articoli presenti all'interno
> del Campionario stesso**

- verrà aggiornato, sulla base delle quantità attualmente impostate, il
  valore della disponibilità dell'interno Box (sia quello aggiornato
  all'ultima sincronizzazione che quello richiesto in tempo reale).

> **ATTEZIONE! Come per i Campionari semplici, anche per quelli
> Configurabili la disponibilità dell'intero Box verrà valutata in
> relazione a quelle che sono le disponibilità e le quantità attualmente
> impostate per i singoli componenti del campionario.**
>
> Nel caso in cui si sia deciso di gestire all'interno del Campionario
> Configurabile anche un' articolo strutturato, inizialmente verrà
> considerata la disponibilità dell'articolo padre piuttosto che quella
> dell'articolo padre più quella di eventuali figli, dipendentemente da
> come è stato impostato il parametro "**Mostra la disponibilità del
> padre**" in fase di configurazione della struttura stessa all'interno
> del Wizard

![](./assets/media/image84.png)

> Una volta impostata una ben precisa configurazione, e selezionato
> quindi il relativo articolo figlio, verrà poi considerata la sua
> effettiva disponibilità solo nel caso in cui questo sia stato anche
> esportato e gestito all'interno del sito; in caso contrario continuerà
> ad essere considerata la disponibilità dell'articolo padre oppure
> quella del padre + figli.

Come per i Campionari semplici anche in questo caso le uniche cose da
fare, lato gestionale, per poter gestire all\'interno del proprio sito
e-commerce questa tipologia di articoli, è quella di esportare e sul
sito sia l'articolo Campionario che tutti i suoi componenti.

Per quel che riguarda invece le formule gestibili, lato Mexal, per
determinare in maniera dinamica le quantità dei singoli articoli
componenti il Campionario, è bene sottolineare come, **nel caso dei
Campionari Configurabili, non siano ovviamente considerate** essendo in
queste condizioni l'utente stesso, in fase di acquisto, a poter variare
tali quantità.

Infine è bene sottolineare anche come:

- **All'interno del Carrello e della Wishlist** verranno visualizzati,
  in relazione ai Campionari Configurabili, sia l'articolo Campionario
  che l'elenco dei suoi componenti

![](./assets/media/image85.png)

> Per l'articolo Campionario sarà possibile modificare la quantità
> presente in carrello, eliminarlo dal carrello, inserire note di riga,
> date di scadenza ecc...
>
> **L'elenco dei componenti, al contrario è in sola visualizzazione** e
> non sarà quindi possibile variare dal Carrello ne tanto meno dalla
> Wishlist la composizione del Campionario.
>
> Per ogni componente verranno visualizzate tutte le informazioni
> impostate in fase di configurazione del Carrello/Wishlist ad eccezione
> del prezzo e del totale di riga (informazioni queste visualizzate a
> livello globale solo ed esclusivamente per l'intero Campionario)

- Il passaggio di un Campionario configurabile tra i componenti
  Carrello, Wishlist, o Comparatore comporterà il passaggio anche di
  tutti suoi componenti. Nello specifico, **all'interno del Comparatore,
  verrà però visualizzato il solo Campionario** (no elenco componenti)
  con il prezzo dettato dalla specifica composizione per esso impostata.

- **Per ogni inserimento in Carrello / Wishlist / Comparatore di un
  Campionario Configurabile verrà sempre creata una nuova riga**. Nel
  momento in cui si dovessero quindi inserire in carrello, ad esempio,
  due distinti box configurabili con due diverse configurazioni,
  verranno create due righe distinte, una corrispondente al primo Box
  con la relativa lista di componenti e una corrispondente al secondo
  Box anch'essa con la relativa lista di componenti.

- All'interno dei Componenti Ordine / Reso verrà visualizzato (a
  differenza di quanto avviene in Carrello o in Wishlist) solo l'elenco
  dei componenti e per ciascuno di essi verrà visualizzato sia il prezzo
  unitario che il totale di riga.

