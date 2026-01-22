# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_form_res.bmp](./assets/media/image112.png){width="4.272916666666666in"
height="3.0972222222222223in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Caricamento Javascript**: se selezionato, consente di caricare il
  relativo componente in maniera asincrona al termine del caricamento
  della pagina web.

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Caricamento Javascript** e **Statico** si veda anche quanto indicato
> all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Staticizzazione e caricamento
> asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

- **Id/Name:** consente di personalizzare i selector HTML "id" e "name"
  per il componente in oggetto in modo tale da poterlo intercettare e
  personalizzare, a livello di CSS o di codice javascript, in maniera
  più semplice ed immediata.

- **Crea Contatto in Puffin CRM** -- visualizzato solo nel caso in cui
  sia stata attivata correttamente l'integrazione con Puffin CRM.

> Consente, se abilitato, di mappare i campi interni al form con i
> relativi campi delle anagrafiche Lead di Puffin
>
> Per maggiori informazioni relativamente a come poter attivare
> l'integrazione Passweb -- Puffin si veda quanto indicato all'interno
> del capitolo "*Sito -- Preferenze -- Integrazioni -- Puffin CRM*" di
> questo manuale.
>
> Relativamente a come poter creare un Lead su Puffin partendo da un
> Form Passweb si rimanda invece a quanto indicato nel successivo
> capitolo "*Creazione Lead su Puffin CRM*"

- **Tipo Valore**: consente di definire quello che dovrà essere il
  funzionamento del form impostando la specifica azione che verrà poi
  eseguita alla sua conferma. È possibile selezionare uno dei seguenti
  valori:

  - **Mail:** al salvataggio del form verrà inviata una mail, contenente
    il form compilato dall'utente sul sito, all'indirizzo specificato
    nel successivo campo "**Indirizzo e-mail**" (campo obbligatorio)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_mail_res.bmp](./assets/media/image113.png){width="4.259722222222222in"
height="3.0909722222222222in"}

> In queste condizioni sarà inoltre possibile personalizzare l'oggetto
> della mail (campo **Oggetto Mail**), il testo della Mail (campo
> **Testo Mail**) ed il Template utilizzato per realizzare questa stessa
> mail (campo **Template Mail**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_mail_componente_form.bmp](./assets/media/image114.png){width="4.9743055555555555in"
height="3.00625in"}

> Per maggiori informazioni in merito alla personalizzazione del
> template utilizzato per generare le mail inviate dal componente Form
> si veda anche il successivo capitolo "*Componente Form --
> Personalizzazione del Template delle Email*" di questo manuale

- **Csv / xml:** in questo caso i dati inserti dai vari utenti in fase
  di compilazione del form verranno salvati all'interno di un file csv /
  xml che potrà poi essere scaricato e gestito dall'apposita sezione del
  Wizard ("*Utenti -- Gestione Forms*").

> **ATTENZIONE!** Per maggiori informazioni relativamente alla gestione
> dei file csv o xml prodotti dai form si veda anche la sezione "*Utenti
> -- Gestione Forms*" di questo manuale
>
> È comunque possibile anche in queste condizioni compilare i campi
> Indirizzo Email, Oggetto / Testo / Template Mail (campi che in queste
> condizioni non sono però obbligatori) per fare in modo che oltre al
> salvataggio dei dati all'interno di un apposito file venga comunque
> inviata, all'indirizzo indicato, una mail contenente i dati del form
> compilato dall'utente sul sito.

- **Custom con evento javascript:** in questo caso sarà possibile
  intercettare l'evento di click sul pulsante di conferma del form e
  personalizzare quindi l'azione che dovrà essere eseguita alla conferma
  del form stesso. In questo senso è possibile utilizzare la libreria
  jQuery e le relative funzioni disponibili su ogni sito Passweb.

- **Custom con evento post:** selezionando questo valore sarà poi
  possibile indicare all'interno del successivo campo "**Action Post**"
  l 'url con i relativi parametri della chiamata post cui ridirigere
  l'utente una volta confermato il form stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_action_post_res.bmp](./assets/media/image115.png){width="4.2659722222222225in"
height="3.0909722222222222in"}

> **ATTENZIONE!** in queste condizioni alla conferma del form verranno
> effettuati eventuali controlli di validazione sui dati inseriti (campi
> obbligatori, numerici ecc...) e nel caso in cui tali controlli vengano
> superati correttamente verrà poi avviato il post sull' url indicato
> all'interno del campo "**Action Post**"

- **Carrello tramite file:** selezionando questa opzione sarà poi
  possibile utilizzare il form per realizzare un modulo di aggiunta
  automatica articoli in carrello tramite l'upload di un file esterno
  appositamente realizzato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_aggiunta_articoli_carrello_res.bmp](./assets/media/image116.png){width="4.253472222222222in"
height="3.0909722222222222in"}

> In queste condizioni i successivi campi **"Separatore File"** e
> "**Campi Codice**" consentiranno rispettivamente di;

- **Separatore File:** consente di indicare, selezionando una delle
  opzioni presenti all'interno del relativo menu a tendina, il carattere
  separatore dei vari campi che verrà poi utilizzato nella realizzazione
  del file contente l'elenco di articoli da aggiungere automaticamente
  in carrello.

- **Campi Codice:** consente di specificare quali informazioni potranno
  effettivamente essere presenti, nel tracciato del file di importazione
  in corrispondenza della colonna "Codice"

> **ATTENZIONE!** Per maggiori informazioni relativamente a questa
> particolare configurazione del componente Form si veda anche il
> capitolo "*Varianti Responsive -- Lista Componenti Ecommerce --
> Componente Carrello Custom -- Aggiunta articoli in carrello tramite
> file*" di questo manuale.

- **Tipo di conferma:** permette di decidere come si dovrà comportare il
  componente nel momento in cui l'utente cliccherà sul pulsante di
  conferma effettuando così il submit del form. È possibile selezionare
  uno dei seguenti valori:

  - **Con caricamento della pagina:** in queste condizioni al click sul
    pulsante di login verrà ricaricata l'intera pagina web.

  - **Senza caricamento della pagina:** in queste condizioni al click
    sul pulsante di conferma verrà ricaricato solo il componente in
    esame senza effettuare il reload dell'intera pagina web

<!-- -->

- **Azione alla conferma:** tale campo, visibile solo nel caso in cui il
  precedente parametro sia stato impostato sul valore Mail, csv, o xml,
  consente di specificare se alla conferma del form l'utente dovrà
  essere ridiretto ad una specifica pagina oppure se gli dovrà essere
  visualizzato un semplice messaggio di ringraziamento. E' quindi
  possibile selezionare uno dei seguenti valori

  - **Messaggio:** selezionando questo valore alla conferma da parte
    dell'utente dei dati immessi nel form, il form stesso scomparirà e
    al suo posto verrà visualizzato il messaggio inserito nel successivo
    campo **"Messaggio"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_form_messaggio_res.bmp](./assets/media/image117.png){width="4.980555555555555in"
height="3.0in"}

- **Pagina di Ringraziamento:** selezionando questo valore, alla
  conferma del form l'utente verrà ridiretto alla pagina selezionata nel
  sottostante albero delle pagine (**Pagina di ringraziamento**).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_form_ringraziamento_res.bmp](./assets/media/image118.png){width="4.9743055555555555in"
height="2.99375in"}

- **Posizionamento dei campi:** consente di posizionare gli elementi
  principali del componente, vale a dire il form stesso ed il pulsante
  di conferma, secondo uno schema prestabilito. E' possibile selezionare
  uno dei seguenti valori:

  - Affiancati a destra

  - Affiancati a sinistra

  - Affiancati e giustificati

  - Affiancati e opposti

  - Centrati e affiancati

  - Centrati e Incolonnati

  - Incolonnati a destra

  - Incolonnati a sinistra

  - Custom

> Supponendo dunque di selezionare l'opzione "**Affiancati a Sinistra**"
> gli elementi principali del componente, il form e il pulsante di
> conferma, si posizioneranno un a fianco all'altro a partire dal bordo
> sinistro dell'elemento in cui sono contenuti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\posizionamento_elementi_form.bmp](./assets/media/image119.png){width="5.110416666666667in"
height="2.870138888888889in"}

> Selezionando invece l'opzione "Centrati e Incolonnati" i due elementi
> si posizioneranno al centro del loro elemento padre uno sotto
> all'altro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\posizionamento_elementi_form_2.bmp](./assets/media/image120.png){width="5.110416666666667in"
height="2.870138888888889in"}

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento dei campi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** consente di definire
  l'ordine di visualizzazione degli elementi principali del componente
  in esame, permettendo dunque, già in fase di configurazione del
  componente di decidere se dovrà essere visualizzato prima il form e
  poi il pulsante di conferma o viceversa.

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
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali" di questo
manuale.

**Il componente Form è a tutti gli effetti un Componente di tipo
Contenitore e come tale va trattato e gestito**

In particolare all'interno di un componente di tipo Form sarà possibile
inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il Componente "Form".

- **Componenti per il Form:** contiene tutta una serie di controlli che
  potranno essere utilizzati per definire i vari campi del form .

L'inserimento di questi componenti all'interno del Form avverrà
utilizzando le solite tecniche (Drag and Drop o Point and Click) già
esaminate all'interno di questo manuale (per maggiori informazioni in
questo senso si rimanda allo specifico capitolo).

