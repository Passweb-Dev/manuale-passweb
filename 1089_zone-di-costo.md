# ZONE DI COSTO



Come evidenziato all'interno del precedente capitolo **per poter
definire l'esatto importo di un costo di una Spesa Accessoria sarà
necessario codificare e associare al costo stesso almeno una zona di
spedizione.**

**NOTA BENE:** è possibile associare ad ogni costo una o più zone di
spedizione in relazione alle quali poter indicare la modalità di calcolo
del costo stesso (tabellare, fissa o sommatoria) ed i relativi importi.

Considerando poi che, potrebbe configurarsi, la necessità di codificare
la stessa tipologia di calcolo di un costo, e anche gli stessi importi,
per differenti aree geografiche, Passweb offre all'utente la possibilità
di organizzare e raggruppare queste aree in Zone di spedizione distinte.

Per ogni singola Zona di spedizione sarà quindi possibile definire la
tipologia di calcolo del costo in esame con i relativi importi e
associare poi alla zona stessa una o più aree geografiche distinte
selezionando in questo senso la Nazione, la Regione, la Provincia e
anche il singolo C.A.P. che identificano l'area geografica desiderata.

**NOTA BENE:** la selezione della Regione con relative Province e Codici
di Avviamento Postale potrà avvenire solo ed esclusivamente in relazione
alla nazione Italia.

Infine è anche possibile, volendo, escludere determinate aree
geografiche dalla zona di spedizione che si sta configurando.

La tabella \"**Zone di Costo**\" presente all\'interno della maschera
"**Configurazione del Costo**" consente quindi di realizzare quanto
sopra indicato.

![](./assets/media/image433.png)

Per prima cosa sarà quindi necessario creare una nuova "**Zona di
Costo**" in relazione alla quale andranno poi definite le modalità di
calcolo del costo della spesa accessoria oltre, ovviamente, alle varie
aree geografiche da associare alla zona stessa.

**Una volta impostati i parametri di configurazione precedentemente
analizzati, cliccando sul pulsante "Salva" presente nella parte bassa
della maschera verrà automaticamente creata una prima Zona di spedizione
con associata l'area geografica "Tutto il mondo".**

In ogni caso tale Zona potrà sempre essere modificata e/o eliminata
secondo le specifiche esigenze del caso.

I pulsanti presenti nella barra degli strumenti consentono infatti di:

- **Modifica / Elimina Zona**"
  (![](./assets/media/image297.png) )
  (![](./assets/media/image298.png) ): consente di modificare / eliminare la Zona di
  spedizione attualmente selezionata in elenco.

- **Svuota**
  (![](./assets/media/image299.png) ): consente di eliminare in blocco
  tutte le Zone di spedizione presenti in elenco.

- **Aggiungi Zona**
  (![](./assets/media/image300.png) ): consente di creare una nuova Zonda di spedizione

Cliccando su quest'ultimo pulsante verrà infatti aperta la maschera
"**Configurazione Zona**" all'interno della quale poter specificare i
parametri di configurazione della Zona stessa

![](./assets/media/image434.png)

In particolare per ogni singola Zona di spedizione sarà necessario
indicare un valore per i seguenti parametri:

**Nome:** consente di impostare un'etichetta identificativa della Zona
di spedizione che si sta codificando

**Tipo di Spesa:** consente di definire la specifica modalità di calcolo
che dovrà essere utilizzata per il costo associato alla Zona che si sta
codificando. E' possibile selezionare uno tra i seguenti valori:

- **Fissa:** in questo caso verranno considerate, per la zona in
  oggetto, costi accessori **Fissi** il cui importo dovrà essere
  indicato all'interno del successivo campo "**Indicare i parametri di
  Spesa (Valore)**"..

- **Sommatoria:** in queste condizioni, l'importo del costo in oggetto
  verrà determinato moltiplicando per ogni articolo in ordine, la
  quantità di questo stesso articolo per il valore che esso ha in
  relazione all'attributo specificato in corrispondenza dell' omonimo
  parametro "**Attributo**" presente nella configurazione del costo. I
  totali di queste moltiplicazioni verranno poi sommati tra loro ed il
  risultato definitivo determinerà l'importo del costo in oggetto

- **Tabellare:** selezionando questo valore verranno considerate, per la
  zona in oggetto, delle spese di trasporto **Tabellari.** Sarà quindi
  necessario definire i vari scaglioni con i relativi importi da
  applicare

**ATTENZIONE!** per maggiori informazioni in merito alle diverse
tipologie di spesa si vedano anche i successivi capitoli di questo
manuale

Una volta definita la modalità di calcolo da utilizzare per la Zona di
spedizione che si sta codificando, sarà poi necessario, come detto,
associare a questa stessa zona una o più aree geografiche, agendo in
questo senso all'interno della sezione "**Aree di Spedizione**".

![](./assets/media/image302.png)

In questo senso sarà possibile agire in maniera inclusiva, andando
quindi ad includere una ad una tutte le aree geografiche da associare
alla Zona in esame, oppure, volendo sarà possibile operare anche in
maniera esclusiva andando cioè ad escludere dalla Zona in esame
determinate aree geografiche.

**Ovviamente nel momento in cui si dovesse decidere di lavora in maniera
"esclusiva" sarà comunque indispensabile includere nella stessa Zona
almeno un'area geografica valida**

**ATTENZIONE!** Zone di spedizione con sole aree geografiche da
escludere non avrebbero, ovviamente, alcun senso e il relativo costo
accessorio non potrebbe mai essere applicato

In altri termini supponendo, ad esempio, di dover gestire tutta l'Italia
tranne Anacapri, anziché andare ad includere nella nostra Zona di
spedizione uno ad uno tutte le regioni e le provincie gestite potremmo,
in maniera molto più semplice:

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

Per includere o escludere determinate aree geografiche dalla Zona di
spedizione che si sta codificando è sufficiente agire dai relativi
pulsanti presenti nella barra degli strumenti della sezione "Aree di
Spedizione", pulsanti questi che consentono rispettivamente di:

**Italia** (
![](./assets/media/image303.png) ): consente di associare alla zona di
spedizione che si sta codificando una specifica area geografica
all'interno della nazione Italia.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Configurazione Italia**"

![](./assets/media/image304.png)

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa zona
di spedizione:

**ATTENZIONE!** si ricorda che Zone di spedizione con sole aree
geografiche da escludere non avrebbero, ovviamente, alcun senso.

Nel momento in cui si dovesse decidere, dunque, di escludere determinate
aree geografiche da una zona di spedizione sarà di fondamentale
importanza verificare che, per la stessa zona, sia presente, almeno,
anche un' area geografica il cui parametro "**Gestione**" è stato
correttamente impostato su "**Includi**"

**Regione / Provincia / Località / CAP**: consente di specificare la
Regione / Provincia / Località / CAP dell'area geografica che si sta
codificando

Selezionando la regione verrà visualizzata la combo box relativa alle
provincie della regione stessa e, una volta indicata la provincia,
verranno visualizzati il campo relativo alle località e l'area
all'interno della quale poter differenziare ulteriormente in base ai
singoli codici di avviamento postale (**utile soprattutto nel caso in
cui sia necessario gestire i "C.A.P." disagiati**)

![Videate\\configurazione_italia_2.bmp](./assets/media/image305.png)

Per aggiungere un nuovo C.A.P. sarà sufficiente indicarlo all'interno
dell'apposito campo e confermare poi da tastiera con il pulsante
"Invio".

In fase di inserimento dei C.A.P è inoltre possibile utilizzare il
carattere "\_" come wildcard per sostituire uno dei caratteri
effettivamente presenti nel relativo codice di avviamento postale.

**ATTENZIONE!** è fondamentale gestire correttamente il carattere \_
ricordando sempre che **un "underscore" sostituisce un solo carattere**

Supponendo dunque di indicare come C.A.P. il valore "**4_900**" verranno
poi presi in considerazione e validati tutti i codici di avviamento
postale che hanno come primo carattere 4, come secondo carattere un
qualunque valore, come terzo carattere 9, come quarto carattere 0 e come
quindi carattere ancora 0

Supponendo invece di indicare come C.A.P. il valore "**47\_\_\_**" (47
seguito da tre distinti caratteri di underscore), verranno poi presi in
considerazione e validati tutti i codici di avviamento postale che
iniziano con 47 e che proseguono con altri 3 caratteri qualsiasi.

> **NOTA BENE:** la differenziazione per Regione, Provincia e Codice di
> Avviamento Postale può essere effettuata solo ed esclusivamente per la
> nazione Italia.

Il pulsante "**Salva**" presente nella parte bassa della pagina,
consente di salvare l'area geografica codificata accodandola a quelle
già presenti in elenco.

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
![](./assets/media/image306.png) ): consente di associare alla zona di
spedizione che si sta codificando una specifica area geografica
all'interno di una nazione diversa dall'Italia.

Cliccando su questo pulsante verrà visualizzata la maschera
"**Configurazione Paesi Esteri**"

![](./assets/media/image307.png)

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa zona
di spedizione:

**ATTENZIONE!** si ricorda che Zone di spedizione con sole aree
geografiche da escludere non avrebbero, ovviamente, alcun senso

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
![](./assets/media/image308.png) ): consente di associare all'Area di
spedizione che si sta codificando una zona geografica relativa ad una
Nazione diversa dall'Italia.

Cliccando su questo pulsante verrà visualizzata la maschera
"**Configurazione Nazioni**"

![](./assets/media/image309.png)

all'interno della quale sarà necessario indicare un valore per i
seguenti parametri:

**Gestione**: consente di decidere se l'area geografica che si sta
codificando dovrà essere **inclusa** o **esclusa** dalla relativa zona
di spedizione:

**ATTENZIONE!** si ricorda che Zone di spedizione con sole aree
geografiche da escludere non avrebbero, ovviamente, alcun senso

Nel momento in cui si dovesse decidere, dunque, di escludere determinate
aree geografiche da una zona di spedizione sarà di fondamentale
importanza verificare che, per la stessa zona, sia presente, almeno,
anche un' area geografica il cui parametro "**Gestione**" è stato
correttamente impostato su "**Includi**"

**Nazioni:** consente di indicare l'elenco delle Nazioni che devono
essere associate alla zona di spedizione che si sta codificando

Per associare alla zona di spedizione una specifica Nazione, è
sufficiente selezionarla dall'elenco di sinistra ed inserirla in quello
di destra cliccando sul pulsante raffigurante una piccola freccia verde.
Allo stesso modo per eliminare l'associazione tra le zona di spedizione
in esame ed una specifica Nazione, sarà sufficiente selezionarla
dall'elenco di destra e cliccare poi sul pulsante raffigurante una
piccola freccia rossa.

**Importa da file** ( ): consente di definire le varie aree geografiche
da associare alla zona di spedizione in esame importandole in blocco da
un file di tipo txt o csv appositamente formattato.

Cliccando su questo pulsante verrà visualizzata la maschera
"**Importazione Aree da File**"

![](./assets/media/image435.png)

all'interno della quale poter selezionare (campo **File**), importandolo
ad esempio dal proprio pc, il file .txt o .csv con indicate tutte le
aree geografiche da associare alla zona in esame.

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
> zona di spedizione

- **nazione**: codice iso a 2 caratteri della nazione

- **provincia**: sigla della provincia

- **localita**: nome della localita

- **cap**: codice di avviamento postale della localita (con possibilità
  di utilizzare il carattere "\_" come carattere wildcard)

- **km**: campo numerico con due decimali. Distanza massima (in
  chilometri) tra l'indirizzo di spedizione merce indicato dall'utente
  in fase di checkout ed eventuali punti vendita associati al metodo di
  trasporto, affinché questi stessi punti vendita possano essere
  ritenuti "validi" per la spedizione.

> **ATTENZIONE**! il campo km è gestito unicamente per Spedizioni in cui
> è attiva la gestione dei Punti Vendita

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

FR;;;

IT;SA;;

IT;RN;;47900

IT;RN;Viserba;47922

IT;RN;Viserbella;

Nelle condizioni sopra indicate verrebbero quindi aggiunte alla zona di
spedizione in esame 5 distinte aree geografiche: la prima relativa alla
nazione Francia, la seconda relativa all'area geografica corrispondente
alla provincia di Salerno in Italia, la terza relativa alla provincia di
Rimini e nello specifico al codice di avviamento postale 47900, la
quarta sempre relativa alla provincia di rimini ma più specificatamente
alla località Viserba e al codice di avviamento postale 47922 e la
quinta relativa alla provincia di rimini e nello specifico alla località
Viserbella.

> **NOTA BENE:** nel caso di "Importazione da file" non verranno
> effettuati controlli di alcun tipo relativamente alle aree geografiche
> eventualmente già associate alla zona in esame. Occorre quindi fare
> particolare attenzioni, in queste condizioni, a non inserire delle
> aree geografiche doppie o triple.

**Esporta** (
![](./assets/media/image311.png) ): consente di esportare all'interno di
un file csv, nello stesso formato valido anche per l'importazione,
l'elenco di tutte le aree geografiche attualmente associate alla zona di
spedizione in esame.

Cliccando su questo pulsante verrà infatti visualizzata un'ulteriore
sezione "**Esportazione Aree**"

![](./assets/media/image312.png)

all'interno della quale poter indicare il carattere separatore che dovrà
essere utilizzato in fase di creazione del file csv.

Il pulsante "**Salva**" presente nella parte bassa della maschera
consente di avviare la procedura di esportazione

**Elimina Area** (
![](./assets/media/image313.png) ): consente di eliminare l'area geografica
attualmente selezionata in elenco

**Svuota** ( ): consente di eliminare in blocco tutte le aree
geografiche associate alla zona di spedizione in esame

Il pulsante "**Salva**" presente nella parte bassa della maschera
"Configurazione del Costo" consente di salvare il Costo appena
configurato.

##### COSTI FISSI

Nel momento in cui l'esigenza dovesse essere quella di utilizzare per
una determinata zona geografica dei costi fissi, sarà necessario
impostare, per prima cosa, nella maschera di configurazione della Zona,
il parametro "**Tipo Spesa**" sul valore "**Fissa**" e successivamente
indicare l'esatto importo da applicare all'interno del campo
"**Valore**"

![](./assets/media/image314.png)

**Valore** consente di definire l'importo da applicare al costo
accessorio in oggetto, nel caso in cui l'indirizzo di spedizione della
merce rientri in una delle aree geografiche associate alla zona che si
sta codificando. Sono accettati i seguenti valori:

- **Valori numerici positivi -- es. "20":** supponendo dunque di
  inserire all'interno del campo in esame il valore 20, nel caso in cui
  l'indirizzo di spedizione della merce rientri in una delle aree
  geografiche associate alla zona che si sta codificando, l'importo da
  considerare per il costo accessorio in oggetto sarà di 20 €

- **Valori numerici negativi -- es. "-20":** supponendo dunque di
  inserire all'interno del campo in esame il valore -20 nel caso in cui
  l'indirizzo di spedizione della merce rientri in una delle aree
  geografiche associate alla zona che si sta codificando l'importo da
  considerare per il costo accessorio in oggetto sarà di -20 €.

> **In queste condizioni dunque il costo accessorio non aumenterà il
> totale del documento ma, al contrario, andrà ad abbattere tale
> importo.**

- **Valori percentuali positivi -- es. "20%":** supponendo dunque di
  inserire all'interno del campo in esame il valore 20%, nel caso in cui
  l'indirizzo di spedizione della merce rientri in una delle aree
  geografiche associate alla zona che si sta codificando, l'importo da
  considerare per il costo accessorio in oggetto sarà pari al 20% del
  Totale Merce o dell'Imponibile dipendentemente da quanto impostato per
  il parametro **"Scaglioni e Calcolo Percentuale**" presente nella
  maschera di configurazione del costo accessorio precedentemente
  esaminata

> Inoltre il Totale Merce così come l'Imponibile, utilizzato come base
> di calcolo, verrà considerato comprensivo o meno di eventuali articoli
> spesa aggiunti in carrello a seguito dell'applicazione di determinate
> promozioni o buoni sconto, dipendentemente dall'impostazione scelta
> per il parametro "**Gestione Totale Merce**" presente nella sezione
> "*Catalogo -- Configurazione Parametri Catalogo*" del Wizard

- **Valori percentuali negativi -- es. "-20%":** anche in questo caso
  l'importo da considerare per il costo accessorio verrà calcolato come
  percentuale del Totale Merce o dell'Imponibile dipendentemente da
  quanto impostato per il parametro **"Scaglioni e Calcolo
  Percentuale**" presente nella maschera di configurazione del costo
  stesso.

> Trattandosi inoltre di valori negativi, anche in queste condizioni il
> costo accessorio non aumenterà il totale del documento ma, al
> contrario andrà ad abbattere tale importo.

**In ogni caso l'importo presente all'interno del campo Valore o quello
risultante dalla percentuale indicata sarà sempre considerato
comprensivo di IVA (l'eventuale aliquota considerata sarà quella
indicata all'interno del gestionale per l'articolo di tipo S utilizzato
per gestire la corrispondente spesa accessoria)**

Supponendo dunque che quello in oggetto sia l'unico costo che concorre a
determinare il valore della spesa accessoria, occorre allora considerare
che:

- per quel che riguarda gli OX nel piede del documento comparirà la voce
  "Spese Accessorie" con l'esatto importo indicato all'interno di questo
  campo

- per quel che riguarda gli OC nel piede del documento comparirà la voce
  "Spese Accessorie" con l'importo indicato all'interno di questo campo
  scorporato dell'IVA, IVA questa che verrà aggiunta alla corrispondente
  voce presente anch'essa nel piede del documento.

##### COSTI CON SOMMATORIA

Nel momento in cui l'esigenza dovesse essere quella di calcolare per una
determinata zona geografica dei costi accessori in maniera più dinamica,
potrebbe essere necessario impostare, nella maschera di configurazione
della Zona, il parametro "**Tipo Spesa**" sul valore "**Sommatoria**"

![](./assets/media/image317.png)

In queste condizioni, l'importo del costo in oggetto verrà determinato
moltiplicando per ogni articolo in ordine, la quantità di questo stesso
articolo per il valore che esso ha in relazione all'attributo
specificato in corrispondenza dell' omonimo parametro "**Attributo**"
presente nella configurazione del costo.

I totali di queste moltiplicazioni verranno poi sommati tra loro ed il
risultato definitivo determinerà l'importo del costo in oggetto

L'importo ottenuto verrà espresso nella valuta indicata in fase di
configurazione del costo (campo "**Valuta di riferimento**"). Nel caso
in cui l'ordine effettuato dall'utente faccia riferimento ad un\'altra
valuta l'importo verrà convertito nella valuta di destinazione.

**ESEMPIO**

Supponiamo di aver codificato un attributo articolo chiamato "Valore
Costo Accessorio" e di aver indicato, in fase di configurazione del
costo all'interno del campo "Attributo", proprio l'attributo appena
considerato

Supponiamo inoltre di aver impostato per i due articoli LETTDVD1 e
LETTDVD2 tale attributo sui valori:

**LETTDVD1 🡪 Valore Costo Accessorio** = 5**;**

**LETTDVD2 🡪 Valore Costo Accessorio** = **10;**

Supponiamo inoltre di aver attivato in Passweb una spesa accessoria con
associato un costo per il quale è stata definita una zona di spedizione
merce con campo "**Tipo** **Spesa**" impostato sul valore
"**Sommatoria**"

In queste condizioni dunque nel caso in cui venga fatto un ordine con i
due articoli:

**LETTDVD1 in quantità 2;**

**LETTDVD2 in quantità 3;**

venga selezionata la spesa accessoria in oggetto e l'indirizzo di
spedizione merce appartenga alla zona appena considerata, i due articoli
in ordine contribuiranno alla determinazione della spesa accessoria in
questo modo:

(2 x 5)+(3 x 10) = 40

Il costo con cui questi due articoli concorreranno al valore complessivo
della spesa accessoria sarà quindi di 40 euro (ipotizzando anche di aver
utilizzato come valuta di riferimento per questa spese accessoria
l'euro)

##### COSTI TABELLARI

Nel momento in cui l'esigenza dovesse essere quella di utilizzare per
una determinata zona geografica dei costi accessori che consentano di
applicare diversi valori a seconda di determinati scaglioni, sarà
necessario impostare, nella maschera di configurazione della Zona, il
parametro "**Tipo Spesa**" sul valore "**Tabellare**"

In queste condizioni verrà infatti visualizzata la tabella qui di
seguito riportata

![](./assets/media/image318.png)

attraverso la quale poter definire i vari scaglioni, ed il relativo
importo, che verranno poi considerati per determinare il valore del
costo in esame nel caso in cui l'indirizzo di spedizione della merce
rientri in una delle aree geografiche associate alla zona di spedizione
che si sta codificando.

Per poter definire questi scaglioni occorrerà quindi indicare uno
specifico valore per i seguenti campi:

**Fino a:** valore numerico che definisce il limite del corrispondente
scaglione. L'unità di misura dello scaglione è determinata sulla base di
quanto impostato all'interno del campo "Scaglioni e Calcolo Percentuale"
presente nella maschera di configurazione del costo precedentemente
esaminata.

Dipendentemente dunque da quanto impostato per questo parametro il
valore indicato nel campo "Fino a" potrà fare riferimento al Totale
Merce, all'Imponibile, al Numero Articolo o a uno specifico campo
personalizzato (quello indicato all'interno del campo "Attributo").

**Valore:** importo del costo relativo al corrispondente scaglione. In
particolare all'interno di questo campo è possibile indicare:

- **L'esatto importo (valore numerico) da considerare per lo scaglione
  in oggetto oppure un valore in percentuale (valore numerico seguito
  dal simbolo %).**

> In quest'ultimo caso la percentuale indicata verrà calcolata sul
> Totale Merce o sull'Imponibile dipendentemente da quanto impostato per
> il parametro "Scaglioni e Calcolo Percentuale" presente nella maschera
> di configurazione del costo precedentemente esaminata.
>
> Inoltre il Totale Merce così come l'Imponibile, utilizzato come base
> di calcolo, verrà considerato comprensivo o meno di eventuali articoli
> spesa aggiunti in carrello a seguito dell'applicazione di determinate
> promozioni o buoni sconto, dipendentemente dall'impostazione scelta
> per il parametro "**Gestione Totale Merce**" presente nella sezione
> "*Catalogo -- Configurazione Parametri Catalogo*" del Wizard
>
> **In ogni caso l'esatto valore presente all'interno di questo campo o
> quello risultante dalla percentuale indicata sarà sempre considerato
> comprensivo di IVA (l'eventuale aliquota considerata sarà quella
> indicata all'interno del gestionale per l'articolo di tipo S
> utilizzato per gestire la corrispondente spesa accessoria**
>
> Anche in questo caso occorre dunque considerare che:

- per quel che riguarda gli OX nel piede del documento comparirà la voce
  "Spese Accessorie" con l'esatto importo indicato all'interno di questo
  campo

- per quel che riguarda gli OC nel piede del documento comparirà la voce
  "Spese Accessorie" con l'importo indicato all'interno di questo campo
  scorporato dell'IVA, IVA questa che verrà aggiunta alla corrispondente
  voce presente anch'essa nel piede del documento.

> **Come per le spese fisse, anche in questo caso sono accettati sia
> valori positivi che valori negativi (sia fissi che in percentuale)**.
>
> Ovviamente, anche in queste condizioni, utilizzando valori negativi il
> costo accessorio non aumenterà il totale del documento ma, al
> contrario andrà ad abbattere tale importo.

- **Il carattere \#**. In questo caso, nel momento in cui le condizioni
  d'ordine dovessero essere tali da far ricadere il costo accessorio
  all'interno di questo scaglione, questo non verrà considerato.

> **L'utilizzo del carattere \# consente quindi di considerare un
> determinato costo accessorio solo ed esclusivamente nel momento in cui
> si rientri all'interno di determinati scaglioni**.

- **Formula:** è possibile definire esattamente la formula da utilizzare
  per determinare il valore del costo accessorio che dovrà essere
  applicato nel momento in cui le condizioni d'ordine dovessero essere
  tali da far ricadere il costo stesso all'interno dello scaglione in
  esame.

> Nella definizione della formula è possibile utilizzare:

- **gli operatori standard (+-\*/)**

- **elevatore a potenza (\^).--** Es 2\^3

- **radice quadrata (sqrt) --** Es. sqrt(16)

- **modulo (%) --** Es. 10%3 🡪 consente di dividere il primo argomento
  per il secondo, restituendo solo il resto.

- **valore assoluto (abs)**

- **valore intero (int) --** Es int(5.2) 🡪 5

- **valore intero superiore (ceiling) --** Es ceiling(5.2) 🡪 6

- **parentesi tonde**

- **la variabile x che rappresenta l'esatto valore del misuratore
  (prezzo, numero articoli o campo personalizzato) che ha fatto ricadere
  il costo accessorio nello specifico scaglione**

- **la variabile y che rappresenta il valore del Totale Merce NON
  ivato**

- **la variabile z che rappresenta il valore del Totale Merce Ivato**

> **ATTENZIONE!** Nel caso in cui dovessero essere inseriti nella
> formula dei valori decimali il carattere di separazione tra i valori
> interi e quelli decimali dovrà essere il "."

Ovviamente nel caso di ordini con spese accessorie determinate sulla
base di costi di tipo tabellare, nel caso in cui vengano apportate
modifiche a questi stessi ordini tali spese verranno opportunamente
ricalcolate tenendo conto, eventualmente, anche della zona di spedizione
merce

**ESEMPIO**

Nel caso in cui venga utilizzato come base di calcolo per gli scaglioni
del costo tabellare un campo personalizzato (nello specifico quello
indicato all'interno del campo "Attributo" presente nella maschera di
configurazione del costo), il passaggio da uno scaglione ad un altro e
conseguentemente l'applicazione di uno specifico importo per il costo in
esame, dipenderà dal numero di articoli presenti in ordine e dal valore
che questo campo personalizzato ha per ciascuno di questi stessi
articoli.

Supponiamo dunque di aver codificato un attributo articolo chiamato, ad
esempio, "**Misuratore Costo Accessorio**" e di aver indicato, in fase
di configurazione del costo all'interno del campo "**Attributo**",
proprio l'attributo appena considerato.

Supponiamo anche di aver impostato per i due articoli LETTDVD1 e
LETTDVD2 tale attributo sui valori:

**LETTDVD1 🡪 Misuratore Costo Accessorio = 11;**

**LETTDVD2 🡪 Misuratore Costo Accessorio = 12;**

Supponiamo inoltre di aver attivato in Passweb una spesa accessoria con
associato un costo per il quale è stata definita una zona di spedizione
merce con campo "**Tipo** **Spesa**" impostato sul valore
"**Tabellare**" e con i seguenti scaglioni:

- **Fino a: 200 Valore: 20**

- **Fino a 500 Valore: 10**

- **Oltre Valore: 5**

In queste condizioni dunque nel caso in cui venga fatto un ordine con i
due articoli:

**LETTDVD1 in quantità 2;**

**LETTDVD2 in quantità 10;**

venga selezionata la spesa accessoria in oggetto e l'indirizzo di
spedizione merce appartenga alla zona appena considerata, per ottenere
l\'importo del costo in questione verrà effettuato il seguente calcolo:

(11x2)+(12x10) = 142

Il risultato ottenuto rientra nel primo scaglione (fino a 200) e quindi
il valore del costo che verrà utilizzato, in queste condizioni, per
determinare il valore complessivo della corrispondente spesa accessoria
sarà esattamente 20 € (ipotizzando ovviamente di aver utilizzato come
valuta di riferimento per la corrispondente spesa accessoria proprio
l'euro).

I pulsanti "**Importa da file**" e "**Esporta**" consentono infine di
popolare in maniera massiva, mediante import di appositi file csv, la
tabella dei diversi scaglioni.

Nello specifico cliccando sul pulsante "**Importa da File**" verrà
visualizzata la maschera "**Importazione Scaglioni da file**"

![](./assets/media/image319.png)

all'interno della quale poter indicare:

- **File (csv-txt)**: consente di selezionare il file txt o csv
  contenente l'elenco dei valori da utilizzare per definire i vari
  scaglioni e i relativi importi da applicare

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di importazione possa funzionare in maniera
corretta è necessario, ovviamente, che il file in oggetto soddisfi
determinate specifiche. In particolare:

- Il file dovrà avere estensione .csv o .txt

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione

- L'intestazione, ossia la prima riga del file, deve contenere **i campi
  di seguito indicati nell'ordine indicato e con le diciture indicate**:
  fino A, Valore

> Considerata l'intestazione del file, ogni suo record dovrà ovviamente
> contenere le seguenti informazioni:

- **fino A:** valore di definizione del relativo scaglione

- **Valore:** importo da applicare in corrispondenza del relativo
  scaglione

<!-- -->

- L'importo da utilizzare in corrispondenza dello scaglione "**Oltre**"
  sarà quello inserito, all'interno del file di importazione, sulla riga
  in cui è stato indicato il numero 0 in corrispondenza della colonna
  "Fino A"

In definitiva dunque, supponendo di voler utilizzare come carattere
separatore il ; il file da importare dovrà avere una struttura del tipo
di quella indicata

**fino A;Valore**

**10;20**

**20;40**

**30;60**

**40;80**

**0;100**

Cliccando invece sul pulsante "Esporta" verrà visualizzata la maschera
"**Esportazione Scaglioni**"

![](./assets/media/image320.png)

all'interno della quale poter avviare la procedura di esportazioni, in
un apposito file csv con il carattere separatore indicato in
corrispondenza del relativo parametro, degli scaglioni attualmente
codificati per la zona geografica in esame.

**ATTENZIONE!** E' possibile, ovviamente, effettuare l'esportazione dei
soli scaglioni già salvati

Nel momento in cui si dovesse, dunque, compilare manualmente la tabella
degli scaglioni e si dovesse tentare poi di effettuare un'esportazione
di questi valori senza aver prima cliccato sul pulsante "Salva" il file
di esportazione generato potrà essere vuoto oppure potrà contenere i
valori precedentemente salvati per i relativi scaglioni.

