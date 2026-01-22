# SPECIFICHE CUSTOM -- PRESTASHOP / MAGENTO



Nel momento in cui l'esigenza dovesse essere quella di gestire delle
Specifiche Custom da utilizzare in fase di pubblicazione articoli su
Prestashop o Magento occorre tenere in considerazione, innanzitutto, il
fatto che in queste condizioni:

- possono essere create **solamente Specifiche Custom "Semplici"** (del
  tipo "nome:valore") che consentono dunque di gestire situazioni in cui
  il dato da inviare alla piattaforma terza ha un valore "diretto" come
  potrebbe essere, ad esempio, una stringa, un numero ...

- tali Specifiche **potranno essere utilizzate unicamente nel caso in
  cui il metodo di pubblicazione articoli dovesse essere via CSV**

Per codificare una nuova specifica di questo tipo è necessario accedere
alla sezione "**Gestione Specifiche**" del Wizard (menu "*Catalogo --
Altri Marketplace*") e cliccare poi sul pulsante **Aggiungi Specifica**
(
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_specifica_custom.bmp](./assets/media/image324.png) ) presente nella contestuale barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Dati
Specifica**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dati_specifica_prestashop.bmp](./assets/media/image325.png)

all'interno della quale poter impostare tutti i parametri di
configurazione della specifica custom che si intende creare.

Nello specifico sarà possibile indicare un valore per i seguenti campi .

**Nome**: consente di assegnare un nome descrittivo alla specifica che
si sta codificando in maniera tale da poterla poi identificare
univocamente tra tutte le specifiche custom effettivamente presenti in
elenco (il nome assegnato all'interno di questo campo sarà poi quello
mostrato in griglia in corrispondenza della colonna "Descrizione")

**Marketplace**: consente di indicare, selezionandolo da un apposito
menu a tendina, il Marketplace in relazione al quale potrà poi essere
utilizzata la specifica custom che si sta codificando.

In questo caso, ovviamente**, andrà selezionata l'opzione Prestashop o
Magento**

**ATTENZIONE!** una volta assegnato un Marketplace ad una Specifica
questo non potrà più essere modificato. Nel caso in cui fosse necessario
apportare una modifica a questo parametro sarà quindi necessario
eliminare la specifica e crearne una nuova

**Pubblicazione:** consente di indicare il metodo di pubblicazione in
relazione al quale sarà poi possibile utilizzare la specifica in esame.

Considerando che, come precedentemente evidenziato, le Specifiche Custom
create per Prestashop e Magento potranno poi essere utilizzate solo nel
caso di pubblicazioni via CSV, l'unica opzione disponibile, in queste
condizioni, sarà proprio CSV

**ATTENZIONE!** sulla base di quanto precedentemente evidenziato, i
valori presenti all'interno di questo campo varieranno in relazione a
quanto impostato in corrispondenza del parametro "Marketplace"

**Tag** -- visualizzato solo nel caso in cui il precedente parametro
"Marketplace" sia stato impostato sull'opzione Prestashop o Magento.

Consente di impostare parte del nome che verrà poi utilizzato, nel
tracciato record dei file csv, come intestazione per gestire il campo
relativo alla specifica in esame.

In questo senso infatti è bene sottolineare che **l'intestazione
utilizzata per gestire nel file csv il campo relativo ad una determinata
specifica custom si otterrà sempre concatenando alla stringa "custom\_"
il valore inserito all'interno del campo Tag.**

Supponendo dunque di aver codificato una nuova specifica impostando il
suo campo Tag sul valore "Sottotitolo", e di averla poi gestita in una
determinata Inserzione, nel tracciato record dei file di pubblicazione
prodotti da quella stessa inserzione troveremo (in coda ai campi
"standard") anche il campo "**custom_Sottotitolo**" relativo appunto
alla specifica custom in questione

Una volta completata la codifica, la specifica in questione verrà poi
resa disponibile, assieme a quelle "standard", nell'elenco delle
specifiche effettivamente gestibili per ogni Inserzione ma solo per il
Marketplace e il metodo pubblicazione indicati in fase di configurazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\specifiche_custom_2.bmp](./assets/media/image326.png)

Come per una qualsiasi altra specifica sarà quindi possibile
selezionarla, inserirla tra le specifiche gestite per l'Inserzione e
configurarla indicando anche il Campo e/o l'Attributo Articolo da cui
dovrà prelevare il suo valore.

**ATTENZIONE!** Per maggiori informazioni relativamente a come poter
inserire una determinata specifica in un Inserzione e su come mapparla,
si veda quanto indicato nel successivo capitolo (*Gestione Inserzioni*)
di questo manuale

Infine, una cosa di fondamentale importanza da tenere sempre in
considerazione, in queste condizioni, è che nel momento in cui dovessero
essere aggiunte / eliminate delle specifiche, tanto a livello generale
(cancellando cioè alcune delle specifiche tra quelle presenti
all'interno della maschera "Lista delle Specifiche") quanto sulla
singola Inserzione (aggiungendo o togliendo cioè delle specifiche tra
quelle effettivamente gestite nella singola Inserzione), questo tipo di
operazione andrà poi a modificare inevitabilmente il tracciato record
dei file csv eventualmente prodotti a seguito di ogni operazione di
pubblicazione articoli.

In conseguenza di ciò se la modalità adottata per la scrittura di questi
file dovesse essere "In append" è chiaro che tra una pubblicazione e
l'altra i dati presenti all'interno dei file potrebbero non essere più
coerenti provocando quindi dei problemi in fase di importazione dati
sulla piattaforma terza.

**ATTENZIONE! Nel momento in cui si dovesse decidere di aggiungere /
eliminare delle specifiche custom dalle varie Inserzioni è necessario
accertarsi anche di aver correttamente svuotato il repository utilizzato
per la pubblicazione dei file csv in maniera tale da evitare incoerenza
nei dati presenti all'interno di questi file e conseguenti problemi in
fase di importazione dati sulla piattaforma terza**

