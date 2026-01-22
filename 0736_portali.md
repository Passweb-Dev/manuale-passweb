# PORTALI



All'interno di questa sezione è possibile configurare l'integrazione con
portali generici, esterni a Passweb, che espongono endpoint
interrogabili mediante apposite chiamate API per prelevare dati che
potranno poi essere visualizzati direttamente sul front end del sito.

In questo senso la logica utilizzata è sostanzialmente la stessa di
quella che permette a Passweb di comunicare con le Web Api Mexal (per
maggiori informazioni in merito si vedano anche i precedenti capitoli di
questo manuale).

Una volta completata l'integrazione con un determinato portale, per
effettuare le chiamate agli endpoint da esso esposti sarà dunque
necessario utilizzare gli strumenti di editing avanzato di Passweb
(Layout di pagina o Componente HTML) per effettuare chiamate Ajax in
POST al seguente url

**/effettuaChiamataPortale**

indicando anche determinati parametri necessari per comporre in maniera
corretta la richiesta che verrà poi inoltrata allo specifico portale
direttamente dal server di Passweb

**ATTENZIONE!** **la chiamata effettivamente inoltrata al portale
esterno sarà sempre di tipo server to server** (sarà quindi il server
Passweb a interrogare il relativo endpoint) in maniera tale da evitare
eventuali problemi (CORS, requisiti di sicurezza ...) che potrebbero
sorgere in caso di chiamate di tipo client -- server.

Detto che per poter utilizzare questo tipo di funzionalità sono
necessarie, ovviamente, specifiche conoscenze tecniche (gestione di
chiamate API Rest, Javascript, CSS, HTML ...) è bene sottolineare anche
alcune cose di fondamentale importanza.

Nello specifico:

- La logica e l'interfaccia da utilizzare per lo scambio di dati tra le
  due piattaforme (Passweb -- Portale) dovrà essere sviluppata
  interamente lato client utilizzando gli strumenti messi a disposizione
  da Passweb: Layout di Pagina (sezione Javascript), Componente HTML,
  componente Form ...

- I dati prelevati dal portale esterno (tipicamente in formato JSON)
  dovranno poi essere inseriti nella pagina e graficati secondo le
  specifiche esigenze del caso, utilizzando ancora una volta gli
  strumenti messi a disposizione da Passweb: Layout di Pagina (sezione
  CSS), Componente HTML ...

> In questo senso nel caso in cui l'endpoint esterno dovesse ritornare,
> ad esempio, una serie di codici articolo (relativi a prodotti
> effettivamente gestiti all'interno del sito) sarà poi possibile
> utilizzare anche una specifica funzione javascript messa a
> disposizione da Passweb per visualizzare questi stessi articoli
> all'interno di un componente "Risultati Ricerca" o "Catalogo
> Ecommerce" (per maggiori informazioni in merito si rimanda a quanto
> indicato all'interno del capitolo "*Developer -- Funzione Javascript
> per applicazione Filtro di Ricerca*" di questo manuale).

- I dati prelevati dal servizio esterno non potranno, in nessun caso,
  essere memorizzati nella base dati di Passweb ne potranno in alcun
  modo modificare le logiche di funzionamento del proprio sito Ecommerce

Nei successivi capitoli di questo manuale vedremo più nel dettaglio come
poter configurare l'integrazione tra Passweb e un portale che espone
effettivamente degli endpoint interrogabili mediante apposite chiamate
API ed esamineremo anche un semplice esempio di come implementare, una
volta effettuata l'integrazione, questo tipo di chiamate.

