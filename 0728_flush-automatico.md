# FLUSH AUTOMATICO



Impostando il parametro Flush sul valore "**Automatico**" il reset della
cache verrà gestito in maniera completamente automatica da Passweb che
si preoccuperà di svuotare la cache del sito nelle seguenti situazioni:

- **[In fase di sincronizzazione dati dal gestionale verso il
  sito]{.underline}.**

> Nello specifico, pochi istanti prima della sincronizzazione, Passweb
> andrà a disattivare l'utilizzo della cache e lo manterrà disattivo per
> tutta la durata della sincronizzazione. Occorre infatti considerare
> che le variazioni apportate alla base dati del sito da questa
> operazione potrebbero anche essere consistenti e, allo stesso modo, la
> sincronizzazione potrebbe durare parecchio tempo per cui si correrebbe
> il rischio di visualizzare sul sito, per tutto il periodo della
> sincronizzazione, dei dati non aggiornati.
>
> **Al termine della sincronizzazione Passweb si preoccuperà poi di
> svuotare la cache (eliminando quindi i vecchi dati)** **e di
> riattivarla** in maniera tale che possa poi essere ricostruita con
> dati correttamente aggiornati

- **[A seguito di nuovi ordini effettuati all'interno del
  sito.]{.underline}**

> Nello specifico se a seguito di un nuovo ordine effettuato all'interno
> del sito le disponibilità degli articoli coinvolti dovessero subire
> **una variazione significativa, passando cioè da "Disponibile" a "Non
> Disponibile" o viceversa**, Passweb provvederà ad effettuare
> automaticamente il flush della Cache.
>
> **ATTENZIONE!** Nelle condizioni indicate il flush automatico della
> Cache avverrà indipendentemente dalle impostazioni settate per il
> parametro "**Gestione Acquisto**" presente all'interno della maschera
> "**Configurazione Catalogo**" del Wizard
>
> Nel caso in cui la variazione delle disponibilità degli articoli
> coinvolti non dovesse invece essere "significativa" non verrà
> effettuato alcun flush.
>
> Questo da una parte farà sì che un eventuale valore della
> disponibilità stampato all'interno della pagina prodotto e aggiornato
> all'ultima sincro non sia effettivamente quello corretto ma dall'altra
> parte, evitando il reset, darà alla cache il tempo di costruirsi
> rendendo quindi i suoi effetti, in termini di prestazioni, più
> evidenti.
>
> Resterebbe, è vero, il problema del valore della disponibilità
> stampato all'interno della pagina che non è esattamente quello più
> aggiornato, ma questo problema potrebbe essere facilmente aggirato
> utilizzando anziché il numero esatto il classico semaforo (verde /
> rosso) oppure inserendo il testo che indica la data di ultimo
> aggiornamento del valore mostrato e il pulsante per richiedere il
> valore corretto in tempo reale.

- **[A seguito di una "Importazione Risorse Articolo /
  Categoria"]{.underline}**

> Ogni qual volta dovesse essere effettuata un' importazione di risorse
> articolo o di immagini di categoria, al termine dell'operazione
> Passweb provvederà ad effettuare automaticamente il flush della Cache

- **[A seguito di una importazione csv di dati articolo e/o di dati di
  categorie merceologiche]{.underline}**

> Ogni qual volta dovesse essere effettuata un' importazione massiva
> (via csv) di dati articolo o di dati di categorie merceologiche, al
> termine dell'operazione Passweb provvederà ad effettuare
> automaticamente il flush della Cache

- **[A seguito di variazione dati sul Wizard del sito]{.underline}**

> Ogni qualvolta dovesse essere effettuata una variazione all'interno
> del Wizard ad un dato cachabile Passweb provvederà a resettare
> automaticamente la cache.
>
> Questo significa quindi che se dovesse essere effettuata una
> variazione ad un parametro di configurazione che dovesse in qualche
> modo variare il codice HTML di una pagina del sito (pensiamo ad
> esempio ad una diversa impostazione di visualizzazione per il
> configuratore di prodotto, ad una diversa impostazione del controllo
> di visualizzazione delle taglie ...), al salvataggio, verrà
> automaticamente resettata la cache
>
> Allo stesso modo nel momento in cui dovesse essere effettuata una
> variazione alla configurazione o ai contenuti di un componente
> cachabile, anche in questo caso al salvataggio Passweb provvederà
> automaticamente ad effettuare il reset della cache, cosa questa che
> avverrà anche nel momento in cui dovesse essere variata la posizione
> di un determinato componente all'interno della pagina web (anche tale
> operazione comporterebbe infatti una variazione del codice HTML della
> pagina coinvolta)

**ATTENZIONE!** Anche in questo caso ovviamente nulla vieta, se
necessario, di poter effettuare uno o più reset manuali mediante i
relativi pulsanti

