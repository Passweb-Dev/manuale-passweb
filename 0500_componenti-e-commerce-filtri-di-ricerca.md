# COMPONENTI E-COMMERCE -- FILTRI DI RICERCA



Come precedentemente evidenziato, per poter creare correttamente un
pannello di Ricerca Ecommerce sarà necessario, per prima cosa,
configurare il componente "**Ricerca sul sito**" (sezione dei Componenti
Comuni) impostando il parametro "**Tipo**" sul valore "**Ricerca
E-Commerce**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_ecommerce0_res.bmp](./assets/media/image24.png)

e settare poi gli altri parametri di configurazione coerentemente con il
tipo di pannello di ricerca che si intende realizzare (filtri vincolati,
pannello collegato ad altri pannelli di ricerca presenti sul sito
ecc...)

Una volta terminata la configurazione del pannello di ricerca sarà poi
necessario inserire al suo interno i singoli campi (campi di testo
libero, menu a tendina, lista check box ecc...) che dovranno andare a
comporre i vari filtri.

In questo senso sarà possibile inserire all'interno di un pannello di
ricerca Ecommerce i seguenti elementi:

- Filtro Testo

- Filtro Lista

- Filtro Indice

- Filtro Checkbox

- Filtro Slider

- Filtro Treeview

- Filtro Autocompletamento

- Filtro Set Attributi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_ricerca_catalogo_aggiunta_componenti_res.bmp](./assets/media/image595.png)

Per maggiori informazioni in relazione alle diverse tipologie di campi
gestibili all'interno di un pannello di ricerca Ecommerce si vedano
anche i successivi capitoli di questo manuale.

In ogni caso ad ogni Componente E-commerce inserito all'interno del
pannello di ricerca dovrà necessariamente corrispondere uno specifico
campo Mexal o uno specifico Attributo Articolo, e sarà poi su questi
elementi che verrà effettuata la ricerca, lato sito, sulla base dei
valori indicati dall'utente all'interno di questi stessi campi.

Nella maschera di configurazione di ciascun componente inserito
all'interno di un pannello di ricerca sarà sempre presente quindi il
parametro "**Tipologia di Filtro**" mediante il quale poter indicare lo
specifico campo Mexal o lo specifico Attributo Passweb su cui dovrà
essere realizzato il filtro di ricerca che si intende implementare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_testo_configurazione1_res.bmp](./assets/media/image596.png)

In particolare nel caso in cui il campo "**Tipologia di Filtro**" sia
impostato sul valore:

**Filtro su Campo Articolo:** sarà possibile selezionare dal sottostante
menu a tendina ("**Campo su cui far Filtro**") lo specifico campo
dell'Anagrafica Articoli del gestionale cui far corrispondere il campo
di filtro che si sta configurando.

Nello specifico dipendentemente dalla tipologia di componente
utilizzato, sarà possibile selezionare uno tra i seguenti valori:

- **Titolo Articolo:** selezionando questo valore, il campo in esame
  corrisponderà, di base, **al campo Descrizione** dell'**Anagrafica
  Articoli del gestionale**. Inserendolo quindi all'interno del pannello
  di ricerca esso consentirà di ricercare gli articoli presenti nel
  Catalogo E-Commerce secondo quello che è il valore per essi inserito
  all'interno del campo "Descrizione" della loro Anagrafica gestionale

> Per i siti Ecommerce collegati a Mexal nel caso di gestione in
> multilingua, dipendentemente dalla lingua di partenza del sito, la
> ricerca del testo indicato verrà effettuata sul valore del
> corrispondente campo Mexal in italiano o in lingua. Ovviamente questo
> tipo di gestione richiede che siano state correttamente impostate in
> Mexal le descrizioni in lingua dei vari articoli e che sia stata
> stabilita in Passweb una specifica corrispondenza tra le lingue del
> sito e i codici della **"Tabella Lingue Estere"** di Mexal (per
> maggiori informazioni in merito si veda anche il capitolo
> *"Configurazione -- Parametri Paese Lingua e Valuta -- Gestione
> Lingua"* di questo manuale).
>
> Ovviamente nel caso in cui il Titolo dell'articolo non sia stato
> mappato con la Descrizione presente nella relativa anagrafica
> gestionale ma con uno specifico Attributo Passweb, piuttosto che con
> un valore personalizzato inserito direttamente nell'anagrafica Passweb
> dello specifico articolo, anche le ricerche effettuate mediante il
> campo in questione varieranno di conseguenza.
>
> Per maggiori informazioni relativamente a come poter mappare il Titolo
> dell'articolo sulla descrizione gestione, su di un attributo Passweb o
> su di un valore personalizzato, si veda la relativa sezione di questo
> manuale "*Sito -- Preferenze -- SEO Titolo / Permalink Articolo*"

- **Descrizione Articolo**: selezionando questo valore, il campo in
  esame corrisponderà al campo **"Descrizione"** presente all'interno
  della maschera **"Modifica Articolo"** qui di seguito riportata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_descrizione.bmp](./assets/media/image430.png)

> Inserendolo quindi all'interno del pannello di ricerca esso consentirà
> di ricercare gli articoli presenti nel Catalogo E-Commerce secondo
> quello che è il contenuto per essi inserito all'interno del campo
> "Descrizione" sopra evidenziato (contenuto questo che può essere
> prelevato direttamente da Docuvision).
>
> Nel caso di siti multilingua, dipendentemente dalla lingua di partenza
> del sito, la ricerca del testo indicato verrà effettuata sul valore
> del campo Descrizione in italiano o in lingua.

- **Codice Articolo**: selezionando questo valore, il campo in esame
  corrisponderà al campo **Codice** dell'**Anagrafica Articoli del
  gestionale**. Inserendolo quindi all'interno pannello di ricerca esso
  consentirà di ricercare gli articoli presenti nel Catalogo E-Commerce
  secondo quello che è il codice per essi definito all'interno del
  gestionale

- **Codice Alternativo Articolo (solo Ecommerce Mexal)**: selezionando
  questo valore, il campo in esame consentirà di effettuare ricerche sui
  codici alternativi degli articoli codificati in Mexal.

- **Codice Alias Articolo:** selezionando questo valore, il campo in
  esame consentirà di effettuare ricerche sui codici Alias definiti per
  i relativi articoli all'interno del gestionale.

- **Codice Articolo + Codice Alias Articolo:** selezionando questo
  valore, il campo in esame consentirà di ricercare gli articoli
  presenti nel Catalogo E-Commerce sia secondo quello che è il loro
  codice Alias, sia secondo quello che è il loro effettivo codice
  articolo.

> **ATTENZIONE!** La ricerca sui campi "Codice Articolo", "Codice
> Alternativo", "Codice Alias" e "Codice Articolo + Codice Alias" **è
> una ricerca "per valore iniziale".**
>
> Supponendo dunque di avere un articolo con codice "AR123" nel momento
> in cui dovesse essere effettuata una ricerca per codice indicando come
> valore da ricercare "123" non verrà restituito nessun risultato

- **Codice Articolo + Titolo Articolo:** selezionando questo valore, il
  campo in esame consentirà di ricercare gli articoli presenti nel
  Catalogo E-Commerce sia secondo quello che è il loro codice, sia
  secondo quella che è la loro descrizione.

- **Codice Articolo + Descrizione Articolo:** selezionando questo
  valore, il campo in esame consentirà di ricercare gli articoli
  presenti nel Catalogo E-Commerce sia secondo quello che è il loro
  codice, sia secondo quello che è il contenuto per essi inserito
  all'interno del campo "Descrizione" precedentemente evidenziato.

- **Codice** **Articolo** + **Titolo Articolo + Descrizione Articolo:**
  selezionando questo valore, il campo in esame consentirà di ricercare
  gli articoli presenti nel Catalogo E-Commerce secondo quello che è il
  loro codice, la loro descrizione o il contenuto per essi inserito
  all'interno del campo "Descrizione" precedentemente evidenziato.

- **Categoria Merceologica --** opzione disponibile solo per componenti
  **Filtro Lista, Filtro Indice, Filtro Checkbox, Filtro Treeview**

> Selezionando questo valore, il campo in esame consentirà di
> visualizzare all'interno del pannello di ricerca l'elenco di tutte le
> descrizioni delle Categorie Merceologiche degli articoli presenti in
> Catalogo.
>
> In queste condizioni, in particolare, i valori stampati all'interno
> del pannello di ricerca varieranno in relazione alla pagina in cui è
> inserito il componente "Filtro/Ricerca Ecommerce" che ospita il
> "Filtro Indice" che si sta realizzando.
>
> Nello specifico se il componente "Filtro/Ricerca Ecommerce" è inserito
> all'interno di una Pagina Generica (pagina bianca) o all'interno di
> una pagina Ecommerce (pagina verde) verranno stampate le descrizione
> delle sole categorie merceologiche di primo livello.
>
> Nel caso in cui invece il componente "Filtro/Ricerca Ecommerce" sia
> inserito in una specifica Pagina Catalogo (pagina blu) verranno
> stampate le sole descrizioni delle sotto categorie di primo livello
> della categoria merceologica corrispondente alla Pagina Catalogo
> considerata.

- **Categoria Merceologica e Sotto Categorie --** opzione disponibile
  solo per componenti **Filtro Lista, Filtro Indice, Filtro Checkbox,
  Filtro Treeview**

> Selezionando questo valore, il campo in esame consentirà di
> visualizzare all'interno del pannello di ricerca l'elenco di tutte le
> descrizioni delle Categorie Merceologiche degli articoli presenti nel
> Catalogo E-Commerce.
>
> Anche in queste condizioni i valori visualizzati all'interno della
> combo box varieranno in relazione alla pagina in cui è inserito il
> componente "Filtro/Ricerca Ecommerce" che ospita il "Filtro Indice"
> che si sta realizzando.
>
> A differenza del caso precedente però, in queste condizioni, se il
> componente "Filtro/Ricerca Ecommerce" è inserito all'interno di una
> Pagina Generica (pagina bianca) o all'interno di una pagina Ecommerce
> (pagina verde) verrà visualizzato l'elenco di tutte le categorie
> merceologiche (fino ad un livello di profondità N) gestite all'interno
> del sito e che hanno almeno un articolo pubblicato.
>
> Nel caso in cui invece il componente sia inserito in una specifica
> pagina Catalogo (pagina blu), corrispondente ad una specifica
> categoria merceologica, verranno visualizzate tutte le sue sotto
> categorie gestite all'interno del sito e che hanno almeno un articolo
> pubblicato.

- **Categoria Statistica Articolo:** selezionando questo valore, il
  campo in esame consentirà di ricercare gli articoli presenti nel
  Catalogo E-Commerce secondo quella che è la descrizione della loro
  Categoria Statistica di appartenenza all'interno del gestionale.

- **Natura (solo Ecommerce Mexal):** selezionando questo valore, il
  campo in esame consentirà di ricercare gli articoli presenti nel
  Catalogo E-Commerce secondo quella che è la descrizione della Natura
  Mexal cui sono stati associati.

- **Disponibilità --** opzione disponibile solo per il componente
  **Filtro Checkbox**

> In queste condizioni il campo in esame consentirà di ricercare gli
> articoli presenti in Catalogo sulla base della loro **disponibilità
> Passweb**
>
> Selezionando quindi il relativo check verranno visualizzati, come
> risultato del filtro, i soli articoli per i quali la disponibilità
> memorizzata in Passweb risulti essere maggiore di zero.
>
> **ATTENZIONE!** Nel valutare quella che per Passweb è la quantità
> effettiva di un certo articolo su di un determinato magazzino occorre
> sempre tener conto di quanto impostato alla pagina "**Catalogo --
> Configurazione Parametri Catalogo**" all'interno della sezione
> "Disponibilità" sia in termini di formula utilizzata per il calcolo
> della disponibilità che in termini di Scorta Minima

- **Listino** -- opzione disponibile solo per componenti **Filtro Lista,
  Filtro Indice, Filtro Checkbox, Filtro Slider**

> Selezionando questo valore, il campo in esame consentirà di ricercare
> gli articoli presenti in Catalogo sulla base del loro **Prezzo di
> Listino**.
>
> **ATTENZIONE: la ricerca per prezzo verrà effettuata tendo conto solo
> ed esclusivamente dei prezzi definiti nel listino utilizzato per
> l'utente che sta navigando il sito. Non verrà quindi considerata, in
> questo tipo di ricerca, nessun tipo di particolarità e/o scontistica
> definita all'interno del gestionale o in fase di configurazione del
> sito stesso.**
>
> [Nel caso infatti di particolarità prezzo e/o sconto il prezzo
> effettivo degli articoli non è memorizzato nel database di Passweb ma
> viene calcolato in tempo reale sulla base delle condizioni commerciali
> definite per lo specifico articolo e/o per lo specifico utente che sta
> navigando il sito]{.underline}.
>
> **Nel caso in cui si dovesse quindi decidere di utilizzare una ricerca
> per prezzo e, allo stesso tempo, anche delle particolarità prezzo e/o
> sconto, una volta impostato un certo range ed effettuata la ricerca,
> nei risultati potrebbero rientrare anche articoli il cui prezzo di
> listino soddisfa effettivamente il range impostato ma con un prezzo
> effettivo che, in virtù di determinate particolarità, risulta essere
> al di fuori di quanto precedentemente impostato in fase di ricerca.**
>
> **ATTENZIONE! Dalle ricerche per prezzo verranno ovviamente esclusi
> gli articoli con "Prezzo a Richiesta**" (per maggiori informazioni in
> merito a questa particolare funzionalità si veda anche la sezione
> "*"Configurazione Gestionale -- Attivazione Passweb -- Funzionalità
> Mexal Articoli -- Prezzo Articoli a Richiesta"* di questo manuale)
>
> In queste condizioni nella maschera di configurazione del componente
> verrà visualizzato anche il campo **Step**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\flitro_lista_step_prezzo_res.bmp](./assets/media/image597.png)

> mediante il quale poter indicare l'intervallo di definizione dei vari
> scaglioni di prezzo su cui sarà poi possibile effettuare le ricerche.
>
> Supponendo quindi di impostare questo campo sul valore 100,
> all'interno del sito sarà poi possibile ricercare gli articoli il cui
> prezzo di listino ricade nel range 0-100€, 100€-200€, 200€-300€ ... Il
> valore dell'ultimo scaglione verrà determinato in automatico sulla
> base dei prezzi di listino degli articoli effettivamente presenti in
> catalogo.

![Videate\\flitro_lista_step_prezzo2.bmp](./assets/media/image598.png)

> **ATTENZIONE! Nel caso in cui lo step impostato dovesse essere tale da
> produrre un numero di scaglioni superiore a 100, al salvataggio del
> componente verrà visualizzato un apposito messaggio di errore e non
> verrà di fatto impostato nessun tipo di scaglione.**

![Videate\\flitro_lista_step_prezzo3.bmp](./assets/media/image599.png)

> **ATTENZIONE! Impostando questo tipo di filtro per la prima volta,
> sarà poi necessario effettuare una sincronizzazione totale in modo
> tale da aggiornare il database del sito con i prezzi di listino
> corretti.**

- **Codici Fornitore --** opzione disponibile solo per componenti
  **Filtro Testo, Filtro Autocompletamento, Filtro Lista, Filtro Indice,
  Filtro Checkbox**

> Selezionando questo valore, il campo in esame consentirà di ricercare
> gli articoli presenti all'interno del Catalogo Ecommerce sulla base
> dei "Codici Conto Fornitore" ad essi associati mediante l'apposita
> tabella gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\codici_fornitore.bmp](./assets/media/image600.png)

> **ATTENZIONE!** affinché un articolo possa essere ricercato per quelli
> che sono i suoi Codici Fornitore è necessario che:

- I fornitori in esame siano stati correttamente associati all'articolo
  all'interno della tabella sopra evidenziata

- I fornitori in esame siano stati correttamente esportati e gestiti
  all'interno del sito

<!-- -->

- **Nominativo Fornitori: --** opzione disponibile solo per componenti
  **Filtro Testo, Filtro Autocompletamento, Filtro Lista, Filtro Indice,
  Filtro Checkbox**

> Selezionando questo valore, il campo in esame consentirà di ricercare
> gli articoli presenti all'interno del Catalogo Ecommerce sulla base
> del "Nominativo" dei fornitori ad essi associati mediante l'apposita
> tabella gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nominativi_fornitore.bmp](./assets/media/image601.png)

> **ATTENZIONE!** come per i codici fornitore, anche in questo caso,
> affinché un articolo possa essere ricercato per quelli che sono i
> Nominativi dei suoi Fornitori è necessario che:

- I fornitori in esame siano stati correttamente associati all'articolo
  all'interno della tabella sopra evidenziata

- I fornitori in esame siano stati correttamente esportati e gestiti
  all'interno del sito

<!-- -->

- **Codice Articolo Fornitori --** opzione disponibile solo per
  componenti **Filtro Testo, Filtro Autocompletamento, Filtro Lista,
  Filtro Indice, Filtro Checkbox**

> Selezionando questo valore, il campo in esame consentirà di ricercare
> gli articoli presenti all'interno del Catalogo Ecommerce sulla base
> dei loro "Codici Articolo Fornitore"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\codici_articolo_fornitore.bmp](./assets/media/image602.png)

- **FullText:** selezionando questo valore il Componente "Filtro Testo"
  che si sta realizzando consentirà di ricercare gli articoli presenti
  in Catalogo sulla base dei valori presenti, per ciascuno di essi,
  all'interno del campo **FullText**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_fulltext_configurazione_2.bmp](./assets/media/image603.png)

> Per maggiori informazioni relativamente a come creare e gestire il
> campo FullText evidenziato in figura si veda anche la corrispondente
> sezione di questo manuale "*Catalogo -- Configurazione Parametri
> Catalogo -- Catalogo Mexal / Ho.Re.Ca. -- Ricerca*"

- **Taglie** / **Taglie Disponibili** **--** **(solo Ecommerce Mexal)
  --** opzione disponibile solo per componenti **Filtro Indice, Filtro
  Checkbox, Filtro Lista**

> Selezionando questo valore, il campo in esame consentirà di ricercare
> gli articoli presenti all'interno del Catalogo in base ai valori di
> una determinata serie di Taglie/Colori (definita mediante l'apposita
> tabella gestionale).
>
> In queste condizioni nella maschera di configurazione del componente
> verrà infatti visualizzato anche il campo **Serie Taglie**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtri_articolo_taglie_colori.bmp](./assets/media/image604.png)

> mediante il quale poter appunto indicare, selezionandola dal relativo
> menu a tendina, la specifica serie di Taglie/Colori in relazione a cui
> dovranno poi essere mostrate le varie opzioni di ricerca.
>
> In particolare:

- nel momento in cui per il campo "**Serie Taglie**" dovesse essere
  indicata una specifica serie di Taglie/Colori, le opzioni di ricerca
  visualizzate sul front end del sito saranno relative unicamente a
  quella stessa serie.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_articolo_taglie_colori.bmp](./assets/media/image605.png)

> In queste condizioni inoltre se non dovesse essere indicata una
> specifica Label, come intestazione del campo di ricerca verrà
> utilizzata automaticamente la descrizione associata all'interno del
> gestionale alla serie di Taglie/Colori in questione

- nel momento in cui per il campo **"Serie Taglie**" non dovesse invece
  essere indicata nessuna serie in particolare, lasciando quindi il
  campo stesso non valorizzato, allora le opzioni di ricerca
  visualizzate sul front end del sito dipenderanno esattamente dalla
  specifica pagina in cui è stato inserito il componente di ricerca.

> In questo senso se il componente di ricerca dovesse essere inserito
> nella pagina "Negozio" (e quindi nel catalogo generale) le opzioni di
> ricerca visualizzate sul front end del sito saranno relative a tutte
> le serie di Taglie/Colori attualmente gestite.

![Videate\\filtri_articolo_taglie_colori2.bmp](./assets/media/image606.png)

> Se il componente di ricerca dovesse invece essere inserito in una
> determinata pagina di categoria le opzioni di ricerca visualizzate sul
> front end del sito saranno relative unicamente alle serie di
> Taglie/Colori associate agli articoli di quella stessa categoria.
>
> **ATTENZIONE!** l' eventuale icona del colore associato al relativo
> elemento della serie di taglie/colori verrà visualizzata solo
> all'interno di **Filtri Indice** e **Filtri Checkbox**. Nei Filtri
> lista verrà quindi visualizzata sempre e solo la descrizione del
> relativo elemento
>
> Per maggiori informazioni relativamente a come poter attivare e
> gestire all'interno del proprio sito una ricerca articoli basata sui
> valori di una determinata serie di Taglie/Colori si veda anche quanto
> indicato nel corrispondente capitolo di questo manuale ( "*Catalogo
> Gestione Articoli -- Taglie o Colori Ecommerce Mexal -- Ricerca
> Articoli per Taglia/Colore*" )

- **Strutture** **--** opzione disponibile solo per componenti **Filtro
  Indice, Filtro Checkbox** e **Filtro Lista**

> Selezionando questo valore, il componente in esame consentirà di
> ricercare gli articoli presenti all'interno del Catalogo sulla base
> dei possibili valori assunti dai campi delle strutture effettivamente
> abilitati per la funzionalità di ricerca articoli.
>
> In queste condizioni nella maschera di configurazione del componente
> verrà visualizzato anche il campo **Struttura**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtri_articolo_strutture.bmp](./assets/media/image607.png)

> mediante il quale poter indicare, selezionandola dal relativo menu a
> tendina, la specifica Struttura in relazione a cui dovranno poi essere
> mostrate le varie opzioni di ricerca.
>
> In particolare:

- nel momento in cui per il campo in esame dovesse essere indicata una
  specifica Struttura, le opzioni di ricerca visualizzate poi
  all'interno del pannello di ricerca saranno riferite sempre e soltanto
  ai campi di quella stessa struttura abilitati per la funzione di
  ricerca, indipendentemente dalla pagina in cui è stato inserito il
  filtro.

- nel momento in cui per il campo in esame non dovesse invece essere
  indicata nessuna Struttura in particolare, lasciando quindi il campo
  stesso non valorizzato, allora le opzioni di ricerca visualizzate sul
  front end del sito dipenderanno esattamente dalla specifica pagina in
  cui è stato inserito il componente di ricerca.

> In questo senso se il componente di ricerca dovesse essere inserito
> nella pagina "Negozio" (e quindi nel catalogo generale) le opzioni di
> ricerca visualizzate sul front end del sito saranno relative ai campi,
> abilitati per la funzione di ricerca articoli, di una qualsiasi
> struttura a cui appartengono gli articoli presenti in catalogo.
>
> **E' semplice comprendere quindi come, in queste condizioni, le
> opzioni di selezione presenti all'interno del pannello di ricerca
> potrebbero anche essere particolarmente numerose, aumentando di
> conseguenza i tempi di caricamento della pagina e riducendo di fatto
> anche l'usabilità del corrispondente pannello di ricerca**
>
> Se il pannello di ricerca dovesse invece essere inserito all'interno
> di una specifica pagina di categoria, le opzioni di selezione saranno
> relative ai campi, abilitati per la funzionalità di ricerca articoli,
> delle sole strutture cui appartengono gli articoli di quella specifica
> categoria
>
> **ATTENZIONE! in considerazione di quanto detto, al fine di
> ottimizzare le prestazioni del sito e l'usabilità stessa dei filtri, è
> sempre consigliabile utilizzare questo tipo di ricerca non a livello
> generale sull'intero catalogo ma solamente nelle specifiche pagine di
> categoria in cui sono effettivamente presenti degli articoli
> strutturati** (configurando quindi il filtro in maniera tale che
> lavori su di una specifica struttura e non su tutte quelle che possono
> essere effettivamente gestite all'interno sito)
>
> Per maggiori informazioni relativamente a come poter attivare e
> gestire la ricerca articoli sulla base delle opzioni disponibili per
> un determinato campo di una struttura si veda anche quanto indicato
> nel corrispondente capitolo di questo manuale ( "*Catalogo Gestione
> Articoli -- Strutture Ecommerce Mexal / Ho.Re.Ca. -- Gestione
> Strutture -- Ricerca Articoli su campi struttura*" )

**Filtro su Attributo Articolo:** sarà possibile selezionare dal
sottostante menu a tendina ("**Attributo su cui far Filtro**") solo ed
esclusivamente uno degli Attributi Articolo (siano essi di tipo Mexal
siano essi di tipo Passweb) precedentemente codificati all'interno della
corrispondente sezione del Wizard.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> degli Attributi Articolo ed al processo di categorizzazione degli
> articoli gestiti all'interno del sito si rimanda alla relativa sezione
> di questo manuale (Catalogo -- Gestione Attributi Articoli).

Nel caso in cui l'Attributo selezionato sia di tipo numerico nella
maschera di configurazione del componente potrebbe essere visualizzato
anche il campo **Step**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_lista_step_res.bmp](./assets/media/image608.png)

mediante il quale poter indicare l'intervallo di definizione dei vari
scaglioni che rappresenteranno poi le diverse possibili opzioni di
scelta presenti all'interno del menu a tendina.

Supponendo dunque di impostare questo campo sul valore 100, verranno
visualizzate le seguenti opzioni di scelta: 0-100, 100-200, 200-300 ...
L'utente potrà quindi ricercare tutti gli articoli per i quali
l'attributo collegato al campo di ricerca in questione ha un valore
compreso in uno dei range indicati

Il valore del primo e dell'ultimo scaglione verranno determinati
automaticamente sulla base de valori impostati sui vari articoli per
l'attributo in esame.

**ATTENZIONE! Nel caso in cui lo step impostato dovesse essere tale da
produrre un numero di scaglioni superiore a 100, al salvataggio del
componente verrà visualizzato un apposito messaggio di errore e non
verrà di fatto impostato nessun tipo di scaglione.**

In queste condizioni, inoltre, nel caso in cui il campo della Videata
Aggiuntiva Articoli di Mexal a cui si vuol far corrispondere il
componente in oggetto, non compaia tra quelli in elenco sarà necessario:

a)  Accertarsi di aver lanciato la funzione di **"Aggiornamento
    Attributi Mexal"** dalla pagina "Parametri Sincronizzazione" di
    Passweb

b)  Accertarsi di aver creato in Passweb l'**Attributo Articolo di tipo
    Mexal**, corrispondente al campo della Videata Aggiuntiva Articoli
    che si desidera utilizzare

> **NOTA BENE:** è possibile far corrispondere al componente in esame
> unicamente quei campi delle Videate Aggiuntive Articolo di Mexal per i
> quali è stato creato in Passweb un corrispondente "Attributo Articolo"
> di tipo Mexal.

Infine oltre al parametro "Tipologia di Filtro" nella maschera di
configurazione di ciascun componente inserito all'interno di un pannello
di ricerca saranno sempre presenti anche i seguenti parametri

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia il Campo di input)

> E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame, permettendo dunque, già in fase di
> configurazione del componente stesso di decidere quale elemento dovrà
> essere visualizzato prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

- **Posizionamento del bottone rimuovi filtro:** consente di decidere
  dove posizionare il pulsante di rimozione del filtro che verrà
  visualizzato solo dopo aver utilizzato il campo in esame per applicare
  uno specifico filtro di ricerca. E' possibile decidere di posizionare
  tale pulsate primo o dopo il campo di filtro.

- **Nome Tracciamento:** consente di assegnare al componente in esame un
  nome che verrà poi utilizzato per identificare il relativo campo di
  ricerca nel momento in cui si dovesse decidere di tracciare le
  ricerche interne al sito mediante Google Analytics (per maggiori
  informazioni in merito si veda anche quanto indicato all'interno del
  capitolo "*Google Analytics -- Google Analytics 4 -- Monitoraggio
  Ecommerce -- Ricerca Search*" di questo manuale).

