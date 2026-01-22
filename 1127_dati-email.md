# DATI EMAIL



All'interno della sezione "**Dati Email**" è possibile, come
precedentemente evidenziato, indicare in tutte le lingue gestite
all'interno del sito, i contenuti delle e-mail transazionali inviate in
automatico dall'applicazione in corrispondenza dei diversi possibili
stati assunti dagli ordini all'interno del sito e-commerce.

![](./assets/media/image617.png)

Per ciascuna mail sarà possibile indicare i seguenti dati:

**Utenti Email di ... (solo Ecommerce Mexal):** consente di specificare
le tipologie di utenti cui dovrà essere inviata la corrispondente Email,
**indipendentemente dal fatto che l'ordine venga poi generato
direttamente da un cliente o, per suo conto, da parte di un Agente**.

E\' possibile selezionare uno dei seguenti valori:

- **Cliente e Agente intestatario Ordine:** la corrispondente mail verrà
  inviata al Cliente e all'Agente intestatari del documento (per
  **Agente intestatario del documento** si intende l'Agente presente in
  testata del corrispondente documento Mexal e quindi l' Agente che ha
  realmente effettuato l'ordine per conto del cliente)

- **Cliente, Agente intestatario Ordine e Agente associato al Cliente:**
  la corrispondente mail verrà inviata al Cliente intestatario del
  documento, all'Agente intestatario del documento e all'Agente
  associato in Mexal al cliente intestatario del documento stesso(che
  può non coincidere, soprattutto in una gestione gerarchica di Agenti e
  Sotto Agenti, con l'Agente intestatario del documento)

- **Cliente:** la corrispondente mail verrà inviata al cliente
  intestatario del documento

- **Agente intestatario Ordine:** la corrispondente mail verrà inviata
  all'Agente intestatario del documento

- **Agente intestatario Ordine e Agente associato al Cliente:** la
  corrispondente mail verrà inviata all'Agente intestatario del
  documento e all'Agente associato, in Mexal, al cliente intestatario
  del documento stesso

- **Agente intestatario Ordine e Agenti gerarchia:** la corrispondente
  mail verrà inviata all'Agente intestatario dell'ordine e a tutti gli
  Agenti che sono collocati, rispetto ad esso, ad un livello gerarchico
  superiore nella gerarchia agenti in uso all'interno del sito

- **Agente intestatario Ordine, Agente associato al cliente e Agenti
  gerarchia:** la corrispondente mail verrà inviata all'Agente che ha
  effettuato l'ordine, all'Agente associato, in Mexal, al cliente
  intestatario del documento e agli Agenti che, rispetto ad essi, sono
  collocati ad un livello gerarchico superiore nella gerarchia agenti in
  uso all'interno del sito

- **Cliente, Agente intestatario Ordine e Agenti gerarchia:** la
  corrispondente mail verrà inviata al cliente intestatario del
  documento, all'Agente intestatario dell'ordine e a tutti gli Agenti
  che sono collocati, rispetto ad esso, ad un livello gerarchico
  superiore nella gerarchia agenti in uso all'interno del sito

- **Cliente, Agente intestatario Ordine, Agente associato al cliente e
  Agenti gerarchia:** la corrispondente mail verrà inviata al cliente
  intestatario del documento, all'Agente che ha effettuato l'ordine,
  all'Agente associato, in Mexal, al cliente intestatario del documento
  e agli Agenti che, rispetto ad essi, sono collocati ad un livello
  gerarchico superiore nella gerarchia agenti in uso all'interno del
  sito

**Oggetto E-Mail di ...:** consente di specificare l'oggetto della
corrispondente Email.

**Testo E-Mail di ...:** consente di definire il contenuto della
corrispondente Email. Il pulsante "**Sorgente**" presente nella barra
degli strumenti dell'editor di testo consente di editare il corpo della
mail lavorando direttamente a livello di codice HTML.

Il Check "**Allegati**" presente in corrispondenza di tutte le diverse
tipologie di Mail presenti all'interno di questa sezione, ad eccezione
delle sole mail relative alla "**Lista Regalo**"

![](./assets/media/image618.png)

consente invece di indicare se alle mail di quella determinata tipologia
dovranno essere allegati o meno anche tutti i file che hanno il campo
"**Mail**" impostato sul valore S

![](./assets/media/image619.png)

In questo senso è bene ricordare che:

- gli allegati ad un determinato ordine inseriti sul Front End dagli
  utenti del sito, avranno sempre il campo "Mail" impostato a S.

- i file allegati al documento operando da Docuvision (solo Ecommerce
  Mexal) avranno il campo Mail impostato a S solo nel caso in cui siano
  documenti di tipo "Stampa"

- per i file allegati ad un determinato documento operando direttamente
  dal Wizard di Passweb il campo Mail è impostabile direttamente in fase
  di upload dell'allegato stesso e, a differenza degli allegati inseriti
  da Front End e/o di quelli inseriti da Docuvision, potrà essere
  modificato in un qualsiasi momento.

Per maggiori informazioni relativamente a come poter allegare file ad un
ordine operando direttamente dal Wizard di Passweb si veda anche il
successivo capitolo "*Gestione Ordini -- Allegati Ordine*" di questo
manuale.

Il campo "**Indirizzi Email in CCN**" presente solo per le mail di
"**Conferma Ordine**" e di "**Evasione Ordine**" consente di indicare
uno o più indirizzi email (separati da ; ) cui inoltrare in copia
nascosta la relativa mail.

**ATTENZIONE!** Questo campo, assieme al segnaposto "**Se Mail Conferma
Ordine**" utilizzabile in fase di costruzione delle mail, può tornare
particolarmente utile soprattutto nel momento in cui si debbano gestire
integrazioni con servizi di recensioni (come ad esempio Trsustpilot )
che, per automatizzare il processo, possono richiedere la ricezione
delle mail legate agli ordini effettuati sul sito, magari inserendo
anche al loro interno specifici metadati (per maggiori informazioni
relativamente all'utilizzo dei segnaposto condizionali in fase di
definizione delle mail ordine si veda anche il successivo capitolo
"*Personalizzazione del template di ordini / bolle / fatture*" di questo
manuale)

Il pulsante "**Aggiungi Segnaposto**" anch'esso presente in
corrispondenza di ogni campo di tipo "**Oggetto Email**" e "**Testo
Email**",

![](./assets/media/image620.png)

Consente, infine, di personalizzare l'oggetto e/o il testo della
relativa mail inserendo appositi segnaposto che verranno poi valorizzati
dinamicamente da Passweb a seconda, ad esempio, di chi effettua
l'ordine, di dove viene inviata la merce, del tipo di documento generato
ecc...

Nello specifico per comporre l'oggetto delle mail presenti all'interno
di questa sezione del Wizard è possibile utilizzare i seguenti
segnaposto:

- **Agente (solo Ecommerce Mexal):** verrà sostituito, in fase di
  creazione della mail, con il nominativo dell'eventuale agente
  associato al relativo documento.

- **Cliente:** verrà sostituito, in fase di creazione della mail, con il
  nominativo del cliente cui è destinata la merce

- **Cliente di fatturazione:** verrà sostituito, in fase di creazione
  della mail, con il nominativo del cliente che ha effettuato l'ordine

- **Data:** verrà sostituito, in fase di creazione della mail, con la
  data di emissione relativo documento

- **Documenti di Origine:** nel caso in cui l'ordine in questione
  dovesse essere trasformato prima in bolla e successivamente in
  fattura, questo segnaposto verrà sostituito, in fase di creazione
  della mail, con la sigla della bolla che ha generato la relativa
  fattura.

- **Documenti Ordine di Origine:** verrà sostituito, in fase di
  creazione della mail, con la / le sigla/e dei documenti "Ordine" che
  hanno generato il documento in esame. Tale segnaposto potrà quindi
  essere utilizzato, ad esempio, nella mail di evasione per indicare
  l'ordine o gli ordini che hanno generato la relativa bolla / fattura

- **Indirizzo:** verrà sostituito, in fase di creazione della mail, con
  l'indirizzo di spedizione della merce

- **Nome del sito:** verrà sostituito, in fase di creazione della mail,
  con il nome assegnato al proprio sito web

- **Numero Documento:** verrà sostituito, in fase di creazione della
  mail, con l'identificativo Passweb del relativo documento

- **Se il documento è un preventivo:** nel momento in cui si dovesse
  decidere di utilizzare questo segnaposto, all'interno del campo in
  esame verrà inserita la seguente istruzione condizionale

> **\$if(isquotation)\$ \$else\$ \$endif\$**
>
> mediante la quale poter differenziare l'oggetto delle mail a seconda
> del fatto che il relativo documento sia un ordine oppure un
> preventivo.
>
> Nello specifico, il testo da utilizzare nel caso in cui il documento
> in questione dovesse essere un preventivo andrà inserito tra le due
> istruzioni \$if(isquotation)\$ e \$else\$, mentre il testo da
> visualizzare nel caso in cui il documento dovesse essere un ordine
> andrà inserito tra le istruzioni \$else\$ e \$endif\$ come
> nell'esempio qui di seguito riportato:
>
> \$if(isquotation)\$ **Oggetto della mail generata da un preventivo**
> \$else\$ **Oggetto della mail generata da un ordine** \$endif\$

![](./assets/media/image621.png)

> Ovviamente **all'interno della condizione if è possibile utilizzare
> sia del semplice testo** (come nel caso sopra evidenziato) **sia altri
> segnaposto** in maniera tale, ad esempio, da visualizzare nell'oggetto
> della mail l'indirizzo di spedizione merce solo nel caso in cui il
> documento prodotto sia effettivamente un ordine.

- **Se l'utente è un Privato / Pubblica amministrazione / Azienda:** nel
  momento in cui si dovesse decidere di utilizzare uno di questi
  segnaposto, all'interno del campo in esame verrà inserita,
  rispettivamente la seguente istruzione condizionale

> **\$if(isuserprivate)\$ \$endif\$**
>
> **\$if(isuserpubliccompany)\$ \$endif\$**
>
> **\$if(isusercompany)\$ \$endif\$**
>
> mediante la quale poter differenziare l'oggetto delle mail a seconda
> del fatto che l'utente destinatario sia un Privato, una Pubblica
> Amministrazione o un utente di tipo Azienda.
>
> Anche in questo caso, ovviamente, il testo da inserire nel momento in
> cui l'utente dovesse essere, ad esempio, un Privato dovrà essere
> posizionato tra l' istruzioni \$if(isuserprivate)\$ e l'istruzione
> \$endif\$

- **Sigla Documento:** verrà sostituito, in fase di creazione della
  mail, con la sigla associata dal gestionale al relativo documento

- **Url del Sito:** verrà sostituito, in fase di creazione della mail,
  con l' url del proprio sito web

**ATTENZIONE!** A default nell'oggetto delle varie mail vengono
automaticamente inseriti i segnaposto relativi al Cliente, all' Agente e
all'Indirizzo di spedizione della merce.

Per quel che riguarda invece il testo delle mail, oltre ai segnaposto
appena analizzati, sarà possibile utilizzare anche il segnaposto
**"Dettaglio Documento"**

In questo senso è bene ricordare che il testo delle mail, configurabili
all'interno dei questa sezione del Wizard, è composto, essenzialmente,
da due distinti elementi:

- Un "**Testo libero**"

- **Il dettaglio del documento**, ossia i dati relativi allo specifico
  ordine (elenco di articoli, totali, indirizzi di spedizione ecc...)

Il "Testo Libero" può essere inserito, gestito e personalizzato,
direttamente all'interno del relativo campo "Testo Email di...".

Il Dettaglio del documento, invece, può essere personalizzato sempre
dalla pagina "Configurazione Parametri dell'Ordine", all'interno però
della sezione "Documento". Per maggiori informazioni in merito si vedano
anche i successivi capitoli di questo manuale.

Una volta definito e personalizzato il dettaglio del documento, questo
potrà poi essere inserito in una qualsiasi posizione del corpo della
relativa mail utilizzando, appunto, il segnaposto "Dettaglio Documento"
evidenziato in figura.

**ATTENZIONE!** Nel caso in cui si decida di non utilizzare nel testo di
una mail il segnaposto "Dettaglio Documento" i dati del relativo
documento verranno inseriti come ultimo elemento della corrispondente
mail

**NOTA BENE:** per attivare l'invio di una mail connessa ad un
particolare stato dell'ordine è sufficiente specificare per essa un
oggetto. Nel caso in cui non venga indicato nessun oggetto la relativa
mail non verrà inviata.

Per maggiori informazioni relativamente alle diverse tipologie di mail
transazionali gestite da Passweb si veda anche il successivo capitolo di
questo manuale

##### EMAIL TRANSAZIONALI

Di seguito sono indicate le diverse tipologie di Mail gestite da Passweb
ed inviate in maniera automatica nel momento in cui l'ordine andrà ad
assumere un determinato stato.

**[E-MAIL DI INVIO ORDINE]{.underline}**

Mail inviata, subito dopo aver effettuato l\'ordine.

Nel caso in cui si sia deciso di inviare questa mail al cliente
intestatario del documento, questa stessa mail verrà inviata anche ad
eventuali indirizzi mail associati all'indirizzo di spedizione merce
selezionato. Allo stato attuale l\'ordine è memorizzato ancora solamente
all\'interno del database di Passweb e si trova nello stato di
\"**NUOVO** \"

**[E-MAIL DI CONFERMA ORDINE]{.underline}**

Mail inviata nel momento in cui l'ordine verrà inserito sul gestionale.

Nel caso in cui si sia deciso di inviare questa mail al cliente
intestatario del documento, questa stessa mail verrà inviata anche ad
eventuali indirizzi mail associati all'indirizzo di spedizione merce
selezionato. Allo stato attuale l\'ordine sarà memorizzato sul database
di Passweb e anche all\'interno del gestionale.

In Passweb si troverà nello stato di \"**MEMORIZZATO**\".

**[E-MAIL DI SOSPENSIONE ORDINE]{.underline}**

Mail inviata quando, sul gestionale, almeno una riga dell\'ordine si
trova nello stato di Sospeso.

Nel caso in cui si sia deciso di inviare questa mail al cliente
intestatario del documento, questa stessa mail verrà inviata anche ad
eventuali indirizzi mail associati all'indirizzo di spedizione merce
selezionato.

In Passweb l\'ordine si troverà nello stato **SOSPESO**.

**[E-MAIL DI SOSTITUZIONE ORDINE]{.underline}**

Mail inviata nel momento in cui, dopo una sincronizzazione, dovesse
essere riscontrato un conflitto dovuto alla modifica contemporanea dello
stesso \"Ordine Sospeso\" sia all\'interno del gestionale che
all\'interno del sito web (vedi anche pagina *\"Ordini - Stati
dell\'Ordine\"* di questo manuale).

Nel caso in cui si sia deciso di inviare questa mail al cliente
intestatario del documento, questa stessa mail verrà inviata anche ad
eventuali indirizzi mail associati all'indirizzo di spedizione merce
selezionato.

In Passweb l\'ordine si troverà nello stato **SOSPESO**.

**[E-MAIL DI EVASIONE ORDINE]{.underline}**

Mail inviata subito dopo la sincronizzazione successiva all\'evasione
dell\'ordine (indipendentemente dal fatto che l\'evasione avvenga
tramite bolla o tramite fattura). Nel caso di evasioni parziali verranno
inviate più mail di evasione.

Nel caso in cui si sia deciso di inviare questa mail al cliente
intestatario del documento, questa stessa mail verrà inviata anche ad
eventuali indirizzi mail associati all'indirizzo di spedizione merce
selezionato.

**ATTENZIONE!** **La mail di Evasione potrà essere inviata solo ed
esclusivamente in relazione ad ordini che sono presenti su Passweb anche
nello stato di "Trasformato"**

Ciò significa dunque che nel momento in cui l'ordine dovesse nascere
direttamente nel gestionale dove verrà poi trasformato in bolla o
fattura, l'esportazione sul sito di tali bolle / fatture non produrrà
l'invio di nessuna mail di evasione.

Allo stesso modo se il documento di origine proveniente dal sito dovesse
essere un preventivo e tale preventivo dovesse essere trasformato
direttamene in bolla / fattura senza passare dall'ordine e, soprattutto,
senza esportare prima l'ordine all'interno del sito, non potrà essere
inviata da Passweb nessuna mail di evasione.

**[E-MAIL DI ANNULLAMENTO ORDINE]{.underline}**

Mail inviata nel momento in cui:

- dopo una sincronizzazione l'ordine dovesse trovarsi nello stato di
  "Annullato"

- si dovesse decidere di annullare da Wizard (pulsante "**Annulla
  Ordine**") un ordine inizialmente posto nello stato di "Pagamento non
  confermato".

**[E-MAIL DI FUORI FIDO -- SOLO ECOMMERCE MEXAL]{.underline}**

Mail inviata nel momento in cui, in fase di inserimento ordine sul
gestionale, dovesse essere ritornato da Mexal l'errore "**Cliente Fuori
Fido**"

Nello specifico l'errore in questione verrà ritornato quando:

- in Mexal il cliente che ha effettuato l'ordine risulta essere fuori
  fido

- il parametro "**Messaggio fuori fido doc. magazzino**" presente nella
  maschera "**Progressivi**" del relativo cliente è impostato su
  "**Bloccante**"

![](./assets/media/image622.png)

In queste condizioni, inoltre, l'ordine verrà portato nello stato di
"**Pagamento non confermato**" e potrà essere Annullato, Eliminato o
Confermato dall'amministratore, operando direttamente dal Wizard,
esattamente come avviene per tutti i documenti che si trovano in questo
specifico stato (per maggiori informazioni in merito si veda ad esempio
quanto indicato nei capitoli di questo manuale relativi ai pagamenti
online)

**[E-MAIL DI NOTIFICA ALLEGATO]{.underline}**

Mail di notifica inviata ai destinatari indicati all'interno del campo
"Utenti Email Notifica Allegato", nel momento in cui, operando
direttamente dal Wizard di Passweb, dovessero essere aggiunti ad un
determinato ordine dei nuovi allegati con il flag "**Notifica Utente**"
selezionato.

![](./assets/media/image623.png)

**ATTENZIONE!** Nel caso in cui, in fase di inserimento di un nuovo
allegato da Wizard, non dovesse essere selezionato il flag "Notifica
Utente", indipendentemente dal fatto di aver configurato o meno la mail
di Notifica non verrà comunque inviata ai destinatari indicati nessun
tipo di comunicazione.

**[LISTA REGALO]{.underline}**

Mail inviata al gestore della relativa Lista Regalo nel momento in cui
un ordine originato a partire da essa dovesse essere memorizzato (stato
"Confermato") sul gestionale

**NOTA BENE:** per maggiori informazioni relativamente ai diversi
possibili stati che potrà assumere un ordine all'interno del sito
e-commerce, si veda anche il successivo capitolo "Stati dell'Ordine".

