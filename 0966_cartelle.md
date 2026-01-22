# CARTELLE



All'interno di questa sezione del Wizard è possibile visualizzare e
gestire tutte le cartelle attualmente presenti in Area Riservata.

![](./assets/media/image239.png)

Per ogni singola cartella presente in elenco è indicato:

- l'identificativo (campi Id)

- il nome (campo Nome)

- il percorso di localizzazione (campo Path)

- la dimensione (campo Dimensione)

**ATTENZIONE! Tra le cartelle presenti in elenco verranno evidenziate in
rosso le "Cartelle non Assegnate" ossia quelle cartelle presenti in area
riservata (sezione "Documenti") create da utenti non più gestiti
all'interno del sito.**

Il pannello di "**Ricerca**" consente di impostare uno specifico filtro
di ricerca attraverso il quale poter selezionare, tra tutti le cartelle
presenti in elenco, solamente quelle che soddisfano i parametri del
filtro impostato.

È possibile effettuare delle ricerche filtrando per identificativo
cartella (campo **Id**), nome della Cartella (campo **"Nome"**) e per
tipologia della cartella. In quest'ultimo caso è possibile filtrare le
cartelle effettivamente associate ad utenti ancora gestiti all'interno
del sito (campo "Assegnata" = Si) oppure quelle "Non Assegnate" (campo
"Assegnata" = No) ossia **create da utenti non più gestiti all'interno
del sito**.

I pulsanti presenti nella barra degli strumenti consentono invece di:

**Elimina** (
![](./assets/media/image95.png) ): consente di eliminare definitivamente
la cartella selezionata e tutti i file in essa contenuti

**Esportazione Cartelle** (
![](./assets/media/image96.png) ): consente di esportare in un file .csv l'elenco
delle cartelle attualmente presenti in griglia. Nel file di
esportazione, per ciascuna cartelle saranno indicati i seguenti campi:

- **id**: identificativo cartella

- **nome**: nome cartella

- **idpadre**: identificativo cartella padre

- **creatore**: utente che ha creato la cartella

- **amministratore**: utente amministratore della cartella

- **percorso**: percorso della cartella in area riservata

- **dimensione**: dimensione in byte della cartella

**Files** (
![](./assets/media/image97.png) ): consente di accedere ai file presenti
all'interno della cartella attualmente selezionata.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
**"Elenco File"**

![](./assets/media/image240.png)

contenente l'elenco di tutti i file attualmente presenti all'interno
della cartella in esame.

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

**Scarica Cartella** (
![](./assets/media/image99.png) ): consente di effettuare il download di
uno zip contenente tutti i file presenti all'interno della cartella

**Scarica File** (
![](./assets/media/image100.png) ): consente di effettuare il download del file
attualmente selezionato in elenco.

**Svuota Cartella** (
![](./assets/media/image101.png) ): consente di eliminare dal sito tutti i file
presenti nella cartella in esame

**Elimina File** (
![](./assets/media/image102.png) ): consente di eliminare dal sito il file
attualmente selezionato in elenco

Relativamente alla gestione delle **Cartelle Non Assegnate** occorre
sottolineare che nel caso in cui si decida di eliminare un utente dal
sito, , contestualmente alla sua eliminazione, verranno automaticamente
eliminate anche tutte le cartelle presenti in Area Riservata create da
quello stesso utente, che non risultano essere legate ad altri gruppi e
che non hanno file al loro interno.

Nel momento in cui queste cartelle dovessero invece contenere dei file o
dovessero essere legate anche ad altri utenti ancora gestiti all'interno
del sito non potranno, ovviamente, essere eliminate in maniera
automatica.

D'altra parte avendo eliminato l'utente che le ha create verrà a ora
mancare anche la possibilità di gestirle direttamente all'interno
dell'Area Riservata modificandone, se necessario le proprietà
(Lettura/Scrittura/Modifica) o i permessi di visualizzazione, operazioni
queste effettuabili solo ed esclusivamente dall'utente che ha creato la
specifica cartella.

Per risolvere questo tipo di problema è necessario assegnare a queste
cartelle un nuovo proprietario e questo lo si può fare agendo
esattamente da questa sezione del Wizard.

Nello specifico, sarà sufficiente individuare la Cartella Non Assegnata
da gestire tra quelle presenti in elenco, selezionarla e cliccare sul
pulsante **Assegna Utente** (
![](./assets/media/image103.png) ) presente nella contestuale barra degli strumenti

**Assegna Utente**
(![](./assets/media/image103.png) ): consente di gestire la cartella selezionata,
assegnandola ad un nuovo proprietario.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Dati Cartella**"

![](./assets/media/image241.png)

all'interno della quale sono visualizzati gli Utenti e i Gruppi
attualmente associati alla cartella e che possono quindi ancora
accedere, con i permessi inizialmente stabiliti da chi aveva creato
questa stessa cartella, ai suoi contenuti operando direttamente
dall'Area Riservata del sito.

Per eliminare uno degli utenti o dei gruppi che hanno accesso alla
cartella è sufficiente selezionarlo dal box di destra e cliccare sulla
piccola freccia rossa.

Allo stesso modo per abilitare uno degli utenti o dei gruppi presente
nel box di sinistra ad accedere ai contenuti della cartella è
sufficiente selezionarlo ed inserirlo nel box di destra cliccando sulla
piccola freccia verde.

Il campo **"Assegna a"** consente invece di assegnare alla cartella in
esame un nuovo proprietario selezionandolo tra tutti gli utenti ancora
gestiti all'interno del sito.

**ATTENZIONE! Nel momento in cui si dovesse assegnare alla cartella un
nuovo proprietario questa non verrà più considerata come una "Cartella
Non Assegnata"**

Per maggiori informazioni relativamente alle diverse sezioni e
funzionalità dell'Area Riservata si veda anche la sezione *"Struttura
Sito -- Area Riservata"* di questo manuale.

