# PUBBLICAZIONE ARTICOLI CON QUANTITA' MULTIPLE



Per i siti ecommerce collegati a Mexal è possibile, volendo, pubblicare
sulla piattaforma terza anche articoli che, lato gestionale, sono
trattati a confezione e che sono quindi venduti a quantità multiple.

In Mexal questo tipo di gestione si attiva, come noto, utilizzando il
campo "**Confezione**" presente nella maschera "**Altri Dati
anagrafici**" di ogni singolo articolo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\marketplace_articoli_confezione.bmp](./assets/media/image655.png){width="4.175in"
height="2.6555555555555554in"}

Nel momento in cui si dovesse decidere di pubblicare sulla piattaforma
terza anche questa particolare tipologia di articoli andrà sempre
considerato che **su Prestashop verranno poi creati automaticamente due
diversi prodotti**:

- **un prodotto singolo** con codice (Riferimento) / nome prelevati dai
  relativi dati presenti all'interno del gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prestashop_articoli_confezione_1.bmp](./assets/media/image656.png){width="5.538888888888889in"
height="3.50625in"}

> **ATTENZIONE!** A default il prodotto singolo sarà impostato in
> maniera tale da non essere visibile all'interno del catalogo web
>
> Nel caso in cui l'esigenza dovesse essere quella di rendere
> acquistabile sul sito anche il singolo prodotto, oltre alla
> confezione, sarà necessario agire attraverso i relativi parametri di
> configurazione direttamente dal Back end di Prestashop

- **un prodotto bundle** (Pacco di Prodotti) con codice del tipo
  "**codiceGestionale-pck**", nome del tipo "**titoloGestionale --
  Pack**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prestashop_articoli_confezione_2.bmp](./assets/media/image657.png){width="5.538888888888889in"
height="3.50625in"}

> Ovviamente le immagini utilizzate per questo prodotto saranno
> esattamente le stesse impostate, eventualmente, sul gestionale per il
> corrispondente articolo singolo

**ATTENZIONE!** Nel momento in cui il titolo del prodotto bundle creato
automaticamente da Passweb non dovesse soddisfare le specifiche esigenze
del caso sarà possibile modificare questo valore direttamente sulla
piattaforma terza, ricordandosi poi però di disabilitare per Passweb (a
livello di Account) la possibilità di sovrascriver il titolo in uso
sulla piattaforma terza con il corrispondente dato in uso all'interno
del gestionale (per maggiori informazioni in merito si veda anche quanto
indicato nel precedente capitolo "**Prestashop -- Configurazione Account
-- Articoli**" di questo manuale)

Nel momento in cui tale opzione non dovesse essere disabilitata infatti,
ad ogni pubblicazione il titolo del prodotto impostato su Prestashop
verrà sovrascritto con quello generato in automatico da Passweb.

Per quel che riguarda le **quantità** con cui i due prodotti verranno
pubblicati sulla piattaforma terza occorre invece sottolineare che:

- Il numero di pezzi presente all'interno dell'articolo bundle sarà
  determinato, ovviamente, dal numero di pezzi impostati per la
  confezione all'interno del gestionale

- La quantità con cui l' articolo bundle sarà effettivamente disponibile
  su Prestashop, dovrà sempre essere rapportata alla quantità
  dell'articolo singolo prelevata da Passweb e al numero di pezzi
  presenti nella singola confezione.

Supponendo dunque di gestire, lato mexal, un dato articolo a confezione
multipla di 4 unità e di avere per esso (sui magazzini impostati per
l'esportazione su Prestashop) una disponibilità di 238 unità:

- L'articolo singolo verrà pubblicato in quantità pari a 236

- L'articolo bundle verrà pubblicato in quantità pari a 59 (in maniera
  tale che 59 x 4 dia effettivamente il totale delle quantità
  disponibili per il singolo prodotto)

Infine per quel che riguarda i **prezzi** di questi due articoli
occorrerà considerare che:

- Per l'articolo singolo, tanto il prezzo base quanto eventuali prezzi
  speciali per gruppi utente, coincideranno esattamente con il prezzo
  definito lato gestionale per la singola unità di prodotto

- Per l'articolo bundle, tanto il prezzo base quanto eventuali prezzi
  speciali per gruppi utente, saranno invece riferiti sempre alla
  confezione e calcolati quindi come il prezzo della singola unità di
  prodotto per il numero di pezzi presenti all'interno della confezione

Supponendo anche in questo caso dunque di trattare, lato mexal, un
articolo a confezione multipla di 4 con un prezzo unitario di 40€, il
prezzo dell'articolo singolo creato su Prestashop sarà anch'esso di 40€
mentre quello dell'articolo bundle sarà di 40 x 4 = 160€

