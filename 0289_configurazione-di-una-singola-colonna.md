# CONFIGURAZIONE DI UNA SINGOLA COLONNA



In un contesto responsivo potrebbe non essere sufficiente assegnare alla
griglia uno schema fisso di colonne. Tipicamente, anzi, l'esigenza è
proprio quella di andare a dire, in qualche modo, come lo schema di base
dovrà modificarsi al variare della larghezza del dispositivo di
visualizzazione del sito.

Una volta inserito all'interno della griglia lo schema di base, sarà
quindi necessario andare a configurare ogni singola colonna
assegnandogli il corretto dimensionamento e la corretta visibilità in
relazione alle diverse risoluzioni del dispositivo di visualizzazione
utilizzato.

In questo senso cliccando sull'icona "**Contenuto e Configurazione**"
presente sul R.O.C. di ogni singola colonna della griglia verrà aperta
**la sua maschera di gestione e configurazione** suddivisa in varie
sezioni

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\colonna_configurazione.bmp](./assets/media/image107.png)

Come al solito all'interno della sezione "**Dati Componente**" sarà
possibile settare i principali parametri di configurazione della
colonna.

Nello specifico il campo:

- **Nome:** (obbligatorio) consente di gestire il nome identificativo
  della Colonna in esame. Considerando che la colonna è stata inserita
  in maniera automatica sulla base di un certo schema stabilito in
  precedenza, in questo campo verrà visualizzato, inizialmente, il nome
  assegnato alla colonna da Passweb stesso.

> L'utente ha comunque la facoltà di variare tale nome come e quando
> vuole.

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

All'interno della sezione **"Avanzate e Animazioni**" è invece
possibile, come per un qualsiasi altro componente Passweb, impostare,
tra le altre cose, la visibilità della colonna in oggetto in relazione
allo specifico dispositivo in cui verrà poi visualizzato il sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visibilita_colonna.bmp](./assets/media/image108.png)

La sezione "**Gestione Contenuti**" consente infine di impostare **il
dimensionamento della colonna** in relazione alle diverse risoluzioni
dei dispositivi di visualizzazione utilizzati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\colonna_gestione_contenuti.bmp](./assets/media/image109.png)

In particolare per ogni tipologia di dispositivo gestita (dispositivi
extra large, large, medium, small ed extra small) è possibile indicare
un valore per i seguenti parametri:

- **Larghezza:** consente di indicare, secondo la solita convenzione, il
  numero di sezioni che la colonna in esame dovrà andare ad occupare
  all'interno della riga in corrispondenza di quella specifica tipologia
  di dispositivo.

> **ATTENZIONE!** Il valore presente all'interno di questo campo per
> dispositivi Extra Large coincide, inizialmente, con quello assegnato
> alla colonna stessa in fase di definizione dello schema base.
>
> Oltre allo specifico dimensionamento della colonna, selezionabile da
> un apposito menu a tendina, è possibile inoltre, per tutte le
> tipologie di dispositivi ad eccezione di quelli extra large, impostare
> il campo Larghezza anche sul valore "**Eredita dal dispositivo più
> piccolo impostato, 12/12 altrimenti**"
>
> Il risultato che otterremo selezionando, laddove possibile, questa
> opzione, sarà quello di ereditare per la colonna in esame in
> corrispondenza di quella specifica tipologia di dispositivo, lo stesso
> dimensionamento impostato per il dispositivo di visualizzazione
> immediatamente più piccolo.
>
> Nel caso in cui non esistano dispositivi più piccoli di quello
> considerato con impostato uno specifico dimensionamento, il risultato
> sarà quello di dimensionare la colonna in esame a 12/12 attribuendole
> quindi la larghezza dell'intera riga
>
> **[ESEMPIO]{.underline}**
>
> Se la nostra esigenza dovesse quindi essere, ad esempio, quella di
> ottenere una griglia a 3 colonne affiancate su di una stessa riga in
> corrispondenza di risoluzioni maggiori di 1200 px che si linearizza
> disponendo queste stesse colonne una sotto l'altra in corrispondenza
> di risoluzioni minori a 768px sarà necessario impostare il parametro
> Larghezza di ciascuna di queste colonne come di seguito indicato:
>
> **DISPOSITIVI EXTRA LARGE \> = 1200px**
>
> Larghezza = 4/12
>
> (valore derivante dalla configurazione dello schema base di colonne
> inserito in fase iniziale all'interno della griglia)
>
> **DISPOSITIVI LARGE \>= 992 px e \< 1200px**
>
> Larghezza = Eredita dal dispositivo più piccolo impostato, 12/12
> altrimenti
>
> (valore ereditato dai dispositivi medium)
>
> **DISPOSITIVI MEDIUM \>= 768 e \< 992 px**
>
> Larghezza = 4/12
>
> (valore fissato)
>
> **DISPOSITIVI SMALL \>= 576 e \< 768 px**
>
> Larghezza = Eredita dal dispositivo più piccolo impostato, 12/12
> altrimenti
>
> (valore ereditato dai dispostivi extra small)
>
> **DISPOSITIVI EXTRA SMALL \<= 576 px**
>
> Larghezza = Eredita dal dispositivo più piccolo impostato, 12/12
> altrimenti
>
> (non essendoci dispositivi più piccoli con impostato uno specifico
> dimensionamento la colonna sarà dimensionata a 12/12)

- **Offset Sinistro:** consente di assegnare o meno alla colonna in
  esame un margine sinistro automatico. E' possibile selezionare uno dei
  seguenti valori:

  - **SI:** selezionando questa opzione verrà assegnato alla colonna in
    esame, in corrispondenza di quella specifica tipologia di
    dispositivo, un margine sinistro automatico, allineando di
    conseguenza questa stessa colonna, e tutte quelle che vengono dopo
    di lei, sulla parte destra della griglia

  - **Eredita dal dispositivo più piccolo impostato:** in queste
    condizioni il valore del parametro verrà ereditato da quello
    impostato per lo stesso parametro nel dispositivo di visualizzazione
    immediatamente più piccolo.

> Nel caso in cui non esistano dispositivi più piccoli di quello
> considerato per i quali il parametro in oggetto sia stato impostato a
> SI alla colonna non verrà ovviamente assegnato nessun offset sinistro

- **Offset Destro:** consente di assegnare o meno alla colonna in esame
  un margine destro automatico. E' possibile selezionare uno dei
  seguenti valori:

  - **SI:** selezionando questa opzione verrà assegnato alla colonna in
    esame, in corrispondenza di quella specifica tipologia di
    dispositivo, un margine destro automatico, allineando di conseguenza
    questa stessa colonna, e tutte quelle che vengono prima di lei,
    sulla parte sinistra della griglia

  - **Eredita dal dispositivo più piccolo impostato:** in queste
    condizioni il valore del parametro verrà ereditato da quello
    impostato per lo stesso parametro nel dispositivo di visualizzazione
    immediatamente più piccolo.

> Nel caso in cui non esistano dispositivi più piccoli di quello
> considerato per i quali il parametro in oggetto sia stato impostato a
> SI alla colonna non verrà ovviamente assegnato nessun offset destro

Ovviamente l'applicazione tanto di un offset destro quanto di un offset
sinistro potrà avere un senso solo nel momento in cui le colonne
presenti in griglia siano state configurate in maniera tale da non
occupare l'intera larghezza della riga (ossia tutte e 12 le sezioni in
cui la riga stessa è divisa)

**ATTENZIONE! Nel momento in cui ad una data colonna dovesse essere
assegnato sia un offset destro che un offset sinistro la colonna stessa
si posizionerà esattamente al centro dello spazio disponibile
all'interno della griglia**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\colonna_offset.bmp](./assets/media/image110.png)

