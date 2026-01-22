# GESTIONE ATTRIBUTI



La pagina **"Gestione Attributi"** accessibile dalla voce di menu
***"Utenti -- Configurazione Utenti Sito"*** consente di definire e
gestire gli Attributi Cliente che potranno poi essere utilizzati per gli
utenti del proprio sito ecommerce.

All'interno di questa pagina verrà quindi visualizzata la maschera
**"Attributi per gli Utenti E-Commerce"**

![](./assets/media/image195.png)

attraverso la quale poter definire una lista di Attributi che potranno
essere utilizzati, assieme ai campi dell'anagrafica clienti/fornitori
del gestionale, per gestire le informazioni relative ai clienti del
proprio sito e-commerce.

Tali informazioni potranno poi essere utilizzate all'interno di
componenti quali ad esempio la "Registrazione Utente" o il "Profilo
Utente" oppure per classificare e ricercare gli utenti presenti
all'interno della sezione "Clienti" dell'Area Riservata del proprio sito
Ecommerce.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![](./assets/media/image29.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![](./assets/media/image30.png) )

All'interno di questa sezione è possibile definire, dipendentemente
dalla tipologia di sito considerata, due diverse tipologie di Attributi:

- **Mexal:** sono **Attributi Cliente corrispondenti a specifici campi
  Mexal.** Ogni attributo di questa categoria può corrispondere:

  - **ad uno specifico campo di un'apposita videata aggiuntiva
    clienti/fornitori di Mexal**.

  - **ad un campo MyDB che fa parte di una tabella di tipo "Anagrafica
    MyDB" utilizzata come estensione Standard o Riportabile delle
    tabelle Clienti / Fornitori**

> In Passweb sarà quindi necessario definire l'associazione tra questi
> attributi ed i relativi campi del gestionale in maniera tale da poter
> poi **valorizzare questi attributi prelevando/inserendo per ogni
> cliente le informazioni necessarie direttamente da/su Mexal**

- **Passweb:** sono **Attributi Cliente definiti direttamente in
  Passweb.** La creazione e la gestione di questi attributi è demandata
  interamente a Passweb. Ogni attributo di questo tipo **dovrà quindi
  essere definito direttamente all'interno del Wizard** del proprio sito
  e-commerce e le corrispondenti informazioni non verranno mai
  memorizzate all'interno del gestionale.

**ATTENZIONE!** Per i siti Ecommerce collegati ad uno dei gestionali
Ho.Re.Ca. sono gestiti solo ed esclusivamente Attributi di tipo Passweb

In definitiva dunque all'interno del sito sarà possibile utilizzare:

- **i principali campi dell'anagrafica clienti/fornitori del
  gestionale**;

- **i campi delle videate aggiuntive clienti/fornitori di Mexal** per i
  quali è stato creato in Passweb un apposito Attributo Cliente con la
  relativa associazione al campo Mexal desiderato.

- **i campi MyDB** per i quali è stato creato in Passweb un apposito
  Attributo Cliente con la relativa associazione al campo desiderato

- **gli Attributi Cliente di tipo Passweb**, definiti e gestiti
  direttamente all'interno del Wizard del sito stesso

##### ATTRIBUTI MEXAL

Come precedentemente evidenziato gli **Attributi Mexal altro non sono se
non Attributi Cliente corrispondenti a specifici campi Mexal**.

Ogni attributo di questa categoria può corrispondere:

- ad uno specifico campo di un'apposita Videata Aggiuntiva
  Clienti/Fornitori del gestionale.

- ad un campo MyDB che fa parte di una tabella di tipo "Anagrafica MyDB"
  utilizzata come estensione Standard o Riportabile delle anagrafiche
  Clienti / Fornitori

Per creare un nuovo Attributo Cliente di tipo Mexal è necessario, per
prima cosa, portarsi all'interno della pagina **"Gestione Attributi"**
accessibile dalla voce di menu ***"Utenti -- Configurazione Utenti Sito
-- Gestione Attributi"*** del Wizard e cliccare, successivamente, sul
pulsante **"Nuovo Attributo"**
(![](./assets/media/image196.png) ) presente nella barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera **Attributi**

![](./assets/media/image197.png)

all'interno della quale poter definire le caratteristiche dell'Attributo
che si sta realizzando.

Nello specifico i campi presenti all'interno di questa maschera
consentono rispettivamente di:

**Nome Attributo:** consente di definire il nome dell'Attributo Utente
che si sta realizzando.

**Sorgente Dati (solo Ecommerce Mexal):** consente di indicare la
sorgente da cui dovranno poi essere prelevati i valori dell'attributo
che si sta realizzando.

**Nel caso in esame questo campo dovrà essere impostato, ovviamente, sul
valore "Mexal"** (come evidenziato nella figura sopra riportata) Una
volta impostata la sorgente dati occorrerà poi settare anche tutta una
serie di altri parametri che varieranno in relazione alla scelta fatta
per il parametro in oggetto.

**Campo Mexal**: consente di indicare lo specifico campo Mexal su cui
dovrà essere mappato l'attributo utente in esame

In questo senso dal relativo menu a tendina sarà possibile selezionare:

![](./assets/media/image198.png)

- uno qualsiasi dei campi delle Videate Aggiuntive Clienti/Fornitori di
  Mexal

> **ATTENZIONE!** nel caso in cui il campo di una Videata Aggiuntiva sia
> effettivamente presente all'interno del gestionale ma non ancora nel
> menu a tendina sopra evidenziato sarà necessario allineare la base
> dati di Passweb con quella di Mexal attraverso l'apposita funzione di
> **"Aggiornamento Attributi Mexal"** (vedi anche "*Configurazione --
> Parametri Sincronizzazione*" di questo manuale). Successivamente sarà
> necessaria anche una sincronizzazione per consentire a Passweb di
> prelevare da Mexal i valori corretti per il nuovo campo.

- uno qualsiasi dei campi MyDB precedentemente creati all'interno
  dell'apposita sezione del Wizard ("*Configurazione -- MyDB -- Campi
  MyDB*") e mappati, ovviamente, con campi di Tabelle MyDB utilizzate
  come estensione delle anagrafiche cliente / fornitore

> **ATTENZIONE! Nel momento in cui si dovesse decidere di creare un
> Attributo Utente mappato con un campo MyDB sarà poi necessario fare
> particolare attenzione al fatto che il dato inserito dall'utente sul
> front end del sito sia effettivamente compatibile con il tipo di dato
> accettato dal relativo campo MyDB**
>
> Se si dovesse infatti creare, ad esempio, un attributo utente di tipo
> testuale mappato con un campo MyDB numerico, il valore inserito a
> front end dall'utente potrebbe causare, in fase di sincronizzazione,
> un errore a seguito del quale il dato stesso non verrà poi inserito
> nel corrispondente campo Mexal.
>
> Un problema del tutto analogo si potrebbe verificare anche nel caso in
> cui il numero di caratteri accettati a front end per l'attributo in
> esame dovesse essere maggiore a quelli effettivamente gestiti dal
> relativo campo MyDB
>
> Per evitare questo tipo di problemi occorre quindi utilizzare,
> all'interno dei form di registrazione / profilo utente gli elementi
> corretti applicando, laddove possibile, i relativi controlli di
> validazione.
>
> Se ad esempio l'attributo in esame dovesse essere stato mappato su di
> un campo MyDB numerico di 4 caratteri, all'interno dei form di
> registrazione / profilo utente andrebbe inserito un componente "Campo
> di Testo" configurato in maniera tale che possa accettare solo valori
> numerici con un valore massimo pari a 9999
>
> Per maggiori informazioni relativamente alla gestione dei campi MyDB
> si veda anche quanto indicato all'interno del capitolo
> "*Configurazione -- MyDB*" di questo manuale

**ATTENZIONE!** Tra i campi presenti all'interno del menu a tendina
potranno comparire, se attivati in maniera corretta, anche quelli
relativi alle Funzionalità Mexal "Ulteriore Descrizione 1/2/3". Per
maggiori informazioni relativamente all'attivazione di questi campi si
rimanda all'apposita sezione di questo manuale "*CATALOGO -- GESTIONE
CATALOGO - Funzionalità Mexal -- Ulteriore Descrizione 1/2/3
(Clienti)".*

**Tipo Campo:** consente di specificare la tipologia dell'Attributo
Utente che si sta realizzando. E' possibile selezionare uno dei seguenti
valori:

- **Testo:** selezionando questa opzione verrà creato un Attributo
  Utente di tipo Testo utilizzabile quindi per memorizzare qualsiasi
  informazione di tipo testuale inserita dall'utente all'interno del
  form di Registrazione e/o di Profilo.

- **File:** selezionando questa opzione verrà creato invece un Attributo
  Utente di tipo File adatto quindi a contenere eventuali file uplodati
  dall'utente all'interno del modulo di Registrazione e/o di Profilo.

> **In questo caso il campo gestionale utilizzato per mappare
> l'attributo in esame dovrà essere, necessariamente, un campo di tipo
> "F" (File) di una Videata Aggiuntiva Clienti / Fornitori e la
> dimensione impostata per esso dovrà essere sufficiente a contenere il
> percorso di localizzazione (path) del file stesso.**
>
> **ATTENZIONE!** Nel caso in cui il campo gestionale utilizzato per
> mappare l'attributo in esame dovesse essere invece un campo MyDB di
> tipo Alfanumerico, al suo interno verrà memorizzato solo ed
> esclusivamente il nome del file uplodato dall'utente. In queste
> condizioni l'accesso al file vero e proprio potrà quindi avvenire solo
> dal Wizard di Passweb
>
> Per maggiori informazioni relativamente alla creazione in Mexal di
> campi di tipo File all'interno di Videate Aggiuntive Clienti/Fornitori
> si rimanda alla specifica documentazione di prodotto.
>
> Per quel che riguarda invece la possibilità da parte degli utenti del
> sito di uplodare file all'interno dei moduli di Registrazione e/o di
> Profilo Utente si veda anche il corrispondente capitolo di questo
> manuale ("*Lista Componenti Interazione Utente -- Componenti Interni
> ai Componenti Interazione Utente -- Campo File* ")

**Campo in sola lettura:** consente, se selezionato, di impostare
l'attributo che si sta codificando come attributo di sola lettura. In
queste condizioni dunque il valore dell'attributo potrà essere gestito,
cliente per cliente solo ed esclusivamente all'interno del gestionale.

**ATTENZIONE!** Nel momento in cui si dovesse decidere di creare un
Attributo Utente Mexal in sola lettura, eventuali campi pubblicati
all'interno del sito in componenti quali la "Registrazione" o il
"Profilo Utente" dovrebbero anch'essi, per ovvie ragioni, essere
impostati come campi non modificabili.

In ogni caso per ogni attributo utente mexal in sola lettura verranno
applicate le seguenti regole

- Eventuali variazioni apportate sul front end del sito a campi mappati
  con attributi di questo tipo non verranno mai memorizzate ne tanto
  meno inserite all'interno del gestionale.

- Sul back-end del sito, nella sezione "Attributi" della maschera "Dati
  Utente" i campi mappati su questo tipo di attributi saranno sempre e
  soltanto campi in sola lettura.

**Visualizza in Area Riservata**: consente di indicare se l'attributo in
esame dovrà o meno essere presente anche nel **form di ricerca** della
sezione "Clienti" presente nell'Area Riservata del proprio sito
Ecommerce.

Supponendo dunque di aver selezionato il parametro in questione, ad
esempio, per l'Attributo Utente "Professione"

![](./assets/media/image199.png)

portandoci poi in Area Riservata, all'interno della sezione Clienti,
avremo la possibilità di ricercare gli utenti presenti in elenco anche
sulla base di questo stesso attributo

![](./assets/media/image200.png)

In queste condizioni, inoltre, l'attributo indicato comparirà anche
(**se opportunamente valorizzato**) tra le informazioni aggiuntive dello
specifico cliente

![](./assets/media/image201.png)

**Etichetta del campo**: consente di specificare, in tutte le lingue
attualmente gestite, la label da utilizzare per l'attributo in esame nel
momento in cui questo stesso attributo dovesse essere visualizzato anche
nella sezione "Clienti" dell'Area Riservata del sito

Per maggiori informazioni relativamente alla sezione "Clienti" dell'Area
Riservata di un sito Ecommerce, si veda anche quanto indicato nel
relativo capitolo di questo manuale (*Siti Ecommerce Area Riservata e
B2B -- Business Clienti*)

##### ATTRIBUTI PASSWEB

Come precedentemente evidenziato gli **Attributi Passweb** altro non
sono se non **Attributi Cliente definiti direttamente in Passweb.** La
creazione e la gestione di questi attributi è demandata interamente a
Passweb. Ogni attributo di questo tipo **dovrà quindi essere definito
direttamente all'interno del Wizard** del proprio sito e-commerce e le
corrispondenti informazioni non verranno mai memorizzate all'interno del
gestionale.

Per creare un nuovo Attributo Cliente di tipo Passweb è necessario, per
prima cosa, portarsi all'interno della pagina **"Gestione Attributi"**
accessibile dalla voce di menu ***"Utenti -- Gestione Parametri Utente
Ecommerce"*** del Wizard e cliccare, successivamente, sul pulsante
**"Nuovo Attributo"**
(![](./assets/media/image196.png) ) presente nella barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera **Attributi**

![](./assets/media/image202.png)

all'interno della quale poter definire le caratteristiche dell'Attributo
che si sta realizzando.

Nello specifico i campi presenti all'interno di questa maschera
consentono rispettivamente di:

**Nome Attributo:** consente di definire il nome dell'Attributo Utente
che si sta realizzando.

**Sorgente Dati (solo Ecommerce Mexal):** consente di indicare la
sorgente da cui dovranno poi essere prelevati i valori dell'attributo
che si sta realizzando.

**Nel caso in esame questo campo dovrà essere impostato, ovviamente, sul
valore "Passweb"** (come evidenziato nella figura sopra riportata) Una
volta impostata la sorgente dati occorrerà poi settare anche tutta una
serie di altri parametri che varieranno in relazione alla scelta fatta
per il parametro in oggetto.

**ATTENZIONE!** Nel caso di siti Ecommerce collegati ad uno dei
gestionali Ho.Re.Ca. sono gestiti solo ed esclusivamente Attributi
Cliente di tipo Passweb per cui il parametro "Sorgente Dati" non verrà
visualizzato.

**Tipo Campo:** consente di specificare la tipologia dell'Attributo
Utente che si sta realizzando. E' possibile selezionare uno dei seguenti
valori:

- **Testo:** selezionando questa opzione verrà creato un Attributo
  Utente di tipo Testo utilizzabile quindi per memorizzare qualsiasi
  informazione di tipo testuale inserita dall'utente all'interno del
  form di Registrazione e/o di Profilo.

- **File:**selezionando questa opzione verrà creato invece un Attributo
  Utente di tipo File adatto quindi a contenere eventuali file uplodati
  dall'utente all'interno del modulo di Registrazione e/o di Profilo.

> Per maggiori informazioni relativamente alla possibilità da parte
> degli utenti del sito di uplodare file all'interno dei moduli di
> Registrazione e/o di Profilo Utente si veda anche il corrispondente
> capitolo di questo manuale ("*Varianti Sito Responsive -- Lista
> Componenti Interazione Utente -- Componenti Interni ai Componenti
> Interazione Utente -- Campo File* ")

La valorizzazione di questo attributo potrà poi avvenire direttamente da
parte dell'utente agendo, ad esempio, sul form di registrazione al sito,
oppure dall'amministratore del sito agendo dalla sezione "**Attributi**"
della maschera "**Dati Utente**" del Wizard.

![](./assets/media/image203.png)

**Visualizza in Area Riservata**: consente di indicare se l'attributo in
esame dovrà o meno essere presente anche nel **form di ricerca** della
sezione "Clienti" presente nell'Area Riservata del proprio sito
Ecommerce.

Supponendo dunque di aver selezionato il parametro in questione, ad
esempio, per l'Attributo Utente "Professione"

![](./assets/media/image204.png)

portandoci poi in Area Riservata, all'interno della sezione Clienti,
avremo la possibilità di ricercare gli utenti presenti in elenco anche
sulla base di questo stesso attributo

![](./assets/media/image200.png)

In queste condizioni, inoltre, l'attributo indicato comparirà anche
(**se opportunamente valorizzato**) tra le informazioni aggiuntive dello
specifico cliente

![](./assets/media/image201.png)

**Etichetta del campo**: consente di specificare, in tutte le lingue
attualmente gestite, la label da utilizzare per l'attributo in esame nel
momento in cui questo stesso attributo dovesse essere visualizzato anche
nella sezione "Clienti" dell'Area Riservata del sito

Per maggiori informazioni relativamente alla sezione "Clienti" dell'Area
Riservata di un sito Ecommerce, si veda anche quanto indicato nel
relativo capitolo di questo manuale (*Siti Ecommerce Area Riservata e
B2B -- Business Clienti*)

##### AZIONI SUGLI ATTRIBUTI

Tornando ora a prendere in considerazione la maschera principale
"Attributi per gli utenti Ecommerce" i pulsanti presenti nella barra
degli strumenti consentono rispettivamente di:

![Videate\\attributi_utenti_ecommerce.bmp](./assets/media/image195.png)

**Modifica Attributo**
(![](./assets/media/image205.png) ): permette di variare le proprietà dell'attributo
selezionato.

**Elimina Attributo**
(![](./assets/media/image206.png) ): permette di eliminare definitivamente l'attributo
selezionato.

**Nuovo Attributo**
(![](./assets/media/image196.png) ): permette di accedere alla maschera di creazione di
un nuovo attributo precedentemente esaminata

**Utilità**
(![](./assets/media/image207.png) ): consente di richiamare alcune
procedure automatiche che potranno essere effettuate sulle anagrafiche
di tutti i clienti gestiti sul sito.

Cliccando infatti su questo pulsante verrà ricaricata la griglia degli
attributi, che diventerà ora a selezione multipla e che visualizzerà i
soli attributi di tipo Passweb.

**NOTA BENE:** le procedure automatiche gestite all'interno di questa
sezione potranno essere lanciate solo ed esclusivamente in relazione ad
attributi cliente di tipo Passweb. Gli attributi cliente di tipo Mexal,
con i relativi valori, potranno infatti essere gestiti solo ed
esclusivamente all'interno del gestionale (o direttamente dagli stessi
utenti all'interno delle apposite pagine del sito web).

Nella barra degli strumenti compariranno ora nuove icone a ciascuna
delle quali sarà associata una specifica procedura.

![](./assets/media/image208.png)

In particolare il pulsante:

**Azzera** (
![](./assets/media/image209.png) ): consente di rimuovere, per tutti i clienti gestiti
all'interno del sito il valore degli attributi selezionati in elenco

**Deseleziona**
(![](./assets/media/image24.png) ): consente di deselezionare in un colpo
solo tutti gli attributi attualmente selezionati in elenco.

**Gestione**
(![](./assets/media/image210.png) ): consente di uscire dalla sezione
relativa alle Utilità tornando quindi alla normale gestione degli
Attributi Cliente.

