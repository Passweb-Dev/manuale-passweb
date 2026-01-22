# FILTRO TREEVIEW



Il Componente "**Filtro TreeView**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_filtro_tree_res.bmp](./assets/media/image627.png){width="2.5340277777777778in"
height="2.5458333333333334in"}

**può essere inserito unicamente all'interno del componente Ecommerce di
primo livello "Ricerca"**.

Grazie a questo componente sarà possibile visualizzare all'interno del
pannello di ricerca **un elenco gerarchico** di tutti i possibili valori
assunti (per gli articoli gestiti all'interno del sito) dall'Attributo
Articolo o dal campo del gestionale che verrà fatto corrispondere al
componente in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\filtro_treeview_esempio.bmp](./assets/media/image628.png){width="5.429166666666666in"
height="3.5027777777777778in"}

**ATTENZIONE!** **L'unico dato effettivamente gestito a livello
gerarchico (padre -- figlio) è quello relativo alle Categorie e alle
Sotto Categorie merceologiche.**

Mappando quindi il componente in oggetto con il campo Mexal "**Categoria
Merceologica e Sotto Categorie**" verrà effettivamente visualizzato
l'elenco di tutte le categorie ed eventuali sotto categorie
merceologiche, organizzate all'interno di una struttura gerarchica ad
albero del tipo di quella rappresentata in figura.

In tutti gli altri casi, considerando che i valori del campo Mexal/
Ho.Re.ca. e/o dell'Attributo Articolo mappato, sono organizzati sempre e
solo su di un unico livello, il comportamento del componente "Filtro
TreeView" sarà in tutto e per tutto simile a quello del componente
"Filtro Indice" precedentemente esaminato.

Ogni singola voce visualizzata all'interno del componente, se cliccata,
consentirà di filtrare gli articoli in catalogo sulla base del valore
appena selezionato. Il risultato del filtro verrà poi visualizzato nella
stessa pagina in cui si trova il pannello di ricerca o, al limite, nella
specifica pagina di destinazione impostata nella configurazione del
pannello stesso.

Nel momento in cui si dovesse decidere dunque di far corrispondere
questo componente alle Categorie e Sotto Categorie Merceologiche a
livello statistico, indipendentemente dal fatto di ricercare i prodotti
della categoria "informatica" piuttosto che quelli della categoria
"fotografia" la pagina in cui verranno visualizzati i risultati sarà
sempre la stessa e questo renderà più complicato capire cosa
effettivamente cercano gli utenti del nostro sito.

In questo senso utilizzando un menu di categoria articoli il risultato
che si otterrebbe potrebbe sembrare analogo in quanto, di fatto, si
otterrebbero sempre tutti gli articoli appartenenti ad una specifica
categoria merceologica.

In realtà, in questo caso, il risultato è profondamente diverso,
soprattutto a livello statistico. Utilizzando infatti un menu di
categoria, gli articoli corrispondenti alla categoria merceologica
selezionata verranno visualizzati all'interno della specifica pagina
(es. www.ecommerce.passweb.it/catalogo-articoli/informatica) il che
renderà sicuramente più facile capire quali sono le categorie
merceologiche più ricercate all'interno del sito, analizzando
semplicemente quelle che sono le pagine di categoria più visitate.

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata **la sua maschera di gestione e
configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_treeview_configurazione_res.bmp](./assets/media/image629.png){width="5.153472222222222in"
height="3.1041666666666665in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di specificare il nome del Componente che si sta
realizzando

**Pubblico**: consente di impostare la visibilità lato sito web del
componente che si sta realizzando.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Label**: consente di specificare un'etichetta identificativa del
componente che si sta realizzando. Tale etichetta verrà poi visualizzata
all'interno del pannello di ricerca in corrispondenza dei valori assunti
dal componente in oggetto

**Campo di ordinamento**: visualizzato solo ed esclusivamente nel caso
in cui il parametro "Tipologia Filtro" sia impostato sul valore "Filtro
su Campo Articolo" e, contestualmente, il parametro "Campo su cui far
filtro" sia impostato sul valore "Categoria Merceologica" o "Categoria
Merceologica e Sotto Categorie".

Consente di definire se l'ordinamento delle categorie e sotto categorie
merceologiche visualizzate all'interno del componente dovrà essere
determinato sulla base della loro **Descrizione**, del loro **Codice** o
del valore **Personalizzato** inserito all'interno del campo "Posizione
nel Menu Categoria" presente nella maschera di configurazione della
categoria stessa.

**Visualizza il numero di elementi per le opzioni:** consente, se
selezionato, di visualizzare a fianco di ogni singola voce in elenco,
l'esatto numero di articoli in catalogo per i quali l'attributo in esame
assume quello specifico valore.

**Tipo di Caricamento:** consente di specificare come dovrà essere
gestita la visualizzazione delle voci di livello maggiore a 1.

E' possibile selezionare una delle seguenti opzioni:

- **A Richiesta:** in queste condizioni al caricamento della pagina web
  saranno presenti (nel DOM della pagina stessa) solo ed esclusivamente
  voci di primo livello. Eventuali voci di livello maggiore o uguale a 2
  verranno inserite all'interno della pagina solo ed esclusivamente nel
  momento in cui un utente dovesse richiederne la visualizzazione
  (cliccando per questo sull'apposita icona di apertura delle relative
  sotto voci).

> **Tale opzione potrebbe essere utile per diminuire i tempi di
> caricamento della pagina soprattutto nel caso in cui il numero delle
> sotto voci sia estremamente elevato**

- **Tutto in una Volta:** in queste condizioni al caricamento della
  pagina web saranno presenti (nel DOM della pagina stessa) tutte le
  voci del componente

**Tipo di Stili applicati alla TreeView:** consente di specificare lo
stile di visualizzazione del controllo nel momento in cui questo dovesse
essere mappato con il campo Mexal "Categorie e Sotto Categorie
Merceologie" dando quindi origine ad una struttura gerarchia ad albero
organizzata su diversi livelli.

E' possibile selezionare uno tra i seguenti valori.

- **Lista:** selezionando questo valore verranno visualizzate le voci di
  ogni livello.

- **TreeView:** selezionando questo valore, inizialmente verranno
  visualizzate soltanto le voci di primo livello. Eventuali sotto-voci
  verranno visualizzate (nascoste) al click del mouse sull'apposita
  icona di apertura (chiusura) presente a fianco di ciascuna voce che
  presenti almeno una voce di livello inferiore.

**Immagine Controllo Apri/Chiudi Ramo --** Visualizzato solo nel caso in
cui il parametro "Tipo di Stili applicati alla Treeview" sia stato
impostato sul valore "TreeView".

Consente di selezionare una specifica immagine da poter utilizzare per
il controllo di apertura / chiusura delle sottovoci. Nel caso in cui non
venga specificata nessun immagine il controllo di apertura delle
sottovoci sarà rappresentato da un **\[+\]** e quello di chiusura da un
**\[-\].**

**Tempo di comparsa (ms) --** presente solo per menu di tipologia
TreeView.

Consente di indicare uno specifico intervallo di tempo (in millisecondi)
che dovrà intercorrere prima dell'apertura/chiusura delle voci di
livello inferiore.

Per maggiori informazioni in merito a come poter indicare lo specifico
campo Mexal o lo specifico Attributo Passweb su cui dovrà essere
realizzato il filtro di ricerca che si intende implementare si veda
anche il precedente capitolo "*Componenti Ecommerce -- Filtri di
ricerca*" di questo manuale

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

