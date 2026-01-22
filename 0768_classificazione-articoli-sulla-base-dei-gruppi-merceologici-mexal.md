# CLASSIFICAZIONE ARTICOLI SULLA BASE DEI GRUPPI MERCEOLOGICI MEXAL



La presenza in Mexal delle "**Anagrafiche dei Gruppi Merceologici**"
offre un'importante possibilità di classificazione degli articoli a
magazzino, classificazione questa che verrà poi ripresa e sfruttata
anche da Passweb e dal relativo sito e-commerce.

Ad ogni categoria merceologica creata sul gestionale ed esportata sul
sito potrà corrispondere, infatti, una specifica pagina web e,
soprattutto, i menu di categoria articolo gestiti all'interno del sito
verranno auto generati da Passweb in maniera completamente automatica
proprio sulla base dell'albero delle categorie merceologiche definito
nel gestionale.

In questo senso inoltre è bene sottolineare anche che, all'interno del
gestionale, sarà anche possibile, volendo, **impostare una
categorizzazione articoli ad hoc per il sito Ecommerce definendo quindi,
in maniera specifica, quale categoria merceologia esportare o meno
all'interno del sito (in questo senso è comunque richiesta una versione
gestionale maggiore o uguale alla 2021C)**

**ATTENZIONE!** le prestazioni dell'applicativo potrebbero essere
condizionate dall'utilizzo di un numero eccessivo di Categorie
Merceologiche. **Si consiglia quindi, in fase di categorizzazione web,
di restare sempre al di sotto delle 1000 Categorie Merceologiche.**

Per poter definire, all'interno del gestionale, le varie Categorie
Merceologiche sarà necessario accedere, per prima cosa, alla sezione
**\"Anagrafica Gruppo Merceologico\"** agendo sul corrispondente menù
*\"Magazzino -- Tabelle aziendali --Gruppi merceologici articoli\"*:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_anagrafica_gruppi_merceologici.bmp](./assets/media/image71.png)

Per creare un nuovo Gruppo Merceologico sarà necessario cliccare sul
pulsante "**Nuovo**". In questo modo verrà infatti aperta la maschera di
creazione di una nuova anagrafica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_anagrafica_gruppo_merceologico.bmp](./assets/media/image72.png)

all'interno della quale poter impostare tutte le informazioni e i
parametri di configurazione della categoria merceologica che si intende
realizzare.

In particolare il campo:

All'interno di questa maschera sarà ora necessario indicare, tra gli
altri, un valore per i seguenti campi:

**Codice:** consente di impostare il codice della categoria merceologica
che si sta codificando.

**Categoria Web**: permette, se impostato a **Si**, di marcare la
categoria in esame come "categoria web". L'utilizzo di questo parametro
consente quindi di definire in maniera specifica quelle che dovranno
essere le categorie merceologiche da esportare e utilizzare all'interno
del sito.

**ATTENZIONE!** Nel momento in cui si dovesse decidere di utilizzare per
il sito Ecommerce una categorizzazione articoli ad hoc, diversa da
quella in uso all'interno del gestionale, oltre al parametro "Categoria
web" sarà necessario anche:

- associare i vari articoli ad una delle categorie web appositamente
  definite (agendo per questo attraverso l'apposito campo "Categoria
  web" presente all'interno della maschera "Altri dati anagrafici
  dell'anagrafica articolo)

- impostare Passweb in maniera tale che alla sincronizzazione vengano
  prelevate solo ed esclusivamente le categorie web con le relative
  associazioni articolo.

> Per maggiori informazioni in merito a queste operazioni si veda anche
> quanto indicato nel seguito di questo capitolo.

**Descrizione:** consente di impostare la descrizione della categoria
merceologica che si sta codificando.

**ATTENZONE:** il testo inserito all'interno di questo campo verrà
utilizzato come valore, relativo alla lingua Italiana, per il campo
**"Nome Categoria Articolo"** della corrispondente pagina Passweb e
conseguentemente anche come etichetta di default per eventuali menu di
categoria articoli auto generati.

**Codice Padre**: consente di impostare il Gruppo Merceologico che dovrà
essere considerato come padre della categoria articolo che si sta
codificando. E' possibile selezionare una delle categorie
precedentemente codificate. **Nel caso in cui il campo in oggetto non
fosse valorizzato la corrispondente categoria verrebbe considerata come
radice principale**

Per maggiori informazioni relativamente alle diverse opzioni di
creazione di un Gruppo Merceologico, si consiglia comunque di fare
riferimento alla relativa documentazione Mexal.

Dopo aver codificato le varie categorie merceologiche, stabilendo quindi
i vari legami Padre- Figlio, sarà possibile visualizzare anche l'albero
appena creato.

In questo senso è sufficiente selezionare dall'elenco dei gruppi
merceologici quello desiderato e cliccare poi sul pulsante "**Visualizza
per Struttura (F3)**". In questo modo verrà infatti visualizzata la
rappresentazione della struttura ad albero di quello specifico gruppo
merceologico, ovvero il codice merceologico padre con i relativi figli
(codici preceduti dal carattere \"+\"):

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\albero_gruppi_mexal.bmp](./assets/media/image73.png)

> **NOTA BENE:** per maggiori informazioni relativamente alla codifica e
> alla gestione dei gruppi merceologici all'interno del gestionale si
> rimanda al relativo manuale Mexal.

Una volta definiti i gruppi merceologici ed il relativo albero, il passo
successivo sarà ovviamente quello di andare ad associare i vari articoli
a queste stesse categorie merceologiche.

In questo senso sarà possibile procedere in due modi diversi a seconda
del fatto di voler utilizzare all'interno del sito la stessa
categorizzazione effettivamente in uso anche all'interno del gestionale
oppure una categorizzazione realizzata ad hoc per il sito Ecommerce.

Nel primo caso (utilizzo sul sito della stessa categorizzazione in uso
anche all'interno del gestionale) sarà necessario:

- **Lato gestionale** portarsi nell'anagrafica dello specifico articolo

- Cliccare sul pulsante **"Altri dati anagrafici" (F5)** in modo tale da
  aprire la maschera qui di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\anagrafica_ar_opzioni.bmp](./assets/media/image74.png)

- Indicare all'interno del campo **"Gruppo merceologico"** il codice del
  gruppo cui associare l'articolo in esame (è attivo anche il tasto
  funzione F2 attraverso il quale poter effettuare una ricerca sui
  gruppi merceologici precedentemente realizzati)

- **Lato sito** sarà invece necessario accedere alla sezione
  "*Configurazione -- Configurazione Gestionale*" del Wizard e
  verificare di aver impostato il parametro "**Categorizzazione**" sul
  valore "**Primaria**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_categoria_articolo_primaria.bmp](./assets/media/image75.png)

**ATTENZIONE!** in queste condizioni verranno esportate sul sito **tutte
le categorie merceologiche definite all'interno del gestionale** e
l'associazione articolo -- categoria sarà quella definita mediante il
parametro "**Gruppo merceologico**" presente nella scheda "**Altri dati
anagrafici**" della relativa anagrafica gestionale

Nel momento in cui l'esigenza dovesse invece essere quella di utilizzare
all'interno del sito una categorizzazione ad hoc sarà necessario:

- **Lato gestionale** accedere all'anagrafica dei vari articoli e
  associarli alla categoria merceologica desiderata operando questa
  volta mediante il parametro **"Categoria WEB"** presente all'interno
  della maschera **"Altri dati anagrafici"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\anagrafica_ar_opzioni2.bmp](./assets/media/image76.png)

> **ATTEZIONE!** all'interno del campo "Categoria WEB" sopra evidenziato
> potranno essere selezionate ed inserite solo ed esclusivamente le
> categorie merceologiche precedentemente marcate come "categorie web"
> mediante l'apposito parametro "**Categoria web**" presente
> nell'anagrafica della categoria stessa.
>
> **Inoltre, nel momento in cui l'esigenza dovesse essere quella di
> inserire all'interno di questo campo una determinata categoria figlio
> sarà necessario verificare di aver marcato come "categoria web" anche
> la relativa categoria padre.**

- **Lato sito** sarà invece necessario accedere alla sezione
  "*Configurazione -- Configurazione Gestionale*" del Wizard e
  verificare di aver impostato il parametro "**Categorizzazione**" sul
  valore "**Secondaria**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_categoria_articolo_secondaria.bmp](./assets/media/image77.png)

**ATTENZIONE!** in queste condizioni verranno esportate sul sito **solo
ed esclusivamente le categorie merceologiche marcate come "categorie
web"** e l'associazione articolo -- categoria sarà quella definita
mediante il parametro **"Categoria WEB"** presente all'interno della
maschera **"Altri dati anagrafici"**

Dopo aver codificato i vari gruppi merceologici, realizzando la
struttura ad albero desiderata, ed aver effettuato le varie associazioni
Articolo -- Gruppo Merceologico, alla successiva sincronizzazione
Passweb preleverà tutte queste informazioni e, come precedentemente
evidenziato, creerà in maniera completamente automatica una pagina
"Catalogo" e una pagina "Prodotto" per ciascuna delle categorie
merceologiche realizzate in Mexal riproponendo esattamente la stessa
struttura ad albero definita all'interno del gestionale.

Ovviamente ad ogni pagina del sito corrispondente ad una delle categorie
merceologiche realizzate in Mexal sarà associato anche il corretto
filtro articoli. In queste condizioni, dunque, inserendo ad esempio
all'interno di una pagina "Catalogo" il componente E-commerce
**"Catalogo E-commerce"** esso visualizzerà unicamente gli articoli
associati in Mexal alla relativa categoria merceologica.

**ATTENZIONE!** nel caso in cui :

- vengano apportate variazioni ad una struttura preesistente di
  categorie articolo

- vengano effettuate nuove associazioni "articolo/trattamento --
  categoria articolo"

- si decida di passare dalla categorizzazione in uso all'interno del
  gestionale ad una categorizzazione ad hoc per il sito

sarà necessario lanciare una sincronizzazione sito --gestionale per
consentire a Passweb di prelevare correttamente le nuove informazioni.

