# MICRODATA



I **microdati (microdata)** sono una tipologia di "dati strutturati" che
utilizza un **formato di marcatura semantica** introdotto con HTML5 e
che prevede di arricchire il contenuto della pagina web con metadati
(dati su dati) strutturati e leggibili da software e agenti automatici.

Tecnicamente, i microdati consistono in un insieme di **specifici**
**attributi HTML** che vengono aggiunti agli elementi della pagina per
fornire un contesto semantico e chiarire quindi ai diversi sistemi
automatici di cosa si sta parlando

Questi attributi sono:

- **itemscope**: identifica il contenitore dei Microdati

- **itemtype**: stabilisce il tipo di entità che si andrà a descrivere
  (es. una persona, una recensione, una ricetta, un prodotto ecc.)

<!-- -->

- **itemprop:** identifica il tipo di proprietà (e quindi di
  informazione) da fornire al motore di ricerca, piuttosto che al
  sistema di AI, al Chatbot o a qualsiasi altro sistema automatico in
  grado di interpretare questi dati strutturati

Con questi attributi si "arricchisce" il normale codice HTML della
pagina, senza modificarne la resa visiva. I motori di ricerca possono
così interpretare il contenuto come un insieme di **oggetti (items)**
con **proprietà (properties)** e **relazioni (relations)**.

Supponiamo, ad esempio, di voler inserire in una determinata pagina
delle informazioni relative ad una data persona.

**Senza l'utilizzo dei Microdati** potremmo ricorrere ad un semplice
markup di questo tipo:

\<div\>

Mi chiamo Mario Rossi, e questo è il mio numero di telefono 022345678.

Lavoro come Blogger per il sito

\<a href="http://www.miosito.com"\> www.miosito.com\</a\>

\</div\>

che però, sulla base di quanto evidenziato anche all'interno del
precedente capitolo di questo manuale, alla fine risulterebbe utile e
funzionale unicamente ad un utente umano.

**Utilizzando i Microdati**, e modificando di conseguenza il markup
HTML, potremo invece fornire in maniera esplicita anche ai motori di
ricerca, ad esempio, delle informazioni più precise e dettagliate
relativamente a questo tipo di contenuto presente all'interno della
pagina web..

\<div **itemscope** **itemtype=\"http://schema.org/Person\"**\>

Mi chiamo \<span **itemprop="name"**\>Mario Rossi\</span\>,

e questo è il mio numero di telefono \<span
**itemprop=\"telephone\"**\>022345678\</span\>.

Lavoro come \<span **itemprop=\"jobTitle\"**\>Blogger\</span\> per il
sito

\<a href=\"http:// www.miosito.com \"
**itemprop=\"url\"**\>www.webmarketingpolicy.com\</a\>.

\</div\>

- L'elemento **itemscope** della prima riga indica che all'interno di
  questo div sono contenuti dei microdati

- Il valore **itemtype="http://schema.org/Person"** presente sempre
  nella prima riga indica che l'elemento che vogliamo descrivere
  mediante Microdati è una persona (in questo caso viene infatti
  utilizzata la struttura di schema.org relativa alle persone).

- I valori preceduti da **itemprop** rappresentano, infine, gli
  attributi dell'elemento persona. **itemprop="name"**, ad esempio,
  informa esplicitamente il motore di ricerca che quanto presente
  all'interno di quel Tag è esattamente il nome della persona. Allo
  stesso modo **itemprop="telephone"** indica al motore di ricerca che
  quello è un numero di telefono ecc...

Il contenuto visivo per l'utente è identico, ma per un motore di ricerca
diventa chiaro:

- che si sta parlando di una persona

- che il nome di quella persona è Mario Rossi

- che il suo numero di telefono è 022345678

- che il suo lavoro è il Blogger

Nel caso in cui dovessimo poi avere la necessità di inserire più
informazioni di entità diverse potremmo ricorrere all'utilizzo delle
entità nidificate. Supponiamo, in questo senso di voler inserire tra le
informazioni di Mario Rossi anche il suo indirizzo di residenza.
L'Indirizzo è, di per sé, un entità indipendente che può essere
collegata all'entità Persona per cui il markup HTML da utilizzare sarà
il seguente:

\<div **itemscope** **itemtype=\"http://schema.org/Person\"**\>

Mi chiamo \<span **itemprop="name"**\>Mario Rossi\</span\>,

e questo è il mio numero di telefono \<span
**itemprop=\"telephone\"**\>022345678\</span\>.

\<div **itemprop=\"address\" itemscope
itemtype=\"http://schema.org/PostalAddress\"**\>

\<span **itemprop=\"streetAddress\"**\>Via Flamina 12\</span\>

\<span **itemprop=\"addressLocality\"**\>Rimini\</span\>

\<span **itemprop=\"postalCode\"**\>47922\</span\>

\</div\>

Lavoro come \<span **itemprop=\"jobTitle\"**\>Blogger\</span\> per il
sito

\<a href=\"http:// www.miosito.com \"
**itemprop=\"url\"**\>www.webmarketingpolicy.com\</a\>.

\</div\>

In questo modo dunque all'interno dell'entità Persona è stata nidificata
l'entità Indirizzo con i seguenti attributi:

- **itemprop="streetAddress":** attributo utilizzato per indicare una
  via all'interno di un indirizzo

- **itemprop="addressLocality":** attributo utilizzato per indicare la
  Città all'interno di un indirizzo

- **itemprop="postalCode":** attributo utilizzato per indicare il Codice
  Postale all'interno di un indirizzo

Ovviamente il tipo di attributi da utilizzare dipenderà dal tipo di
informazione che si vuole comunicare al motore di ricerca, piuttosto che
al sistema di AI che analizza il contenuto della pagina, e quindi dal
tipo di Schema dichiarato all'interno dell'attributo itemtype.

**ATTENZIONE!** il vocabolario semantico utilizzato dai microdati è,
come detto, quello di Schema.org. Tutta la documentazione relativa ai
tipi di Schema che possono essere adottati, alle diverse tipologie di
informazione che possono essere descritte con i microdati e ai relativi
attributi da utilizzare sono quindi disponibili all'indirizzo
<http://schema.org/>

Una volta compreso il modo in cui i microdati tendono a rappresentare e
ad esporre le informazioni ai motori di ricerca, piuttosto che ai
sistemi di AI, alle piattaforme social, a Google Shopping o ad un
qualunque altro sistema automatico, resta ora da capire come poter
effettivamente riportare tutto questo all'interno del proprio sito
Passweb.

In questo senso è possibile procedere in due modi diversi
dipendentemente dal tipo di informazione (quindi dal tipo di Schema) che
si intende adottare e dallo specifico Componente Passweb utilizzato.

Nel caso in cui l'informazione da descrivere mediante Microdati sia
relativa ad una Persona, un Indirizzo, un Video, un Numero di Telefono o
comunque relativa ad un qualche cosa **implementabile in Passweb con
componenti non Ecommerce**, è possibile sfruttare il campo **"Attributi
Addizionali"** presente nella maschera di configurazione di ogni
componente per inserire in maniera corretta, secondo quanto previsto dal
relativo schema, i vari attributi itemscope, itemtype e itemprop.

In alternativa è anche possibile (e forse più rapido) utilizzare
direttamente il **Componente HTML** in maniera tale da inserire
direttamente il Markup desiderato.

**Nel caso in cui invece l'informazione da descrivere mediante Microdati
sia relativa ad elementi più prettamente Ecommerce (Recensioni,
Prodotti, Prezzi, Disponibilità ecc...)** il campo "Attributi
Addizionali" presente nella maschera di configurazione del relativo
Componente (es. Catalogo Ecommerce) da solo non è sufficiente per
modificare correttamente il markup dell'elemento secondo quando
richiesto dal vocabolario di schema.org e, ovviamente, non si ha neppure
la possibilità di intervenire direttamente sul markup HTML di questi
componenti.

In queste condizioni dunque per poter implementare i Microdati anche in
relazione a questi elementi Ecommerce, sarà necessario agire
direttamente dalla sezione "**Dati Strutturati"**" presente all'interno
della pagina "*Sito -- Preferenze -- Integrazioni*" del Wizard
impostando, per prima cosa, il parametro "**Formato dati strutturati**"
sull'opzione "Microdata"

![](./assets/media/image2.png)

**ATTENZIONE!** nel momento in cui si dovesse variare l'impostazione
settata per il parametro "Formato dati strutturati", passando ad esempio
da Microdata a Json-ld o viceversa, per vedere l'effettiva modifica nel
codice sorgente della pagina sarà necessario eliminare prima i cookie
del browser

I check presenti in corrispondenza del parametro "**Proprietà gestite**"
(sezione "**Schema Ecommerce**") consentono poi di abilitare o meno un
determinato Schema di Microdati modificando di conseguenza il Markup
HTML dei componenti Ecommerce che gestiscono quel tipo di informazione.

Nello specifico il check:

- **Schema AggregateRating**: consente di abilitare lo Schema relativo
  al risultato delle valutazioni (stelline) assegnate complessivamente
  ad un dato prodotto modificando di conseguenza il Markup HTML del
  componente "**Rating Review**" in maniera tale da implementare su di
  esso l'utilizzo dei relativi Microdati (Votazione complessiva di un
  prodotto).

- **Schema BreadcrumbList:** consente di abilitare lo Schema relativo
  alle cosiddette "Briciole di Pane" modificando di conseguenza il
  Markup HTML del componente "**Info Navigazione**" in maniera tale da
  implementare su di esso l'utilizzo dei relativi Microdati

> **ATTENZIONE!** Attivando questo Schema i Microdati verranno
> implementati solo ed esclusivamente **sui componenti "Info
> Navigazione" inseriti all'interno delle pagine "Prodotto"**.

- **Schema Product:** consente di abilitare lo Schema relativo ai
  prodotti venduti all'interno di un sito Ecommerce modificando di
  conseguenza il Markup HTML del componente "**Catalogo Ecommerce**" e
  dei singoli componenti presenti all'interno delle **Pagine Prodotto**
  in maniera tale da implementare su di esse l'utilizzo dei relativi
  Microdati.

> Per questo Schema è possibile gestire individualmente le seguenti
> proprietà:

- **Codice Prodotto:** consente di modificare il Markup HTML del
  componente **"Dati Articolo"** nel momento in cui questo dovesse
  essere **mappato con il campo gestionale "Codice"**.

> Attivando questa proprietà, nel markup del componente in esame
> comparirà quindi anche un frammento di codice analogo a quello di
> seguito indicato:
>
> *\< span itemprop=\"productId\" \>*
>
> *\< span itemprop=\"sku\" \>STSM01\< /span \>*
>
> *\< /span \>*
>
> utile per istruire gli spider del motore di ricerca relativamente al
> fatto che il valore "STSM01" è esattamente il codice di quello
> specifico prodotto.

- **Descrizione Prodotto:** consente di modificare il Markup HTML del
  componente **"Descrizione"** in maniera tale da implementare su di
  esso l'utilizzo dei relativi Microdati

> Attivando questa proprietà, nel markup del componente in esame
> comparirà quindi anche un frammento di codice analogo a quello di
> seguito indicato:
>
> *\< span itemprop=\"description\" \>Multifunzione 3 in 1 Laser a
> colori - Massimo formato di stampa: A4 ...\< /span \>*
>
> utile per istruire gli spider del motore di ricerca relativamente al
> fatto che il valore indicato all'interno dello span è esattamente la
> descrizione di quello specifico prodotto.

- **Immagine Prodotto:** consente di modificare il Markup HTML del
  componente **"Immagine Rappresentativa"** in maniera tale da
  implementare su di esso l'utilizzo dei relativi Microdati

> Attivando questa proprietà, nel markup del componente in esame
> all'interno del tag img verrà quindi inserita anche la proprietà
>
> itemprop=\"image\"
>
> utile per istruire gli spider del motore di ricerca relativamente al
> fatto che quella indicata in corrispondenza della proprietà src è
> esattamente l'immagine del prodotto

- **Titolo Prodotto:** consente di modificare il Markup HTML del
  componente **"Titolo"** in maniera tale da implementare su di esso
  l'utilizzo dei relativi Microdati

> Attivando questa proprietà, nel markup del componente in esame
> comparirà quindi anche un frammento di codice analogo a quello di
> seguito indicato:
>
> *\< span itemprop=\"name\" \>Stampante Samsung CLP 365W\< /span \>*
>
> utile per istruire gli spider del motore di ricerca relativamente al
> fatto che il valore "Stampante Samsung CLP 365W" è esattamente il nome
> di quello specifico prodotto.

- **Schema Offer/AggregateOffer:** consente di abilitare lo Schema
  relativo alle informazioni di tipo Prezzo modificando di conseguenza
  il Markup HTML dei componenti **"Prezzo"** presenti all'interno dei
  componenti "**Catalogo Ecommerce**" e/o "**Scheda Prodotto**". Per
  questo Schema è possibile gestire individualmente la seguente
  proprietà

  - **Disponibilità prodotto:** consente di modificare il Markup HTML
    del componente **"Prezzo"** mediante l'inserimento del Tag

> **\< meta itemprop=\"availability\" content=http://schema.org/InStock
> \>** oppure
>
> **\< meta itemprop=\"availability\"
> content=http://schema.org/OutOfStock \>**
>
> dipendentemente dal fatto che il relativo articolo risulti essere o
> meno disponibile e quindi acquistabile all'interno del sito
>
> **ATTENZIONE!** lo schema Offer/AggregateOffer verrà applicato solo ed
> esclusivamente ai Componenti "Prezzo" presenti all'interno del
> "Catalogo Ecommerce" e della "Scheda Prodotto" e solo nel caso in cui
> sia stato attivato anche lo Schema Product. Nel momento in cui dovesse
> essere attivato questo Schema verrà quindi attivato in maniera
> automatica anche lo Schema Product.

- **Schema Rating:** consente di abilitare lo Schema relativo ad un
  singolo commento/recensione modificando di conseguenza il Markup HTML
  del componente "**Rating Articolo**" in maniera tale da implementare
  su di esso l'utilizzo dei relativi Microdati.

- **Schema Review:** consente di abilitare lo Schema relativo ai
  commenti/recensioni associate ai vari prodotti in vendita all'interno
  di un sito Ecommerce modificando di conseguenza il Markup HTML del
  componente "**Commenti Associati**".

> Per questo Schema è possibile gestire individualmente le seguenti
> proprietà:

- **Testo Commento:** consente di modificare il Markup HTML del
  componente "**Testo Commento**" in maniera tale da implementare su di
  esso l'utilizzo dei relativi Microdati

- **Data Commento:** consente di modificare il Markup HTML del
  componente "**Data Commento**" in maniera tale da implementare su di
  esso l'utilizzo dei relativi Microdati

- **Autore Commento:** consente di modificare il Markup HTML del
  componente "**Autore Commento**" in maniera tale da implementare su di
  esso l'utilizzo dei relativi Microdati

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
gestire dei Microdati di prodotto diversi da quelli appena analizzati
(es. la marca del prodotto) sarà necessario agire mediante il componente
**"Dati Articolo"** inserendo, nello specifico, la proprietà desiderata
all'interno del campo **Itemprop Microdata (Schema.org)** (per maggiori
informazioni in merito si veda anche quanto indicato all'interno del
capitolo "*Varianti sito responsive -- Lista Componenti Ecommerce --
Componenti interni ai componenti ecommerce -- Dati Articolo*" di questo
manuale)

