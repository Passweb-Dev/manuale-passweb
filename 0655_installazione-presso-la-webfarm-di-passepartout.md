# INSTALLAZIONE PRESSO LA WEBFARM DI PASSEPARTOUT



Nel caso di installazioni Mexal presso la server farm di Passepartout
sarà necessario, per prima cosa, impostare il radio button presente
nella parte alta della maschera sul valore **"Installazione WebFarm"**
in maniera tale da poter visualizzare tutti i parametri necessari per
realizzare l'integrazione sito-gestionale in questa specifica
configurazione di prodotto.

![](./assets/media/image4.png)

In queste condizioni, dunque, sarà necessario specificare un valore per
i seguenti parametri:

**Dominio**: dominio dell\'installazione Mexal all\'interno della web
Farm Passepartout a cui collegare il sito web.

**Sigla Azienda**: sigla dell'azienda, presente all\'interno
dell'installazione Mexal, cui collegare il sito e-commerce. **E'
possibile collegare alla stessa azienda Mexal fino ad un massimo di 9
siti differenti**

**Sottoazienda (opzionale):** codice (numerico) dell'eventuale
Sottoazienda cui dovrà essere effettivamente collegato il sito
e-commerce

**Login Server:** login di sistema dell\'utente abilitato all\'utilizzo
di Mexal (campo vuoto nel caso in cui l\'installazione di Mexal sia
stata effettuata senza autenticazione).

**Password Server:** password di sistema dell\'utente abilitato
all\'utilizzo di Mexal e relativa alla login digitata nel campo
precedente (campo vuoto nel caso in cui l\'installazione di Mexal sia
stata effettuata senza autenticazione).

**NOTA BENE**: in riferimento alla nuova gestione degli utenti Mexal BP
Mixer (attiva a partire dalla versione 2012E) **è indispensabile che
l'utente corrispondente alle credenziali inserite nei precedenti campi
(Login Server e Password Server) abbia un livello di gestione ben
definito**. In caso contrario non sarà possibile effettuare la
sincronizzazione sito -- gestionale e verrà ritornato un messaggio di
errore del tipo "Livello di gestione non definito per l\'utente XXXX
Occorre definire il livello di gestione in \"Configurazione utenti\"
oppure definire il livello di gestione predefinito in \"Impostazioni
configurazioni predefinite\"

Per maggiori informazioni in merito alla gestione utenti Mexal si
rimanda all'apposito manuale

**Lingua Installazione:** consente di indicare, selezionandola dal
relativo menu a tendina, quale delle lingue attive all'interno del sito
dovrà essere considerata come la lingua principale in relazione alla
quale prelevare poi i dati dal gestionale.

Supponendo dunque di impostare come "Lingua Installazione" l' Inglese,
tutti i dati prelevati dal gestionale (es. descrizioni delle anagrafiche
articolo, descrizioni delle tabelle gestionali ...), che di norma
verrebbero considerati in italiano e associati quindi all'interno del
sito alla lingua italiana, verranno considerati come dati in inglese e
verranno quindi associati (nei vari campi multilingua) alla
corrispondente lingua Inglese

**ATTENZIONE!** la lingua impostata all'interno del parametro "Lingua
Installazione" determinerà, ovviamente, anche la lingua cui farà
riferimento il parametro "**Aggiorna descrizioni in ... dal
Gestionale**" presente all'interno della maschera "**Parametri di
Sincronizzazione**" del Wizard

![](./assets/media/image5.png)

**Sottodominio Predesk:** codice identificativo dell\'installazione
Mexal all\'interno della web Farm Passepartout, a cui collegare il sito
web

**NOTA BENE**: la corretta impostazione dei parametri sopra evidenziati
è di fondamentale importanza ai fini delle corretta integrazione tra il
sito e-commerce e il gestionale Mexal

**Categorizzazione:** consente di impostare il tipo di categorizzazione
articoli che dovrà poi essere utilizzato all'interno del gestionale. E'
possibile selezionare uno dei seguenti valori:

- **Primaria:** selezionando questa opzione all'interno del sito web
  verrà utilizzata la stessa categorizzazione articoli in uso anche
  all'interno del gestionale.

> In queste condizioni:

- **verranno esportate sul sito tutte le categorie merceologiche
  definite all'interno del gestionale**

- l'associazione **articolo -- categoria** sarà quella definita mediante
  il parametro "**Gruppo merceologico**" presente nella maschera
  "**Altri dati anagrafici**" della relativa anagrafica articolo

![](./assets/media/image6.png)

- **Secondaria:** selezionando questa opzione all'interno del sito web
  verrà utilizzata una categorizzazione articoli realizzata (sempre
  all'interno del gestionale) da hoc proprio per il sito Ecommerce

> In queste condizioni:

- **verranno esportate sul sito solo ed esclusivamente le categorie
  merceologiche marcate come "categorie web"** (utilizzando in questo
  senso l'apposito parametro presente nell'anagrafica gestionale della
  categoria stessa)

![](./assets/media/image7.png)

- l'associazione **articolo -- categoria** sarà quella definita mediante
  il parametro "**Categoria WEB**" presente nella maschera "**Altri dati
  anagrafici**" della relativa anagrafica articolo

![](./assets/media/image8.png)

Per maggiori informazioni relativamente alla possibilità di definire
all'interno del gestionale una categorizzazione articoli ad hoc per il
sito Ecommerce si veda anche quanto indicato all'interno del capitolo
"*Catalogo -- Classificazione articoli sulla base dei gruppi
merceologici Mexal*" di questo manuale

**ATTENZIONE!** Nel momento in cui si dovese decidere di variare il tipo
di categorizzazione, passando da quella primaria a quella secondaria o
viceversa, **sarà poi necessario eseguire una sincronizzazione totale**
in maniera tale da consentire a Passweb di aggiornare correttamente i
dati relativi alla categorie merceologiche in uso all'interno del sito.

Il parametro **"Gestione Pagine"** presente all'interno della sezione
"**Docuvision**" consente invece di decidere se attivare la gestione del
documentale Passepartout a Pagine oppure quella a Revisioni.

In particolare selezionando questo parametro, Passweb considererà attiva
la **gestione di Docuvision a Pagine**. Nel caso in cui il parametro in
oggetto non venga selezionato, Passweb considererà invece attiva la
**gestione di Docuvision a Revisioni**.

**Come indicato nella relativa etichetta il parametro "Gestione Pagine"
ha effetto solo ed esclusivamente nel caso in cui la versione del
gestionale sia inferiore alla 2011B**

**Nel caso in cui la versione del gestionale sia maggiore o uguale alla
2011B sarà possibile impostare, per ogni singolo documento, la sua
gestione a pagine o a revisioni direttamente all'interno di Mexal**

**NOTA BENE**: per maggiori informazioni su come impostare, direttamente
all'interno del gestionale, uno specifico documento Docuvision a Pagine
o a Revisioni si rimanda all'apposito manuale.

Infine, all'interno della sezione "**Web API**" è possibile impostare le
credenziali di un utente Mexal appositamente abilitato alla gestione
delle relative API

![](./assets/media/image9.png)

Per maggiori informazioni relativamente a come poter effettuare delle
chiamate alle Web API di Mexal all'interno del proprio sito Passweb si
veda anche quanto indicato nel relativo capitolo di questo manuale
("*Configurazione -- Mexal Configurazione Gestionale -- Web API Mexal*")

