# COMPONENTI PER IL FORM - CAMPO FILE



Il Componente **"Campo File"** permette di inserire all'interno del Form
un campo di input di tipo File grazie al quale chi compila il form potrà
allegare al form stesso un generico file.

Rilasciando il componente all'interno del form si aprirà **la sua
maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_campo_file_res.bmp](./assets/media/image142.png)

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

> Tale condizione potrà essere definita sulla base del valore assunto:

- dal campo "Nazione" eventualmente presente all'interno del form in
  esame

- da uno qualsiasi dei campi presenti all'interno del form per cui sia
  stato correttamente valorizzato, in fase di configurazione, il
  parametro "**Id/name**"

> Per maggiori informazioni in merito a come poter impostare una
> condizione di visibilità per un campo del form, si veda anche il
> successivo capitolo "*Condizioni di visibilità e obbligatorietà per i
> campi del form*" di questo manuale.

- **Campo Obbligatorio:** consente di stabilire se il campo che si sta
  editando debba o meno essere obbligatoriamente compilato per poter
  procedere poi alla conferma del form.

- **Condizioni di Obbligatorietà:** visualizzato solo nel caso in cui il
  precedente parametro "Campo Obbligatorio" sia stato impostato sul
  valore SI.

> Consente di impostare una condizione in base alla quale poter definire
> quando il campo in esame dovrà o meno essere considerato come
> obbligatorio per la corretta compilazione del form.
>
> Tale condizione potrà essere definita sulla base del valore assunto:

- dal campo "Nazione" eventualmente presente all'interno del form in
  esame

- da uno qualsiasi dei campi presenti all'interno del form per cui sia
  stato correttamente valorizzato, in fase di configurazione, il
  parametro "**Id/name**"

> Per maggiori informazioni in merito a come poter impostare una
> condizione di obbligatorietà, per un campo del form si veda anche il
> successivo capitolo "*Condizioni di visibilità e obbligatorietà per i
> campi del form*" di questo manuale.

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

L'utilizzo che verrà fatto degli allegati al form dipenderà poi da come
è stato configurato il form stesso e quindi dal fatto che alla conferma
i risultati vengano inviati via mail oppure salvati in un apposito file
csv o xml.

In particolare, nel caso in cui il form sia stato configurato per
inviare i risultati via mail, alla conferma i file caricati all'interno
del form verranno inviati come allegati alla mail; inoltre, nel corpo
della mail verrà indicato, in corrispondenza di ogni campo di tipo file,
il nome del relativo allegato (che sarà del tipo file\_\<id campo
file\>\_\<numero di riga\>).

Nel caso in cui invece il form sia stato configurato in maniera tale da
salvare i risultati all'interno di un apposito file csv/xml, alla
conferma i dati del form verranno aggiunti al relativo file csv/xml;
eventuali allegati verranno invece memorizzati in un apposita cartella
del sito, cartella questa che verrà, ovviamente, conteggiata nel calcolo
dello spazio disco disponibile da contratto.

> **NOTA BENE:** nel caso in cui il form sia stato configurato per
> salvare i risultati in formato csv o xml, eventuali allegati al form
> andranno ad incidere sullo spazio disco disponibile da contratto.

In fase di download, lato Wizard, dei file csv o xml contenenti i
risultati del form, verrà creato uno zip contenente sia il csv/xml che
l'insieme dei file via via allegati al form in questione.

> **NOTA BENE:** il download lato Wizard dei file csv o xml contenenti i
> risultati del form con i relativi allegati non eliminerà in maniera
> definitiva dal server queste risorse che continueranno dunque ad
> occupare parte dello spazio disco disponibile da contratto.

Nel caso in cui, dunque, l'esigenza sia quella di liberare spazio disco,
eliminando i risultati di un form con i relativi eventuali allegati,
sarà necessario agire dall'apposita sezione del Wizard ("*Utenti --
Gestione Forms*").

