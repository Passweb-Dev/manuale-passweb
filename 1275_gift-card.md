# GIFT CARD



In questa sezione è possibile visualizzare informazioni dettagliate
relativamente a quelli che sono i codici delle Gift Card gestite e
utilizzate all'interno del proprio sito Ecommerce.

**ATTENZIONE! tutti i dati presenti all'interno di questa sezione si
basano sulle matrici Passweb, ossia sulla copia di ordini effettuati
direttamente all'interno del sito (non nati, quindi, all'interno del
gestionale e solo successivamente esportati) e questo in conseguenza del
fatto che lato gestionale non possono essere memorizzati i riferimenti
relativi a questo tipo di informazioni**

Per maggiori dettagli relativamente alle matrici Passweb si veda anche
la sezione "*Ordini -- Gestione Ordini*" di questo manuale.

All'interno della maschera **Gift Cards** verranno quindi visualizzati
tutti i codici Gift Card che sono stati utilizzati almeno una volta
all'interno di un documento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_gc_0.bmp](./assets/media/image34.png){width="6.0125in"
height="3.5340277777777778in"}

E' possibile filtrare i dati in elenco in base al nome del cliente
intestatario dell\'ordine (campo "**Nome / Ragione Sociale"**), in base
alla tipologia di Gift Card utilizzata (campo "**Gift Card**") o allo
specifico codice Gift Card (campo "**Codice**").

Per ciascuno dei codici presenti in elenco sono visualizzate le seguenti
informazioni:

- **Gift Card**: tipologia di Gift Card cui è stato assegnato il codice
  in esame

- **Codice**: codice assegnato alla Gift Card

- **N. Utilizzi**: numero di volte in cui il codice in oggetto è stato
  effettivamente utilizzato

- **Subtotale**: somma dei totali di tutte le righe delle matrici
  Passweb in cui è stato utilizzato il codice Gift Card in oggetto
  (utile per visualizzare, ad esempio, il valore degli sconti generati
  dal codice in esame).

- **Totale**: somma dei totali ordine di tutte le matrici Passweb in cui
  è stato utilizzato il codice Gift Card in oggetto

**ATTENZIONE!** Nel caso in cui il sito gestisca più di una singola
valuta, nella maschera sopra evidenziata verranno visualizzate righe
diverse per valute diverse

Cliccando su uno dei codici presenti in elenco è poi possibile accedere
ad ulteriori dettagli relativi all'utilizzo di questo stesso codice.

In questo modo verranno infatti visualizzate le righe di tutte le
matrici Passweb coinvolte nell'utilizzo del codice Gift Card selezionato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_gc_1.bmp](./assets/media/image35.png){width="6.0125in"
height="3.5340277777777778in"}

e per ciascuna di esse verranno visualizzate le seguenti informazioni:

- **Gift Card**: tipologia di Gift Card cui è stato assegnato il codice
  in esame

- **Codice**: codice assegnato alla Gift Card

- **Subtotale**: totale della riga della matrice convolta
  nell'applicazione del codice in oggetto

- **Totale**: totale ordine della matrice in cui è presente la riga
  coinvolta nell'applicazione del codice in oggetto

- **Nome / Ragione Sociale**: nome / ragione sociale dell\'utente
  intestatario dell\'ordine in cui è presente la riga coinvolta
  nell'applicazione del codice in oggetto

- **Email**: indirizzo mail dell\'utente intestatario dell\'ordine in
  cui è presente la riga coinvolta nell'applicazione del codice in
  oggetto

- **Data**: data di creazione della matrice (e quindi dell'ordine) in
  cui è presente la riga coinvolta nell'applicazione del codice in
  oggetto

Cliccando su ciascuna delle righe presenti all'interno di questa
maschera, sarà possibile accedere anche al dettaglio dell'intera matrice
in cui è stato utilizzato il relativo codice Gift Card.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_gc_2.bmp](./assets/media/image36.png){width="6.0125in"
height="3.5340277777777778in"}

Il link presente nella parte alta della maschera di dettaglio, in
corrispondenza della voce "**Documenti Correlati**", consente di passare
dal dettaglio della matrice a quello del relativo ordine e viceversa.

Volendo, infine, è anche possibile esportare, in formato csv, i dati
relativi alle statistiche di utilizzo dei codici Gift Card.

Per far questo è sufficiente selezionare uno dei formati di esportazione
presenti nel menu a tendina attivabile cliccando sul campo evidenziato
in figura e cliccare poi sul pulsante "**Esporta**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_gc_3.bmp](./assets/media/image37.png){width="6.0125in"
height="3.5340277777777778in"}

Nello specifico l'opzione:

- **Elenco Gift Cards**: consente di generare un file csv contenente i
  seguenti dati:

  - nome della Gift Card

  - codice della Gift Card

  - numero di volte in cui il codice è stato utilizzato

  - somma dei totali delle righe coinvolte nell'utilizzo del codice Gift
    Card

  - somma dei totali (e relativa valuta) degli ordini in cui è stato
    utilizzato il relativo codice Gift Card.

- **Elenco Righe**: consente di generare un file csv con i seguenti
  dati:

  - nome della Gift Card

  - codice della Gift Card

  - codice dell\'articolo spesa coinvolto nell'utilizzo della Gift Card

  - quantità dell\'articolo spesa coinvolto nell'utilizzo della Gift
    Card

  - totale di riga

  - valuta

  - codice conto del cliente intestatario del documento in cui è stato
    utilizzato il codice Gift Card

  - nome del cliente intestatario del documento in cui è stato
    utilizzato il codice Gift Card

  - indirizzo email intestatario del documento in cui è stato utilizzato
    il codice Gift Card

  - data di emissione del documento

- **Elenco Articoli Quantità**: consente di generare un file csv con i
  dati raggruppati per codice articolo in cui sono presenti il nome
  della Gift Card, il codice utilizzato, il codice dell\'articolo spesa,
  il numero di righe in cui è presente l\'articolo e la somma delle
  quantità articolo.

- **Elenco Articoli e Utenti**: consente di generare un file csv con i
  dati raggruppati per codice articolo e per utente, in cui sono
  presenti il nome della Gift Card, il codice utilizzato, il codice
  dell\'articolo spesa, il numero di righe in cui è presente
  l\'articolo, la somma delle quantità articolo, il codice conto del
  cliente, il nome del cliente e l\'indirizzo email del cliente.

