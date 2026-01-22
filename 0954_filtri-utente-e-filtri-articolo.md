# FILTRI UTENTE E FILTRI ARTICOLO



In Passweb è possibile associare ad ogni gruppo di utenti tre diverse
tipologie di filtri:

- **filtri articolo**: insieme di regole utilizzate per definire gli
  articoli che potranno essere visualizzati, e conseguentemente
  acquistati, dagli utenti appartenenti allo specifico gruppo

- **filtri utente:** insieme di regole che definiscono i criteri di
  appartenenza degli utenti ad uno specifico gruppo

- **filtri cliente agente:** insieme di regole mediante le quali poter
  applicare il filtro articoli definito sullo stesso gruppo solo ed
  esclusivamente ai clienti che soddisfano queste regole e che sono
  gestiti dagli agenti appartenenti al gruppo stesso

![](./assets/media/image136.png)

##### FILTRI ARTICOLO

Un **Filtro Articoli** altro non è se non un insieme di regole
utilizzate per definire l'insieme di articoli che potranno essere
visualizzati, e conseguentemente acquistati, dai vari utenti
appartenenti ad uno specifico gruppo.

**Nel momento in cui, dunque, si decida di associare ad uno specifico
gruppo utenti dei filtri articolo, poi gli utenti di quel gruppo avranno
la possibilità di visualizzare e conseguentemente di acquistare
all'interno del sito i soli articoli che soddisfano il filtro
impostato.**

Per creare un nuovo filtro articoli sarà necessario portarsi nella
maschera di configurazione delle proprietà del gruppo desiderato ed
agire dalla corrispondente sezione "**Filtro Articoli**".

![](./assets/media/image137.png)

Cliccando sul pulsante **"Aggiungi un nuovo filtro"** verranno
visualizzati i campi su cui poter impostare la condizione che definirà,
per gli utenti appartenenti al gruppo in esame, il criterio di
visualizzazione degli articoli all'interno del sito web.

![](./assets/media/image138.png)

Il campo di input presente nella parte alta del piccolo pop up consente,
digitando almeno 3 caratteri, di filtrare gli elementi presenti in
elenco.

Nello specifico poi il campo:

- **Codice:** consente di definire il filtro articoli sulla base del
  loro codice gestionale

- **Categoria:** consente di definire il filtro articoli sulla base del
  loro gruppo merceologico di appartenenza. Utilizzando questo campo
  sarà quini possibile, ad esempio, selezionare tutti gli articoli
  appartenenti a una determinata categoria merceologica.

> **ATTENZIONE!** in questo caso non verranno fatte distinzioni tra
> categorie primarie o secondare e verrà quindi valutata l'appartenenza
> degli articoli alle categorie merceologiche indicate indipendentemente
> dal fatto che queste siano la sua categoria primaria (definita
> all'interno del gestionale) o una delle categorie secondarie

- **Categoria Primaria:** come nel caso precedente consente di definire
  il filtro articoli sulla base del loro gruppo merceologico di
  appartenenza. A differenza del caso precedente questa volta verranno
  però prese in considerazione le sole categorie merceologiche primarie

- **Disponibilità:** consente di definire il filtro articoli sulla base
  della loro disponibilità **memorizzata localmente** sul database del
  sito. Grazie a questo campo sarà quindi possibile selezionare, ad
  esempio, tutti gli articoli a disponibilità maggiore di zero e/o
  maggiore di un certo numero specificato in fase di definizione della
  regola di filtro.

> **ATTENZIONE:** la disponibilità considerata nei filtri articolo è
> solo ed esclusivamente quella memorizzata localmente sul database del
> sito aggiornata dunque all'ultima sincronizzazione e/o all'ultima
> operazione utile (es. nuovi ordini inserti nel gestionale). Non viene
> considerata, in questo senso, la disponibilità in tempo reale
> memorizzata per i vari articoli all'interno del gestionale.
>
> Per maggiori informazioni relativamente alla gestione della
> disponibilità articolo in locale sul proprio sito ecommerce si veda
> anche la sezione *"Catalogo -- Configurazione Parametri -- Catalogo
> Mexal / Ho.Re.Ca."* di questo manuale.

- **Gestione Acquisto:** consente di definire il filtro articoli sulla
  base di quella che è la loro specifica modalità di acquisto ("Acquista
  sempre" oppure "Acquista solo se disponibile")

- **Offerte/Novità/Fine Serie:** consente di definire il filtro articoli
  sulla base del fatto che un certo articolo compaia o meno all'interno
  delle Offerte, delle Novità o dei Fine Serie

- **Prezzo a richiesta:** consente di impostare il filtro articoli in
  base al fatto che per lo specifico prodotto sia stata attivata o meno
  la funzionalità di "Prezzo a richiesta"

- **Categoria Statistica:** consente di definire il filtro articoli
  sulla base della loro "Categoria Statistica".

- **Visualizza in negozio:** consente di impostare il filtro articoli in
  base al fatto che per lo specifico prodotto sia stata attivata o meno
  la funzionalità di "Visualizza in negozio"

- **Natura (solo Ecommerce Mexal):** consente di definire il criterio di
  visualizzazione degli articoli sulla base della loro "Natura" Mexal.
  Per maggiori informazioni relativamente alla gestione lato Passweb
  delle Nature Mexal si veda anche la sezione *"Catalogo -- Gestione
  Articolo -- Nature"* di questo manuale.

- **Codice Alternativo (solo Ecommerce Mexal):** consente di definire il
  criterio di visualizzazione degli articoli sulla base del loro codice
  alternativo Mexal

- **Categoria Sconto / Sconto Quantità / Provvigione / Formazione
  Prezzo:** consente di impostare il filtro articoli sulla base della
  Categoria Sconto / Sconto Quantità / Provvigione / Formazione Prezzo
  di appartenenza dello specifico prodotto

- **Serie Taglie / Colori:** consente di impostare il filtro articoli
  sulla base della specifica Serie di Taglie / Colori cui appartiene il
  prodotto

- **Struttura:** consente di impostare il filtro articoli sulla base
  della struttura di appartenenza dello specifico prodotto (valido per
  articoli padri di struttura)

- **Struttura Origine:** consente di impostare il filtro articoli sulla
  base della struttura di appartenenza dello specifico prodotto (valido
  per articoli figli di struttura)

- **Tipologia** consente di impostare il filtro sulla base della
  tipologia dei vari articoli.

> Ovviamente le tipologie gestite sono le stesse definite all'interno
> del gestionale ossia: Articoli Semplici (tipo A), Articoli Spesa (tipo
> S), Articoli Modificatori (tipo M), Articoli Campionario (tipo C) ...

- **Alias ASIN / GTIN / EPID:** consente di impostare il filtro articoli
  sulla base del fatto che per esso sia stato valorizzato o meno il
  campo Alias ASIN / GTIN / EPID

- **Nelle liste di Amazon / eBay:** consente di impostare il filtro
  articoli sulla base dell'appartenenza dello specifico prodotto alle
  liste Amazon / eBay

- **Stato su Amazon / eBay:** consente di impostare il filtro articoli
  sulla base dello stato assunto dallo specifico prodotto su Amazon /
  eBay

Oltre ai campi sopra indicati, sarà possibile utilizzare come campo di
filtro anche un qualsiasi attributo articolo appositamente mappato
all'interno di Passweb (nella selezione dei campi di filtro gli
attributi articolo sono evidenziati rispetto ai campi nativi mediante un
colore di sfondo grigio)

Per maggiori informazioni relativamente alla gestione degli attributi
articolo all'interno di Passweb, si veda la corrispondente sezione
*"Catalogo -- Attributi Articolo - Attributi"* di questo manuale.

Una volta selezionato il campo su cui impostare il filtro, sarà
necessario selezionare l'operatore da utilizzare all'interno del filtro
stesso ed il valore che il campo dovrà assumere affinché la regola di
visualizzazione degli articoli possa essere soddisfatta.

![](./assets/media/image139.png)

In questo senso, ovviamente, gli operatori disponibili e le modalità di
inserimento del valore da soddisfare potranno cambiare in relazione alla
tipologia di campo su cui è stato impostato il filtro.

Nel caso, ad esempio, in cui il filtro sia stato impostato sul campo
"**Categoria**", dopo aver selezionato l'operatore relazionale
desiderato, sarà necessario cliccare sull'etichetta "**Categorie**" che
comparirà subito dopo questo stesso operatore. In questo modo verrà
aperta una piccola finestra contenente l'elenco delle categorie
merceologiche attualmente gestite all'interno del sito

![](./assets/media/image140.png)

Sarà quindi sufficiente selezionare le categorie merceologiche
desiderate, utilizzando, se necessario, anche il campo di ricerca
presente immediatamente al di sopra dell'albero delle categorie, e
chiudere poi la finestra di selezione cliccando in un qualsiasi punto
della pagina.

**NOTA BENE:** la selezione di una certa categoria, comporterà che il
relativo filtro prenda in considerazione anche tutte le eventuali sotto
categorie.

All'interno del campo Valore è possibile utilizzare anche due
pseudo-metodi che possono ritornare, in maniera dinamica, il valore di
determinati campi legati all'anagrafica dell'utente attualmente connesso
sul sito.

I due pseudo-metodi in questione sono:

- **GETFIELDUSER**: metodo che restituisce il valore di determinati
  campi legati all'anagrafica dell'utente attualmente connesso

- **GETFIELDAGENT**: metodo che restituisce il valore di determinati
  campi legati all'anagrafica dell'agente attualmente connesso

Entrambi questi metodi accettano in ingresso due diversi parametri:

**alias tabella**: codice alias della tabella sul database del sito da
cui verranno prelevati i dati. I valori utilizzabili per questo
parametro sono:

- **ue**: i dati verranno prelevati dalla tabella del database
  contenenti i dati anagrafici dell'utente

- **ad**: i dati verranno prelevati dalla tabella del database
  contenenti gli attributi utente

**parametro secondario**: i valori utilizzabili per questo parametro
variano in relazione a quanto impostato per il parametro "alias
tabella".

Nello specifico

- Se per il parametro "alias tabella" è stato utilizzato il valore
  **ue**, in questo secondo parametro dovrà essere indicato il nome del
  campo da cui prelevare il dato. Sono gestiti i seguenti nomi campo

  - **codiceIntegrazione**: restituisce il codice conto gestionale
    dell'utente attualmente connesso

  - **codiceFiscale**: restituisce il codice fiscale dell'utente
    attualmente connesso

  - **partitaIva**: restituisce la partita IVA dell'utente attualmente
    connesso

- Se per il parametro "alias tabella" è stato utilizzato il valore
  **ad** in questo secondo parametro dovrà essere indicato
  l'identificativo (ID) dell'attributo utente da cui prelevare il dato.

> **ATTENZIONE!** per reperire l'ID dell'attributo utente che si
> desidera utilizzare è sufficiente accedere alla maschera "**Utenti --
> Configurazione Utenti Sito -- Gestione Attributi**" del Wizard,
> individuare l'attributo desiderato e prelevare il suo identificativo
> dalla colonna ID

![](./assets/media/image141.png)

**ATTENZIONE! i filtri articolo basati sugli pseudo-metodi indicati
potrebbero risultare particolarmente onerosi per cui andrebbero
utilizzati solo nel momento in cui non sia effettivamente possibile
raggiungere il risultato desiderato con i filtri standard**

In questo senso un possibile caso d'uso potrebbe essere quello di
rendere visibili, e quindi acquistabili, determinati articoli solo a
singoli utenti (per maggiori informazioni in merito si veda l'Esempio 3
indicato nei successivi capitoli di questo manuale)

**ATTENZIONE! Volendo è possibile concatenare tra loro due o più
condizioni di filtro, basate anche su più campi differenti, in maniera
tale da realizzare delle query più o meno complesse a seconda del tipo
di risultato che si desidera ottenere.**

Al termine di ogni condizione verrà infatti visualizzata una **"e"**,
corrispondente all'operatore logico "**AND"**, e utilizzata, a default,
per concatenare tra loro eventuali ulteriori condizioni che dovranno
essere considerate nella costruzione della query di selezione degli
articoli.

Cliccando su questo elemento verrà aperta una piccola finestra
all'interno della quale poter selezionare eventuali ulteriori operatori
logici da utilizzare nella costruzione della propria query.

![](./assets/media/image142.png)

In questo senso, come precedentemente evidenziato, la **"e"**
corrisponderà all'operatore logico **AND** mentre la **"o"**
all'operatore logico **OR.** Le eventuali parentesi, poste prima o dopo
questi operatori, potranno essere utilizzate, esattamente come avviene
in algebra, per specificare quali condizioni dovranno essere valutate
prima e quali dopo.

Il pulsante "**Copia Filtro**" presente immediatamente al di sotto del
campo in esame consente di copiare rapidamente la stringa corrispondente
al filtro impostato, stringa questa che potrà poi essere inserita in un
eventuale file di importazione nel momento in cui si dovesse gestire
un'importazione massiva dei parametri di configurazione dei gruppi
utente (per maggiori informazioni in merito si veda quanto indicato nei
precedenti capitoli di questo manuale)

**ATENZIONE!!: Nel caso in cui un utente appartenga contemporaneamente a
più gruppi, questo stesso utente potrà visualizzare e conseguentemente
acquistare all'interno del sito, solo ed esclusivamente gli articoli che
ricadono nell'intersezione dei filtri associati ai suoi gruppi di
appartenenza, cioè quegli articoli che soddisfano, contemporaneamente,
tutte le condizioni impostate nei vari filtri.**

Tale regola, valida in generale, ha delle casistiche particolari che
vanno analizzate nel momento in cui ad effettuare ordini sul sito siano
degli Agenti (siti B2B).

In particolare in queste condizioni il comportamento dell'applicazione
dipenderà da come è stato impostato il parametro "**Gestione Filtri
Articoli Agente"** presente nella sezione "*Catalogo -- Configurazione
Parametri -- Catalogo Mexal*" del Wizard

![](./assets/media/image143.png)

Per chiarire meglio questo aspetto consideriamo i due casi seguenti:

**CASO 1**

Supponiamo che:

- l'Agente X possa gestire, all'interno del sito, solo gli articoli che
  fanno parte della categoria "Casalinghi".

- l'agente abbia tra i suoi clienti il signor Y, che appartiene al
  gruppo P per il quale è stato indicato un filtro che restituisce come
  risultato tutti gli articoli che hanno il codice che inizia con "P".

- il parametro Gestione Filtri Articoli Agente sia stato impostato sul
  valore "**Considera i filtri articoli Agente e Cliente**"

In queste condizioni una volta che l'Agente X ha effettuato il login,
alla pagina catalogo verranno visualizzati gli articoli che in Mexal
sono stati assegnati alla categoria "Casalinghi" o ad una delle sue
sottocategorie.

Nel momento in cui l'Agente X, andrà ad effettuare un ordine per il
signor Y, nel negozio verranno mostrati solo gli articoli appartenenti
alla categoria "Casalinghi," o alle sue sottocategorie, e il cui codice
articolo inizia con "P".

**CASO 2**

Supponiamo che:

- l'Agente X possa gestire, all'interno del sito, solo gli articoli che
  fanno parte della categoria "Casalinghi".

- l'agente abbia tra i suoi clienti il signor Y, che appartiene al
  gruppo P per il quale è stato indicato un filtro che restituisce come
  risultato tutti gli articoli che hanno il codice che inizia con "P".

- il parametro Gestione Filtri Articoli Agente sia stato impostato sul
  valore "**Considera solo i filtri articoli Agente**"

In queste condizioni una volta che l'Agente X ha effettuato il login,
alla pagina catalogo verranno gli articoli che in Mexal sono stati
assegnati alla categoria "Casalinghi" o ad una delle sue sottocategorie.

Nel momento in cui l'Agente X, andrà ad effettuare un ordine per il
signor Y, nel negozio verranno comunque visualizzati tutti gli articoli
che in Mexal sono stati assegnati alla categoria "Casalinghi" o ad una
delle sue sottocategorie indipendentemente dal fatto che il loro codice
articolo inizi o meno con "P" (non viene quindi considerato il filtro
impostato sul gruppo di appartenenza del cliente)

**NOTA BENE:** i filtri articolo impostati su di un gruppo utenti
vengono poi gestiti nei componenti Catalogo, Offerte/Novità, Abbinati e
Prodotto. Non vengono invece gestiti nel componente Campionario (se
l'utente può acquistare l'articolo campionario deve vedere tutti gli
elementi che compongono il campionario, indipendentemente dai filtri
articolo) e nel componente Configuratore (se l'utente può acquistare
l'articolo strutturato, deve poter visualizzare tutte le combinazioni
degli elementi della struttura, indipendentemente dai filtri articolo).

Ovviamente nel momento in cui un qualsiasi utente effettui
l'autenticazione al sito entrerà automaticamente a far parte del gruppo
Standard "**Utente** **Autenticato**" e, conseguentemente, sarà in grado
di visualizzare i soli articoli che soddisferanno eventuali filtri
impostati su tale gruppo.

Allo stesso modo, prima di effettuare il login, ogni utente apparterrà,
a default, al gruppo Standard "**Utente** **non** **Autenticato**" e
sarà quindi in grado di visualizzare i soli articoli che soddisferanno
eventuali filtri impostati su tale gruppo.

**ATTENZIONE: In Passweb i filtri articolo possono essere applicati,
oltre che ai gruppi utente, anche a:**

- **specifici componenti ecommerce quali: Offerte/Novità, Popolarità
  Prodotto, Risultati Ricerca**

- **specifiche funzionalità dell'applicativo quali: regole per la
  valorizzazione di attributi articolo, feed articolo, configurazione
  costi per spese accessorie, buoni sconto**

**La modalità di realizzazione e gestione dei filtri articolo applicati
ai suddetti componenti e/o alle suddette funzionalità è esattamente la
stessa di quella appena considerata per i gruppi utente.**

Per maggiori informazioni in merito agli specifici componenti ecommerce
o alle specifiche funzionalità dell'applicativo si rimanda ai relativi
capitoli di questo manuale.

Di seguito verranno mostrati due semplici esempi di filtri articolo
applicabili ad un qualsiasi gruppo utente

###### ESEMPIO 1: VISUALIZZAZIONE DEI SOLI ARTICOLI IN OFFERTA

Per fare in modo che gli utenti appartenenti ad un certo gruppo possano
visualizzare all'interno del sito i soli articoli marcati come articoli
in offerta (campo Passweb "Gest. Art. in Offerta" = S / campo Offerta,
dell'Anagrafica Passweb dell'articolo, selezionato) sarà necessario
impostare su questo stesso gruppo un semplice filtro articoli,
costituito da un'unica condizione, come quello mostrato in figura

![Videate\\filtro_articoli_3.bmp](./assets/media/image144.png)

**Per ottenere questo risultato sarà quindi sufficiente utilizzare come
campo cui applicare il filtro articoli il campo "Offerte", come
operatore relazionale l'operatore "uguale" e come valore il valore
"Vero"**

###### ESEMPIO 2: VISUALIZZAZIONE DEGLI ARTICOLI IN OFFERTA O NOVITA' APPARTENENTI AD UNA SEPCIFICA CATEGORIA MERCEOLOGICA

Supponendo di voler gestire un gruppo di utenti in grado di visualizzare
all'interno del sito solo ed esclusivamente gli articoli appartenenti ad
una specifica categoria merceologica (es. Informatica) e marcati come
articoli Novità (campo Passweb "Gest. Art. in Novità" = S / campo
Novità, dell'Anagrafica Passweb dell'articolo, selezionato) oppure come
articoli in Offerta (campo Passweb "Gest. Art. in Offerta" = S / campo
Offerta, dell'Anagrafica Passweb dell'articolo, selezionato), sarà
necessario impostare, su questo stesso gruppo, un filtro articoli
costituito da tre distinte condizioni opportunamente concatenate tra
loro come mostrato in figura

![Videate\\filtro_articoli_7.bmp](./assets/media/image145.png)

Considerando che l'id 109 corrisponde, nell'esempio in questione, alla
categoria merceologica "Informatica", il filtro sopra evidenziato
consentirà agli utenti dei gruppo di visualizzare all'interno del sito
solo ed esclusivamente gli articoli risultanti dalla query

**Categoria Merceologica = Informatica AND (Novità = Vero OR Offerte =
Vero)**

L'ordine di priorità impostato tramite l'utilizzo delle parentesi farà
sì che venga valutata, prima di tutto, la condizione **( Novità = Vero
OR Offerte = Vero )** in modo tale da considerare tutti gli articoli
marcati, all'interno del gestionale, come articoli Novità oppure come
articoli in Offerta. Tali articoli verranno poi messi in **AND** con la
condizione **Categoria Merceologica = 2** e quindi, di questi, verranno
visualizzati all'interno del sito solo ed esclusivamente quelli
appartenenti alla categoria merceologica "Informatica" (corrispondente
appunto all'id 2)

###### ESEMPIO 3: VISUALIZZAZIONE DI DETERMINATI ARTICOLI A SINGOLI UTENTI 

Supponiamo di dover gestire un caso piuttosto particolare in cui tre
diversi utenti del sito devono poter visualizzare e acquistare, una
volta effettuata l'autenticazione, un singolo prodotto soltanto,
ovviamente diverso per ognuno di essi.

Nello specifico:

- l'utente con codice conto 502.00006 deve poter vedere ed acquistare
  solamente l'articolo con codice ACBA02

- l'utente con codice conto 502. 00026 deve poter vedere ed acquistare
  solamente l'articolo con codice ACBA04

- l'utente con codice conto 502. 00033 poter vedere ed acquistare
  solamente l'articolo con codice ACBA06

I prerequisiti indispensabili per poter arrivare ad ottenere questo tipo
di risultato sono due:

- Porre il sito dietro autenticazione, in modo tale che soltanto gli
  utenti autenticati possano effettivamente visualizzare ed acquistare i
  prodotti in catalogo

- Creare un Attributo Articolo di tipo Mexal chiamato, ad esempio,
  "**Codice Conto Cliente**" mappato sul campo di una videata aggiuntiva
  articolo che dovremo poi valorizzare, per i tre articoli interessati,
  con il codice conto dell'utente che potrà vedere quello stesso
  prodotto una volta effettuato l'accesso al sito.

![](./assets/media/image146.png)

![](./assets/media/image147.png)

Una volta soddisfatte queste due condizioni potremo poi procedere in due
modi diversi.

Potremmo ad esempio pensare di creare, sul sito, 3 distinti gruppi
utente con le seguenti caratteristiche:

- Gruppo 1 con filtro utenti impostato come "Codice uguale 502.00006" e
  filtro articoli impostato come "Codice Cliente = 502.00006"

- Gruppo 2 con filtro utenti impostato come "Codice uguale 502.00026" e
  filtro articoli impostato come "Codice Cliente = ACBA04",

- Gruppo 3 con filtro utenti impostato come "Codice uguale 502.00033" e
  filtro articoli impostato come "Codice Cliente = ACBA06"

In questo modo il filtro utenti impostato sui gruppi inserirà
automaticamente i singoli utenti all'interno di ciascuno di essi e il
filtro articoli, impostato sull'Attributo Articolo **Codice Cliente**
precedentemente creato, farà sì che ogni utente possa effettivamente
vedere ed acquistare, una volta effettuata l'autenticazione, soltanto il
singolo prodotto a lui dedicato.

Ovviamente nel momento in cui il numero di clienti singoli a cui rendere
visibili determinati articoli dovesse aumentare, questa soluzione
richiederebbe la creazione di un numero piuttosto elevato di Gruppi
Utente cosa questa che la renderebbe difficilmente applicabile sia a
livello di gestione che a livello di prestazioni.

Lo stesso risultato si potrebbe però ottenere in modo diverso,
utilizzando un solo Gruppo Utente e gli pseudo-metodi indicati nei
precedenti capitoli di questo manuale.

Il Gruppo in esame che potremmo chiamare, ad esempio, "**Gruppo Utenti
Singoli**" dovrebbe avere un Filtro Articoli configurato come di seguito
indicato:

- **Codice Conto Cliente uguale GETFIELDUSER (ue, codiceIntegrazione)**

![](./assets/media/image148.png)

e all'interno di questo gruppo dovrebbero essere inseriti i 3 utenti con
codice conto 502.00006, 502.00026 e 502.00033

In queste condizioni lo pseudo-metodo **GETFIELDUSER(ue,
codiceIntegrazione),** impostato come valore del campo di filtro,
ritornerà esattamente il codice conto dell'utente attualmente connesso
sul sito, per cui se l'utente loggato dovesse essere, ad esempio, il
502.00006 la condizione del filtro verrebbe validata soltanto per
l'articolo ACBA02 ma non per l'articolo ACBA04 che, secondo la stessa
logica potrà invece essere visualizzato ed acquistato solo dall'utente
con codice conto 502.00026.

##### FILTRI UTENTE

Un **Filtro Utente** altro non è se non un insieme di regole che
definiscono i criteri di appartenenza degli utenti ad uno specifico
gruppo.

**Associando quindi ad un gruppo un Filtro Utente, potranno poi far
parte di questo stesso gruppo solo ed esclusivamente gli utenti che
soddisfano il filtro impostato.**

I filtri utente possono rivelarsi dunque particolarmente utili per
realizzare in maniera completamente automatica l'associazione fra i vari
utenti del sito e relativi gruppi.

Per i gruppi cui è stato associato un filtro utente infatti,
l'associazione "Gruppo -- Utente" verrà gestita in maniera completamente
automatica da Passweb in diversi momenti:

- **In fase di salvataggio del gruppo**: salvando un gruppo con dei
  filtri utente associati, Passweb cercherà, fra tutti gli utenti del
  sito, quelli che soddisfano il filtro impostato e li inserirà
  automaticamente all'interno del gruppo in esame.

- **In fase di registrazione utente**: alla conferma della registrazione
  da parte di un nuovo utente Passweb si preoccuperà di controllarne i
  dati anagrafici per verificare se questi possano soddisfare o meno uno
  dei filtri utente associato ai vari gruppi e, eventualmente, si
  preoccuperà di inserire il nuovo utente all'interno del corrispondente
  gruppo.

- **In fase di aggiornamento del profilo**: nel caso in cui un utente
  del sito decida di variare i propri dati anagrafici, rispetto a quanto
  inserito in fase di registrazione, alla conferma delle nuove
  impostazioni Passweb si preoccuperà di controllare i nuovi dati
  anagrafici per verificare se questi possano soddisfare o meno uno dei
  filtri utente associato ai vari gruppi e, eventualmente, si
  preoccuperà poi di inserire il nuovo utente all'interno del
  corrispondente gruppo.

- **In fase di sincronizzazione**: in fase di sincronizzazione Passweb
  si preoccuperà di verificare la presenza di nuovi utenti eventualmente
  esportati dal gestionale, ne controllerà i dati anagrafici per
  verificare se questi possano soddisfare o meno uno dei filtri utente
  associato ai vari gruppi e, eventualmente, si preoccuperà di inserire
  i nuovi utenti all'interno dei corrispondenti gruppi.

> **ATTENZIONE!** dopo aver associato un filtro utente ad un gruppo,
> l'associazione "Utente -- Gruppo" verrà gestita solo ed esclusivamente
> da Passweb. **Non è quindi possibile in alcun modo inserire
> manualmente degli utenti in gruppi con associato uno specifico
> filtro**
>
> Per la stessa ragione associando un filtro utenti ad un certo gruppo,
> tutti gli utenti presenti in quello stesso gruppo e che non soddisfano
> il nuovo filtro verranno automaticamente eliminati dal gruppo.

**ATTENZIONE!** Se da una parte dunque l'utilizzo dei filtri utente
potrebbe rivelarsi effettivamente molto utile per automatizzare la
procedura di associazione "Utente -- Gruppo", dall'altra parte occorre
anche considerare che **una volta definiti per un certo gruppo dei
filtri utente poi non sarà più possibile associare a questo gruppo dei
nuovi utenti in maniera manuale.**

Per creare un nuovo filtro utente sarà necessario portarsi nella
maschera di configurazione delle proprietà del gruppo desiderato ed
agire poi dalla corrispondente sezione "**Filtro Utenti**".

![](./assets/media/image149.png)

Cliccando sul pulsante **"Aggiungi un nuovo filtro"** verranno
visualizzati, all'interno di un apposito menu a tendina, i vari campi su
cui poter impostare la regola che definirà il criterio di appartenenza
al gruppo.

![](./assets/media/image150.png)

Il campo di input presente nella parte alta del piccolo pop up consente,
digitando almeno 3 caratteri, di filtrare gli elementi presenti in
elenco.

Nello specifico poi il campo:

- **Privato:** consente di definire regole di appartenenza al gruppo
  basate sul concetto di Privato/Azienda

- **Nazione:** consente di definire regole di appartenenza al gruppo
  basate sulla provenienza dei vari utenti.

- **Codice:** consente di definire regole di appartenenza al gruppo
  basate direttamente sui codici gestionali delle relative anagrafiche
  utenti.

- **Categoria Statistica** / **Zona:** consentono di definire regole di
  appartenenza al gruppo basate sul valore dei relativi campi
  gestionali.

- **Ente Pubblico:** consente di definire regole di appartenenza al
  gruppo basate sul fatto che l'utente abbia dichiarato di essere o meno
  un' Ente Pubblico

- **Fattura elettronica:** consente di definire regole di appartenenza
  al gruppo basate sul fatto che l'utente abbia dichiarato o meno di
  voler ricevere fattura elettronica

- **Partita Iva:** consente di definire regole di appartenenza al gruppo
  che possono essere basate sulla specifica partita iva degli utenti
  piuttosto che sul fatto che un utente abbia o meno inserito nella sua
  anagrafica una partita iva

- **Codice Fiscale:** consente di definire regole di appartenenza al
  gruppo che possono essere basate sullo specifico codice fiscale degli
  utenti piuttosto che sul fatto che un utente abbia o meno inserito
  nella sua anagrafica un codice fiscale

- **Tipologia Utente** / **Tipologia Cliente** consentono di definire
  regole di appartenenza al gruppo basate sul fatto che gli utenti in
  questione siano dei clienti abilitati o meno ad accedere in area
  riservata, degli agenti oppure dei semplici contatti (ossia utenti
  registrati ma che non hanno ancora effettuato il loro primo ordine)

- **Utente Ospite**: consente di definire regole di appartenenza al
  gruppo basate sul fatto che l'utente in esame sia o meno un utente di
  tipo "**Ospite**" e quindi sul fatto che abbia deciso di creare o meno
  un proprio account per accedere al sito

- **Agente** **-- solo Ecommerce Mexal**: consente di definire regole di
  appartenenza al gruppo basate sull'associazione agente -- cliente
  definita direttamente all'interno del gestionale. Grazie a questo
  campo sarà quindi possibile, ad esempio, creare in maniera
  completamente automatica un Gruppo costituito da tutti i clienti
  associati, all'interno del gestionale, ad un determinato Agente.

Oltre ai campi sopra indicati, sarà poi possibile utilizzare come campo
di filtro anche un qualsiasi attributo utente appositamente mappato
all'interno di Passweb (nella selezione dei campi di filtro gli
attributi articolo sono evidenziati rispetto ai campi nativi mediante un
colore di sfondo grigio)

Per maggiori informazioni relativamente alla gestione degli attributi
utente all'interno di Passweb, si veda la corrispondente sezione
*"Utenti -- Configurazione Utenti -- Gestione Attributi"* di questo
manuale.

**NOTA BENE:** per i gruppi di tipo "**Utente Non Autenticato**" è
possibile utilizzare come campo di filtro solo ed esclusivamente il
campo "Nazione"

Una volta selezionato il campo su cui impostare il filtro, sarà
necessario selezionare l'operatore da utilizzare all'interno del filtro
stesso ed il valore che il campo dovrà assumere affinché la regola in
esame possa essere soddisfatta.

![](./assets/media/image151.png)

![](./assets/media/image152.png)

In questo senso, ovviamente, gli operatori disponibili e le modalità di
inserimento del valore da soddisfare potranno cambiare in relazione alla
tipologia di campo su cui è stato impostato il filtro.

Nel caso in cui, ad esempio, il filtro sia stato impostato sul campo
"**Nazione**", dopo aver selezionato l'operatore relazionale desiderato,
sarà necessario cliccare sull'etichetta "**Nazioni**" che comparirà
subito dopo questo stesso operatore.

In questo modo verrà aperta una piccola finestra contenente l'elenco
delle nazioni gestite all'interno del sito (quello selezionate alla
pagina "Gestione Paesi" del Wizard).

![](./assets/media/image153.png)

Sarà quindi sufficiente, a questo punto, selezionare i paesi desiderati
tra quelli presenti in elenco, e chiudere la finestra di selezione del
Paese cliccando in un qualsiasi punto dell'area della maschera colorata
in grigio scuro.

**E' inoltre possibile concatenare tra loro due o più regole in maniera
tale da realizzare dei filtri utente più o meno complessi a seconda del
tipo di risultato che si desidera ottenere.**

Al termine di ogni regola verrà infatti visualizzata una **"e"**,
corrispondente all'operatore logico "**AND"**, e utilizzata, a default,
per concatenare tra loro eventuali ulteriori regole che dovranno essere
considerate nella costruzione del filtro in questione.

Cliccando su questo elemento verrà aperta una piccola finestra
all'interno della quale poter selezionare eventuali ulteriori operatori
logici da utilizzare nella costruzione del proprio filtro.

![](./assets/media/image154.png)

In questo senso, come precedentemente evidenziato, la **"e"**
corrisponderà all'operatore logico **AND** mentre la **"o"**
all'operatore logico **OR.** Le eventuali parentesi, poste prima o dopo
questi operatori, potranno essere utilizzate, esattamente come avviene
in algebra, per specificare quali condizioni dovranno essere valutate
prima e quali dopo.

Il pulsante "**Copia Filtro**" presente immediatamente al di sotto del
campo in esame consente di copiare rapidamente la stringa corrispondente
al filtro impostato, stringa questa che potrà poi essere inserita in un
eventuale file di importazione nel momento in cui si dovesse gestire
un'importazione massiva dei parametri di configurazione dei gruppi
utente (per maggiori informazioni in merito si veda quanto indicato nei
precedenti capitoli di questo manuale)

Di seguito verranno mostrati due semplici esempi di filtri utente
realizzati per creare, ad esempio, un gruppo di soli utenti privati ed
un gruppo di soli utenti italiani di professione Avvocato o
Commercialista.

**[ESEMPIO 1: GRUPPO DI UTENTI DI TIPO "PRIVATO"]{.underline}**

Per creare un Gruppo Utenti contenente solo ed esclusivamente utenti di
tipo "Privato" sarà necessario creare un semplice filtro utenti
costituito da una sola regola come quello mostrato in figura

![](./assets/media/image155.png)

**Per ottenere questo risultato sarà quindi sufficiente utilizzare come
campo cui applicare il filtro utenti il campo "Privato", come operatore
relazionale l'operatore "uguale" e come valore il valore "Vero"**

**[ESEMPIO 2: GRUPPO CON UTENTI DI NAZIONALITA' ITALIANA E DI
PROFESSIONE AVVOCATO O COMMERCIALISTA]{.underline}**

Supponendo di voler realizzare un gruppo utenti contenente solo ed
esclusivamente utenti italiani di professione Avvocato o Commercialista,
e supponendo in tal senso di aver precedentemente mappato un apposito
attributo cliente per gestire la "Professione" degli utenti, sarà ora
necessario creare un filtro utenti costituito da tre distinte regole
opportunamente concatenate tra loro come mostrato in figura

![](./assets/media/image156.png)

Considerando che l'id 108 corrisponde, nell'esempio in questione, alla
nazione "Italia" , il filtro utenti sopra evidenziato consentirà di
inserire all'interno dello specifico gruppo solo ed esclusivamente
utenti che soddisfano il seguente requisito

**Nazione = Italia AND (Professione = Avvocato OR Professione =
Commercialista)**

L'ordine di priorità impostato tramite l'utilizzo delle parentesi farà
si che venga valutata, prima di tutto, la condizione **(Professione =
Avvocato OR Professione = Commercialista)** in modo tale da considerare
tutti gli utenti con il campo Professione impostato sul valore
"Avvocato" o sul valore "Commercialista". Tali utenti verranno poi messi
in **AND** con la condizione **Nazione = 108** e quindi, di questi,
verranno inseriti all'interno del gruppo solo ed esclusivamente quelli
appartenenti alla nazione "Italia" (corrispondente appunto all'id 108)

**[ESEMPIO 3: GRUPPO CON UTENTI PRIVI DI PARTITA IVA / CODICE
FISCALE]{.underline}**

Supponendo di voler realizzare un gruppo contenente solo ed
esclusivamente utenti che non hanno valorizzato, nella loro anagrafica,
il campo Partita IVA / Codice Fiscale, sarà ora necessario creare un
filtro utenti costituito dalla regola evidenziata in figura

![](./assets/media/image157.png)

**ATTENZIONE! i campi Partita Iva e Codice Fiscale consentono di
realizzare filtri di tipo testuale**

In altri termini dunque, per ottenere quanto richiesto, il campo da
selezionare dovrà essere "**Partita IVA** / **Codice Fiscale**",
l'operatore dovrà essere "**uguale**" e il campo "**Valore**" dovrà
essere impostato su "**stringa vuota**"

**ATTENZIONE!** Per impostare il campo Valore su "stringa vuota" è
necessario entrare nel campo e cancellare il segnaposto "Valore"

In maniera del tutto analoga, nel momento in cui l'esigenza dovesse
essere quella di creare gruppi di utenti che hanno impostato all'interno
della loro anagrafica un valore per il campo Partita Iva / Codice
Fiscale, il filtro da impostare sarà esattamente analogo a quello appena
esaminato con la differenza che l'operatore da utilizzare dovrà essere,
in questo caso, "diverso da"

##### FILTRI CLIENTI AGENTE

Un **Filtro Clienti Agente** altro non è se non un insieme di regole
mediante le quali poter applicare eventuali filtri articolo definiti
sullo stesso gruppo non a tutti gli utenti del gruppo ma solo ed
esclusivamente ai clienti associati agli agenti che fanno parte di tale
gruppo e che soddisfano le condizioni definite mediante questo "Filtro
Clienti Agente"

La tipologia di filtro da realizzare è del tutto analoga a quella
precedentemente analizzata per i filtri utente. Anche in questo caso
quindi per creare un nuovo "filtro clienti agente" sarà necessario
portarsi nella maschera di configurazione delle proprietà del gruppo
desiderato ed agire poi dalla corrispondente sezione "**Filtro Clienti
Agente**".

![](./assets/media/image158.png)

Cliccando sul pulsante **"Aggiungi un nuovo filtro"** verranno
visualizzati i vari campi su cui poter impostare la regola che definirà
l'insieme dei clienti, tra quelli associati agli agenti facenti parte
del gruppo, ai quali dovranno essere applicati eventuali filtri articolo
definiti sullo stesso gruppo.

![](./assets/media/image159.png)

I campi "**Privato**" e "**Nazione**" consentiranno di definire il
criterio di selezione dei clienti sulla base della loro provenienza
piuttosto che sul concetto di Privato/Azienda.

Oltre ai campi sopra indicati, sarà poi possibile utilizzare come campo
di filtro anche un qualsiasi attributo utente appositamente mappato
all'interno di Passweb (nella selezione dei campi di filtro gli
attributi articolo sono evidenziati rispetto ai campi nativi mediante un
colore di sfondo grigio)

Per maggiori informazioni relativamente alla gestione degli attributi
utente all'interno di Passweb, si veda la corrispondente sezione
*"Utenti -- Configurazione Utenti Sito -- Gestione Attributi"* di questo
manuale.

**NOTA BENE:** per i gruppi di tipo "**Utente Non Autenticato**" è
possibile utilizzare come campo di filtro solo ed esclusivamente il
campo "Nazione"

Una volta selezionato il campo su cui impostare il filtro, sarà
necessario selezionare l'operatore da utilizzare all'interno del filtro
stesso ed il valore che il campo dovrà assumere affinché la regola in
esame possa essere soddisfatta.

![](./assets/media/image160.png)

![](./assets/media/image161.png)

È inoltre possibile concatenare tra loro due o più regole in maniera
tale da realizzare dei filtri utente più o meno complessi a seconda del
tipo di risultato che si desidera ottenere.

Al termine di ogni regola verrà infatti visualizzata una **"e"**,
corrispondente all'operatore logico "**AND"**, e utilizzata, a default,
per concatenare tra loro eventuali ulteriori regole che dovranno essere
considerate nella costruzione del filtro in questione.

Cliccando su questo elemento verrà aperta una piccola finestra
all'interno della quale poter selezionare eventuali ulteriori operatori
logici da utilizzare nella costruzione del proprio filtro.

![](./assets/media/image162.png)

In questo senso, come precedentemente evidenziato, la **"e"**
corrisponderà all'operatore logico **AND** mentre la **"o"**
all'operatore logico **OR.** Le eventuali parentesi, poste prima o dopo
questi operatori, potranno essere utilizzate, esattamente come avviene
in algebra, per specificare quali condizioni dovranno essere valutate
prima e quali dopo.

Il pulsante "**Copia Filtro**" presente immediatamente al di sotto del
campo in esame consente di copiare rapidamente la stringa corrispondente
al filtro impostato, stringa questa che potrà poi essere inserita in un
eventuale file di importazione nel momento in cui si dovesse gestire
un'importazione massiva dei parametri di configurazione dei gruppi
utente (per maggiori informazioni in merito si veda quanto indicato nei
precedenti capitoli di questo manuale)

Di seguito verrà illustrato un possibile caso d'uso relativo alla
creazione e all'applicazione di un "Filtro Clienti Agente"

**[CASO D'USO]{.underline}**

L' Agente A1 può, in generale, effettuare ordini per i clienti C1, C2,
C3 e C4 e vendere articoli appartenenti alle categorie CAT1, CAT2 e
CAT3.

Inoltre:

- al cliente C1 possono essere venduti solo ed esclusivamente articoli
  appartenenti alla categoria CAT1

- al solo cliente C4 possono essere venduti esclusivamente articoli
  appartenenti alla categoria CAT5

Per gestire questa casistica è necessario creare tre gruppi:

- GRUPPO1: gruppo in cui va inserito l\'agente A1, con filtro articoli
  impostato a "**Categoria IN CAT1,CAT2,CAT3**"

- GRUPPO2: gruppo in cui va inserito l\'agente A1, con filtro articoli
  impostato a "**Categoria = CAT1**" e con filtro clienti agente
  impostato a "**Codice = C1**"

- GRUPPO3: gruppo in cui va inserito l\'agente A1, con filtro articoli
  impostato a "**Categoria = CAT5**" e con filtro clienti agente
  impostato a "**Codice = C4**".

