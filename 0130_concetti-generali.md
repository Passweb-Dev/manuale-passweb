# CONCETTI GENERALI



Prima di passare ad analizzare le diverse componenti dell'ambiente di
sviluppo di Passweb è bene fissare alcuni concetti di fondamentale
importanza che stanno alla base della soluzione in modo tale da
chiarire, anche agli utenti meno esperti, la logica dell'Editing Grafico
e della costruzione di una pagina web.

In linea generale ogni pagina è suddivisa in **Contenitori** e
**Componenti**; i primi definiscono la struttura del sito, mentre i
secondi sono oggetti grafici, più o meno complessi, che l'utente può
inserire all'interno di un Contenitore, come "scatole cinesi". Con
"scatole cinesi" si indica una serie di scatole di grandezza crescente,
che possono essere inserite l\'una nell\'altra in sequenza.

Allo stesso modo possiamo rappresentare i Contenitori, nel caso di
Passweb, come le scatole più grandi che racchiudono il sito e la sua
struttura, mentre le scatole piccole sono i vari Componenti che
contengono a loro volta le scatole più piccole ancora che rappresentano
i Contenuti.

Più genericamente possiamo affermare che il **Contenitore** è tutto ciò
che riguarda la struttura del sito (Corpo Pagina, Riquadro Sito, Colonna
Centrale, ecc) e che contiene i **Componenti**, i quali a loro volta,
proprio come le scatole cinesi, contengono i **Contenuti**.

**La struttura delle scatole è differente ma la personalizzazione
grafica della scatola avverrà sempre nelle medesime modalità**.

Le proprietà grafiche di una scatola sono infatti le stesse, sia che si
tratti di un Contenitore, di un Componente o di un Contenuto e per
intervenire su tali proprietà si utilizza, in Passweb, sempre lo stesso
strumento, il cosiddetto **Style Editor**

A livello tecnico lo Style Editor altro non è se non un editor visuale
per l'impostazione delle proprietà CSS dei vari tag HTML presenti
all'interno della pagina web

![](./assets/media/image2.png)

Si tratterà quindi, molto semplicemente, di selezionare la specifica
scatola su cui intervenire dunque lo specifico Contenitore piuttosto che
lo specifico Componente, aprire lo Style Editor, selezionare,
eventualmente, dal relativo menu a tendina lo specifico Contenuto su cui
intervenire e agire poi sulla specifica proprietà grafica che si
desidera effettivamente modificare (es. dimensione, posizionamento,
allineamento, colore, bordi, sfondo ecc).

![](./assets/media/image3.png)

**ATTENZIONE!** I Contenitori e i Componenti potranno essere selezionati
direttamente all'interno della pagina web dipendentemente dal fatto di
aver abilitato la modalità di gestione dei Contenitori o quella dei
Componenti. Una volta selezionato uno di questi elementi ed aperto lo
Style Editor la scelta dello specifico Contenuto su cui intervenire,
avviene sempre all'interno dell'apposito menu a tendina (filtrabile
mediante l'apposito campo di ricerca)

Una volta selezionato uno di questi Contenuti Passweb evidenzierà il
corrispondente elemento all'interno della pagina web con un apposito
bordo tratteggiato in maniera tale da avere ben chiaro il Contenuto su
cui si andrà effettivamente ad agire.

![](./assets/media/image4.png)

Per maggiori informazioni relativamente all'utilizzo dello Style Editor
si veda anche la sezione *"Live Editing per Varianti Responsive -- Style
Editor (Editing Grafico)"* di questo manuale

Oltre ai Contenitori, ai Componenti e ai Contenuti il Live Editing di
Passweb mette a disposizione dell'utente anche tutta una serie di
funzioni necessarie per gestire ogni singolo aspetto del proprio sito
come ad esempio la creazione e la configurazione delle proprietà di una
nuova pagina web oppure la gestione dei Temi o ancora la creazione e la
gestione di diversi Layout piuttosto che di diverse Varianti.

Ciascuna di queste funzioni è accessibile direttamente dalla
corrispondente voce del menu "**Editing**"

![](./assets/media/image5.png)

