# CREAZIONE DI UNA VARIANTE RESPONSIVA



Le Varianti Responsive possono essere create e gestite operando
direttamente all'interno del Live Editing.

Nello specifico per poter accedere alla maschera di creazione e gestione
delle Varianti è necessario cliccare sul relativo pulsante **Gestione
Varianti**
(![Videate\\pulsante_gestione_varianti_me.bmp](./assets/media/image1.png) ) presente nel menu di Editing del Sito
o, in alternativa, sul corrispondente pulsante presente nella Barra
degli Strumenti del Live Editing
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\barra_strumenti_gestione_varianti.bmp](./assets/media/image2.png) ).

In entrambi i casi verrà comunque visualizzata la maschera "**Gestione
Varianti**" mediante la quale poter gestire tutte le Varianti Sito
attualmente codificate oltre che, ovviamente, poterne creare di nuove.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_2_res.bmp](./assets/media/image3.png)

Per creare una nuova Variante Responsiva sarà necessario, per prima
cosa, cliccare sul pulsante "**Crea una Variante**" presente nella parte
sinistra della maschera in maniera tale da poter accedere alla maschera
di definizione della nuova Variante

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_3_res.bmp](./assets/media/image4.png)

all'interno della quale poter indicare:

- **Nome della Variante Sito:** consente di assegnare alla Variante che
  si sta realizzando uno specifico nome

- **Codice:** consente di assegnare alla Variante che si sta realizzando
  uno specifico codice identificativo

- **Colore:** consente di assegnare alla Variante che si sta realizzando
  uno specifico colore (in maniera tale da poterla identificare così
  come avviene con il Nome e/o con il Codice, tra l'elenco delle altre
  Varianti gestite)

- **Tipologia:** consente di impostare la tipologia della Variante che
  si sta realizzando. Come precedentemente indicato a partire dalla
  versione 2019A sarà possibile creare unicamente nuove varianti di tipo
  Responsivo.

La sezione "**Generazione Pagine di Categoria**" consente di indicare la
specifica pagina che dovrà essere utilizzata come Template in fase di
creazione di nuove Pagine Catalogo e/o Prodotto generate a seguito della
creazione, all'interno del gestionale, di **nuove** categorie
merceologiche.

**ATTENZIONE!** Dalle pagine utilizzate come Template verranno prese non
solo le impostazioni grafiche ed i componenti in esse presenti ma anche
le proprietà della pagina stessa per cui se, ad esempio, la pagina
utilizzata come Template dovesse essere visibile ai soli utenti
autenticati anche tutte le nuove pagine di Categoria generate a partire
da essa avranno questo tipo di impostazione.

E' possibile indicare un specifico Template per le seguenti tipologie di
Pagina:

- **Pagina Negozio Padre:** sono le Pagine Catalogo (pagine blu)
  relative a Categorie Merceologiche che hanno altre sotto categorie e
  quindi altre Pagine Catalogo

- **Pagina Negozio Foglia:** sono le Pagine Catalogo (pagine blu)
  relative alle Categorie Merceologiche di ultimo livello prive dunque
  di ulteriori sotto categorie

- **Pagina Prodotto:** sono le normali Pagine Prodotto (pagine rosse)
  del sito

La distinzione tra "Pagina Negozio Padre" e "Pagina Negozio Foglia"
diventa di fondamentale importanza nel momento in cui si dovesse
implementare, ad esempio, una struttura di navigazione del sito che
preveda l'utilizzo del componente "Catalogo Ecommerce" solo ed
esclusivamente all'interno delle Pagine Catalogo Foglia, utilizzando
invece per le Pagine Catalogo Padre il componente "Lista Categorie" (per
maggiori informazioni relativamente a queste due tipologie d componenti
si vedano i successivi capitoli di questo manuale).

Considerando infatti che, in queste condizioni, la struttura delle
Pagine Catalogo, dovrà essere differente a seconda del fatto che siano
presenti o meno, per una determinata categoria merceologia anche delle
ulteriori sotto categorie, diventerà di fondamentale importanza
utilizzare per le Pagine Catalogo Padre e per le Pagine Catalogo Foglia
due Template distinti in maniera tale da automatizzare il processo di
creazione di nuove pagine di categoria senza dover ogni volta
intervenire in maniera manuale collegando e/o distribuendo i componente
corretti nelle relative pagine.

In questo senso dunque i parametri presenti all'interno della sezione
"Generazione Pagine di Categoria" consentono rispettivamente di:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\generazione_pagine_categoria_res.bmp](./assets/media/image5.png)

**Pagina Negozio Padre:** consente di indicare la specifica pagina del
sito che dovrà essere utilizzata come Template per la creazione di una
NUOVA "Pagina Negozio Padre".

**ATTENZIONE! Il parametro in oggetto ha effetto solo ed esclusivamente
sulla creazione di NUOVE Pagine Catalogo mentre non influenza o varia in
alcun modo eventuali pagine dello stesso tipo già presenti all'interno
del sito.**

E' possibile selezionare una delle seguenti opzioni.

- **Pagina Generica:** in queste condizioni eventuali nuove "Pagine
  Catalogo Padre", generate a seguito della creazione all'interno del
  gestionale di nuove categorie merceologiche, **verranno create
  assumendo come Template la "Pagina Negozio"** (radice di tutte le
  categorie merceologiche).

> Tali pagine assumeranno quindi lo stesso aspetto grafico e avranno
> esattamente gli stessi componenti della pagina Negozio.

- **Pagina Categoria Padre**: in queste condizioni eventuali nuove
  "Pagine Catalogo Padre", generate a seguito della creazione
  all'interno del gestionale di nuove categorie merceologiche,
  **verranno create assumendo come Template la Pagina Catalogo di
  livello immediatamente superiore.**

> Tali pagine assumeranno quindi lo stesso aspetto grafico, e avranno
> esattamente gli stessi componenti della loro Pagina Padre.
>
> **ATTENZIONE**! Nel caso in cui la Categoria Merceologica in questione
> dovesse essere di primo livello, e non avere quindi nessun padre
> gerarchico di livello immediatamente superiore verrà utilizzata come
> template, ovviamente, la pagina "Negozio"

- **Pagina Specifica**: in queste condizioni sarà possibile indicare,
  selezionandola dal relativo albero delle pagine, la specifica Pagina
  Catalogo che dovrà essere utilizzata come template per la creazione di
  eventuali nuove "Pagine Catalogo Padre".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\generazione_pagine_categoria_3_res.bmp](./assets/media/image6.png)

> Tali pagine assumeranno quindi lo stesso aspetto grafico, e avranno
> esattamente gli stessi componenti della Pagina selezionata all'interno
> dell'albero evidenziato in figura

**Pagina Negozio Foglia:** consente di indicare la specifica pagina del
sito che dovrà essere utilizzata come Template per la creazione di una
NUOVA "Pagina Negozio Foglia".

**ATTENZIONE! Il parametro in oggetto ha effetto solo ed esclusivamente
sulla creazione di NUOVE Pagine Catalogo mentre non influenza o varia in
alcun modo eventuali pagine dello stesso tipo già presenti all'interno
del sito.**

Anche in questo caso è possibile selezionare una delle seguenti opzioni.

- **Pagina Generica:** in queste condizioni eventuali nuove "Pagine
  Catalogo Foglia", generate a seguito della creazione all'interno del
  gestionale di nuove categorie merceologiche, **verranno create
  assumendo come Template la "Pagina Negozio"** (radice di tutte le
  categorie merceologiche).

> Tali pagine assumeranno quindi lo stesso aspetto grafico e avranno
> esattamente gli stessi componenti della pagina Negozio.

- **Pagina Categoria Padre**: in queste condizioni eventuali nuove
  "Pagine Catalogo Foglia", generate a seguito della creazione
  all'interno del gestionale di nuove categorie merceologiche,
  **verranno create assumendo come Template la Pagina Catalogo di
  livello immediatamente superiore.**

> Tali pagine assumeranno quindi lo stesso aspetto grafico, e avranno
> esattamente gli stessi componenti della loro Pagina Padre.
>
> **ATTENZIONE**! Nel caso in cui la Categoria Merceologica in questione
> dovesse essere di primo livello, e non avere quindi nessun padre
> gerarchico di livello immediatamente superiore verrà utilizzata come
> template, ovviamente, la pagina "Negozio"

- **Pagina Specifica**: in queste condizioni sarà possibile indicare,
  selezionandola dal relativo albero delle pagine, la specifica Pagina
  Catalogo che dovrà essere utilizzata come template per la creazione di
  eventuali nuove "Pagine Catalogo Foglia".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\generazione_pagine_categoria_4_res.bmp](./assets/media/image7.png)

> Tali pagine assumeranno quindi lo stesso aspetto grafico, e avranno
> esattamente gli stessi componenti della Pagina selezionata all'interno
> dell'albero evidenziato in figura

**Ovviamente, alla prima sincronizzazione Sito -- Gestionale, l'unico
Template disponibile sarà quello della pagina "Negozio" (non essendo
ancora presente sul sito alcuna categoria merceologica).**

Nel caso in cui l'esigenza dovesse essere quella di creare Pagine
Catalogo con layout differenti ai diversi livelli gerarchici sarà quindi
necessario:

- esportare le categorie merceologiche che dovranno poi essere
  utilizzate come Template

- inserire i componenti desiderati all'interno delle diverse pagine (es.
  "Catalogo Ecommerce" in una Pagina Catalogo Foglia e "Lista Categorie"
  in una Pagina Catalogo Padre)

- impostare correttamente i tre parametri presenti all'interno della
  sezione "**Generazione Pagine di Categoria**" nella maschera di
  configurazione della Variante Sito in cui si sta operando

- esportare tutte le altre Categorie Merceologiche in maniera tale che
  ciascuna di esse possa ora ereditare il layout corretto dal relativo
  Template

**ATTENZIONE!** operando in questo modo diventa di fondamentale
importanza accertarsi che le Pagine Catalogo utilizzate come Template
siano effettivamente sempre presenti all'interno del sito. In caso
contrario la generazione di nuove Pagine Catalogo potrebbe non
rispettare i vincoli inizialmente impostati

**Pagina Prodotto**: consente di indicare sulla base di quale pagina
dovranno essere create nuove Pagine Prodotto generate a seguito della
creazione all'interno del gestionale di nuove categorie merceologiche.

**ATTENZIONE! Il parametro in oggetto ha effetto solo ed esclusivamente
sulla creazione di nuove Pagine Prodotto mentre non influenza o varia in
alcun modo eventuali pagine dello stesso tipo già presenti all'interno
del sito.**

E' possibile selezionare una delle seguenti opzioni.

- **Pagina Generica:** in queste condizioni eventuali nuove Pagine
  Prodotto, generate a seguito della creazione all'interno del
  gestionale di nuove categorie merceologiche, **verranno create
  assumendo come Template la "Pagina Prodotti"** (radice dell'albero
  delle pagine prodotto relative alle diverse categorie gestite
  all'interno del sito).

> Tali pagine assumeranno quindi lo stesso aspetto grafico della pagina
> "Prodotti" oltre ad avere, ovviamente, tutti i componenti presenti in
> questa stessa pagina.

- **Pagina Categoria Padre**: in queste condizioni eventuali nuove
  Pagine Prodotto, generate a seguito della creazione all'interno del
  gestionale di nuove categorie merceologiche, **verranno create
  assumendo come Template la Pagina Prodotto di livello immediatamente
  superiore.**

> Tali pagine assumeranno quindi lo stesso aspetto grafico della loro
> Pagina Padre oltre ad avere, ovviamente, tutti i componenti presenti
> in questa stessa pagina.
>
> **ATTENZIONE!** Nel caso in cui la Categoria Merceologica in questione
> dovesse essere di primo livello, e non avere quindi nessun padre
> gerarchico di livello immediatamente superiore verrà utilizzata come
> template la pagina "Prodotti"
>
> **Per la stessa ragione, ovviamente, alla prima sincronizzazione Sito
> -- Gestionale, l'unico Template disponibile sarà quello della pagina
> "Prodotti" (non essendo ancora presente sul sito alcuna categoria
> merceologica).**

All'interno della sezione "**Parametri Cookie Privacy**", infine, è
possibile decidere se abilitare o meno, per il proprio sito, un apposito
Popup volto ad informare gli utenti relativamente all'utilizzo, da parte
del sito stesso, dei cookies in maniera tale da soddisfare la vigente
normativa Europea in materia (per maggiori informazioni in merito si
vedano anche i successivi capitoli di questo manuale).

Una volta impostati i parametri richiesti, cliccando sul pulsante
"**Salva**", presente nella parte alta della maschera, la nuova Variante
verrà creata e inserita tra quelle presenti in elenco nella Maschera di
Gestione delle Varianti..

La sezione "**Copia Testi**" presente sempre nella parte sinistra della
maschera "Gestione Varianti" consente invece di copiare tutti i testi
attualmente presenti, per la variante indicata all'interno del campo
"**Sorgente**", in "Gestione Testi/Messaggi del Sito", nella
corrispondente sezione della Variante indicata all'interno del campo
"**Destinazione**"

