# INSTALLAZIONE PRESSO LA WEBFARM DI PASSEPARTOUT



Nel caso di installazioni presso la server farm di Passepartout sarà
necessario, per prima cosa, impostare il radio button presente nella
parte alta della maschera sul valore **"Installazione WebFarm"** in
maniera tale da poter visualizzare tutti i parametri necessari per
realizzare l'integrazione sito-gestionale in questa specifica
configurazione di prodotto.

![Videate\\parametri_conf_Horeca_generale.bmp](./assets/media/image104.png)

In queste condizioni sarà quindi necessario specificare un valore per i
seguenti campi:

**Prodotto:** consente di selezionare lo specifico gestionale Ho.Re.Ca
con cui dovrà integrarsi il sito

**Dominio**: dominio dell\'installazione gestionale all\'interno della
web Farm Passepartout a cui collegare il sito web.

**Login Server**: login di accesso al gestionale.

**Password Server**: password di accesso al gestionale.

**NOTA BENE**: i parametri "Server", "Porta", "Login Server" e "Password
Server" possono essere trovati nella maschera "Replica Dati" del
gestionale all'interno della scheda "Configurazione" sezione "Parametri
di connessione"

![Videate\\replica_dati2.bmp](./assets/media/image105.png)

**Valuta Installazione:** consente di indicare, selezionandola da un
apposito menu a tendina, la valuta di gestione definita all'interno del
gestionale e che e che dovrà quindi essere utilizzata anche all'interno
del sito

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

![](./assets/media/image106.png)

**Forza cultura italiana:** consente di settare l'analogo parametro
presente anche all'interno della maschera "Replica Dati --
Configurazione" del gestionale

![](./assets/media/image107.png)

**ATTENZIONE:** il parametro in oggetto deve essere impostato
esattamente allo stesso modo tanto sul gestionale quanto sul Wizard di
Passweb. In caso contrario in fase di sincronizzazione potrebbero essere
ritornati degli errori ed il processo potrebbe non andare a buon fine.

**Categorizzazione:** consente di impostare il tipo di categorizzazione
articoli che dovrà poi essere utilizzato all'interno del gestionale. E'
possibile selezionare uno dei seguenti valori:

- **Primaria:** selezionando questa opzione all'interno del sito web
  verrà utilizzata la stessa categorizzazione articoli in uso anche
  all'interno del gestionale.

> In queste condizioni:

- **verranno esportate sul sito tutte le categorie merceologiche
  definite all'interno del gestionale**

- l'associazione articolo -- categoria sarà quella definita mediante il
  parametro "**Categoria**" presente nella scheda "**Anagrafica**" della
  relativa anagrafica gestionale

![](./assets/media/image108.png)

- **Secondaria:** selezionando questa opzione all'interno del sito web
  verrà utilizzata una categorizzazione articoli realizzata (sempre
  all'interno del gestionale) da hoc proprio per il sito Ecommerce

> In queste condizioni:

- **verranno esportate sul sito solo ed esclusivamente le categorie
  merceologiche marcate come "categorie web"**

- l'associazione articolo -- categoria sarà quella definita mediante il
  parametro "**Categoria Passweb**" presente nella scheda "**Lista
  Articoli e Listini**" della relativa anagrafica gestionale

![](./assets/media/image109.png)

Per maggiori informazioni relativamente alla possibilità di definire
all'interno del gestionale una categorizzazione articoli ad hoc per il
sito Ecommerce si veda anche quanto indicato all'interno del capitolo
"*Catalogo -- Classificazione articoli sulla base dei gruppi
merceologici Ho.Re.Ca*." di questo manuale

**ATTENZIONE!** Nel momento in cui si dovese decidere di variare il tipo
di categorizzazione, passando da quella primaria a quella secondaria o
viceversa, **sarà poi necessario eseguire una sincronizzazione totale**
in maniera tale da consentire a Passweb di aggiornare correttamente i
dati relativi alla categorie merceologiche in uso all'interno del sito.

**Gestione Lista Valori Varianti**: consente di definire come dovranno
essere gestite le Varianti in relazione alla possibilità di
personalizzare le diverse opzioni di scelta in maniera differente per i
singoli prototipi esportati e gestiti all'interno del sito.

E' possibile selezionare uno dei seguenti valori:

- **Prototipo:** selezionando questa opzione gli elementi dei diversi
  insiemi di valori verranno replicati per ogni singolo prototipo legato
  alla Variante considerata. In queste condizioni sarà quindi possibile
  definire un titolo, un colore, un'immagine, un testo e una posizione
  differenti sullo stesso elemento per prototipi diversi.

> Supponendo quindi di dover gestire due prototipi "PR1" e "PR2" legati
> alla stessa Variante con nella lista valori l'elemento "BIA", con
> questa configurazione, sarà possibile fare in modo, ad esempio, che
> per l'opzione "BIA" venga mostrata l'etichetta "BIANCO" sul prototipo
> "PR1" e "BIANCO PERLATO" sul prototipo "PR2".
>
> **ATTENZIONE!** **in queste condizioni, nel caso in cui si dovesse
> decidere di utilizzare una sola Variante per tutti i prototipi gestiti
> all'interno del sito, raggruppando al suo interno anche insiemi di
> valori che possono non essere utilizzati per determinati prototipi, il
> numero di possibili combinazioni da gestire e da replicare sui singoli
> articoli potrebbe aumentare esponenzialmente allungando di
> conseguenza, in maniera anche considerevole, i tempi di eventuali
> sincronizzazioni totali.**
>
> Per maggiori informazioni relativamente a come poter personalizzare le
> opzioni di scelta dei singoli prototipi si veda anche quanto indicato
> all'interno della sezione "*Catalogo -- Gestione Articoli -- Strutture
> Ecommerce Ho.Re.Ca. Gestione Articoli -- Modifica Elementi Struttura*"
> di questo manuale.

- **Unica -- opzione selezionata a default**: selezionando questa
  opzione gli elementi dei diversi insiemi di valori saranno unici per
  tutti i prototipi legati alla Variante considerata. In queste
  condizioni **NON sarà quindi possibile** definire un titolo, un
  colore, un'immagine, un testo e una posizione differenti, sullo stesso
  elemento, per i diversi prototipi gestiti

> Facendo quindi riferimento allo stesso esempio precedentemente
> considerato, in queste condizioni per l'opzione "BIA" verrà mostrata,
> per entrambi i prototipi "PR1" e "PR2", sempre e soltanto la stessa
> etichetta.
>
> **ATTENZIONE!** Per ovvie ragioni se il parametro in questione dovesse
> essere impostato sul valore "**Unica**" non sarà più possibile
> visualizzare, nella maschera di configurazione dei singoli elementi
> della struttura (*Modifica Elementi Campi Struttura*), il parametro
> "**Elementi raggruppati per codice"**
>
> Altra cosa di fondamentale importanza da tenere in considerazione è
> che in queste condizioni **se le strutture gestite all'interno del
> sito dovessero essere impostate come "Esplose completamente" verrà a
> mancare il legame tra i padri di struttura e l'Insieme di Valori per
> cui non sarà possibile gestire i filtri articolo basati sulle
> strutture**
>
> **ATTENZIONE!** Nel momento in cui si dovesse decidere di impostare il
> parametro "Gestione Lista Valori Varianti" sull'opzione "Unica" per
> attivare i filtri di ricerca basati sulle strutture sarà necessario
> gestire queste stesse strutture come "Vincolate al precedente livello"

Nel momento in cui si dovesse decidere di variare il parametro in esame,
passando da una gestione all'altra verrà visualizzato il messaggio
"**E\' necessario effettuare una sincronizzazione totale affinché la
modifica sia effettiva**".

Come indicato dal messaggio dunque, fintanto che non sarà effettuata una
sincronizzazione totale, sul front end del sito verrà mantenuta la
vecchia gestione. Al termine della sincronizzazione totale, dopo aver
ultimato la procedura di importazione delle varianti, verrà effettuato
lo switch sulla nuova impostazione che, a questo punto, sarà quindi
gestita anche sul front end del sito.

**ATTENZIONE!** Nel momento in cui si dovesse decidere di variare il
parametro in esame, passando da una gestione all'altra è di fondamentale
importanza ricordare anche che eventuali personalizzazioni fatte sulle
singole opzioni di scelta (titolo, colore, descrizione \...) andranno
perse e dovranno quindi essere reimpostate da zero

Una volta decisa, dunque, la modalità di gestione dei valori delle
Varianti sarebbe bene non modificare più il parametro in questione.

Una volta impostati correttamente tutti parametri sopra indicati il sito
web potrà comunicare correttamente con il gestionale Ho.Re.Ca. (e con il
relativo Message Box). Questo potrebbe però non essere sufficiente per
gestire sul sito i dati effettivamente presenti all'interno del
gestionale.

**Per fare in modo che articoli, clienti, ordini ecc... possano essere
correttamente trasferiti tra il gestionale Ho.Re.Ca. ed il sito web,
occorre infatti verificare che anche il gestionale sia correttamente
configurato per inviare sul Message Box i dati che dovranno poi essere
prelevati da Passweb ed utilizzati per la costruzione e la pubblicazione
lato front end del sito stesso.**

In particolare nel caso di:

- Collegamento tra un sito Passweb ed un server **Beauty** sarà
  necessario portarsi nella maschera di configurazione "**Replica
  Dati**"

> ed assicurarsi che vengano gestite in **Invio e in Ricezione** sul
> Message Box tutte le informazioni relative ai seguenti elementi:

- **Appuntamenti Beauty**

- **Articoli**

- **Clienti/Agenzie**

- **Disponibilità Risorse Beauty**

- **Documenti di Magazzino**

> Per ciascuno degli elementi sopra indicati la "**Modalità**" di
> sincronizzazione deve essere impostata sul valore "**Pianificata**"

- Collegamento tra un sito Passweb ed un server **Menu** sarà necessario
  portarsi nella maschera di configurazione "**Replica Dati**"

> ed assicurarsi che vengano gestite **in Invio e in Ricezione** sul
> Message Box tutte le informazioni relative ai seguenti elementi:

- **Articoli**

- **Clienti/Agenzie**

- **Documenti di Magazzino**

- **Prenotazione Tavoli**

> Per ciascuno degli elementi sopra indicati la "**Modalità**" di
> sincronizzazione deve essere impostata sul valore "**Pianificata**"

- Collegamento tra un sito Passweb ed un server **Retail** sarà
  necessario portarsi nella maschera di configurazione "**Replica
  Dati**"

> ed assicurarsi che vengano gestite **in Invio e in Ricezione** sul
> Message Box tutte le informazioni relative ai seguenti elementi:

- **Articoli**

- **Clienti/Agenzie**

- **Documenti di Magazzino**

- **Promozione**

> Per ciascuno degli elementi sopra indicati la "**Modalità**" di
> sincronizzazione deve essere impostata sul valore "**Pianificata**"

**NOTA BENE**: per maggiori informazioni relativamente alla
configurazione della replica dati del server Ho.Re.Ca., si rimanda al
corrispondente manuale.

Anche in questo caso per completare l'integrazione sito-gestionale sarà
poi necessario decidere quali articoli ed eventualmente quali clienti
esportare, quali funzionalità sui clienti e/o su gli articoli abilitare
e come poterle configurare in maniera corretta.

Nello specifico la selezione dei clienti e, soprattutto, degli articoli
da esportare all'interno del sito andrà fatta all'interno del relativo
gestionale Ho.Re.Ca.

Per quel che riguarda invece l'attivazione e la configurazione di
determinate funzionalità articolo/cliente (es. quantità massima o minima
di vendita ecc...), sarà necessario agire direttamente all'interno del
Wizard di Passweb.

Per maggiori informazioni relativamente all' esportazione di articoli e
clienti si vedano i successivi capitoli di questo manuale.

Per quel che riguarda invece l'attivazione e/o la configurazione di
determinate funzionalità Articolo/Cliente si veda anche la sezione
"*Catalogo -- Gestione Articoli -- Articoli -- Anagrafica
Articolo/Servizio -- Anagrafica Passweb*" di questo manuale.

