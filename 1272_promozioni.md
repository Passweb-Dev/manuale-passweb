# PROMOZIONI



In questa sezione è possibile visualizzare informazioni dettagliate
relativamente a quelle che sono le Promozioni gestite e utilizzate
all'interno del proprio sito Ecommerce.

**ATTENZIONE! tutti i dati presenti all'interno di questa sezione si
basano sulle matrici Passweb, ossia sulla copia di ordini effettuati
direttamente all'interno del sito (non nati, quindi, all'interno del
gestionale e solo successivamente esportati sul sito) e questo in
conseguenza del fatto che lato gestionale non possono essere memorizzati
i riferimenti relativi a questo tipo di informazioni**

Per maggiori dettagli relativamente alle matrici Passweb si veda anche
la sezione "*Ordini -- Gestione Ordini*" di questo manuale.

All'interno della maschera Promozioni verranno quindi visualizzate tutte
le Promozioni attive all'interno del sito e che sono state utilizzate
almeno una volta all'interno di un documento.

![](./assets/media/image21.png)

E' possibile filtrare i dati in elenco in base al Nome / Ragione Sociale
/ Email del cliente intestatario dell\'ordine (campo "**Nome / Ragione
Sociale / Email"**) oppure in base alla nome della promozione stessa
(campo "**Promozione**")

Per ciascuna delle promozioni presenti in elenco sono visualizzate le
seguenti informazioni:

- **Promozione:** nome della promozione

- **N. Utilizzi**: numero di volte in cui la promozione in oggetto è
  stata effettivamente utilizzata

- **Subtotale**: somma dei totali di tutte le righe delle matrici in cui
  è stata utilizzata la promozione in oggetto (utile per visualizzare,
  ad esempio, il valore degli sconti generati dalla specifica
  promozione).

- **Totale**: somma dei totali ordine di tutte le matrici in cui è stata
  utilizzata la relativa promozione

**ATTENZIONE!** Nel caso in cui il sito gestisca più di una singola
valuta, nella maschera sopra evidenziata verranno visualizzate righe
diverse per valute diverse

Cliccando su una delle promozioni presenti in elenco è poi possibile
accedere ad ulteriori dettagli relativi alla promozione in questione.

In questo modo verranno infatti visualizzate le righe di tutte le
matrici Passweb coinvolte nella Promozione selezionata

![](./assets/media/image22.png)

e per ciascuna di esse verranno visualizzate le seguenti informazioni:

- **Promozione**: nome della promozione

- **Subtotale**: totale della riga della matrice convolta nella
  promozione in oggetto

- **Totale**: totale ordine della matrice in cui è presente la riga
  relativa alla promozione in oggetto

- **Utente**: nome dell\'utente intestatario dell\'ordine in cui è
  presente la riga relativa alla promozione in oggetto

- **Email**: indirizzo mail dell\'utente intestatario dell\'ordine in
  cui è presente la riga relativa alla promozione in oggetto

- **Data**: data di creazione della matrice (e quindi dell'ordine) in
  cui è presente la riga relativa alla promozione in oggetto

Cliccando su ciascuna delle righe presenti all'interno di questa
maschera, sarà possibile accedere anche al dettaglio dell'intera matrice
in cui è stata utilizzata la relativa promozione.

![](./assets/media/image23.png)

Il link presente nella parte alta della maschera di dettaglio, in
corrispondenza della voce "**Documenti Correlati**", consente di passare
dal dettaglio della matrice a quello del relativo ordine e viceversa,
mentre quello presente in corrispondenza degli articoli coinvolti nella
promozione consente di visualizzare il nome della promozione utilizzata.

![](./assets/media/image24.png)

Volendo, infine, è anche possibile esportare, in formato csv, i dati
relativi alle statistiche di utilizzo delle Promozioni.

Per far questo è sufficiente selezionare uno dei formati di esportazione
presenti nel menu a tendina evidenziato in figura e cliccare poi sul
pulsante "**Esporta**"

![](./assets/media/image25.png)

Nello specifico l'opzione:

- **Elenco Promozioni**: consente di generare un file csv contenente i
  seguenti dati:

  - nome della promozione

  - numero di righe in cui è presente la promozione

  - somma dei totali delle righe coinvolte nella promozione

  - somma dei totali (e relativa valuta) degli ordini in cui è stata
    utilizzata la relativa promozione.

- **Elenco Righe**: consente di generare un file csv con i seguenti
  dati:

  - nome della promozione

  - codice dell\'articolo coinvolto nella promozione

  - quantità dell\'articolo coinvolto nella promozione

  - totale di riga

  - valuta

  - codice conto del cliente intestatario del documento in cui è stata
    utilizzata la promozione

  - nome del cliente intestatario del documento in cui è stata
    utilizzata la promozione

  - indirizzo email intestatario del documento in cui è stata utilizzata
    la promozione

- **Elenco Articoli Quantita**: consente di generare un file csv con i
  dati raggruppati per codice articolo in cui sono presenti il nome
  della promozione, il codice dell\'articolo, il numero di righe in cui
  è presente l\'articolo e la somma delle quantità articolo.

- **Elenco Articoli e Utenti**: consente di generare un file csv con i
  dati raggruppati per codice articolo e per utente, in cui sono
  presenti il nome della promozione, il codice dell\'articolo, il numero
  di righe in cui è presente l\'articolo, la somma delle quantità
  articolo, il codice conto del cliente, il nome del cliente e
  l\'indirizzo email del cliente.

- **Elenco Articoli**: consente di generare un file csv contenente
  l'elenco degli articoli presenti negli ordini in cui è stata applicata
  una determinata promozione

> **ATTENZIONE!** Per ottenere questa opzione di esportazione è
> necessario, per prima cosa, aver selezionato dal relativo campo
> presente nel form di ricerca (campo "**Promozione**"), la specifica
> promo in relazione alla quale si desidera produrre il file di
> esportazione
>
> Il file csv conterrà le seguenti informazioni:

- **Id Matrice**: identificativo della matrice passweb originata
  dall'ordine in cui è stata applicata la relativa promo

- **Codice**: codice dell'articolo presente nell'ordine in cui è stata
  applicata la relativa promozione

- **Titolo**: titolo dell'articolo presente nell'ordine in cui è stata
  applicata la relativa promozione

- **Nome Promozione**: nome della promozione. Tale valore sarà presente
  solo ed esclusivamente in corrispondenza delle righe articolo che, in
  qualche modo, sono state oggetto della promozione in esame

- **Qta**: quantità dell'articolo presente nell'ordine in cui è stata
  applicata la relativa promozione

- **Subtotale**: totale di riga

> Grazie a questo modello di esportazione sarà possibile, ad esempio,
> sapere esattamente quali articoli sono stati in qualche modo oggetto
> di una determinata promozione.
>
> Per far questo sarà infatti sufficiente selezionare la promozione
> desiderata tra quelle presenti in elenco nel relativo campo di
> ricerca, esportare i dati utilizzando il modello in esame e,
> successivamente, filtrare i dati presenti all'interno del csv facendo
> in modo di visualizzare le sole righe articolo in corrispondenza delle
> quali viene riportato il nome della promozione.
>
> Ovviamente affinché tutto questo possa avere un senso sarà necessario
> utilizzare promo che in qualche modo aggiungano degli sconti agli
> articoli in ordine. Nel momento in cui la promo dovesse infatti
> aggiungere in ordine un determinato articolo spesa, senza intervenire
> direttamente sugli articoli, capire da questa esportazioni, quali
> siano stati effettivamente i prodotti oggetto della promo diventerebbe
> più complicato.

