# INVIO A CLERK DI FEED CLIENTI / ORDINI



Considerando che tutto il funzionamento di Clerk è basato sulla
condivisione dei dati del proprio sito ecommerce, è abbastanza semplice
comprendere che un punto fondamentale di tutto il processo di
integrazione sarà effettivamente quello di inviare a Clerk, in fase di
attivazione del servizio, non solo gli articoli venduti sul sito ma
anche quello che è lo storico dei clienti e degli ordini attualmente
presenti (oltre poi al fatto di effettuare l'invio di questi dati in
maniera continuativa anche dopo l'attivazione del servizio)

Come indicato all'interno del capitolo "*Passweb e Clerk --*
*Integrazione -- Sincronizzazione Dati*" di questo manuale, tutto ciò
può essere fatto mediante la creazione di appositi feed json che Clerk
andrà poi a prelevare per inserire i dati in essi contenuti all'interno
del suo sistema.

Ovviamente all'interno di questi file potranno essere presenti
informazioni "sensibili" come nome, cognome, indirizzo mail, prodotti
acquistati ecc... per cui l'invio di questi dati dovrà essere, sicuro,
ed effettuato in maniera conforme a quanto richiesto dal GDPR.

Dal punto di vista della sicurezza è bene sottolineare nuovamente che
Passweb gestisce la Token Authentication di Clerk (
<https://help.clerk.io/it/integrations/any-webshop/data-feeds/> ) per
cui i feed creati potranno effettivamente essere consumati solo a
seguito di connessioni crittografate (il sito dovrà quindi essere dotato
di certificato SSL) e solo se la richiesta arriva effettivamente da
Clerk. In altre parole richiamando l'url di un feed inserendolo
semplicemente nella barra degli indirizzi del browser verrà ritornato un
errore 401 e i dati del feed non verranno quindi mai visualizzati.

Inoltre per quel che riguarda il GDPR è bene ricordare che:

- Ogni dato personale condiviso richiede una legittima alimentazione

- **Dati recenti di clienti (es. ultimi due anni) già coperti da
  contratto** (quindi già iscritti al sito e che hanno o meno già
  effettuato degli ordini) **possono essere inviati a Clerk senza
  ulteriori richieste se la finalità è quella di personalizzare le
  raccomandazioni di prodotto**

> Ovviamene se cambia la finalità, nello specifico se questi dati
> verranno poi utilizzati anche a scopi marketing, potranno essere
> inviati solo se l'utente ha fornito esplicito consenso

- Gli ordini storici o i clienti senza chiaro consenso di "condivisione
  a terzi" dovrebbero essere esclusi dai feed utilizzati per inviare i
  dati a Clerk. In alternativa prima di inviarli dovrebbe essere
  raccolto il relativo consenso, oppure i "Termini e Condizioni del
  sito" accettati in fase di check-out dovrebbero essere integrati per
  esplicitare questa condivisione.

Per maggior informazioni relativamente a come poter creare e gestire i
feed Clienti e Ordini, oltre a quelli relativi ad Articoli, Categorie
Merceologiche e Pagine del sito si veda anche quanto indicato nel
precedente capitolo "*Passweb e Clerk --* *Integrazione*" di questo
manuale
