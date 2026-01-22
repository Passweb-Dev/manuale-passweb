# PARAMETRI IMMAGINI



La pagina **"Parametri Immagini"** accessibile dalla voce di menu
***"Catalogo -- Configurazione Parametri Catalogo"*** consente di
impostare le dimensioni e la qualità delle immagini articolo e delle
immagini di categoria in uso all'interno del sito, sia per la versione
desktop che per la versione mobile.

**ATTENZIONE!** Al fine di ottimizzare le prestazioni del sito si
consiglia di indicare sempre, laddove possibile, una dimensione
specifica anche per le immagini mobile, immagini queste che verranno poi
effettivamente utilizzate in corrispondenza di risoluzioni inferiori ai
575px

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_tipologie_immagini.bmp](./assets/media/image42.png){width="5.604166666666667in"
height="3.33125in"}

**[LISTA DELLE TIPOLOGIE IMMAGINI NEL CATALOGO]{.underline}**

All'interno di questa sezione è possibile impostare dimensioni e qualità
per le seguenti tipologie di immagine:

- **Immagine del catalogo**: immagine utilizzata all'interno di
  componenti quali il Catalogo Ecommerce, Offerte / Novità, Popolarità
  Prodotto, Abbinati Ecommerce ...

- **Immagine principale della scheda prodotto**: è l'immagine che verrà
  considerata come immagine principale all'interno della scheda prodotto
  (solitamente è quella per la quale vengono impostate le dimensioni
  maggiori).

- **Immagini secondarie della scheda prodotto:** sono le immagini che
  verranno considerate come immagini secondarie all'interno della scheda
  prodotto.

- **Immagine del catalogo su dispositivi mobile:** immagine catalogo in
  uso all'interno di dispositivi mobile (per risoluzioni inferiori ai
  768px)

- **Immagine principale della scheda prodotto su dispositivi mobile:**
  immagine principale della scheda prodotto in uso all'interno di
  dispositivi mobile (per risoluzioni inferiori ai 768px)

- **Immagini secondarie della scheda prodotto su dispositivi mobile:**
  immagine secondaria della scheda prodotto in uso all'interno di
  dispositivi mobile (per risoluzioni inferiori ai 768px)

Per maggiori informazioni relative a come distinguere ed identificare
l'immagine del catalogo rispetto alle immagini (principale e secondarie)
della scheda prodotto, si veda il successivo capitolo di questo manuale
"*Associazione delle Immagini e delle Schede Tecniche Articolo
all'interno del gestionale*".

Selezionando una delle tipologie di immagini presenti in elenco, il
pulsante "**Modifica**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image43.png){width="0.3958333333333333in"
height="0.18819444444444444in"} ) posto nella contestuale barra degli
strumenti, consentirà di accedere alla maschera **"Configurazione
Immagine"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_immagine.bmp](./assets/media/image44.png){width="5.604166666666667in"
height="3.5256944444444445in"}

all'interno della quale poter gestire i relativi parametri di
configurazione:

- **Altezza / Larghezza:** consente di indicare l'altezza / larghezza in
  pixel che dovrà assumere la relativa immagine

> Indicando dei valori specifici per l\'altezza e per la larghezza,
> l'immagine verrà ridimensionata in maniera completamente automatica da
> Passweb attraverso uno specifico algoritmo di ridimensionamento in
> modo tale da ottenere un\'immagine dalle dimensioni indicate e che
> mantenga comunque il più possibile le caratteristiche dell\'immagine
> originale
>
> **ATTENZIONE!** se il ridimensionamento è volto ad ottenere un
> immagine più piccola, non ci sarà perdita di qualità; al contrario se
> il ridimensionamento è finalizzato ad ottenere un\'immagine più grande
> di quella di partenza il processo potrebbe portare ad una
> significativa perdita di qualità dell\'immagine

- **Qualità:** valore numerico da 0 a 100. Consente di impostare la
  qualità con cui dovrà essere ricampionata la relativa immagine durante
  il processo di importazione.

> **ATTENZIONE! Un'alta qualità dell'immagine aumenta di conseguenza il
> peso della stessa. Con qualità pari a 100 il peso dell'immagine
> ricampionata dalla procedura di importazione potrebbe anche essere
> superiore a quello del file originale**
>
> Impostando una qualità pari a 0 il processo di ricampionamento verrà
> gestito in automatico da Passweb cercando di trovare un compromesso
> ottimale tra qualità e peso dell'immagine. Lasciando il campo vuoto
> non viene fatto nessun ricampionamento (sarà come impostare qualità =
> 100).

- **Immagine Watermark:** consente di indicare (selezionandola tra le
  risorse già presenti all'interno del sito) l'immagine da applicare
  come watermark alla relativa immagine articolo

- **Allineamento verticale / orizzontale:** consente di definire il
  posizionamento (verticale / orizzontale) che dovrà assumere lil
  watermark rispetto alla corrispondente immagine articolo

- **Immagine preview:** consente di selezionare un'immagine tra quelle
  presenti in gestione risorse cui applicare il watermark in maniera
  tale da ottenere una preview del risultato che si andrà poi ad
  ottenere nel momento in cui si dovesse decidere di applicare
  effettivamente il watermark a tutte le immagini articolo della
  tipologia indicata

> Per visualizzare la preview è sufficiente cliccare sul pulsante
> "**Visualizza l'anteprima del watermark**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_immagine_2.bmp](./assets/media/image45.png){width="5.604166666666667in"
height="3.5256944444444445in"}

Il pulsante "**Salva**" posto nella parte bassa della maschera consente
di applicare le impostazioni settate avviando quindi la procedura di
applicazione del Watermark e quella di ridimensionamento delle immagini.

Nel momento in cui l'esigenza dovesse essere quella di rimuovere un
eventuale watermark precedentemente applicato, sarà sufficiente
eliminare l'Immagine Watermark (cliccando sul pulsante raffigurante una
piccola X) e cliccare poi sul pulsante "Salva"

Ovviamente, una volta impostata un'immagine watermark questa verrà poi
applicata automaticamente anche ad eventuali nuove immagini articolo
importate in fase di sincronizzazione

**ATTENZIONE! Il Watermark verrà applicato solo ed esclusivamente alle
immagini rielaborate da Passweb mantenendo inalterate le immagini
originali.**

In conseguenza di ciò le immagini inserite nella pagina web (quelle
effettivamente indicizzabili) saranno, eventualmente, dotate di
Watermark, mentre all'interno della galleria delle immagini prodotto
continueranno ad essere visualizzate le risorse originali prive di
Watermark.

Il fatto conservare inalterate le immagini originali, oltre a limitare
l'occupazione su disco, consentirà a Passweb di poter effettuare tutte
le rielaborazioni del caso (ridimensionamenti, eliminazione e/o
applicazione di un nuovo Watermark ...) potendo partire sempre dalle
risorse originali di ogni singolo prodotto

Se l'esigenza dovesse essere quindi quella di applicare un Watermark
anche alle immagini originali, sarà necessario operare esternamente a
Passweb creando ed importando all'interno del sito immagini già marcate
con un Watermark.

**[IMMAGINE CATALOGO DI DEFAULT]{.underline}**

La sezione "**Immagine Catalogo di Default**" consente invece di
impostare, selezionandola tra quelle disponibili all'interno del sito
(pulsante "**Scegli file**"), l'immagine che dovrà essere utilizzata
come immagine articolo (sia nel catalogo che nella scheda prodotto) nel
momento in cui a quello stesso prodotto non dovesse essere stata
associata una specifica risorsa (tipicamente è l'immagine "foto non
disponibile").

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\immagine_catalogo_default.bmp](./assets/media/image46.png){width="5.207638888888889in"
height="3.3180555555555555in"}

I due pulsanti visualizzati in corrispondenza di questo campo, una volta
caricata l'immagine, consentiranno rispettivamente di effettuare il
download della stessa (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_download_img_default.bmp](./assets/media/image47.png){width="0.2923611111111111in"
height="0.2534722222222222in"} ) e di eliminarla (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_img_default.bmp](./assets/media/image48.png){width="0.2791666666666667in"
height="0.22708333333333333in"} )

**[LISTA DELLE TIPOLOGIE DI IMMAGINI DI CATEGORIA]{.underline}**

La sezione "**Lista delle tipologie di immagini di Categoria**" consente
di impostare quella che dovrà essere la qualità e la dimensione da
utilizzare, per le immagini di categoria merceologica, su dispositivi
mobile (risoluzioni inferiori ai 575px)

Anche in questo caso dunque il pulsante "**Modifica**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image43.png){width="0.3958333333333333in"
height="0.18819444444444444in"} ) posto nella contestuale barra degli
strumenti, consentirà di accedere alla relativa maschera di
**"Configurazione Immagine"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_immagini_categoria_mobile.bmp](./assets/media/image49.png){width="5.604166666666667in"
height="3.5256944444444445in"}

all'interno della quale poter impostare i parametri di configurazione.

Una volta impostati questi parametri il pulsante "**Salva**", posto
nella parte bassa della maschera, consentirà di applicare le
impostazioni settate avviando quindi la relativa procedura di
ridimensionamento e conversione delle immagini.

**ATTENZIONE!** I parametri impostati all'interno di questa maschera
avranno effetto solo ed esclusivamente sulle immagini di categoria
utilizzate all'interno del componente "**Lista Categorie**". In questo
senso non verranno quindi considerate le eventuali immagini utilizzate
all'interno del componente "Menu di Categoria"

**[IMMAGINE CATEGORIA DI DEFAULT]{.underline}**

La sezione "**Immagine Categoria di Default**" consente di impostare,
selezionandola tra quelle disponibili all'interno del sito (pulsante
"**Scegli file**"), l'immagine che dovrà essere utilizzata all'interno
del componente "**Lista Categorie**", come immagine di default nel caso
in cui alla relativa categoria merceologica non sia stata assegnata una
specifica risorsa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\immagine_categoria_default.bmp](./assets/media/image50.png){width="5.207638888888889in"
height="3.3180555555555555in"}

I due pulsanti visualizzati in corrispondenza di questo campo, una volta
caricata l'immagine, consentiranno rispettivamente di effettuare il
download della stessa (
![Videate\\pulsante_download_img_default.bmp](./assets/media/image51.png){width="0.2923611111111111in"
height="0.2534722222222222in"} ) e di eliminarla (
![Videate\\pulsante_elimina_img_default.bmp](./assets/media/image52.png){width="0.2791666666666667in"
height="0.22708333333333333in"} )

