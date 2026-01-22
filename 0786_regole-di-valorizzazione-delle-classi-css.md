# REGOLE DI VALORIZZAZIONE DELLE CLASSI CSS



Come evidenziato nei precedenti capitoli di questo manuale, le Regole di
valorizzazione delle Classi CSS permettono di associare massivamente, a
tutti gli articoli che soddisfano i criteri di selezione impostati nella
regola in esame, una o più classi CSS andando a valorizzare, nello
specifico, il campo "**Classi Regole**" presente nella loro Anagrafica
Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regola_classi_css_1.bmp](./assets/media/image305.png)

Per maggiori informazioni relativamente ai campi "Classi Regole" e
"Classi Custom" si veda anche quanto indicato all'interno del
corrispondente capitolo di questo manuale "*Catalogo -- Gestione
Articoli -- Articoli -- Anagrafica Articolo -- Anagrafica Passweb --
Classi CSS*"

Per creare una nuova Regola di questo tipo sarà necessario per prima
cosa cliccare sul pulsante **Nuova Regola Classi** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuova_regola_classi.bmp](./assets/media/image299.png) ) presente nella barra degli strumenti della maschera
"**Regole di valorizzazione**"

In questo modo verrà infatti visualizzata la maschera di creazione della
nuova regola

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regola_classi_css_2.bmp](./assets/media/image306.png)

mediante la quale poter definire il filtro di selezione articoli e le
classi CSS che dovranno poi essere assegnate a questi stessi prodotti.

Nello specifico dunque il campo:

- **Nome**: consente di assegnare un nome alla regola che si sta
  realizzando

- **Filtro**: consente di definire il filtro articoli necessario per
  individuare tutti i prodotti che dovranno poi essere oggetto della
  regola in esame (Per maggiori informazioni relativamente alla
  creazione di un filtro articoli si veda anche la sezione "*Utenti --
  Gruppi Utenti Sito -- Filtri Utente e Filtri Articolo -- Filtri
  Articolo*" di questo manuale)

- **Classi Regole**: consente di indicare le classi CSS che dovranno
  essere assegnate agli articoli che soddisfano il filtro impostato
  mediante il precedente parametro

Per quel che riguarda poi il campo "**Classi Regole**" è bene
sottolineare anche che:

- Nel momento in cui l'esigenza dovesse essere quella di assegnare agli
  articoli che soddisfano il filtro di selezione impostato due o più
  classi CSS sarà sufficiente inserirle tutte all'interno di questo
  campo separandole con uno spazio

- Una volta applicata la regola in esame, le classi indicate verranno
  inserite, per tutti gli articoli che soddisfano il filtro impostato,
  all'interno del campo "**Classi Regole**" presente nella loro
  Anagrafica Passweb.

> **ATTENZIONE!** il campo "Classi Regole" presente nell' Anagrafica
> Passweb del singolo articolo è un campo in sola lettura il cui
> contenuto potrà quindi essere gestito unicamente mediante
> l'applicazione di apposite regole articolo

- Nel momento in cui l'esigenza dovesse essere quindi quella di
  eliminare, per determinati articoli, eventuali classi CSS
  precedentemente assegnate mediante l'applicazione di apposite regole,
  sarà sufficiente creare ed applicare un'ulteriore regola di questo
  tipo lasciando però, questa volta, il campo "Classi Regole" non
  valorizzato.

> Applicando una regola di questo tipo (campo "Classi Regole" non
> valorizzato) infatti, l'effetto sarà proprio quello di svuotare, per
> tutti i prodotti che soddisfano il filtro impostato, il relativo campo
> presente nella loro Anagrafica Passweb.

- Nel momento in cui dovessero essere applicate contemporaneamente più
  regole diverse agli stessi articoli, il campo "Classi Regole" presente
  nella loro Anagrafica Passweb verrà valorizzato facendo il merge dei
  valori indicati in ogni singola regola.

> Ciò significa dunque che se dovessimo avere, ad esempio, una "Regola
> 1" che filtra tutti gli articoli il cui codice inizia per A impostando
> poi per essi la classe css "classeA" e anche una "Regola 2" che filtra
> invece tutti gli articoli il cui codice inizia per AB andando ad
> impostare per essi la classe css "classeAB", allora l'applicazione di
> entrambe queste regole farà sì che per l'articolo "ACCENDINO" il campo
> "Classi Regole" sia valorizzato con la sola classe "classea" mentre
> per l'articolo "ABITO" il campo "Classi Regole" verrà valorizzato con
> entrambe le classi indicate nelle regole e quindi con "classeA
> classeAB"

**ATTENZIONE! Tutte le regole di valorizzazione delle classi CSS sono in
esecuzione automatica**

Ciò significa dunque, che ogni regola di questo tipo verrà valutata ed
eventualmente applicata a seguito di ogni sincronizzazione sito --
gestionale.

Volendo è comunque possibile applicare manualmente anche questo tipo di
regole, esattamente allo stesso modo di quanto avviene per le regole di
valorizzazione degli attributi articolo, cliccando quindi sul pulsante
"**Applica Regola**" presente nella contestuale barra degli strumenti.

In questo caso però è bene sottolineare che, per non perdere dei valori,
l'applicazione manuale di una determinata regola comporterà
automaticamente anche l'applicazione di tutte le altre regole che
dovrebbero essere applicate agli stessi articoli individuati dal filtro
di selezione impostato per la regola eseguita manualmente.

**[ATTENZIONE!]{.underline}**

Le classi CSS impostate sui vari articoli mediante l'applicazione delle
regole in questione verranno poi applicate, sul front end del sito:

- al componente "**Scheda Prodotto**"

- **alle celle dei relativi articoli** presenti all'interno di
  componenti quali:

  - **Catalogo Ecommerce**

  - **Abbinati**

  - **Offerte** / **Novità**

  - **Popolarità Prodotto**

  - **Risultati Ricerca**

  - **Lista Regalo**

  - **Selezione Regalo**

  - **Campionario Ecommerce**

- alle celle dei risultati del componente "**Autocompletamento**"
  inserito in **Carrello**

