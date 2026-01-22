# HTML5 -- TAG SEMANTICI



Per poter comprendere al meglio il significato e l'utilizzo dei tag
semantici, implementabili in un sito Passweb mediante l'utilizzo del
Componente Contenitore, occorre innanzitutto considerare come l'avvento
di HTML5 abbia introdotto un set di nuovi elementi, non presenti in
HTML4, che rendono più semplice la definizione della struttura di una
pagina web.

Cerchiamo di comprendere meglio questo concetto.

La maggior parte delle pagine scritte in HTML4 contiene, generalmente,
una serie di elementi strutturali piuttosto comuni come header, footer e
colonne ed è una prassi piuttosto comune quella di definire questi
elementi strutturali nel markup HTML della pagina, utilizzando tag div e
assegnando a ciascuno di essi uno specifico id e/o una specifica classe
descrittiva.

Di seguito viene riportata l'immagine di quella che potrebbe essere la
struttura di una pagina HTML4 realizzata utilizzando un layout a due
colonne.

![](./assets/media/image1.png)

Come si può facilmente osservare, dal punto di vista strutturale una
pagina che adotta questo tipo di layout è costituita da un header
(intestazione), un footer (piede), una barra orizzontale di navigazione
posta immediatamente al di sotto dell'intestazione e un area centrale
utilizzata per gestire i contenuti principali della pagina.

Quest'area centrale è costituita a sua volta da un contenitore delle
colonne e da due colonne interne (colonna_sinstra e colonna_destra)
utilizzate rispettivamente per gestire, ad esempio, i post di un
ipotetico blog e una barra laterale con elementi collegati in qualche
modo ai contenuti della precedente colonna (es. elementi di filtraggio
dei post del blog).

Ognuno di questi elementi strutturali è realizzato utilizzando un tag
div con specifici attributi id o class utilizzati, tra le altre cose,
anche per identificare il tipo di contenuti che verranno poi gestiti
all'interno di queste stesse div.

Anche Passweb, in perfetto accordo con le più comuni prassi HTML4,
utilizza, per generare il markup delle proprie pagine web, una struttura
di questo tipo lasciando all'utente la possibilità di configurare lo
specifico layout che intende utilizzare, decidendo quali contenitori
strutturali (testata alta, testa media, colonna centrale ecc...)
abilitare o meno.

In ogni caso tutti questi contenitori strutturali sono realizzati, a
livello di markup, mediante apposite div.

![](./assets/media/image2.png)

L'uso del generico tag div è così diffuso perché in HTML4 non esistono
specifici tag semantici che possano identificare e descrivere in maniera
chiara le diverse parti di una pagina web e i contenuti in esse
presenti, per cui, come detto, si tende ad utilizzare sempre il tag div
(o al limite dei tag span) demandando l'identificazione della tipologia
dei loro contenuti agli attributi id e/o class.

HTML5, al contrario del suo predecessore, gestisce questa problematica
in maniera diversa introducendo, come inizialmente evidenziato, tutta
una serie di nuovi tag semantici in grado di identificare essi stessi le
diverse sezioni di una pagina web e i contenuti in esse presenti (senza
dover quindi ricorrere a specifici attributi).

Il layout a due colonne appena esaminato potrebbe ora essere tradotto in
HTML5 come di seguito indicato

![](./assets/media/image3.png)

Come si può facilmente osservare le diverse sezioni della pagina sono
ora identificate da specifici tag e il corrispondente markup potrebbe
quindi essere del tipo di quello indicato in figura.

![](./assets/media/image4.png)

L'utilizzo di questi tag semantici può portare ad ottenere diversi
vantaggi, in termini di pulizia ed ordine del codice della pagina web,
in termini di tecnologie assistive e anche, ovviamente, in termini SEO e
di indicizzazione delle varie pagine.

In questo senso in particolare il problema di utilizzare solo ed
esclusivamente dei div è sempre lo stesso ossia che il tag div in se è
privo di qualsiasi significato, non aggiunge valore semantico alla
pagina ne tanto meno aiuta a contestualizzare i contenuti di ciò che
viene poi inserito al suo interno. I tag semantici, al contrario,
possono permettere ai motori di ricerca di fare il crawl di un sito
ignorando, ad esempio, alcune sezioni della pagina, come possono essere
quelle racchiuse dai tag header o footer, o al limite di utilizzare i
contenuti di queste sezioni per scopi di indicizzazione differenti (come
ad esempio identificare informazioni sul copyright o scoprire il nome o
il logo del sito).

In questo modo l'indicizzazione effettuata dal motore di ricerca sarà
indubbiamente molto più efficiente e piena di significato. Considerando
infine l'importanza sempre crescente che Google stesso assegna alla
semantica di una pagina web e alla pertinenza dei vari contenuti
presenti all'interno della varie sezioni è semplice comprendere i
benefici che si potranno ottenere, soprattutto in ottica futura,
identificando le specifiche sezioni delle proprie pagine mediante questi
tag semantici.

Riportando ora tutto questo discorso in ambito Passweb, occorre
considerare, per prima cosa, che **quelli che per Passweb sono i
cosiddetti "Contenitori Strutturali" della pagina, attivabili o meno
attraverso le apposite funzioni della gestione layout, saranno sempre
realizzati mediante tag div e identificati in maniera specifica
attraverso appositi attributi id (es. div id = "topHeader" ).**

Questo di per se non rappresenta un problema perché non è a questo
livello che si rende necessario assegnare, in Passweb, un valore
semantico allo specifico tag. Ogni singolo Contenitore Strutturale delle
pagine generate da Passweb può essere infatti utilizzato dall'utente
come meglio crede.

In altri termini non è detto, ad esempio, che il Contenitore Strutturale
identificato da Passweb in fase di creazione della pagina web come
"Piede" (div id="footer") debba essere a tutti i costi il piede della
pagina e contenere quindi solo ed esclusivamente informazioni tipiche
del corrispondente tag HTML5 "footer".

Per assurdo si potrebbe realizzare un layout di pagina dove l'unico
Contenitore Strutturale effettivamente attivo è proprio quello che il
layout di Passweb identifica come "Piede". Al suo interno potrebbero
quindi essere inserite tutte le diverse tipologie di contenuto della
pagina web partendo da quelli tipicamente inseriti nella testata di una
pagina (e che dovrebbero essere identificati in HTML5 con il tag
header), passando per il menu di navigazione (che dovrebbe essere
identificato dal tag nav) e finendo con i contenuti principali della
pagina (identificati ad esempio da tag article, section o aside)

**In quest'ottica dunque i tag semantici vanno utilizzati, in Passweb,
in base ai diversi Componenti e ai relativi Contenuti effettivamente
inseriti nei diversi Contenitori Strutturali.**

**Questo lo si può fare racchiudendo gli specifici componenti ed i
relativi contenuti all'interno di un "Componente Contenitore" più
esterno per il quale è effettivamente possibile decidere lo specifico
tag che dovrà essere utilizzato nella sua creazione.**

Supponiamo ad esempio di gestire in Passweb un layout che preveda
l'utilizzo di due soli contenitori strutturali:

- Testata Alta

- Colonna Centrale

In Testata Alta oltre ai classici elementi di "intestazione" del sito,
come logo e/o nome, dovremo inserire anche il menu di navigazione ,
mentre in Colonna Centrale saranno gestiti tutti i contenuti principali
della pagina web e quelli relativi a copyright, termini di licenza,
privacy policy ecc....

In queste condizioni, per assegnare il corretto valore semantico ai
diversi elementi del sito dovremo utilizzare:

- In Testata Alta **due distinti Componenti Contenitore**, il primo
  configurato in maniera tale che venga generato con un tag **header**

![](./assets/media/image5.png)

> il secondo configurato invece in maniera tale che venga generato con
> un tag **nav**

![](./assets/media/image6.png)

> All'interno del primo contenitore andremo poi ad inserire Componenti
> Immagine e/o Paragrafo mediante i quali inserire il logo ed il nome
> del sito.
>
> All'interno del secondo contenitore andremo invece ad inserire un
> Componente Menu mediante il quale gestire il menu di navigazione del
> sito

- In Colonna Centrale dovremo invece utilizzare, dipendentemente dai
  contenuti da gestire, Componenti Contenitori distinti configurati in
  maniera tale da essere generati ad esempio con tag article o section
  e, sicuramente anche un Componente Contenitore configurato in maniera
  tale da essere generato con un tag footer (all'interno del quale
  andranno poi inseriti componenti Paragrafo o menu da utilizzare per
  gestire i footer link, le informazioni di privacy, di copyright
  ecc...)

**In questo modo ogni singola sezione della pagina sarà effettivamente
identificata, anche a livello semantico, dal corretto tag HTML5 coerente
con i contenuti effettivamente presenti all'interno di quella stessa
sezione**

Per maggiori informazioni relativamente alla gestione del Componente
Contenitore si veda anche la sezione *"Live Editing -- Lista Componenti
Comuni -- Componente Contenitore"* di questo manuale

Una volta compresa la filosofia che sta alla base dell'utilizzo dei tag
semantici e come poter implementare questi stessi tag all'interno di un
sito Passweb, vediamo ora nel più nel dettaglio il significato di
ciascuno di essi in maniera tale da aver ben chiaro, ad esempio, quando
utilizzare un tag header piuttosto che un tag nav.

