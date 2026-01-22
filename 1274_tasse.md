# TASSE



In questa sezione è possibile visualizzare informazioni dettagliate
relativamente agli ordini che contengono articoli soggetti ad una delle
Tasse addizionali codificate e gestite all'interno del sito

**ATTENZIONE! come per le promozioni anche in questo caso tutti i dati
presenti all'interno di questa sezione sono riferiti ad ordini
effettuati direttamente all'interno del sito (non nati, quindi,
all'interno del gestionale e solo successivamente esportati sul sito)**

All'interno della maschera Tasse verranno quindi visualizzate tutte le
Tasse addizionali attive all'interno del sito e che sono state
utilizzate almeno una volta all'interno di un documento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_tasse_0.bmp](./assets/media/image30.png){width="6.0125in"
height="3.5340277777777778in"}

E' possibile filtrare i dati in elenco in base al nome del cliente
intestatario dell\'ordine (campo "**Nome / Ragione Sociale/Email"**)
oppure in base alla nome della Tassa stessa (campo "**Tassa**")

Per ciascuna delle tasse presenti in elenco sono visualizzate le
seguenti informazioni:

- **Tassa:** nome assegnato alla relativa Tassa addizionale

- **N. Utilizzi**: numero di volte in cui la tassa in oggetto è stata
  effettivamente utilizzata

- **Subtotale**: somma dei totali di tutte le righe delle matrici in cui
  è stata utilizzata la tassa in oggetto.

- **Totale**: somma dei totali ordine di tutte le matrici in cui è stata
  utilizzata la tassa in oggetto

**ATTENZIONE!** Nel caso in cui il sito gestisca più di una singola
valuta, nella maschera sopra evidenziata verranno visualizzate righe
diverse per valute diverse

Cliccando su una delle tasse presenti in elenco è poi possibile accedere
ad ulteriori dettagli relativi alla tassa in questione.

In questo modo verranno infatti visualizzate le righe di tutte le
matrici Passweb in cui è stata utilizzata la tassa in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_tasse_1.bmp](./assets/media/image31.png){width="6.0125in"
height="3.5340277777777778in"}

e per ciascuna di esse verranno visualizzate le seguenti informazioni:

- **Tassa**: nome della promozione

- **Subtotale**: totale della riga della matrice in cui è stata
  utilizzata la tassa in oggetto

- **Totale**: totale ordine della matrice in cui è presente la riga
  relativa alla tassa in oggetto

- **Utente**: nome dell\'utente intestatario dell\'ordine in cui è
  presente la riga relativa alla tassa in oggetto

- **Email**: indirizzo mail dell\'utente intestatario dell\'ordine in
  cui è presente la riga relativa alla tassa in oggetto

- **Data**: data di creazione della matrice (e quindi dell'ordine) in
  cui è presente la riga relativa alla tassa in oggetto

Cliccando su ciascuna delle righe presenti all'interno di questa
maschera, sarà possibile accedere anche al dettaglio dell'intera matrice
in cui è stata utilizzata la relativa tassa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_tasse_2.bmp](./assets/media/image32.png){width="6.0125in"
height="3.5340277777777778in"}

Il link presente nella parte alta della maschera di dettaglio, in
corrispondenza della voce "**Documenti Correlati**", consente di passare
dal dettaglio della matrice a quello del relativo ordine e viceversa

Volendo, infine, è anche possibile esportare, in formato csv, i dati
relativi alle statistiche di utilizzo delle Tasse addizionali.

Per far questo è sufficiente selezionare uno dei formati di esportazione
presenti nel menu a tendina evidenziato in figura e cliccare poi sul
pulsante "**Esporta**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\statistiche_tasse_3.bmp](./assets/media/image33.png){width="6.0125in"
height="3.5340277777777778in"}

Nello specifico l'opzione:

- **Elenco Tasse**: consente di generare un file csv contenente i
  seguenti dati:

  - nome della tassa

  - numero di righe in cui è stata applicata la tassa

  - somma dei totali delle righe in cui è stata applicata la tassa

  - somma dei totali (e relativa valuta) degli ordini in cui è stata
    applicata la relativa tassa.

- **Elenco Righe**: consente di generare un file csv con i seguenti
  dati:

  - nome della tassa

  - codice dell\'articolo soggetto alla tassa

  - quantità dell\'articolo soggetto alla tassa

  - totale di riga

  - valuta

  - codice conto del cliente intestatario del documento in cui è stata
    applicata la tassa

  - nome del cliente intestatario del documento in cui è stata applicata
    la tassa

  - indirizzo email intestatario del documento in cui è stata applicata
    la tassa

- **Elenco Articoli Quantità**: consente di generare un file csv con i
  dati raggruppati per codice articolo in cui sono presenti il nome
  della tassa, il codice dell\'articolo, il numero di righe in cui è
  presente l\'articolo e la somma delle quantità articolo.

- **Elenco Articoli e Utenti**: consente di generare un file csv con i
  dati raggruppati per codice articolo e per utente, in cui sono
  presenti il nome della tassa, il codice dell\'articolo, il numero di
  righe in cui è presente l\'articolo, la somma delle quantità articolo,
  il codice conto del cliente, il nome del cliente e l\'indirizzo email
  del cliente.

