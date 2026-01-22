# VISITOR: 'AUTO' -- OPZIONE DI DEFAULT



**ATTENZIONE!** si ricorda che il fatto di impostare lo script di
configurazione di Clerk senza indicare in maniera esplicita un'opzione
per il parametro visitor, equivale di fatto all'impostazione *visitor:
'auto'*

In queste condizioni verrà attivata la modalità cookieless di Clerk. I
visitatori verranno tracciati attraverso ID di sessione anonimi generati
da Clerk stesso (attraverso il suo script di configurazione) utilizzando
uno specifico algoritmo che, di fatto, garantisce che le sessioni di
acquisto rimangano anonime. L'ID di sessione generato da Clerk non
contiene quindi nessun dato personale, non viene memorizzato in alcun
modo sui dispositivi dell'utente e impedisce il tracciamento a lungo
termine (oltre i 30 giorni)

**ATTENZIONE!** Per maggiori informazioni relativamente all'algoritmo
utilizzato per generare gli ID di sessione anonimi si rimanda alla
relativa documentazione di prodotto (
<https://help.clerk.io/it/platform/data/cookieless-solution/#privacy-settings>
)

Il vantaggio di questa configurazione è rappresentato, indubbiamente,
dal fatto che il visitor id può essere considerato come un dato
pseudonimo che non viene salvato né nei cookie né tanto meno in local
storage e, in conseguenza di ciò, lo script di Clerk potrebbe essere
attivato indipendentemente dall'accettazione o meno dei cookie.

In ogni caso, anche in queste condizioni potrebbe comunque essere
necessario:

- dichiarare in Privacy Policy che il sito sta trattando dei dati
  pesudonimi (ID generato da IP + User Agent)

- avere una base legale adeguata (preferibilmente Legittimo Interesse)

- garantire all'utente un'opzione di Opt-Out che, se esercitata,
  disabiliti di fatto l'attivazione di tutti i moduli Clerk
  eventualmente presenti sul proprio sito (per maggiori informazioni in
  merito si veda quanto indicato all'interno del successivo capitolo
  "*Opzione di Opt-Out*" di questo manuale).

Oltre a ciò occorre anche considerare altri due aspetti di fondamentale
importanza legati all'opzione *visitor: 'auto'*.

**Il primo** è che per come vengono generati e gestiti, in queste
condizioni, gli ID di sessione**, qualsiasi visitatore che dovesse
navigare sullo stesso sito, dalla stessa rete, con lo stesso tipo di
dispositivo e utilizzando anche lo stesso browser, si troverà di fatto a
condividere lo stesso ID di sessione già utilizzata da un altro
utente.**

Una possibile conseguenza di quanto appena detto potrebbe essere quindi
che una raccomandazione basta, ad esempio, sulla cronologia di
navigazione tenga conto per un secondo utente di quelli che sono i
prodotti già visitati da un altro utente prima di lui e che con lui
condivide lo stesso ID di sessione.

**Il secondo aspetto** è invece legato all'utilizzo del componente
"Popolarità Prodotto" di Passweb per la visualizzazione di determinate
Raccomandazioni Clerk.

Come spiegato nei precedenti capitoli di questo manuale ("*Passweb Clerk
-- Raccomandazioni*") infatti la visualizzazione delle Raccomandazioni
di Clerk all'interno di un componente "Popolarità Prodotto" richiede
necessariamente di effettuare apposite chiamate server alle API messe a
disposizione da Clerk.

Il problema in questo senso è rappresentato dal fatto che,
dipendentemente dalla tipologia di Raccomandazione considerata, per
poter ritornare i codici articolo oggetto della raccomandazione stessa,
anche le chiamate API potrebbero dover utilizzare necessariamente un
visitor id che, nel caso specifico, non potrà essere quello utilizzato
lato client, ossia tanto per intenderci quello utilizzato ad esempio per
la visualizzazione dei risultati di ricerca o per il tracciamento del
click sui diversi prodotti presenti in tali risultati e questo perché
l'impostazione *visitor: 'auto'* non consente di accedere all'ID di
sessione effettivamente generato da Clerk.

In queste condizioni le chiamate API utilizzeranno quindi un ID di
sessione, sempre anonimo e generato con lo stesso algoritmo da parte di
Clerk ma, per forza di cose, differente da quello utilizzato per
raccogliere i dati di navigazione dell'utente (**si ricorda infatti che
il tracciamento Clerk all'interno del proprio sito Passweb è effettuato
interamente lato client**)

La conseguenza di tutto ciò sarà quindi che i dati presenti all'interno
di Raccomandazioni Clerk incentrate sul visitatore (Visitor Click
History, Visitor Alternatives ...) gestite mediante il componente
"Popolarità Prodotto" di Passweb potrebbero non essere coerenti con
l'effettiva sessione di navigazione dell'utente.

**ATTENZIONE!** utilizzando l'impostazione *visitor: 'auto'* per
implementare le Raccomandazioni Clerk incentrate sul visitatore (Visitor
Click History, Visitor Alternatives ...) potrebbe essere necessario
ricorrere all'injection oppure all'embedding all'interno del sito,
mediante l'utilizzo di un componente HTML, del relativo snippet di
codice fornito direttamente da Clerk con tutto ciò che ne consegue, sia
a livello di costruzione grafica del componente sia, soprattutto, a
livello di visualizzazione dei prezzi

Occorre infatti ricordare anche che nel momento in cui si dovesse
decidere di implementare una Raccomandazione Clerk mediante embedding o
injection il prezzo visualizzato per i prodotti oggetto della
raccomandazione sarà, generalmente, lo stesso prezzo di listino inserito
anche nel Feed Articoli utilizzato per l'integrazione Passweb -- Clerk e
questo, se da una parte potrebbe essere corretto per un sito B2C in cui
il prezzo dei prodotti non cambia a seconda dell'utente loggato,
dall'altra parte potrebbe anche non andar bene nel caso in cui il prezzo
dei prodotti dovesse invece variare a seconda dell'utente.

In queste condizioni potrebbe quindi essere necessario non inserire
nelle Raccomandazioni Clerk implementate mediante embedding o injection
del codice il prezzo dei prodotti, prezzo questo che dovrà essere
visualizzato normalmente all'interno della corrispondente scheda
prodotto

In definitiva, sulla base di quanto detto e al netto dei possibili
"problemi" relativi alle Raccomandazioni incentrate sul visitatore, la
modalità cookieless di Clerk, corrispondente all'impostazione *visitor:
'auto'*, **è indubbiamente una delle più efficaci e anche delle più
semplici da implementare**, soprattutto in considerazione del fatto che,
in queste condizioni, non è necessario sottoporre tutto il sistema
all'accettazione dei Cookie.

**ATTENZIONE! in ogni caso il consiglio è sempre quello di verificare
direttamente con il supporto Clerk o con il proprio DPO che la soluzione
adottata sia effettivamente conforme a quanto richiesto dal GDPR**

