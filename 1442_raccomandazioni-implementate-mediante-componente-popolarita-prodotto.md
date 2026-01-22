# RACCOMANDAZIONI IMPLEMENTATE MEDIANTE COMPONENTE POPOLARITA' PRODOTTO



Come già evidenziato nei precedenti capitoli di questo manuale, a
differenza del modulo di ricerca, le Raccomandazioni di Clerk potranno
essere implementate e inserite nelle pagine del proprio sito Ecommerce
utilizzando anche un componente nativo di Passweb, nello specifico il
componente "**Popolarità Prodotto**"

Per far questo sarà sufficiente impostare il parametro "**Tipologia**"
presente nella maschera di configurazione del componente sull'opzione
"**Reccomendations Clerk**" come nella figura di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popolarita_prodotto_clerk.bmp](./assets/media/image55.png)

Il successivo campo "**Logica Raccomandazione Clerk**" consente invece
di decidere che tipo di raccomandazione dovrà effettivamente essere
implementata mediante il componente in oggetto.

In questo senso è possibile selezionare una delle seguenti opzioni:

- **Best Sellers** -- Prodotti più popolari -- **Può essere inserito in
  una qualsiasi pagina del sito**

> Visualizza i prodotti più popolari nel tuo negozio, specificamente
> quelli che sono stati inclusi nel maggior numero di ordini per un
> periodo prolungato. La quantità dello stesso prodotto in ogni ordine
> non influisce su questo ranking. Ovviamente verranno presi in
> considerazione solo gli ordini inviati a Clerk

- **Hot Products** -- Prodotti di tendenza -- **Può essere inserito in
  una qualsiasi pagina del sito**

> Evidenzia gli articoli che hanno avuto un recente aumento nelle
> vendite. Non c'è un intervallo di tempo fisso, viene calcolato
> dinamicamente in base ai cambiamenti nelle vendite dei prodotti. Ad
> esempio, se un prodotto solitamente viene venduto tre volte a
> settimana e improvvisamente viene venduto 20 volte in due giorni,
> allora verrà identificato come di tendenza e inserito in questa
> raccomandazione.

- **Newest Products** -- Prodotti aggiunti di recente -- **Può essere
  inserito in una qualsiasi pagina del sito**

> Mostra gli articoli che sono stati aggiunti più di recente al
> catalogo, con i più recenti mostrati per primi. Per valutare ciò viene
> utilizzato il valore del campo "created_at" presente nel feed articoli
> utilizzato per l'integrazione tra le due piattaforme

- **Best Sellers In Category** -- Prodotti più popolari nella categoria
  -- **Deve essere inserito in una Pagina di Categoria**

> Visualizza i prodotti più popolari di una determinata Categoria
> Merceologica. La logica adottata dunque è la stessa dei Best Sellers
> riferita però non all'intero catalogo ma ad una specifica Categoria
> merceologica

- **Hot Products In Category** -- Prodotti di tendenza nella Categoria
  -- **Deve essere inserito in una Pagina di Categoria**

> Evidenzia gli articoli di una determinata categoria merceologica che
> hanno avuto un recente aumento nelle vendite. La logica adottata
> dunque è la stessa di Hot Products riferita però non all'intero
> catalogo ma ad una specifica Categoria merceologica

- **Newest Products In Category** -- Prodotti aggiunti di recente in una
  categoria -- **Deve essere inserito in una Pagina di Categoria**

> Mostra gli articoli che sono stati aggiunti più di recente ad una
> determinata Categoria Merceologica. La logica adottata dunque è la
> stessa di Newest Products riferita però non all'intero catalogo ma ad
> una specifica Categoria merceologica

- **Best Alternative Products** -- Prodotti simili ad un determinato
  articolo -- **Deve essere inserito in una Pagina Prodotto**

> Mostra gli articoli più simili al prodotto visualizzato, ordinati per
> popolarità.
>
> Confronta i prodotti in base agli attributi disponibili (e che sono
> stati inseriti quindi nel feed articoli utilizzato per l'integrazione
> tra le due piattaforme) come name, brand, category, price

- **Best Cross-Sell Products** -- Prodotti più probabili da acquistare
  assieme ad un determinato prodotto -- **Deve essere inserito in una
  Pagina Prodotto**

> Visualizza quelli che sono gli articoli più probabili da acquistare
> insieme al prodotto visualizzato. Considera i prodotti che vengono
> comunemente acquistati insieme e quelli che sono potrebbero
> completarsi a vicenda, come una cintura con dei pantaloni. Questo
> viene fatto analizzando i modelli di acquisto tipici per visualizzare
> raccomandazioni adatte, anche per prodotti che non sono ancora stati
> acquistati insieme.
>
> Ad esempio, se è normale acquistare un paio di scarpe da calcio e
> parastinchi della stessa marca e colore, Clerk darà priorità a queste
> coppie per tutte le marche e colori anche se non sono ancora stati
> venduti insieme.

- **Most Sold With --** Prodotti più venduti assieme ad un determinato
  articolo -- **Deve essere inserito in una Pagina Prodotto o nella
  pagina Carrello**

> Identifica i prodotti che sono stati frequentemente acquistati insieme
> a un dato prodotto o a un dato insieme di prodotti (es. prodotti in
> carrello). Rispetto ai Best Cross-Sell Products, questa logica conta
> solo gli articoli che sono stati venduti con il prodotto/i
> specificato/i, senza prevedere nulla.
>
> Ovviamente vengono presi in considerazione solo gli ordini inviati a
> Clerk

- **Visitor Recommendation** -- Prodotti più probabili in base alla
  navigazione dello specifico utente -- **Può essere inserito in una
  qualsiasi pagina del sito**

> Mostra i prodotti che potrebbero essere acquistati con maggior
> probabilità dall'utente che sta navigando il sito e lo fa in base a
> quelli che sono i dati di navigazione recenti di quello stesso utente.
> Combina raccomandazioni di cross-sell e alternative per trovare le
> migliori corrispondenze per ogni visitatore.
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- Visitor Alternatives -- Prodotti simili ad un determinato prodotto che
  potrebbero essere acquistati dallo specifico utente -- **Deve essere
  inserito in una Pagina Prodotto**

> Visualizza i prodotti simili ad un altro prodotto e che potrebbero
> essere acquistati con maggior probabilità dallo specifico visitatore
> in base alla sua cronologia di navigazione recente
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- **Visitor Click History** -- Prodotti cliccati dall'utente -- **Può
  essere inserito in una qualsiasi pagina del sito**

> Mostra esattamente i prodotti visitati dall'utente
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- **Recommendations Based On Orders** -- Prodotti abbinati in base agli
  ordini precedenti del cliente -- **Può essere inserito in una
  qualsiasi pagina del sito**

> Visualizza i prodotti che un cliente può acquistare con maggior
> probabilità in base ai suoi acquisti passati. Combina cross-sell e
> alternative per trovare le migliori raccomandazioni.
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- **Similar To Order History** -- Prodotti simili in base agli ordini
  del cliente -- **Può essere inserito in una qualsiasi pagina del
  sito**

> Visualizza i prodotti simili che un cliente può acquistare con maggior
> probabilità in base ai suoi acquisti passati. Combina cross-sell e
> alternative per trovare le migliori raccomandazioni.
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- **Customer Order History** -- Prodotti acquistati in precedenza
  dall'utente -- **Può essere inserito in una qualsiasi pagina del
  sito**

> Visualizza esattamente i prodotti acquistati dallo specifico cliente
>
> Per funzionare al meglio potrebbe richiedere che l'utente abbia
> effettuato l'autenticazione al sito

- **What Customers Look At Right Now** -- Prodotti che altri utenti
  stanno attualmente guardando -- **Può essere inserito in una qualsiasi
  pagina del sito**

> Mostra i prodotti cliccati più di recente da qualsiasi visitatore del
> sito

- **Recently Purchased Products** -- Prodotti acquistati di recente da
  altri utenti -- **Può essere inserito in una qualsiasi pagina del
  sito**

> Visualizza gli articoli acquistati più recentemente da qualsiasi
> cliente sul sito web.

**ATTENZIONE!** come indicato il valore impostato in corrispondenza del
campo "Logica Raccomandazione Clerk" sarà indicativo anche della pagina
in cui dovrà poi essere effettivamente inserito il componente Popolarità
Prodotto.

Nello specifico, ad esempio, se il componente dovesse essere configurato
per visualizzare i prodotti della raccomandazione "**Best Alternative
Products**" è abbastanza evidente che dovrà poi essere inserito in una
Pagina Prodotto. Diversamente infatti verrebbe a mancare il contesto
necessario per il corretto funzionamento della raccomandazione stessa.
In altre parole Passweb non potrebbe sapere il codice articolo da
passare a Clerk nella chiamata API per farsi ritornare l'elenco dei
prodotti più venduti assieme ad esso e in conseguenza di ciò all'interno
di quel componente "Popolarità Prodotto" non verrebbe visualizzato alcun
prodotto.

I restanti parametri presenti nella maschera di configurazione del
componente consentiranno di impostarlo secondo quelle che sono le sue
tradizionali logiche di funzionamento (per maggiori informazioni in
merito si rimanda quindi a quanto indicato all'interno del capitolo
"*Componenti Ecommerce -- Componente Popolarità Prodotto --
Configurazione*" di questo manuale)

Una volta salvato il componente, nel momento in cui dovesse essere
visualizzata la pagina in cui è stato inserito, verrà effettuata una
chiamata all'endpoint Clerk collegato alla specifica raccomandazione
indicata in fase di configurazione del componente e verranno quindi
restituiti da Clerk i codici articolo oggetto di questa raccomandazione.
Tali codici verranno poi utilizzati da Passweb per visualizzare i
relativi prodotti all'interno del componente Popolarità secondo quelle
che sono le sue tradizionali modalità di funzionamento.

Ovviamente l'ordine di visualizzazione di questi prodotti varierà in
relazione alla specifica raccomandazione Clerk considerata e sarà Clerk
stesso a stabilirlo ritornando già l'elenco dei codici articolo
nell'esatto ordine in cui devono essere visualizzati.

In queste condizioni non avrebbe alcun senso definire e variare
direttamente dal componente Passweb l'ordinamento degli articoli (anzi
facendolo si perderebbe proprio lo scopo principale della
raccomandazione) ed è questa la ragione per cui una volta impostato il
parametro "Tipologia" sull'opzione "Reccomendations Clerk" scomparirà,
nella maschera di configurazione del componente, la sezione "Gestione
Campi di Ordinamento" (presente invece nel momento in cui il componente
dovesse essere utilizzato "normalmente")

Infine, per quel riguarda i vantaggi che si possono ottenere adottando
questo metodo di implementazione possiamo sottolineare:

- La facilità di implementazione. Utilizzando un componente nativo di
  Passweb non è necessario conoscere altri linguaggi o altri strumenti
  per costruire l'interfaccia grafica del componente o per determinare
  quali informazioni visualizzare e quali no

- La possibilità di visualizzare per ogni articolo oggetto della
  raccomandazione uno qualsiasi dei dati presenti in Passweb e non solo
  quelli inseriti nel feed utilizzato per realizzare l'integrazione tra
  le due piattaforme

- La possibilità di visualizzare sempre e comunque i prezzi corretti per
  ogni articolo indipendentemente dall'utente attualmente loggato e da
  quelle che possono essere eventuali condizioni commerciali a lui
  riservate

Per quel che riguarda invece gli svantaggi questi sono da ricercarsi
soprattutto nel fatto che il componente "Popolarità Prodotto" non può
essere inserito, ad esempio, nel pop up di aggiunta in carrello per cui
nel momento in cui l'esigenza dovesse essere quella di inserire una
raccomandazione collegata al prodotto attualmente inserito in carrello
l'unica possibilità sarà quella di utilizzare la modalità embedding o
injection con tutto ciò che ne consegue.

Inoltre dal punto di vista delle prestazioni in questo caso parte del
lavoro dovrà essere effettuato direttamente sul database di Passweb in
quanto è vero sì che l'elenco dei prodotti da visualizzare all'interno
del componente non dovrà essere determinato da Passweb ma gli verrà
ritornato direttamente da Clerk, è anche vero però che poi dovranno
comunque essere effettuate direttamente sul database del sito tutte le
query necessarie per visualizzare i campi articolo che si è deciso di
inserire all'interno del componente, comprese ovviamente anche quelle
necessarie per il calcolo del prezzo.

**ATTENZIONE!** per maggiori informazioni relativamente al modulo
Reccomendations di Clerk e alle Best Practice da seguire per capire
esattamente quale raccomandazione implementare in quale pagina e in
quale modo si consiglia sempre di fare riferimento alla relativa
documentazione di prodotto (es.
<https://help.clerk.io/it/platform/recommendations/best-practices/> )
e/o di rivolgersi direttamente all'assistenza Clerk

