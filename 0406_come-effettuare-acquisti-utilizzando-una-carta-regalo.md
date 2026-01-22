# COME EFFETTUARE ACQUISTI UTILIZZANDO UNA CARTA REGALO



Come più volte evidenziato in Passweb è possibile gestire diverse
tipologie di Gift Card:

- Gift Card Fisiche

- Gift Card Virtuali

- Gift Card di tipo Ho.Re.Ca.

A seconda della tipologia considerata, il processo di creazione e
gestione di queste carte regalo può essere differente.

Per maggiori informazioni relativamente alle modalità di attivazione e
di gestione delle Gift Card Ho.Re.Ca. si rimanda a quanto indicato nel
relativo capitolo di questo manuale ("*Utenti -- Gift Card -- Gift Card
Ho.Re.Ca.*")

Per quel che riguarda invece le Gift Card Fisiche e Virtuali le
principali differenze riguardano più che altro il processo di creazione
e di attivazione dei relativi codici.

Lato utente invece il procedimento mediante il quale poter riscattare il
codice di una Gift Card Fisica o Virtuale e, soprattutto, quello
mediante il quale poterla utilizzare per effettuare acquisti all'interno
del sito è piuttosto uniforme.

Quello che può cambiare da un caso (Gift Card Fisiche) all'altro (Gift
Card Virtuali) è relativo, più che altro, alle modalità di riscatto del
codice della Gift Card.

Nello specifico il processo di gestione di una **Gift Card Virtuale**
prevede che l'acquirente, ad un certo punto, condivida con l'effettivo
beneficiario della carta regalo il suo link di attivazione.

Tale link può essere reperito in diversi modi:

- Può essere inserito nella mail di attivazione che viene inviata
  all'acquirente nel momento stesso in cui viene esportata sul sito la
  fattura / corrispettivo di acquisto della Gift Card (per maggiori
  informazioni in merito si veda anche la sezione "*Utenti -- Gift Card
  -- Dati Emai*l" di questo manuale)

- Lo si può ottenere visualizzando sul front end del sito il dettaglio
  del documento di acquisto della relativa Gift Card (per maggiori
  informazioni in merito si veda anche la sezione "*Varianti Sito
  Responsive -- Lista Componenti Ecommerce -- Componente Ordini --
  Codici Gift Card*" di questo manuale)

- L'amministratore del sito ha la possibilità di ottenere il link di
  condivisione anche all'interno del Wizard dalla maschera di gestione
  dei codici Gift Card (per maggiori informazioni in merito si veda
  anche la sezione "*Utenti -- Gift Card -- Codici*" di questo manuale)

**ATTENZIONE!** ottenuto il link di condivisione sarà poi compito
dell'acquirente condividerlo con l'effettivo beneficiario della carta
regalo utilizzando il canale che meglio crede (mail, applicazioni di
messaggistica, social ...)

Dall'altro lato il beneficiario della carta regalo una volta ricevuto il
link di attivazione dovrà semplicemente cliccarci sopra e verrà
automaticamente ricondotto alla pagina Gift Card del sito, pagina questa
all'interno della quale dovrà essere inserito il componente Gift Card
che l'utente andrà poi ad utilizzare per riscattare il proprio codice.

In questo senso è bene sottolineare che il componente Gift Card sarà
visibile, all'interno dell'omonima pagina, solo dopo aver effettuato
l'autenticazione per cui l'utente che accede per la prima volta al sito
per riscattare il suo codice dovrà essere messo nelle condizioni di
ricevere questo tipo di informazione (utilizzando ad esempio un
messaggio del tipo "Per riscattare la tua carta regalo devi essere
autenticato") e, soprattutto, dovrà essere messo nelle condizioni di
poter effettuare la registrazione / autenticazione al sito.

![](./assets/media/image247.png)

Una volta effettuata l'autenticazione verrà visualizzato il componente
"Gift Card" suddiviso in due distinte sezioni:

![](./assets/media/image248.png)

Nella parte bassa verrà visualizzata una tabella contenente l'elenco dei
codici Gift Card già riscattati dall'utente in esame (con il relativo
importo, stato e data di scadenza) e il saldo attuale dato dalla somma
dei residui delle Gift Card ancora attive.

Nella parte alta del componente invece, all'interno della sezione
"**Buono Regalo**" verrà visualizzato il "**Dettaglio della Gift Card**"
secondo quelli che sono i dati inseriti all'interno della sezione
"**Template**" presente nella maschera di creazione e gestione delle
Gift Card

![](./assets/media/image249.png)

Per maggiori informazioni in merito alla creazione e alla gestione del
"Template" utilizzato per il "Dettaglio della Gift Card" si veda anche
quanto indicato all'interno della sezione "*Utenti -- Gift Card --
Template"* di questo manuale.

Il pulsante "**Applica al tuo Account**", presente all'interno della
sezione "Buono Regalo" permetterà all'utente di riscattare il codice
della carta regalo e di caricare sul proprio account il relativo importo

**ATTENZIONE!** La sezione "Buono Regalo" verrà visualizzata solo ed
esclusivamente nel caso in cui l'accesso alla pagina Gift Card del sito
avvenga a partire da un "link di condivisione"

In questo senso può essere interessante sottolineare come l'utilizzo di
un set di opzioni di personalizzazione (custom option) gestito sulle
Gift Card potrebbe consentire all'acquirente di personalizzare il
"Dettaglio della Gift Card". Si potrebbe pensare, ad esempio, di gestire
nel set di opzioni (e di inserire quindi anche all'interno del
"Template") un campo di testo e un campo immagine che l'acquirente
andrebbe poi a completare con un messaggio e un'immagine personalizzata
da mostrare al beneficiario nel momento in cui questo andrà a riscattare
il suo codice partendo dal link di condivisione.

Nel caso di **Gift Card Fisiche** invece si presuppone che il codice da
riscattare sia stato stampato direttamente sulla carta regalo che viene
poi spedita / consegnata al beneficiario. In queste condizioni dunque
non ci sono link di condivisione e il beneficiario, una volta ottenuto
il codice, dovrà quindi accedere alla pagina Gift Card del sito (anche
in questo caso previa autenticazione) dove potrà utilizzare il
componente "Gift Card" da noi inserito per riscattarlo.

![](./assets/media/image250.png)

Non essendo partiti, come detto, da un link di condivisione all'interno
del componente "Gift Card" non sarà presente la sezione "Buono Regalo"
ma solamente la tabella contenente l'elenco dei codici Gift Card già
riscattati dall'utente.

In queste condizioni dunque per riscattare il proprio codice l'utente
dovrà semplicemente inserirlo all'interno del campo "**Codice Buono
Regalo**" e cliccare poi sul pulsante "**Applica al tuo account**"

**ATTENZIONE!** **ogni Codice Gift Card è applicabile ad un unico
account cliente**. Nel momento in cui si tentasse dunque di riscattare
un codice che è già stato riscattato ed associato ad un altro account
utente, verrà visualizzato un apposito messaggio di errore.

Nulla vieta ovviamente di utilizzare il campo "**Codice Buono Regalo**"
anche nel caso di riscatto di un codice collegato ad una Gift Card
Virtuale, anche se, ovviamente, questo presuppone il fatto di
condividere con il beneficiario non il link di attivazione ma
direttamente il codice della carta regalo.

In ogni caso una volta riscattato un codice questo verrà aggiunto alla
tabella contenente l'elenco dei codici già riscattati e associati
all'account dell'utente in esame. Per ciascuno dei codici presenti in
questa tabella verranno visualizzate le seguenti informazioni:

- Codice della Gift Card riscattato

- Importo iniziale della Gift Card

- Saldo attuale della Gift Card

- Scadenza della Gift Card

- Stato della Gift Card

Oltre a queste informazioni nella parte alta della tabella verrà sempre
indicato anche il **saldo totale**, ossia l'importo effettivamente
utilizzabile per effettuare acquisti all'interno del sito, dato dalla
**somma dei residui delle Gift Card ancora attive**.

Infine per ciascuno dei codici in tabella è presente anche un pulsante
"**Transazioni**" che consente di accedere all'elenco di tutte le
operazioni che sono state fatte in relazione al codice in esame.

![](./assets/media/image251.png)

Nello specifico su ogni singolo codice Gift Card possono essere
effettuate operazioni di tre tipi diversi:

- **Aggiunta della carta regalo all'account**: evento che si verifica
  nel momento in cui l'utente utilizzerà il pulsante "**Applica al tuo
  Account**" per riscattare il codice in esame:

- **Transazione**: evento che si verifica nel momento in cui un utente
  utilizzerà il saldo della corrispondente carta regalo per effettuare
  acquisti all'interno del sito. In questo caso è presente anche un link
  diretto al dettaglio dell'ordine in cui è stato effettivamente
  utilizzato quel saldo.

- **Variazione amministrativa**: evento che si verifica nel momento in
  cui l'amministratore del sito dovesse decidere di variare da Wizard il
  residuo della corrispondente carta regalo

I testi descrittivi delle diverse tipologie di transazione possono
essere personalizzati all'interno della sezione "Testi/Messaggi Sito"
agendo sul componente "Gift Card".

Una volta riscattato il Codice Gift Card e caricato sul proprio account
l'importo della carta regalo, questo potrà poi essere utilizzato per
effettuare acquisti all'interno del sito.

In questo senso, già in Carrello l'utente può avere la possibilità di
visualizzare, all'interno della sezione "**Gift Card**", l'importo
effettivamente utilizzabile su quel determinato ordine (per maggiori
informazioni relativamente a come poter attivare in Carrello la sezione
"Gift Card" si veda anche quanto indicato all'interno del capitolo
"*Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componente
Carrello Custom -- Configurazione*" di questo manuale)

![](./assets/media/image252.png)

Ovviamente però l'effettivo utilizzo del saldo Gift Card sull'ordine in
esame avverrà all'interno del componente Checkout.

In questo senso è bene sottolineare che mentre nel componente Carrello
la visibilità del check "Usa il saldo" è subordinata alla configurazione
del parametro "Visualizza saldo Gift Card", **in Checkout lo stesso
check verrà automaticamente visualizzato, all'interno della sezione
pagamenti, nel momento in cui l'utente dovesse avere un saldo Gift Card
spendibile per l'ordine in questione**

![](./assets/media/image253.png)

**ATTENZIONE!** tanto in carrello quanto in checkout l'importo
visualizzato in corrispondenza del check "**Usa il saldo**" **è quello
effettivamente spendibile per l'ordine corrente e non il saldo globale
delle Gift Card caricate sull'account dell'utente (**che è invece
visibile solo all'interno del componente "Gift Card")

Verranno quindi già determinati, in maniera completamente automatica,
gli importi effettivamente spendibili per l'ordine corrente sulla base
di quanto indicato, in fase di configurazione di ogni singola Gift Card,
in relazione ai campi "**Applicazione utilizzo**" e "**Condizioni**".

Nello specifico poi la procedura di calcolo dell'importo effettivamente
utilizzabile per l'ordine in esame prende in considerazione per primi i
codici Gift Card che stanno per scadere e, a parità di scadenza, quelli
con un residuo inferiore.

Se poi si è in modifica di un ordine sospeso vengono considerati
spendibili anche gli importi gestiti sull'ordine stesso.

Infine, nel momento in cui l'applicazione del saldo Gift Card dovesse
coprire interamente l'ordine, azzerando i totali del documento:

- in carrello verrà automaticamente nascosto il modulo che consente
  all'utente di richiedere un preventivo sulle eventuali spese di
  pagamento

- in checkout verranno automaticamente nascoste le diverse opzioni di
  pagamento

In queste condizioni, inoltre, l'ordine verrà inserito all'interno del
gestionale con il campo relativo al pagamento non valorizzato.

**ATTENZIONE!** **per fare in modo che l'applicazione del saldo Gift
Card all'ordine possa funzionare in maniera corretta è indispensabile
selezionare, tra i parametri di configurazione del componente Checkout,
il campo** "**Visualizza Totale**"

Nel caso in cui il parametro indicato non dovesse essere selezionato,
non verranno visualizzati i Totali del documento e l'applicazione del
saldo Gift Card all'ordine potrebbe non avvenire in maniera corretta

