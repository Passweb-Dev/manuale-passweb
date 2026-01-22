# CREAZIONE DI UNA NUOVA INSERZIONE



Dopo aver correttamente configurato l'integrazione Passweb -- Amazon, ed
aver abilitato almeno un Marketplace, il passo successivo dovrà quindi
essere quello di creare un' Inserzione da poter poi utilizzare per
mettere effettivamente in vendita alcuni articoli del proprio sito web
sul marketplace definito all'interno dell'Inserzione stessa.

Portandosi quindi nella sezione "*Catalogo -- Amazon -- Gestione
Inserzioni*" del Wizard verrà visualizzata la maschera "**Lista delle
Inserzioni Amazon**"

![](./assets/media/image201.png)

all'interno della quale verranno visualizzate tutte le Inserzioni
attualmente configurate.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![](./assets/media/image69.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![](./assets/media/image70.png) )

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Elimina Inserzione** (
  ![](./assets/media/image202.png) ): consente di eliminare l'inserzione attualmente
  selezionata in elenco.

**NOTA BENE:** eliminando un'inserzione verranno eliminate anche tutte
le liste di articoli ad essa collegate. Gli articoli già messi in
vendita all'interno di un Marketplace Amazon, attraverso una lista
eliminata automaticamente a seguito della cancellazione di un'
Inserzione, continueranno comunque a vivere come entità a se stanti
all'interno del corrispondente sito Amazon

- **Modifica Inserzione** (
  ![](./assets/media/image203.png) ): consente di accedere alla maschera
  di configurazione dell'Inserzione attualmente selezionata in maniera
  tale da poterne gestire le singole regole di vendita.

- **Copia Inserzione** (
  ![](./assets/media/image72.png) ): consente di copiare l' Inserzione
  attualmente selezionata in elenco (verrà creata una nuova inserzione
  con le stesse esatte regole di gestione definite sull' Inserzione
  sorgente).

- **Aggiungi Inserzione** (
  ![](./assets/media/image73.png) ): consente di codificare una nuova Inserzione.

Cliccando su quest'ultimo pulsante verrà infatti visualizzata la
maschera "**Dati Inserzione**"

![](./assets/media/image204.png)

attraverso cui poter definire le specifiche regole di vendita che
andranno a caratterizzare l'Inserzione stessa.

In questo senso la sezione **"Impostazioni Generali"** consente di
definire le caratteristiche generali dell'Inserzione. Nello specifico il
campo:

- **Nome:** consente di assegnare un nome alla nuova inserzione in
  maniera tale da poterla poi identificare, tra tutte quelle codificate,
  nelle successive fasi di pubblicazione degli articoli.

- **Account Amazon:** consente di indicare lo specifico Account che
  verrà utilizzato nel momento in cui, in fase di pubblicazione degli
  articoli su Amazon, dovesse essere selezionata l'Inserzione in esame.

> E' possibile selezionare uno degli Account precedentemente configurati
> all'interno della corrispondente sezione "Gestione Account" e per i
> quali è stata quindi concessa allo sviluppatore "Passepartout"
> l'autorizzazione ad utilizzare l'Account stesso per pubblicare
> articoli sui Marketplace Amazon.

- **Sito Amazon:** consente di indicare lo specifico Marketplace da
  associare all' Inserzione che si sta realizzando.

> E' possibile selezionare solo ed esclusivamente uno dei marketplace
> precedentemente abilitati all'interno della corrispondente sezione
> "Marketplace".
>
> **ATTENZIONE!** Nel caso in cui per il marketplace selezionato non
> siano ancora state caricate in Passweb le relative categorie
> merceologiche (tra il momento di attivazione del marketplace e il
> caricamento delle relative categorie merceologiche potrebbero passare
> del tempo) verrà visualizzato un apposito messaggio.

- **Valuta:** consente di specificare la valuta da utilizzare per gli
  articoli messi in vendita attraverso questa inserzione.

> **ATTENZIONE!** Le valute utilizzabili su di un certo marketplace
> dipendono direttamente dallo specifico marketplace selezionato

Relativamente alla selezione della Valuta il comportamento
dell'applicazione sarà differente a seconda del fatto di considerare un
sito Ecommerce collegato a Mexal oppure ad uno dei gestionali Ho.Re.Ca.

**[ECOMMERCE MEXAL]{.underline}**

Nel caso di siti Ecommerce collegati a Mexal è possibile sfruttare la
Tabella Valute del gestionale con relative conversioni pubblicando
articoli, quindi, anche su marketplace che accettano solo valute diverse
dall'euro.

Se l'esigenza dovesse quindi essere, ad esempio, quella di mettere in
vendita articoli sul marketplace Inglese, che accetta come valuta oltre
all' Euro anche la Sterlina, sarà necessario per prima cosa gestire tale
valuta in Mexal.

Successivamente sarà poi necessario attivare all'interno del proprio
sito Passweb il paese **"United Kingdom"** in maniera tale da poter
gestire la sterlina anche sul sito Ecommerce.

La conversione tra i prezzi in euro del listino associato alla specifica
inserzione e quelli in sterline verrà poi effettuata in automatico
dall'applicazione utilizzando i fattori di conversione definiti nella
relativa tabella gestionale.

**ATTENZIONE! Nel caso in cui non dovesse essere gestita in Mexal la
valuta utilizzata da uno specifico marketplace Amazon non sarà poi
possibile configurare Inserzioni per quello specifico marketplace.**

**[ECOMMERCE HO.RE.CA]{.underline}**

Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca. non
essendo presente all'interno del gestionale una Tabella Valute con
relativi fattori di conversione sarà possibile configurare delle
inserzioni solo ed esclusivamente su quei marketplace che accettano
l'euro come valuta di gestione.

**ATTENZIONE:** **la scelta del marketplace cui associare un' Inserzione
è di fondamentale importanza non solo perché gli articoli messi in
vendita su Amazon attraverso apposite liste collegate a questa
Inserzione saranno poi disponibili solo ed esclusivamente nel
corrispondente Marketplace, ma anche perché le successive regole che
occorrerà definire per completare l'Inserzione potranno variare proprio
in conseguenza dello specifico marketplace selezionato.**

Selezionando infatti uno dei marketplace disponibili, oltre alla valuta
di gestione, verranno abilitate anche le ulteriori sezioni presenti
nella parte bassa della maschera di configurazione, sezioni queste
all'interno delle quali indicare:

![](./assets/media/image205.png)

- **Categoria:** consente di impostare le informazioni relative alla
  specifica Categoria Merceologica e alla Tipologia di prodotti che
  verranno messi in vendita attraverso l'inserzione che si sta
  codificando.

> **ATTENZIONE! Affinchè la pubblicazione degli articoli possa andare a
> buon fine è necessario indicare una Tipologia di Prodotto coerente con
> la Categoria Merceologica selezionata**

- **Descrizione:** consente di impostare le condizioni di vendita dei
  prodotti esportati sul marketplace collegato all'inserzione che si sta
  codificando oltre ai cosiddetti "Identificativi del Catalogo Amazon"
  ossia i codici (UPC, EAN, ISBN) utilizzati per identificare
  univocamente i vari articoli all'interno del Marketplace Amazon

- **Pagamento:** consente di impostare le modalità di pagamento
  selezionabili per gli articoli messi in vendita mediante l'Inserzione
  che si sta codificando

- **Spedizione:** consente di impostare le modalità di spedizione della
  merce relative agli articoli messi in vendita mediante l'Inserzione
  che si sta codificando

- **Prezzo, quantità e formato:** consente di definire i prezzi degli
  articoli messi in vendita mediante l'Inserzione che si sta codificando

- **Sincronizzazione:** consente di attivare determinate regole grazie
  alle quali poter abilitare / disabilitare, in maniera del tutto
  automatica, la messa in vendita, la rimessa in vendita e il blocco
  della vendita sul Marketplace degli articoli gestiti tramite
  l'Inserzione che si sta codificando.

Per maggiori informazioni relativamente a ciascuna delle sezioni sopra
indicate si vedano i successivi capitoli di questo manuale

##### CATEGORIA

All'interno di questa sezione è necessario definire, innanzitutto, la
Categoria Merceologica cui verranno associati, sullo specifico
Marketplace Amazon, gli articoli messi in vendita tramite l'Inserzione
che si sta considerando.

Per associare all'Inserzione una specifica categoria merceologica è
sufficiente cliccare sul pulsante "**Cambia Categoria**" presente
all'interno della sezione "**Categoria**" e selezionare poi quella
desiderata dal relativo menu a tendina.

![](./assets/media/image206.png)

Dipendentemente dalla Categoria Merceologia indicata potrà poi essere
possibile selezionare anche una o più sottocategorie

**ATTENZIONE!** Le categorie e sotto categorie merceologiche
selezionabili dipendono direttamente dallo specifico marketplace e non
possono dunque essere personalizzate in alcun modo. La descrizione di
tali categorie sarà poi in italiano o in lingua dipendentemente, anche
in questo caso, dal marketplace considerato.

A differenza di quanto avviene per eBay, nel caso di Amazon è
indispensabile indicare, oltre alla Categoria Merceologica anche la
**Tipologia di Prodotto**, selezionandola, anche in questo caso, dal
relativo menu a tendina

![](./assets/media/image207.png)

**ATTENZIONE! La tipologia di prodotto, così come la Categoria
Merceologica è un dato obbligatorio, in assenza del quale non sarà
possibile salvare la relativa Inserzione**

**La Tipologia di prodotto selezionata dovrà inoltre essere coerente con
la Categoria Merceologica indicata** all'interno del precedente campo.
Se ciò non dovesse avvenire non sarà poi possibile pubblicare articoli
mediante l'Inserzione che si sta realizzando.

**ATTENZIONE! Amazon, in questo senso, non fornisce una esatta
corrispondenza tra le diverse Categorie Merceologiche e le
corrispondenti Tipologie di Prodotto per cui non è possibile, data la
Categoria Merceologica, selezionare automaticamente la corretta
Tipologia di Prodotto.**

In ogni caso nel momento in cui la Tipologia di prodotto selezionata non
dovesse essere corretta, in relazione alla Categoria Merceologica
indicata, quando si andrà poi a pubblicare gli articoli sul Marketplace
di Amazon verrà ritornato un messaggio di errore in cui verranno forniti
anche dei suggerimenti relativamente alle possibili Tipologie di
prodotto da selezionare per poter portare a termine correttamente la
pubblicazione degli articoli.

Una volta selezionata la Tipologia di Prodotto verranno poi visualizzati
all'interno della successiva sezione "**Specifiche**" tutti i campi
obbligatori da poter utilizzare per pubblicare informazioni aggiuntive
sugli articoli messi in vendita, informazioni queste che potranno poi
essere visualizzate sul marketplace Amazon nella scheda prodotto dei
vari articoli.

**ATTENZIONE!** Le specifiche obbligatorie per poter completare
correttamente l'Inserzione sono indicate da un piccolo asterisco rosso
posto immediatamente a fianco del nome.

![](./assets/media/image208.png)

Volendo è anche possibile aggiungere ulteriori specifiche, non
obbligatorie, al fine di dettagliare maggiormente le informazioni
relative agli articoli pubblicati.

Per far questo è necessario:

- cliccare sul pulsante "**Aggiungi Specifiche**" in maniera tale da
  visualizzare un elenco di tutte le specifiche gestibili in relazione
  alla Categoria Merceologica in cui si sta operando:

![](./assets/media/image209.png)

- selezionare le specifiche desiderate dall'elenco di sinistra ed
  inserirle in quello di destra cliccando per questo sul pulsante
  "**Seleziona**"

- Cliccare sul pulsante "**Conferma**"

**ATTENZIONE!** **Relativamente alle informazioni pubblicate e
visualizzate per ogni singolo prodotto va detto che Amazon si comporta
diversamente da eBay.**

Nel caso in cui il prodotto da mettere in vendita mediante l'inserzione
di Passweb dovesse essere già presente sul Marketplace Amazon, in fase
di pubblicazione non verrà mai creata una nuova scheda prodotto ma
Amazon stessa cercherà di agganciare il prodotto Passweb all'articolo
già presente sul Marketplace verificando che tutti i dati passati siano
effettivamente quelli corretti e necessari per effettuare l'aggancio
(stesso ASIN, stesso codice EAN, stesso titolo ...).

**In sostanza dunque sarà Amazon, sulla base dei suoi criteri interni di
gestione a decidere se il prodotto pubblicato contiene tutte le
informazioni corrette per poter effettuare l'aggancio**, così come sarà
Amazon stessa a decidere se il nostro prodotto dovrà comparire
direttamente nella **"Buy Box"**, nel riquadro **"Confronta offerte su
Amazon"** oppure solamente **nell'elenco delle offerte effettuate da
tutti gli altri venditori** di quello stesso articolo.

Per maggiori informazioni in merito in merito alla gestione della Buy
Box e ai criteri di pubblicazione di Amazon si veda anche il successivo
capitolo "*Amazon **--** La scheda prodotto e la Buy Box*" di questo
manuale oppure si consulti la relativa documentazione accessibile
direttamente sulla Seller Central dal Back End del proprio Account
Venditore.

Nel caso in cui alcune delle specifiche obbligatorie non siano state
compilate al salvataggio dell'Inserzione verrà visualizzato un apposito
messaggio di errore

Ogni specifica potrà avere diverse proprietà e ogni proprietà dovrà
assumere un determinato valore. Nel caso evidenziato in figura, ad
esempio, la specifica "Disco Rigido" avrà le proprietà:

- Descrizione del disco rigido

- Interfaccia del disco rigido

- Velocità del disco rigido

- ...

![](./assets/media/image210.png)

Per definire il valore che dovrà assumere una certa proprietà è
necessario, innanzitutto, indicare da dove poter andare a prelevare
questo valore selezionando, per questo, una delle opzioni disponibili
all'interno del relativo menu a tendina.

![](./assets/media/image211.png)

Nello specifico è possibile selezionare una delle seguenti opzioni:

- **Nessuno:** selezionando questa opzione la specifica corrispondente
  non verrà valorizzata e, conseguentemente, all'interno della scheda
  prodotto di Amazon non verrà visualizzata, in relazione a questa
  specifica, nessuna informazione aggiuntiva.

- **Attributo Amazon:** in questo caso sarà possibile indicare il valore
  da utilizzare per la corrispondente specifica selezionandolo, se
  possibile, tra quelli messi a disposizione direttamente da Amazon
  oppure digitandolo direttamente all'interno del campo **Valore**

- **Attributo Passweb:** in questo caso sarà possibile indicare il
  valore da utilizzare per la corrispondente specifica, selezionandolo
  tra gli attributi articolo attualmente mappati all'interno di Passweb
  (campo **Valore**).

- **Personalizzato:** in questo caso sarà possibile indicare
  esplicitamente il valore che dovrà assumere all'interno di Amazon la
  corrispondente specifica (campo **Valore**).

- **Elemento di Variazione:** necessario per inserzioni adibite ad
  accogliere articoli con elementi Varianti (es. taglie colori) consente
  di indicare come dovrà essere gestito il corrispondente elemento di
  Variazione.

> Per maggiori informazioni in merito alla possibilità di pubblicare
> sulla piattaforma terza articoli a taglie / colori si veda anche il
> relativo capitolo di questo manuale (*Amazon -- Articoli a Taglie e
> Colori*)

Nel caso in cui per una determinata specifica dovesse essere possibile
aggiungere più volte la stessa proprietà, comparirà a fianco del nome
della specifica un piccolo più che se cliccato inserirà la proprietà in
esame all'interno della relativa specifica

![](./assets/media/image212.png)

**ATTENZIONE!** **Tutti gli articoli messi in vendita attraverso una
certa Inserzione, oltre ad avere le stesse modalità di gestione,
visualizzeranno nelle loro schede prodotto anche le stesse specifiche (e
quindi potenzialmente gli stessi valori).**

In questo senso le uniche informazioni dinamiche, che potranno quindi
variare da articolo ad articolo anche all'interno della stessa
Inserzione, sono quelle gestite mediante gli Attributi Articolo definiti
in Passweb.

**In sostanza dunque mappando una certa specifica con un Attributo
Amazon o con un campo Personalizzato poi tutti gli articoli messi in
vendita mediante l'Inserzione in esame avranno, per la stessa specifica,
lo stesso esatto valore.**

**Nel caso in cui invece la specifica sia stata mappata con un Attributo
Passweb, essendo il valore di questi attributi diverso articolo per
articolo, anche prodotti messi in vendita tramite la stessa Inserzione
potranno visualizzare, nella relativa scheda prodotto di Amazon, per la
stessa specifica informazioni differenti.**

**ATTENZIONE!** Non è detto che la scheda prodotto presente in Amazon
visualizzi esattamente le informazioni inserite lato Passweb. Per
maggiori informazioni in merito si veda anche il successivo capitolo
"*Amazon -- La scheda prodotto e la buy box*"

##### DESCRIZIONE

All'interno di questa sezione è possibile impostare:

- informazioni aggiuntive rispetto alle specifiche già indicate nella
  sezione Categoria, e relative sempre ai prodotti che verranno
  pubblicati mediante l'Inserzione che si sta codificando -- sezioni
  **Generale**, **Descrizione**, **Dimensioni Prodotto**, **Parole
  Chiave** ecc..

- una "**data di rilascio**" per gli articoli pubblicati mediante le
  relative inserzioni

- **le condizioni di vendita dei prodotti** esportati sul marketplace
  collegato all'Inserzione che si sta codificando -- sezione
  **Condizioni**

- informazioni relative alla spedizione -- sezioni **Dimensioni Pacco**
  e **Dettagli di Spedizione**

- i cosiddetti "**Identificativi del Catalogo Amazon**" ossia i codici
  (UPC, EAN, ISBN o ASIN) utilizzati per identificare univocamente i
  vari articoli all'interno del Catalogo Amazon -- sezione
  **Identificativi del Catalogo Amazon**

![](./assets/media/image213.png)

###### METODI DI DESCRIZIONE

La sottosezione "**Metodo di Descrizione**" consente di decidere se
compilare i campi relativi al tab "Descrizione" secondo quanto
configurato all'interno di uno dei Template precedentemente codificati
(e magari già utilizzato in qualche altra inserzione) oppure se
realizzarne uno nuovo

Nel primo caso (applicazione di un Template preconfigurato) sarà
sufficiente selezionare il Template desiderato tra quelli presenti
all'interno dell'apposito menu a tendina.

Nel secondo caso (definizione di nuovi parametri per i campi presenti
all'interno della maschera) sarà sufficiente settare il campo "**Metodo
di Descrizione**" sull'opzione "**Custom"** e procedere poi alla
configurazione dei restanti parametri.

In questo caso inoltre, una volta impostati e salvati correttamente
tutti i valori verrà automaticamente creato anche un nuovo Template
(visualizzabile e gestibile all'interno della maschera "**Lista dei
Metodi di Descrizione**" precedentemente analizzata) con il nome
dell'Inserzione che si sta realizzando.

###### GENERALE

La sottosezione "**Generale**" del tab "Descrizione" consente di
impostare ulteriori informazioni di carattere generale sugli articoli
che saranno poi pubblicati mediante l'Inserzione in oggetto (es.
Produttore, Quantità del pacco, Paese di Origine, Codice Fiscale del
prodotto ...)

![](./assets/media/image214.png)

Dipendentemente dallo specifico campo considerato sarà quindi possibile
valorizzare la relativa informazione, per ciascuno degli articoli messi
in vendita tramite l'Inserzione in esame, con:

- **Attributi Articolo** relativi ad appositi campi presenti all'interno
  del gestionale

- **Attributi Passweb** codificati all'interno dell'apposita sezione del
  Wizard

- **Valori Personalizzati**, inseriti direttamente all'interno del
  relativo campo di input. Utilizzando dei Valori Personalizzati, questi
  saranno poi gli stessi per tutti gli articoli pubblicati mediante
  l'Inserzione che si sta codificando

In particolare poi il campo "**SKU**" oltre che con "Valori
Personalizzati" e con "Attributi Passweb" potrà essere mappato anche con
i seguenti Attributi Articolo

- **Codice:** in questo caso, per ciascuno degli articoli coinvolti
  nell'Inserzione, il valore dello SKU verrà prelevato direttamente dal
  codice gestionale del relativo articolo

- **Codice Alternativo:** in questo caso, per ciascuno degli articoli
  coinvolti nell'Inserzione, il valore dello SKU verrà prelevato
  direttamente dal codice alternativo utilizzato all'interno del
  gestionale per il corrispondente articolo

Il parametro "**A parità di ASIN aggancia il prodotto a quello già
esistente su Amazon**" consente invece di decidere se agganciare o meno
in fase di pubblicazione un'eventuale prodotto già presente sul
marketplace non solo in base al valore del campo con cui è stato mappato
lo SKU ma tenendo conto anche dell'ASIN assegnato allo stesso prodotto.

Nello specifico se il parametro in esame dovesse essere:

- **Attivato:** in questo caso se su Amazon esiste **un solo prodotto**
  c**on ASIN uguale a quello assegnato ad uno degli articoli coinvolti
  nell'inserzione**, in fase di pubblicazione il prodotto in questione
  verrà agganciato a quello già presente sul marketplace .

> Se invece su Amazon dovessero essere presenti **più prodotti con ASIN
> uguale a quello assegnato ad uno degli articoli coinvolti
> nell'inserzione** allora se oltre all'ASIN l'articolo in esame dovesse
> avere anche lo SKU uguale a quello del prodotto già presente sul
> Marketplace, in fase di pubblicazione verrà agganciato l'articolo già
> presente, in caso contrario verrà invece creato un nuovo articolo con
> ASIN uguale a quello già presente su Amazon e con SKU uguale invece a
> quello settato nell'inserzione

- **Disattivato**: in questo caso il controllo **verrà fatto unicamente
  in base allo SKU** per cui se su Amazon dovesse essere presente un
  articolo con SKU uguale a quello settato per uno dei prodotti
  coinvolti nell'inserzione, in fase di pubblicazione verrà agganciato
  quel prodotto.

> In caso contrario verrà invece creato un nuovo prodotto

Come il campo SKU anche il "**Titolo**", oltre che con "Valori
Personalizzati" e con "Attributi Passweb" potrà essere mappato con il
seguente Attributo Articolo

- **Titolo:** in questo caso, per ciascuno degli articoli coinvolti
  nell'Inserzione, il nome dell'articolo da passare ad Amazon sarà
  esattamente lo stesso di quello visualizzato in Passweb all'interno
  del componente "Titolo". In questo senso l'effettivo valore
  (descrizione presente nell'anagrafica gestionale, valore di un
  attributo o valore personalizzato) dipendono direttamente da come si è
  deciso di gestire il "Titolo" dell'articolo

Infine il campo "**Codice Fiscale prodotto**", mappabile con un "Valore
Personalizzato" o un "Attributo Passweb" consente di indicare il codice
necessario ad Amazon per individuare l'aliquota iva da assegnare ai
prodotti coinvolti nell'inserzione in esame

**ATTENZIONE!** Tale campo potrebbe essere richiesto come obbligatorio
nel momento in cui si dovesse attivare su Amazon la fatturazione
elettronica

**ATTENZIONE!** i prezzi passati ad Amazon da Passweb sono già
comprensivi di IVA per cui eventuali scorpori secondo l'aliquota
corrispondente al codice indicato verranno eventualmente calcolati
direttamente da Amazon

Per maggiori informazioni relativamente ai codici corrispondenti alle
diverse aliquote si consiglia di fare riferimento direttamente alla
documentazione Amazon disponibile al seguente link
<https://sellercentral.amazon.it/help/hub/reference/G202088390>

**ATTENZIONE!** Considerando che Amazon a differenza di eBay non mette a
disposizione dell'utente una Sandbox in cui effettuare pubblicazioni di
prova, la data di rilascio potrebbe essere particolarmente utile (se
impostata molto in avanti nel tempo) per effettuare test di
pubblicazione sull'ambiente di produzione senza correre il rischio che
articoli di test vengano effettivamente visti ed acquistati all'interno
del Marketplace.

###### IDENTIFICATIVI CATALOGO AMAZON

Gli "**Identificativi Catalogo Amazon**" sono dei codici necessari per
identificare univocamente ogni singolo prodotto all'interno del catalogo
Amazon.

In questo senso è bene subito fare alcune considerazioni di fondamentale
importanza:

- Nel momento in cui si dovesse pubblicare un articolo con il codice
  ASIN, EAN, UPC o ISBN uguale a quello di un altro articolo già
  presente su Amazon, non verrà creata, nel Marketplace, una nuova
  pagina prodotto e la nostra inserzione verrà invece agganciata a
  quella dell'articolo già presente sul Marketplace stesso (posto
  ovviamente che tutti i dati passati in fase di pubblicazione siano
  coerenti con quelli già presenti sul Marketplace e con quanto
  richiesto da Amazon stessa)

- **Per agganciare, in fase di pubblicazione, un articolo già presente
  su Amazon si consiglia di utilizzare sempre, laddove possibile, il
  codice ASIN come campo chiave. In questo modo sarà infatti possibile,
  generalmente, procedere alla pubblicazione senza dover gestire
  nell'inserzione altre specifiche.**

> Nel momento in cui si dovesse invece decidere di utilizzare come campo
> chiave lo SKU, il codice EAN o un altro identificativo Amazon,
> potrebbe poi essere necessario gestire nell'Inserzione altre
> specifiche richieste dal Marketplace che potranno variare in relazione
> alla specifica categoria di prodotto da pubblicare e che, soprattutto,
> potrebbero dover avere esattamente gli stessi valori delle specifiche
> attualmente presenti su Amazon

- Agganciando uno dei prodotti già presenti sul Marketplace **le
  caratteristiche dell'articolo da noi pubblicato non saranno (ad
  eccezione del prezzo ovviamente) quelle definite nell'Inserzione ma
  bensì quelle relative all'articolo già presente nella Buy Box di
  Amazon**

Detto questo, occorre poi sottolineare che dipendentemente dallo
specifico marketplace su cui si sta operando ed anche dalla tipologia di
prodotti messi in vendita può essere necessario / obbligatorio indicare,
in fase di pubblicazione, per ogni articolo coinvolto nell'Inserzione:

- **il codice ASIN:** rappresenta ossia il codice identificativo
  (interno) assegnato ai vari prodotti direttamente da Amazon

- **il codice UPC**: rappresenta il codice numerico di ogni articolo
  soggetto alle norme UPC (Universal Product Code) in uso,
  principalmente, negli Stati Uniti

- **il codice EAN**: (European Article Number) è il classico Codice a
  Barre in uso principalmente in Europa

- **il codice ISBN**: (International Standard Book Number) è un numero
  che identifica a livello internazionale, in modo univoco e duraturo,
  un titolo o un'edizione di un titolo di un determinato autore

Ciascuno di questi campi può essere mappato con uno dei valori
selezionabili all'interno del corrispondente menu a tendina

![](./assets/media/image215.png)

E' quindi possibile valorizzare questi codici, per ciascuno degli
articoli messi in vendita tramite l'Inserzione in esame, con:

- uno qualsiasi degli **Attributi Articolo** attualmente gestiti
  all'interno del proprio sito Passweb

- il **codice articolo** in uso all'interno del gestionale

- il **codice alternativo** dell'articolo in uso all'interno del
  gestionale

- il **codice alias** dell'articolo in uso all'interno del gestionale.

> **ATTENZIONE!** A differenza del codice e del codice alternativo,
> all'interno del gestionale possono essere definiti anche più codici
> alias per lo stesso prodotto.
>
> In questo caso dunque l'applicazione si comporterà in maniera diversa
> a seconda del fatto che il gestionale collegato al sito Ecommerce sia
> Mexal oppure uno dei gestionali Ho.Re.Ca.
>
> **[SITI ECOMMERCE COLLEGATI A MEXAL]{.underline}**
>
> In questo caso è possibile marcare uno degli N codici alias in uso
> all'interno del gestionale in maniera tale da identificarlo
> esattamente come quello che dovrà poi essere passato ad Amazon in fase
> di pubblicazione dell'articolo.
>
> Per far questo è sufficiente accedere alla maschera di creazione del
> codice Alias

![](./assets/media/image87.png)

> e compilare i vari campi come di seguito indicato:

- **Codice**: inserire il valore del codice (EPID / UPC / EAN / ISBN)
  che dovrà essere passato ad Amazon in fase di pubblicazione del
  prodotto

- **Descrizione:** indicare la tipologia di codice Amazon che si intende
  mappare.

> In particolare nel caso in cui il codice in esame debba essere
> considerato come l' ASIN all'interno di questo campo andrà inserito il
> valore **ASIN**.
>
> Se invece il codice in esame dovrà essere considerato come il codice
> UPC / EAN / ISBN da passare ad Amazon all'interno del campo
> descrizione andrà inserito il valore **GTIN**

- **Elemento TG -- solo per articoli a Taglia:** indicare,
  selezionandola dall'apposito menu a tendina, la specifica Taglia cui
  il codice in esame dovrà essere riferita

> Supponendo dunque di aver utilizzato all'interno del gestionale N
> codici alias per un determinato articolo e di aver marcato in maniera
> corretta solo uno di essi come codice ASIN (secondo quanto sopra
> indicato) il campo "ASIN" presente nella sezione "Identificativi
> Catalogo Amazon" andrà poi impostato sul valore "**Codice Alias
> ASIN**" come evidenziato in figura

![](./assets/media/image216.png)

> In queste condizioni in fase di pubblicazione sul marketplace verrà
> passato ad Amazon il codice alias marcato sul gestionale come codice
> ASIN.
>
> Allo stesso modo se l'esigenza dovesse essere quella di passare ad
> Amazon il codice UPC / EAN / ISBN sarà necessario marcare uno tra gli
> N codici Alias utilizzati secondo quanto precedentemente indicato e
> impostare poi, questa volta, il relativo campo UPC / EAN / ISBN
> dell'Inserzione presente nella sezione "**Codice Alias GTIN**"

![](./assets/media/image217.png)

> **ATTENZIONE!** Nel caso in cui per determinate ragioni dovessero
> essere marcati più codici alias come, ad esempio, codici ASIN da
> passare ad Amazon, in fase di pubblicazione verrà considerato, ai fini
> dell'inserzione sul marketplace, solo il primo valore utile.
>
> **[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI
> HO.RE.CA.]{.underline}**
>
> In questo caso sarà possibile mappare il campo ASIN con il codice
> alias di una determinata tipologia (es. Codice EAN13, Codice EAN8
> ecc...) selezionandola tra quelle in uso all'interno del gestionale.
>
> A differenza di Mexal in questo caso però, non è possibile marcare uno
> degli N codici alias o EAN in uso all'interno del gestionale come
> quello che identifica in maniera specifica il codice da passare ad
> Amazon in fase di pubblicazione pertanto, nel momento in cui un
> determinato articolo dovesse avere più valori per la stessa tipologia
> di Alias verrà considerato, ai fini dell'inserzione sul marketplace,
> solo il primo valore utile.

**ATTENZIONE! Per poter mettere in vendita correttamente degli articoli
all'interno di uno qualsiasi dei marketplace Amazon è necessario gestire
almeno uno dei codici sopra indicati**. Nel caso in cui non si dovesse
gestire nessuno di questi codici, generalmente, non sarà possibile
pubblicare articoli sui marketplace Amazon.

In realtà esiste anche la possibilità, **se opportunamente abilitati da
Amazon stessa**, di vendere articoli privi di codici identificativi
(UPC, EAN o ISBN)

In fase di pubblicazione delle proprie inserzioni vanno infatti
considerate le seguenti casistiche:

**[CASO 1 🡪 Il venditore gestisce articoli dotati di bar code (e quindi
di uno specifico codice identificativo)]{.underline}**

In queste condizioni il venditore deve necessariamente identificare i
prodotti che mette in vendita sul marketplace Amazon con il loro codice
univoco utilizzando i campi precedentemente analizzati

**[CASO 2 🡪 Il venditore gestisce articoli prodotti senza Bar Code (e
che non hanno quindi uno specifico codice identificativo)]{.underline}**

In queste condizioni il venditore dovrà:

a.  Chiedere specificatamente ad Amazon l'autorizzazione per l'esenzione
    all'utilizzo dei codici identificativi (Bar code) **relativamente ad
    uno specifico Brand**

> **ATTENZIONE**: Il Brand per il quale si richiede l'esenzione
> all'utilizzo dei codici identificativi deve essere esattamente lo
> stesso inserito, in fase di configurazione dell'inserzione,
> all'interno del campo "**Marca**"

![](./assets/media/image218.png)

> E' di fondamentale importanza che il Brand, in relazione al quale si è
> richiesta l'esenzione, coincida esattamente con quello inserito poi
> all'interno del campo evidenziato in figura

b.  Nel caso in cui Amazon accetti la richiesta il Venditore riceverà
    un' Email del tipo

> *"Your exemption has been accepted, use **PARAMETER_1** to identify
> your products instead of the StandardProductId"*
>
> dove **PARAMETER_1** sarà un codice speciale fornito da Amazon stessa
> al venditore e che il venditore dovrà utilizzare per "marcare" i
> propri prodotti.
>
> Tale codice andrà inserito, in fase di configurazione della relativa
> inserzione su Passweb all'interno del campo "**MFR Number Part**"
> evidenziato in figura (sezione "Identificativi Catalogo Amazon")

![](./assets/media/image219.png)

> Amazon verificherà in fase di pubblicazione che il codice
> "**PARAMETER_1**" ed il brand inserito all'interno del campo "Marca"
> siano effettivamente quelli in relazione ai quali è stata richiesta
> l'esenzione all'utilizzo dei codici identificativi e, in caso
> affermativo, procederà alla pubblicazione.
>
> **ATTENZIONE**! In queste condizioni il campo "**Ignora ID Prodotto**"
> deve essere impostato sul valore "**Nessuno**"

c.  Nel caso in cui Amazon non accetti la richiesta e/o i dati inseriti
    all'interno dei campo "**Marca**" e "**MFR Number Part**" non
    coincidano con quelli in relazione ai quali è stata richiesta
    l'esenzione, il venditore non potrà pubblicare articoli privi di
    codici identificativi

**[CASO 3 🡪 Il venditore è allo stesso tempo anche il produttore degli
articoli da pubblicare all'interno del Marketplace]{.underline}**

In queste condizioni il venditore dovrà:

a.  Registrare il proprio Brand nel relativo catalogo Amazon (per
    maggiori informazioni in merito rivolgersi alla relativa assistenza
    o documentazione Amazon).

> **ATTENZIONE**: Il Brand registrato all'interno dei cataloghi Amazon
> deve essere esattamente lo stesso inserito poi, in fase di
> configurazione dell'inserzione, all'interno del campo "**Marca**"

![](./assets/media/image218.png)

b.  Nel caso in cui Amazon accetti la richiesta il Venditore riceverà
    un' Email del tipo

> *"Your brand registration has been accepted, use PARAMETER_2 to
> identify your products instead of the StandardProductId"*
>
> dove **PARAMETER_2** sarà un codice speciale fornito da Amazon stessa
> al venditore e che il venditore dovrà utilizzare per "marcare" i
> propri prodotti.
>
> Tale codice andrà inserito, in fase di configurazione della relativa
> inserzione su Passweb all'interno del campo "**MFR Number Part**"
> evidenziato in figura (sezione "Identificativi Catalogo Amazon")

![Videate\\amazon_mfr_number_part_2.bmp](./assets/media/image219.png)

> Amazon verificherà in fase di pubblicazione che il codice
> "**PARAMETER_2**" ed il brand inserito all'interno del campo "Marca"
> siano effettivamente quelli in relazione ai quali è stata richiesta la
> registrazione all'interno dei cataloghi Amazon.
>
> **ATTENZIONE!** In queste condizioni il campo "**Ignora ID Prodotto**"
> deve essere necessariamente impostato sul valore "**Private Label**"

a)  Nel caso in cui Amazon non accetti la richiesta e/o i dati inseriti
    all'interno dei campo "Marca" e "MFR Number Part" non coincidano con
    quelli in relazione ai quali è stata richiesta la registrazione, il
    venditore non potrà pubblicare articoli privi di codici
    identificativi

**ATTENZIONE! I codici ASIN, EAN, UPC o ISBN sono di fondamentale
importanza anche per quella che è la particolare modalità di vendita
adottata da Amazon all'interno dei propri Marketplace.**

A differenza di quanto avviene con eBay infatti, mettendo in vendita
degli articoli su Amazon **non è detto che vengano poi create,
all'interno del relativo Marketplace, delle nuove pagine Prodotto**.

La creazione di una nuova pagina prodotto all'interno del Marketplace
dipende infatti dal codice EAN, UPC o ISBN dell'articolo che si è deciso
di pubblicare.

In particolare:

- **Se l'articolo messo in vendita dovesse avere un codice EAN, UPC o
  ISBN uguale a quello di un altro articolo già presente all'interno del
  Marketplace** (probabilità piuttosto frequente nel momento in cui si
  dovessero rivendere articoli prodotti da altri) **Amazon** **non
  creerà nessuna nuova pagina Prodotto**.

> **ATTENZIONE!** In queste condizioni Amazon tenterà di aggancerà la
> nostra inserzione all'articolo già presente sul marketplace (che
> potrebbe anche essere stato pubblicato da un altro Venditore) e sarà
> sempre Amazon, sulla base dei suoi criteri interni di gestione, a
> decidere se il nostro prodotto dovrà comparire direttamente nella
> **"Buy Box"**, nel riquadro **"Confronta offerte su Amazon"** oppure
> solamente **nell'elenco delle offerte effettuate da tutti gli altri
> venditori** di quello stesso articolo.

- **Se l'articolo messo in vendita dovesse avere un codice EAN, UPC o
  ISBN che non coincide con quello di nessun altro articolo già presente
  sul Marketplace** (cosa che si verificherà sicuramente nel momento in
  cui dovessimo essere gli unici produttori e rivenditori del prodotto
  pubblicato) **Amazon creerà una nuova pagina Prodotto** contente tutte
  le specifiche inviate a seguito della nostra pubblicazione

> In queste condizioni, essendo gli unici venditori del prodotto
> pubblicato, il nostro articolo verrà ovviamente inserito all'interno
> della relativa Buy Box di Amazon
>
> Per maggiori informazioni in merito in merito alla gestione della Buy
> Box e ai criteri di pubblicazione di Amazon si veda anche il
> successivo capitolo "Amazon -- La scheda prodotto e la Buy Box" di
> questo manuale oppure si consulti la relativa documentazione
> accessibile direttamente sulla Seller Central dal Back End del proprio
> Account Venditore.

Il campo **ASIN** presente all'interno della sezione "Identificativi
Catalogo Amazon" consente invece di gestire, a livello di Inserzione, il
codice ASIN ossia il codice identificativo associato da Amazon stessa
agli articoli pubblicati all'interno del marketplace.

![](./assets/media/image220.png)

A differenza dei codici EAN/UPC/ISBN, ovviamente, il valore del codice
ASIN potrà essere determinato solo a seguito di una prima pubblicazione
degli articoli coinvolti nell'inserzione, **per cui tale campo diventerà
utile, e dovrà effettivamente essere valorizzato, solo nel caso in cui
gli articoli pubblicati mediante l'inserzione in esame siano già
presenti all'interno del marketplace (ad esempio perché pubblicati
esternamente Passweb).**

In queste condizioni infatti l'inserimento del codice ASIN corretto
consentirà a Passweb di agganciare l'articolo già presente sul
marketplace, articolo questo che potrà quindi essere gestito, d'ora in
avanti direttamente da Passweb sia a livello di quantità presenti sul
marketplace che a livello di regole automatiche di messa in vendita,
rimessa in vendita e blocco.

**ATTENZIONE! Per agganciare, in fase di pubblicazione, un articolo già
presente su Amazon si consiglia di utilizzare sempre, laddove possibile,
il codice ASIN come campo chiave. In questo modo sarà infatti possibile,
generalmente, procedere alla pubblicazione senza dover gestire
nell'inserzione altre specifiche.**

Nel momento in cui si dovesse invece decidere di utilizzare come campo
chiave lo SKU, il codice EAN o un altro identificativo Amazon, potrebbe
poi essere necessario gestire nell'Inserzione altre specifiche richieste
dal Marketplace che potranno variare in relazione alla specifica
categoria di prodotto da pubblicare e che, soprattutto, potrebbero dover
avere esattamente gli stessi valori delle specifiche attualmente
presenti su Amazon

Come già visto per i codici EAN, UPC e ISBN anche il campo relativo al
codice ASIN potrà essere valorizzato, per ciascuno degli articoli messi
in vendita tramite l'Inserzione in esame, con:

- il **codice articolo** in uso all'interno del gestionale

- il **codice alternativo** dell'articolo in uso all'interno del
  gestionale (solo Ecommerce Mexal)

- uno dei **codici alias** (EAN13, EAN8, Code39 ....) dell' articolo
  (solo Ecommerce Ho.Re.Ca.)

- uno qualsiasi degli **Attributi Articolo** attualmente gestiti
  all'interno del proprio sito Passweb

Nel caso in cui alcuni articoli pubblicati mediante l'inserzione che
stiamo realizzando dovessero essere già presenti sul marketplace sarà
dunque necessario, ad esempio:

- creare un apposito attributo articolo chiamato "ASIN Mexal"

- impostare il campo **ASIN** presente all'interno della sezione
  "Identificativi Catalogo Amazon" sull'attributo creato al punto
  precedente

- valorizzare l'attributo "ASIN Mexal" per ciascuno degli articoli già
  presenti sul marketplace con il relativo codice ASIN prelevandolo
  direttamente da Amazon stessa

In alternativa, e sempre nel caso in cui si desideri ovviamente
agganciare all'inserzione Passweb articoli già presenti sul marketplace,
potrebbe anche essere possibile non valorizzare il campo ASIN a livello
di Inserzione e andare poi ad inserire manualmente, o tramite import
csv, su ogni singolo articolo presente nella lista di vendita, prima di
effettuare la pubblicazione, il relativo codice ASIN.

![](./assets/media/image221.png)

Per maggiori informazioni in merito si veda anche il successivo capitolo
*"Gestione lista di vendita e pubblicazione su Amazon"*

Il campo **Parent ASIN** infine, è di fondamentale importanza nel caso
di articoli gestiti a taglie / colori e consente di raggruppare tutte le
taglie / colori di uno stesso articolo all'interno della stessa scheda
prodotto Amazon

![](./assets/media/image222.png)

Nel caso in cui l'esigenza dovesse dunque essere quella di pubblicare
una nuova taglia e/o un nuovo colore per un articolo già presente nel
database Amazon e quindi con la sua scheda prodotto già presente sul
Marketplace, sarà necessario valorizzare il campo **Parent ASIN** con il
codice ASIN di questo stesso articolo.

**In caso contrario la nuova taglia / colore dell'articolo non verrà
inserita come possibile opzione di scelta nella scheda prodotto
dell'articolo padre ma andrà a creare su Amazon una nuova singola scheda
prodotto.**

Anche in questo caso come già visto per i codici EAN, UPC, ISBN e ASIN
anche il campo relativo al codice "Parent ASIN" potrà essere
valorizzato, per ciascuno degli articoli messi in vendita tramite
l'Inserzione in esame, con:

- il **codice articolo** in uso all'interno del gestionale

- il **codice alternativo** dell'articolo in uso all'interno del
  gestionale (solo Ecommerce Mexal)

- uno dei **codici alias** (EAN13, EAN8, Code39 ....) dell' articolo
  (solo Ecommerce Ho.Re.Ca.)

- uno qualsiasi degli **Attributi Articolo** attualmente gestiti
  all'interno del proprio sito Passweb

###### CONDIZIONI

La sottosezione "**Condizioni**" del tab "Descrizione" consente di
impostare **le condizioni di vendita dei prodotti** esportati sul
marketplace collegato all'Inserzione che si sta codificando

In questo senso sarà quindi necessario selezionare uno dei valori
disponibili tra quelli presenti all'interno del relativo menu a tendina
(campo **Condizioni**) e inserire un'eventuale Nota (campo **Nota sulle
Condizioni**).

![](./assets/media/image223.png)

**ATTENZIONE!** Le condizioni di vendita sono fornite direttamente da
Amazon, possono variare a seconda dello specifico marketplace su cui si
sta operando e non possono essere in alcun modo personalizzate

###### IMMAGINI

La sottosezione "**Immagini**" del tab "Descrizione" consente di
impostare ulteriori **Immagini** dell'articolo da passare al Marketplace
in fase di pubblicazione degli articoli coinvolti nell'Inserzione.

In questo senso va detto che è possibile decidere di pubblicare su
Amazon fino a 8 immagini diverse selezionando il valore desiderato
all'interno del corrispondente campo presente in questa sezione

![](./assets/media/image224.png)

**ATTENZIONE!** Come Immagini aggiuntive verranno utilizzate le
**Immagini Secondarie della Scheda Prodotto** Passweb.

Nel momento in cui si dovesse quindi decidere di pubblicare su Amazon,
ad esempio, 4 Immagini sarà poi necessario accertarsi che per gli
articoli facenti parte dell'Inserzione in oggetto siano correttamente
gestite all'interno del sito Passweb oltre all'Immagine Principale anche
altre 3 Immagini Secondarie

###### DESCRIZIONE

La sottosezione "**Descrizione**" del tab "Descrizione" consente di
impostare la descrizione dei prodotti coinvolti nell'inserzione

![](./assets/media/image225.png)

Il campo in esame può essere mappato con uno degli Attributi Passweb
attualmente gestiti, oppure con l'Attributo Articolo "Descrizione". In
quest'ultimo il valore della descrizione verrà prelevato direttamente
dal campo "Descrizione" presente nell'anagrafica Passweb del relativo
articolo

###### DIMENSIONI PACCO E DETTAGLI SPEDIZIONE

Per quel che riguarda i dati relativi alle spedizioni che verranno poi
effettuate per ordini collegati all'inserzione che si sta realizzando,
la sezione:

- **Dimensioni Prodotto**: consente di impostare informazioni quali
  Lunghezza, Larghezza, Altezza, Peso e Volume dei prodotti coinvolti
  nell'Inserzione

- **Dimensioni Pacco:** consente di impostare informazioni quali
  Lunghezza, Larghezza, Altezza, Peso e Volume del Pacco

- **Dettagli di Spedizione**: consente invece di definire il peso della
  spedizione, l'unità di misura utilizzata per il calcolo del peso e
  soprattutto il "**Gruppo dei costi di spedizione**" associato
  all'inserzione

![](./assets/media/image226.png)

**ATTENZIONE! Per evitare eventuali messaggi di warning in fase di
pubblicazione degli articoli occorre impostare correttamente il campo
"Gruppo dei costi di spedizione**"

**Gruppo dei costi di spedizione:** consente di impostare il "Gruppo dei
costi di spedizione" da associare ai vari articoli che verranno
pubblicati mediante l'inserzione in oggetto.

Tale campo risulta essere quindi di fondamentale importanza in quanto a
seconda dello specifico gruppo che verrà utilizzato per un determinato
articolo, questo stesso articolo potrà essere venduto su Amazon con
certe spese di spedizione piuttosto che con altre.

**ATTENZIONE!** La creazione dei diversi gruppi dei costi di spedizione
e, di fatto dunque, la gestione e la definizione delle spese di
spedizione può essere impostata solo ed esclusivamente all'interno del
Back end di Amazon dalla relativa sezione "**Impostazioni di
Spedizione**".

Per il parametro in oggetto è possibile selezionare uno dei seguenti
valori:

- **Nessuno:** selezionando questa opzione la specifica corrispondente
  non verrà valorizzata e, conseguentemente, in fase di pubblicazione
  degli articoli collegati all'inserzione in esame non verrà indicato ad
  Amazon nessun Gruppo dei costi di spedizione.

> **In queste condizioni potrebbero essere notificati in fase di
> pubblicazione eventuali messaggi di warning che non dovrebbero
> comunque pregiudicare la corretta pubblicazione degli articoli**

- **Valore Personalizzato:** selezionando questa opzione sarà possibile
  indicare nel successivo campo il nome del Gruppo dei Costi di
  spedizione da utilizzare per la pubblicazione degli articoli collegati
  all'inserzione che si sta realizzando.

> **ATTENZIONE!** Il nome del gruppo dei costi di spedizione deve
> coincidere esattamente con uno di quelli creati in Amazon all'interno
> della relativa sezione "**Impostazioni di Spedizione**" (per maggiori
> informazioni in merito si consiglia di fare riferimento alla specifica
> documentazione Amazon)

![](./assets/media/image227.png)

> In queste condizioni, ovviamente, il gruppo dei costi di spedizione
> impostato sarà sempre lo stesso per tutti gli articoli collegati
> all'inserzione che si sta realizzando.
>
> Nel caso in cui l'esigenza dovesse essere invece quella di utilizzare
> un Gruppo dei Costi di Spedizione diverso articolo per articolo sarà
> allora necessario utilizzare l'opzione "**Attributi Passweb**"

- **Attributo Passweb:** in questo caso sarà possibile indicare il
  valore da utilizzare per la corrispondente specifica, selezionandolo
  tra gli attributi articolo attualmente mappati all'interno di Passweb.

> Anche in questo caso il nome del Gruppo dei costi di spedizione
> impostato, mediante l'Attributo indicato, articolo per articolo dovrà
> coincidere esattamente con uno di quelli creati in Amazon all'interno
> della relativa sezione "**Impostazioni di Spedizione**".
>
> In queste condizioni sarà quindi possibile indicare un diverso gruppo
> dei costi di spedizione per ogni singolo articolo pubblicato
> all'interno del Marketplace.

###### PAROLE CHIAVE

La sottosezione "**Parole Chiave**" del tab "Descrizione" consente di
impostare le eventuali Keyword di ricerca e gli elenchi puntati
(caratteristiche descrittive) che dovranno essere utilizzati per gli
articoli coinvolti nell'Inserzione

![](./assets/media/image228.png)

Anche in questo caso, tanto le Parole Chiave, quanto gli Elenchi Puntati
potranno esser mappati su di un "Valore Personalizzato" oppure su un ben
preciso "Attributo Passweb"

##### PAGAMENTO

All'interno di questa sezione è possibile specificare le modalità di
pagamento che dovranno essere rese disponibili agli utenti Amazon in
fase di acquisto degli articoli messi in vendita tramite l'Inserzione
che si sta codificando.

![](./assets/media/image229.png)

**ATTENZIONE! La lista dei possibili pagamenti è fornita direttamente da
Amazon e potrebbe variare a seconda dello specifico marketplace su cui
si sta operando**

Per abilitare un pagamento tra quelli presenti in elenco è sufficiente
selezionare il check presente in corrispondenza del pagamento stesso.

Considerando inoltre che gli ordini effettuati su Amazon potrebbero poi
essere importati in Passweb e da qui essere inseriti sul gestionale,
sarà necessario anche mappare ciascuno dei pagamenti abilitati con una
delle modalità di pagamento gestite sul proprio sito Passweb e
corrispondenti quindi ad uno dei Pagamenti codificati nelle relative
tabelle gestionali.

In questo senso è possibile indicare la modalità di pagamento desiderata
selezionandola tra quelle disponibili all'interno del corrispondente
menu a tendina

![](./assets/media/image230.png)

##### SPEDIZIONE

All'interno di questa sezione è possibile impostare alcuni parametri
relativi alla spedizioni che dovranno essere utilizzate per gli articoli
messi in vendita mediante l'Inserzione in esame

![](./assets/media/image231.png)

In particolare il parametro:

**Tempo di spedizione:** consente di indicare quello che dovrebbe essere
il tempo di spedizione raccomandato selezionandolo tra uno di quelli
presenti all'interno del corrispondente menu a tendina e forniti
direttamente da Amazon.

**Articolo Spesa per Confezione Regalo**: consente di indicare,
selezionandolo dal relativo menu a tendina, l'articolo Spesa che dovrà
essere utilizzato nei relativi documenti gestionali per gestire
eventuali Confezioni Regalo legate ad articoli coinvolti nell'Inserzione
che si sta codificando

All'interno della sezione "**Spedizione**" è possibile definire invece
gli articoli di tipo Spesa che dovranno essere utilizzati (ed inseriti
quindi nel corpo dei relativi documenti gestionali) per gestire le spese
di spedizione di prodotti venduti sul marketplace, rispettivamente, con
"**Spedizioni Standard**" e con "**Spedizioni Express**"

**ATTENZIONE!** **Il costo delle spese di spedizione può essere definito
solo ed esclusivamente all'interno del Back end di Amazon dalla relativa
sezione "Impostazioni di Spedizione".**

![Videate\\amazon_gruppo_costi_spedizione2.bmp](./assets/media/image192.png)

All'interno di questa sezione sarà infatti possibile impostare diversi
"Gruppi di costi di spedizione" definendo per ciascuno di essi specifici
costi sia per le spedizioni di tipo Standard che per quelle di tipo
Express.

Lato Passweb sarà invece possibile, come indicato nei precedenti
capitoli di questo manuale, associare agli articoli presenti in una
lista di vendita uno dei "Gruppi di costi di spedizione" definiti su
Amazon.

Nel momento in cui un cliente dovesse acquistare sul marketplace un
determinato articolo selezionando per esso, ad esempio, una spedizione
"Standard", nel corpo del relativo documento gestionale verrà inserito
l'articolo spesa indicato all'interno del campo "**Articolo Spesa per
Spedizione Standard**" con un valore pari a quello definito, su Amazon,
per la spedizione di tipo standard all'interno del gruppo dei costi di
spedizione associato all'articolo in esame.

**ATTENZIONE!** I parametri "**Articolo Spesa per Spedizioni Standard**"
e "**Articolo Spesa per Spedizioni Express**" definiti a livello di
singola Inserzione non sono obbligatori

In relazione a questi due parametri è quindi bene ricordare sempre che:

- Nel momento non dovessero essere valorizzati sulla singola Inserzione
  verranno utilizzati gli articoli spesa impostati per gli stessi
  parametri definiti però a livello di Account

- Se impostati, quelli a livello di singola Inserzione hanno priorità
  rispetto a quelli impostati a livello di Account

##### PREZZO QUANTITA' FORMATO

All'interno di questa sezione è possibile definire le condizioni di
vendita degli articoli in relazione ad informazioni quali il prezzo e la
tipologia di vendita.

![](./assets/media/image232.png)

In questo senso la sezione "**Metodo di Prezzo, quantità e formato**"
consente di decidere se adottare uno dei Template precedentemente
codificati (e magari già utilizzato in qualche altra inserzione) oppure
realizzarne uno nuovo.

Nel primo caso (applicazione di un Template preconfigurato) sarà
sufficiente selezionare il Template desiderato tra quelli presenti
all'interno dell'apposito menu a tendina.

Nel secondo caso (definizione di nuovi parametri per quantità prezzo e
formato) sarà sufficiente settare il campo "**Metodo di Prezzo, quantità
e formato**" sull'opzione "**Custom"** e procedere poi alla
configurazione dei restanti parametri presenti all'interno della pagina.

In questo caso inoltre, una volta impostati e salvati correttamente
tutti i valori verrà automaticamente creato anche un nuovo Template
(visualizzabile e gestibile all'interno della maschera "**Lista dei
Metodi di Prezzo, quantità e formato**" precedentemente analizzata) con
il nome dell'Inserzione che si sta realizzando.

###### QUANTITA' DI ARTICOLI PUBBLICATI

All'interno della sezione "**Quantità**" è possibile definire la
quantità con cui gli articoli pubblicati mediante questa stessa
inserzione dovranno poi essere disponibili sul Marketplace.

**ATTENZIONE!** A differenza di quanto avviene nell'integrazione con i
Marketplace eBay, è possibile pubblicare su Amazon anche articoli in
quantità pari a 0, cosa questa utile in fase di test (considerando anche
che Amazon non mette a disposizione delle Sandbox per cui tutte le
pubblicazioni avvengono sempre nel marketplace reale)

![](./assets/media/image233.png)

- **Singolo oggetto:** in queste condizioni ogni articolo messo in
  vendita tramite l'Inserzione in esame verrà considerato come oggetto
  singolo ed avrà quindi, sul marketplace, quantità disponibile pari a 1

- **Valore Personalizzato:** in queste condizioni è possibile indicare
  all'interno del successivo campo "**Valore della Quantità**" l'esatto
  valore con cui ogni articolo messo in vendita tramite l'Inserzione in
  esame dovrà poi essere disponibile, sul relativo marketplace

> Supponendo quindi di impostare il campo "**Valore Quantità**" a 5,
> ogni articolo messo in vendita tramite l'Inserzione in esame verrà
> pubblicato e sarà quindi disponibile sul relativo Marketplace in
> quantità pari a 5

- **Quantità in magazzino:** selezionando questa opzione sarà poi
  possibile impostare la quantità con cui gli articoli dovranno essere
  pubblicati sul relativo Marketplace, come una percentuale della
  quantità in cui gli stessi articoli sono effettivamente disponibili
  all'interno dei magazzini definiti in fase di configurazione
  dell'Account collegato all' Inserzione.

> Per maggiori informazioni relativamente a come definire i magazzini
> associati ad un Account Amazon si veda anche la sezione "*Amazon --
> Gestione Account"* di questo manuale.
>
> **ATTENZIONE!** Nel valutare quella che per Passweb è la quantità
> effettiva di un certo articolo su di un determinato magazzino occorre
> sempre tener conto di quanto impostato alla pagina "**Catalogo --
> Configurazione Parametri Catalogo**" all'interno della sezione
> "Disponibilità" sia in termini di formula utilizzata per il calcolo
> della disponibilità che in termini di Scorta Minima
>
> In queste condizioni sarà quindi necessario impostare un valore anche
> per i seguenti campi:

![](./assets/media/image234.png)

- **Percentuale della Quantità:** consente di impostare, selezionandola
  dall'apposito menu a tendina, la percentuale di articoli
  effettivamente disponibili sul magazzino collegato all'Account che
  dovranno poi essere pubblicati e resi disponibili all'interno del
  Marketplace

- **Quantità condizionale:** consente di abilitare/disabilitare la
  pubblicazione degli articoli sul marketplace, in relazione al fatto
  che la quantità determinata sulla base della percentuale di articoli
  disponibili nel magazzino collegato all'Account soddisfi determinate
  specifiche.

> Nel momento in cui il parametro "Quantità condizionale" dovesse quindi
> essere impostato sul valore "Abilitata" verranno visualizzati due
> ulteriori campi, "Quantità minima di vendita" e "Quantità massima di
> vendita" mediante i quali poter rispettivamente:

- **Quantità minima di vendita:** consente di impostare la soglia minima
  che la percentuale indicata per gli articoli disponibili nel magazzino
  collegato all'Account dovrà necessariamente superare affinchè questi
  stessi articoli possano essere effettivamente pubblicati e resi
  disponibili anche sul Marketplace

- **Quantità massima di vendita:** consente di impostare la quantità
  massima con cui gli articoli potranno essere resi disponibili sul
  Marketplace indipendentemente da quello che è il valore della
  percentuale per essi indicata mediante il precedente parametro
  "Percentuale della Quantità"

**ATTENZIONE! la quantità di pubblicazione degli articoli calcolata
mediante i parametri impostati all'interno di questa sezione verrà
utilizzata come valore di default per tutti gli articoli venduti
mediante l'Inserzione in esame.**

In ogni caso sarà comunque possibile intervenire in fase di
pubblicazione e modificare manualmente la quantità di pubblicazione di
ogni singolo articolo coinvolto nell'inserzione (per maggiori
informazioni in merito si veda anche il successivo capitolo "Gestione
lista di vendita e pubblicazione su Amazon")

**ATTENZIONE! Eventuali modifiche alle impostazioni per il calcolo della
quantità di pubblicazione avranno effetto solo ed esclusivamente sui
nuovi articoli aggiunti alla lista collegata all'Inserzione in esame**
(le quantità di pubblicazione degli articoli già presenti in lista non
verranno quindi variate in alcun modo)

Per meglio comprendere il significato e l'utilizzo dei parametri appena
analizzati si considerino anche i seguenti esempi:

**[ESEMPIO 1]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace determinati articoli
sempre e solamente in quantità unitaria

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità" nel seguente modo:

Quantità = Singolo Oggetto

oppure

Quantità = Valore Personalizzato

Valore della Quantità = 1

**[ESEMPIO 2]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace determinati articoli
sempre e solamente in quantità pari a 5

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità" nel seguente modo:

- Quantità = Valore Personalizzato

- Valore della Quantità = 5

**[ESEMPIO 3]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace gli articoli
coinvolti nell'Inserzione in una quantità pari al **20%** della loro
effettiva disponibilità sul Magazzino associato all'Account che si sta
utilizzando

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità" nel seguente modo:

- Quantità = Quantità in magazzino

- Percentuale della Quantità = 20%

- Quantità Condizionale = Disabilitata

Supponendo che la disponibilità definita alla pagina "*Catalogo --
Configurazione Parametri Catalogo*" del Wizard sia stata impostata sulla
formula

- Esistenza = Inventario + Carico -- Scarico

e che un determinato articolo coinvolto nell'inserzione **abbia
esistenza pari a 80** nel magazzino associato all'Account, in queste
condizioni **questo stesso articolo verrà pubblicato sul Marketplace in
quantità pari a 16** (ossia esattamente il 20% della sua disponibilità
attuale)

**[ESEMPIO 3]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace gli articoli
coinvolti nell'Inserzione in una quantità pari al **20%** della loro
effettiva disponibilità sul Magazzino associato all'Account che si sta
utilizzando, rispettando però i vincoli di non pubblicarne mai una
quantità superiore a 20 e inferiore a 10

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità" nel seguente modo:

- Quantità = Quantità in magazzino

- Percentuale della Quantità = 20%

- Quantità Condizionale = Abilitata

- Quantità minima di vendita = 10

- Quantità massima di vendita = 20

Supponiamo, anche in questo caso, che la disponibilità definita alla
pagina "*Catalogo -- Configurazione Parametri Catalogo*" del Wizard sia
stata impostata sulla formula

- Esistenza = Inventario + Carico -- Scarico

Supponiamo inoltre di voler pubblicare sul Marketplace 3 distinti
articoli che, nel magazzino associato all'Account utilizzato, hanno
attualmente le seguenti esistenze:

- **Articolo-A 🡪** Esistenza = 80

- **Articolo-B 🡪** Esistenza = 200

- **Articolo-C 🡪** Esistenza = 40

In queste condizioni

In queste condizioni si otterranno i seguenti risultati:

- **Articolo-A** 🡪 Pubblicato sul Marketplace in quantità pari a 16
  (ossia esattamente il 20% della sua disponibilità attuale)

- **Articolo-B 🡪** Pubblicato sul Marketplace in quantità pari a 20.
  Considerando infatti che il 20% della sua disponibilità attuale
  sarebbe pari a 40 questo andrebbe oltre il limite impostato
  all'interno del campo "Quantità massima di vendita" per cui anche se
  il 20% della sua disponibilità attuale è effettivamente pari a 40
  unità, l'articolo verrà comunque pubblicato sul marketplace in
  quantità pari a 20

- **Articolo-C 🡪** Non Pubblicato sul Marketplace in conseguenza del
  fatto che il 20% della sua disponibilità attuale è pari a 8 unità
  calore questo che non supera la soglia di 10 unità impostata
  all'interno del campo "Quantità minima di vendita"

###### PREZZO DEGLI ARTICOLI PUBBLICATI

All'interno della sezione **"Prezzo"** è possibile definire esattamente
il prezzo con cui dovranno essere messi in vendita, sul marketplace
Amazon, gli articoli collegati all'Inserzione che si sta considerando.

![](./assets/media/image235.png)

In questo senso il campo:

**Prezzo:** consente di indicare lo specifico listino del gestionale che
dovrà essere utilizzato per determinare il prezzo degli articoli messi
in vendita mediante l'Inserzione in esame.

Nel caso di siti Ecommerce collegati a Mexal è possibile, come
evidenziato nei precedenti capitoli di questo manuale, mettere in
vendita articoli anche su marketplace Amazon che gestiscono valute
diverse dall'euro.

In queste condizioni, la conversione nella valuta di gestione del
marketplace, dei prezzi determinati dal listino indicato all'interno del
campo in esame verrà effettuata secondo i fattori di conversione
definiti nella corrispondente tabella Mexal

**Modifica del Prezzo:** consente di modificare il prezzo con cui gli
articoli coinvolti nell'Inserzione verranno pubblicati sul marketplace
rispetto a quello che è il loro prezzo attuale definito dal listino
gestionale impostato all'interno del precedente parametro.

Sono accettati i seguenti valori:

- **0:** in queste condizioni il prezzo degli articoli coinvolti
  nell'Inserzione coinciderà esattamente con il loro prezzo di listino

- **Valori decimali privi di segno (es. 2.5):** in queste condizioni il
  prezzo di listino degli articoli coinvolti nell'Inserzione verrà
  moltiplicato per il valore inserito.

> Supponendo dunque di inserire all'interno di questo campo i valori:

- 1 🡪 Il prezzo di pubblicazione dell'articolo sarà esattamente il suo
  prezzo di listino

- 2 🡪 Il prezzo di pubblicazione dell'articolo sarà esattamente il
  doppio del suo prezzo di listino

- 0.5 🡪 Il prezzo di pubblicazione dell'articolo sarà esattamente la
  metà del suo prezzo di listino

<!-- -->

- **Valori fissi con segno + o -- (es. +3 oppure -5):** in queste
  condizioni il prezzo di listino degli articoli coinvolti
  nell'Inserzione verrà maggiorato/diminuito esattamente del valore
  indicato

> Supponendo dunque di inserire all'interno di questo campo i valori:

- +3 Il prezzo di pubblicazione dell'articolo sarà maggiorato di 3 €
  rispetto al suo prezzo di listino

- -5 Il prezzo di pubblicazione dell'articolo sarà diminuito di 5 €
  rispetto al suo prezzo di listino

##### SINCRONIZZAZIONE

All'intero di questa sezione è possibile attivare/disattivare
determinate regole mediante le quali poter automatizzare:

- **La pubblicazione** sul Marketplace degli articoli coinvolti
  nell'Inserzione in esame -- sezione "**Regole di Messa in Vendita**"

- **L' interruzione della pubblicazione** sul Marketplace degli articoli
  coinvolti nell'Inserzione in esame -- sezione "**Regole di Blocco**"

- **La ripubblicazione** degli articoli coinvolti nell'inserzione in
  esame, **che erano già stati pubblicati sul Marketplace** ma per i
  quali era stata precedentemente arrestata (manualmente o
  automaticamente) la messa in vendita -- sezione "**Regole di Rimessa
  in Vendita**"

![](./assets/media/image236.png)

In questo senso la sezione "**Metodo di Sincronizzazione**" consente di
decidere se adottare uno dei Template precedentemente codificati (e
magari già utilizzato in qualche altra inserzione) oppure realizzarne
uno nuovo.

Nel primo caso (applicazione di un Template preconfigurato) sarà
sufficiente selezionare il Template desiderato tra quelli presenti
all'interno dell'apposito menu a tendina.

Nel secondo caso (definizione di nuovi parametri per quantità prezzo e
formato) sarà sufficiente settare il campo "**Metodo di
Sincronizzazione**" sull'opzione "**Custom"** e procedere poi alla
configurazione dei restanti parametri presenti all'interno della pagina.

In questo caso inoltre, una volta impostati e salvati correttamente
tutti i valori verrà automaticamente creato anche un nuovo Template
(visualizzabile e gestibile all'interno della maschera "**Lista dei
Metodi di Sincronizzazione**" precedentemente analizzata) con il nome
dell'Inserzione che si sta realizzando.

###### REGOLE DI MESSA IN VENDITA

All'intero di questa sezione è possibile definire un' insieme di
condizioni in relazione alle quali poter automatizzare la pubblicazione
sul Marketplace degli articoli coinvolti nell'Inserzione in esame

![](./assets/media/image237.png)

Nello specifico per quel che riguarda le "**Regole di Messa in
Vendita**" il campo:

- **Messa in Vendita:** consente di abilitare / disabilitare
  l'attivazione delle condizioni di pubblicazione automatica degli
  articoli sul Marketplace.

> E' possibile selezionare uno dei seguenti valori:

- **Abilitata:** in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale (Parziale o Totale) verranno valutate le condizioni
  definite nei successivi campi e gli articoli coinvolti nell'Inserzione
  che dovessero soddisfare tali condizioni verranno automaticamente
  pubblicati all'interno del marketplace.

- **Non Abilitata:** in queste condizioni non verrà applicata nessuna
  regola automatica, per cui gli articoli coinvolti nell'Inserzione
  potranno essere pubblicati all'interno del Marketplace solo ed
  esclusivamente in maniera manuale

<!-- -->

- **Stato dell'Articolo:** consente di decidere se l'applicazione delle
  regole automatiche di messa in vendita deve essere relativa o meno ai
  soli articoli effettivamente pubblicati all'interno del proprio sito
  ecommerce:

> E' possibile selezionare uno dei seguenti valori:

- **Pubblicato**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul
  Marketplace, tra tutti gli articoli coinvolti nell'Inserzione,
  solamente quelli per i quali il campo "**Pubblica**" è stato impostato
  a **SI**

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente alla funzionalità di
> Pubblicazione legate al campo "Pubblica" si vedano anche i capitoli
> "*Configurazione Gestionale -- Mexal Parametri configurazione
> gestionale -- Mexal Attivazione Passweb -- Funzionalità Mexal Articoli
> -- Pubblicare / Nascondere articoli all'interno del sito*" e
> "Configurazione Gestionale -- *Ho.Re.Ca. Parametri configurazione
> gestionale -- Funzionalità di gestione articoli - Pubblicare /
> Nascondere articoli all'interno del sito* " di questo manuale

- **Disponibilità in magazzino:** consente di decidere se l'applicazione
  delle regole automatiche di messa in vendita deve essere relativa o
  meno ai soli articoli effettivamente disponibili nel magazzino
  associato all'Account che si sta utilizzando.

> E' possibile selezionare uno dei seguenti valori:

- **In Magazzino**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  pubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli che risultano essere effettivamente
  disponibili (disponibilità maggiore di 0) sul magazzino associato
  all'Account che si sta utilizzando

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente a come poter associare uno
> specifico magazzino all'Account utilizzato per pubblicare articoli sul
> Marketplace si veda anche la sezione "*Amazon -- Gestione Account*" di
> questo manuale.
>
> Si ricorda inoltre che la disponibilità sul magazzino verrà valutata
> sulla base della formula impostata all'interno dell'omonimo campo
> presente alla pagina "*Catalogo -- Configurazione Parametri Catalogo*"
> del Wizard

- **Quantità nel magazzino:** consente di decidere se l'applicazione
  delle regole automatiche di messa in vendita deve essere relativa o
  meno ai soli articoli coinvolti nell'Inserzione che risultino essere
  disponibili in una certa quantità all'interno del magazzino associato
  all'Account che si sta utilizzando

> E' possibile selezionare uno dei seguenti valori:

- **Maggiore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  pubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli per i quali la quantità disponibile
  nel magazzino associato all'Account che si sta utilizzando è maggiore
  o uguale al valore impostato nel successivo campo "**Quantità**"

- **Tra il**: : in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  tra tutti gli articoli coinvolti nell'Inserzione, solamente quelli per
  i quali la quantità disponibile nel magazzino associato all'Account
  che si sta utilizzando è compresa nel range di valori definito nei
  successivi campi "**Quantità** **minima**" e "**Quantità**
  **massima**".

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  tutti gli articoli coinvolti nell'Inserzione.

<!-- -->

- **Quantità calcolata:** consente di decidere se l'applicazione delle
  regole automatiche di messa in vendita deve essere relativa o meno ai
  soli articoli coinvolti nell'Inserzione per i quali la quantità da
  pubblicare all'interno del marketplace soddisfi determinate
  condizioni.

> E' possibile selezionare uno dei seguenti valori:

- **Maggiore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  pubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli che dovranno essere effettivamente
  pubblicati in una quantità maggiore o uguale al valore impostato nel
  successivo campo "**Quantità**"

- **Tra il**: : in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  , tra tutti gli articoli coinvolti nell'Inserzione, solamente quelli
  che dovranno essere effettivamente pubblicati in una quantità compresa
  nel range di valori definito nei successivi campi "**Quantità**
  **minima**" e "**Quantità** massima".

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente pubblicati sul Marketplace
  tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente a come determinare, per gli
> articoli coinvolti nell' Inserzione, quella che dovrà essere la loro
> quantità di pubblicazione si veda anche il precedente capitolo
> ("*Prezzo Quantità Formato*") di questo manuale

**ATTENZIONE! Le condizioni di messa in vendita automatica definite
mediante i parametri sopra analizzati sono in AND tra loro. Per avviare
la messa in vendita automatica degli articoli coinvolti nell'Inserzione
è necessario quindi che tutte le condizioni impostate siano
soddisfatte**

Nel caso in cui per un determinato articolo coinvolto nell'inserzione
una o più condizioni non dovessero essere verificate tale articolo non
rientrerà tra quelli messi in vendita automaticamente alla
sincronizzazione Sito -- Gestionale

###### REGOLE DI MODIFICA IN VENDITA

All'interno di questa sezione è possibile decidere se, ed eventualmente
in che termini dovranno essere aggiornati a seguito di una
sincronizzazione Sito -- Gestionale, gli articoli pubblicati mediante
l'inserzione in esame.

![](./assets/media/image238.png)

Nello specifico dunque il campo:

**Modifica in Vendita:** consente di abilitare / disabilitare, in fase
di sincronizzazione Sito -- Gestionale, l'aggiornamento automatico, sul
relativo marketplace, degli articoli pubblicati mediante l'inserzione in
esame.

Ovviamente le impostazioni settate all'interno delle successive sezioni
"Condizioni -- Modifiche Parziali**"** e "Condizioni -- Modifiche
Totali" avranno effetto solo nel caso in cui il parametro in esame sia
stato impostato sul valore "**Abilitata**"

All'interno della sezione "**Condizioni -- Modifiche Parziali**" è
possibile impostare delle regole mediante le quali poter definire se a
seguito di una sincronizzazione Sito -- Gestionale, dovranno essere
aggiornati anche sul relativo marketplace **la Quantità e / o il
Prezzo** degli articoli pubblicati mediante l'Inserzione in esame.

In questo senso dunque il campo:

- **Quantità:** consente di decidere se a seguito di una
  sincronizzazione Sito -- Gestionale dovrà essere aggiornata, anche sul
  relativo marketplace, **la Quantità** degli articoli pubblicati
  mediante l'Inserzione in esame.

> E' possibile selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione, a seguito di una sincronizzazione
  Sito -- Gestionale **non verrà mai aggiornata** la quantità degli
  articoli pubblicati sul relativo marketplace mediante l'inserzione in
  esame.

- **Si:** selezionando questa opzione, nel momento in cui a seguito di
  una Sincronizzazione Sito -- Gestionale la quantità (su Passweb) di un
  determinato articolo coinvolto nell'inserzione dovesse risultare
  variata rispetto alla sincronizzazione precedente o non allineata con
  la quantità attualmente disponibile sul marketplace, potrebbe partire
  la procedura di aggiornamento automatico della relativa quantità anche
  sul marketplace.

> **ATTENZIONE!** in queste condizioni l'effettivo aggiornamento della
> quantità sul marketplace dipenderà direttamente da come verrà
> impostato il successivo parametro

- **Condizione Quantità**: consente di decidere se l'aggiornamento della
  quantità sul marketplace dovrà avvenire a prescindere o solo al
  verificarsi di una determinata condizione. Ovviamente le impostazioni
  di questo campo avranno senso solo ed esclusivamente nel caso in cui
  il precedente parametro "Quantità" sia stato impostato sul valore Si.

> E' possibile selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione nel momento in cui a seguito di
  una Sincronizzazione Sito -- Gestionale la quantità di un determinato
  articolo coinvolto nell'inserzione dovesse risultare variata (su
  Passweb) rispetto alla sincronizzazione precedente **verrà sempre
  eseguita** la procedura di aggiornamento automatico della relativa
  quantità anche sul marketplace

- **Si:** selezionando questa opzione la procedura di aggiornamento
  automatico della relativa quantità sul marketplace verrà eseguita
  **solo ed esclusivamente nel caso in cui la quantità dell'articolo che
  dovrebbe essere effettivamente pubblicata sulla marketplace risulti
  essere minore o uguale a quella impostata nel successivo campo
  "Modifica quando la Quantità è inferiore o uguale a"**

<!-- -->

- **Modifica quando la Quantità è inferiore o uguale a:** visibile solo
  nel caso in cui il precedente parametro sia stato impostato sul valore
  Si. Consente di impostare, per gli articoli coinvolti nell'inserzione
  in esame, il valore della quantità sulla base del quale determinare se
  dovrà o meno essere lanciata la procedura di aggiornamento della
  relativa quantità anche sul marketplace

> Facendo riferimento alle impostazioni visualizzate in figura

![](./assets/media/image239.png)

> supponendo che nell'Inserzione siano coinvolti gli articoli ARTA,
> ARTB, ARTC e che a seguito di una sincronizzazione la quantità di
> questi articoli risultino variate rispetto la sincronizzazione
> precedente assumendo ora i seguenti valori:
>
> Quantità su Passweb di ARTA dopo la sincronizzazione = 4
>
> Quantità su Passweb di ARTB dopo la sincronizzazione = 3
>
> Quantità su Passweb di ARTC dopo la sincronizzazione = 2
>
> Quello che si otterrà è che a seguito della sincronizzazione in esame
> verrà aggiornata sul marketplace la quantità degli articoli ARTB e
> ARTC ma non quella dell'articolo ARTA
>
> **ATTENZIONE!** Nel valutare quella che per Passweb è la quantità
> effettiva di un certo articolo su di un determinato magazzino occorre
> sempre tener conto di quanto impostato alla pagina "**Catalogo --
> Configurazione Parametri Catalogo**" all'interno della sezione
> "Disponibilità" sia in termini di formula utilizzata per il calcolo
> della disponibilità che in termini di Scorta Minima

**ATTENZIONE! A seguito dell'applicazione di una regola di "Modifica
parziale" della quantità verrà eseguita una transazione di tipo
"Quantità" che provvederà ad aggiornare sulla piattaforma terza, la sola
quantità degli articoli coinvolti**

Così come i parametri appena analizzati determinano le regole di
modifica della sola quantità degli articoli pubblicati mediante
l'inserzione in esame, allo stesso modo i successivi parametri della
sezione "**Condizioni -- Modifiche Parziali**" determinano invece le
regole di modifica relative solo al prezzo degli articoli pubblicati sul
marketplace.

In particolare dunque il campo:

- **Prezzo:** consente di decidere se a seguito di una sincronizzazione
  Sito -- Gestionale dovrà essere aggiornato, anche sul relativo
  marketplace, **il Prezzo** degli articoli pubblicati mediante
  l'Inserzione in esame.

> E' possibile selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione, a seguito di una sincronizzazione
  Sito -- Gestionale **non verrà mai aggiornato** il prezzo degli
  articoli pubblicati sul relativo marketplace mediante l'inserzione in
  esame.

- **Si:** selezionando questa opzione, nel momento in cui a seguito di
  una Sincronizzazione Sito -- Gestionale il prezzo di un determinato
  articolo coinvolto nell'inserzione dovesse risultare variato (su
  Passweb) rispetto alla sincronizzazione precedente potrebbe partire la
  procedura di aggiornamento automatico del prezzo anche sul
  marketplace.

> **ATTENZIONE!** in queste condizioni l'effettivo aggiornamento del
> prezzo sul marketplace dipenderà direttamente da come verrà impostato
> il successivo parametro

- **Condizione Prezzo**: consente di decidere se l'aggiornamento del
  prezzo sul marketplace dovrà avvenire a prescindere o solo al
  verificarsi di una determinata condizione. Ovviamente le impostazioni
  di questo campo avranno senso solo ed esclusivamente nel caso in cui
  il precedente parametro "Prezzo" sia stato impostato sul valore Si.

> E' possibile selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione nel momento in cui a seguito di
  una Sincronizzazione Sito -- Gestionale il prezzo di un determinato
  articolo coinvolto nell'inserzione dovesse risultare variato (su
  Passweb) rispetto alla sincronizzazione precedente **verrà sempre
  eseguita** la procedura di aggiornamento automatico del prezzo anche
  sul marketplace

- **Si:** selezionando questa opzione la procedura di aggiornamento
  automatico del prezzo sul marketplace verrà eseguita **solo ed
  esclusivamente nel caso in cui il prezzo dell'articolo su Passweb
  dovesse aver subito una variazione (in positivo o in negativo)
  maggiore o uguale alla percentuale indicata all'interno del successivo
  campo "Modifica quando il Prezzo è superiore o uguale a"**

<!-- -->

- **Modifica quando il Prezzo è superiore o uguale a:** visibile solo
  nel caso in cui il precedente parametro sia stato impostato sul valore
  Si. Consente di impostare, per gli articoli coinvolti nell'inserzione
  in esame, il differenziale di prezzo sulla base del quale determinare
  se dovrà o meno essere lanciata la procedura di aggiornamento del
  prezzo anche sul marketplace

> **[Esempio:]{.underline}**
>
> Facendo riferimento alle impostazioni visualizzate in figura

![](./assets/media/image240.png)

> supponiamo che nell'Inserzione siano coinvolti gli articoli ARTA e
> ARTB e che a seguito di una sincronizzazione il prezzo di questi
> articoli risulti variato rispetto la sincronizzazione precedente come
> indicato in tabella

  --------------------------------------------------------------------
             **PREZZO          **PREZZO DOPO     **VARIAZIONE PREZZO**
             INIZIALE**        SINNCRO**         
  ---------- ----------------- ----------------- ---------------------
  **ARTA**   23.25 €           23.26 €           0.01 €

  **ARTB**   24 €              24.50 €           0.50 €
  --------------------------------------------------------------------

> Ora, avendo impostato il campo "Modifica quando il Prezzo è superiore
> o uguale a" sul valore 1%, il differenziale cui far riferimento per i
> due articoli sarà rispettivamente di
>
> Differenziale ARTA 🡪 **0.23 €**
>
> Differenziale ARTB 🡪 **0.24 €**
>
> In definitiva dunque la variazione di prezzo subita dall'articolo ARTA
> (di 0.01€) è inferiore al suo differenziale (di 0.23€) e quindi a
> seguito della sincronizzazione il prezzo di questo articolo sul
> marketplace resterà invariato.
>
> Al contrario la variazione di prezzo subita dall'articolo ARTB (di
> 0.50€) è superiore al suo differenziale (di 0.24 €) per cui a seguito
> della sincronizzazione il prezzo dell'articolo ARTB verrà aggiornato
> anche sul marketplace.

**ATTENZIONE! A seguito dell'applicazione di una regola di "Modifica
parziale" del prezzo verrà eseguita una transazione di tipo "Prezzo" che
provvederà ad aggiornare sulla piattaforma terza, il solo prezzo degli
articoli coinvolti**

In definitiva dunque, le regole impostate all'interno della sezione
"Condizioni -- Modifiche Parziali" possono determinare, eventualmente,
**un aggiornamento automatico dei soli campi Quantità e/o Prezzo**.
Tutte le altre informazioni dei prodotti pubblicati sul Marketplace
mediante l'Inserzione in esame non verranno modificate in alcun modo a
seguito dell'applicazione di queste regole

All'interno della sezione "**Condizioni -- Modifiche Totali**" è invece
possibile decidere come comportarsi nel momento in cui a seguito di una
sincronizzazione Sito -- Gestionale l'applicazione dovesse rilevare una
modifica al "Metodo di Quantità, Prezzo e Formato" o al "Metodo di
Descrizione" utilizzato nell'Inserzione in esame.

![](./assets/media/image241.png)

In particolare dunque il campo:

**Metodi di Descrizione**: permette di decidere come comportarsi nel
momento in cui a seguito di una sincronizzazione Sito -- Gestionale
l'applicazione dovesse rilevare una modifica al "Metodo di descrizione"
utilizzato nell'Inserzione in esame (per maggiori informazioni in merito
alla creazione di un "Metodo di Descrizione" e alla sua associazione ad
una determinata Inserzione si vedano i precedenti capitoli di questo
manuale)

E' possibile selezionare uno dei seguenti valori:

- **Si:** selezionando questa opzione nel momento in cui a seguito di
  una sincronizzazione Sito -- Gestionale Passweb dovesse rilevare una
  modifica, rispetto alla sincronizzazione precedente, ad uno qualsiasi
  dei campi presenti nel "Metodo di Descrizione" utilizzato per
  l'Inserzione in esame, **verrà eseguita automaticamente la procedura
  di aggiornamento sul marketplace di tutti i campi di tutti gli
  articoli coinvolti nell'Inserzione in esame**

- **No:** selezionando questa opzione se anche, a seguito di una
  sincronizzazione Sito -- Gestionale, dovesse essere rilevata una
  modifica, rispetto alla sincronizzazione precedente, ad uno qualsiasi
  dei campi presenti nel "Metodo di Descrizione" utilizzato per
  l'Inserzione in esame **non verrà comunque lanciata nessuna procedura
  di aggiornamento automatico** dei dati sul marketplace. In queste
  condizioni dunque i campi degli articoli pubblicati sul marketplace
  potrebbero continuare ad avere, anche dopo la sincronizzazione, gli
  stessi valori

**Metodi di Prezzo, quantità e formato**: permette di decidere come
comportarsi nel momento in cui a seguito di una sincronizzazione Sito --
Gestionale l'applicazione dovesse rilevare una modifica al "Metodo di
quantità prezzo e formato" utilizzato nell'Inserzione in esame (per
maggiori informazioni in merito alla creazione di un "Metodo di quantità
prezzo e formato" e alla sua associazione ad una determinata Inserzione
si vedano i precedenti capitoli di questo manuale)

E' possibile selezionare uno dei seguenti valori:

- **Si:** selezionando questa opzione nel momento in cui a seguito di
  una sincronizzazione Sito -- Gestionale Passweb dovesse rilevare una
  modifica, rispetto alla sincronizzazione precedente, ad uno qualsiasi
  dei campi presenti nel "Metodo di quantità prezzo e formato"
  utilizzato per l'Inserzione in esame, **verrà eseguita automaticamente
  la procedura di aggiornamento sul marketplace di tutti i campi di
  tutti gli articoli coinvolti nell'Inserzione in esame**

- **No:** selezionando questa opzione se anche, a seguito di una
  sincronizzazione Sito -- Gestionale, dovesse essere rilevata una
  modifica, rispetto alla sincronizzazione precedente, ad uno qualsiasi
  dei campi presenti nel "Metodo di Descrizione" utilizzato per
  l'Inserzione in esame **non verrà comunque lanciata nessuna procedura
  di aggiornamento automatico** dei dati sul marketplace. In queste
  condizioni dunque i campi degli articoli pubblicati sul marketplace
  potrebbero continuare ad avere, anche dopo la sincronizzazione, gli
  stessi valori

**ATTENZIONE! A seguito dell'applicazione di una regola di "Modifica
totale" verrà eseguita una transazione di tipo "Modifica" che provvederà
ad aggiornare sulla piattaforma terza, per gli articoli coinvolti, tutte
le specifiche gestite nella relativa Inserzione (oltre eventualmente a
quantità e prezzo)**

###### REGOLE DI RIMESSA IN VENDITA

All'intero di questa sezione è possibile definire un' insieme di
condizioni in relazione alle quali poter automatizzare la
ripubblicazione degli articoli coinvolti nell'inserzione in esame.

**ATTENZIONE! Con il termine "ripubblicazione" si intende definire una
nuova pubblicazione di quegli articoli che erano già stati pubblicati
sul Marketplace e per i quali però era stata precedentemente arrestata
(manualmente o automaticamente) la messa in vendita.**

In altri termini dunque, mentre l'operazione di pubblicazione è relativa
a quegli articoli che non si trovano attualmente sul Marketplace, la
ripubblicazione o rimessa in vendita, è un'operazione relativa invece ai
soli articoli che, pur essendo ancora all'interno del Marketplace, non
possono attualmente essere acquistati.

![](./assets/media/image242.png)

Per quel che riguarda le "**Regole di Rimessa in Vendita**" il campo:

- **Rimessa in Vendita:** consente di abilitare / disabilitare
  l'attivazione delle condizioni di ripubblicazione automatica degli
  articoli sul Marketplace.

> E' possibile selezionare uno dei seguenti valori:

- **Abilitata:** in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale (Parziale o Totale) verranno valutate le condizioni
  definite nei successivi campi e gli articoli coinvolti nell'Inserzione
  che dovessero soddisfare tali condizioni verranno automaticamente
  ripubblicati all'interno del marketplace.

- **Non Abilitata:** in queste condizioni non verrà applicata nessuna
  regola automatica, per gli articoli coinvolti nell'Inserzione potranno
  eventualmente essere ripubblicati all'interno del Marketplace solo ed
  esclusivamente in maniera manuale

<!-- -->

- **Inviare Feed Prezzo:** se attivato, consente di aggiornare, in fase
  di ripubblicazione degli articoli, anche il loro prezzo

> **ATTENZIONE!** Nel caso in cui il parametro in questione non dovesse
> essere attivato, in fase di ripubblicazione degli articoli verrà
> aggiornata, sul relativo marketplace, solo ed esclusivamente la loro
> quantità

- **Stato dell'Articolo:** consente di decidere se l'applicazione delle
  regole automatiche di rimessa in vendita deve essere relativa o meno
  ai soli articoli effettivamente pubblicati all'interno del proprio
  sito ecommerce:

> E' possibile selezionare uno dei seguenti valori:

- **Pubblicato**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace, tra tutti gli articoli coinvolti nell'Inserzione,
  solamente quelli per i quali il campo "**Pubblica**" è stato impostato
  a **SI**

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente alla funzionalità di
> Pubblicazione legate al campo "Pubblica" si vedano anche i capitoli
> "*Configurazione Gestionale -- Mexal Parametri configurazione
> gestionale -- Mexal Attivazione Passweb -- Funzionalità Mexal Articoli
> -- Pubblicare / Nascondere articoli all'interno del sito*" e
> "Configurazione Gestionale -- *Ho.Re.Ca. Parametri configurazione
> gestionale -- Funzionalità di gestione articoli - Pubblicare /
> Nascondere articoli all'interno del sito* " di questo manuale.

- **Disponibilità in magazzino:** consente di decidere se l'applicazione
  delle regole automatiche di rimessa in vendita deve essere relativa o
  meno ai soli articoli effettivamente disponibili nel magazzino
  associato all'Account che si sta utilizzando.

> E' possibile selezionare uno dei seguenti valori:

- **In Magazzino**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  ripubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli che risultano essere effettivamente
  disponibili (disponibilità maggiore di 0) sul magazzino associato
  all'Account che si sta utilizzando

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente a come poter associare uno
> specifico magazzino all'Account utilizzato per pubblicare articoli sul
> Marketplace si veda anche la sezione "*Amazon -- Gestione Account*" di
> questo manuale.
>
> Si ricorda inoltre che la disponibilità sul magazzino verrà valutata
> sulla base della formula impostata all'interno dell'omonimo campo
> presente alla pagina "*Catalogo -- Configurazione Parametri Catalogo*"
> del Wizard

- **Quantità nel magazzino:** consente di decidere se l'applicazione
  delle regole automatiche di rimessa in vendita deve essere relativa o
  meno ai soli articoli coinvolti nell'Inserzione che risultino essere
  disponibili in una certa quantità all'interno del magazzino associato
  all'Account che si sta utilizzando

> E' possibile selezionare uno dei seguenti valori:

- **Maggiore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  ripubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli per i quali la quantità disponibile
  nel magazzino associato all'Account che si sta utilizzando è maggiore
  o uguale al valore impostato nel successivo campo "**Quantità**"

- **Tra il**: : in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace tra tutti gli articoli coinvolti nell'Inserzione,
  solamente quelli per i quali la quantità disponibile nel magazzino
  associato all'Account che si sta utilizzando è compresa nel range di
  valori definito nei successivi campi "**Quantità** **minima**" e
  "**Quantità** **massima**".

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace tutti gli articoli coinvolti nell'Inserzione.

<!-- -->

- **Quantità calcolata:** consente di decidere se l'applicazione delle
  regole automatiche di rimessa in vendita deve essere relativa o meno
  ai soli articoli coinvolti nell'Inserzione per i quali la quantità da
  pubblicare all'interno del marketplace soddisfi determinate
  condizioni.

> E' possibile selezionare uno dei seguenti valori:

- **Maggiore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verranno automaticamente
  ripubblicati sul Marketplace, tra tutti gli articoli coinvolti
  nell'Inserzione, solamente quelli che dovranno essere effettivamente
  pubblicati in una quantità maggiore o uguale al valore impostato nel
  successivo campo "**Quantità**"

- **Tra il**: : in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace , tra tutti gli articoli coinvolti nell'Inserzione,
  solamente quelli che dovranno essere effettivamente pubblicati in una
  quantità compresa nel range di valori definito nei successivi campi
  "**Quantità** **minima**" e "**Quantità** massima".

- **Qualsiasi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verranno automaticamente ripubblicati sul
  Marketplace tutti gli articoli coinvolti nell'Inserzione.

> Per maggiori informazioni relativamente a come determinare, per gli
> articoli coinvolti nell' Inserzione, quella che dovrà essere la loro
> quantità di pubblicazione si veda anche il precedente capitolo
> ("*Prezzo Quantità Formato*") di questo manuale

**ATTENZIONE! Le condizioni di rimessa in vendita automatica definite
mediante i parametri sopra analizzati sono in AND tra loro. Per avviare
la rimessa in vendita automatica degli articoli coinvolti
nell'Inserzione è necessario quindi che tutte le condizioni impostate
siano soddisfatte**

Nel caso in cui per un determinato articolo coinvolto nell'inserzione
una o più condizioni non dovessero essere verificate tale articolo non
rientrerà tra quelli che alla sincronizzazione Sito -- Gestionale
verranno rimessi automaticamente in vendita

###### REGOLE DI BLOCCO

All'intero di questa sezione è possibile attivare/disattivare
determinate regole mediante le quali poter automatizzare l' interruzione
della pubblicazione sul Marketplace degli articoli coinvolti
nell'Inserzione in esame

**ATTENZIONE!** Interrompendo la pubblicazione di determinati articoli
all'interno del Marketplace questi non potranno più essere venduti ma
resteranno comunque presenti all'interno del marketplace stesso e, in
queste condizioni, potranno quindi essere soggetti ad eventuali regole
di rimessa in vendita.

![](./assets/media/image243.png)

A differenza delle condizioni definite nelle "Regole di messa in
vendita" e di quelle definite nelle "Regole di rimessa in vendita", le
**"Condizioni di Interruzione"** presenti all'interno di questa sezione
verranno sempre valutate singolarmente ad ogni sincronizzazione Sito --
Gestionale (sono quindi condizioni in OR).

In conseguenza di ciò nel momento in cui, per un certo articolo, dovesse
essere verificata anche una soltanto di queste condizioni, verrà
automaticamente interrotta la pubblicazione sul Marketplace
dell'articolo in questione.

Nello specifico dunque per quel che riguarda le condizioni di
interruzione presenti all'interno di questa sezione il campo

- **Quando l'articolo non è pubblicato:** consente di decidere se
  interrompere o meno, alla sincronizzazione, la pubblicazione degli
  articoli coinvolti nell'Inserzione per i quali il campo "**Pubblica**"
  è stato impostato a **NO**

> E' possibile selezionare uno dei seguenti valori:

- **Interrompi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verrà interrotta automaticamente la pubblicazione
  di tutti quegli articoli coinvolti nell'Inserzione per i quali il
  campo "**Pubblica**" è stato impostato a **NO**

- **Nessuna azione**: in queste condizioni alla sincronizzazione Sito --
  Gestionale non verrà eseguita, in relazione a questa specifica
  condizione di blocco, nessuna azione per cui anche nel momento in cui
  determinati articoli dovessero avere il campo "Pubblica" impostato a
  NO, questi resteranno comunque in vendita all'interno del Marketplace.

> Per maggiori informazioni relativamente alla funzionalità di
> Pubblicazione legate al campo "Pubblica" si vedano anche i capitoli
> "*Configurazione Gestionale -- Mexal Parametri configurazione
> gestionale -- Mexal Attivazione Passweb -- Funzionalità Mexal Articoli
> -- Pubblicare / Nascondere articoli all'interno del sito*" e
> "Configurazione Gestionale -- *Ho.Re.Ca. Parametri configurazione
> gestionale -- Funzionalità di gestione articoli - Pubblicare /
> Nascondere articoli all'interno del sito* " di questo manuale.

- **Quando l'articolo è esaurito:** consente di decidere se interrompere
  o meno, alla sincronizzazione, la pubblicazione degli articoli
  coinvolti nell'Inserzione che risultino essere a disponibilità minore
  o uguale a 0 sul magazzino associato all'Account che si sta
  utilizzando.

> E' possibile selezionare uno dei seguenti valori:

- **Interrompi**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verrà interrotta automaticamente la pubblicazione
  di tutti quegli articoli coinvolti nell'Inserzione che risultino
  essere a disponibilità minore o uguale a 0 sul magazzino associato
  all'Account che si sta utilizzando

- **Nessuna azione**: in queste condizioni alla sincronizzazione Sito --
  Gestionale non verrà eseguita, in relazione a questa specifica
  condizione di blocco, nessuna azione per cui anche nel momento in cui
  determinati articoli dovessero essere, sul magazzino associato
  all'Account che si sta utilizzando, a disponibilità 0 questi
  resteranno comunque in vendita all'interno del Marketplace

> Per maggiori informazioni relativamente a come poter associare uno
> specifico magazzino all'Account utilizzato per pubblicare articoli sul
> Marketplace si veda anche la sezione "*Amazon -- Gestione Account*" di
> questo manuale.
>
> **ATTENZIONE!** Nel valutare quella che per Passweb è la quantità
> effettiva di un certo articolo su di un determinato magazzino occorre
> sempre tener conto di quanto impostato alla pagina "**Catalogo --
> Configurazione Parametri Catalogo**" all'interno della sezione
> "Disponibilità" sia in termini di formula utilizzata per il calcolo
> della disponibilità che in termini di Scorta Minima

- **Quando la quantità nel magazzino è:** consente di decidere se
  interrompere o meno, alla sincronizzazione, la pubblicazione degli
  articoli coinvolti nell'Inserzione che risultino essere disponibili in
  una certa quantità all'interno del magazzino associato all'Account che
  si sta utilizzando

> E' possibile selezionare uno dei seguenti valori:

- **Minore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verrà automaticamente interrotta
  la pubblicazione sul Marketplace, di tutti gli articoli coinvolti
  nell'Inserzione, per i quali la quantità disponibile nel magazzino
  associato all'Account che si sta utilizzando è minore o uguale al
  valore impostato nel successivo campo "**Quantità**"

- **Tra il**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verrà automaticamente interrotta la pubblicazione
  sul Marketplace, di tutti gli articoli coinvolti nell'Inserzione, per
  i quali la quantità disponibile nel magazzino associato all'Account
  che si sta utilizzando è compresa nel range di valori definito nei
  successivi campi "**Quantità** **minima**" e "**Quantità**
  **massima**".

- **Nessuna Azione**: in queste condizioni alla sincronizzazione Sito --
  Gestionale non verrà eseguita, in relazione a questa specifica
  condizione di blocco, nessuna azione per cui gli articoli coinvolti
  nell'Inserzione resteranno in vendita all'interno del Marketplace
  indipendentemente da quella che è la loro disponibilità all'interno
  del magazzino associato all'Account che si sta utilizzando.

<!-- -->

- **Quando la quantità calcolata è:** consente di decidere se
  interrompere o meno, alla sincronizzazione, la pubblicazione degli
  articoli coinvolti nell'Inserzione in relazione a quella che è la
  quantità con cui questi stessi articoli dovrebbero essere messi in
  vendita all'interno del Marketplace

> E' possibile selezionare uno dei seguenti valori:

- **Minore o Uguale**: in queste condizioni a seguito di una
  sincronizzazione Sito -- Gestionale verrà automaticamente interrotta
  la pubblicazione sul Marketplace, di tutti gli articoli coinvolti
  nell'Inserzione per i quali la quantità con cui questi stessi articoli
  dovrebbero essere effettivamente messi in vendita all'interno del
  Marketplace risulti essere minore o uguale al valore impostato nel
  successivo campo "**Quantità**"

- **Tra il**: in queste condizioni a seguito di una sincronizzazione
  Sito -- Gestionale verrà automaticamente interrotta la pubblicazione
  sul Marketplace, di tutti gli articoli coinvolti nell'Inserzione per i
  quali la quantità con cui questi stessi articoli dovrebbero essere
  effettivamente messi in vendita all'interno del Marketplace risulti
  essere compresa nel range di valori definito nei successivi campi
  "**Quantità** **minima**" e "**Quantità** massima".

- **Nessuna Azione**: in queste condizioni alla sincronizzazione Sito --
  Gestionale non verrà eseguita, in relazione a questa specifica
  condizione di blocco, nessuna azione per cui gli articoli coinvolti
  nell'Inserzione resteranno in vendita all'interno del Marketplace
  indipendentemente da quella la quantità con cui questi stessi articoli
  dovrebbero essere effettivamente messi in vendita all'interno del
  Marketplace.

> Per maggiori informazioni relativamente a come determinare, per gli
> articoli coinvolti nell' Inserzione, quella che dovrà essere la loro
> quantità di pubblicazione si veda anche il precedente capitolo
> ("*Prezzo Quantità Formato*") di questo manuale

