# CONFIGURAZIONE ACCOUNT



Una volta completati tutti i passaggi descritti nel precedente capitolo
di questo manuale per connettere Passweb a Prestashop occorrerà ora
creare e configurare correttamente un apposito Account di integrazione.

Nello specifico sarà necessario:

- Portarsi, nel Wizard di Passweb, all'interno della sezione "**Catalogo
  -- Altri Marketplace -- Gestione Account**" e cliccare sul pulsante
  "Aggiungi Account" presente nella parte alta della pagina

- All'interno della maschera "Dati Account" assegnare un nome
  all'Account che si sta configurando (campo **Descrizione**) e
  selezionare, all'interno del campo "**Marketplace**" l'opzione
  "**Prestashop**"

![](./assets/media/image594.png)

- Compilare quindi i campi presenti all'interno della sezione
  "**Credenziali**" con i dati di seguito indicati:

  - **Host**: url del sito Prestashop con cui realizzare l'integrazione
    (può essere necessario inserire l'url del sito comprensivo di www)

  - **Protocollo Host:** selezionare il protocollo (http o https)
    attualmente in uso sul proprio sito Prestashop

  - **Token:** token di accesso alle API Prestashop.

> Per ottenere questa informazione è sufficiente accedere al Back end
> del proprio sito Prestashop, portarsi all'interno della sezione
> "**Parametri Avanzati - Webservice**" e individuare tra quelle
> presenti in elenco la chiave di integrazione relativa a Passweb (per
> maggiori informazioni in merito si faccia riferimento a quanto
> indicato nel precedente capitolo di questo manuale)

![](./assets/media/image595.png)

> chiave questa che dovrà essere copiata ed incollata all'interno del
> campo in questione

- **Store -- visualizzato solo dopo aver effettuato un primo salvataggio
  dell'Account in esame**

> Consente di indicare, selezionandolo dall'apposito menu a tendina, il
> Negozio Prestashop con cui si vuole realizzare l'integrazione.
>
> In questo senso occorre infatti ricordare che Prestashop mette a
> disposizione degli utenti la possibilità di gestire più Negozi (siti
> web) da uno stesso back end di amministrazione.
>
> Fatta questa osservazione la cosa importante da tenere sempre ben
> presente è ora che l**'integrazione Passweb -- Prestashop lavora a
> livello di singolo Negozio**.
>
> In conseguenza di ciò nel momento in cui su Prestashop dovesse essere
> stata attivata la funzionalità del "Multi Negozio" all'interno del
> campo "Store" avremo la possibilità di selezionare uno qualsiasi dei
> Negozi attivi e presenti all'interno della sezione "**Configura --
> Parametri Avanzati -- Multi Negozio**" del back end di Prestashop

![](./assets/media/image596.png)

> **ATTENZIONE**! Ovviamente se l'esigenza dovesse essere quella di
> esportare i prodotti e acquisire ordini da tutti i Negozi gestiti su
> Prestashop sarà necessario creare uno specifico Account di
> Integrazione e delle specifiche Inserzioni per ciascuno di essi
>
> Per maggiori informazioni in merito alla gestione del Multi Negozio su
> Prestashop si rimanda alla specifica documentazione di prodotto

Una volta impostati i principali parametri di configurazione, cliccando
sul pulsante "**Salva**" compariranno nuove sezione (Metodi di
Pubblicazione, Articoli, Ordini, Clienti, Schedulazione, Backup,
Download CSV) all'interno delle quali poter configurare in maniera più
dettagliata altri aspetti dell'integrazione.

Per maggiori informazioni in merito a ciascuna di queste sezioni si
vedano i successivi capitoli di questo manuale.

##### METODI DI PUBBLICAZIONE ARTICOLI

All'interno di questa sezione è possibile decidere quale dovrà essere il
metodo adottato per la pubblicazione dei dati articolo sulla piattaforma
terza.

In questo senso dunque è bene ricordare che, come già indicato nei
precedenti capitoli di questo manuale, Passweb offre due diverse
modalità di esportazione dei dati articolo:

- **via API**: i dati articolo verranno trasferiti ed inseriti sulla
  piattaforma terza in maniera automatica sfruttando, appunto, le API
  messe a disposizione dalla piattaforma stessa

> In questo caso il processo di pubblicazione dipende ovviamente, oltre
> che dalle elaborazioni interne a Passweb, anche dai tempi di risposta
> delle relative API.
>
> Ipotizzando un tempo di pubblicazione del singolo articolo attorno ai
> 5 secondi la pubblicazione di 1000 articoli impiegherebbe un tempo
> pari all\'incirca a 1.5 ore. Nel momento in cui i tempi di
> pubblicazione del singolo articolo dovessero raddoppiare passando a 10
> secondi la pubblicazione di 1000 articoli impiegherebbe all\'incirca
> un tempo pari a 3 ore.
>
> **ATTENZIONE! In considerazione di ciò la pubblicazione di articoli
> via API è consigliata solo per un numero di articoli inferiore a
> 10000**
>
> Allo stesso modo, prima di adottare questo specifico metodo di
> pubblicazione, si consiglia sempre di valutare attentamente quelli che
> sono i tempi effettivi richiesti per il trasferimento delle
> informazioni in relazione al numero complessivo di articoli
> effettivamente gestiti e a quelli che sono i tempi di risposta delle
> API presenti sulla propria installazione Prestashop.

- **via CSV**: i dati articolo verranno pubblicati all'interno di
  appositi file csv. Tali file potranno poi essere:

  - scaricati direttamente dal Wizard di Passweb e uplodati manualmente
    sulla piattaforma terza

  - accessibili ad uno specifico url (sotto il dominio assegnato al
    proprio connettore Passweb)

  - copiati automaticamente all'interno di un'area condivisa (Ftp,
    Google Drive ...) stabilita in fase di configurazione del proprio
    Account di integrazione

> Adottando questo metodo di pubblicazione sarà possibile, ovviamente,
> avere un maggior controllo relativamente a quelle che sono le
> informazioni da inserire sulla piattaforma terza.
>
> Sarà possibile, ad esempio, sviluppare processi personalizzati di
> elaborazione dei dati presenti all'interno dei file csv prodotti da
> Passweb oppure si potrebbe pensare di utilizzare anche uno dei tanti
> moduli di importazione massiva disponibili per la piattaforma terza.
> Infine, non dovendo passare da singole chiamate API ma potendo
> inserire massivamente il contenuto dei file prodotti da Passweb
> direttamente nel database del proprio sito Prestashop anche i tempi di
> upload delle informazioni potrebbero ridursi sensibilmente rispetto ad
> una pubblicazione via API.
>
> Questo tipo di pubblicazione è quindi assolutamente da preferirsi nel
> momento in cui il numero di articoli gestiti dovesse essere
> particolarmente elevato (dell'ordine delle decine di migliaia)
>
> **ATTENZIONE**! **In ogni caso, in questa configurazione un' eventuale
> elaborazione dei file csv prodotti da Passweb così come l'effettivo
> upload dei relativi dati nella piattaforma terza restano operazioni in
> carico a chi gestisce effettivamente lo specifico sito Prestashop**

I parametri presenti all'interno del tab "**Metodi di pubblicazione**"
consentono quindi di settare, in relazione al metodo di pubblicazione
scelto, i diversi parametri di configurazione.

Nello specifico il campo:

**Modalità di pubblicazione articoli:** consente di impostare quello che
dovrà essere il metodo utilizzato per la pubblicazione dei dati articolo
sulla piattaforma terza. E' possibile selezionare uno dei seguenti
valori:

- **API:** selezionando questa opzione la pubblicazione dei dati
  articolo sulla piattaforma terza avverrà sfruttando completamente le
  API messe a disposizione dalla piattaforma stessa. Non sono quindi
  richiesti, per ovvie ragioni, altri specifici parametri di
  configurazione

![](./assets/media/image597.png)

- **CSV**: in questo caso la pubblicazione dei dati articolo avverrà
  mediante la creazione di appositi file csv il cui contenuto dovrà poi
  essere importato sulla piattaforma terza. In queste condizioni sarà
  quindi necessario impostare anche tutta una serie di altri parametri
  necessari per configurare in maniera corretta la creazione dei file
  csv e il repository in cui andarli poi ad inserire.

> Per maggiori informazioni relativamente alla pubblicazione articoli
> via csv si rimanda a quanto indicato nel successivo capitolo di questo
> manuale.

##### PUBBLICAZIONE ARTICOLI VIA CSV

Come precedentemente indicato nel momento in cui si dovesse decidere di
optare per una pubblicazione articoli via csv, sarà necessario impostare
poi anche tutta una serie di parametri che consentiranno di
personalizzare, secondo le specifiche esigenze del caso, il processo di
creazione e gestione di questi stessi file.

![](./assets/media/image598.png)

In particolare dunque il campo

**Separatore File CSV:** consente di impostare, selezionandolo da un
apposito menu a tendina, il carattere da utilizzare, in fase di
creazione del file csv, come separatore dei campi

**Modalità scrittura file:** consente di decidere quale dovrà essere il
metodo utilizzato per gestire i contenuti dei file csv a seguito di
pubblicazioni successive. E' possibile selezionare uno dei seguenti
valori:

- **In aggiunta (append)**: selezionando questa opzione i dati generati
  a seguito di una nuova pubblicazione verranno aggiunti (in append) a
  quelli già presenti all'interno dello stesso tipo di file.

> In queste condizioni, dunque, nel momento in cui un determinato
> articolo dovesse essere oggetto di due pubblicazioni successive (ad
> esempio perché risulta variato il suo prezzo o la sua giacenza) dopo
> l'ultima pubblicazione all'interno del file csv troveremo, per
> l'articolo in esame, due distinte entry una per ogni pubblicazione
> effettuata. All'interno del file csv è comunque presente una colonna
> con l'indicazione della data della pubblicazione che ha prodotto
> quella specifica entry.
>
> Nel momento in cui si dovesse quindi decidere di lavorare in queste
> condizioni occorre sempre tenere in considerazione alcune cose di
> fondamentale importanza. Nello specifico:

- **Passweb produrrà file csv distinti per ogni singola lista di
  vendita** per cui pubblicazioni successive di articoli appartenenti ad
  una stessa lista andranno in append sui relativi file senza modificare
  quelli prodotti a seguito di operazioni di pubblicazione di articoli
  appartenenti a liste diverse.

- **In fase di importazione dati su Prestashop, è di fondamentale
  importanza considerare che all'interno del file possono essere
  presenti più entry per lo stesso prodotto evitando quindi di andare
  poi a creare, a seguito dell'importazione, articoli distinti con lo
  stesso Riferimento**

> In questo senso, utilizzando ad esempio il modulo di importazione
> standard presente in Prestashop sarebbe necessario selezionare in fase
> di importazione l'opzione "**Usare il riferimento prodotto come parola
> chiave**". In questo modo infatti la prima entry presente nel file
> creerà, se non già presente, il nuovo articolo mentre le entry
> successive agganceranno (usando il "Riferimento = Codice Gestionale"
> come chiave) la stessa anagrafica già presente su Prestashop.

- Nel momento in cui due diversi record presenti nel file di
  importazione e relativi allo stesso articolo dovessero avere due
  diversi valori per una stessa Feature (Funzione), in fase di
  importazione il modulo standard di Prestashop non andrà a cancellare
  il primo valore sovrascrivendolo con il secondo ma andrà semplicemente
  ad aggiungere allo stesso prodotto una seconda Feature uguale alla
  precedente ma con un diverso valore.

> **ATTENZIONE! La stessa cosa avverrebbe ovviamente anche se non si
> dovesse lavorare in append e i file di importazione dovessero comunque
> avere per lo stesso articolo e per la stessa Feature dei valori
> diversi**
>
> Nel momento in cui l'esigenza dovesse essere quindi quella di
> sovrascrivere in fase di importazione anche i valori di eventuali
> Feature già presenti per i prodotti su Prestashop è necessario
> valutare attentamente se il modulo di importazione utilizzato offre
> questa possibilità e in alternativa rivolgersi direttamente al gestore
> del sito Prestashop.

- **Tra una pubblicazione e l'altra è necessario verificare attentamente
  di non aver variato eventuali specifiche custom presenti
  nell'Inserzione utilizzata per la pubblicazione** (per maggiori
  informazioni relativamente alla gestione delle Specifiche Custom si
  veda quanto indicato nel precedente capitolo "*Altri Marketplace --
  Gestione Specifiche*" di questo manuale).

> Aggiungendo o eliminando delle specifiche custom tra una pubblicazione
> e l'altra, si andrebbe infatti a variare il formato del tracciato
> record utilizzato nei file csv prodotti da Passweb e questo potrebbe,
> ovviamente, causare delle incoerenze nei dati presenti all'interno del
> file con conseguenti problemi in fase poi di importazione dati sulla
> piattaforma terza.
>
> **ATTENZIONE! Nel momento in cui si dovesse decidere di utilizzare "In
> append" come modalità di scrittura file è di fondamentale importanza
> ricordarsi sempre di svuotare il repository utilizzato per la
> pubblicazione dei file ogni qual volta dovessero essere apportate
> modifiche alle specifiche presenti nelle Inserzioni utilizzate per la
> pubblicazione e, conseguentemente, al tracciato record dei file
> prodotti**

- **Sovrascrivi**: selezionando questa opzione i file generati a seguito
  di una determinata pubblicazione andranno sempre e comunque a
  sovrascrivere quelli attualmente presenti nel repository utilizzato (e
  relativi ovviamente alla stessa lista di vendita). Nel momento in cui
  nel repository non dovesse essere presente quella particolare
  tipologia di file questo verrà ricreato da zero.

> **In ogni caso, in queste condizioni, i file csv all'interno del
> repository conterranno sempre e soltanto i dati relativi all'ultima
> pubblicazione effettuata**

- **Crea sempre nuovo file**: selezionando questa opzione verranno
  prodotti, a seguito di ogni nuova pubblicazione, sempre e comunque
  file distinti senza eliminare o modificare in alcun modo quelli
  attualmente presenti nel repository utilizzato per la pubblicazione

**Nome file CSV:** consente di personalizzare parte del nome dei file
csv prodotti da Passweb aggiungendogli una specifica stringa.

**ATTENZIONE!** Il campo "Nome file CSV" consente di personalizzare solo
parte del nome dei file prodotti da Passweb

In generale occorre infatti considerare che, dipendentemente dalla
tipologia di articoli coinvolti nella pubblicazione, Passweb potrebbe
poi generare, **per ogni singola lista di vendita** e per ogni singola
lingua gestita nello store Prestashop collegato in fase di
configurazione dell'Account, due diversi file:

- Un file relativo agli articoli semplici con nome
  "**ArticoliSemplici_idListaVendita_timestamp_NomeFileCSV_it.csv"**

- Un file per le combinazioni relative ad articoli con varianti
  (strutturati e/o a taglie / colori) con nome
  "**Combinazioni_idListaVendita_timestamp_NomeFileCSV_it**"

dove

- **ArticoliSemplici\_ / Combinazioni\_** è una parte non modificabile
  del nome file indicativa del fatto che al suo interno sono contenuti
  dati relativi ad articoli semplici o alle combinazioni generate a
  seguito di una determinata pubblicazione

- **idListaVendita\_** è una parte non modificabile del nome file che
  indica l'**id** della lista di vendita cui appartengono gli articoli
  presenti nel file csv.

> In questo senso è sempre bene ricordare che verranno prodotti file
> distinti per liste di vendita diverse

- **timestamp\_** è una parte del nome file gestita direttamente da
  Passweb che riporta il timestamp (data e ora) della pubblicazione che
  ha prodotto quel determinato file

- **NomeFileCSV** è la parte variante del nome file determinata sulla
  base della stringa impostata per il campo "Nome File CSV"

- **\_it / \_en ..** è una parte non modificabile del nome file
  indicativa della lingua cui fanno riferimento i dati presenti
  all'interno del file stesso

**ATTENZIONE! Una volta definito quello che dovrà essere il nome dei
file prodotti da Passweb in fase di pubblicazione articoli è di
fondamentale importanza non andare poi a modificarlo**

In questo senso infatti è bene sottolineare che in fase di salvataggio
sul repository esterno dei file prodotti a seguito della pubblicazione
di una determinata lista articoli, Passweb controllerà, per prima cosa,
se nella cartella indicata sono già presenti file dello stesso tipo
inseriti a seguito di pubblicazioni precedenti (**il controllo verrà
effettuato analizzando le parti invarianti del nome file escluso
ovviamente il timestamp**) e:

- in caso positivo eliminerà questi file sostituendoli con quelli
  prodotti dalla pubblicazione in corso. Il nome dei nuovi file resterà
  dunque invariato nei suoi elementi non modificabili ad eccezione del
  timestamp che riporterà sempre data e ora della pubblicazione in
  esame. L'effettivo contenuto di questi file (quindi il fatto che
  all'interno del file stesso siano presenti solo i dati dell'ultima
  pubblicazione o che questi vadano in append ai dati già presenti)
  dipenderà invece da come è stato settato il parametro "**Modalità
  scrittura file**" precedentemente analizzato

- in caso negativo Passweb provvederà semplicemente a ricreare da zero i
  relativi file senza preoccuparsi di cancellare eventuali altri file
  presenti nella stessa cartella di appoggio

In queste condizioni dunque, nel momento in cui si dovesse modificare,
tra una pubblicazione e l'altra, per una qualsiasi ragione, uno degli
elementi invarianti del nome file (es. ArticoliSemplici, Combinazioni,
\_it ...), a seguito di una nuova pubblicazione verranno creati sempre e
comunque dei nuovi file seguendo le specifiche indicate all'interno di
questo capitolo.

Se invece il parametro "**Modalità di scrittura file**" dovesse essere
impostato sull'opzione "**Crea sempre nuovo file**" in fase di
pubblicazione Passweb non effettuerà alcun tipo di controllo sugli
elementi eventualmente presenti nella cartella di appoggio ma si
limiterà a creare sempre e comunque file distinti con all'interno i dati
relativi alla sola pubblicazione in esame.

Una volta compreso come impostare Passweb per creare questi file CSV,
resta ora da capire come gestirne il contenuto e come renderli
effettivamente disponibili alla piattaforma terza.

In questo senso, per quel che riguarda la gestione dei contenuti il
tutto dipende, essenzialmente, da come verrà poi impostata l'Inserzione
utilizzata per la pubblicazione e da quelli che saranno i campi per essa
gestiti.

**E' con l'Inserzione infatti che andremo a definire esattamente quali
informazioni dovranno essere passate alla piattaforma terza (e inserite
quindi nei relativi file csv) per ogni singolo prodotto coinvolto.**

Dal punto di vista strutturale i file csv prodotti da Passweb avranno,
in testata, tutti i campi ritornati dalle chiamate API **getproduct**
(per il file relativo agli articoli semplici) e **getcombination** (per
il file relativo alla combinazioni) più eventuali campi aggiuntivi
determinati da specifiche custom codificate all'interno della
corrispondente sezione del Wizard e correttamente gestite
nell'Inserzione utilizzata per la pubblicazione (per maggiori
informazioni relativamente alla gestione delle specifiche custom si veda
anche quanto indicato nel relativo capitolo "*Altri Marketplace --
Gestione Specifiche*" di questo manuale)

Sostanzialmente dunque all'interno di questi file troveremo come
intestazioni e quindi come campi delle singole entry:

- Gli stessi campi presenti anche nei relativi file di esempio
  ("**Prodotti file di esempio**" e "**Combinazioni file di esempio**")
  scaricabili direttamente dal back end di Prestashop alla pagina
  "**Parametri Avanzati -- Importa**"

![Videate\\prestashop_download_file_esempio.bmp](./assets/media/image599.png)

- Alcuni campi aggiunti e gestiti automaticamente da Passweb tra cui ad
  esempio:

  - **Id_Category_Default**: campo all'interno del quale verrà riportato
    l'identificativo della categoria di default da assegnare in
    Prestashop al corrispondente articolo. Questo campo verrà
    valorizzato nel csv sulla base delle impostazioni settate nella
    relativa Inserzione per la specifica "**Category Default**"

> **ATTENZIONE!** Il campo in esame non è mappabile direttamente
> mediante la funzionalità di importazione standard presente su
> Prestashop, per cui lo stesso identificativo verrà inserito anche come
> primo elemento all'interno del campo "**Categorie**" (campo
> quest'ultimo che conterrà l'elenco degli id di tutte le categorie
> associate all'articolo)

- **Additional_Delivery_Times**: campo da poter settare con il valore
  0/1/2 corrispondente all'opzione che dovrà poi assumere il radio
  button corrispondente al parametro "**Tempi di consegna**" presente
  nel tab "**Spedizione**" dell'anagrafica articolo di Prestashop

- ...

<!-- -->

- Eventuali campi corrispondenti a Specifiche Custom codificate
  all'interno della relativa sezione del Wizard e correttamente gestite
  nell'Inserzione utilizzata per la pubblicazione

> **ATTENZIONE!** eventuali campi corrispondenti a Specifiche Custom
> verranno aggiunti sempre in coda ai campi presenti a default
> all'interno del file csv e saranno facilmente riconoscibili in virtù
> del fatto che il loro nome inizia sempre con "custom\_".

**ATTENZIONE!** **Non tutti i campi presenti a default nei file csv
prodotti da Passweb sono al momento gestibili con delle corrispondenti
Specifiche "Standard"**. Nel momento in cui l'esigenza dovesse essere
quindi quella di valorizzare uno dei campi dei file csv mediante una
determinata Specifica non ancora presente nelle Inserzioni Passweb, sarà
necessario farne apposita richiesta a Passepartout che valuterà poi la
possibilità di inserirla tra le Specifiche "Standard". In alternativa è
sempre possibile creare e gestire apposite Specifiche Custom operando
dalla relativa sezione del Wizard.

Detto delle intestazioni, per quel che riguarda invece le singole entry
dei file csv, i valori presenti per ogni riga (e quindi per ogni
articolo) in corrispondenza della relativa colonna dipenderanno dal
fatto di aver inserito o meno la corrispondente specifica
nell'Inserzione utilizzata per la pubblicazione e, ovviamente, da come
questa stessa specifica è stata mappata e valorizzata.

In virtù di ciò, nel momento in cui nell'Inserzione utilizzata per la
pubblicazione dovessero essere gestite, ad esempio, le specifiche
"**Description**" e "**Description** **Short**" allora le righe del file
csv relative agli articoli pubblicati mediante l'Inserzione in esame
avranno le colonne "**Description**" e "**Description_Short**"
valorizzate con la "Descrizione" e la "Descrizione breve" dei
corrispondenti prodotti, descrizioni queste che verranno prelevate
esattamente dai campi impostati in fase di mapping della relativa
specifica.

Se invece le due specifiche "**Description**" e "**Description Short**"
non dovessero essere gestite nell'Inserzione, il file csv manterrà
comunque come intestazioni le relative colonne ma, in questo caso, per
ogni articolo coinvolto nell'Inserzione, e quindi per ogni singola riga
del file csv, i campi corrispondenti a queste colonne saranno,
ovviamente, non valorizzati.

Infine, occorre anche considerare che:

- determinati campi del file csv, per ovvie ragioni, saranno sempre
  valorizzati indipendentemente da quelle che sono le specifiche
  effettivamente gestite nella corrispondente Inserzione. E' il caso ad
  esempio:

  - del **codice articolo** che verrà sempre inserito in corrispondenza
    della colonna "**Reference**"

  - della **quantità di prodotto disponibile** che verrà sempre inserito
    in corrispondenza della colonna "**Quantity**"

  - del **prezzo articolo** che verrà sempre inserito in corrispondenza
    della colonna "**Price**"

  - ...

- Per i campi che accettano valori multipli e che sono gestiti in
  automatico da Passweb (es. categorie merceologiche) come carattere di
  separazione dei singoli valori verrà utilizzata sempre la ","

> Ovviamente nel momento in cui il campo che accetta valori multipli
> dovesse essere gestito con una specifica mappata, ad esempio, con un
> Attributo Passweb, la valorizzazione del relativo attributo dovrà
> essere gestita manualmente utilizzando anche come separatore dei
> singoli valori un carattere adeguato.
>
> In questo senso il separatore potrebbe anche essere un carattere
> diverso dalla "," ed andrebbe poi dichiarato e gestito in fase di
> importazione direttamente su Prestashop. **Considerando comunque che
> Passweb, come detto, utilizza come carattere di separazione dei valori
> multipli proprio la "," è consigliabile, al fine di evitare problemi o
> confusioni in fase di importazione, utilizzare sempre questo stesso
> carattere come separatore di eventuali valori multipli**.

- Per quel che riguarda infine i campi corrispondenti ad eventuali
  **"Funzionalità" (Features)** presenti su Prestashop, se gestiti
  mediante una Specifica mappata con "Attributo Marketplace" Passweb
  provvederà a valorizzare la relativa colonna del file csv con la
  notazione corretta richiesta da Prestashop
  (**Nome:Valore:Posizione:Personalizzato** ). Nel momento in cui queste
  specifiche dovessero invece essere mappate con "Attributo Passweb" o
  "Personalizzato" occorrerà fare attenzione ad inserire i relativi
  valori con la notazione corretta richiesta da Prestashop in maniera
  tale da non avere poi problemi in fase di importazione.

**ATTENZIONE!** Il link "**Scarica File CSV di esempio**" presente
all'interno del tab "Metodi di pubblicazione" consente di scaricare uno
zip contenente degli esempi di file csv che possono essere prodotti da
Passweb a seguito di una pubblicazione articoli

Ovviamente in questi file di esempio sono presenti solo i campi Standard
e non quelli legati ad eventuali Specifiche Custom.

**Proprio per questo è sempre consigliabile effettuare una prima
pubblicazione di prova per verificare esattamente la struttura dei file
prodotti da Passweb e quelli che sono i dati in essi contenuti.**

Solo dopo aver verificato struttura e contenuto dei file csv sarà
infatti possibile impostare, secondo le specifiche esigenze del caso, la
procedura più corretta di upload dei dati sulla piattaforma terza,
**procedura questa che, come più volte evidenziato, dovrà comunque
essere eseguita esternamente a Passweb e sarà quindi in carico a chi
gestisce lo specifico sito Prestashop**

**ATTENZIONE!** Così come è indispensabile non modificare manualmente il
nome dei file prodotti da Passweb **allo stesso modo e per ovvie ragioni
è di fondamentale importanza non alterare in nessun modo neppure la
struttura di questi stessi file**

E' ovviamente possibile prelevare i file dal Repository in cui Passweb
andrà a salvarli per poi modificarli ed elaborarli secondo le specifiche
esigenze del caso ma fintantoché verranno lasciati all'interno di questo
repository, la loro struttura non dovrà essere modificata in alcun modo.
Andando infatti a eliminare, rinominare o aggiungere manualmente campi
alla struttura di base si correrà il rischio di compromettere le
successive pubblicazioni creando dei tracciati non più gestibili in
maniera corretta.

Per quel che riguarda infine la modalità attraverso cui rendere
disponibili i file prodotti da Passweb questa può essere impostata
sempre dal tab "Metodi di pubblicazione" operando all'interno della
sezione "**Repository**"

![](./assets/media/image600.png)

Nello specifico dunque il campo:

**Repository CSV:** consente di impostare, selezionandola da un apposito
menu a tendina, la particolare tipologia di Repository in cui Passweb
dovrà andare a salvare i file csv prodotti a seguito di ogni
pubblicazione articoli. E' possibile selezionare uno dei seguenti
valori:

- **Non gestito**: selezionando questa opzione non verrà utilizzato
  nessun Repository per cui i file csv prodotti da Passweb a seguito di
  ogni pubblicazione dovranno essere poi scaricati manualmente operando
  all'interno del tab "**Download CSV**" presente nella maschera di
  configurazione dell'Account

- **FTP:** in questo caso, al termine di ogni pubblicazione, i file
  prodotti da Passweb verranno copiati in un' apposita cartella
  all'interno di un' area FTP

- **Google Drive:** in questo caso, al termine di ogni pubblicazione, i
  file prodotti da Passweb verranno copiati in una specifica cartella
  Google Drive

- **URL Passweb:** selezionando questa opzione i file prodotti da
  Passweb al termine di ogni pubblicazione non verranno copiati in
  nessun repository ma saranno accessibili direttamente via web a
  specifici indirizzi sotto il dominio assegnato al proprio connettore
  Passweb

Ovviamente a seconda della particolare tipologia selezionata andranno
poi settati altri parametri di configurazione necessari a Passweb per
potersi effettivamente connettere con quello specifico repository.

Per maggiori informazioni relativamente a come poter configurare il
collegamento con ciascuno dei repository sopra riportati si veda quanto
indicato nei successivi capitoli di questo manuale

###### DOWNLOAD MANUALE

Nel momento in cui l'esigenza dovesse essere quella di gestire i file
csv prodotti da Passweb in maniera completamente manuale, e senza quindi
ricorrere a nessun Repository, sarà sufficiente impostare il parametro
"**Repository CSV**" sull'opzione "**Non Gestito**"

![](./assets/media/image601.png)

In queste condizioni dunque a seguito di ogni operazione di
pubblicazione articoli (indipendentemente dal fatto che sia una
pubblicazione lanciata manualmente o eseguita in automatico a seguito di
una sincronizzazione e/o dell'applicazione di una determinata regola) i
file CSV prodotti da Passweb non verranno copiati in nessun Repository e
dovranno quindi essere scaricati in maniera manuale operando all'interno
del tab "**Download CSV**" presente anch'esso nella maschera di
configurazione del proprio Account Prestashop

![Videate\\google_merchant_csv4.bmp](./assets/media/image446.png)

All'interno di questa sezione, visibile solo nel momento in cui per
l'Account in esame si stia utilizzando un metodo di pubblicazione
articoli via CSV, è infatti presente l'elenco dei vari file prodotti da
Passweb a seguito delle ultime pubblicazioni effettuate.

**ATTENZIONE! Passweb conserva uno storico dei file relativo alle ultime
10 pubblicazioni**

Per ciascuno degli elementi presenti in elenco è indicata (colonna
"**Data Ora Creazione**") data e ora in cui è stata effettuata la
pubblicazione articoli che ha prodotto poi i relativi file.

I pulsanti presenti in corrispondenza delle colonne "**Elimina**" e
"**Scarica**" consentono invece di:

**Elimina** (
![Videate\\pulsante_elimina_backup_marketplace.bmp](./assets/media/image447.png) ): consente di eliminare definitivamente
i file csv prodotti dalla corrispondente pubblicazione.

**Scarica** (
![Videate\\pulsante_scarica_backup_marketplace.bmp](./assets/media/image448.png) ): consente di effettuare il download
dei relativi file csv.

Nello specifico e come già evidenziato nei precedenti capitoli di questo
manuale, dipendentemente dalla tipologia di articoli coinvolti nella
pubblicazione e dalle lingue gestite nello store Prestashop collegato al
proprio Account per ogni pubblicazione potranno essere prodotti diversi
file. Il pulsante "Scarica" consente quindi di effettuare il download di
uno zip contenente tutti i file prodotti a seguito della relativa
pubblicazione

**ATTENZIONE!** In queste condizioni Passweb si preoccuperà solamente di
creare, a seguito di ogni pubblicazione, i relativi file CSV. Tali file
non saranno copiati e non saranno quindi disponibili attraverso nessuna
area comune per cui l'unica possibilità sarà poi quella di scaricarli
dal Wizard e copiarli manualmente in un area in cui siano effettivamente
accessibili al modulo o alla procedura Prestashop deputata alla loro
elaborazione.

###### PUBBLICAZIONE VIA FTPS

La pubblicazione via FTPS consente di inserire, in maniera completamente
automatica, i file prodotti da Passweb a seguito di ogni operazione di
pubblicazione articoli (indipendentemente dal fatto che sia una
pubblicazione lanciata manualmente o eseguita in automatico a seguito di
una sincronizzazione e/o dell'applicazione di una determinata regola)
all'interno di un'apposita area FTP rendendoli così disponibili al
modulo o alla procedura Prestashop deputata alla loro elaborazione.

**ATTENZIONE!** **sono accettate solo ed esclusivamente connessioni
sicure FTPS (FTP over SSL) in modalità Implicita o Esplicita**. Non sarà
quindi possibile utilizzare semplici connessioni FTP non protette da SSL

Per maggiori informazioni in merito alla propria area FTP e alle
relative modalità di connessione si consiglia di fare riferimento
direttamente al fornitore del servizio

Per attivare questo tipo di repository è necessario, per prima cosa,
impostare il parametro "**Repository CSV**" sull'opzione "**FTPS**"

![](./assets/media/image602.png)

Fatto questo sarà poi necessario impostare anche tutta una serie di
altri parametri necessari per consentire a Passweb di accedere all'area
FTP in esame.

Nello specifico dunque il campo:

- **Username:** consente di impostare lo username di accesso all'area
  FTP in cui dovranno essere copiati i file prodotti da Passweb

- **Password:** consente di impostare la password di accesso all'area
  FTP in cui dovranno essere copiati i file prodotti da Passweb

- **Host:** consente di indicare il percorso della cartella all'interno
  dell'area FTP in cui dovranno poi essere copiati i file prodotti da
  Passweb.

> **ATTENZIONE! E' necessario indicare il percorso completo della
> cartella (comprensivo quindi del nome della cartella stessa). La
> cartella deve inoltre essere già presente all'interno dell'area ftp**

- **Porta:** consente di indicare la porta di accesso su cui è attivo il
  servizio ftp

- **Modalità:** consente di impostare la specifica modalità di
  connessione FTPS (**Implicita** o **Esplicita**) da utilizzare per la
  connessione alla relativa area di appoggio

Nel momento in cui i parametri di accesso impostati non dovessero essere
corretti e/o la cartella di destinazione non dovesse essere già presente
nell'area ftp, in fase di pubblicazione verrà ritornato un apposito
messaggio di errore

Infine, per quel che riguarda la copia dei file prodotti da Passweb
all'interno di quest'area FTP occorre ricordare che:

- **Passweb produrrà file csv distinti per ogni singola lista di
  vendita**

- **Passweb non effettuerà operazioni di cancellazione di file
  eventualmente presenti all'interno della cartella**. Un'eventuale
  eliminazione dei file prodotti da Passweb dopo che il loro contenuto è
  stato correttamente processato ed importato all'interno di Prestashop
  rimane dunque un operazione in carico alla procedura di elaborazione
  di questi stessi file (procedura che come più volte indicato deve
  essere eseguita e gestita esternamente a Passweb)

- Il metodo di scrittura dei file all'interno della cartella FTP è
  regolato dal parametro "**Modalità scrittura file**" precedentemente
  esaminato

- Per garantire un funzionamento corretto della procedura è necessario,
  ovviamente, non alterare in alcun modo ne il nome dei file prodotti da
  Passweb ne tanto meno la loro struttura. Nel momento in cui tale
  vincolo non dovesse essere rispettato si potrebbero riscontrare
  problemi relativi al fatto che ad ogni pubblicazione Passweb andrà a
  riscrivere un nuovo file indipendentemente da quanto impostato per il
  parametro "Modalità scrittura file" o, cosa peggiore, i dati
  all'interno del file potrebbero risultare corrotti causando poi
  problemi in fase di upload all'interno della piattaforma terza.

###### PUBBLICAZIONE VIA GOOGLE DRIVE

La pubblicazione via Google Drive consente di inserire, in maniera
completamente automatica, i file prodotti da Passweb a seguito di ogni
operazione di pubblicazione articoli (indipendentemente dal fatto che
sia una pubblicazione lanciata manualmente o eseguita in automatico a
seguito di una sincronizzazione e/o dell'applicazione di una determinata
regola) all'interno di un'apposita cartella in uno spazio Google Drive
rendendoli così disponibili al modulo o alla procedura Prestashop
deputata alla loro elaborazione.

Per attivare questo tipo di repository è necessario, per prima cosa,
impostare il parametro "**Repository CSV**" sull'opzione "**Google
Drive**"

![](./assets/media/image603.png)

Fatto questo sarà poi necessario impostare anche tutta una serie di
altri parametri necessari per consentire a Passweb di connettersi
correttamente al relativo spazio di Google Drive.

Per maggiori informazioni relativamente a come poter creare in maniera
corretta una cartella Google Drive e a come reperire tutti i parametri
di configurazione necessari per consentire a Passweb di connettersi con
tale cartella si rimanda a quanto indicato nell'analogo capitolo di
questo manuale relativo all'integrazione con Google Merchant
(*Marketplace -- Altri Marketplace -- Google Merchant -- Configurazione
Account -- Metodi di Pubblicazione - Pubblicazione articoli via CSV --
Pubblicazione via Google Drive*)

###### PUBBLICAZIONE VIA URL PASSWEB

La pubblicazione via Url Passweb consente di rendere disponibili i file
prodotti da Passweb a seguito di ogni operazione di pubblicazione
articoli (indipendentemente dal fatto che sia una pubblicazione lanciata
manualmente o eseguita in automatico a seguito di una sincronizzazione
e/o dell'applicazione di una determinata regola) via web a specifici
indirizzi sotto il dominio assegnato al proprio Connettore Passweb.

Per attivare questo tipo di repository è necessario impostare il
parametro "**Repository CSV**" sull'opzione "**URL Passweb**"

![](./assets/media/image604.png)

In queste condizioni non sarà necessario impostare nessun'altro
parametro di configurazione essendo i file in esame disponibili
direttamente via web a specifici indirizzi.

In questo senso per ottenere l' url dei singoli file prodotti da Passweb
sarà necessario concatenare l'indirizzo indicato all'interno del campo
"**URL**" con il nome dello specifico file che si vuole ottenere. Per
maggiori informazioni relativamente al nome assegnato da Passweb ai file
prodotti a seguito di ogni operazione di pubblicazione si veda anche
quanto indicato nel precedente capitolo "*Metodi di Pubblicazione*" di
questo manuale

**ATTENZIONE! In queste condizioni, per ovvie ragioni, NON verrà mai
inserito nel nome file il timestamp dell'operazione.** In caso contrario
infatti il nome dei file sarebbe diverso ad ogni pubblicazione e
diventerebbe quindi complesso poterci accedere non conoscendo
esattamente data e ora della pubblicazione in esame.

Supponendo dunque di fare riferimento alla figura sopra riportata (e
all'indirizzo indicato all'interno del campo URL) e di voler accedere al
file in italiano prodotto a seguito della pubblicazione di articoli
semplici appartenenti alla lista di vendita con id 16, l' url da
considerare sarà esattamente il seguente

**https://www.clobis.net/MarketplaceFeed/15/ArticoliSemplici_16_NomeFileCSV_it.csv**

Infine, anche in questo caso, i dati dell'ultima pubblicazione saranno
gli unici presenti all'interno del file, o andranno in append a quelli
eventualmente prodotti da pubblicazioni precedenti dipendentemente dalle
impostazioni settate per il parametro "**Modalità scrittura file**"

##### ARTICOLI

All'interno del tab "**Articoli**" è possibile impostare i parametri di
configurazione del proprio Account in relazione alla pubblicazione dei
prodotti sul Marketplace.

![](./assets/media/image605.png)

Il parametro "**Magazzino degli articoli**" (sezione "Generale")
consente di indicare quelli che dovranno essere i Magazzini da collegare
all'Account in esame

**ATTENZIONE!** Per poter salvare correttamente l'Account è necessario
indicare almeno un Magazzino. **Inoltre i magazzini indicati all'interno
di questa sezione saranno poi quelli che verranno presi in
considerazione per valutare la disponibilità degli articoli in fase di
applicazione di una regola per la pubblicazione automatica di questi
stessi prodotti sulla piattaforma terza**

Il check "**Invia email articoli**", presente anch'esso all'interno
della sezione "**Generale**" consente invece di abilitare / disabilitare
l'invio delle email relative alle operazioni di pubblicazione articoli
sul relativo marketplace.

**ATTENZIONE!** Nel momento in cui tale check dovesse essere
disabilitato, al termine di una qualsiasi operazione di pubblicazione
articoli (comprese quelle relative a regole di "Messa / Modifica /
Rimessa in Vendita" e a regole di Blocco) non verrà più inviata alcuna
mail. In queste condizioni dunque per controllare l'esito di queste
operazioni sarà necessario utilizzare gli strumenti disponibili
all'interno del Wizard (Log Articolo e Log Liste di Vendita)

La sezione "**Parametri Articolo**" consente di decidere come si dovrà
comportare l'applicativo in relazione all'aggiornamento di eventuali
prezzi creati per specifici gruppi di utenti oltre che ad alcune
specifiche che, di base, dovranno essere gestite obbligatoriamente nelle
varie Inserzioni.

Nello specifico dunque il parametro:

**Aggiornare i listini sul Marketplace**: permette di definire quello
che dovrà essere il funzionamento dell'integrazione Passweb --
Prestashop in relazione alla possibilità di aggiornare o meno, in fase
di pubblicazione articoli, eventuali prezzi speciali definiti per
l'articolo stesso ed associati a specifici gruppi di utenti.

Nel momento in cui il parametro in questione dovesse essere selezionato,
in fase di pubblicazione degli articoli verranno aggiornati su
Prestashop, se necessario, anche eventuali prezzi associati a specifici
Gruppi Utente secondo quanto definito nella maschera di configurazione
della relativa Inserzione (tab "Prezzo, quantità e formato", sezione
"Listini")

Al contrario, **se l'esigenza dovesse essere quella di non modificare in
fase di pubblicazione, eventuali prezzi** definiti direttamente su
Prestashop ed associati a specifici Gruppi Utente, sarà necessario
verificare di non aver selezionato il parametro in questione.

Per maggiori informazioni relativamente alla possibilità di associare ai
gruppi utente definiti in Prestashop specifici listini gestionali
(creando così i relativi prezzi speciali) si veda anche quanto indicato
all'interno del capitolo "*Altri Marketplace -- Gestione Inserzioni --
Creazione di una nuova Inserzione -- Prezzo Quantità Formato -- Prezzo*"
di questo manuale.

**Sovrascrivere il titolo sul Marketplace**: permette di definire quello
che dovrà essere il funzionamento dell'integrazione Passweb --
Prestashop in relazione alla specifica "**Name**".

Tale specifica è obbligatoria e dovrà quindi essere necessariamente
gestita in ogni singola Inserzione utilizzata per pubblicare i prodotti.
In conseguenza di ciò, di base, **il Nome dell'articolo su Prestashop
sarà controllato da Passweb**

**ATTENZIONE!** Nel caso di articoli a **taglie e/o colori**, o comunque
gestiti mediante Inserzioni che contengono elementi di variazione, per
variare il titolo di quello che su Prestashop è un articolo padre sarà
necessario effettuare la pubblicazione di almeno un articolo figlio. Per
maggiori informazioni relativamente a come vengono costruiti su
Prestashop i Titoli di articoli padre si veda anche quanto indicato
all'interno del capitolo "*Marketplace -- Altri Marketplace --
Prestashop -- Pubblicazione di articoli a Taglie e Colori*" di questo
manuale.

Nel momento in cui l'esigenza dovesse essere invece quella di **non
modificare il nome del prodotto su Prestashop** (ad esempio perché
l'articolo era già presente sulla piattaforma terza o perché dopo essere
stato pubblicato sono state fatte delle modifiche in tal senso
direttamente su Prestashop), sarà necessario verificare **di NON aver
selezionato il parametro in esame**

**Sovrascrivere la categoria di default sul Marketplace**: permette di
definire quello che dovrà essere il funzionamento dell'integrazione
Passweb -- Prestashop in relazione alla specifica "**Category
Default**".

Tale specifica è obbligatoria e dovrà quindi essere necessariamente
gestita in ogni singola Inserzione utilizzata per pubblicare i prodotti.
In conseguenza di ciò, di base, **l'associazione del prodotto alla
categoria merceologica principale** **sarà controllata da Passweb**

**ATTENZIONE!** In queste condizioni se dovessero essere apportate delle
variazioni alla categoria principale che Passweb trasmette a Prestashop,
al termine della pubblicazione verrà correttamente impostata, per gli
articoli coinvolti, la nuova categoria principale **mentre la vecchia
continuerà ad essere associata a questi stessi articoli come categoria
secondaria**. Nel momento in cui l'esigenza dovesse essere quella di
eliminare anche l'associazione con la categoria secondaria, tale
operazione dovrà essere effettuata direttamente su Prestashop.

Nel momento in cui l'esigenza dovesse essere invece quella di **non
modificare su Prestashop l'associazione "articolo -- categoria
merceologica principale"** (ad esempio perché l'articolo era già
presente sulla piattaforma terza o perché dopo essere stato pubblicato
sono state fatte delle modifiche in tal senso direttamente su
Prestashop), sarà necessario verificare **di NON aver selezionato il
parametro in esame**

**ATTENZIONE!** i parametri "**Aggiornare i listini sul Marketplace**",
"**Sovrascrivere il titolo sul Marketplace**" e "**Sovrascrivere la
categoria di default sul Marketplace**" sono configurati tutti a livello
di Account e si comporteranno quindi allo stesso modo per tutte le
inserzioni e le liste di vendita che fanno a capo ad esso. **Tutti e tre
i parametri, inoltre, risulteranno essere selezionati a default**

**Escludi Feed Immagini**: consente, se selezionato, di inibire la
trasmissione alla piattaforma terza di eventuali immagini articolo
caricate direttamente all'interno del gestionale Passepartout.

Ovviamente, nel momento in cui si dovesse decidere di selezionare questo
parametro, sarà poi inutile gestire nelle Inserzioni collegate
all'Account in esame, eventuali specifiche legate alle immagini
articolo.

**ATTENZIONE!** Il parametro "**Escludi Feed Immagini**" a default
risulta essere NON selezionato.

Nel momento in cui l'esigenza dovesse essere dunque quella di non
inviare mai le immagini articolo alla piattaforma terza,
indipendentemente dal fatto di averle o meno inserite sul gestionale
Passepartout, sarà necessario accertarsi di aver correttamente
selezionato il parametro in esame

La sezione "**Backup**" consente, infine, di impostare alcuni parametri
di configurazione relativamente al backup effettuato automaticamente da
Passweb ad ogni pubblicazione per gli articoli presenti, in quello
stesso momento, sulla piattaforma terza.

Nello specifico il parametro:

**Formato del file di backup:** consente di impostare il formato di file
da utilizzare in relazione alla funzione di download del relativo
backup, funzione questa che potrà poi essere eseguita cliccando
sull'apposito pulsante (
![Videate\\pulsante_scarica_backup_marketplace.bmp](./assets/media/image448.png) ): presente nella sezione "**Backup**"
della maschera "**Dati Account**".

E' possibile selezionare una delle seguenti opzioni:

- **JSON:** in queste condizioni in fase di download verrà scaricato un
  unico file .json contenente tutte le informazioni salvate da Passweb
  prima della pubblicazione che ha portato alla generazione di quello
  stesso backup.

- **CSV:** in queste condizioni in fase di download verranno generati e
  scaricati all'interno di un apposito file zip, per ciascuna delle
  lingue gestite nello store Prestashop definito sull'Account di
  integrazione, **due distinti file .csv**, uno relativo agli articoli
  semplici (es. backup_345_articoliSemplici_it.csv) e uno relativo
  invece alle combinazioni (es. backup_345_combinazioni_it.csv) presenti
  su Prestashop al momento del backup.

> In queste condizioni sarà inoltre possibile selezionare dal relativo
> menu a tendina (campo "**Separatore File CSV**") il carattere da
> utilizzare, in fase di creazione dei relativi file, come carattere di
> separazione dei vari campi.

Per quel riguarda i file di **backup in formato json** occorre poi
sottolineare che:

- Il file in formato json verrà generato e salvato automaticamente da
  Passweb prima di ogni pubblicazione/modifica/arresto di un articolo
  sulla piattaforma terza

- All'interno del file json non sono presenti, ovviamente, tutti i dati
  gestiti su Prestashop per i vari articoli ma solamente quelli ottenuti
  da Prestashop stesso a seguito di apposite chiamate API

Per quel che riguarda i file di **backup in formato csv** occorre invece
sottolineare che:

- Tali file verranno generati a runtime (ossia direttamente in fase di
  download) partendo dal corrispondente file json. In conseguenza di ciò
  i campi presenti all'interno del file (e quindi le varie intestazioni
  del tracciato csv) così come i relativi valori, corrispondono con
  quanto presente all'interno del file json, anche se, ovviamente, tali
  campi potranno poi essere organizzati in maniera diversa.

- Nel caso di campi che accettano valori multipli (es. categorie
  merceologiche) come carattere di separazione dei singoli valori verrà
  utilizzato il carattere "**,**"

- Per quel che riguarda le "Funzionalità" queste verranno salvate nel
  formato standard richiesto da Prestashop e quindi come
  "**Nome:Valore:Posizione:Personalizzato**". Nel momento in cui poi
  dovessero essere gestite, per un determinato articolo più
  "Funzionalità", ogni blocco "Nome:Valore:Posizione:Personalizzato"
  sarà separato (come per i valori multipli) dal carattere "**,**"

- Nel caso in cui nello store Prestashop collegato all'account in esame,
  siano gestite più lingue, verranno inseriti all'interno di un apposito
  file .zip due distinti file (articoli semplici e combinazioni) per
  ciascuna delle lingue gestite.

**ATTENZIONE!** **Si consiglia di effettuare un download di esempio dei
file di backup sia in formato json che in formato csv in maniera tale da
poter verificare l'effettiva struttura di questi stessi file e i dati in
essi contenuti**

Per maggiori informazioni in merito alla funzione di backup si veda
anche quanto indicato all'interno del successivo capitolo
"*Configurazione Account -- Backup*" di questo manuale.

In ogni caso occorre sempre considerare che i backup effettuati da
Passweb non sono copie omnicomprensive di tutte le informazioni presenti
su Prestashop, ma contengono solo ed esclusivamente i dati ottenuti da
Prestashop stesso a seguito di determinate chiamate API.

**In considerazione di ciò i backup di Passweb non devono in alcun modo
andare a sostituire quelli effettuati direttamente da Prestashop che,
per ragioni di sicurezza dovranno, ovviamente, essere effettuati
regolarmente e direttamente sulla piattaforma terza in modo tale da
poter ripristinare tutte le informazioni necessarie nel momento in cui
dovessero verificarsi problemi di qualsiasi tipo.**

##### ORDINI

All'interno di questa sezione è possibile decidere se l'Account in esame
dovrà interagire o meno con la piattaforma terza anche a livello di
ordini ed eventualmente in che modo.

![](./assets/media/image606.png)

Per maggiori informazioni in merito si rimanda a quanto indicato
all'interno del successivo capitolo "*Configurazione Ordini*"

##### CLIENTI

All'interno di questa sezione è possibile decidere se aggiornare o meno,
a seguito di apposite operazioni di sincronizzazione, le anagrafiche dei
clienti presenti su Passweb con i dati prelevati direttamente dalla
piattaforma esterna.

![](./assets/media/image607.png)

Per maggiori informazioni in merito alla gestione dei clienti si veda
anche quanto indicato all'interno del successivo capitolo "*Codifica
Automatica di nuove anagrafiche utente*"

##### SCHEDULAZIONE

All'interno di questa sezione è possibile schedulare le operazioni di
sincronizzazione automatica tra Passweb e la piattaforma esterna.

![](./assets/media/image318.png)

Per maggiori informazioni in merito alla gestione dei clienti si veda
anche quanto indicato all'interno del successivo capitolo
"*Sincronizzazione*"

##### BACKUP

All'interno di questa sezione è possibile visualizzare e gestire i
backup effettuati da Passweb relativamente alle anagrafiche articolo dei
prodotti presenti sulla piattaforma terza prima della pubblicazione
effettuata da Passweb stesso.

Prima di procedere all'analisi delle funzionalità e dei campi presenti
all'interno di questa maschera occorre fare alcune considerazioni di
fondamentale importanza.

In questo senso è bene quindi sottolineare che, prima di ogni
pubblicazione/modifica/arresto di un articolo sulla piattaforma terza,
Passweb leggerà l'elenco di tutti i prodotti attualmente presenti sulla
piattaforma stessa e salverà determinati dati delle relative anagrafiche
all'interno di un apposito file json, file questo che potrà poi essere
scaricato in locale e, se necessario, utilizzato come base dati da
ripristinare sulla piattaforma terza.

**ATTENZIONE!** Il backup effettuato da Passweb non è una copia
omnicomprensiva di tutte le informazioni presenti sulla piattaforma
terza per i vari articoli. All'interno dei file di backup vengono
salvate unicamente le informazioni restituite da Prestashop stesso a
seguito di apposite chiamate API che, nello specifico, sono quelle di
seguito indicate:

- **http://www.urlsito.it/api/products**

- **http://www.urlsito.it/api/combinations**

- **http://www.urlsito.it/api/stock_availables**

- **http://www.urlsito.it/api/product_features**

- **http://www.urlsito.it/api/product_options**

- **http://www.urlsito.it/api/product_option_values**

Nel momento in cui a seguito di una determinata pubblicazione effettuata
da Passweb dovessero quindi essere rilevati determinati problemi, come
ad esempio la perdita e/o la sovrascrittura indesiderata di specifiche
informazioni, sarà possibile scaricare il relativo file json in maniera
tale da verificare quella che era la situazione prima della
pubblicazione stessa ed eventualmente ripristinarla.

Il ripristino potrà essere effettuato mediante procedure personalizzate
di elaborazione del file di backup, procedure queste che dovranno essere
sviluppate ad hoc secondo le specifiche esigenze del caso **e che non
sono in carico a Passepartout**.

Considerando poi che il file di backup potrà essere scaricato in formato
json ma anche in formato csv (dipendentemente dalle impostazioni settate
per il corrispondente parametro Passweb) il ripristino potrebbe anche
essere effettuato mediante le funzioni standard di import dati presenti
sulla piattaforma terza oppure mediante l'utilizzo di appositi moduli
gestibili, anch'essi, direttamente sulla piattaforma terza.

**ATTENZIONE! Le immagini dei prodotti presenti su Prestashop non sono
mai oggetto di backup da parte di Passweb**

**ATTENZIONE!!** In ogni caso, è sempre bene considerare che i backup
effettuati da Passweb non sono copie omnicomprensive di tutte le
informazioni presenti su Prestashop, ma contengono solo ed
esclusivamente i dati ottenuti da Prestashop stesso a seguito delle
chiamate API precedentemente indicate.

**In considerazione di ciò i backup di Passweb non devono in alcun modo
andare a sostituire quelli effettuati direttamente da Prestashop che,
per ragioni di sicurezza dovranno, ovviamente, essere effettuati in
maniera regolare e direttamente sulla piattaforma terza in modo tale da
poter ripristinare tutte le informazioni necessarie nel momento in cui
dovessero verificarsi problemi di qualsiasi tipo.**

Una volta effettuato l'accesso alla sezione "Backup" della maschera
"Dati Account" verrà quindi visualizzato un elenco di tutti i Backup
attualmente disponibili

![](./assets/media/image319.png)

**ATTENZIONE! Passweb conserva in automatico i backup effettuati negli
ultimi 7 giorni**

Per ciascuno degli elementi presenti in elenco è indicata (colonna
"**Data del backup**") data e ora in cui è stato effettuato il relativo
backup che, sulla base di quanto detto, corrisponderanno esattamente con
la data e l'ora della specifica operazione di
pubblicazione/modifica/arresto effettuata da Passweb e che ha prodotto
la creazione del relativo file di backup.

I pulsanti presenti in corrispondenza delle colonne "Elimina" e
"Scarica" consentono invece di:

**Elimina** (
![](./assets/media/image608.png) ): consente di eliminare definitivamente
il corrispondente file di backup.

In questo senso è bene ricordare, come precedentemente evidenziato, che
Passweb conserva al massimo i backup degli ultimi 7 giorni e che
l'eliminazione automatica dei file antecedenti a tale data avverrà solo
a seguito di una nuova pubblicazione/modifica/arresto di articoli sulla
piattaforma terza (e conseguentemente a seguito della creazione di un
nuovo file di backup)

In conseguenza di ciò se per un determinato periodo di tempo non
dovessero essere effettuate pubblicazioni di alcun tipo, non verrebbero
neppure eliminati file di backup anche se più vecchi di 7 giorni.
Inoltre nel momento in cui a seguito di una certa pubblicazione
dovessero risultare da eliminare tutti i backup presenti in elenco,
Passweb provvederà comunque a mantenere attivi gli ultimi 5, in maniera
tale da poter sempre avere uno storico da ripristinare.

Per comprendere meglio questo discorso consideriamo il seguente esempio:

**[ESEMPIO]{.underline}**

Periodo di conservazione dei backup: 7 giorni

Supponiamo di effettuare nel periodo che va dal 10/11/2021 al
17/11/2021, 20 pubblicazioni e supponiamo poi di sospendere queste
pubblicazioni fino al 30/11/2021

In queste condizioni quando il 1/12/2021 torneremo a fare una nuova
pubblicazione di articoli ci ritroveremo ad avere, nella sezione Backup,
20 file tutti più vecchi di 7 giorni e che quindi dovrebbero essere
eliminati.

Come detto però Passweb manterrà sempre uno storico di almeno gli ultimi
5 backup effettuati per cui a seguito della pubblicazione del 1/12/2021
avremo disponibili un file di backup effettuato in tale data (che
rientra quindi nel criterio dei 7 giorni di conservazione) e gli ultimi
4 dei 20 presenti prima della pubblicazione stessa (e che risulteranno
quindi essere più vecchi degli ultimi 7 giorni).

**Scarica** (
![](./assets/media/image448.png) ): consente di effettuare il download
dei relativi file di backup.

Nello specifico, per ciascuno dei backup presenti in elenco sarà
possibile decidere di scaricare, utilizzando il corrispondente menu a
tendina:

- i dati di tutti gli articoli presenti su Prestashop prima della
  pubblicazione/modifica/arresto effettuata da Passweb che ha prodotto
  la creazione del relativo file di backup -- opzione **Tutti**

- i dati dei soli articoli presenti su Prestashop e gestiti direttamente
  da Passweb -- opzione "**Gestiti su Passweb**"

- i dati degli articoli presenti su Prestashop e gestiti da Passweb
  mediante una specifica lista di vendita -- opzione corrispondente al
  **nome della singola Lista di Vendita**

Una volta indicata la tipologia di dati che si desidera ottenere,
cliccando sul pulsante di download (
![Videate\\pulsante_scarica_backup_marketplace.bmp](./assets/media/image448.png) ) verrà prodotto e scaricato sulla
macchina dell'utente un archivio compresso (.zip) contenente i file di
backup richiesti.

Tali file saranno in formato json o csv in base alle impostazioni
settate per il parametro "**Formato del File di Backup**" presente
all'interno del tab "Articoli"

![](./assets/media/image609.png)

In particolare, nel momento in cui il parametro evidenziato in figura
dovesse essere impostato sul valore **JSON**, all'interno del file .zip
sarà presente un unico file .json contenente tutte le informazioni
richieste

Nel caso in cui il parametro evidenziato in figura dovesse invece essere
impostato sul valore **CSV**, all'interno del file .zip saranno presenti
, per ciascuna delle lingue gestite nello store Prestashop definito
sull'Account di integrazione, **due distinti file .csv**, uno relativo
agli articoli semplici (es. backup_345_articoliSemplici_it.csv) e uno
relativo invece alle combinazioni (es. backup_345_combinazioni_it.csv)
presenti su Prestashop al momento del backup.

Il pulsante "**Scarica qui un file di esempio**", presente nella
maschera relativa ai backup, consente di effettuare il download di un
esempio di file di backup generati da Passweb (sia in formato json che
in formato csv)

![](./assets/media/image610.png)

**Prima di procedere ad un eventuale ripristino si consiglia sempre di
scaricare il file di esempio in maniera tale da poter verificare
esattamente l'effettiva struttura dei file di backup e i dati in essi
contenuti**

Occorre infatti sottolineare che nei file di backup generati da Passweb
(sia in formato json che in formato csv) possono essere presenti anche
dei campi che non sono poi mappabili mediante la funzionalità di
importazione dati presente a default su Prestashop. Alcuni esempi in
questo senso possono essere rappresentati dai seguenti campi:

- **Id_Category_Default**: campo che riporta l'identificativo della
  categoria di default assegnata in Prestashop al corrispondente
  articolo. Questo campo non è mappabile direttamente mediante la
  funzionalità di importazione standard presente su Prestashop, per cui
  lo stesso identificativo è stato inserito come primo elemento anche
  all'interno del campo "**Categorie**" (che conterrà l'elenco degli id
  di tutte le categorie associate all'articolo)

- **Location**: campo che contiene il valore del parametro "**Ubicazione
  di magazzino**" presente nel tab "**Quantità**" dell'anagrafica
  articolo di Prestashop.

- **Additional_Delivery_Times**: campo che contiene il valore (0/1/2)
  del radio button corrispondente al parametro "**Tempi di consegna**"
  presente nel tab "**Spedizione**" dell'anagrafica articolo di
  Prestashop

- **Show_Condition**: campo che contiene il valore del flag (0/1)
  "**Mostra la condizione nella pagina del prodotto**" presente nel tab
  "**Opzioni**" dell'anagrafica articolo di Prestasho**p**

- **Unit_Price_Ratio**: campo che contiene il fattore di conversione
  utilizzato per calcolare, a partire dal prezzo dell'articolo, il suo
  prezzo unitario

- ...

Nel momento in cui l'esigenza dovesse essere quindi quella di importare
in Prestashop dati del tipo di quelli sopra indicati sarà necessario
operare direttamente da Prestashop mediante apposite personalizzazioni o
eventuali moduli aggiuntivi.

**ATTENZIONE!** In ogni caso, come già evidenziato in precedenza,
eventuali procedure personalizzate di elaborazione dei file di backup, e
successivo ripristino dei relativi dati sulla piattaforma terza, **non
sono in carico a Passepartout**

##### DOWNLOAD CSV

All'interno di questa sezione, visibile solo nel momento in cui si
dovesse decidere di adottare come metodo di pubblicazione dei prodotti
la pubblicazione via CSV (indipendentemente dal tipo di repository
utilizzato), sarà possibile visualizzare e gestire in maniera manuale i
vari file prodotti da Passweb a seguito di una qualsiasi operazione
(automatica o manuale) di pubblicazione / arresto articoli

![](./assets/media/image320.png)

**ATTENZIONE! Passweb conserva uno storico dei file relativo alle ultime
10 pubblicazioni effettuate**

Si ricorda inoltre che anche eventuali operazioni di "Arresto Articoli"
indipendentemente dal fatto di essere effettuate manualmente o
automaticamente a seguito dell'applicazione di una determinata regola,
verranno ovviamente considerate come delle "pubblicazioni" e produrranno
quindi, all'interno della sezione in esame, i relativi file CSV.

**In ogni caso, un' eventuale elaborazione dei file csv prodotti da
Passweb così come l'effettivo upload dei relativi dati nella piattaforma
terza restano operazioni in carico a chi gestisce effettivamente lo
specifico sito Prestashop**

