# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_menu_categoria_configurazione2_res.bmp](./assets/media/image261.png){width="4.6194444444444445in"
height="2.932638888888889in"}

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
essere reso statico

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

**Filtro Articoli:** consente di impostare una condizione di pre
filtraggio mediante la quale poter stabilire quali articoli dovranno
essere considerati o meno per la generazione del menu di categoria.

**ATTENZIONE!** L'applicazione di un filtro articoli su di un menu di
categoria potrebbe limitare, ovviamente, il numero di voci presenti
all'interno del menu e, allo stesso modo, potrebbe anche andare ad
impattare sull'indicazione del numero di articoli eventualmente presente
in corrispondenza di ciascuna voce.

**In conseguenza di ciò l'applicazione di un filtro articoli su di un
menu di categoria andrebbe necessariamente considerata soltanto nel
momento in cui sia stata impostata un'analoga condizione di pre
filtraggio anche sul componente "Catalogo Ecommerce", in maniera tale da
mantenere correttamente allineati i due componenti.**

In caso contrario infatti potrebbero verificarsi situazioni in cui
cliccando su una delle voci del menu l'utente verrebbe ricondotto alla
relativa pagina di categoria che potrebbe però essere priva di articoli
(a causa di una condizione di pre filtraggio applicata al componente
"Catalogo Ecommerce") o quanto meno non contenere esattamente lo stesso
numero di articoli indicato nel menu a fianco della relativa voce.

Applicando invece anche al menu di categoria la stessa condizione di pre
filtraggio impostata sul componente Catalogo Ecommerce, le voci presenti
all'interno del menu, così come l'indicazione del numero di articoli
associati a ciascuna voce, rifletteranno esattamente gli articoli
effettivamente visualizzati in Catalogo

I parametri presenti all'interno della sezione "**Opzioni del Menu**"
consentono rispettivamente di:

**Abilita le protezioni sulle singole voci:** selezionando questo
parametro verranno automaticamente nascoste dal menu tutte le voci
collegate a pagine che l'utente attualmente connesso non è abilitato a
vedere.

Per maggiori informazioni su come abilitare delle restrizioni di
visualizzazione sulle specifiche pagine del sito si veda anche la
sezione "Live Editing per Varianti Responsive -- Pagine" di questo
manuale.

**Mostra l'immagine del menu categoria:** se impostato a SI, consente di
visualizzare, in corrispondenza di ogni singola voce di menu, l'immagine
associata, lato Wizard, alla corrispondente categoria merceologica
(sezione "**Risorsa Menu Categoria**" della maschera di gestione delle
immagini delle categorie merceologiche)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_categorie_immagine_categoria.bmp](./assets/media/image262.png){width="4.6194444444444445in"
height="2.675in"}

Per maggiori informazioni in merito alle immagini associabili ad ogni
singola categoria merceologica si veda anche la sezione "*Catalogo --
Gestione Articoli -- Articoli -- Gestione Articoli Categorie
Merceologiche -- Categoria Merceologica Immagini*" di questo manuale

I parametri presenti invece all'interno della sezione "**Tipologia di
Menu**" consentono di definire la tipologia di menu da utilizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_categorie_tipologia_res.bmp](./assets/media/image263.png){width="4.6194444444444445in"
height="2.932638888888889in"}

Nello specifico dunque il parametro :

**Tipo di Mapping:** consente di impostare il tipo di Mapping che dovrà
essere utilizzato per le voci del menu che si sta realizzando. E'
possibile selezionare uno dei seguenti valori:

- **Automatico (basato sulla Pagina Negozio in cui è inserito):** in
  questo caso all'interno del menu verranno visualizzate solo ed
  esclusivamente le voci contestuali alla specifica pagina di tipo
  Catalogo in cui verrà inserito il Componente. In altre parole,
  inserendo, in queste condizioni, il menu all'interno della pagina
  Negozio, esso conterrà le voci relative a tutte le categorie
  merceologiche definite all'interno del gestionale. Inserendolo invece,
  ad esempio, all'interno della pagina di tipo "Catalogo" relativa alla
  categoria merceologica "Categoria A", esso conterrà solo ed
  esclusivamente le voci relative alle categorie merceologiche che si
  trovano, sul gestionale, al di sotto della "Categoria A".

> **NOTA BENE:** in queste condizioni **il numero di voci e la struttura
> del menu potrà quindi variare in relazione alla specifica pagina in
> cui il menu stesso verrà inserito**. In particolare inserendo il menu
> all'interno di una pagina generica del sito esso non visualizzerà,
> ovviamente, alcuna voce.

- **Pagina Negozio Specifica:** in questo caso all'interno del menu
  verranno visualizzate, indipendentemente dalla pagina in cui verrà poi
  inserito il Componente, le voci contestuali alla pagina di tipo
  Catalogo selezionata all'interno del sottostante albero delle pagine

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_menu_categoria_configurazione1_rs.bmp](./assets/media/image264.png){width="4.613194444444445in"
height="2.9506944444444443in"}

> Selezionando, ad esempio, la pagina "Radice Catalogo" il menu conterrà
> le voci relative a tutte le categorie merceologiche, indipendentemente
> dal fatto che il Componente venga poi inserito all'interno della
> pagina "Negozio" o all'interno della pagina di tipo catalogo relativa
> alla categoria merceologica "Categoria A". In queste condizioni quindi
> il numero di voci e la struttura del menu sarà sempre la stessa
> indipendentemente dalla specifica pagina in cui viene inserito.
>
> **NOTA BENE:** nel caso in cui si decida di inserire il menu di
> categoria all'interno di una pagina generica del sito sarà quindi
> necessario selezionare questo tipo di opzione.

**Campo di Ordinamento:** consente di indicare la specifica modalità di
ordinamento che dovrà essere adottata in relazione alle vari voci
presenti all'interno del menu in oggetto.

E' possibile selezionare uno dei seguenti valori:

- **Codice:** selezionando questo valore le voci del menu di categoria
  articoli verranno ordinate sulla base di quello che è il codice della
  corrispondente categoria merceologica all'interno del gestionale

- **Descrizione:** selezionando questo valore le voci del menu di
  categoria articoli verranno ordinate sulla base di quella che è la
  descrizione della corrispondente categoria merceologica all'interno
  del gestionale (ordinamento di tipo Stringa)

- **Personalizzato:** selezionando questo valore le voci del menu di
  categoria articoli verranno ordinate sulla base del valore (numerico)
  assegnato in Passweb alla corrispondente pagina di categoria (campo
  **"Posizione nel Menu di Categoria"**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\posizione_menu_categoria.bmp](./assets/media/image265.png){width="4.6194444444444445in"
height="2.68125in"}

> **NOTA BENE:** a differenza delle precedenti opzioni, l'ordinamento
> "Personalizzato" è un ordinamento di tipo numerico.
>
> Impostando questo tipo di ordinamento, nel caso in cui due o più voci
> dello stesso livello abbiano lo stesso valore di ordinamento (stesso
> numero) queste verranno ordinate in base al codice della
> corrispondente categoria merceologica.
>
> Nel caso in cui invece per alcune voci non venga impostato nessun
> valore di ordinamento (campo "Posizione nel Menu di Categoria" vuoto)
> queste verranno collocate nelle ultime posizioni del menu ed ordinate
> tra loro in base al codice della corrispondente categoria
> merceologica.

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

E' possibile selezionare uno tra i seguenti valori.

- **Flottante Orizzontale:** selezionabile solo per menu con caricamento
  "Tutto in una volta"

> Selezionando questo valore verranno visualizzate, in orizzontale,
> soltanto le voci di menu di primo livello. Eventuali sotto-voci
> verranno visualizzate al passaggio del mouse sulle voci di livello
> superiore.

- **Flottante Verticale:** selezionabile solo per menu con caricamento
  "Tutto in una volta"

> Selezionando questo valore verranno visualizzate, in verticale,
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

- **Offcanvas:** selezionando questa opzione il menu verrà posizionato
  al di fuori della pagina web dove invece comparirà soltanto un
  pulsante utile a richiamarlo.

> I successivi parametri consentono poi di decidere dove e come dovrà
> essere visualizzato il menu nel momento in cui un utente dovesse
> richiamarlo cliccando sull'apposito pulsante.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_cat_offcanvas.bmp](./assets/media/image266.png){width="4.411111111111111in"
height="3.1041666666666665in"}

> Nello specifico dunque il parametro:

- **Inizializzazione menù:** consente di impostare la modalità di
  apertura iniziale del menu

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
> sito oppure uno degli Attributi Immagine gestiti (campo "**Attributi
> Immagine**").
>
> Nel momento in cui non dovesse essere indicata alcuna immagine, per il
> pulsante di apertura verrà utilizzata la classica icona, normalmente
> presente (soprattutto in ambito mobile), per gestire questo tipo di
> elementi
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\icona_menu_offcanvas.bmp](./assets/media/image267.png){width="0.24513888888888888in"
> height="0.21458333333333332in"}

- **Testo del bottone offcanvas**: consente di indicare il testo di un
  eventuale label da mostrare a fianco dell'immagine di apertura del
  menu

<!-- -->

- **TreeView:** selezionando questo valore verranno visualizzate
  soltanto le voci di menu di primo livello. Eventuali sotto-voci
  potranno essere visualizzate (nascoste) al click del mouse.

> In queste condizioni sarà inoltre necessario indicare un valore per i
> seguenti parametri:

- **Immagine Controllo Apri/Chiudi Ramo (presente solo per menu di
  tipologia TreeView):** consente di selezionare una specifica immagine
  da poter utilizzare per il controllo di apertura / chiusura delle
  sottovoci. E' possibile indicare una delle immagini presenti nel
  database del sito oppure uno degli Attributi Immagine gestiti.

> Nel caso in cui non venga specificata nessun immagine il controllo di
> apertura delle sottovoci sarà rappresentato da un **\[+\]** e quello
> di chiusura da un **\[-\].**

- **Gestione del ramo al click sulla voce:** consente di specificare
  quale dovrà essere il comportamento del menu nel momento in cui
  l'utente cliccherà su una voce che ha anche delle sottovoci. E'
  possibile selezionare uno dei seguenti valori:

  - **Indirizzamento alla pagina:** in queste condizioni cliccando sulla
    voce di menu l'utente verrà ricondotto alla pagina indicata nel link
    di collegamento associato alla voce stessa

  - **Apertura/Chiusura del ramo:** in queste condizioni cliccando sulla
    voce di menu si apriranno/chiuderanno le sottovoci senza effettuare
    alcun cambiamento di pagina

  - **Apertura/Chiusura del ramo e Indirizzamento alla pagina:** in
    queste condizioni cliccando sulla voce di menu si
    apriranno/chiuderanno le sottovoci e l'utente verrà anche ricondotto
    alla pagina indicata nel link di collegamento associato alla voce
    stessa

- **Chiusura dei rami al medesimo livello:** selezionando questo
  parametro, in fase di apertura di un voce del menu verranno
  automaticamente chiuse tutte le voci dello stesso livello attualmente
  aperte. Nel caso in cui il parametro in questione non venga
  selezionato sarà invece possibile mantenere aperte contemporaneamente
  più voci di menu dello stesso livello.

**Tipo di Stili applicati al Menu per dispositivi mobili \< 992px:**
visibile solo nel caso in cui il parametro "**Tipo di Stili applicati al
Menu**" non sia stato impostato sull'opzione Off Canvas

Consente di indicare la tipologia di menu che dovrà essere utilizzata
nel momento in cui il dispositivo di visualizzazione del sito dovesse
avere una larghezza inferiore ai 992px.

In questo senso è possibile decidere di utilizzare un menu a **Lista**,
un menu **Off Canvas** oppure (parametro "**Non Visualizzare**")
mantenere esattamente la stessa tipologia di menu utilizzata anche per
dispositivi di visualizzazione del sito con larghezza maggiore o uguale
a 992px

**ATTENZIONE!** Grazie al parametro "Tipo di Stili applicati al Menu per
dispositivi mobili \< 992px" è possibile cambiare dinamicamente la
tipologia di menu utilizzata in base alla larghezza del dispositivo di
visualizzazione del sito senza dover per forza di cose realizzare due
differenti menu con le relative opzioni di visualizzazione.

**Profondità:** consente di impostare il livello di profondità per la
visualizzazione delle voci di menu. Impostando ad esempio questo campo
sul valore 3 verranno visualizzate (nella maniera specificata dal
precedente parametro "Tipo di Stili applicati al menu") le voci di primo
secondo e terzo livello

**Visualizza Numero di Articoli a fianco del Nome:** selezionando questo
parametro verrà visualizzato, a fianco di ogni singola voce di menu, il
numero esatto di articoli presenti all'interno della corrispondente
categoria merceologica e di eventuali sue sottocategorie

**Nascondi le Categorie che non hanno Articoli associati:** selezionando
questo valore sarà possibile nascondere all'interno del menu tutte le
voci corrispondenti a categorie merceologiche che non contengono
articoli.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

