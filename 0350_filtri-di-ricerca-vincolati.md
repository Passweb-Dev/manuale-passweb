# FILTRI DI RICERCA VINCOLATI



I filtri vincolati messi a disposizione da Passweb permettono agli
utenti del sito di effettuare ricerche articoli in maniera progressiva
aggiornando cioè le possibili opzioni di scelta messe a disposizione dal
pannello di ricerca, sulla base dei valori mano a mano selezionati
dall'utente stesso all'interno dei vari campi.

Il vantaggio che si può avere nell'utilizzare questo tipo di soluzione è
piuttosto evidente.

Supponiamo infatti di considerare un tradizionale pannello di ricerca i
cui campi non sono in alcun modo vincolati tra loro.

In queste condizioni tutti i campi all'interno del pannello saranno
sempre visibili e, soprattutto, ognuno di essi mostrerà sempre tutte le
possibili opzioni di scelta, indipendentemente dal fatto che l\'utente
abbia o meno già impostato dei parametri di ricerca.

![](./assets/media/image29.png)

Nell'esempio considerato in figura dunque anche nel caso in cui l'utente
abbia già impostato il valore "**TV 2D**" per il campo "**Cat.
Merceologica**" il successivo campo di ricerca "**Sotto Cat.
Merceologica**" continuerà a mostrare tutte le possibili opzioni di
scelta dettate dagli articoli presenti all'interno dalla pagina e
quindi, non solo le sotto categorie merceologiche delle TV 2D ma anche
quelle delle TV 3D e delle SMART TV.

![](./assets/media/image30.png)

**ATTENZIONE!** Nell'esempio considerato "**Cat. Merceologica**" e
"**Sotto Cat. Merceologica**" sono **due Attributi Articolo di tipo
Passweb** opportunamente valorizzati, articolo per articolo, all'interno
delle relative anagrafiche Passweb. Per maggiori informazioni sugli
Attributi Articolo si veda anche il capitolo *"Catalogo -- Gestione
Attributi Articolo"* di questo manuale

In queste condizioni dunque l'utente potrebbe anche selezionare
un'opzione non valida per il campo relativo alle sottocategorie
merceologiche (es. SMART TV -- SAMSUNG) impostando di fatto una ricerca
non corretta e non ottenendo quindi alcun risultato.

![](./assets/media/image31.png)

Per risolvere questo tipo di problema è possibile utilizzare i filtri
vincolati in modo tale che le possibili opzioni di scelta presenti
all'interno dei vari campi del pannello di ricerca, dipendano non solo
dagli articoli presenti all'interno della pagina in cui si trova il
pannello ma anche da quello che l'utente ha selezionato all'interno
degli stessi campi di ricerca.

Supponendo dunque di configurare il pannello di ricerca impostando il
campo "**Tipologia Filtro**" sul valore "**Vincolato al precedente
livello**"

![](./assets/media/image32.png)

ci troveremo in una situazione in cui le opzioni di scelta presenti
all'interno del campo "Sotto Cat. Merceologica" dipenderanno
direttamente da quello che l'utente ha selezionato nel campo precedente
(inoltre il campo "Sotto Cat. Merceologica" verrà visualizzato solo dopo
che l'utente ha selezionato un valore per il campo "Cat. Merceologica).

In questo caso dunque, nel momento in cui l'utente dovesse selezionare
per il campo "**Cat. Merceologica**" il valore **TV 2D**, il successivo
campo di ricerca "**Sotto Cat. Merceologica"** mostrerà solo ed
esclusivamente le possibili opzioni compatibili con la selezione
impostata dall'utente

![](./assets/media/image33.png)

Grazie ai filtri vincolati quindi è possibile guidare l'utente nelle sue
ricerche di articoli all'interno del sito riducendo al minimo i casi in
cui tali ricerche non portino ad ottenere alcun risultato.

Il fatto poi di visualizzare all'interno del pannello di ricerca i
diversi campi solo dopo aver impostato un valore per il campo
precedente, oppure visualizzare sempre tutti i campi di ricerca
aggiornando però le diverse possibili opzioni per ciascuno di essi sulla
base delle varie selezioni impostate dall'utente, dipende, come
precedentemente evidenziato, dalle particolari impostazioni di
configurazione settate per il pannello di ricerca.

Nell'esempio di filtri vincolati appena considerato le possibili opzioni
di scelta per ogni campo di ricerca sono dettate, oltre che dalle
impostazioni di configurazione del pannello, dai valori assunti, per il
corrispondente attributo, da tutti gli articoli presenti all'interno
della pagina in cui è inserito il pannello di ricerca.

Ora questa condizione, in determinate circostanze, potrebbe comunque
portare ad ottenere dei risultati non corretti.

Per capirci meglio consideriamo un ulteriore esempio.

Supponiamo di dover gestire la vendita di accessori compatibili,
contemporaneamente, con più articoli differenti, come potrebbe essere il
caso, ad esempio, di cartucce d'inchiostro compatibili con diversi
modelli e marche di stampanti.

Potremmo quindi avere:

- una "**Cartuccia x23**" compatibile con una stampante **HP** modello
  "**Photosmart 6520**" e con una stampante **CANON** modello "**PIXIMA
  MX 925**"

- una "**Cartuccia y35**" compatibile con una stampante **HP** modello
  "**Photosmart 6520**", con una stampante **HP** modello "**D4H21B**" e
  con una stampante **SAMSUNG** modello "**CLP 365W**"

  ------------------------------------------------------------------------
  **CARTUCCIA**     **MARCA STAMPANTE         **MODELLO STAMPANTE
                    COMPATIBILE**             COMPATIBILE**
  ----------------- ------------------------- ----------------------------
  Cartuccia x23     HP, CANON                 Photosmart 6520, PIXMA MX

  Cartuccia y35     HP, SAMSUNG               Photosmart 6520, D4H21B, CLP
                                              365W
  ------------------------------------------------------------------------

Per rappresentare questa situazione all'interno del nostro sito potremmo
pensare di creare due Attributi Articolo di tipo Passweb "**Stampante**
**-- Marca**" e "**Stampante -- Modello**"

![](./assets/media/image34.png)

entrambi di tipo "**Selezione Multipla**" ed entrambi in grado di
accettare due o più valori.

![](./assets/media/image35.png)

Nella sezione "**Gestione Opzioni**" andremo quindi ad indicare tutti i
valori che lo specifico attributo potrà assumere per gli articoli
gestiti all'interno del nostro sito.

![](./assets/media/image36.png)

Questo elenco di valori ci servirà nel momento in cui dovremo andare a
valorizzare, articolo per articolo, questi stessi attributi e, come
vedremo meglio tra poco, anche per definire delle specifiche
combinazione di marca e modello utili a risolvere determinati problemi
in fase di ricerca articoli.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> degli Attributi Articolo in Passweb si veda anche il capitolo
> "Catalogo -- Gestione Attributi Articolo" di questo manuale.

Una volta creati questi due attributi dovremo poi:

- utilizzarli per creare un apposito "Set di Attributi" da associare
  alla categoria merceologia delle stampanti

![](./assets/media/image37.png)

- compilare l'anagrafica Passweb delle stampanti e delle cartucce
  inserendo per ciascuno di questi articoli i valori corretti per gli
  attributi Marca e Modello

![](./assets/media/image38.png)

A questo punto potremo realizzare un pannello di ricerca da inserire
nella pagina delle stampanti con all'interno due campi che possano
consentire all'utente di selezionare la marca e il modello della
stampante e/o delle cartucce desiderate. Inoltre, per guidare l'utente
nella sua selezione potremo, come precedentemente evidenziato,
utilizzare anche dei filtri vincolati in modo tale che, una volta
selezionata la marca, poi il campo modello mostri effettivamente i soli
modelli compatibili con la marca selezionata.

![](./assets/media/image39.png)

In queste condizioni però, l'utilizzo dei semplici filtri vincolati non
risolve completamente i nostri problemi. Supponendo infatti di
selezionare la marca HP otterremo un risultato del tipo di quello
rappresentato in figura.

![](./assets/media/image40.png)

Come risultato del filtro "Marca = HP" otterremo cioè le due stampanti
"**Photosmart 6520"**, "**D4H21B**" e le cartucce d'inchiostro **x23** e
**y25** compatibili con stampanti di marca HP.

Il filtro funziona dunque in maniera corretta ma la presenza, nei
risultati di ricerca, delle due cartucce compatibili anche con altre
marche ed altri modelli di stampanti ci porta ad ottenere un risultato
indesiderato.

Le due cartucce d'inchiostro x23 e y35 sono infatti compatibili anche
con stampanti CANON "PIXMA MX 925" e SAMSUNG "CLP 365W" per cui pur
avendo selezionato la marca HP ed avendo comunque ottenuto risultati
corretti a livello di filtro articoli, il campo "Modello" del pannello
di ricerca mostrerà anche i valori "PIXMA MX 925" e "CLP 365W" non
coerenti con la selezione effettuata per il campo marca (coerenti però
con il fatto che le due cartucce presenti come risultato del filtro di
ricerca hanno anche questi valori nel loro attributo "Modello").

Selezionando quindi il modello PIXMA MX 25 otterremo come unico
risultato la cartuccia x23 senza però la relativa stampante (di marca
CANON).

![](./assets/media/image41.png)

Questa situazione può essere migliorata utilizzando non dei semplici
filtri vincolati, ma bensì dei **filtri vincolati sulla base di
specifiche combinazioni di attributi.**

In sostanza anziché basare le possibili opzioni di scelta visualizzate
all'interno dei campi del pannello di ricerca sui valori assunti, per i
relativi attributi, dagli articoli risultati del filtro, potremo
definire esattamente le varie combinazioni di attributi possibili e fare
poi in modo che siano tali combinazioni a determinare le possibili
opzioni presenti all'interno del pannello di ricerca.

Per fare questo dovremo quindi selezionare il set di attributi
utilizzato per le stampanti, cliccare sul pulsante "**Combinazioni**"
come mostrato in figura

![](./assets/media/image42.png)

e creare le diverse combinazioni di attributi possibili (pulsante
"**Nuova Combinazione**") indicando uno specifico valore per l'attributo
marca e quelli che sono i relativi valori dell'attributo modello
coerenti con l'impostazione precedente.

![](./assets/media/image43.png)

> **NOTA BENE:** i valori utilizzabili per ogni singolo attributo sono
> esattamente quelli inseriti in fase di creazione dell'attributo stesso
> all'interno della sezione "Gestione Opzioni".

In questo modo potremo quindi creare le combinazioni di attributi
mostrate in figura

![](./assets/media/image44.png)

stabilendo ad esempio che per la marca HP dovranno essere considerati i
soli modello "Photosmart 6520" e "D4H21B"

Una volta definite le possibili combinazioni di attributi dovremo
solamente impostare il pannello di ricerca in maniera tale da utilizzare
dei filtri vincolati sulla base delle combinazioni di attributi appena
definite.

Per questo dovremo, ovviamente, impostare il parametro "Tipologia
Filtro" sul valore "Vincolato a tutti i livelli" o "Vincolato al livello
precedente" e, soprattutto, dovremo selezionare il check "**Considera le
Combinazioni di Attributi**"

![](./assets/media/image45.png)

Con queste impostazioni nel momento in cui l'utente dovesse selezionare
per il campo "Marca" il valore HP, il successivo campo "Modello"
mostrerà i soli valori "Photosmart 6520" e "D4H21B" perché, nelle
combinazioni di attributi che abbiamo definito, i soli valori possibili
per l'attributo "Modello" in corrispondenza del valore "Marca = HP" sono
proprio "Photosmart 6520" e "D4H21B"

![](./assets/media/image46.png)

Ora quindi non solo i risultati del filtro sono corretti ma anche le
possibili opzioni di scelta presenti all'interno del pannello di ricerca
sono coerenti con le selezioni effettuate dall'utente in fase di
ricerca.

Selezionando quindi per il campo "Modello" il valore "D4H21B" otterremo
come risultato del filtro la stampante HP D4H21B e la cartuccia
d'inchiostro ad essa compatibile.

> **NOTA BENE:** nel caso in cui il campo presente all'interno del
> pannello di ricerca sia relativo ad un attributo non appartenente ad
> un filtro set attributi verranno considerate per esso tutte le
> possibili combinazioni in cui è presente l'attributi stesso. In caso
> contrario verranno invece considerate le sole combinazione definite
> per lo specifico set di attributi.

