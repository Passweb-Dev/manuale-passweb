# AREE DI SPEDIZIONE



La sezione "**Aree di Spedizione**", presente nella maschera di
configurazione di ogni Consegna consente di definire le aree geografiche
(**identificate poi con i relativi indirizzi di spedizione merce**)
entro cui la Consegna in esame dovrà essere ritenuta valida.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_aree_spedizione.bmp](./assets/media/image383.png){width="4.565277777777778in"
height="1.6819444444444445in"}

**ATTENZIONE!** Ovviamente affinché la consegna in esame possa essere
effettivamente utilizzabile all'interno del sito è necessario assegnarle
almeno un'Area di Spedizione. In conseguenza di ciò, nel momento in cui
non dovesse essere indicata in maniera specifica nessuna Area di
Spedizione per la consegna in esame, al salvataggio questa verrà
automaticamente impostata come valida per "**Tutto il mondo**"

Allo stesso modo considerando che ogni consegna dovrà essere associata
ad almeno un Metodo di Trasporto è semplice comprendere come **le Aree
di Spedizione definite per la consegna debbano essere incluse nelle zone
di spedizione impostate per il trasporto ad essa associato**.

Nel momento in cui si dovesse infatti associare, ad esempio, ad una
consegna valida per l'Emilia Romagna un metodo di spedizione valido per
la Toscana, ovviamente quel tipo di consegna non potrà mai essere
selezionato all'interno del sito inquanto un indirizzo di spedizione (in
Toscana) utile alla visualizzazione del metodo di trasporto
pregiudicherebbe la visualizzazione della consegna (valida solo in
Emilia Romagna) e viceversa.

In fase di codifica delle aree geografiche sarà possibile agire in
maniera inclusiva, andando quindi ad includere una ad una tutte le aree
geografiche da associare alla Consegna in esame, oppure, volendo sarà
possibile operare anche in maniera esclusiva andando cioè ad escludere
per la Consegna in esame determinate aree geografiche.

**Ovviamente nel momento in cui si dovesse decidere di lavora in maniera
"esclusiva" sarà comunque indispensabile includere per la stessa
Consegna almeno un'area geografica valida**

**ATTENZIONE!** Consegne con sole aree geografiche da escludere non
avrebbero, ovviamente, alcun senso

In altri termini supponendo, ad esempio, di dover gestire le consegne in
tutta Italia tranne che ad Anacapri, anziché andare ad includere uno ad
uno tutte le regioni e le provincie gestite potremmo, in maniera molto
più semplice:

- Creare una prima area geografica corrispondente a tutta l'Italia e
  quindi con le opzioni:

  - Gestione = Includi

  - Nazione = Italy

- Creare una seconda area geografica da escludere relativa alla sola
  città di Anacapri e quindi con le opzioni:

  - Gestione = Escludi

  - Nazione = Italy

  - Provincia = Napoli

  - CAP = 80071

Per includere o escludere determinate aree geografiche dalla Consegna in
esame è sufficiente agire dai relativi pulsanti presenti nella barra
degli strumenti della sezione "Aree di Spedizione", pulsanti questi che
consentono rispettivamente di:

**Italia** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_italia.bmp](./assets/media/image303.png){width="0.2791666666666667in"
height="0.1951388888888889in"} ): consente di gestire le arre di
spedizione relative al territorio italiano.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Configurazione Italia**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_italia_delivery.bmp](./assets/media/image384.png){width="5.759722222222222in"
height="3.3180555555555555in"}

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa
consegna

**ATTENZIONE!** si ricorda che consegne con sole aree geografiche da
escludere non avrebbero, ovviamente, alcun senso

Nel momento in cui si dovesse decidere, dunque, di escludere determinate
aree geografiche da una consegna sarà di fondamentale importanza
verificare che, per la stessa zona, sia presente, almeno, anche un' area
geografica il cui parametro "**Gestione**" è stato correttamente
impostato su "**Includi**"

**Regione / Provincia / Località / CAP**: consente di specificare la
Regione / Provincia / Località / CAP dell'area geografica che si sta
codificando

Per aggiungere un nuovo C.A.P. sarà sufficiente indicarlo all'interno
dell'apposito campo e confermare poi da tastiera con il pulsante
"Invio".

In fase di inserimento dei C.A.P è inoltre possibile utilizzare il
carattere "\_" come wildcard per sostituire uno dei caratteri
effettivamente presenti nel relativo codice di avviamento postale.

**ATTENZIONE!** è fondamentale gestire correttamente il carattere \_
ricordando sempre che **un "underscore" sostituisce un solo carattere**

Supponendo dunque di indicare come C.A.P. il valore "4_900" verranno poi
presi in considerazione e validati tutti i codici di avviamento postale
che hanno come primo carattere 4, come secondo carattere un qualunque
valore, come terzo carattere 9, come quarto carattere 0 e come quindi
carattere ancora 0

Supponendo invece di indicare come C.A.P. il valore "**47\_\_\_**" (47
seguito da tre distinti caratteri di underscore), verranno poi presi in
considerazione e validati tutti i codici di avviamento postale che
iniziano con 47 e che proseguono con altri 3 caratteri qualsiasi.

> **NOTA BENE:** la differenziazione per Regione, Provincia e Codice di
> Avviamento Postale può essere effettuata solo ed esclusivamente per la
> nazione Italia.

Il campo "**Ore aggiuntive consegna**" (presente anche nel momento in
cui si dovessero configurare aree di spedizione diverse dall'Italia)
consente invece di indicare il numero di ore necessarie per portare a
termine la consegna sulla specifica area di spedizione, ore queste che
andranno poi ad aggiungersi a quelle già indicate, a livello generale,
mediante l'apposito parametro presente nella maschera di configurazione
della Consegna in questione.

**ATTENZIONE!** si ricorda che le ore di consegna indicate andranno poi
ad influire sugli intervalli di consegna effettivamente selezionabili
dall'utente in fase di checkout

Il pulsante "**Salva**" presente nella parte bassa della pagina consente
di salvare l'area geografica codificata accodandola a quelle già
presenti in elenco.

In questo senso è necessario considerare anche le seguenti casistiche:

- Se è già presente in elenco un'area geografica precedentemente
  codificata come "**Italia -- Tutte le regioni**" e, per la nuova area
  che si sta codificando, viene indicata invece oltre alla nazione
  Italia anche una specifica regione e/o provincia, alla conferma l'area
  "Italia-Tutte le Regioni" sarà automaticamente rimossa e sostituita
  dalla specifica area appena codificata

- Se in elenco sono già presenti una o più aree geografiche del tipo
  "**Italia-Regione-Specifica Provincia**" e per la nuova area che si
  sta codificando viene selezionata l'opzione "Tutte le regioni", alla
  conferma tutte le aree "Italia-Regione-Provincia" saranno rimosse

- Se è già presente in elenco un'area geografica codificata come
  "**Italia-Regione-Provincia-Cap**" e per la nuova area che si sta
  codificando viene indicata, oltre alla nazione Italia, anche la stessa
  regione e la stessa provincia ma non il CAP, alla conferma l'area
  precedentemente presente in elenco verrà eliminata e sostituita da
  quella nuova appena codificata

- Se è già presente in elenco un'area geografica codificata come
  "**Italia- Regione-Provincia**" e per la nuova area che si sta
  codificando viene indicata, oltre alla nazione Italia, anche la stessa
  regione, la stessa provincia e in più anche una specifica località e/o
  uno specifico CAP, alla conferma l'area precedentemente presente in
  elenco verrà eliminata e sostituita da quella nuova appena codificata.

- Se è già presente in elenco un'area geografica codificata come
  "**Italia -Regione-Provincia -- Località**" e per la nuova area che si
  sta codificando viene indicata, oltre alla nazione Italia anche la
  stessa regione, la stessa provincia, la stessa località e in più
  vengono indicati anche specifici CAP, alla conferma l'area
  precedentemente presente in elenco verrà eliminata e sostituita da
  quella nuova appena codificata.

- Se sono già presenti in elenco aree geografica codificate come
  "**Italia -- Regione-Provincia --Località --CAP**" e per la nuova area
  che si sta codificando viene indicata oltre alla nazione Italia anche
  la stessa regione, la stessa provincia e la stessa la località ma non
  il CAP, alla conferma tutte le aree precedentemente codificate anche
  il CAP associato verranno eliminate e sostituite da quella nuova
  appena codificata.

- Se sono già presenti in elenco aree geografica codificate come
  "**Italia -- Regione - Provincia --Località --CAP**" e per la nuova
  area che si sta codificando viene indicata oltre alla nazione Italia
  anche la stessa regione e la stessa provincia ma non il CAP e la
  Località, alla conferma tutte le aree precedentemente codificate anche
  il CAP e la località associata verranno eliminate e sostituite da
  quella nuova appena codificata.

**Paesi Esteri** (
![Videate\\pulsante_paesi_esteri.bmp](./assets/media/image385.png){width="0.5131944444444444in"
height="0.21458333333333332in"} ): consente di associare alla consegna
che si sta codificando una specifica area geografica all'interno di una
nazione diversa dall'Italia.

Cliccando su questo pulsante verrà visualizzata la maschera
"**Configurazione Paesi Esteri**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_configurazione_paesi_esteri.bmp](./assets/media/image386.png){width="5.584722222222222in"
height="3.441666666666667in"}

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa
consegna

**ATTENZIONE!** si ricorda che consegne con sole aree geografiche da
escludere non avrebbero, ovviamente, alcun senso

Nel momento in cui si dovesse decidere, dunque, di escludere determinate
aree geografiche da una zona di spedizione sarà di fondamentale
importanza verificare che, per la stessa zona, sia presente, almeno,
anche un' area geografica il cui parametro "**Gestione**" è stato
correttamente impostato su "**Includi**"

**Nazione / Stato / Provincia / Località / CAP**: consente di
specificare la Nazione, lo Stato / Provincia, la Località e il CAP
dell'area geografica che si sta codificando

Nel momento in cui l'esigenza dovesse essere quella di inserire,
all'interno di una zona geografica, più provincie contemporaneamente,
sarà sufficiente selezionarle dal relativo elenco sulla sinistra in
corrispondenza del campo "Stato / Provincia" ed inserirle in quello di
destra cliccando sull'icona della piccola freccia verde rivolta verso
destra.

Anche in questo caso in fase di inserimento di eventuali C.A.P sarà
possibile utilizzare il carattere "\_" come wildcard per sostituire uno
dei caratteri effettivamente presenti nel relativo codice di avviamento
postale.

**Nazioni** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nazioni.bmp](./assets/media/image308.png){width="0.38333333333333336in"
height="0.1951388888888889in"} ): consente di definire le arre di
consegna a livello di intere Nazioni

Cliccando su questo pulsante verrà visualizzata la maschera
"**Configurazione Nazioni**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_configurazione_nazioni.bmp](./assets/media/image387.png){width="5.584722222222222in"
height="3.441666666666667in"}

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa
consegna

**ATTENZIONE!** si ricorda che consegne con sole aree geografiche da
escludere non avrebbero, ovviamente, alcun senso

Nel momento in cui si dovesse decidere, dunque, di escludere determinate
aree geografiche da una zona di spedizione sarà di fondamentale
importanza verificare che, per la stessa zona, sia presente, almeno,
anche un' area geografica il cui parametro "**Gestione**" è stato
correttamente impostato su "**Includi**"

**Nazioni:** consente di indicare l'elenco delle Nazioni che devono
essere associate alla consegna che si sta codificando

Per associare alla consegna una specifica Nazione, è sufficiente
selezionarla dall'elenco di sinistra ed inserirla in quello di destra
cliccando sul pulsante raffigurante una piccola freccia verde rivolta
verso destra. Allo stesso modo per eliminare l'associazione tra le zona
di consegna in esame ed una specifica Nazione, sarà sufficiente
selezionarla dall'elenco di destra e cliccare poi sul pulsante
raffigurante la piccola freccia rossa rivolta verso sinistra

**Importa da file**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_da_file.bmp](./assets/media/image388.png){width="0.6166666666666667in"
height="0.1951388888888889in"} ): consente di definire le varie aree
geografiche importandole in blocco da un file di tipo txt o csv
appositamente formattato.

Cliccando su questo pulsante verrà infatti visualizzata un'ulteriore
sezione "**Importazione Aree da File**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_aree_da_file.bmp](./assets/media/image310.png){width="5.792361111111111in"
height="3.5131944444444443in"}

all'interno della quale poter selezionare (campo **File**), importandolo
ad esempio dal proprio pc, il file .txt o .csv con indicate tutte le
aree geografiche da codificare.

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che è stato utilizzato
all'interno del file di importazione come separatore per i vari campi

Affinché la procedura possa terminare in maniera corretta è necessario
che il file txt o csv utilizzato soddisfi determinate regole. Nello
specifico:

- L'intestazione, ossia la prima riga del file, deve essere costituita
  dai seguenti campi

> *gestione;nazione;provincia;localita;cap;km*

- per ogni record del file (e quindi per ogni area geografica) è
  possibile inserire, nell'ordine indicato, le seguenti informazioni:

  - **gestione: 0** nel caso in cui la relativa area geografica debba
    essere inclusa nella Zona, **1** nel caso in cui la relativa area
    geografica debba essere esclusa

> **ATTENZIONE!** Il campo "gestione" non è obbligatorio e può quindi
> anche non essere inserito nel tracciato record del file di
> importazione. In questo caso (**campo non specificato**) **la relativa
> area geografica verrà considerata, a default, come inclusa** nella
> consegna

- **nazione**: codice iso a 2 caratteri della nazione

- **provincia**: sigla della provincia

- **localita**: nome della localita

- **cap**: codice di avviamento postale della localita (con possibilità
  di utilizzare il carattere \_ come carattere wildcard)

- **oreconsegna**: numero di ore necessarie per portare a termine la
  consegna sulla relativa zona geografica.

> **ATTENZIONE**! le ore indicate all'interno di questo campo andranno
> poi a sommarsi, solo per la zona geografica in esame, a quelle
> generali definite a livello di Consegna

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.

> In questo senso è quindi necessario che il valore dei campi contenenti
> interruzioni di riga, doppi apici e/o lo stesso carattere utilizzato
> anche come separatore sia necessariamente racchiuso da virgolette

Supponendo di voler utilizzare come carattere separatore il ; la
struttura del file potrebbe quindi essere:

FR;;;;

IT;SA;;;

IT;RN;;47900;

IT;RN;Viserbella;;

IT;RN;Viserba;47922;2

Nelle condizioni sopra indicate verrebbero quindi aggiunte 5 distinte
aree geografiche: la prima relativa alla nazione Francia, la seconda
relativa all'area geografica corrispondente alla provincia di Salerno in
Italia, la terza relativa alla provincia di Rimini e nello specifico al
codice di avviamento postale 47900, la quarta relativa alla provincia di
rimini e nello specifico alla località Viserbella, la quinta sempre
relativa alla provincia di rimini ma più specificatamente alla località
Viserba e al codice di avviamento postale 47922.

In quest'ultimo caso inoltre verranno considerate anche, per la relativa
zona, un tempo di consegna aggiuntivo pari a due ore.

> **NOTA BENE:** nel caso di "Importazione da file" non verranno
> effettuati controlli di alcun tipo relativamente alle aree geografiche
> eventualmente già associate alla zona in esame. Occorre quindi fare
> particolare attenzioni, in queste condizioni, a non inserire delle
> aree geografiche doppie o triple.

**Esporta** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image311.png){width="0.3506944444444444in"
height="0.18194444444444444in"} ): consente di esportare all'interno di
un file csv, nello stesso formato valido anche per l'importazione,
l'elenco di tutte le aree geografiche attualmente presenti in elenco.

Cliccando su questo pulsante verrà infatti visualizzata un'ulteriore
sezione "**Esportazione Aree**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_aree.bmp](./assets/media/image312.png){width="5.792361111111111in"
height="3.5131944444444443in"}

all'interno della quale poter indicare il carattere separatore che dovrà
essere utilizzato in fase di creazione del file csv.

Il pulsante "**Salva**" presente nella parte bassa della maschera
consente di avviare la procedura di esportazione

**Elimina Area** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_zona_geografica.bmp](./assets/media/image313.png){width="0.4673611111111111in"
height="0.18194444444444444in"} ): consente di eliminare l'area
geografica attualmente selezionata in elenco

**Svuota** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_svuota_area.bmp](./assets/media/image299.png){width="0.31180555555555556in"
height="0.175in"} ): consente di eliminare in blocco tutte le aree
geografiche associate alla zona in esame

Sulla base di quanto visto fino ad ora, dovrebbe ormai essere chiaro che
la configurazione proposta per le consegne a domicilio offre
all'amministratore del sito la possibilità di definire la zona
geografica entro cui deve ricadere l'indirizzo di spedizione del cliente
per fare in modo che la consegna stessa sia effettivamente selezionabile
all'interno del sito, in due modi diversi:

- A livello di configurazione del metodo di trasporto associato alla
  consegna

- A livello di configurazione della consegna stessa

Nel momento in cui l'esigenza dovesse essere dunque quella di gestire
regole di consegna diverse per diverse aree geografiche si potrebbe
procedere in due modi:

- Creare N metodi di trasporto uguali ma con zone di spedizione diverse
  e associare a ciascuno di essi una "Consegna" valida indipendentemente
  dall'area di spedizione (quindi in "Tutto il mondo") ma con regole
  diverse

- Creare un unico metodo di spedizione valido su più zone geografiche e
  associare ad esso più "Consegne" differenziate non solo per le regole
  di consegna ma anche in base all'area di spedizione

Supponiamo, ad esempio, di dover gestire su Rimini consegne nei giorni
di Lunedì, Mercoledì, Venerdì e su Riccione consegne il Martedì e il
Giovedì. Per soddisfare questo tipo di esigenza potremmo:

- Creare due metodi di spedizioni uguali (di tipo "Consegna a
  domicilio") differenziati in base alle zone di spedizione uno valido
  su Rimini e uno valido su Riccione e due diverse "Consegne" valide
  entrambe in tutto il mondo ma con regole di consegna diverse.

> Al metodo di spedizione valido su Rimini dovrà essere associata la
> consegna nei giorni di Lunedì, Mercoledì e Venerdì mentre alla metodo
> di spedizione valido su Riccione dovrà essere associata la consegna
> nei giorni di Martedì e Giovedì

- Creare un unico metodo di spedizione (di tipo "Consegna a domicilio")
  valido nelle provincie di Rimini e Riccione e assegnare a questo
  stesso metodo due "Consegne" differenziate sia per le regole che per
  le aree di spedizione. Una di queste dovrà quindi essere configurata
  come valida solo per Rimini e con consegne nei giorni di Lunedì,
  Mercoledì e Venerdì mentre l'altra dovrà essere configurata come
  valida solo per Riccione e con consegne nei giorni di Martedì e
  Giovedì

In entrambi i casi nel momento in cui l'utente dovesse indicare in fase
di ordine un indirizzo di spedizione che ricade:

- su Rimini, tra i metodi di spedizione, gli verrà proposta anche la
  consegna a domicilio nei giorni di Lunedì, Mercoledì e Venerdì

- su Riccione, tra i metodi di spedizione, gli verrà proposta anche la
  consegna a domicilio nei giorni di Martedì e Giovedì

- su di una qualsiasi altra area geografica diversa da Rimini e da
  Riccione, la consegna a domicilio non verrà proposta tra i possibili
  metodi di spedizione

Una volta definita la tipologia di consegna a domicilio, lo step
successivo sarà ovviamente quello di impostare per essa l'insieme delle
regole di preparazione e di consegna che andranno poi a definire
esattamente i giorni e gli intervalli orari in cui le consegne potranno
essere effettivamente portate a termine.

Per maggiori informazioni in merito si veda quanto indicato nei
successivi capitoli di questo manuale.

