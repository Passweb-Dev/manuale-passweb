# RACCOMANDAZIONI



Il modulo **Recommendations** di Clerk rappresenta un'ottima soluzione
per aumentare il valore medio dell'ordine, la conversione e il
coinvolgimento dell'utente. Grazie al suo sistema di intelligenza
artificiale e ad una raccolta continua dei dati di navigazione e
acquisto, questo modulo è in grado di offrire suggerimenti di prodotto
altamente pertinenti, dinamici e personalizzati in tempo reale.

Le raccomandazioni di Clerk si adattano perfettamente a ogni fase del
funnel di acquisto e possono essere integrate in homepage, nelle pagine
di categoria, nelle schede prodotto, in pagina carrello, all'interno di
email marketing ...

Il modulo supporta infatti più di 20 diverse tipologie di
raccomandazioni tra cui ad esempio:

- Best Sellers

- Hot Products

- Best Sellers In Category

- Hot Product In Category

- Best Alternative Products

- Best Cross-Sell Products

- Most Sold With

- Recommendations Based On Keywords

- Visitor Recommendations

- Visitor Alternatives

- Recommendations Based On Orders

- ...

Per maggiori informazioni relativamente alle diverse tipologie di
raccomandazioni offerte da Clerk e alle relative logiche che determinano
quali prodotti dovranno essere visualizzati al loro interno si rimanda
alla specifica documentazione di prodotto (es.
<https://help.clerk.io/it/platform/recommendations/logics/> )

Per quel che riguarda invece i dati visualizzabili in corrispondenza di
ogni singolo prodotto presente all'interno di queste raccomandazioni
tutto dipende, essenzialmente, da come queste verranno poi implementate
all'interno del sito Passweb.

**A differenza di quanto visto per il modulo di ricerca, infatti, le
Raccomandazioni di Clerk possono essere implementate all'interno del
proprio sito anche utilizzando un componente nativo di Passweb, nello
specifico il componente "Popolarità Prodotto"**

In sostanza dunque, dal punto di vista implementativo, potremo decidere
di operare in due modi diversi.

Nello specifico potremo decidere di:

- configurare tutto (interfaccia grafica, contenuti, logiche da
  applicare per la visualizzazione dei prodotti ...) direttamente
  all'interno di Clerk esattamente allo stesso modo di quanto visto per
  il modulo di ricerca e lasciare poi che sia Clerk stesso ad iniettare
  le raccomandazioni nelle pagine del nostro sito oppure embeddare i
  relativi snippet di codice con un componente HTML

- utilizzare il componente "Popolarità Prodotto" di Passweb per
  effettuare chiamate API ad uno degli endpoint messi a disposizione da
  Clerk e visualizzare quindi i prodotti restituiti all'interno di
  questo stesso componente Passweb

Detto che, comunque, questi due modi di lavorare non sono alternativi e
possono tranquillamente essere utilizzati assieme, nei successivi
capitoli verranno analizzati più nel dettaglio mettendone in evidenza
anche vantaggi e svantaggi

Per maggiori informazioni relativamente alla configurazione e alle
possibilità offerte dal modulo Reccomendations di Clerk, si consiglia di
fare riferimento alla relativa documentazione di prodotto e/o di
chiedere direttamente all'assistenza Clerk

