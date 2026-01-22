# CLASSIFICAZIONE ARTICOLI SULLA BASE DEI GRUPPI MERCEOLOGICI HO.RE.CA.



La presenza all'interno dei gestionali Ho.Re.Ca. delle "**Categorie
Articolo**" offre un'importante possibilità di classificazione che verrà
poi ripresa e sfruttata anche da Passweb e dal relativo sito web.

Ad ogni categoria merceologica creata sul gestionale ed esportata sul
sito potrà corrispondere, infatti, una specifica pagina web e,
soprattutto, i menu di categoria articolo gestiti all'interno del sito
verranno auto generati da Passweb in maniera completamente automatica
proprio sulla base dell'albero delle categorie merceologiche definito
nel gestionale.

In questo senso inoltre è bene sottolineare anche che, all'interno del
gestionale, sarà anche possibile, volendo, **impostar una
categorizzazione articoli ad hoc per il sito Ecommerce definendo quindi,
in maniera specifica, quale categoria merceologia esportare o meno
all'interno del sito (in questo senso è comunque richiesta una versione
gestionale maggiore o uguale alla 2020E)**

**ATTENZIONE!** le prestazioni dell'applicativo potrebbero essere
condizionate dall'utilizzo di un numero eccessivo di Categorie
Merceologiche. **Si consiglia quindi, in fase di categorizzazione web,
di restare sempre al di sotto delle 1000 Categorie Merceologiche.**

Per poter definire, all'interno del gestionale, le varie Categorie
Merceologiche sarà necessario, per prima cosa, effettuare un doppio
click sulla voce di menu **"Articoli - Categoria Articolo"** presente
all'interno del Navigatore.

![](./assets/media/image78.png)

In questo modo verrà infatti aperta la maschera **"Categoria articolo
\<nuovo\>"** all'interno della quale poter impostare tutte le
informazioni e i parametri di configurazione della categoria
merceologica che si intende realizzare.

![](./assets/media/image79.png)

In particolare il campo:

- **Nome:** consente di definire il nome della categoria merceologica
  che si sta codificando.

> **NOTA BENE:** il campo Nome è un campo chiave per la categoria
> merceologica. Nel momento in cui si dovesse dunque modificare il Nome
> di una categoria articolo già creata (anche solo modificando i
> caratteri da minuscolo a maiuscolo) , si verrebbe di fatto a creare
> una nuova categoria articolo. A seguito di una modifica di questo
> tipo, alla successiva sincronizzazione, Passweb creerà quindi una
> nuova pagina "Catalogo" utilizzando come template della pagina stessa
> l'attuale pagina "Negozio" del sito.

- **Categoria Madre:** nome della Categoria Articolo che dovrà essere
  considerata come madre (radice) della categoria che si sta
  codificando. E' possibile selezionare una delle categorie articolo
  precedentemente codificate. **Nel caso in cui il campo in oggetto non
  fosse valorizzato la corrispondente categoria verrebbe considerata
  come radice principale**

> **NOTA BENE:** una volta inserita una sotto categoria, alla categoria
> madre non è più possibile assegnare direttamente degli articoli,
> questi devono essere assegnati alle relative sottocategorie.

- **Disponibile:** abilitando la disponibilità di una categoria, si
  rendono vendibili tutti gli articoli a lei assegnati, se risultano in
  corso di validità. Al contrario se una categoria viene resa non
  disponibile, tutti i suoi articoli non saranno più vendibili;

> **NOTA BENE:** il parametro "Disponibile" non ha alcuna influenza
> sugli articoli gestiti all'interno del sito. In conseguenza di ciò
> articoli/servizi appartenenti a categorie merceologiche per cui il
> parametro in oggetto non è stato selezionato potranno comunque
> continuare ad essere gestiti e venduti all'interno del sito. L'unico
> parametro che abilita o meno la gestione di un articolo/servizio
> all'interno del sito è il parametro "Abilita Passweb" presente
> nell'anagrafica dell'articolo/servizio stesso.

- **Cat. Passweb:** permette, se selezionato, di marcare la categoria in
  esame come "categoria web". L'utilizzo di questo parametro consente
  quindi di definire in maniera specifica quelle che dovranno essere le
  categorie merceologiche da esportare e utilizzare all'interno del
  sito.

> **ATTENZIONE!** Nel momento in cui si dovesse decidere di utilizzare
> per il sito Ecommerce una categorizzazione articoli ad hoc, diversa da
> quella in uso all'interno del gestionale, oltre al parametro "Cat.
> Passweb" sarà necessario anche:

- associare i vari articoli ad una delle categorie web appositamente
  definite (agendo per questo attraverso l'apposito campo presente nella
  sezione "Lista articoli e listini" dell'anagrafica articolo)

- impostare Passweb in maniera tale che alla sincronizzazione vengano
  prelevate solo ed esclusivamente le categorie web con le relative
  associazioni articolo.

> Per maggiori informazioni in merito a queste operazioni si veda anche
> quanto indicato nel seguito di questo capitolo.

- **Immagine:** consente di personalizzare il corrispondente pulsante di
  categoria assegnandovi un'immagine a piacere. L'immagine inserita
  all'interno di questo campo verrà considerata, all'interno del
  corrispondente sito Passweb, come immagine rappresentativa della
  corrispondente categoria merceologica (ed utilizzata ad esempio
  all'interno del componente Ecommerce "Lista Categorie").

> L'immagine rappresentativa di una categoria merceologica potrebbe
> anche essere inserita direttamente all'interno di Passweb (per
> maggiori informazioni in merito si veda anche la sezione *"Catalogo --
> Gestione Articoli -- Gestione Articoli Categorie Merceologiche"* di
> questo manuale)
>
> In queste condizioni, a seguito di una sincronizzazione, l'immagine
> della categoria articolo caricata all'interno del gestionale potrebbe
> anche, dipendentemente da quanto impostato per il parametro
> **"Aggiornamento file da Horeca"** (sezione "Configurazione --
> Parametri di sincronizzazione" del Wizard), andare a sovrascrivere
> l'immagine caricata per la categoria stessa direttamente all'interno
> di Passweb.

- **Descrizione**: consente di specificare una descrizione per la
  categoria merceologica che si sta codificando. Tale descrizione verrà
  poi utilizzata lato Passweb come nome della corrispondente pagina
  "Catalogo" e conseguentemente anche come etichetta, in italiano, della
  corrispondente voce del menu di categoria articoli.

> **NOTA BENE:** nel caso in cui l'esigenza sia quella di modificare
> l'etichetta, in italiano, di una specifica voce del menu di categoria
> articoli, sarà necessario modificare nel gestionale quanto presente
> all'interno del campo Descrizione e **NON** quanto presente
> all'interno del campo Nome. In quest'ultimo caso infatti non verrebbe
> modificata la categoria esistente ma ne verrebbe creata una nuova con
> tutte le conseguenze del caso.
>
> La modifica o meno, a seguito di una sincronizzazione, del nome in
> italiano delle pagine Catalogo, e delle etichette delle voci dei menu
> di categoria articoli, con quanto presente all'interno del campo
> "Descrizione" nell'anagrafica Ho.Re.Ca. della corrispondente categoria
> merceologica, dipende anche da come è stato impostato, in Passweb il
> parametro "Aggiornamento descrizioni in italiano da Horeca -- Tabella
> Categorie Merceologiche" (in proposito si veda anche la sezione
> *"Configurazione -- Parametri di Sincronizzazione"* di questo
> manuale).

Per maggiori informazioni relativamente agli altri parametri di
configurazione della Categoria Merceologica si rimanda alla relativa
documentazione di prodotto.

Nel caso del gestionale **Beauty** molto importante è anche la scheda
**"Risorse"** dove è possibile trovare la tabella "**Tipi risorsa**" in
cui indicare gli eventuali tipi di risorsa che dovranno essere trasmessi
ai trattamenti/servizi appartenenti a tale categoria (necessario nel
caso della gestione delle prenotazioni di servizi/trattamenti) e quelli
che dovranno essere inviati al sito ai fini di una prenotazione via web
dello specifico trattamento/servizio.

![](./assets/media/image80.png)

> **NOTA BENE:** i valori impostati all'interno della tabella "Tipi
> Risorsa" di una categoria articolo, verranno trasmessi a tutti gli
> articoli/servizi/trattamenti associati poi a questa stessa categoria.

Ad esempio, in caso di categoria Cat_Visita Medica, è necessaria la
risorsa di tipo Medico e la risorsa Camerino. In questo caso, se in fase
di configurazione nuovo Trattamento, verrà assegnata la categoria
Cat_Visita Medica, il nuovo trattamento erediterà in automatico le
risorse Medico e Lettino.

Le colonne **"Qta minima"** e , **"Qta"** indicano rispettivamente la
quantità di risorse obbligatorie e la quantità totale di risorse
facoltative più le risorse obbligatorie. Ad esempio se viene inserito il
tipo risorsa Istruttore con Qta minima =1 e Qta = 2, allora tutti i
trattamenti appartenenti alla categoria che si sta configurando
erediteranno la stessa configurazione. In fase di presa
dell'appuntamento da gestionale per tali trattamenti verranno mostrate
tutte le risorse richieste con quantità pari a quanto inserito nella
colonna Qta, nel caso dell'esempio sopra verranno mostrate 2 risorse di
tipo Medico ed una risorsa di tipo Lettino. Al momento della scelta
delle risorse sarà necessario selezionare 1 risorsa di tipo Medico e 1
risorsa di tipo Lettino, mentre la scelta della risorsa aggiuntiva di
tipo Medico è opzionale: quindi l'appuntamento può essere salvato
selezionando 1 medico ed 1 lettino, oppure in aggiunta selezionando 2
medici ed 1 lettino.

La colonna **"Passweb"** consente invece di specificare se la
corrispondente risorsa dovrà o meno essere inviata al sito ai fini di
una prenotazione via web dello specifico trattamento/servizio.

**IMPORTANTE: Relativamente alla prenotazione via web (attraverso il
corrispondente sito Passweb) dei servizi/trattamenti con più risorse
associate, è necessario indicare una sola risorsa obbligatoria, l'unica
che verrà di fatto inviata al sito, con Qta minima = 1. Tutte le altre
risorse eventualmente associate alla categoria merceologica, e di
conseguenza ereditate dai trattamenti/servizi appartenenti alla
categoria stessa, dovranno essere impostate con Qta minima = 0. (per
maggiori informazioni in merito si veda anche la precedente sezione
"Esportazione/Eliminazione di servizi/trattamenti dal gestionale
Ho.Re.Ca. al sito web").**

**In sostanza dunque ai fini della prenotazione via web i
trattamenti/servizi multi risorsa dovranno essere considerati come
quelli mono risorsa. Le eventuali ulteriori risorse, impostate come
facoltative sulla base dei parametri sopra indicati, dovranno quindi
essere associate al trattamento/servizio dal gestore, operando
direttamente all'interno del gestionale Ho.Re.Ca. sulla prenotazione che
questo ha ricevuto dal sito web.**

> **NOTA BENE:** le risorse associate ai trattamenti/servizi gestiti via
> web, non vengono inviate al sito in fase di sincronizzazione, ma
> vengono gestite ed inviate in modo dinamico nel momento stesso in cui,
> in fase di prenotazione web, verrà richiesta la disponibilità dello
> specifico trattamento/servizio.

Una volta definiti i gruppi merceologici ed il relativo albero, il passo
successivo sarà ovviamente quello di andare ad associare i vari articoli
a queste stesse categorie merceologiche.

In questo senso sarà possibile procedere in due modi diversi a seconda
del fatto di voler utilizzare all'interno del sito la stessa
categorizzazione effettivamente in uso anche all'interno del gestionale
oppure una categorizzazione realizzata ad hoc per il sito Ecommerce.

Nel momento in cui l'esigenza dovesse essere quindi quella di utilizzare
all'interno del sito Ecommerce la stessa categorizzazione in uso anche
all'interno del gestionale sarà necessario:

- Lato gestionale accedere all'anagrafica dei vari articoli e associarli
  alla categoria merceologica desiderata mediante il parametro
  "**Categoria**" presente all'interno della scheda "**Anagrafica**"

![](./assets/media/image81.png)

- Lato sito sarà invece necessario accedere alla sezione
  "*Configurazione -- Configurazione Gestionale*" del Wizard e
  verificare di aver impostato il parametro "**Categorizzazione**" sul
  valore "**Primaria**"

![](./assets/media/image82.png)

**ATTENZIONE!** in queste condizioni verranno esportate sul sito tutte
le categorie merceologiche definite all'interno del gestionale e
l'associazione articolo -- categoria sarà quella definita mediante il
parametro "Categoria" presente nella scheda "Anagrafica" della relativa
anagrafica gestionale

Nel caso in cui l'esigenza dovesse essere invece quella di utilizzare
all'interno del sito una categorizzazione ad hoc sarà necessario:

- Lato gestionale accedere all'anagrafica dei vari articoli e associarli
  alla categoria merceologica desiderata operando questa volta mediante
  il parametro **"Categoria Passweb"** presente all'interno della scheda
  "**Lista Articoli e Listini**"

![](./assets/media/image83.png)

> **ATTEZIONE!** all'interno del campo "Categoria Passweb" sopra
> evidenziato potranno essere selezionate ed inserite solo ed
> esclusivamente le categorie merceologiche precedentemente marcate come
> "categorie web" mediante l'apposito parametro "**Cat. Passweb**"
> presente nell'anagrafica della categoria stessa.
>
> Inoltre, nel momento in cui l'esigenza dovesse essere quella di
> inserire all'interno di questo campo una determinata categoria figlio
> sarà necessario verificare di aver marcato come "categoria web" anche
> la relativa categoria padre.

- Lato sito sarà invece necessario accedere alla sezione
  "*Configurazione -- Configurazione Gestionale*" del Wizard e
  verificare di aver impostato il parametro "**Categorizzazione**" sul
  valore "**Secondaria**"

![](./assets/media/image84.png)

**ATTENZIONE!** in queste condizioni verranno esportate sul sito solo ed
esclusivamente le categorie merceologiche marcate come "categorie web" e
l'associazione articolo -- categoria sarà quella definita mediante il
parametro "Categoria Passweb" presente nella scheda "Lista Articoli e
Listini" della relativa anagrafica gestionale

Infine, dopo aver codificato i vari gruppi merceologici, realizzando la
struttura ad albero desiderata, ed aver effettuato le varie associazioni
"Articolo/Trattamento -- Categoria Articolo", alla successiva
sincronizzazione Passweb preleverà tutte queste informazioni e creerà,
in maniera completamente automatica (come per Mexal), una pagina
"Catalogo" e una pagina "Prodotto" per ciascuna delle categorie
esportate riproponendo quindi anche all'interno del sito la stessa
struttura ad albero definita sul gestionale

Ovviamente ad ogni pagina del sito corrispondente ad una delle categorie
merceologiche realizzate all'interno del gestionale sarà associato anche
il corretto filtro articoli/trattamenti. In queste condizioni, dunque,
inserendo ad esempio all'interno di una pagina Catalogo il componente
E-commerce **"Catalogo E-commerce"** esso visualizzerà unicamente gli
articoli/trattamenti associati nel gestionale alla relativa categoria
articolo.

**ATTENZIONE!** nel caso in cui :

- vengano apportate variazioni ad una struttura preesistente di
  categorie articolo

- vengano effettuate nuove associazioni "articolo/trattamento --
  categoria articolo"

- si decida di passare dalla categorizzazione in uso all'interno del
  gestionale ad una categorizzazione ad hoc per il sito

sarà necessario lanciare una sincronizzazione sito --gestionale per
consentire a Passweb di prelevare correttamente le nuove informazioni.

