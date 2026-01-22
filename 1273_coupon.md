# COUPON



In questa sezione è possibile visualizzare informazioni dettagliate
relativamente a quelli che sono i Buoni Sconto gestiti e utilizzati
all'interno del proprio sito Ecommerce.

**ATTENZIONE! tutti i dati presenti all'interno di questa sezione si
basano sulle matrici Passweb, ossia sulla copia di ordini effettuati
direttamente all'interno del sito (non nati, quindi, all'interno del
gestionale e solo successivamente esportati sul sito) e questo in
conseguenza del fatto che lato gestionale non possono essere memorizzati
i riferimenti relativi a questo tipo di informazioni**

Per maggiori dettagli relativamente alle matrici Passweb si veda anche
la sezione "*Ordini -- Gestione Ordini*" di questo manuale.

All'interno della maschera Coupons verranno quindi visualizzati tutti i
Buoni Sconto attivi all'interno del sito e che sono stati utilizzati
almeno una volta all'interno di un documento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_bs_0.bmp](./assets/media/image26.png){width="6.0125in"
height="3.5340277777777778in"}

E' possibile filtrare i dati in elenco in base al nome del cliente
intestatario dell\'ordine (campo "**Nome / Ragione Sociale"**), in base
al nome (campo "**Buono**") o al codice sconto (campo "**Coupon**")
assegnati, in fase di configurazione, allo specifico Buono Sconto.

Per ciascuno dei Buoni Sconto presenti in elenco sono visualizzate le
seguenti informazioni:

- **Buono:** nome assegnato al Buono Sconto

- **N. Utilizzi**: numero di volte in cui il Buono Sconto in oggetto è
  stato effettivamente utilizzato

- **Subtotale**: somma dei totali di tutte le righe delle matrici
  Passweb in cui è stato utilizzato il Buono Sconto in oggetto (utile
  per visualizzare, ad esempio, il valore degli sconti generati dal
  Buono Sconto in esame).

- **Totale**: somma dei totali ordine di tutte le matrici Passweb in cui
  è stato utilizzato il Buono Sconto in oggetto

**ATTENZIONE!** Nel caso in cui il sito gestisca più di una singola
valuta, nella maschera sopra evidenziata verranno visualizzate righe
diverse per valute diverse

Cliccando su uno dei Buoni Sconto presenti in elenco è poi possibile
accedere ad ulteriori dettagli relativi all'utilizzo del Buono in
questione.

In questo modo verranno infatti visualizzate le righe di tutte le
matrici Passweb coinvolte nell'utilizzo del Buono Sconto selezionato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_bs_1.bmp](./assets/media/image27.png){width="6.0125in"
height="3.5340277777777778in"}

e per ciascuna di esse verranno visualizzate le seguenti informazioni:

- **Buono**: nome assegnato al Buono Sconto

- **Subtotale**: totale della riga della matrice convolta
  nell'applicazione del Buono Sconto in oggetto

- **Totale**: totale ordine della matrice in cui è presente la riga
  coinvolta nell'applicazione del Buono Sconto in oggetto

- **Utente**: nome dell\'utente intestatario dell\'ordine in cui è
  presente la riga coinvolta nell'applicazione del Buono Sconto in
  oggetto

- **Email**: indirizzo mail dell\'utente intestatario dell\'ordine in
  cui è presente coinvolta nell'applicazione del Buono Sconto in oggetto

- **Data**: data di creazione della matrice (e quindi dell'ordine) in
  cui è presente la riga coinvolta nell'applicazione del Buono Sconto in
  oggetto

Cliccando su ciascuna delle righe presenti all'interno di questa
maschera, sarà possibile accedere anche al dettaglio dell'intera matrice
in cui è stato utilizzato il relativo Buono Sconto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_bs_2.bmp](./assets/media/image28.png){width="6.0125in"
height="3.5340277777777778in"}

Il link presente nella parte alta della maschera di dettaglio, in
corrispondenza della voce "**Documenti Correlati**", consente di passare
dal dettaglio della matrice a quello del relativo ordine e viceversa,
mentre quello presente in corrispondenza degli articoli coinvolti
nell'utilizzo del Buono Sconto consente di visualizzare il nome del
Buono Sconto effettivamente utilizzato all'interno di quel documento.

Volendo, infine, è anche possibile esportare, in formato csv, i dati
relativi alle statistiche di utilizzo dei Buoni Sconto.

Per far questo è sufficiente selezionare uno dei formati di esportazione
presenti nel menu a tendina evidenziato in figura e cliccare poi sul
pulsante "**Esporta**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_bs_4.bmp](./assets/media/image29.png){width="6.0125in"
height="3.5340277777777778in"}

Nello specifico l'opzione:

- **Elenco Coupons**: consente di generare un file csv contenente i
  seguenti dati:

  - nome del Buono Sconto

  - codice sconto applicato nell'utilizzo del Buono

  - numero di righe in cui è presente il Buono Sconto

  - somma dei totali delle righe coinvolte nell'utilizzo del Buono
    Sconto

  - somma dei totali (e relativa valuta) degli ordini in cui è stato
    utilizzato il relativo Buono Sconto.

- **Elenco Righe**: consente di generare un file csv con i seguenti
  dati:

  - nome del Buono Sconto

  - codice sconto applicato nell'utilizzo del Buono

  - codice dell\'articolo coinvolto nell'utilizzo del Buono Sconto

  - quantità dell\'articolo coinvolto nell'utilizzo del Buono Sconto

  - totale di riga

  - valuta

  - codice conto del cliente intestatario del documento in cui è stato
    utilizzato il Buono Sconto

  - nome del cliente intestatario del documento in cui è stato
    utilizzato il Buono Sconto

  - indirizzo email intestatario del documento in cui è stato utilizzato
    il Buono Sconto

- **Elenco Articoli Quantita**: consente di generare un file csv con i
  dati raggruppati per codice articolo in cui sono presenti il nome del
  Buono, il codice sconto utilizzato, il codice dell\'articolo, il
  numero di righe in cui è presente l\'articolo e la somma delle
  quantità articolo.

- **Elenco Articoli e Utenti**: consente di generare un file csv con i
  dati raggruppati per codice articolo e per utente, in cui sono
  presenti il nome del Buono, il codice sconto utilizzato, il codice
  dell\'articolo, il numero di righe in cui è presente l\'articolo, la
  somma delle quantità articolo, il codice conto del cliente, il nome
  del cliente e l\'indirizzo email del cliente.

