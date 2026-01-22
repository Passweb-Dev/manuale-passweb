# CREAZIONE DI UNA NUOVA INSERZIONE



Dopo aver correttamente configurato l'integrazione Passweb -- eBay, ed
aver abilitato almeno un Marketplace, il passo successivo dovrà quindi
essere quello di creare un' Inserzione da poter poi utilizzare per
mettere effettivamente in vendita alcuni articoli del proprio sito web
sul marketplace definito all'interno dell'Inserzione stessa.

Portandosi quindi nella sezione "*Catalogo -- eBay -- Gestione
Inserzioni*" del Wizard verrà visualizzata la maschera "**Lista delle
Inserzioni eBay**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_inserzioni_ebay.bmp](./assets/media/image68.png)

all'interno della quale verranno visualizzate tutte le Inserzioni
attualmente configurate.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image69.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image70.png) )

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Cancella Inserzione** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_cancella_inserzione.bmp](./assets/media/image71.png) ): consente di eliminare l'inserzione
  attualmente selezionata in elenco.

**NOTA BENE:** eliminando un'inserzione verranno eliminate anche tutte
le liste di articoli ad essa collegate. Gli articoli già messi in
vendita all'interno di un Marketplace eBay, attraverso una lista
eliminata automaticamente a seguito della cancellazione di un'
Inserzione, continueranno comunque a vivere come entità a se stanti
all'interno del corrispondente sito eBay

- **Modifica Inserzione** ( ): consente di accedere alla maschera di
  configurazione dell'Inserzione attualmente selezionata in maniera tale
  da poterne gestire le singole regole di vendita.

- **Copia Inserzione** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_copia_inserzione.bmp](./assets/media/image72.png) ): consente di copiare l' Inserzione
  attualmente selezionata in elenco (verrà creata una nuova inserzione
  con le stesse esatte regole di gestione definite sull' Inserzione
  sorgente).

- **Aggiungi Inserzione** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_inserzione.bmp](./assets/media/image73.png) ): consente di codificare una nuova Inserzione.

Cliccando su quest'ultimo pulsante verrà infatti visualizzata la
maschera "**Dati Inserzione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dati_inserzione.bmp](./assets/media/image74.png)

attraverso cui poter definire le specifiche regole di vendita che
andranno a caratterizzare l'Inserzione stessa.

In questo senso la sezione **"Impostazioni Generali"** consente di
definire le caratteristiche generali dell'Inserzione. Nello specifico il
campo:

- **Nome:** consente di assegnare un nome alla nuova inserzione in
  maniera tale da poterla poi identificare, tra tutte quelle codificate,
  nelle successive fasi di pubblicazione degli articoli.

- **Account eBay:** consente di indicare lo specifico Account che verrà
  utilizzato nel momento in cui, in fase di pubblicazione degli articoli
  su eBay, dovesse essere selezionata l'Inserzione in esame. E'
  possibile selezionare uno degli Account Venditore precedentemente
  configurati all'interno della corrispondente sezione "Gestione
  Account".

> **Si ricorda inoltre che utilizzando un account di tipo Sandbox le
> liste di articoli collegate a questa Inserzione verranno pubblicate
> solo ed esclusivamente all'interno dell'ambiente di test di eBay.**
>
> **ATTENZIONE!** Nel caso in cui tale Inserzione debba essere
> utilizzata per mettere in vendita articoli nel "modo reale" è
> necessario impostare all'interno di questo campo un account eBay di
> tipo **"Produzione"**

- **Sito eBay:** consente di indicare lo specifico Marketplace da
  associare all' Inserzione che si sta realizzando.

> E' possibile selezionare solo ed esclusivamente uno dei marketplace
> precedentemente abilitati all'interno della corrispondente sezione
> "Marketplace".
>
> **ATTENZIONE!** Nel caso in cui per il marketplace selezionato non
> siano ancora state caricate in Passweb le relative categorie
> merceologiche (tra il momento di attivazione del marketplace e il
> caricamento delle relative categorie merceologiche potrebbero passare
> alcuni minuti) verrà visualizzato un apposito messaggio.

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
vendita articoli sul marketplace statunitense, che accetta come valuta
solo ed esclusivamente il dollaro, sarà necessario per prima cosa
gestire tale valuta in Mexal.

Successivamente sarà poi necessario attivare all'interno del proprio
sito Passweb il paese **"United States"** in maniera tale da poter
gestire il dollaro anche sul sito Ecommerce.

La conversione tra i prezzi in euro del listino associato alla specifica
inserzione e quelli in dollaro verrà poi effettuata in automatico
dall'applicazione utilizzando i fattori di conversione definiti nella
relativa tabella gestionale.

**ATTENZIONE! Nel caso in cui non dovesse essere gestita in Mexal la
valuta utilizzata da uno specifico marketplace di eBay non sarà poi
possibile configurare Inserzioni per quello specifico marketplace.**

**[ECOMMERCE HO.RE.CA]{.underline}**

Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca. non
essendo presente all'interno del gestionale una Tabella Valute con
relativi fattori di conversione sarà possibile configurare delle
inserzioni solo ed esclusivamente su quei marketplace che accettano
l'euro come valuta di gestione.

**ATTENZIONE:** **la scelta del marketplace cui associare un' Inserzione
è di fondamentale importanza non solo perché gli articoli messi in
vendita su eBay attraverso apposite liste collegate a questa Inserzione
saranno poi disponibili solo ed esclusivamente nel corrispondente sito
eBay, ma anche perché le successive regole che occorrerà definire per
completare l'Inserzione potranno variare proprio in conseguenza dello
specifico marketplace eBay selezionato.**

Selezionando infatti uno dei marketplace disponibili, oltre alla valuta
di gestione, verranno abilitate anche le ulteriori sezioni presenti
nella parte bassa della maschera di configurazione, sezioni queste
all'interno delle quali indicare:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\eBay_41.bmp](./assets/media/image75.png)

- **Categoria:** consente di impostare le informazioni relative alle
  categorie merceologiche primaria e secondaria cui dovranno essere
  associati gli articoli messi in vendita attraverso l'inserzione che si
  sta codificando.

- **Descrizione:** consente di impostare le condizioni di vendita dei
  prodotti esportati sul marketplace collegato all'inserzione che si sta
  codificando oltre ai cosiddetti "Identificativi del Catalogo eBay"
  ossia i codici (UPC, EAN, ISBN) utilizzati per identificare
  univocamente i vari articoli all'interno del Catalogo eBay

- **Pagamento:** consente di impostare le modalità di pagamento
  selezionabili per gli articoli messi in vendita mediante l'Inserzione
  che si sta codificando

- **Spedizione:** consente di impostare le modalità di spedizione della
  merce relative agli articoli messi in vendita mediante l'Inserzione
  che si sta codificando

- **Restituzione:** consente di impostare le condizioni di restituzione
  della merce

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

All'interno di questa sezione è possibile impostare le Categorie
Merceologiche primaria e secondaria cui verranno associati, sullo
specifico Marketplace eBay, gli articoli messi in vendita tramite
l'Inserzione che si sta considerando.

Per associare all'Inserzione una specifica categoria merceologica è
sufficiente cliccare sul pulsante "**Cambia Categoria**" e selezionarla
poi dal relativo menu a tendina.

**ATTENZIONE!** L'elenco delle categorie disponibili è fornito
direttamente dallo specifico marketplace eBay

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\eBay_42.bmp](./assets/media/image76.png)

Dipendentemente dalla Categoria Merceologia indicata potrà poi essere
possibile selezionare anche una o più sottocategorie

**ATTENZIONE!** Le categorie e sotto categorie merceologiche
selezionabili dipendono direttamente dallo specifico marketplace e non
possono dunque essere personalizzate in alcun modo. La descrizione di
tali categorie sarà poi in italiano o in lingua dipendentemente, anche
in questo caso, dal marketplace considerato

Una volta selezionate Categorie e Sotto Categorie merceologiche è
necessario cliccare sul pulsante **"Conferma la Categoria"**

A questo punto all'interno della successiva sezione "**Specifiche**"
verranno visualizzati tutti i campi da poter utilizzare per pubblicare
informazioni aggiuntive sugli articoli messi in vendita, informazioni
queste che verranno poi visualizzate sul marketplace eBay nella scheda
prodotto dei vari articoli

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\eBay_45.bmp](./assets/media/image77.png)

**ATTENZIONE!** Le specifiche obbligatorie per poter completare
correttamente l'Inserzione sono indicate da un piccolo asterisco rosso
posto immediatamente a fianco del nome.

Nel caso in cui alcune delle specifiche obbligatorie non siano state
compilate al salvataggio dell'Inserzione verrà visualizzato un apposito
messaggio

Per definire il valore che dovrà assumere una certa specifica è
necessario, innanzitutto, indicare da dove poter andare a prelevare
questo valore selezionando, per questo, una delle opzioni disponibili
all'interno del relativo menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\eBay_46.bmp](./assets/media/image78.png)

Nello specifico è possibile selezionare una delle seguenti opzioni:

- **Nessuno:** selezionando questa opzione la specifica corrispondente
  non verrà valorizzata e, conseguentemente, all'interno della scheda
  prodotto di eBay non verrà visualizzata, in relazione a questa
  specifica, nessuna informazione aggiuntiva

- **Attributo eBay:** in questo caso sarà possibile indicare il valore
  da utilizzare per la corrispondente specifica, selezionandolo tra
  quelli messi a disposizione direttamente da eBay (campo **Valore**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_47.bmp](./assets/media/image79.png)

- **Attributo Passweb:** in questo caso sarà possibile indicare il
  valore da utilizzare per la corrispondente specifica, selezionandolo
  tra gli attributi articolo attualmente mappati all'interno di Passweb
  (campo **Valore**).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_48.bmp](./assets/media/image80.png)

- **Attributo Articolo:** presente solo in corrispondenza di determinati
  campi. In questo caso sarà possibile indicare il valore da utilizzare
  per la corrispondente specifica, selezionandolo direttamente tra i
  campi articolo presenti all'interno del relativo menu a tendina

- **Personalizzato:** in questo caso sarà possibile indicare
  esplicitamente il valore che dovrà assumere all'interno di eBay la
  corrispondente specifica (campo **Valore**).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_49.bmp](./assets/media/image81.png)

- **Elemento di Variazione:** necessario per inserzioni adibite ad
  accogliere articoli con elementi Varianti (es. taglie colori) consente
  di indicare come dovrà essere gestito il corrispondente elemento di
  Variazione.

> Per maggiori informazioni in merito alla possibilità di pubblicare
> sulla piattaforma terza articoli a taglie / colori si veda anche il
> relativo capitolo di questo manuale (*eBay -- Articoli a Taglie e
> Colori*)

**ATTENZIONE!** **Tutti gli articoli messi in vendita attraverso una
certa Inserzione, oltre ad avere le stesse modalità di gestione,
visualizzeranno nelle loro schede prodotto anche le stesse specifiche (e
quindi potenzialmente gli stessi valori).**

In questo senso le uniche informazioni dinamiche, che potranno quindi
variare da articolo ad articolo anche all'interno della stessa
Inserzione, sono quelle gestite mediante gli Attributi Articolo definiti
in Passweb.

**In sostanza dunque mappando una certa specifica con un Attributo eBay
o con un campo Personalizzato poi tutti gli articoli messi in vendita
mediante l'Inserzione in esame avranno, per la stessa specifica, lo
stesso esatto valore.**

**Nel caso in cui invece la specifica sia stata mappata con un Attributo
Passweb, essendo il valore di questi attributi diverso articolo per
articolo, anche prodotti messi in vendita tramite la stessa Inserzione
potranno visualizzare, nella relativa scheda prodotto eBay, per la
stessa specifica informazioni differenti**

##### DESCRIZIONE

All'interno di questa sezione è possibile definire altre informazioni di
carattere descrittivo relativamente a quelli che saranno poi gli
articoli che andranno a far parte dell'inserzione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_50a0.bmp](./assets/media/image82.png)

###### METODI DESCRIZIONE

La sottosezione "**Metodo di Descrizione**" consente di decidere se
compilare i campi relativi al tab "Descrizione" secondo quanto
configurato all'interno di uno dei Template precedentemente codificati
(e magari già utilizzato in qualche altra inserzione) oppure se
realizzarne uno nuovo.

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

Come precedentemente evidenziato, oltre alle specifiche indicate
all'interno della precedente sezione "Categoria", nella scheda prodotto
di eBay verrà sempre visualizzata anche:

- un' **Immagine** articolo

- il **Titolo** (nome) dell'articolo

- una **Descrizione**.

La sottosezione "**Generale**" del tab "Descrizione" consente di gestire
queste informazioni.

Nello specifico, per quel che riguarda l'Immagine verrà utilizzata
**l'immagine principale della scheda prodotto Passweb** mentre i valori
utilizzati per definire all'interno della scheda prodotto di eBay il
Titolo e la Descrizione dell'articolo possono variare in relazione a
quanto impostato per gli omonimi campi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_50a.bmp](./assets/media/image83.png)

In particolare dunque i campi presenti all'interno della sezione
**"Generale"** consentono rispettivamente:

**Titolo:** consente di definire, selezionandolo tra quelli presenti
all'interno del corrispondente menu a tendina, lo specifico campo
Passweb il cui valore dovrà essere utilizzato, nella Scheda Prodotto di
eBay, come Titolo per il relativo articolo. In questo senso è possibile
utilizzare:

- il campo "**Titolo**" corrispondente all'omonimo componente Ecommerce

- i campi **Descrizione**, **Descrizione** **HTML** / **HTML2** /
  **HTML3**

- uno qualsiasi degli **Attributi Passweb** attualmente codificati e
  gestiti all'interno del sito

**Sotto Titolo:** consente di definire, selezionandolo tra quelli
presenti all'interno del corrispondente menu a tendina, lo specifico
campo Passweb il cui valore dovrà essere utilizzato, nella Scheda
Prodotto di eBay, come Sotto Titolo per il relativo articolo. In questo
senso è possibile utilizzare:

- il campo "**Titolo**" corrispondente all'omonimo componente Ecommerce

- i campi **Descrizione**, **Descrizione** **HTML** / **HTML2** /
  **HTML3**

- uno qualsiasi degli **Attributi Passweb** attualmente codificati e
  gestiti all'interno del sito

**ATTENZIONE!** A differenza dei campi Titolo e Descrizione il campo
Sotto Titolo non è obbligatorio

**Descrizione:** consente di definire, selezionandolo tra quelli
presenti all'interno del corrispondente menu a tendina, lo specifico
campo Passweb il cui valore dovrà essere utilizzato, nella Scheda
Prodotto di eBay, come Descrizione per il relativo articolo.

In questo senso è possibile utilizzare:

- l'opzione **Nessuno**. Opzione da selezionare nel momento in cui
  l'esigenza dovesse essere quella di **agganciare prodotti già
  pubblicati su eBay** evitando di sovrascrivere la loro descrizione con
  quella eventualmente presente in Passweb.

> **ATTENZIONE!** si ricorda che nel caso in cui i prodotti già presenti
> sul Marketplace non dovessero essere stati pubblicati a partire da
> Passweb, e l'esigenza dovesse essere quella di aggiornarne
> semplicemente il prezzo o la quantità senza alterare le altre
> informazioni della scheda prodotto, sarà necessario non solo impostare
> il campo "Descrizione" sull'opzione "Nessuno" ma occorrerà anche
> verificare di aver attivato, sulla corrispondente lista di vendita, il
> parametro "**Considera gli articoli come già in vendita**" (per
> maggiori informazioni in merito si veda anche quanto indicato nei
> successivi capitoli di questo manuale)
>
> Infine, considerando che la Descrizione è comunque un campo
> obbligatorio per la scheda prodotto di eBay nel momento in cui, pur
> avendo impostato il campo Descrizione sull'opzione Nessuno,
> **l'inserzione dovesse comunque essere utilizzata per pubblicare nuovi
> prodotti, allora** **in fase di creazione della nuova scheda verrà
> inviata ad eBay una Descrizione uguale al contenuto del campo Titolo
> utilizzato in Passweb per lo stesso articolo**.

- uno qualsiasi degli **Attributi Passweb** attualmente codificati e
  gestiti all'interno del sito

- i campi **Descrizione**, **Descrizione** **HTML** / **HTML2** /
  **HTML3**

- l'opzione **Template HTML.** Selezionando questa opzione verrà
  visualizzato un editor HTML all'interno del quale poter costruire in
  maniera più dettagliata (operando magari direttamente a livello di
  codice HTML) la scheda dei prodotti che verranno poi pubblicati su
  eBay utilizzando l'inserzione in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_template_HTML.bmp](./assets/media/image84.png)

> Il pulsante "**Aggiungi Segnaposto**" presente immediatamente al di
> sotto dell'editor HTML consente di inserire nel template i seguenti
> campi articolo:

- Descrizione

- Descrizione HTML / Descrizione HTML 2 / Descrizione HTML 3

- Immagine Prodotto

- Titolo

- Codice

- Attributi Passweb

> I segnaposto utilizzati verranno poi sostituiti, in fase di
> pubblicazione, con le relative informazioni degli articoli coinvolti
> nella pubblicazione stessa.

**ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
creare delle Descrizioni eBay più dettagliate e strutturate (quindi non
solo del semplice testo) si consiglia di mappare il campo "Descrizione"
dell'inserzione su uno dei valori **Descrizione** **HTML** / **HTML2** /
**HTML3** oppure sul valore **Template HTML**.

Nel primo caso (Descrizione HTML / HTML2 / HTML3 ) la scheda andrà poi
costruita operando dall'anagrafica Passweb del singolo articolo e potrà
quindi essere differenziata per ogni prodotto sia come contenuti che
come struttura.

Nel secondo caso (Template HTML) sarà invece possibile operare
direttamente dalla maschera di gestione dell'Inserzione, la struttura
della scheda sarà però la stessa per tutti gli articoli coinvolti in
quella stessa Inserzione mentre i dati gestiti mediante segnaposto
saranno valorizzati dinamicamente con le relative informazioni dei
singoli prodotti.

###### CONDIZIONI

La sottosezione "**Condizioni**" del tab "Descrizione" consente di
impostare **le condizioni di vendita dei prodotti** esportati sul
marketplace collegato all'Inserzione che si sta codificando

In questo senso sarà quindi necessario selezionare uno dei valori
disponibili tra quelli presenti all'interno del relativo menu a tendina.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_50b.bmp](./assets/media/image85.png)

**ATTENZIONE!** Le condizioni di vendita sono fornite direttamente da
eBay, possono variare a seconda dello specifico marketplace su cui si
sta operando e non possono essere in alcun modo personalizzate

###### IDENTIFICATIVI CATALOGO EBAY

La sottosezione "**Identificativi del catalogo eBay**" è, forse, la più
importante tra quelle presenti all'interno del tab "Descrizione"
inquanto è quella che consente di impostare i codici EPID, UPC, EAN,
ISBN utilizzati per identificare univocamente i vari articoli
all'interno del Catalogo eBay

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_50c.bmp](./assets/media/image86.png)

In questo senso è bene subito fare alcune considerazioni di fondamentale
importanza:

- **Nel momento in cui l'esigenza dovesse essere quella di agganciare,
  in fase di pubblicazione un prodotto già presente su eBay, sarà
  necessario utilizzare come campo chiave il codic**e **EPID** (EBay
  Product ID) che dovrà essere quindi opportunamente inserito e
  valorizzato per ogni singolo articolo coinvolto nell'inserzione.

> **Se, al contrario, si dovesse decidere di utilizzare come campo
> chiave per agganciare un prodotto già presente sul marketplace un
> altro identificativo eBay (come ad esempio l'EAN o l'UPC) si
> correrebbe il rischio di non agganciare il prodotto già presente sul
> marketplace finendo quindi per creare un duplicato della stessa
> inserzione**
>
> **ATTENZIONE!** Per non duplicare le Inserzioni già presenti sul eBay
> è necessario pubblicare gli articoli verificando di aver gestito per
> ciascuno di essi il corretto EPID

Detto questo, occorre poi sottolineare che dipendentemente dallo
specifico marketplace su cui si sta operando oltre che dalla tipologia
di prodotti messi in vendita può essere necessario / obbligatorio
indicare, in fase di pubblicazione, per ogni articolo coinvolto
nell'Inserzione:

- **il codice EPID:** rappresenta l'EBay Product ID ossia il codice
  identificativo (interno) assegnato ai vari prodotti direttamente da
  EBay

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
> esattamente come quello che dovrà poi essere passato ad EBay in fase
> di pubblicazione dell'articolo.
>
> Per far questo è sufficiente accedere alla maschera di creazione del
> codice Alias

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_codice_alias.bmp](./assets/media/image87.png)

> e compilare i vari campi come di seguito indicato:

- **Codice**: inserire il valore del codice (EPID / UPC / EAN / ISBN)
  che dovrà essere passato ad EBay in fase di pubblicazione del prodotto

- **Descrizione:** indicare la tipologia di codice EBay che si intende
  mappare.

> In particolare nel caso in cui il codice in esame debba essere
> considerato come l'EBay Product ID all'interno di questo campo andrà
> inserito il valore **EPID**.
>
> Se invece il codice in esame dovrà essere considerato come il codice
> UPC / EAN / ISBN da passare ad EBay all'interno del campo descrizione
> andrà inserito il valore **GTIN**

- **Elemento TG -- solo per articoli a Taglia:** indicare,
  selezionandola dall'apposito menu a tendina, la specifica Taglia cui
  il codice in esame dovrà essere riferita

> Supponendo dunque di aver utilizzato all'interno del gestionale N
> codici alias per un determinato articolo e di aver marcato in maniera
> corretta solo uno di essi come codice EPID (secondo quanto sopra
> indicato) il campo "EBay Product ID" presente nella sezione
> "Identificativi Catalogo EBay" andrà poi impostato sul valore
> "**Codice Alias EPID**" come evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_ebay_eipd.bmp](./assets/media/image88.png)

> In queste condizioni in fase di pubblicazione sul marketplace verrà
> passato ad EBay il codice alias marcato sul gestionale come codice
> EPID.
>
> Allo stesso modo se l'esigenza dovesse essere quella di passare ad
> EBay il codice UPC / EAN / ISBN sarà necessario marcare uno tra gli N
> codici Alias utilizzati secondo quanto precedentemente indicato e
> impostare poi, questa volta, il relativo campo UPC / EAN / ISBN
> dell'Inserzione presente nella sezione "**Codice Alias GTIN**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_ebay_gtin.bmp](./assets/media/image89.png)

> **ATTENZIONE!** Nel caso in cui per determinate ragioni dovessero
> essere marcati più codici alias come, ad esempio, codici EPID da
> passare ad EBay, in fase di pubblicazione verrà considerato, ai fini
> dell'inserzione sul marketplace, solo il primo valore utile.
>
> **[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI
> HO.RE.CA.]{.underline}**
>
> In questo caso sarà possibile mappare il campo Identificativo catalogo
> EBay con il codice alias di una determinata tipologia (es. Codice
> EAN13, Codice EAN8 ecc...) selezionandola tra quelle in uso
> all'interno del gestionale.
>
> A differenza di Mexal in questo caso però, non è possibile marcare uno
> degli N codici alias o EAN in uso all'interno del gestionale come
> quello che identifica in maniera specifica il codice da passare ad
> EBay in fase di pubblicazione pertanto, nel momento in cui un
> determinato articolo dovesse avere più valori per la stessa tipologia
> di Alias verrà considerato, ai fini dell'inserzione sul marketplace,
> solo il primo valore utile.

**ATTENZIONE!** Per poter mettere in vendita correttamente degli
articoli all'interno di uno qualsiasi dei marketplace eBay è necessario
gestire almeno uno dei codici sopra indicati. Nel caso in cui non si
dovesse gestire nessuno di questi codici potrebbe non essere possibile
pubblicare articoli sui marketplace di eBay

###### IMMAGINI

La sottosezione "**Immagini**" consente, infine di impostare ulteriori
**Immagini** dell'articolo da visualizzare nella scheda prodotto di
eBay.

In questo senso va detto, come inizialmente evidenziato, che nella
scheda prodotto di eBay verrà sempre visualizzata almeno un'Immagine
corrispondente **all'immagine principale della scheda prodotto
Passweb.**

E' comunque possibile decidere di visualizzare anche delle immagini
aggiuntive, fino ad un massimo di 9, selezionando il valore desiderato
all'interno del corrispondente campo presente in questa sezione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_70.bmp](./assets/media/image90.png)

**ATTENZIONE!** Come Immagini aggiuntive verranno utilizzate le
**Immagini Secondarie della Scheda Prodotto** Passweb.

Nel momento in cui si dovesse quindi decidere di pubblicare su eBay, ad
esempio, 4 Immagini sarà poi necessario accertarsi che per gli articoli
facenti parte dell'Inserzione in oggetto siano correttamente gestite
all'interno del sito Passweb oltre all'Immagine Principale anche altre 3
Immagini Secondarie

##### PAGAMENTO

All'interno di questa sezione è possibile specificare le modalità di
pagamento che dovranno essere rese disponibili agli utenti eBay in fase
di acquisto degli articoli messi in vendita tramite l'Inserzione che si
sta codificando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_52.bmp](./assets/media/image91.png)

**ATTENZIONE! La lista dei possibili pagamenti è fornita direttamente da
eBay e potrebbe variare a seconda dello specifico marketplace su cui si
sta operando**

Per abilitare un pagamento tra quelli presenti in elenco è sufficiente
selezionare il check presente in corrispondenza del pagamento stesso

Considerando inoltre che gli ordini effettuati su eBay potrebbero poi
essere importati in Passweb e da qui essere inseriti sul gestionale,
sarà necessario anche mappare ciascuno dei pagamenti abilitati con una
delle modalità di pagamento gestite sul proprio sito Passweb e
corrispondenti quindi ad uno dei Pagamenti codificati nelle relative
tabelle gestionali.

In questo senso è possibile indicare la modalità di pagamento desiderata
selezionandola tra quelle disponibili all'interno del corrispondente
menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_53.bmp](./assets/media/image92.png)

**ATTENZIONE!** Nel caso in cui si selezioni la modalità di pagamento
relativa a PayPal sarà poi necessario indicare all'interno del relativo
campo (**PayPal Email**) anche l'indirizzo mail associato ad un Account
PayPal valido (di test o di produzione) di tipo Venditore.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_61.bmp](./assets/media/image93.png)

##### SPEDIZIONE

All'interno di questa sezione è possibile indicare tutte le modalità di
spedizione merce che dovranno essere rese disponibili agli utenti eBay
in fase di acquisto degli articoli messi in vendita tramite l'Inserzione
che si sta codificando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_54.bmp](./assets/media/image94.png)

In particolare all'interno della sezione "**Luogo**" è possibile
specificare **Paese**, **CAP** e **Località** da cui risulterà essere
spedita le merce acquistata su eBay tramite l'Inserzione in esame.

All'interno delle sezioni "**Spedizione Nazionale**" e "**Spedizione
Internazionale**" è invece possibile definire esattamente le modalità di
spedizione merce che l'utente eBay potrà selezionare in fase di acquisto
in relazione rispettivamente a spedizioni sul territorio italiano e/o su
paesi esteri.

Per definire una nuova modalità di spedizione è necessario cliccare
innanzitutto sul pulsante "**Aggiungi Metodo**" presente in
corrispondenza tanto della sezione Spedizioni Nazionali quanto di quella
relativa alle Spedizioni Internazionali.

In questo modo verrà infatti inserito un nuovo record in tabella

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_55.bmp](./assets/media/image95.png)

all'interno del quale dover indicare:

- **Servizio:** consente di specificare il servizio che verrà utilizzato
  per la modalità si spedizione merce che si sta codificando (es.
  Corriere Espresso, DHL, Pacco Celere ecc...)

> **ATTENZIONE!** L'elenco dei servizi disponibili è fornito
> direttamente da eBay e potrebbe variare a seconda dello specifico
> marketplace su cui si sta operando

- **Articolo Spesa:** consente di indicare l' Articolo di tipo Spesa che
  dovrà essere utilizzato per gestire i costi relativi alle spese di
  trasporto.

> **ATTENZIONE!** Negli ordini provenienti da eBay le spese di trasporto
> non saranno inserite nel piede del documento ma verranno gestite
> sempre e solamente mediante l'inserimento in ordine di un articolo di
> tipo spesa.
>
> In questo senso, nel caso in cui si dovessero abilitare diversi metodi
> di spedizione è consigliabile utilizzare diversi Articoli di tipo
> Spesa in maniera tale da individuare chiaramente (tramite la loro
> descrizione) la tipologia di trasporto selezionata dall'utente in fase
> di acquisto su eBay.

- **Modalità:** consente di impostare la metodologia di calcolo delle
  spese legate al trasporto che si sta codificando. E' possibile
  selezionare uno dei seguenti valori:

  - **Valore Personalizzato:** consente di indicare nei successivi
    campi, Costo e Spese Aggiuntive, l'esatto importo delle spese di
    spedizione

  - **Gratis:** selezionando questa opzione il trasporto in esame sarà
    gratuito (verranno contemporaneamente azzerati gli importi
    eventualmente indicati nei successivi campi Costo e Spese
    Aggiuntive)

- **Costo:** consente di indicare l' importo delle spese di trasporto
  che verranno applicate nel momento in cui l'utente eBay in fase di
  acquisto dovesse selezionare la modalità di spedizione che si sta
  codificando (la valuta considerata dipenderà dallo specifico
  marketplace su cui si sta operando).

> **ATTENZIONE!** **Inserire in questo campo l'importo del trasporto già
> comprensivo di IVA**
>
> Nel caso in cui dovesse essere poi generato un ordine cliente (OC)
> l'IVA sulle spese di trasporto verrà scorporata secondo l'aliquota
> definita per l'Articolo di tipo Spesa utilizzato per la spedizione in
> esame, ed inserita nella corrispondente voce del piede del documento.

- **Spese Aggiuntive:** consente di indicare l'importo di eventuali
  spese aggiuntive che verranno sommate ai costi del trasporto e
  applicate nel momento in cui l'utente eBay in fase di acquisto dovesse
  selezionare la modalità di spedizione che si sta codificando (la
  valuta considerata dipenderà dallo specifico marketplace su cui si sta
  operando)

> **Come nel caso dei costi di spedizione anche in questo caso l'importo
> inserito all'interno di questo campo dovrà essere quello comprensivo
> di IVA**

- **Tempo di spedizione:** consente di specificare il tempo che verrà
  indicato su eBay come necessario per la spedizione della merce. I
  valori indicati all'interno del corrispondente menu a tendina sono
  definiti direttamente da eBay e non possono quindi essere
  personalizzati in alcun modo

- **Costo "Contrassegno":** consente di impostare un costo aggiuntivo
  che verrà applicato solo ed esclusivamente nel caso in cui l'utente
  dovesse selezionare in fase di acquisto un pagamento in Contrassegno.

> Oltre al costo aggiuntivo è necessario indicare, selezionandolo tra
> quelli presenti all'interno del corrispondente menu a tendina, anche
> un apposito articolo di tipo Spesa, articolo questo che verrà poi
> utilizzato per gestire il costo aggiuntivo e che verrà quindi inserito
> nel corpo del relativo documento gestionale.
>
> **Come nel caso dei costi di spedizione anche questa volta l'importo
> da inserire dovrà essere quello comprensivo di IVA**

Nel caso in cui si stiano codificando delle Spedizioni Internazionali,
oltre alle informazioni sopra indicate, sarà necessario indicare anche
la Nazione di riferimento selezionandola tra quelle presenti in elenco:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_56.bmp](./assets/media/image96.png)

Va detto infine che è ovviamente possibile attivare e gestire dei metodi
di spedizione anche all'interno del proprio Account Venditore di eBay
(dove è possibile, tra l'altro gestire anche delle spese a scaglioni che
non sono però attualmente gestite lato Passweb).

In questo senso occorre però fare alcune precisazioni:

- **Nel caso in cui si dovesse attivare su Passweb un Metodo di
  trasporto non ancora presente all'interno del proprio Account
  Venditore di eBay**, questo verrà attivata automaticamente anche su
  eBay nel momento in cui verranno pubblicati per la prima volta
  articoli associati all'Inserzione che si sta codificando.

- **Nel caso in cui si dovesse attivare all'interno del proprio Account
  Venditore di eBay un metodo di Trasporto non codificato anche nella
  corrispondente Inserzione Passweb,** in fase di importazione ordini da
  eBay potrebbero non essere considerate le spese di spedizione (per cui
  il Totale Ordine presente su Ebay non coinciderebbe più con il totale
  dell'ordine importato su Passweb e, conseguentemente, sul gestionale).

##### RESTITUZIONE

All'interno di questa sezione è possibile specificare quelle che
dovranno essere indicate all'interno di eBay come possibili modalità di
recesso dall'acquisto effettuato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_57.bmp](./assets/media/image97.png)

**E' possibile decidere di abilitare o meno il diritto di recesso.**

Nel caso in cui tale diritto venga attivato sarà poi possibile fornire
ulteriori informazioni che potranno variare da paese a paese e quindi da
marketplace a marketplace

##### PREZZO QUANTITA' FORMATO

All'interno di questa sezione è possibile definire le condizioni di
vendita degli articoli in relazione ad informazioni quali il prezzo, la
tipologia di vendita e/o la durata dell'inserzione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_58.bmp](./assets/media/image98.png)

La sezione "**Metodo di Prezzo, quantità e formato**" consente di
decidere se compilare i campi di questa maschera secondo quanto
configurato all'interno di uno dei Template precedentemente codificati
(e magari già utilizzato in qualche altra inserzione) oppure se
realizzarne uno nuovo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserzione_ebay_metodo_quantita.bmp](./assets/media/image99.png)

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

###### TIPOLOGIA DI VENDITA

All'interno della sezione "**Modalità di Vendita desiderata per
l'oggetto**" è possibile impostare la modalità secondo cui dovranno
essere messi in vendita gli articoli collegati all'Inserzione che si sta
codificando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tipologia_vendita.bmp](./assets/media/image100.png)

Per il campo "**Tipo di Vendita**" è possibile selezionare una delle
seguenti opzioni:

- **Vendita Compralo Subito:** selezionando questa opzione gli articoli
  messi in vendita tramite l'Inserzione in esame verranno trattati come
  articoli a prezzo fisso e potranno quini essere acquistati
  immediatamente

- **Asta Online:** selezionando questa opzione gli articoli messi in
  vendita tramite l'Inserzione in esame verranno gestiti con delle Aste.
  Il prezzo indicato per ogni articolo verrà considerato come prezzo di
  partenza dell'Asta e l'articolo potrà essere acquistato solo nel caso
  in cui si vinca la relativa Asta.

**NOTA BENE:** la gestione delle aste è demandata interamente a eBay.
Per maggiori informazioni in merito si consiglia dunque di consultare la
relativa documentazione.

###### DURATA DELL'INSERIZIONE E QUANTIA' DI ARTICOLI PUBBLICATI

All'interno della sezione "**Quantità e durata**" è possibile definire
la durata dell'inserzione e la quantità con cui gli articoli pubblicati
mediante questa stessa inserzione dovranno poi essere disponibili sul
Marketplace

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\durata_e_quantita.bmp](./assets/media/image101.png)

Nello specifico dunque il campo:

**Durata della Vendita:** consente di indicare il periodo di tempo
durante il quale gli articoli messi in vendita tramite l'Inserzione in
esame dovranno rimanere effettivamente acquistabili all'interno del
marketplace di eBay

**NOTA BENE:** i valori selezionabili dal corrispondente menu a tendina
sono definiti da eBay stesso e possono variare in relazione allo
specifico marketplace selezionato

Al termine del periodo di tempo indicato non sarà più possibile
acquistare all'interno di eBay eventuali articoli collegati
all'Inserzione in esame. In ogni caso è sempre possibile decidere di
interrompere manualmente la vendita all'interno di eBay di un
determinato articolo in un qualsiasi momento.

Nel momento in cui un articolo non dovesse più essere acquistabile
all'interno di eBay (o perché è scaduto il suo periodo di vendita o
perché la sua vendita è stata interrotta manualmente) eBay stesso
provvederà ad inviare al titolare dell'account una specifica mail di
notifica.

**Quantità:** consente di definire la quantità con cui gli articoli
messi in vendita tramite l'Inserzione in esame dovranno poi essere
disponibili sul relativo marketplace.

**ATTENZIONE! eBay non consente la messa in vendita di articoli in
quantità uguale a 0.**

Nel caso in cui, dunque, a seguito di un determinato calcolo la quantità
di un articolo da pubblicare sul marketplace dovesse essere pari a 0, in
fase di pubblicazione verrà ritornato un apposito messaggio di errore

E' possibile selezionare una delle seguenti opzioni:

- **Singolo oggetto:** in queste condizioni ogni articolo messo in
  vendita tramite l'Inserzione in esame verrà considerato come oggetto
  singolo ed avrà quindi, sul marketplace, quantità disponibile pari a 1

- **Valore Personalizzato:** in queste condizioni è possibile indicare
  all'interno del successivo campo "**Valore della Quantità**" l'esatto
  valore con cui ogni articolo messo in vendita tramite l'Inserzione in
  esame dovrà poi essere disponibile, sul relativo marketplace

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserzione_valore_quantita.bmp](./assets/media/image102.png)

> Supponendo quindi di impostare il campo "Valore Quantità" a 5, ogni
> articolo messo in vendita tramite l'Inserzione in esame verrà
> pubblicato e sarà quindi disponibile sul relativo Marketplace in
> quantità pari a 5

- **Quantità in magazzino:** selezionando questa opzione sarà poi
  possibile impostare la quantità con cui gli articoli dovranno essere
  pubblicati sul relativo Marketplace, come una percentuale della
  quantità in cui gli stessi articoli sono effettivamente disponibili
  all'interno dei magazzini definiti in fase di configurazione
  dell'Account collegato all' Inserzione.

> Per maggiori informazioni relativamente a come definire i magazzini
> associati ad un Account eBay si veda anche la sezione "*eBay --
> Gestione Account -- Collegamento dell'Account Venditore di eBay al
> sito Passweb*" di questo manuale.
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserzione_valore_quantita_percentuale.bmp](./assets/media/image103.png)

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
informazioni in merito si veda anche il successivo capitolo
"Associazione degli articoli ad una lista di vendita e pubblicazione su
eBay")

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
presenti all'interno della sezione "Quantità e durata" nel seguente
modo:

Quantità = Singolo Oggetto

oppure

Quantità = Valore Personalizzato

Valore della Quantità = 1

**[ESEMPIO 2]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace determinati articoli
sempre e solamente in quantità pari a 5

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità e durata" nel seguente
modo:

- Quantità = Valore Personalizzato

- Valore della Quantità = 5

**[ESEMPIO 3]{.underline}**

**Esigenza 🡪** Rendere disponibili sul marketplace gli articoli
coinvolti nell'Inserzione in una quantità pari al **20%** della loro
effettiva disponibilità sul Magazzino associato all'Account che si sta
utilizzando

L'esigenza in questione può essere soddisfatta impostando i parametri
presenti all'interno della sezione "Quantità e durata" nel seguente
modo:

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
presenti all'interno della sezione "Quantità e durata" nel seguente
modo:

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
eBay, gli articoli collegati all'Inserzione che si sta considerando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserzioni_prezzo.bmp](./assets/media/image104.png)

In questo senso il campo:

**Prezzo:** consente di indicare lo specifico listino del gestionale che
dovrà essere utilizzato per determinare il prezzo degli articoli messi
in vendita mediante l'Inserzione in esame.

Nel caso di siti Ecommerce collegati a Mexal è possibile, come
evidenziato nei precedenti capitoli di questo manuale, mettere in
vendita articoli anche su marketplace eBay che gestiscono valute diverse
dall'euro.

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_59.bmp](./assets/media/image105.png)

La sezione "**Metodo di Sincronizzazione**" consente di decidere se
compilare i campi di questa maschera secondo quanto configurato
all'interno di uno dei Template precedentemente codificati (e magari già
utilizzato in qualche altra inserzione) oppure se realizzarne uno nuovo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserzione_ebay_metodo_sincronizzazione.bmp](./assets/media/image106.png)

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regole_messa_in_vendita_ebay.bmp](./assets/media/image107.png)

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
> Marketplace si veda anche la sezione "*eBay -- Gestione Account --
> Collegamento dell'Account Venditore di eBay al sito Passweb*" di
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regole_modifica_in_vendita_ebay.bmp](./assets/media/image108.png)

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_regole_modifica_in_vendita_2.bmp](./assets/media/image109.png)

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
sezione "Condizioni -- Modifiche Parziali" determinano invece le regole
di modifica relative solo al prezzo degli articoli pubblicati sul
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_regole_modifica_in_vendita_3.bmp](./assets/media/image110.png)

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_modifiche_totali.bmp](./assets/media/image111.png)

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

Se l'operazione di pubblicazione è relativa dunque a quegli articoli che
non si trovano attualmente sul Marketplace, la ripubblicazione o rimessa
in vendita, è un'operazione relativa invece ai soli articoli che, pur
essendo ancora all'interno del Marketplace, non possono attualmente
essere acquistati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regole_rimessa_in_vendita_ebay.bmp](./assets/media/image112.png)

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
> Marketplace si veda anche la sezione "*eBay -- Gestione Account --
> Collegamento dell'Account Venditore di eBay al sito Passweb*" di
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regole_di_blocco_ebay.bmp](./assets/media/image113.png)

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
> Marketplace si veda anche la sezione "*eBay -- Gestione Account --
> Collegamento dell'Account Venditore di eBay al sito Passweb*" di
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

- **Tra il**: : in queste condizioni a seguito di una sincronizzazione
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

