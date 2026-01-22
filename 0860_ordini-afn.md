# ORDINI AFN



Come già evidenziato nei precedenti capitoli di questo manuale
**relativamente ad ordini contenenti articoli gestiti in modalità AFN,
per ragioni di privacy, Amazon non fornisce a piattaforme esterne dati
inerenti ad esempio il nominativo o l'indirizzo dell'utente che ha
effettuato l'ordine sul Marketplace**.

Questo tipo di ordini potranno comunque essere acquisiti da Passweb
(secondo le stesse modalità in uso per ordini MFN) ma, in conseguenza di
quanto appena detto, saranno ovviamente incompleti e prima di poterli
trasferire al gestionale sarà quindi necessario inserire manualmente i
dati mancanti

In particolare nel momento in cui dovessero essere individuati, a
seguito di una sincronizzazione, ordini provenienti da Amazon con
articoli gestiti in modalità AFN (e in conseguenza di ciò incompleti),
Passweb provvederà a:

- mettere questi stessi ordini nello stato di "**Incompleto da Logistica
  Amazon**"

- inviare all'amministratore del sito un' apposita mail contenente tutti
  i riferimenti relativi a questi stessi ordini.

In queste condizioni, di base, per poter completare l'ordine, in maniera
tale da poterlo poi inserire sul gestionale, sarà necessario:

- accedere alla sezione "**Ordini -- Gestione Ordini**" del Wizard e
  individuare gli ordini incompleti filtrando, ad esempio, sulla base
  dello stato "**Incompleto da Logistica Amazon**"

- prendere nota della mail (del tipo
  **cw3sd2sbxjqz7rm@marketplace.amazon.it**) presente in corrispondenza
  di questi ordini in maniera tale da poterla poi utilizzare come chiave
  di ricerca tra tutti gli utenti del proprio sito ecommerce

> **ATTENZIONE!** I dati mancanti che impediscono all'ordine di poter
> essere trasferito sul gestionale sono relativi infatti al cliente
> intestatario del relativo documento

- portarsi alla sezione "**Utenti -- Utenti Sito**" del Wizard e
  individuare, mediante la mail annotata al punto precedente, l'utente
  intestatario dell'ordine Amazon che risulta essere incompleto

- completare l'anagrafica dell'utente individuato al punto precedente
  inserendo i dati mancanti (**Nome e Indirizzo**), dati questi che
  potranno essere prelevati direttamente dal back end del proprio
  account Amazon

- portarsi nuovamente all'interno della sezione "**Ordini -- Gestione
  Ordini**" del Wizard, selezionare l'ordine in relazione al quale è
  stata appena completata l'anagrafica dell'intestatario e cliccare sul
  pulsante "**Conferma Ordine Incompleto**" presente nella contestuale
  barra degli strumenti

> In questo modo verrà avviata una sincronizzazione parziale (che non
> andrà ad intaccare il monte sincronizzazioni previsto da contratto) a
> seguito della quale l'ordine in esame verrà correttamente trasferito
> sul gestionale.
>
> **ATTENZIONE!** Nel caso in cui si dovesse tentare di utilizzare il
> pulsante "**Conferma Ordine Incompleto**" in relazione ad ordini per i
> quali non è stata ancora completata l'anagrafica del utente
> intestatario, verrà visualizzato un apposito messaggio di errore
>
> In queste condizioni, ovviamente, l'ordine in esame **non** verrà poi
> inserito sul gestionale

Nel momento in cui si volesse comunque acquisire in maniera automatica
anche questi ordini incompleti, ad esempio perché l'unica esigenza in
merito ad essi è quella di averli nel gestionale per poter così
aggiornare in maniera corretta i progressivi degli articoli, sarà
necessario attivare il relativo modulo presente su Passstore (**Amazon
Gestione Ordini AFN**)

L'attivazione di questo modulo abiliterà infatti il campo "**Codice
Cliente per Ordini Incompleti da Logistica Amazon**" presente nella
maschera di configurazione del proprio Account Amazon (sezione
"**Ordini**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_gestione_ordini_afn.bmp](./assets/media/image305.png){width="5.428472222222222in"
height="3.292361111111111in"}

campo questo all'interno del quale poter inserire il codice conto di un
utente del gestionale cui verranno associati in maniera automatica tutti
gli ordini Amazon che si troveranno nello stato "**Incompleto da
Logistica Amazon**"

In questo modo dunque anche tutti gli ordini prelevati dal Marketplace
che dovessero contenere articoli gestiti in modalità AFN e che non
dovessero avere quindi dati quali indirizzo o nominativo dell'utente che
ha effettuato l'ordine verranno comunque inseriti in maniera automatica
all'interno del gestionale (posto ovviamente che il codice conto
indicato all'interno del campo in oggetto corrisponda effettivamente a
quello di un utente correttamente codificato all'interno del
gestionale).

**Ovviamente il cliente cui verranno intestati questi documenti dovrà
essere un cliente fittizio che non potrà in alcun modo corrispondere a
chi ha realmente effettuato l'ordine sul marketplace**

Di base questo non dovrebbe comunque essere un problema perché questa
particolare tipologia di ordini, come precedentemente evidenziato, è
gestita, al livello di spedizione, direttamente da Amazon stessa.

**In ogni caso non sarà ovviamente corretto emettere, all'interno del
gestionale, eventuali fatture fiscali relative a questi ordini** **e
quindi l'unico scopo per cui può essere effettivamente utile abilitare
il modulo in questione e la relativa gestione, è quello di generare
comunque in maniera automatica gli ordini all'interno del gestionali per
ottenere un corretto aggiornamento dei progressivi e delle relative
quantità tanto all'interno di Mexal / HoReCa quanto all'interno del
Marketplace**

Un'ultima considerazione molto importante da fare è quella che riguarda
il comportamento dell'applicativo nel momento in cui si dovesse attivare
il modulo Passstore **Amazon Gestione Ordini AFN** senza però andare poi
ad inserire un codice cliente all'interno del campo "**Codice Cliente
per Ordini Incompleti da Logistica Amazon**".

In queste condizioni infatti Passweb tenterà comunque di inserire in
maniera automatica gli ordini incompleti all'interno del gestionale ma
non potendo associarli ad uno specifico cliente fittizio tenterà di
creare per ogni ordine una singola anagrafica cliente utilizzando i dati
presenti nell'ordine stesso.

Nello specifico se tra i dati presenti nell'ordine acquisto da Amazon
dovesse essere presente:

- Nome e Cognome ed email del cliente tali dati verranno utilizzati per
  cerare una nuova anagrafica gestionale

- Solo l'email nel formato corretto, verrà effettuato uno split tra
  quello che sta prima e dopo la @. La parte prima della @ verrà
  utilizzata come Nome della nuova anagrafica cliente creata all'interno
  del gestionale, la parte dopo la @ come cognome

- Solo l'email ma in un formato non standard (quindi senza @), la nuova
  anagrafica cliente creata all'interno del gestionale avrà Nome =
  Cognome = Email

Considerando comunque che potrebbe anche verificarsi il caso in cui tra
i dati ritornati da Amazon non sia presente né il Nome né il Cognome e
neppure l'email dell'utente che ha effettuato l'ordine, che se anche
tali dati fossero presenti la mail potrebbe essere tipicamente in un
formato criptato del tipo <6k8yh125dtgmzxj@marketplace.amazon.it> e che,
in ogni caso, mancheranno tutti i dati relativi alla spedizione (che,
come detto, per questi ordini sarà gestita interamente da Amazon) è
semplice comprendere come in queste condizioni l'importazione automatica
di questo tipo di ordini all'interno del gestionale potrebbe essere
utile solo ed esclusivamente per l'aggiornamento delle quantità dei
prodotti.

**Sotto questo aspetto si consiglia quindi di utilizzare sempre un
cliente fittizio (in maniera tale da non creare inutilmente anagrafiche
clienti all'interno del gestionale) valorizzando adeguatamente il campo
"Codice Cliente per Ordini Incompleti da Logistica Amazon".**

