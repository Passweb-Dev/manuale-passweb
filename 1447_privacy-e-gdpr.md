# PRIVACY E GDPR



Come indicato nei precedenti capitoli di questo manuale il motore di
Clerk si basa interamente sui dati raccolti dal sito e-commerce, dati
questi che andranno poi ad alimentare i suoi algoritmi di intelligenza
artificiale. Per garantire quindi un funzionamento ottimale dei diversi
moduli attivabili sulla piattaforma è indispensabile alimentare Clerk
con un flusso completo, coerente ed aggiornato di dati relativi:

- ai prodotti in catalogo (descrizioni, categorie, varianti,
  disponibilità, attributi personalizzati ...)

- agli utenti del sito (storico di navigazione e acquisto, nome,
  indirizzo mail, indirizzo, attributi personalizzati ...)

- ai comportamenti che gli utenti hanno all'interno del sito (ricerche,
  click, visualizzazioni di prodotti, aggiunte al carrello, ordini
  effettuati ...)

Ovviamente questi dati, e in sostanza quindi tutto il sistema di
tracciamento di Clerk, dovrà essere implementato in maniera coerente con
quelli che sono i moduli Clerk effettivamente utilizzati all'interno del
sito e conseguentemente con il tipo di risultato che si vuole ottenere
ma, soprattutto, dovrà essere implementato in maniera conforme a quanto
richiesto dal GDPR.

Detto quindi che i punti chiave da gestire sono sostanzialmente sempre
gli stessi, ossia:

- Collocazione dei dati raccolti (i server utilizzati da Clerk sono
  localizzati in Europa, nello specifico in Germania con backup in
  Irlanda)

- Informativa chiara ed esplicita agli utenti del sito relativamente
  all'utilizzo della piattaforma e al tipo di dati che verranno raccolti

- Eventuale richiesta di consenso preventivo prima di effettuare il
  tracciamento

nel caso specifico dei servizi offerti da Clerk occorrerà prendere in
considerazione, principalmente, i seguenti aspetti:

- Gestione del visitor id (script di configurazione di Clerk) con
  eventuale implementazione dell'opzione di Opt Out

- Gestione del parametro collect_email (script di configurazione di
  clerk)

- Invio a Clerk di feed clienti / ordini

