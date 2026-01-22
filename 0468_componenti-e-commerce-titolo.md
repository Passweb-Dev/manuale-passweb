# COMPONENTI E-COMMERCE -- TITOLO



Il componente "**Titolo**" viene utilizzato, tipicamente, per
visualizzare il Titolo o meglio il Nome degli articoli presenti
all'interno di componenti Ecommerce di primo livello come possono essere
il "Catalogo Ecommerce", la "Scheda Prodotto", le "Offerte / Novità"
ecc...

![](./assets/media/image423.png)

Il punto da cui verrà prelevato il Titolo degli articoli e, di
conseguenza, il valore che assumerà il componente in oggetto
all'interno, ad esempio, delle singole celle articoli, dipende
essenzialmente da come è stato impostato il parametro "**Tipo di dato da
utilizzare**" presente all'interno della sezione "**Titolo / Permalink
Articolo**" della pagina "**Sito -- Preferenze -- SEO**" del Wizard

![](./assets/media/image424.png)

**ATTENZIONE!** Il valore assunto dal componente Titolo verrà utilizzato
anche come valore dell'attributo "title" presente nei link alle varie
schede prodotto e dell'attributo "alt" presente nel markup degli
Attributi Passweb di tipo Immagine

Nello specifico dunque nel caso in cui il parametro sopra indicato sia
stato impostato sul valore:

- **Descrizione Gestionale**: il "Titolo" dell' Articolo coinciderà con
  il valore impostato per i singoli articoli all'interno del
  corrispondente campo (Descrizione) della loro anagrafica gestionale

![](./assets/media/image425.png)

![Videate\\horeca_componente_ecommerce_titolo.bmp](./assets/media/image426.png)

- **Attributo Gestionale (solo siti Ecommerce collegati a Mexal):** il
  "Titolo" dell' Articolo coinciderà con il valore impostato per i
  singoli articoli all'interno di un apposito campo di una videata
  aggiuntiva articoli Mexal mappata con un ben preciso Attributo Passweb

<!-- -->

- **Passweb:** il "Titolo" dell' Articolo coinciderà con il valore
  impostato per i singoli articoli all'interno del corrispondente campo
  (Titolo) della loro anagrafica Passweb

![](./assets/media/image427.png)

**ATTENZIONE! Il "Titolo" di un articolo verrà utilizzato anche per
generare il permalink della relativa pagina prodotto ed è quindi
particolarmente importante anche e soprattutto in ottica SEO. Per
maggiori informazioni relativamente alla gestione del "Titolo /
Permalink Articolo" si veda anche la sezione "*Sito -- Preferenze -- SEO
Titolo / Permalink*" di questo manuale**

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![](./assets/media/image428.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di impostare un nome per il Componente che si sta
  editando.

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

- **Tag:** consente di impostare il particolare tag HTML (Titolo H1,
  Titolo H2 ecc... ) con cui dovrà essere generato il componente in
  oggetto (utili ai fini di una miglior indicizzazione della pagina web)

- **Label:** consente di impostare una label che verrà poi visualizzata
  all'interno del sito in corrispondenza del componente in oggetto

- **Abilita link alla pagina dell'Articolo:** se selezionato consente di
  attivare sul componente un link di collegamento alla relativa pagina
  prodotto. Per ovvie ragioni questo parametro non sarà presente nel
  caso in cui il componente in oggetto sia inserito all'interno della
  scheda prodotto

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

