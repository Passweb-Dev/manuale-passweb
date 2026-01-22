# ECOMMERCE HO.RE.CA. -- ARTICOLI COMPOSTI CONFIGURABILI



Come evidenziato nel precedente capitolo di questo manuale, nel caso in
cui l'esigenza dovesse essere quella di gestire dei Box configurabili
dando quindi all'utente la possibilità di decidere, direttamente in fase
di acquisto all'interno del sito, come comporre il suo Box, scegliendo
tra una lista di articoli preconfigurata, quali andare effettivamente ad
inserire all'interno del Box, ed eventualmente in che quantità, e quali
no si dovrà ricorrere per forza di cose ad un articolo **Composto
Configurabile**.

Per gestire questo tipo di articoli sarà quindi necessario, per prima
cosa, rendere configurabile il Composto definito all'interno del
gestionale e impostare i limiti entro i quali l'utente potrà poi
muoversi in fase di composizione del suo Box.

In questo senso dovremo quindi agire dalla sezione "**Dati Articolo**"
(accessibile sul Wizard alla voce di menu "*Catalogo -- Gestione
Articoli*") selezionando il Composto in esame, attivando il check
"**Abilita Configurazione**" e impostando le quantità minime e massime
tra cui l'utente potrà muoversi per ogni singolo componente del
Campionario.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\articoli_composti7.bmp](./assets/media/image92.png)

**ATTENZIONE!** Per maggiori informazioni relativamente a come rendere
configurabile un articolo Composto e come poter impostare per ogni
singolo componente le quantità minime e massime tra cui scegliere si
veda anche la sezione "*Catalogo -- Gestione Articoli -- Articoli --
Anagrafica Articolo/Servizio -- Anagrafica Passweb -- Box*" di questo
manuale

Anche in questo caso affinchè l'articolo possa essere correttamente
gestito all'interno del sito, lato gestionale dovranno essere
soddisfatte determinate caratteristiche di configurazione.

Nello specifico sarà necessario:

- Esportare sul sito l'Articolo Composto e tutti i suoi Componenti
  selezionando per ciascuno di essi, nelle relative anagrafiche il campo
  "**Abilita Passweb**".

> **ATTENZIONE!** nel caso in cui alcuni articoli del Composto non
> vengano esportati, ci sarà, ovviamente, una differenza tra quanto
> impostato sul gestionale e quanto presente invece all'interno del sito
> E-commerce, relativamente all'elenco dei componenti e di conseguenza
> anche relativamente al prezzo del Composto stesso

- L'elenco degli articoli Componenti deve essere ben definito e
  realizzato quindi mediante l'opzione "**Articoli Prestabiliti**"

![Videate\\articoli_composti2.bmp](./assets/media/image87.png)

> **ATTENZIONE!** Non sono attualmente gestiti Articoli Composti in cui
> la lista dei Componenti è definita mediante le opzioni gestionali
> "Articoli presenti nella lista" o "Articoli presenti nelle categorie"

- A differenza dei Composti Semplici**, in questo caso i singoli
  componenti potranno anche essere dei Prototipi**.

> **ATTENZIONE!** **Nel caso in cui si decida di inserire un Prototipo
> come componente di un Composto Configurabile, sarà necessario
> selezionare anche il check "Consenti componenti non definiti" in
> maniera tale da poter garantire la possibilità di caricare
> correttamente in Cassa ordini web contenenti questo tipo di
> articoli.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti8.bmp](./assets/media/image93.png)

- A differenza dei Composti Semplici, in queste condizioni, **è
  possibile gestire lato web anche gli elementi del Composto per i quali
  non è stato selezionato, lato gestionale, il campo "Predefinito".**

![Videate\\articoli_composti3.bmp](./assets/media/image88.png)

> Nell'esempio riportato in figura il prodotto "acqua di Gio" è presente
> nella lista degli "Articoli Prestabiliti" del Composto "Cesto Regalo"
> ma non è stato impostato come **"Predefinito"**. Sul sito si avrà
> comunque la possibilità (essendo il Composto Configurabile) di fare
> inserire all'utente, in fase di configurazione del suo Box, anche
> questo stesso articolo.
>
> **ATTENZIONE! Ovviamente nel momento in cui si volesse decidere di
> abilitare anche elementi non Predefiniti, è consigliabile impostare
> per essi una quantità minima pari a 0 in maniera tale che l'utente
> possa sempre decidere di non inserirli all'interno del suo Box
> esattamente come avviene all'interno del gestionale.**

In queste condizioni dunque il Componente **"Campionario E-commerce"**
inserito all'interno della Scheda Prodotto consentirà non solo di
visualizzare l'elenco dei singoli elementi del Composto (predefiniti e
non predefiniti), ma offrirà all'utente anche la possibilità di decidere
come comporre il suo Box scegliendo quali articoli inserire, ed
eventualmente in che quantità, e quali no, il tutto ovviamente sempre
nei limiti impostati in fase di abilitazione del Composto Configurabile.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti9.bmp](./assets/media/image94.png)

Per ogni singolo componente potrà quindi essere visualizzato:

- **Il configuratore di prodotto**, nel caso in cui il componente in
  questione fosse un Prototipo.

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
  componente la quantità con cui quello stesso articolo dovrà essere
  inserito nel Box.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti10.bmp](./assets/media/image95.png)

> **ATTENZIONE!** Per visualizzare tale campo sarà necessario inserire,
> in fase di creazione della scheda prodotto, all'interno del componente
> "Campionario Ecommerce" anche il componente "**Aggiungi in Carrello**"
>
> Immediatamente al di sopra del campo di input verrà visualizzata anche
> un'etichetta (personalizzabile alla sezione "Testi / Messaggi" del
> Sito agendo sull'elemento "Range" del componente "Aggiungi al
> Carrello") con **l'indicazione delle quantità minima e massima
> impostabili per lo specifico componente.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti11.bmp](./assets/media/image96.png)

> Il valore minimo coincide con quello impostato all'interno del campo
> "**Quantità Minima**" e definito, lato Passweb, in fase di
> abilitazione del singolo componente del Campionario

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\articoli_composti12.bmp](./assets/media/image97.png)

> **ATTENZIONE! Se l'esigenza dovesse essere quella di rendere un
> componente del Box non obbligatorio (come ad esempio dovrebbe essere
> per gli elementi non Predefiniti) sarà sufficiente selezionare per
> esso il parametro "Abilita Configurazione" e contemporaneamente
> impostare la sua "Quantità Minima" sul valore 0 (o al limite lasciare
> vuoto il campo).**
>
> In queste condizioni infatti l'utente potrà impostare per l'articolo
> in questione, in fase di acquisto, una quantità pari a 0 decidendo, di
> fatto, di non inserirlo all'interno del Box.
>
> **ATTENZIONE!** A differenza di quanto avveniva per gli Ecommerce
> Mexal, in queste condizioni il campo "**Predefinito**" è in sola
> visualizzazione ed il suo valore può quindi essere gestito solo ed
> esclusivamente mediante il corrispondente campo gestionale.
>
> Il valore massimo coincide invece con la quantità impostata per lo
> specifico elemento lato gestionale all'interno del campo **Max**

![Videate\\articoli_composti4.bmp](./assets/media/image89.png)

> Infine **nel caso in cui lo specifico componente del Campionario fosse
> stato impostato come "Non Configurabile" (parametro "Abilita
> Configurazione" non selezionato), il campo di input per l'impostazione
> delle quantità sarà disabilitato e non verranno visualizzati neppure i
> relativi pulsanti incrementali**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti13.bmp](./assets/media/image98.png)

> In queste condizioni dunque l'utente non potrà apportare nessun tipo
> di variazione al componente che verrà quindi inserito nel Box così
> come stabilito all'interno del gestionale.

Oltre alle etichette con l'indicazione delle quantità minima e massima
impostabili per lo specifico componente, è possibile visualizzare,
immediatamente al di sotto del componente Campionario, anche un testo
riepilogativo con l'indicazione delle quantità minima e massima globali
effettivamente gestibili per il Box.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti14.bmp](./assets/media/image99.png)

In questo caso il numero minimo di elementi (inteso come quantità
complessive) che dovranno essere necessariamente presenti all'interno
del Box prima di poterlo inserire in carrello, coincide con il valore
impostato, lato Passweb, in corrispondenza del parametro "**Numero
Minimo Componenti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\articoli_composti15.bmp](./assets/media/image100.png)

**ATTENZIONE! Il valore di questo parametro dovrà essere, ovviamente,
minore o uguale alla somma delle quantità minime dei singoli componenti
del Campionario**

Il numero massimo (intesto sempre come quantità complessive) di articoli
che potranno essere inseriti all'interno di un Box configurabile
coincide invece con il valore impostato, lato gestionale, all'interno
del campo "**N° Massimo Complessivo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_composti16.bmp](./assets/media/image101.png)

**ATTENZIONE! Il numero massimo di articoli gestibili all'interno del
Box dovrà essere, ovviamente, maggiore o uguale alla somma delle
quantità massime dei singoli componenti del Campionario**

Nel momento in cui un utente dovesse apportare delle variazioni alle
quantità dei singoli componenti del Box:

- verranno avviati dei controlli per garantire che siano sempre
  rispettati i limiti massimi e minimi impostati tanto sul singolo
  componente quanto complessivamente sull'intero Box.

- verrà ricalcolato, sulla base delle quantità attualmente impostate, il
  prezzo complessivo del Box.

> **ATTEZIONE! Il prezzo complessivo di un Composto Configurabile verrà
> calcolato tenendo conto di quelli che sono i componenti effettivamente
> gestiti sul sito e di quanto impostato, lato gestionale, all'interno
> della sezione "Formula calcolo del prezzo di vendita"**

![Videate\\articoli_composti5.bmp](./assets/media/image102.png)

- verrà aggiornato, sulla base delle quantità attualmente impostate, il
  valore della disponibilità dell'intero Box (sia quello aggiornato
  all'ultima sincronizzazione che quello richiesto in tempo reale).

> **ATTEZIONE! Come per i Composti Semplici, anche per quelli
> Configurabili la disponibilità dell'intero Box verrà valutata in
> relazione a quelle che sono non solo le disponibilità dei singoli
> componenti ma anche in relazione a quella che è la disponibilità del
> Composto in sé.**
>
> Nel caso in cui si sia deciso di gestire all'interno del Composto
> Configurabile anche un Prototipo, inizialmente verrà considerata la
> disponibilità dell'articolo padre piuttosto che quella dell'articolo
> padre più quella di eventuali figli, dipendentemente da come è stato
> impostato il parametro "**Mostra la disponibilità del padre**" in fase
> di configurazione della struttura stessa all'interno del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\disponibilita_campionario.bmp](./assets/media/image103.png)

> Una volta impostata una ben precisa configurazione, e selezionato
> quindi il relativo articolo figlio, verrà poi considerata la sua
> effettiva disponibilità solo nel caso in cui questo sia stato anche
> esportato e gestito all'interno del sito; in caso contrario continuerà
> ad essere considerata la disponibilità dell'articolo padre oppure
> quella del padre + figli.

Infine è bene sottolineare anche come:

- **All'interno dei componenti Carrello, Wishlist, Ordine e Reso**
  verranno sempre visualizzati, in relazione ai Composti Semplici, sia
  l'articolo Composto che l'elenco dei suoi componenti.

![Videate\\articoli_composti6.bmp](./assets/media/image91.png)

> Per l'articolo Composto sarà possibile modificare la quantità presente
> in carrello, eliminarlo dal carrello, inserire note di riga, date di
> scadenza ecc...
>
> **L'elenco dei componenti, al contrario è in sola visualizzazione**.
>
> Per ogni componente verranno visualizzate tutte le informazioni
> impostate in fase di configurazione del Carrello/Wishlist/Ordine/Reso
> ad eccezione del prezzo e del totale di riga (informazioni queste
> visualizzate a livello globale solo ed esclusivamente per l'intero
> articolo Composto).

- Il passaggio di un Composto Semplice tra i componenti Carrello,
  Wishlist, o Comparatore comporterà il passaggio anche di tutti suoi
  componenti. Nello specifico, **all'interno del Comparatore, verrà però
  visualizzato il solo articolo Composto** senza il dettaglio dell'
  elenco componenti.

- **Per ogni inserimento in Carrello / Wishlist / Comparatore di un
  Composto Configurabile verrà sempre creata una nuova riga**. Nel
  momento in cui si dovessero quindi inserire in carrello, ad esempio,
  due distinti box configurabili con due diverse configurazioni,
  verranno create due righe distinte, una corrispondente al primo Box
  con la relativa lista di componenti e una corrispondente al secondo
  Box anch'essa con la relativa lista di componenti.

