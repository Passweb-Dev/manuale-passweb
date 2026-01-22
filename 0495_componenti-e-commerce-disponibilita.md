# COMPONENTI E-COMMERCE -- DISPONIBILITA'



Il Componente **"Disponibilità"**

![](./assets/media/image575.png)

consente di inserire all'interno del corrispondente Componente Ecommerce
di primo livello, un pulsante attraverso cui poter richiedere, per lo
specifico articolo, diversi tipi di disponibilità (tra cui anche la
disponibilità in tempo reale)

Grazie a questo componente è quindi possibile, ad esempio, aprire una
connessione istantanea con il gestionale a seguito della quale verrà
visualizzata, dipendentemente dalle impostazione di configurazione del
componente stesso **l'Esistenza**, la **Disponibilità Netta, la**
**Disponibilità Lorda** ecc... del relativo articolo.

E' inoltre possibile scegliere se visualizzare il valore numerico della
disponibilità oppure un valore simbolico definito dall'utente e
corrispondente a ben precise fasce di livello (es. semaforo rosso per
disponibilità uguali a zero, semaforo arancione per disponibilità tra 0
e 10, semaforo verde per disponibilità maggiori di 10 ecc...).

> **NOTA BENE:** la disponibilità in oggetto potrà essere richiesta sul
> magazzino dell'ordine, sull'insieme dei magazzini gestiti in Mexal
> oppure su un sottoinsieme personalizzato di tali magazzini.

Il testo del pulsante "**Disponibilità**" è personalizzabile alla pagina
"Gestione Testi/Messaggi Sito" agendo sul componente "Disponibilità"

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata **la sua maschera di gestione e
configurazione**

![](./assets/media/image576.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di definire un nome per il Componente "Disponibilità"
che si sta editando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Label:** consente di impostare una label che verrà poi visualizzata
all'interno del sito in corrispondenza del componente in oggetto

**Mostra:** consente di impostare la visibilità del componente sul front
end del sito in relazione alla modalità di acquisto dello specifico
articolo. E' possibile selezionare uno dei seguenti valori:

- **Sempre:** selezionando questa opzione il componente sarà sempre
  visibile sul front end del sito indipendentemente dal fatto che lo
  specifico [articolo]{.underline} possa essere acquistato sempre o solo
  se disponibile

- **Solo se Acquista Sempre:** selezionando questa opzione il componente
  sarà visibile sul front end del sito solo ed esclusivamente nel caso
  in cui la modalità di acquisto dello specifico articolo sia stata
  impostata sul valore "Acquista Sempre"

- **Solo se Acquista se disponibile**: selezionando questa opzione il
  componente sarà visibile sul front end del sito solo ed esclusivamente
  nel caso in cui la modalità di acquisto dello specifico articolo sia
  stata impostata sul valore "Acquista se disponibile"

Per maggiori informazioni relativamente alle modalità di acquisto degli
articoli presenti in catalogo si veda anche la sezione *"Catalogo --
Configurazione Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca. --
Disponibilità"* di questo manuale

**Disponibilità:** consente di impostare il tipo di disponibilità che
verrà visualizzata \\ richiesta cliccando sul corrispondente pulsante.

E' possibile selezionare uno dei seguenti valori:

- **Richiesta in tempo reale:** in questo caso il pulsante "Verifica
  Disponibilità" consentirà di richiedere, **direttamente al gestionale
  e in tempo reale**, la disponibilità dello specifico articolo.

> Tale disponibilità verrà calcolata prendendo in considerazione la
> formula specificata all'interno del successivo campo "**Formula della
> Disponibilità**" valutata sul totale dei magazzini indicati
> all'interno del successivo parametro "**Disponibilità del Magazzino**"

- **Richiesta in tempo reale divisa per magazzino:** selezionando questa
  opzione, come nel caso precedente, il pulsante "Verifica
  Disponibilità" consentirà di richiedere **direttamente al gestionale e
  in tempo reale** la disponibilità dello specifico articolo.

> In queste condizioni però la disponibilità richiesta verrà
> visualizzata suddivisa per singolo magazzino.
>
> I magazzini considerati sono, anche in questo caso, quelli indicati in
> corrispondenza del campo "Disponibilità del Magazzino". Allo stesso
> modo la formula utilizzata per il calcolo della disponibilità sarà
> ancora quella indicata in corrispondenza del successivo campo "Formula
> della Disponibilità"
>
> **ATTENZIONE! Nel caso in cui si decida di attivare questa
> funzionalità occorre tenere conto del fatto che in fase di
> sincronizzazione verranno ricalcolate ed aggiornate ogni volta tutte
> le disponibilità degli articoli presenti per tutti i magazzini
> gestiti. In conseguenza di ciò i tempi di sincronizzazione potrebbero
> aumentare anche notevolmente in relazione al numero di articoli
> (soprattutto quelli gestiti a taglie) e di magazzini gestiti.**

- **Aggiornata all'ultima sincronizzazione:** in questo caso verrà
  visualizzato immediatamente, senza dover dunque cliccare su nessun
  pulsante, il valore della disponibilità aggiornato all'ultima
  sincronizzazione.

> **Non verranno quindi richiesti dati in tempo reale al gestionale** ma
> verranno semplicemente elaborati i dati esportati dal gestionale
> all'ultima sincronizzazione e memorizzati all'interno del database di
> Passweb.
>
> [In particolare, in queste condizioni, il/i magazzino/i e la formula
> considerata per il calcolo della disponibilità saranno esattamente
> quelli impostati alla pagina "Catalogo -- Configurazione Parametri-
> Catalogo Mexal" del Wizard nella sezione Disponibilità]{.underline}.

![](./assets/media/image577.png)

> Per maggiori informazioni in merito si veda anche il corrispondente
> capitolo ("*Catalogo -- Configurazione Parametri Catalogo -- Catalogo
> Mexal / Horeca - Disponibilità*") di questo manuale.

- **Aggiornata all'ultima sincronizzazione divisa per magazzino:**
  selezionando questa opzione, come nel caso precedente, verrà
  visualizzato immediatamente, senza nessuna richiesta in tempo reale al
  gestionale, il valore della disponibilità aggiornato all'ultima
  sincronizzazione.

> A differenza del caso precedente però il valore della disponibilità
> verrà ora visualizzato suddiviso per singolo magazzino.
>
> I magazzini considerati sono, anche in questo caso, quelli indicati in
> corrispondenza del campo "Disponibilità del Magazzino" presente
> all'interno della maschera "Configurazione Parametri Catalogo" del
> Wizard, campo questo che, in queste condizioni, dovrebbe ovviamente
> essere impostato sul valore "Personalizzato" o su "Tutti i magazzini".
>
> **ATTENZIONE! Nel caso in cui si decida di attivare questa
> funzionalità occorre tenere conto del fatto che in fase di
> sincronizzazione verranno ricalcolate ed aggiornate ogni volta tutte
> le disponibilità degli articoli presenti per tutti i magazzini
> gestiti. In conseguenza di ciò i tempi di sincronizzazione potrebbero
> aumentare anche notevolmente in relazione al numero di articoli
> (soprattutto quelli gestiti a taglie) e di magazzini gestiti.**

- **Aggiornata all'ultima sincronizzazione con possibilità di richiesta
  in tempo reale:** in questo caso verrà visualizzato inizialmente, e
  senza dover cliccare su nessun pulsante, il valore della disponibilità
  aggiornato all'ultima sincronizzazione, esattamente come indicato per
  il caso precedente.

> A differenza del caso precedente, in queste condizioni sarà poi
> possibile cliccare sul pulsante "Verifica Disponibilità", in maniera
> tale da aggiornare il valore inizialmente visualizzato con il
> corrispondente valore richiesto e prelevato direttamente dal
> gestionale in tempo reale.
>
> [Anche in questo caso il/i magazzino/i e la formula considerata per il
> calcolo della disponibilità saranno esattamente quelli impostati alla
> pagina "Catalogo -- Configurazione Parametri -- Catalogo Mexal" del
> Wizard nella sezione Disponibilità]{.underline}.

- **Aggiornata all'ultima sincronizzazione divisa per magazzino con
  possibilità di richiesta in tempo reale:** selezionando questa
  opzione, come nel caso precedente, verrà visualizzato inizialmente, e
  senza dover cliccare su nessun pulsante, il valore della disponibilità
  aggiornato all'ultima sincronizzazione con in più il pulsante
  "Verifica Disponibilità" da utilizzare per aggiornare il valore
  iniziale con quelli richiesti in tempo reale al gestionale.

> A differenza del caso precedente, in queste condizioni inoltre sia il
> valore della disponibilità visualizzato inizialmente che quello
> ottenuto come esito della richiesta effettuata in tempo reale al
> gestionale, sarà suddiviso per singolo magazzino.
>
> I magazzini considerati sono, anche in questo caso, quelli indicati in
> corrispondenza del campo "Disponibilità del Magazzino" presente
> all'interno della maschera "Configurazione Parametri Catalogo" del
> Wizard, campo questo che, in queste condizioni, dovrebbe ovviamente
> essere impostato sul valore "Personalizzato" o su "Tutti i magazzini".
>
> **ATTENZIONE! Nel caso in cui si decida di attivare questa
> funzionalità occorre tenere conto del fatto che in fase di
> sincronizzazione verranno ricalcolate ed aggiornate ogni volta tutte
> le disponibilità degli articoli presenti per tutti i magazzini
> gestiti. In conseguenza di ciò i tempi di sincronizzazione potrebbero
> aumentare anche notevolmente in relazione al numero di articoli
> (soprattutto quelli gestiti a taglie) e di magazzini gestiti.**

Relativamente ai valori della disponibilità aggiornati all'ultima
sincronizzazione e memorizzati in Passweb, va inoltre ricordato che, **a
seguito dell'acquisto di un determinato articolo, il numero di elementi
acquistati verrà sottratto al valore della disponibilità memorizzata in
Passweb, per quello stesso articolo, solo ed esclusivamente dopo
l'inserimento nel gestionale del relativo ordine.**

In particolare subito dopo aver inserito l'ordine all'interno del
gestionale l'applicazione andrà a rileggere dal gestionale stesso tutti
i dati necessari per ricalcolare la disponibilità degli articoli
inseriti in ordine, secondo la specifica formula di calcolo selezionata
e andrà poi ad aggiornare quelli che sono i corrispondenti valori
presenti nel database di Passweb (tutto questo, ovviamente, solo nel
caso in cui si sia deciso di gestire una disponibilità aggiornata
all'ultima sincronizzazione).

**NOTA BENE:** l'aggiornamento delle disponibilità memorizzate nel
database di Passweb a seguito dell'inserimento di un nuovo ordine
riguarda solo ed esclusivamente gli articoli presenti all'interno
dell'ordine stesso.

**ATTENZIONE!** Le disponibilità articolo e soprattutto la modalità di
gestione adottata per queste stesse disponibilità, potranno influire
sulla possibilità da parte degli utenti di acquistare o meno determinati
articoli. Per maggiori informazioni in merito si veda anche la sezione
*"Configurazione Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca."* di
questo manuale.

**Visualizza il totale dei magazzini:** visualizzato solo nel caso in
cui il precedente parametro "Disponibilità" sia impostato su uno dei
seguenti valori:

- Richiesta in tempo reale divisa per magazzino

- Aggiornata all'ultima sincronizzazione divisa per magazzino

- Aggiornata all'ultima sincronizzazione divisa per magazzino con
  possibilità di richiesta in tempo reale

Permette di decidere se, oltre al valore della disponibilità suddiviso
per singolo magazzino, dovrà o meno essere mostrata, per il relativo
articolo, anche la disponibilità totale sui magazzini selezionati.

**ATTENZIONE! Nel caso di articoli composti (es. Campionari o DBA
gestite con disponibilità sui singoli componenti) non è detto che la
disponibilità totale sui magazzini selezionati coincida esattamente con
la somma delle disponibilità sul singolo magazzino.**

In queste condizioni infatti la disponibilità dell'articolo composto è
determinata sempre dalle disponibilità dei singoli componenti.

Potremmo quindi trovarci in una situazione in cui un componente, che
deve essere presente nel campionario in quantità 2, risulti disponibile
solo su due dei magazzini selezionati ma in quantità 1 su ciascuno di
essi.

In questo caso quindi il Campionario risulterà non disponibile sui
singoli magazzini mentre potrà avere disponibilità uguale a 1 sul totale
dei magazzini selezionati (e questo proprio perché la disponibilità del
componente in esame sul totale dei magazzini indicati è pari a 2).

**Visualizzazione Magazzini:** visualizzato solo nel caso in cui il
precedente parametro "Disponibilità" sia impostato su uno dei seguenti
valori:

- Richiesta in tempo reale divisa per magazzino

- Aggiornata all'ultima sincronizzazione divisa per magazzino

- Aggiornata all'ultima sincronizzazione divisa per magazzino con
  possibilità di richiesta in tempo reale

Consente di definire come dovranno essere visualizzate, graficamente, le
disponibilità dei singoli magazzini selezionando, in questo senso, una
tra le seguenti opzioni: **In linea, Incolonnato**, **Tabellare**.

**Disponibilità del Magazzino:** visualizzato solo nel caso in cui il
precedente parametro "Disponibilità" sia stato impostato sul valore
"Richiesta in tempo reale".

Consente di indicare il o i magazzini Mexal su cui richiedere la
disponibilità in tempo reale dello specifico articolo. E' possibile
selezionare uno dei seguenti valori:

- **Magazzino dell'ordine:** selezionando questo valore il componente
  consentirà di richiedere la disponibilità in tempo reale sul magazzino
  indicato all'interno del campo "**Numero del Magazzino**" presente
  nella maschera di "**Configurazione Ordini**" del Wizard.

![](./assets/media/image578.png)

- **Tutti i Magazzini:** selezionando questo valore il componente
  consentirà di richiedere la disponibilità sul totale dei magazzini
  Mexal attualmente gestiti (verrà quindi effettuata e visualizzata la
  sommatoria delle disponibilità dello specifico articolo su tutti i
  magazzini Mexal).

- **Personalizzato:** selezionando questo valore verrà visualizzato
  l'elenco dei magazzini Mexal attualmente gestiti. A fianco di ciascun
  magazzino comparirà un apposito check di selezione. L'utente potrà
  quindi selezionare l'insieme dei magazzini su cui effettuare la
  richiesta in tempo reale della disponibilità dello specifico articolo.

![](./assets/media/image579.png)

**Formule della Disponibilità:** visualizzato solo nel caso in cui il
precedente parametro "Disponibilità" sia stato impostato sul valore
"Richiesta in tempo reale".

Consente di impostare, selezionandola tra le opzioni disponibili
all'interno del corrispondente menu a tendina, la specifica formula che
dovrà essere utilizzata per il calcolo della disponibilità da richiedere
a Mexal e conseguentemente da visualizzare all'interno del sito.

**Disponibilità Totale per Articoli a Taglie (solo Ecommerce Mexal):**
consente di specificare se, in relazione agli articoli gestiti in Mexal
mediante la tabelle Taglie/Colori dovrà essere visualizzata una
disponibilità per singola Taglia/Colore (parametro impostato a NO)
oppure se dovrà essere visualizzato un unico valore comprensivo di tutte
le disponibilità delle varie Taglie/Colori

**Visualizza solo taglie disponibili (solo per articoli a Taglie):** se
impostato a **SI** consente di ottenere e visualizzare sul sito le sole
taglie effettivamente disponibili. Se impostato a **NO**, a seguito di
una richiesta di disponibilità verranno invece visualizzate sia le
taglie con disponibilità maggiore di zero sia quelle con disponibilità
pari a 0.

**ATTENZIONE!** L'effettiva visualizzazione delle taglie / colori a
disponibilità minore o uguale a zero è sempre da mettere in relazione
anche a quanto impostato per il parametro "**Mostra solo le taglie
disponibili"** presente nella maschera di configurazione della relativa
serie. Per maggiori informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Catalogo -- Gestione Articoli -- Taglie o
Colori / Ecommerce Mexal -- Configurazione di una serie di taglie*" di
questo manuale

**Visualizzazione Taglie (solo per articoli a Taglie):** consente di
definire come dovranno essere visualizzate graficamente le disponibilità
in relazione ad articoli gestiti a Taglie /Colori selezionando una tra
le seguenti opzioni: **In linea, Incolonnato**, **Tabellare**

**Visualizzazione:** consente di decidere se visualizzare il valore
numerico della disponibilità (**Numero**) o un valore simbolico
(**Fascia**) definito dall'utente e corrispondente a ben precise fasce
di livello definite attraverso il successivo campo **"Gestione
Scaglioni"**

**Gestione Scaglioni:** consente di impostare due o più scaglioni di
disponibilità indicando anche, per ciascuno di essi, il corrispondente
valore che dovrà poi essere visualizzato sul front end del sito nel
momento in cui la disponibilità effettiva del prodotto dovesse ricadere
all'interno di quello stesso scaglione

**ATTENZIONE!** Questi scaglioni verranno presi in considerazione ed
applicati solo nel caso in cui il precedente campo "**Visualizzazione**"
sia stato impostato sul valore **Fascia**

![](./assets/media/image580.png)

Per aggiungere un nuovo scaglione è sufficiente cliccare sull'icona
raffigurante un piccolo +. In questo modo verrà infatti visualizzata,
nella parte destra della finestra, la maschera **"Nuovo Scaglione"**
attraverso cui poter impostare:

- i valori di partenza e di arrivo dello scaglione -- campi **Da -- A**

- il testo o l'immagine da visualizzare sul front end del sito nel
  momento in cui la disponibilità effettiva del prodotto dovesse
  ricadere all'interno di quello stesso scaglione -- campi "**Testo**" /
  "**Immagine**"

In merito alla definizione di questi scaglioni occorre poi ricordare
che:

- Il valore minimo ammesso per il campo "Da" è zero

- Le fasce devono essere contigue.

- Nel caso in cui non venga indicato uno specifico valore per il campo A
  la corrispondente fascia verrà considerata come non limitata
  superiormente

- Nel caso in cui la disponibilità restituita da Mexal sia negativa il
  valore verrà automaticamente convertito in **zero**

- La disponibilità ritornata dal gestionale ricade sempre nella fascia
  in cui il suo valore risulta essere maggiore o uguale al campo "Da" e
  minore del campo "A"

- Nella definizione dei vari scaglioni è possibile utilizzare,
  all'interno dei campi DA e A (pulsante "**Aggiungi segnaposto**"),
  anche il segnaposto "**x**" che verrà poi sostituito a runtime con il
  valore impostato per il relativo articolo in corrispondenza del campo
  "**Soglia Disponibilità**". Per maggiori informazioni in merito si
  veda anche quanto indicato all'interno del capitolo "*Catalogo --
  Configurazione Parametri Catalogo -- Catalogo Mexal / Horeca --
  Disponibilità*" di questo manuale.

> Il segnaposto "x" consente quindi di definire degli scaglioni
> dinamici, diversi da prodotto a prodotto e basati sul valore della
> "Soglia Disponibilità" impostata per ciascuno di essi

- Nella definizione dei vari scaglioni è possibile utilizzare anche

  - **gli operatori standard (+-\*/)**

  - **elevatore a potenza (Pow)**

> [Esempio]{.underline}: supponendo di voler calcolare il valore
> dell'espressione "due alla terza" la formula da utilizzare dovrà
> essere:
>
> **Pow(2,3)**

- **radice quadrata (Sqrt)**

> [Esempio]{.underline}: supponendo di voler calcolare il valore
> dell'espressione "radice quadrata di 16" la formula da utilizzare
> dovrà essere:
>
> **Sqrt(16)**

- **modulo (%)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma:
>
> **10%3**
>
> e consentirà di dividere il primo argomento per il secondo,
> restituendo come risultato solo il resto (nell'esempio indicato il
> risultato ottenuto sarà 1)

- **valore assoluto (Abs)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Abs(-5)**
>
> e consentirà di ottenere come risultato il valore assoluto del numero
> indicato tra parentesi (nell'esempio indicato il risultato ottenuto
> sarà 5)

- **valore intero (Truncate)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Truncate(5.2)**
>
> e consentirà di ottenere come risultato il valore intero del numero
> indicato tra parenesi (nell'esempio considerato il risultato ottenuto
> sarà 5)

- **valore intero superiore (Ceiling)**

> [Esempio]{.underline}: questo operatore dovrà essere utilizzato nella
> forma
>
> **Ceiling(5.2)**
>
> e consentirà di ottenere come risultato il valore intero
> immediatamente superiore al numero indicato tra parentesi
> (nell'esempio indicato il risultato ottenuto sarà 6)

- **parentesi tonde**

- **istruzione condizionale "if"**

> All'interno della formula è possibile utilizzare anche l'istruzione
> condizionale "if" come operatore ternario quindi nel formato
>
> **if(condizione, valore da applicare se condizione verificata, valore
> da applicare se condizione non verificata)**
>
> **ATTENZIONE!** E' fondamentale che come separatore dei decimali venga
> utilizzato sempre e soltanto il "." (punto).
>
> Nel caso in cui si dovesse utilizzare come separatore la "," (virgola)
> la formula non risulterà essere corretta e il risultato ottenuto non
> sarà quindi quello desiderato.

- Per quel che riguarda il valore da visualizzare sul front end del sito
  nel momento in cui la disponibilità effettiva del prodotto dovesse
  ricadere all'interno di quello stesso scaglione è possibile inserire
  un testo generico (es. ALTA, MEDIA, BASSA), un'immagine (es. semaforo
  verde giallo o rosso) o, in alternativa, è possibile utilizzare anche
  il segnaposto "**Disponibilità**" (\$availability\$) che verrà poi
  sostituito, a runtime, con l'esatto valore della disponibilità dello
  specifico prodotto ritornata dal gestionale

> **NOTA BENE:** nel caso in cui il server Mexal non dovesse essere
> reperibile o il valore ottenuto non appartenesse a nessuna delle fasce
> indicate, sul sito verrà visualizzato il carattere **\"-\"**.

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- Il pulsante per la richiesta della disponibilità

- I valori delle disponibilità

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

Occorre infine considerare che

- **nel caso in cui l'articolo sia strutturato** il componente
  "Disponibilità" verrà visualizzato anche sull'articolo padre di
  struttura piuttosto che soltanto nel momento in cui l'utente arrivi a
  configurare un articolo figlio effettivamente esportato e gestito
  all'interno del sito, dipendentemente dal fatto di aver selezionato o
  meno il campo "**Mostra la disponibilità dell'articolo padre**"
  presente tra i parametri di configurazione della relativa struttura
  (per maggiori informazioni in merito si veda anche il capitolo
  "*Catalogo -- Gestione Articoli -- Strutture / Ecommerce Mexal --
  Strutture -- Modifica Struttura*" di questo manuale)

- nel caso in cui il prodotto per il quale si richiede la disponibilità
  dovesse essere **un articolo Campionario, un articolo di tipo DBA (per
  cui si sia deciso di gestire la disponibilità sui componenti) o un
  articolo Composto (Ecommerce Ho.Re.Ca.)** verrà restituita e
  visualizzata all'interno del sito la disponibilità del prodotto in
  relazione a quelle che sono le effettive disponibilità dei singoli
  componenti (determinate anche sulla base di eventuali formule
  impostate all'interno del gestionale).

Supponendo dunque di avere a che fare con un articolo Campionario
composto da:

  -----------------------------------------------------------------------
       **COMPONENTE            **QUANTITA'**         **DISPONIBILITA'
       CAMPIONARIO**                                   COMPONENTE**
  ----------------------- ----------------------- -----------------------
        ARTICOLO 1                   2                      10

        ARTICOLO 2                   1                       3

        ARTICOLO 3                   1                       6
  -----------------------------------------------------------------------

il valore ritornato per la disponibilità di questo componente sarebbe 3.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

**ATTENZIONE! Nel caso di articoli Composti (Ecommerce Ho.Re.Ca.) la
disponibilità verrà valutata in relazione non solo a quella che è la
disponibilità dei singoli Componenti ma tendo in considerazione anche la
disponibilità dello stesso Articolo Composto**

