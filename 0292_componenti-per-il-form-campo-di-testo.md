# COMPONENTI PER IL FORM - CAMPO DI TESTO



Il Componente **"Campo di Testo"** permette di inserire all'interno del
form un classico campo di input.

Il campo, oltre a non accettare valori di formattazione del testo
(maiuscole o minuscole), non conformi con quanto stabilito, può
contenere anche valori numerici o un indirizzo mail.

Una volta inserito il Componente all'interno del form, verrà aperta in
automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image121.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare sarà possibile impostare un valore per i seguenti
parametri:

- **Nome:** consente di inserire un nome per il Componente che si sta
  creando.

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

- **Label (etichetta):** è ciò che sarà visualizzato come etichetta
  propria del campo che l'utente dovrà compilare.

- **Segnaposto:** permette di definire un testo da utilizzare **come
  segnaposto** da poter visualizzare all'interno del campo di input.

> **ATTENZIONE!** Al click dell'utente sul campo in esame il testo
> indicato scomparirà consentendo quindi all'utente di inserire il
> valore desiderato. Quanto indicato all'interno di questo campo non
> verrà quindi considerato alla conferma del form.

- **Valore di default:** consente di indicare un testo che verrà
  utilizzato (e visualizzato) **come valore di default** per il campo in
  esame.

> **ATTENZIONE!** A differenza di quanto indicato per il precedente
> parametro "Segnaposto", il testo inserito all'interno del campo
> "Valore di default" **non scomparirà** in automatico al click
> dell'utente sul campo di input ma, al contrario, verrà considerato
> come se fosse un vero e proprio valore indicato dall\'utente stesso in
> fase di compilazione del form.
>
> Il pulsante "**Aggiungi Segnaposto"** consente di precompilare il
> campo in esame con uno dei seguenti valori di default:

- **\$pageUrl\$ -- Url della Pagina:** url assoluto della pagina web in
  cui è presente il componente Form in esame

- **\$pageTitle\$ -- Titolo della Pagina**: Titolo della pagina in cui è
  presente il componente Form in esame.

> Per maggiori informazioni relativamente a come poter personalizzare il
> Titolo (tag Title) di una pagina del proprio sito si veda anche la
> sezione *"Live Editing per Varianti Responsive -- Pagine -- Pagine
> Generiche"* di questo manuale

- **\$userName\$ -- Nome Cognome/Ragione Sociale Utente**: nome e
  cognome o ragione sociale dell\' utente attualmente loggato.

- **\$userMail\$ -- EMail Utente:** email dell\'utente dell\' utente
  attualmente loggato.

- **\$userPhone\$ -- Telefono Utente:** telefono dell\' utente
  attualmente loggato

- **\$userCode\$** -- **Codice Utente**: codice conto dell\' utente
  attualmente loggato.

- **\$userAddress\$ -- Indirizzo Utente**: indirizzo dell\'utente dell\'
  utente attualmente loggato.

- **\$agentAssociatoCode\$ -- Codice Agente associato (solo Ecommerce
  Mexal):** codice conto dell'agente associato, lato gestionale,
  all'utente attualmente loggato

- **\$agentLoggatoCode\$ -- Codice Agente loggato: (solo Ecommerce
  Mexal):** codice conto dell'agente attualmente loggato

- **\$agentAssociatoName\$ -- Nome Cognome Agente associato (solo
  Ecommerce Mexal):** nominativo dell'agente associato, lato gestionale,
  all'utente attualmente loggato

- **\$agentLoggatoName\$ -- Nome Cognome Agente loggato (solo Ecommerce
  Mexal):** nominativo dell'agente attualmente loggato

> **ATTENZIONE!** Affinchè il campo possa essere correttamente
> precompilato con eventuali dati dell'utente / agente ("Nome Cognome /
> Ragione Sociale", "Email", "Telefono" ...) è necessario, ovviamente,
> che l'utente stesso abbia già effettuato l'autenticazione al sito.

- **\$cmsTitle\$** -- Titolo CMS: titolo dello specifico post CMS
  visualizzato nella pagina in cui è inserito il componente Form in
  esame.

> **ATTENZIONE**! Il segnaposto \$cmsTitle\$ verrà valorizzato,
> ovviamente, solo nel momento in cui il Form sia stato inserito
> all'interno di una pagina utilizzata per visualizzare il dettaglio di
> un articolo CMS e in cui è presente, dunque, anche il componente
> "Dettaglio News".
>
> **E' molto importante, inoltre, che il componente "Dettaglio News" sia
> stato inserito, nella pagina, prima del componente Form,** in caso
> contrario il segnaposto non verrebbe infatti valorizzato in alcun
> modo.

- **\$articleCode\$ -- Codice dell\'Articolo:** codice dello specifico
  articolo cui fa riferimento la pagina prodotto in cui è stato inserito
  il Form in esame.

> **ATTENZIONE!** Affinchè questo segnaposto possa essere correttamente
> valorizzato è necessario, ovviamente, che il Form in esame sia stato
> inserito all'interno di una pagina prodotto.
>
> **NOTA BENE**: affinchè i segnaposto sopra indicati possano funzionare
> in maniera corretta, precompilando il campo di testo con il relativo
> valore, è necessario non alterarne la struttura.
>
> Nel caso in cui, dunque, si dovesse decidere di inserire i segnaposto
> manualmente senza selezionarli dall'apposito menu occorre prestare
> molta attenzione ad utilizzare il nome corretto e a non eliminare le
> parentesi graffe. In caso contrario il segnaposto non verrà più
> considerato come tale ma come del semplice testo da visualizzare, così
> come indicato, all'interno del campo di testo.

- **Tipo Valore:** Indica quali dati potranno essere inseriti
  all'interno del campo

  - **Testo:** all'interno del campo potrà essere inserito un qualsiasi
    carattere alfanumerico maiuscolo o minuscolo (compresi eventuali
    caratteri speciali)

  - **Maiuscolo:** all'interno del campo potranno essere inseriti
    soltanto caratteri testuali maiuscoli

  - **Numerico:** all'interno del campo potranno essere inseriti
    soltanto numeri interi.

  - **Mail:** all'interno del campo dovrà essere inserito un indirizzo
    di posta elettronica. Un apposito controllo verificherà la corretta
    sintassi dell'indirizzo mail inserito che dovrà quindi rispettare il
    formato "*nomecasella@indirizzo.it*".

> **ATTENZIONE! Nel caso in cui si desideri far arrivare una mail
> riassuntiva con i dati del form anche all'utente che lo ha compilato,
> è necessario inserire all'interno del form stesso un campo di tipo
> mail (1) e configuralo inserendo all'interno del campo Id/Name, il
> segnaposto "email" (2)**

![](./assets/media/image122.png)

> In queste condizioni oltre all'indirizzo inserito all'interno del
> campo "Indirizzo E-mail" presente tra i parametri di configurazione
> del form, la mail informativa verrà inviata anche all'indirizzo mail
> inserito dall'utente all'interno del campo in oggetto.
>
> Tale mail verrà inoltre inviata anche nel caso in cui il form sia
> stato configurato per salvare i dati all'interno di un file .xml o
> .csv.
>
> Nella mail inviata all'amministratore del sito il campo "Rispondi a"
> sarà valorizzato automaticamente con l'indirizzo di posta inserito
> dall'utente in fase di compilazione del form all'interno del campo in
> oggetto.
>
> Nella mail inviata all'utente il campo "Rispondi a" non sarà
> ovviamente valorizzato in alcun modo.
>
> **ATTENZIONE! L'indirizzo di posta utilizzato come mittente per queste
> mail sarà quello indicato all'interno della pagina "Parametri
> Posta/SMS" del Wizard.**

- **Decimale:** all'interno del campo potranno essere inseriti
  indifferentemente numeri interi o decimali (utilizzando per questo il
  carattere , oppure il carattere . ).

- **Telefono:** all'interno del campo potranno essere inseriti soltanto
  numeri di telefono nel formato E.164 (lo standard internazionale per
  la telefonia). Un apposito controllo verificherà la correttezza del
  numero inserito che dovrà quindi rispettare le seguenti regole:

  - il primo carattere deve essere un + seguito dal country code (es.
    +39 per l'Italia) e dal numero di telefono

  - il primo numero dopo il + non può essere uno 0

  - il numero di telefono, comprensivo di country code, non può avere
    meno di 5 cifre né più di 15

  - non sono consentiti caratteri speciali (trattini spazi o punti)

> **ATTENZIONE!** nel caso in cui il browser in uso non dovesse
> supportare l'attributo type="tel" (che attiva i controlli sopra
> indicati) il campo verrà gestito come un semplice campo di testo
>
> **ATTENZIONE!** I messaggi di errore visualizzati nel momento in cui
> si dovessero inserire caratteri diversi da quelli richiesti dalla
> specifica tipologia di campo possono essere personalizzati alla pagina
> "**Testi dei Componenti**" del Wizard (menu "***Sito -- Testi /
> Messaggi del sito***") selezionando il componente "**Form**"

- **Valore minimo / massimo:** visibili solo nel caso in cui il campo
  "**Tipo Valore**" sia impostato su "**Numerico**" o "**Decimale**"

> Consentono di impostare un range di validazione per il numero inserito
> a front end all'interno del corrispondente campo di input
>
> Nel momento in cui si dovesse dunque decidere di valorizzare questi
> campi, la validazione del form potrà poi avvenire con successo solo
> nel caso in cui il valore inserito a front end rientri effettivamente
> nel range definito da questi due campi
>
> In queste condizioni inoltre, in corrispondenza del campo di input,
> verrà visualizzato anche un apposito messaggio per informare l'utente
> relativamente al range di valori accettati dal campo in esame

![](./assets/media/image123.png)

- **Step:** visibile solo nel caso in cui il campo "**Tipo Valore**" sia
  impostato su "**Numerico**" o "**Decimale**"

> Consente di impostare lo step di validazione per i valori che verranno
> poi inseriti all'interno del corrispondente campo di input
>
> Nel momento in cui si dovesse dunque decidere di impostare per questo
> parametro un valore diverso da zero, la validazione del form potrà poi
> avvenire con successo solo nel caso in cui il valore inserito a front
> end sia effettivamente un multiplo dello step indicato.
>
> In queste condizioni inoltre, in corrispondenza del campo di input,
> verrà visualizzato anche un apposito messaggio per informare l'utente
> del fatto che il valore da inserire all'interno del campo dovrà essere
> necessariamente un multiplo dello step indicato.

![](./assets/media/image124.png)

> Il testo in questione potrà essere personalizzato alla pagina
> "**Gestione Testi / Messaggi del Sito** (componente "Form" campo
> "Step")
>
> Nel caso in cui l'utente non dovesse rispettare questa indicazione,
> andando quindi ad inserire un valore diverso da un multiplo dello step
> indicato, alla conferma del form verrà visualizzato un apposito
> messaggio di errore.

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

- **Campo Puffin CRM:** visualizzato solo nel caso in cui il form in
  esame sia stato correttamente abilitato per il salvataggio dei dati
  all'interno di Puffin (parametro "**Crea Contatto in Puffin CRM**"
  abilitato).

> Consente di indicare, selezionandolo dal relativo menu a tendina, lo
> specifico campo dell'anagrafica Lead di Puffin in cui dovrà essere
> salvato il dato inserito dall'utente in fase di compilazione del form
> (per maggiori informazioni relativamente a come poter creare un Lead
> su Puffin partendo da un Form Passweb si veda quanto indicato nel
> successivo capitolo "*Creazione Lead su Puffin CRM*")

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

- **Sola Lettura:** consente di stabilire se il campo in oggetto dovrà o
  meno essere in sola lettura. Selezionando quindi questo parametro, il
  corrispondente campo verrà considerato in sola lettura e l'utente non
  avrà alcuna possibilità di inserire o modificare i valori in esso
  contenuti.

> **ATTENZIONE!** L'utilizzo dei segnaposto mediante i quali poter
> precompilare il campo di testo abbinato all'applicazione del flag di
> sola lettura, potrebbe rivelarsi utile, ad esempio, nel caso in cui si
> desideri inserire un form all'interno di una pagina prodotto in
> maniera tale da consentire all'utente del sito di richiedere
> informazioni su di uno specifico articolo.

- **Minimo Caratteri:** consente di indicare il numero minimo di
  caratteri che l'utente dovrà inserire per poter validare il campo.

> Nel caso in cui dovesse essere inserito un numero di caratteri
> inferiore a quello indicato, alla conferma del form verrà visualizzato
> un apposito messaggio di errore.

- **Massimo Caratteri:** consente di indicare il numero massimo di
  caratteri che l'utente potrà digitare durante l'inserimento dei dati.

<!-- -->

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia il Campo di input)

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
> **ATTENZIONE**! Anche in questo caso l'opzione Custom, non attiva
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

