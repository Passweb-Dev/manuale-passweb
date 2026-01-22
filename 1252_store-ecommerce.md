# STORE ECOMMERCE



Come indicato nei precedenti capitoli di questo manuale l'integrazione
Passweb -- Mailchimp offre agli amministratori del sito la possibilità
di inviare a Mailchimp stesso tutta una serie di dati Ecommerce
relativamente a **ordini**, **carrelli abbandonati**, **articoli** e
**clienti** presenti all'interno del proprio sito, dati questi di
fondamentale importanza per chiunque volesse sfruttare le azioni di
marketing automation messe a disposizione dalla piattaforma MailChimp.

**ATTENZIONE!** **In questo senso l'integrazione Passweb -- Mailchimp
prevede l'invio alla piattaforma terza dei dati Ecommerce secondo la
configurazione impostata all'interno della corrispondente sezione del
Wizard.**

**Eventuali azioni di marketing automation andranno quindi attivate e
configurate (anche e soprattutto a livello di template email)
direttamente all'interno di MailChimp.**

Per poter attivare e configurare l'invio dei dati Ecommerce a MailChimp
è necessario agire all'interno della sezione "**Sito -- Gestione
Newsletter -- Stores**" del Wizard sezione questa da cui sarà possibile
attivare e configurare il proprio **Store Mailchimp.**

**Uno Store in MailChimp è una risorsa di primo livello all'interno
della quale verranno raccolti tutti i dati Ecommerce (carrelli
abbandonati, prodotti, clienti e ordini) inviati dal sito collegato allo
Store in questione.**

Ogni Store, in MailChimp deve essere associato ad una specifica Lista,
inoltre una volta creato lo Store ed effettuata l'associazione con la
Lista desiderata, **tale associazione non potrà più essere modificata**.
Nel caso in cui si dovesse agire in questo senso sarà quindi necessario
disconnettere ed eliminare lo Store per poi crearne uno nuovo associato
alla nuova Lista.

Peri i siti multilingua, e soprattutto nel caso in cui il sito in
multilingua gestisca liste di iscrizione diverse per singola lingua,
Passweb offre anche la possibilità di creare uno specifico Store per
ciascuna delle lingue gestite in maniera tale che ciascuno di essi possa
essere effettivamente collegato alla lista corretta.

Supponendo dunque di gestire il nostro sito in Italiano, Inglese e
Francese, e di voler gestire per ciascuna lingua una diverse Lista
MailChimp, sarà anche possibile creare tre distinti Store uno collegato
alla lista Italiana, uno alla lista Inglese ed uno alla lista Francese.

In queste condizioni i dati Ecommerce verranno poi trasmessi allo Store
Italiano, a quello Inglese o a quello francese secondo la seguente
logica:

- Nel caso in cui l'utente cui fanno riferimento i dati Ecommerce si
  trovi già in una lista, tra quelle associate ai vari Store, allora i
  dati relativi ad ordini, carrelli abbandonati ecc... verranno inviati
  allo Store MailChimp collegato alla lista in cui si trova il cliente e
  questo indipendentemente dal fatto che, ad esempio, il nuovo ordine
  e/o il nuovo carrello abbandonato siano stati generati a partire dal
  sito in Italiano da quello in Francese o da quello in Inglese

- Nel caso in cui l'utente cui fanno riferimento i dati Ecommerce non si
  trovi in nessuna delle Liste associate agli Store MailChimp gestiti,
  allora l'iscrizione dell'utente ad uno specifico Store avverrà
  contestualmente all'inserimento del primo ordine, e il tutto dipenderà
  dalla lingua attiva sul sito al momento dell'ordine. Supponendo dunque
  che l'utente in questione effettui il nuovo ordine dal sito in Inglese
  l'utente stesso ed i relativi dati Ecommerce verranno inseriti nello
  Store MailChimp collegato alla lingua Inglese. Nel caso in cui non
  dovesse esistere uno Store MailChimp collegato alla lingua caricata
  sul sito nel momento in cui è stato effettuato il primo ordine,
  l'utente ed i relativi dati Ecommerce verranno inseriti nello store di
  Default (marcato attraverso l'apposito parametro)

