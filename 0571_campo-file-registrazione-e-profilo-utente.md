# CAMPO FILE (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo File"**

![](./assets/media/image134.png)

permette di inserire all'interno dei Form di Registrazione e/o di
Profilo Utente un campo di input di tipo File mediante il quale poter
allegare al form stesso un generico file.

![](./assets/media/image135.png)

Rilasciando il componente all'interno del form si aprirà **la sua
maschera di gestione e configurazione**

![](./assets/media/image136.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

- **Nome:** permette di inserire un nome per il campo che si sta
  editando;

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Id/Name:** consente di personalizzare i selector HTML "id" e "name"
  per il componente in oggetto in modo tale da poterlo intercettare e
  personalizzare, a livello di CSS o di codice javascript, in maniera
  più semplice ed immediata.

> **Il valore inserito all'interno di questo campo verrà utilizzato per
> entrambi i selector indicati**

- **Tab Index:** consente di personalizzare l'ordine di tabulazione del
  form assegnando uno specifico numero d'ordine al campo in oggetto. Una
  volta assegnato un numero d'ordine ad ogni campo del form sarà poi
  possibile spostarsi da un elemento all'altro, utilizzando il tasto
  "TAB" e secondo l'ordine di tabulazione impostato.

> Nel caso in cui si decida di personalizzare l'ordine di tabulazione
> degli elementi del form sarà necessario assegnare uno specifico numero
> d'ordine ad ogni singolo campo. In caso contrario il passaggio da un
> campo all'altro attraverso il tasto TAB si interromperà in
> corrispondenza del campo con l'ultimo numero d'ordine impostato.
>
> Lato accessibilità il consiglio è quello di non definire una
> navigazione personalizzata impostando specifici valori per il
> parametro in oggetto e lasciare quindi che sia il browser stesso, in
> base alla struttura della pagina a definire gli spostamenti tra un
> campo e l'altro attraverso il tasto TAB.

- **Label (etichetta):** il testo inserito in questo campo sarà
  visualizzato come etichetta propria del Campo File.

- **Condizione di Visibilità:** consente di impostare una condizione in
  base alla quale poter definire quando il componente in oggetto dovrà o
  meno essere visibile all'interno del relativo form.

> Nello specifico, tale condizione potrà essere definita sulla base:

- della nazione di appartenenza dell'utente

- del fatto che l'utente abbia dichiarato di essere un Privato oppure
  un'Azienda

- del fatto che l'utente abbia dichiarato di essere o meno un Ente
  Pubblico

- del fatto che l'utente abbia dichiarato o meno di voler ricevere la
  fattura elettronica

- del valore assunto da uno qualsiasi degli "Attributi Utente" (ad
  eccezione di quelli di tipo File) eventualmente inseriti all'interno
  del relativo form

> **ATTENZIONE!** **Affinchè il controllo di visibilità possa funzionare
> in maniera corretta sarà quindi necessario verificare di aver inserito
> nel form di Registrazione / Profilo Utente appositi campi.**
>
> Per maggiori informazioni in merito a come poter impostare una
> specifica condizione di visibilità per un campo del form, si veda
> anche il successivo capitolo "*Condizioni di visibilità e
> obbligatorietà per i campi interni al form di Registrazione/Profilo
> Utente*" di questo manuale.

- **Campo Obbligatorio:** consente di stabilire se il campo che si sta
  editando debba o meno essere obbligatoriamente compilato per poter
  procedere poi alla conferma del form.

- **Condizioni di Obbligatorietà:** visualizzato solo nel caso in cui il
  precedente parametro "Campo Obbligatorio" sia stato impostato sul
  valore SI. Consente di impostare una condizione in base alla quale
  poter definire quando il componente in oggetto dovrà o meno essere
  considerato come obbligatorio per la corretta compilazione del form.

> Nello specifico, tale condizione potrà essere definita sulla base:

- della nazione di appartenenza dell'utente

- del fatto che l'utente abbia dichiarato di essere un Privato oppure
  un'Azienda

- del fatto che l'utente abbia dichiarato di essere o meno un Ente
  Pubblico

- del fatto che l'utente abbia dichiarato o meno di voler ricevere la
  fattura elettronica

- del valore assunto da uno qualsiasi degli "Attributi Utente" (ad
  eccezione di quelli di tipo File) eventualmente inseriti all'interno
  del relativo form

> Per maggiori informazioni in merito a come poter impostare una
> specifica condizione di obbligatorietà per un campo del form, si veda
> anche il successivo capitolo "*Condizioni di visibilità e
> obbligatorietà per i campi interni al form di Registrazione/Profilo
> Utente*" di questo manuale.

- **Dimensione Massima:** consente di definire quella che dovrà essere
  la dimensione massima (in byte) del file da uplodare.

> **ATTENZIONE!** nel caso in cui il campo in esame venga lasciato vuoto
> non verrà impostato alcun limite per cui l'utente potrebbe uplodare un
> file di qualsiasi dimensione andando ad incidere in maniera più o meno
> pesante sullo spazio disco previsto da contratto. **E' quindi
> consigliabile impostare sempre una dimensione massima coerente con
> quello che dovrà essere l'effettivo utilizzo del campo**.

- **Estensioni Consentite:** consente di indicare le estensioni ammesse
  per il file da uplodare. I valori inseriti devono essere separati da
  virgola.

> **ATTENZIONE!** nel caso in cui il campo in esame non venga
> valorizzato l'utente potrà poi effettuare l'upload di un qualsiasi
> tipo di file. Anche in questo caso **è quindi consigliabile impostare
> delle estensioni consentite coerenti con quello che dovrà essere
> l'effettivo utilizzo del campo**.
>
> Inoltre, indipendentemente da quanto impostato all'interno del campo
> in esame non sarà mai possibile allegare file con le seguenti
> estensioni: **.exe, .vb, .aspx, .asp, .jsp**

- **Attributo di destinazione:** consente di impostare, selezionandolo
  dall'apposito menu a tendina, lo specifico Attributo Utente (Passweb o
  Mexal) da agganciare al campo in esame e che dovrà quindi essere
  utilizzato per memorizzare il file uplodato dall'utente.

> **ATTENZIONE! è possibile selezionare solo ed esclusivamente uno degli
> Attributi Utente di tipo File precedentemente creati all'interno
> dell'apposita sezione del Wizard**
>
> Per maggiori informazioni relativamente a come poter creare e gestire
> attributi utente di tipo File si veda anche l'apposita sezione di
> questo manuale ("*Utenti -- Siti Ecommerce -- Configurazione Utenti
> del sito -- Gestione Attributi*")

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La Label

- Il Controllo (ossia il campo di selezione del file)

- Il Messaggio di errore

> E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame, permettendo dunque, già in fase di
> configurazione del componente stesso di decidere quale elemento dovrà
> essere visualizzato prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

La procedura da seguire per poter uplodare un file in fase di
Registrazione al sito e/o di modifica del proprio Profilo è estremamente
semplice.

Sarà infatti sufficiente cliccare sul campo "**Seleziona File**"

![Videate\\campo_file_registrazione.bmp](./assets/media/image137.png)

in modo tale da aprire la maschera di "Esplora Risorse" mediante la
quale poter ricercare lo specifico file da uplodare.

Una volta selezionato il file desiderato verrà avviata la procedura di
upload e all'interno del form, in corrispondenza del campo di tipo File,
verrà visualizzato un messaggio di caricamento in corso

![](./assets/media/image138.png)

**ATTENZIONE!** Nel caso in cui il file selezionato superi le dimensioni
massime impostate in fase di configurazione del componente verrà
visualizzato un apposito messaggio di errore (personalizzabile, come
tutti i testi relativi a questo componente, all'interno della sezione
"Gestione Testi / Messaggi del sito" del Wizard). Stessa cosa ovviamente
nel momento in cui il file dovesse avere una estensione che non rientra
tra quelle definite in fase di configurazione.

![](./assets/media/image139.png)

Al contrario nel caso in cui il file abbia una delle estensioni
consentite e una dimensione inferiore a quella massima impostata la
procedura di upload terminerà in maniera corretta e all'interno del
campo verrà visualizzato il nome del file uplodato.

![](./assets/media/image140.png)

La piccola **X** presente all'interno del campo consente di rimuovere il
file caricato e procedere, eventualmente con l'upload di un altro file.
Cliccando invece sul nome del file verrà avviato il suo download.

In fase di sincronizzazione nel passaggio dei dati da Passweb verso
Mexal, per i nuovi utenti che hanno completato il form di registrazione,
così come per gli utenti del sito che hanno modificato il proprio
profilo, verrà effettuata, in relazione agli Attributi Utente Mexal di
tipo file, la copia dei relativi file sul server Mexal nella cartella
prestabilita.

In tal senso è bene ricordare che nel caso in cui l'installazione Mexal
sia in server farm Passepartout la cartella di destinazione in cui
verranno copiati i file è gestita in automatico dall'applicazione e non
può essere modificata.

Nel caso, invece, di installazioni locali tale cartella dovrà essere
indicata in maniera specifica in fase di configurazione del sito, agendo
per questo all'interno del campo "**Cartella File Utenti**" presente
nella maschera "Parametri Mexal" accessibile dal menu "*Configurazione
-- Configurazione Gestionale*" del Wizard.

![](./assets/media/image141.png)

**ATTENZIONE! Nel caso di Attributi Utente Passweb di tipo file, i file
uplodati resteranno memorizzati unicamente sul database del sito
(occupando spazio disco) e non verranno mai trasferiti all'interno del
gestionale**

L'amministratore del sito avrà comunque la possibilità di effettuare il
download di questi file all'interno della sezione "**Attributi**"
presente nella maschera "**Dati Utente**" del Wizard cliccando
semplicemente sul nome del file, oppure effettuando un'esportazione
massiva dei dati utente

![](./assets/media/image142.png)

**ATTANZIONE!** I campi di tipo file presenti all' interno della
maschera Dati Utenti sono campi in sola lettura. L'amministratore del
sito potrà quindi effettuare il download dei file uplodati dagli utenti
ma non potrà eliminarli in alcun modo.

In caso contrario infatti l'utente del sito potrebbe trovare all'interno
del proprio profilo una situazione diversa rispetto a quella da lui
impostata.

**ATTENZIONE! In fase di sincronizzazione nel passaggio dei dati da
Mexal verso Passweb gli Attributi Utente di tipo file non sono gestiti**

Questo significa dunque eventuali variazioni effettuate, lato gestionale
sui campi relativi agli attributi di tipo "File" non verranno
considerate.

Questo perché non è attualmente possibile determinare se i file
all'interno del gestionale sono stati variati o meno rispetto all'ultima
sincronizzazione. Inoltre tali file sono stati inseriti direttamente
dall'utente e quindi dovrebbero poter essere modificabili solo ed
esclusivamente da lui (i campi di tipo file, in sostanza, non devono
essere utilizzati per lo scambio di file, ma dovrebbero essere un
supporto ad integrazione dei dati presenti normalmente in anagrafica
utente).

