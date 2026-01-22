# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image18.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico.

Ovviamente nel momento in cui si dovesse decidere di staticizzare questo
tipo di componente per fare in modo che vengano poi visualizzate
eventuali nuove categorie inserite dal back end del sito sarà necessario
rigenerare il codice HTML del componente

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Tipo di Stili applicati al Menu:** consente di impostare la tipologia
di menu da utilizzare specificandone dunque lo stile di visualizzazione.
E' possibile selezionare uno tra i seguenti valori.

- **Flottante Orizzontale:** selezionando questo valore verranno
  visualizzate, in orizzontale, soltanto le voci di menu di primo
  livello. Eventuali sotto-voci verranno visualizzate al passaggio del
  mouse sulle voci di livello superiore.

- **Flottante Verticale:** selezionando questo valore verranno
  visualizzate, in verticale, soltanto le voci di menu di primo livello.
  Eventuali sotto-voci verranno visualizzate al passaggio del mouse
  sulle voci di livello superiore.

- **Lista:** selezionando questo valore verranno sempre visualizzate
  tutte le voci di menu (indipendentemente dal loro livello di
  appartenenza).

> **Per sua stessa natura le voci di questo menu potranno essere
> disposte solo ed esclusivamente in Verticale.**

- **Off Canvas:** selezionando questa opzione il menu verrà posizionato
  al di fuori della pagina web dove invece comparirà soltanto un
  pulsante utile a richiamarlo.

> I successivi parametri consentono poi di decidere dove e come dovrà
> essere visualizzato il menu nel momento in cui un utente dovesse
> richiamarlo cliccando sull'apposito pulsante.

![](./assets/media/image19.png)

> Nello specifico dunque il parametro:

- **Posizionamento del menu:** consente di indicare la posizione in cui
  dovrà essere visualizzato il menu nel momento in cui l'utente dovesse
  decidere di richiamarlo. E' possibile decidere di visualizzarlo sulla
  parte sinistra / destra oppure nella parte alta / bassa della pagina
  stessa

- **Sposta il contenuto del sito all'apertura del menu:** se selezionato
  nel momento in cui l'utente dovesse decidere di richiamare il menu,
  questo verrà visualizzato facendo scorrere la parte restante della
  pagina web verso sinistra/destra/alto/basso dipendentemente dalle
  impostazioni settate per il precedente parametro.

> Nel caso in cui il parametro in oggetto non venga selezionato, il menu
> verrà invece visualizzato andando a sovrapporsi ai contenuti della
> pagina lasciando comunque una porzione della pagina stessa sempre
> visibile.

- **Immagine per Off canvas:** consente di indicare la specifica
  immagine da utilizzare per il pulsante di apertura del menu (l'unico
  elemento visualizzato inizialmente all'interno della pagina web).

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![Videate\\icona_menu_offcanvas.bmp](./assets/media/image14.png)

- **TreeView (apertura sottovoci al click del mouse):** selezionando
  questa opzioni il menu verrà costruito visualizzando soltanto le voci
  di menu di primo livello. Eventuali sottovoci verranno visualizzate
  (nascoste) al click del mouse sull'apposita icona di apertura
  (chiusura) presente a fianco di ciascuna voce che presenti almeno una
  voce di livello inferiore.

In questo caso sarà inoltre possibile specificare un valore per i
seguenti parametri:

![](./assets/media/image20.png)

- **Immagine Controllo Apri/Chiudi Ramo:** consente di selezionare una
  specifica immagine da poter utilizzare per il controllo di apertura /
  chiusura delle sottovoci.

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.
>
> Nel caso in cui non venga specificata nessun immagine il controllo di
> apertura delle sottovoci sarà rappresentato da un **\[+\]** e quello
> di chiusura da un **\[-\].**

- **Gestione del ramo al click sulla voce:** consente di specificare
  quale dovrà essere il comportamento del menu nel momento in cui
  l'utente cliccherà su una voce che ha anche delle sottovoci di livello
  inferiore.

> E' possibile selezionare uno dei seguenti valori:

- **Indirizzamento alla pagina:** in queste condizioni cliccando sulla
  voce di menu l'utente verrà ricondotto alla pagina indicata nel link
  di collegamento associato alla voce stessa

- **Apertura/Chiusura del ramo:** in queste condizioni cliccando sulla
  voce di menu si apriranno/chiuderanno le sottovoci senza effettuare
  alcun cambiamento di pagina

- **Apertura/Chiusura del ramo e Indirizzamento alla pagina:** in queste
  condizioni cliccando sulla voce di menu si apriranno/chiuderanno le
  sottovoci e l'utente verrà anche ricondotto alla pagina indicata nel
  link di collegamento associato alla voce stessa

<!-- -->

- **Chiusura dei rami al medesimo livello:** selezionando questo
  parametro, in fase di apertura di una voce del menu verranno
  automaticamente chiuse tutte le voci dello stesso livello attualmente
  aperte. Nel caso in cui il parametro in questione non venga
  selezionato sarà invece possibile mantenere aperte contemporaneamente
  più voci di menu dello stesso livello

**Tipo di Stili applicati al Menu per dispositivi mobili \< 992px:**
visibile solo nel caso in cui il precedente parametro non sia stato
impostato sull'opzione Off Canvas

Consente di indicare la tipologia di menu che dovrà essere utilizzata
nel momento in cui il dispositivo di visualizzazione del sito dovesse
avere una larghezza inferiore ai 992px.

In questo senso è possibile decidere di utilizzare un menu a **Lista**,
un menu **Off Canvas** oppure (parametro "**Non Visualizzare**")
mantenere esattamente la stessa tipologia di menu utilizzata anche per
dispositivi di visualizzazione del sito con larghezza maggiore o uguale
a 992px

**ATTENZIONE!** Grazie al parametro "**Tipo di Stili applicati al Menu
per dispositivi mobili \< 992px"** è possibile cambiare dinamicamente la
tipologia di menu utilizzata in base alla larghezza del dispositivo di
visualizzazione del sito senza dover per forza di cose realizzare due
differenti menu con le relative opzioni di visualizzazione.

**Profondità:** consente di impostare il livello di profondità per la
visualizzazione delle voci di menu. Impostando ad esempio questo campo
sul valore 3 verranno visualizzate (nella maniera specificata dal
precedente parametro "Tipo di Stili applicati al menu") le voci di primo
secondo e terzo livello

**Categoria Radice:** consente di specificare, selezionandola dal
sottostante albero delle categorie, la specifica categoria di News che
dovrà essere considerata come radice del menu. Tutte le categorie poste
al di sotto di quella selezionata come "Categoria Radice" verranno
visualizzate all'interno del relativo menu come voci di primo livello.

> **NOTA BENE:** nel caso in cui si desideri realizzare un menu di
> categorie contenente tutte le categorie di News presenti all'interno
> del sito, sarà quindi necessario selezionare come Categoria Radice la
> voce "Categorie CMS"

**Pagina di Destinazione per l'Archivio News:** come precedentemente
evidenziato, nel momento in cui un utente dovesse cliccare su di una
qualsiasi voce di questo menu, verrà automaticamente ricondotto ad uno
specifico archivio di notizie già filtrate sulla base della categoria di
News selezionata. Il parametro in oggetto consente quindi di selezionare
la specifica pagina del sito cui verrà ricondotto l'utente dopo aver
cliccato su di una qualsiasi voce di questo menu, e che dovrà,
ovviamente, contenere un componente CMS "Archivio News" con il parametro
"Abilita Filtro Categoria" selezionato.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Archivio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.

**Visualizza numero di contenuti a fianco del nome:** se selezionato
consentirà di visualizzare a fianco di ogni singola voce di menu il
numero esatto di notizie presenti all'interno della corrispondente
categoria di News

**Nascondi le categorie che non hanno Contenuti associati:** se
selezionato consentirà di non visualizzare all'interno del menu quelle
voci corrispondenti a categorie di News alle quali non è stato associato
alcun post e prive quindi di qualsiasi tipo di contenuti.

**Visualizza anche i contenuti interni a una Gerarchia di Contenuti:**
selezionando questo parametro l'eventuale numero visualizzato a fianco
di ogni singola voce di menu indicante il numero esatto di notizie
presenti all'interno della corrispondente categoria di News, terrà conto
anche dei contenuti interni ad eventuali notizie strutturate presenti in
archivio

> **NOTA BENE:** il valore assegnato a questo parametro deve essere
> coerente con quello assegnato allo stesso parametro del corrispondente
> componente "Archivio News".

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

