# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_quickview_configurazione_res.bmp](./assets/media/image64.png){width="4.98125in"
height="3.01875in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di definire un nome per il Componente che si sta
editando

**Pubblico** (selezionato a default): consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione**: consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Testo Bottone:** consente di indicare il testo o l'immagine da
utilizzare per il pulsante di apertura della finestra modale all'interno
della quale verrà poi visualizzato il dettaglio del relativo articolo.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Anche il Componente "Quick View", al pari di altri componenti
precedentemente esaminati **può essere considerato a tutti gli effetti
come un "Componente di tipo Contenitore".**

Sarà quindi possibile inserire al suo interno tutta una serie di campi
necessari per poter definire che tipo di informazioni, Mexal e non,
dovranno essere visualizzate per lo specifico articolo. Tali campi, in
ogni caso, per poter esser gestiti liberamente, dovranno inevitabilmente
esser trattati a loro volta come Componenti autonomi editabili
singolarmente.

Una volta inserito quindi il Componente "Quick View" per poterlo poi
personalizzare sarà necessario, attivare la modalità di gestione dei
componenti, portarsi sul Componente in esame e, alla comparsa del R.O.C.
cliccare sull'icona "**Accedi ai componenti interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Quick View" sarà
possibile inserire solamente tre diversi componenti mediante i quali
poter suddividere la finestra modale in tre distinte sezioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\quickview_aggiunta_componenti_res.bmp](./assets/media/image65.png){width="2.8097222222222222in"
height="2.828472222222222in"}

- **Quick View Header:** consente di inserire all'interno della finestra
  di quick view un contenitore per gestire le informazioni in testata

- **Quick View Body:** consente di inserire all'interno della finestra
  di quick view un contenitore per gestire le informazioni di corpo

- **Quick View Footer:** consente di inserire all'interno della finestra
  di quick view un contenitore per gestire le informazioni da collocare
  all'interno del piede

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Ecommerce interni al componente "Quick View" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti E-Commerce -- Componenti Interni ai
> Componenti Ecommerce).

L'inserimento di questi componenti all'interno del Componente "Quick
View" avviene utilizzando le solite tecniche di interazione con l'editor
(Drag and Drop o Point and Click) già esaminate all'interno di questo
manuale (per maggiori informazioni si rimanda allo specifico capitolo di
questo manuale).

**ATTENZIONE!** Almeno uno tra i tre componenti sopra indicati dovrà
essere necessariamente inserito nella finestra di quick view

**E' infatti all'interno dei componenti "Quick View Header" , "Quick
View Body", "Quick View Footer" che andranno poi inseriti le
informazioni Ecommerce (Titolo, Descrizione, Immagine ecc ...)
necessarie per costruire la scheda di dettaglio del relativo articolo**

In particolare come già per i Contenitori Collassabili, anche in questo
caso, inizialmente, i contenuti del componente Quick View non saranno
visibili all'interno della pagina web (e questo non solo sul front end
del sito ma anche all'interno del back end).

**Per poterli gestire sia dal punto di vista grafico che, soprattutto,
dal punto di vista dei loro contenuti, e quindi degli ulteriori elementi
da inserire all'interno della finestra di quick view, la prima cosa da
fare sarà ovviamente quella di richiamare questa stessa finestra
cliccando sul relativo pulsante di apertura esattamente come farebbe sul
front end un normale visitatore del sito.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\quick_view_gestione.bmp](./assets/media/image66.png){width="4.98125in"
height="3.509027777777778in"}

**ATTENZIONE!** la visualizzazione della finestra di quick view
all'interno dell'ambiente di sviluppo è leggermente diversa rispetto a
quella che sarà poi la visualizzazione di questo stesso elemento sul
front end del sito.

In effetti mentre sul front end del sito il quick view verrà aperto
all'interno di un'apposita finestra modale, **all'interno dell'ambiente
di sviluppo, verrà visualizzato sempre e soltanto al di sotto del
pulsante di apertura** in maniera tale da poter poi inserire in esso
ulteriori componenti utilizzando le solite modalità di interazione
proprie di Passweb.

In queste condizioni, per avere un'idea chiara soprattutto del
dimensionamento dei vari elementi, si consiglia sempre di controllare il
risultato finale sul front end del sito.

Una volta richiamata la finestra di quick view all'interno della pagina
sarà poi possibile gestirla, sia a livello grafico che a livello di
contenuti, secondo le normali modalità di interazione proprie di
Passweb.

