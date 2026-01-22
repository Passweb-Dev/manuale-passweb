# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image11.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente al parametro
> **Statico** si veda anche quanto indicato all'interno del capitolo
> "*Configurazione Componenti -- Caratteristiche generali* --
> *Staticizzazione e caricamento asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

All'interno della sotto sezione "**Opzioni del Menu**" è possibile
settare alcuni parametri di fondamentale importanza relativamente a
quello che dovrà poi essere il comportamento del menu stesso all'interno
del sito oltre che, ovviamente, decidere la tipologia di menu da
utilizzare.

Nello specifico dunque il parametro:

**Abilita le protezioni sulle singole voci:** selezionando questo
parametro verranno automaticamente nascoste dal menu tutte le voci
collegate a pagine che l'utente attualmente connesso non è abilitato a
vedere.

Per maggiori informazioni su come abilitare delle restrizioni di
visualizzazione sulle specifiche pagine del sito si veda anche la
sezione "*Live Editing per Varianti Responsive -- Pagine*" di questo
manuale.

**Tipo di Caricamento:** consente di specificare come dovrà essere
gestita la visualizzazione delle voci di menu di livello maggiore a 1.

E' possibile selezionare una delle seguenti opzioni:

- **A Richiesta:** in queste condizioni al caricamento della pagina web
  saranno presenti (nel DOM della pagina stessa) solo ed esclusivamente
  voci di menu di primo livello. Eventuali voci di livello maggiore o
  uguale a 2 verranno inserite all'interno della pagina solo ed
  esclusivamente nel momento in cui un utente dovesse richiederne la
  visualizzazione (cliccando per questo sull'apposita icona di apertura
  delle relative sotto voci).

> **Tale opzione potrebbe essere utile per diminuire i tempi di
> caricamento della pagina soprattutto nel caso in cui il numero delle
> sotto voci sia estremamente elevato**

- **Tutto in una Volta:** in queste condizioni al caricamento della
  pagina web saranno presenti (nel DOM della pagina stessa) tutte le
  voci di menu coerentemente, sempre, con il livello di profondità
  impostato in fase di configurazione del componente stesso

**Tipo di Stili applicati al Menu:** consente di impostare la tipologia
e conseguente lo stile di visualizzazione del menu.

**ATTENZIONE!** Le tipologie di menu selezionabili dipendono anche da
quanto impostato per il precedente parametro "Tipo di Caricamento"

È possibile selezionare uno tra i seguenti valori.

- **Flottante Orizzontale:** selezionabile solo per menu con caricamento
  "Tutto in una volta"

> Selezionando questo valore verranno visualizzate, in orizzontale,
> soltanto le voci di menu di primo livello. Eventuali sotto-voci
> verranno visualizzate al passaggio del mouse sulle voci di livello
> superiore.

- **Flottante Verticale:** selezionabile solo per menu con caricamento
  "Tutto in una volta"

> selezionando questo valore verranno visualizzate, in verticale,
> soltanto le voci di menu di primo livello. Eventuali sotto-voci
> verranno visualizzate al passaggio del mouse sulle voci di livello
> superiore.

- **Lista:** selezionabile solo per menu con caricamento "Tutto in una
  volta"

> Selezionando questo valore verranno sempre visualizzate tutte le voci
> di menu (indipendentemente dal loro livello di appartenenza).
>
> **Per sua stessa natura le voci di questo menu potranno essere
> disposte solo ed esclusivamente in Verticale.**

- **Off Canvas:** selezionando questa opzione il menu verrà posizionato
  al di fuori della pagina web dove invece comparirà soltanto un
  pulsante utile a richiamarlo.

> I successivi parametri consentono poi di decidere dove e come dovrà
> essere visualizzato il menu nel momento in cui un utente dovesse
> richiamarlo cliccando sull'apposito pulsante.

![](./assets/media/image12.png)

> Nello specifico dunque il parametro:

- **Inizializzazione menu:** consente di impostare la modalità di
  apertura iniziale del menu

- **Posizionamento del menu:** consente di indicare la posizione in cui
  dovrà essere visualizzato il menu nel momento in cui l'utente dovesse
  decidere di richiamarlo. È possibile decidere di visualizzarlo sulla
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

> È possibile indicare una delle immagini presenti nel database del sito
> oppure uno degli Attributi Immagine gestiti (campo "**Attributi
> temi**")
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![](./assets/media/image13.png)

- **Alt-text immagine offcanvas**: consente di impostare, in tutte le
  lingue attualmente gestite all'interno del sito, il valore che dovrà
  avere l'attributo alt assegnato all'immagine impostata in
  corrispondenza del precedente parametro "Immagine per Off canvas"

- **Testo del bottone offcanvas**: consente di indicare il testo di un
  eventuale label da mostrare a fianco dell'immagine di apertura del
  menu

<!-- -->

- **TreeView (apertura sottovoci al click del mouse):** selezionando
  questa opzioni il menu verrà costruito visualizzando soltanto le voci
  di menu di primo livello. Eventuali sottovoci verranno visualizzate
  (nascoste) al click del mouse sull'apposita icona di apertura
  (chiusura) presente a fianco di ciascuna voce che presenti almeno una
  voce di livello inferiore.

In questo caso sarà inoltre possibile specificare un valore per i
seguenti parametri:

![](./assets/media/image14.png)

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
un menu **Off Canvas** oppure (parametro "**Non Visualizzare**") di
mantenere esattamente la stessa tipologia di menu utilizzata anche per
dispositivi di visualizzazione del sito con larghezza maggiore o uguale
a 992px

**ATTENZIONE!** Grazie al parametro "**Tipo di Stili applicati al Menu
per dispositivi mobili \< 992px"** è possibile cambiare dinamicamente la
tipologia di menu utilizzata in base alla larghezza del dispositivo di
visualizzazione del sito senza dover per forza di cose realizzare due
differenti menu con le relative opzioni di visualizzazione.

Per ulteriori informazioni relativamente alle diverse tipologie di menu
gestibili all'interno di una Variante Responsiva di Passweb si vedano
anche i successivi capitoli di questo manuali

Una volta definita e configurata la specifica tipologia di menu da
utilizzare, dovranno essere specificate, ovviamente, le singole voci di
questo menu, e questo potrà essere fatto agendo all'interno della
sezione "Gestione Voci" presente nella maschera di configurazione di
questo specifico componente.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

