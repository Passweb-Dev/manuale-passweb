# COMPONENTE CONFIGURATORE



Il componente Configuratore

![](./assets/media/image106.png)

consente di gestire all'interno del proprio sito Ecommerce, **Articoli
Strutturati**, nel caso di siti collegati a Mexal, e **Varianti
Articolo** nel caso di siti collegati ad uno dei gestionali Ho.Re.Ca.

In ogni caso, per poter gestire correttamente all'interno del proprio
sito Ecommerce il configuratore di prodotto è obbligatorio:

- Per i siti Ecommerce collegati a Mexal **associare ad ogni elemento
  padre di struttura esportato e gestito all'interno del sito, una
  Cartella Abbinamenti**

> **ATTENZIONE!** articoli padre privi di Cartella Abbinamenti verranno
> trattati come normali articoli di Magazzino (tipo A). Per essi non
> sarà quindi possibile attivare e gestire all'interno del sito il
> relativo configuratore di prodotto.
>
> Ad ogni livello della cartella abbinamenti definita in Mexal
> corrisponderà un analogo livello di scelta del configuratore web. Allo
> stesso modo le diverse opzioni inserite in un determinato livello
> della cartella abbinamenti determineranno le possibili opzioni di
> scelta all'interno del corrispondente livello del configuratore web.
>
> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> consentire agli utenti del sito di non impostare in fase di
> configurazione web, per certi articoli, nessun valore in
> corrispondenza di un determinato livello della struttura sarà
> necessario inserire nella cartella abbinamenti di quegli stessi
> articoli, in corrispondenza dello stesso livello, un' opzione
> costituita da una stringa di tanti \# quanti sono i caratteri
> riservati per quello specifico livello.
>
> Supponendo ad esempio di avere un livello della "Struttura X"
> denominato "Marca" di 5 caratteri e di dover fare in modo che gli
> utenti del sito possano, in fase di configurazione impostare per l'
> "Articolo A" appartenente a questa struttura il campo Marca su di un
> valore vuoto, sarà necessario inserire nella cartella abbinamenti
> dell' Articolo A, in corrispondenza del livello relativo alla Marca,
> un' opzione costituita dalla seguente stringa \##### di 5 cancelletti.
>
> In queste condizioni nel momento in cui l'utente dovesse configurare
> un prodotto finito selezionando per il campo Marca l'opzione vuota
> (che sul sito potrebbe essere tradotta anche con una stringa del tipo
> "Nessuna Marca") il codice gestionale del relativo articolo avrà,
> nella porzione riservata al livello "Marca", 5 spazi vuoti.

- Per i siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.
  **creare almeno un Articolo Prototipo per ciascuna delle Varianti
  Articolo che si è deciso di gestire all'interno del sito**

Tale componente mette a disposizione dell'utente un configuratore di
prodotto, configuratore questo che potrà essere utilizzato:

- Per l'eventuale codifica di articoli figlio non ancora definiti
  all'interno del gestionale.

- Per raggruppare all'interno di un unico contenitore logico
  (rappresentato da uno specifico padre di struttura) tutta una serie di
  articoli non strutturati offrendo poi all'utente la possibilità di
  arrivare a selezionare questi stessi articoli secondo le stesse esatte
  modalità con cui si arriverebbe a configurare un articolo figlio della
  struttura in esame.

Grazie a questo componente verranno quindi inseriti all'interno della
Scheda Prodotto un insieme di controlli attraverso cui un utente del
sito potrà arrivare a scegliere, tra diverse possibili opzioni, l'esatta
configurazione dell'articolo che intende acquistare.

![](./assets/media/image107.png)

Il Configuratore di prodotto potrà comportarsi in maniera diversa a
seconda di come sono stati impostati, all'interno dell'apposita sezione
di Wizard, i parametri di configurazione e gestione delle strutture
articoli.

In questo senso, ad esempio, il parametro "**Tipologia di
Visualizzazione**" presente all'interno maschera "Modifica Struttura
Articoli" (sezione *"Catalogo -- Gestione Articoli --Strutture"*)
permette di decidere se il configuratore dovrà visualizzare tutti i
livelli di configurazione della struttura con tutte le opzioni
disponibili per ciascuno di essi, oppure se le opzioni di scelta
presenti all'interno di uno specifico livello dovranno dipendere dalle
scelte effettuate dall'utente, in fase di configurazione del prodotto,
ad uno dei livelli precedenti.

![](./assets/media/image108.png)

**Tipologia di Visualizzazione = Esploso Completamente 🡪** il
configuratore visualizzerà sempre tutti i diversi livelli della
struttura e in corrispondenza di ciascuno di essi verranno proposte
tutte le diverse possibili opzioni di scelta determinate sulla base dei
vari elementi presenti, in Mexal, nel corrispondente livello della
Cartella Abbinamenti, in Ho.Re.Ca. nel corrispondente Insieme di Valori

**Tipologia di Visualizzazione = Vincolante al precedente livello 🡪**
inizialmente verranno visualizzate solo le possibili opzioni del primo
livello della struttura. Sulla base dell'opzione selezionata ad un certo
livello verranno poi proposti gli elementi del livello successivo

In quest'ultimo caso inoltre il campo "Generazione Elementi" consente di
decidere sulla base di che cosa dovranno essere definite le diverse
possibili configurazioni di prodotto finito.

![](./assets/media/image109.png)

In particolare se impostato a:

- **Automatico:** le diverse possibili configurazioni di prodotto finto
  a cui l'utente potrà arrivare utilizzando il configuratore, saranno
  determinate sulla base degli articoli figlio già codificati sul
  gestionale e correttamente esportati all'interno del sito web

- **Manuale:** le diverse possibili configurazioni di prodotto finto a
  cui l'utente potrà arrivare utilizzando il configuratore, saranno
  determinate sulla base degli articoli figlio già codificati sul
  gestionale e/o sulla base di precise impostazioni stabilite
  dall'utente direttamente all'interno di Passweb

In ogni caso le diverse possibili opzioni tra cui un utente potrà
scegliere saranno comunque definite sulla base della Cartella
Abbinamenti associata in Mexal all'articolo padre di una determinata
struttura o, nel caso di siti Ho.Re.Ca., sulla base dell'articolo
Prototipo considerato e dei relativi Insiemi di Valori.

Dal punto di vista grafico il configuratore può assumere diversi stili
di visualizzazione dipendentemente, questa volta, da come è stato
impostato il parametro "**Modalità di Visualizzazione**" presente
anch'esso all'interno maschera "**Modifica Struttura Articoli**"
(sezione *"Catalogo -- Gestione Articoli --Strutture"*).

![](./assets/media/image110.png)

**Modalità di Visualizzazione = Lineare:** i diversi livelli della
struttura verranno visualizzati mediante i controlli grafici (Lista,
Radio, Select) impostati per ogni singolo livello in fase di
configurazione della struttura stessa.

![Videate\\modalita_visualizzazione_lineare.bmp](./assets/media/image111.png)

**ATTENZIONE!** La modalità di visualizzazione Lineare è quella adottata
a default per ogni Configuratore di prodotto

**Modalità di Visualizzazione = Tabella Esplosa:** gli ultimi due
livelli della struttura oppure l'ultimo livello più la Taglia/Colore del
prodotto (nel caso in cui ovviamente l'articolo strutturato in esame sia
gestito mediante la tabella Taglie/Colori di Mexal), verranno
visualizzati all'interno di una tabella esplosa che ha in riga tutte le
diverse possibili combinazioni del prodotto in esame, combinazioni
queste che dipenderanno, ovviamente, dal fatto di aver impostato il
parametro "Tipologia di Visualizzazione" sul valore "Esploso
Completamente" o "Vincolante al precedente livello".

![Videate\\modalita_visualizzazione_tabella_esplosa.bmp](./assets/media/image112.png)

In queste condizioni dunque nelle prime due colonne della tabella
saranno riportati i possibili valori degli ultimi due livelli della
struttura o, nel caso di articoli a Taglie/Colori, i possibili valori
dell'ultimo livello della struttura e delle Taglie/Colori del prodotto.

Nella terza colonna verranno invece mostrati i dati del relativo
articolo figlio, dati questi che dipendono esattamente da quelli che
sono gli elementi inseriti all'interno del componente "Configuratore" in
fase di creazione della Scheda Prodotto.

**Modalità di Visualizzazione = Tabella Esplosa Divisa:** gli ultimi due
livelli della struttura oppure l'ultimo livello più la Taglia/Colore del
prodotto (nel caso in cui ovviamente l'articolo strutturato in esame sia
gestito mediante la tabella Taglie/Colori di Mexal), verranno
visualizzati all'interno di una tabella esplosa che ha in riga tutte le
diverse possibili combinazioni del prodotto in esame, combinazioni
queste che dipenderanno, ovviamente, dal fatto di aver impostato il
parametro "Tipologia di Visualizzazione" sul valore "Esploso
Completamente" o "Vincolante al precedente livello"

![Videate\\modalita_visualizzazione_tabella_esplosa_divisa.bmp](./assets/media/image113.png)

A differenza della configurazione precedente (Tabella Esplosa) in questo
caso però i dati degli articoli figli non saranno più raggruppati
all'interno di un\'unica colonna ma saranno inseriti in colonne distinte
la cui intestazione coinciderà esattamente con la label dello specifico
componente inserito all'interno del componente "Configuratore" in fase
di creazione della Scheda Prodotto.

**Modalità di Visualizzazione = Tabella Matrice:** gli ultimi due
livelli della struttura oppure l'ultimo livello più la Taglia/Colore del
prodotto (nel caso in cui ovviamente l'articolo strutturato in esame sia
gestito mediante la tabella Taglie/Colori di Mexal) verranno
visualizzati all'interno di una tabella matriciale che ha in riga un
livello della struttura e in colonna l'ultimo livello della struttura o
l'elenco delle Taglie/Colori gestite per il prodotto in esame

![Videate\\modalita_visualizzazione_tabella_matrice.bmp](./assets/media/image114.png)

In queste condizioni ogni cella della tabella, determinata dall'incrocio
riga/colonna, individuerà un possibile articolo figlio i cui dati
saranno quindi inseriti all'interno della cella stessa.

Anche in questo caso le possibili combinazioni di articoli figli
dipenderanno, ovviamente, dal fatto di aver impostato il parametro
"Tipologia di Visualizzazione" sul valore "Esploso Completamente" o
"Vincolante al precedente livello"

**NOTA BENE:** per maggiori informazioni relativamente alle diverse
possibili opzioni di configurazione e di visualizzazione per il
Configuratore Articoli si vedano anche le sezioni "Catalogo -- Gestione
Articoli -- Strutture Ecommerce Mexal / Ho.Re.Ca." di questo manuale.

Per quel che riguarda **la determinazione del prezzo dei vari articoli
acquistati mediante Configuratore** di prodotto è bene sottolineare che:

- **Nel caso di siti Ecommerce collegati a Mexal** è possibile inserire
  all'interno della Cartella Abbinamenti anche articoli modificatori
  (tipo M) articoli cioè che verranno utilizzati per arrivare a
  determinare il prezzo del prodotto finito sulla base delle scelte
  effettuate dall'utente in fase di configurazione del prodotto.

> Tali articoli sono gestiti anche all'interno di Passweb, per cui se
> correttamente esportati consentiranno di determinare, anche
> all'interno del sito, il prezzo di un prodotto finito sulla base delle
> varie scelte effettuate dall'utente in fase di configurazione del
> prodotto stesso.

- **Nel caso invece di siti Ecommerce collegati ad uno dei gestionali
  Ho.Re.Ca**. non potendo disporre di articoli modificatori che possano
  contribuire in qualche modo alla determinazione del prezzo
  dell'articolo figlio sulla base delle scelte effettuate dall'utente in
  fase di configurazione del prodotto, diventa di fondamentale
  importanza il livello della Variante Articolo a partire dal quale
  verrà poi generato il Prototipo.

> Il prezzo del Prototipo verrà infatti applicato, a default, anche a
> tutte le altre possibili configurazioni di prodotto finito e l'unica
> possibilità di ottenere un articolo figlio con un prezzo diverso dal
> prototipo sarà quella di codificarlo all'interno del gestionale,
> assegnarli il suo specifico prezzo ed esportarlo all'interno del sito.

In effetti, indipendentemente dal fatto di considerare siti Ecommerce
collegati a Mexal o ad uno dei gestionali Ho.Re.Ca., nel momento in cui
**sul database di Passweb dovesse già essere presente un articolo
corrispondente a quello configurato dall'utente in fase di acquisto,
oppure all' "Articolo Alternativo" eventualmente associato alla
configurazione di prodotto in esame, allora sarà esattamente il prezzo
di quell'articolo ad essere considerato ed utilizzato come prezzo di
vendita.**

**NOTA BENE:** se il prezzo ottenuto a seguito di una certa
configurazione di prodotto dovesse essere, per svariate ragioni, diverso
da quello originale, verrà sostituito al prezzo inizialmente
visualizzato per l'articolo padre e il cambiamento verrà notificato con
un'apposita animazione sul campo Prezzo

**ATTENZIONE!** Il prezzo dell'articolo padre (quello da cui parte la
configurazione del prodotto) può essere visualizzato o meno all'interno
del "Catalogo E-commerce", dipendentemente dal fatto di aver selezionato
o meno il parametro **"Visualizzare in catalogo il prezzo dell\'articolo
padre".** Per maggiori informazioni in merito si veda anche la sezione
"*Catalogo -- Gestione Articoli -- Strutture Ecommerce Mexal /
Ho.Re.Ca."* di questo manuale.

Una volta completata la configurazione di un prodotto, oltre al prezzo,
potrebbero poi essere aggiornate automaticamente anche tutte le
informazioni presenti all'interno della scheda prodotto passando da
quelle iniziali, relative all'articolo padre, a quelle relative invece
allo specifico prodotto finito che si è arrivati a configurare.

Questo comportamento dipende essenzialmente da due diversi fattori:

- dalla specifica modalità di visualizzazione impostata per il
  configuratore (**lineare** o **tabellare**)

- da come è stato impostato il parametro "**Riferimento Articoli
  Strutturati**" presente nella maschera di configurazione del singolo
  componente "**Scheda Prodotto**"

**[CONFIGURATORE CON MODALITA' DI VISUALIZZAZIONE LINEARE]{.underline}**

In queste condizioni i dati presenti all'interno di una determinata
scheda prodotto possono passare da quelli del padre a quelli dello
specifico articolo figlio al verificarsi delle seguenti condizioni:

- l'articolo figlio che si è arrivati a configurare è già stato
  codificato sul gestionale ed è stato anche correttamente esportato
  all'interno del sito

- il parametro "**Riferimento Articoli Strutturati**" presente nella
  maschera di configurazione dello specifico componente "**Scheda
  Prodotto**" è stato impostato sul valore "**Figlio**"

![](./assets/media/image115.png)

Se entrambe le condizioni sopra indicate dovessero essere soddisfatte
una volta completata la configurazione dell'articolo figlio tutte le
informazioni inizialmente visualizzate all'interno della scheda prodotto
e riferite all'articolo padre (immagini, prezzo, singoli Attributi
Articolo, interi Set di Attributi ...), verranno automaticamente
aggiornate e sostituite dalle stesse informazioni relative però allo
specifico prodotto finito.

**ATTENZIONE! Affinchè anche all'interno del componente "Abbinati"
vengano visualizzati gli articoli abbinati allo specifico prodotto
finito è necessario inserire tale componente all'interno della "Scheda
Prodotto". In caso contrario verranno visualizzati sempre e comunque gli
abbinati dell'articolo padre di struttura**

Al contrario nel momento in cui la configurazione di prodotto finito
indicata non dovesse corrispondere ad un prodotto finito correttamente
esportato e gestito all'interno del sito oppure il parametro
"**Riferimento Articoli Strutturati**" dovesse essere impostato sul
valore "**Padre**", allora una volta configurato il prodotto finito le
informazioni presenti all'interno della scheda prodotto rimarranno
sempre e comunque quelle iniziali dell'articolo padre.

**[CONFIGURATORE CON MODALITA' DI VISUALIZZAZIONE
TABELLARE]{.underline}**

Nel momento in cui per il configuratore dovesse essere impostata una
modalità di visualizzazione tabellare (Tabella Esplosa, Tabella Esplosa
Divisa, Tabella Matrice) le diverse possibili configurazioni di prodotto
finto verranno inserite direttamente all'interno della relativa tabella.

In queste condizioni quindi **non verrà mai ricaricata la scheda
prodotto dell'articolo padre per visualizzare le informazioni di uno
specifico articolo figlio** in quanto tali informazioni saranno già
presenti nella visualizzazione tabellare del configuratore all'interno
della cella relativa a quello stesso articolo figlio.

Infine, è bene ricordare anche che:

- Nel caso in cui un utente tenti di inserire in carrello un articolo
  non completamente configurato (senza aver cioè impostato un'opzione
  per ogni livello del configuratore), verrà avviata un'animazione che
  modifica il background dei campi non valorizzati, e l'articolo non
  sarà inserito in Carrello. Impostando un'opzione per ogni livello del
  configuratore e cliccando poi sul pulsante "Aggiungi al Carrello"
  l'articolo verrà ovviamente inserito e potrà essere correttamente
  acquistato.

- Nel momento in cui il configuratore dovesse operare nelle condizioni
  di seguito indicate:

  - Tipologia di visualizzazione = Vincolante al precedente livello

  - Modalità di Visualizzazione = Lineare

  - Gestione Acquisto = Acquista solo se disponibile

> e dovesse essere presente una sola configurazione possibile di
> prodotto finito (perché è gestito effettivamente un unico figlio e/o
> perché gli altri articoli figli risultano al momento non disponibili e
> quindi non acquistabili), allora accedendo alla pagina prodotto del
> padre di struttura i diversi livelli del configuratore verranno
> automaticamente precompilati con l'unica opzione disponibile e
> all'utente verrà quindi mostrata, automaticamente, la scheda prodotto
> dell'unico articolo figlio effettivamente acquistabile
>
> **ATTENZIONE!** Nelle condizioni indicate verrà effettuata in maniera
> automatica solo la preselezione delle opzioni presenti nei diversi
> livelli del configuratore. Dovrà quindi essere sempre l'utente ad
> aggiungere definitivamente l'articolo in carrello

- Nel caso in cui l'articolo configurato dall'utente in fase di acquisto
  non fosse ancora presente nelle anagrafiche del gestionale,
  contestualmente all'inserimento dell'ordine verrà anche codificato il
  nuovo articolo utilizzando per questo le logiche proprie del
  gestionale.

> In particolare, nel caso di Mexal, i nuovi articoli così codificati
> nasceranno con **il campo "Trasferisci sul sito" della videata Passweb
> a N** e per essi verranno anche azzerati tutti i listini (questo
> perché sul sito i prezzi vengono calcolati in base al prezzo
> dell'articolo padre e ad eventuali articoli modificatori)

