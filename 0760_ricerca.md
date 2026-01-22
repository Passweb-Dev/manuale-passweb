# RICERCA



All'interno di questa sezione è possibile:

- Indicare i campi Mexal / Ho.Re.Ca. e/o gli attributi Passweb che
  dovranno essere utilizzati per costruire, valorizzare ed associare ad
  ogni articolo, un campo di ricerca FullText utilizzabile poi
  all'interno dei vari pannelli di ricerca presenti sul sito.

<!-- -->

- Decidere se, per determinate tipologie di filtri articolo, la query di
  ricerca dovrà essere del tipo "Inizia per" piuttosto che "Contiene"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_fulltext_configurazione.bmp](./assets/media/image34.png){width="5.7340277777777775in"
height="3.4479166666666665in"}

Relativamente all' esigenza di creare **un unico campo di ricerca**
**che possa consentire di filtrare gli articoli presenti in catalogo
sulla base di specifici Campi Gestionali e/o sulla base di specifici
Attributi Articolo** sarà sufficiente selezionare i Campi e/o gli
Attributi desiderati tra quelli presenti nel box di sinistra in
corrispondenza del parametro **"Campi FullText"**, e inserirli poi nel
box di destra cliccando sul pulsante raffigurante una piccola freccia
rivolta verso destra.

Allo stesso modo per eliminare uno dei Campi e/o degli Attributi
Articolo aggiunti, sarà sufficiente selezionarlo dal box di destra e
reinserirlo nel box di sinistra cliccando sul pulsante raffigurante una
piccola freccia rivolta verso sinistra.

I campi di ricerca presenti immediatamente al di sopra di entrambi i box
consentono, digitando almeno 3 caratteri, di filtrare gli elementi
presenti all'interno del relativo box.

I due pulsanti raffiguranti piccole frecce rivolte verso l'alto e verso
il basso consentono invece di assegnare un ordinamento personalizzato ai
vari Campi/Attributi presenti nel box di destra.

**ATTENZIONE!** gli elementi evidenziati in nero rappresentano Attributi
Articolo Passweb, mentre gli elementi non evidenziati rappresentano
Campi dell'anagrafica articolo gestionale.

Una volta individuati e selezionati tutti i Campi e/o gli Attributi
Articolo da utilizzare per costruire il campo di ricerca FullText sarà
poi sufficiente cliccare sul pulsante "**Salva**", presente nella parte
bassa della maschera, per avviare il processo di creazione di un nuovo
campo, denominato **FullText** che verrà associato ad ogni singolo
articolo gestito sul sito e riempito automaticamente con i valori di
tutti i Campi e di tutti gli Attributi Articolo precedentemente
selezionati.

Per accertarsi dell'avvenuta creazione di questo nuovo campo, sarà
sufficiente accedere all'Anagrafica Passweb di uno qualsiasi degli
articoli attualmente gestiti, portarsi nella sezione "**Descrizioni**" e
verificare la presenza del campo "**FullText**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_fulltext_configurazione_2.bmp](./assets/media/image35.png){width="5.8180555555555555in"
height="3.532638888888889in"}

**ATTENZIONE!** Il campo FullText è, ovviamente, un campo di sola
lettura e, come precedentemente evidenziato, sarà valorizzato
automaticamente, articolo per articolo, con i dati degli Attributi
Passweb e/o dei Campi gestionali selezionati in fase di creazione del
campo stesso.

Terminato il processo di creazione e valorizzazione del campo FullText,
questo stesso campo potrà poi essere utilizzato sul front end del sito,
in fase di ricerca articoli, ricorrendo ai seguenti Componenti:

- **Risultati Ricerca sul sito:** impostando a **Si** il parametro
  "**Abilita la Ricerca sui Dati E-Commerce**", verrà visualizzato un
  ulteriore campo (**Dati Ecommerce**) mediante il quale poter decidere
  quali dati ecommerce dovranno essere effettivamente considerati in
  fase di ricerca articoli.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\risultati_ricerca_dati_ecommerce.bmp](./assets/media/image36.png){width="4.629861111111111in"
height="3.084722222222222in"}

> E' possibile selezionare una delle seguenti opzioni:

- **Generici:** selezionando questa opzione la ricerca articoli verrà
  effettuata prendendo in considerazione per ogni articolo i seguenti i
  campi: codice, titolo, descrizione, codice alternativo, categoria
  merceologica, categoria statistica, natura e attributi articolo (tutti
  quelli attualmente gestiti all'interno del sito)

- **FullText:** selezionando questa opzione la ricerca articoli verrà
  effettuata prendendo in considerazione solamente il campo FullText e,
  in conseguenza di ciò, i soli Campi e/o Attributi Articolo selezionati
  in fase di creazione del campo FullText

> Per maggiori informazioni relativamente al componente "Risultati
> Ricerca sul sito" si veda anche la corrispondente sezione di questo
> manuale "*Componenti Comuni -- Componente Risultati Ricerca sul sito*
> "

- **Filtro Testo / Filtro Autocompletamento:** è sufficiente configurare
  il componente "**Filtro Testo / Filtro Autocompletamento**" inserito
  all'interno di un pannello di ricerca articoli impostando il campo
  "**Tipologia di Filtro**" sul valore "**Filtro su Campo Articolo**",
  selezionando poi in corrispondenza del parametro "**Campo su cui far
  Filtro**" il valore "**FullText**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_testo_full_text.bmp](./assets/media/image37.png){width="4.643055555555556in"
height="3.0909722222222222in"}

> In queste condizioni il campo in esame consentirà di ricercare gli
> articoli presenti in Catalogo sulla base dei valori presenti, per
> ciascuno di essi, all'interno del campo **FullText**
>
> Per maggiori informazioni in merito si veda anche la corrispondente
> sezione di questo manuale "*Varianti Sito Responsive -- Lista
> Componenti Ecommerce -- Componenti interni ai componenti Ecommerce --
> Filtro Testo / Filtro Autocompletamento*"

Per quel che riguarda l'aggiornamento del campo FullText è bene
ricordare che tale campo verrà automaticamente aggiornato e rigenerato
(assicurando dunque che i valori in esso presenti siano sempre allineati
con quelli dei corrispondenti Campi e/o Attributi Articolo selezionati
in fasi di creazione del campo stesso) al verificarsi delle seguenti
condizioni:

- **in fase di sincronizzazione**, per tutti gli articoli che risultino
  essere variati rispetto all'ultima sincronizzazione terminata
  correttamente

- **in fase importazione risorse** (siti Ecommerce Mexal) per tutti gli
  articoli per cui è stata modificata la Descrizione, qualora
  ovviamente, la Descrizione faccia effettivamente parte dei campi
  selezionati in fase di creazione del campo FullText

- **in fase di importazione csv dei dati articolo**, per gli articoli
  variati qualora ovviamente i campi indicati nel csv facciano
  effettivamente parte dei campi selezionati in fase di creazione del
  campo FullText

- **in fase di salvataggio della maschera "Dati Articolo"**,
  raggiungibile dalla voce di menù "Catalogo -- Articoli" del Wizard. In
  queste condizioni verrà ovviamente rigenerato e aggiornato il campo
  FullText dello specifico articolo

- **in fase di salvataggio della maschera "Configurazione Catalogo"**,
  raggiungibile dalla voce di menù "Catalogo -- Catalogo
  Mexal/Ho.Re.Ca.\" del Wizard, per tutti gli articoli, qualora vengano
  variati i campi inizialmente selezionati in fase di creazione del
  campo FullText

Il parametro "**Ricerca sul campo FullText**" consente di impostare la
tipologia di ricerca che dovrà essere effettuata mediante il campo
FullText. Ovviamente, a seconda della tipologia impostata i risultati
ottenuti potranno essere diversi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_fulltext_tipologia.bmp](./assets/media/image38.png){width="5.597222222222222in"
height="3.4479166666666665in"}

E' possibile selezionare uno dei seguenti valori:

- **Full-text** -- opzione di default -- Selezionando questa opzione:

  - le ricerche effettuate saranno più veloci (grazie agli indici
    fulltext) anche su grandi quantità di dati

  - nel caso in cui, in fase di ricerca, venisse specificata parte di
    una parola, i risultati mostreranno solamente le parole che iniziano
    con il testo specificato.

- **Like**: selezionando questa opzione verrà effettuata una ricerca con
  il predicato like per cui:

  - le ricerche effettuate saranno più lente soprattutto su grandi
    quantità di dati.

  - nel caso in cui, in fase di ricerca, venisse specificata parte di
    una parola, i risultati mostreranno tutte le parole che contengono
    il testo specificato, sia esso all\'inizio, alla fine o in mezzo

Il parametro **"Inizia Per"** consente invece di specificare se, per i
campi indicati, dovrà essere effettuata una ricerca del tipo **"inizia
per"** piuttosto che **"contiene"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_inizia_per.bmp](./assets/media/image39.png){width="5.8180555555555555in"
height="3.532638888888889in"}

Nello specifico dunque, selezionando uno dei campi indicati, eventuali
filtri di ricerca mappati su quello stesso campo eseguiranno query del
tipo "**Inizia per**".

Nel momento in cui l'esigenza dovesse invece essere quella di
effettuare, su uno dei campi indicati, ricerche del tipo "**contiene**"
sarà necessario deselezionare il relativo parametro.

**ATTENZIONE!** Le impostazioni di questo parametro avranno effetto:

- all'interno del componente "**Filtro/Ricerca Catalogo E-Commerce**"
  per filtri impostati su:

  - Codice Alternativo Articolo

  - Codice Articolo

  - Codice Articolo + Codici Alias Articolo

  - Codice Articolo + Descrizione Articolo

  - Codice Articolo + Titolo Articolo

  - Codice Articolo + Titolo Articolo + Descrizione Articolo

  - Codici Alias Articolo

  - Codice Articolo Fornitori

  - Codici Fornitori

- in Carrello all'interno del componente "**Autocompletamento**"

