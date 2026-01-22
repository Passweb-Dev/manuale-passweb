# SEO -- PERMALINK



La sezione "**Permalink**", presente all'interno del menu **"Preferenze
--SEO"** consente di definire la struttura dei permalink (e quindi degli
url) delle varie pagine del proprio sito web.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\seo_gestione_permalink.bmp](./assets/media/image29.png){width="5.746527777777778in"
height="3.49375in"}

Nello specifico il campo:

**[FORMATO PERMALINK PAGINA:]{.underline}**

consente di impostare il formato del permalink che dovrà essere
utilizzato per la generazione degli url delle pagine del sito in
relazione, soprattutto, ai siti multilingua.

E' possibile selezionare uno dei seguenti valori:

- **Con sottodirectory lingua:** in queste condizioni l' url delle varie
  pagine del sito conterrà sempre, tra il nome domino e il path della
  pagina, un'ulteriore elemento identificativo della lingua in cui si
  sta effettivamente visitando il sito.

> Supponendo dunque di dover gestire un sito in tre lingue, Italiano,
> Inglese e Francese l' url della pagina Chi Siamo, posizionata in un
> albero delle pagine del tipo di quello qui di seguito riportato
>
> Home
>
> \| \_\_ Azienda
>
> \|\_\_ Chi siamo
>
> potrà essere, nelle tre lingue gestite, il seguente:
>
> Italiano: **www.nomesito.it/it/azienda/chi-siamo**
>
> Francese: **www.nomesito.it/fr/azienda/chi-siamo**
>
> Inglese: **www.nomesito.it/en/azienda/chi-siamo**
>
> **In queste condizioni una stessa pagina web potrebbe quindi avere lo
> stesso nome in lingue differenti in quanto l'univocità dell' url è
> comunque garantita dalla sottodirectory (it/en/fr ...) identificativa
> della lingua considerata**
>
> **ATTENZIONE! Nel caso di siti multilingua, anche e soprattutto in
> ottica SEO, si consiglia utilizzare questo tipo di opzione.**

- **Senza sottodirectory lingua:** selezionando questa opzione l' url
  delle varie pagine del sito sarà formato sempre e soltanto dal nome
  dominio seguito dal path della pagina visitata.

> In queste condizioni, ovviamente, nel caso di siti in multilingua
> l'univocità dell' url di una pagina web può essere garantito solo ed
> esclusivamente dal fatto di assegnare alla stessa pagina nomi diversi
> in lingue diverse.
>
> Supponendo dunque, anche in questo caso, di dover gestire un sito in
> tre lingue, Italiano, Inglese e Francese l' url della pagina Chi
> Siamo, posizionata in un albero delle pagine del tipo di quello qui di
> seguito riportato
>
> Home
>
> \| \_\_ Azienda
>
> \|\_\_ Chi siamo
>
> potrebbe essere, nelle tre lingue gestite, il seguente:
>
> Italiano: **www.nomesito.it/azienda/chi-siamo**
>
> Francese: **www.nomesito.it/societe/a-propos-de-nous**
>
> Inglese: **www.nomesito.it/company/about-us**
>
> dove ovviamente è stato assegnato un nome diverso nelle tre lingue
> gestite sia alla pagina "Azienda" che alla pagina "Chi Siamo"
>
> Nel momento in cui si dovesse decidere di abilitare questa gestione
> per il formato del permalink delle pagine, Passweb attiverà dei
> controlli di univocità del permalink su lingue differenti dello stesso
> elemento, in maniera tale da evitare di poter associare alla stessa
> pagina uno stesso nome in lingue differenti rendendo di fatto non
> raggiungibile una delle due o più pagine che si troverebbero ad avere
> in lingue diverse lo stesso url.
>
> In questo senso dunque, se il sito gestisce più lingue, creando una
> nuova pagina ed assegnandogli un nome solo in Italiano (o comunque
> nella lingua di default), per le pagine in lingua Passweb utilizzerà
> automaticamente lo stesso nome utilizzato per la lingua italiana
> seguito da un suffisso identificativo della lingua considerata.
>
> Supponendo quindi di creare una nuova Pagina "Contatti", assegnandogli
> il nome unicamente in lingua Italiana, per la stessa pagina in lingua
> francese e inglese verranno utilizzati automaticamente i nomi
> "Contatti-fr" e "Contatti-en", nomi questi che, per ovvie ragioni,
> andranno poi personalizzati in maniera corretta.
>
> **ATTENZIONE! Nel caso di siti in una sola lingua (dove non si
> presenta il problema di univocità dell' url di una stessa pagina in
> lingue differenti) è consigliabile utilizzare questa opzione in
> maniera tale da NON aggiungere nell' url delle pagine web un path
> (quello dell'unica lingua gestita) che, anche in ottica SEO, non
> aggiungerebbe nessun valore all' url stesso.**

Sulla base di quanto detto nel momento in cui si dovesse decidere, per
qualche ragione, **di passare dal formato dei permalink "Con
Sottodirectory lingua" a quello "Senza Sottodirectory lingua", Passweb
effettuerà per prima cosa un controllo di univocità** sui permalink
delle varie pagine in lingue differenti in maniera tale da verificare se
sia effettivamente possibile effettuare o meno questo passaggio.

Nel momento in cui dovessero essere trovate delle pagine con lo stesso
permalink in lingue diverse verrà visualizzato un messaggio di errore
("Non è possibile impostare il Formato Permalink Pagina senza la
sottodirectory lingua") e verrà mantenuto il formato dei permalink con
la sottodirectory relativa alla lingua.

Nel caso in cui si decida di passare invece dal formato dei permalink
"Senza la sottodirectory lingua" a quello "Con sottodirectory lingua", è
consigliabile, per prima cosa, verificare che non siano presenti nomi di
pagine in lingua con il suffisso assegnatogli automaticamente da Passweb
in fase di creazione della pagina stessa (es. "Azienda-en").

**Il passaggio al formato "Con sottodirectory" andrà infatti ad
aggiungere all' url delle pagine la sottodirectory relativa alla lingua
ma non modificherà in alcun modo il nome delle pagine e quindi il pezzo
finale del path del url** (che, eventualmente, andrà quindi modificato
in maniera manuale facendo attenzione anche alla corretta gestione dei
relativi alias)

**ATTENZIONE! Per ovvie ragioni è consigliabile non effettuare continui
switch sul formato del permalink delle pagine. Il formato da adottare
andrebbe scelto prima di portare in produzione il sito e, salvo caso
eccezionali, non andrebbe poi modificato**

**In ogni caso nel passaggio da un formato dei permalink all'altro
Passweb si preoccuperà di gestire in maniera completamente automatica i
redirect di tipo 301 dal vecchio al nuovo formato degli url delle pagine
in maniera tale da non creare errori di tipo 404, notificando allo
stesso tempo agli spider dei motori di ricerca il nuovo indirizzo della
pagina web**

[**FORMATO PERMALINK SCHEDA ARTICOLO:**]{.underline}

consente di decidere come dovrà essere gestito e generato **l' url delle
Pagine Prodotto**.

E' possibile selezionare uno dei seguenti valori:

- **Con il percorso di categoria:** in questo caso l' url delle pagine
  prodotto sarà costruito considerando:

  - Il percorso della specifica Pagina Prodotto

  - L'insieme delle categorie e sotto categorie merceologiche di
    appartenenza dello specifico Articolo

  - Il permalink dell'articolo.

> **Es.
> www.miosito.it/catalogo-articoli/prodotti/informatica/accessori/apple/magic-mouse**
>
> dove ovviamente

- **/catalogo-articoli/prodotti** è il percorso della specifica pagina
  Prodotto (che all'interno di Passweb è posta al di sotto della pagina
  "Catalogo")

- **/informatica/accessori/apple** individua l'insieme delle categorie e
  sotto categorie merceologiche di appartenenza dello specifico prodotto

- **/magic-mouse** è il permalink dello specifico articolo

> **ATTENZIONE!** **Per articoli associati a più categorie
> merceologiche, la categoria principale rimarrà sempre quella associata
> all'articolo direttamente all'interno del relativo gestionale
> Passepartout**, mentre tutte le categorie merceologiche associate
> all'articolo all'interno del Wizard di Passweb verranno considerate
> come categorie merceologiche secondarie.
>
> Per maggiori informazioni in merito alla possibilità di associare, in
> Passweb, un articolo a più categorie merceologiche, si veda anche la
> sezione "*Catalogo -- Gestione Articoli -- Articoli -- Anagrafica
> Passweb -- Associazione di un articolo a più categorie merceologiche*"
> di questo manuale.
>
> In conseguenza di ciò nel momento in cui un determinato articolo
> dovesse essere ricercato e trovato all'interno del sito sulla base di
> una delle sue categorie merceologiche secondarie, vistando poi la sua
> scheda si verrà comunque ricondotti alla pagina prodotto generata
> sulla base della sua categoria merceologica principale.
>
> In questo modo si eviterà di creare più pagine prodotto relative allo
> stesso articolo, evitando quindi di incappare in problemi di
> duplicazione dei contenuti.
>
> Allo stesso modo anche il **meta tag rel="canonical"** generato in
> automatico da Passweb sulle pagine prodotto **verrà creato prendendo
> in considerazione sempre e comunque la categoria merceologica
> principale dell'articolo, ossia quella associata all'articolo stesso
> direttamente all'interno del gestionale.**

- **Senza il percorso di categoria:** in questo caso l' url delle pagine
  prodotto sarà costruito considerando (oltre ovviamente al dominio del
  sito) solo ed esclusivamente il permalink delle specifico articolo

> **Es. www.miosito.it/magic-mouse**

**ATTENZIONE!** **Il formato utilizzato per l' url delle Pagine Prodotto
potrebbe avere un impatto abbastanza importante per ottimizzare
l'indicizzazione di queste stesse pagine.**

**In questo senso è consigliabile far generare a Passweb l' url delle
pagine prodotto senza il percorso delle categorie merceologiche evitando
così di incappare in eventuali problemi legati a contenuti duplicati
(soprattutto nel caso in cui si sia deciso di associare uno stesso
articolo a più categorie merceologiche).**

Dal punto di vista SEO infatti Google tende a penalizzare (abbassandone
il ranking) quei siti che presentano contenuti duplicati su più pagine
differenti. Nel momento in cui si dovesse quindi generare l' url delle
pagine prodotto con l'intero percorso delle categorie merceologiche,
agli spider del motore di ricerca potrebbe risultare che l'articolo
"magic-mouse" sia presente non solo all'interno della pagina

- www.miosito.it/catalogo-articoli/prodotti/informatica/accessori/apple/magic-mouse

ma anche all'interno delle pagine:

- www.miosito.it/catalogo-articoli/prodotti/informatica/accessori/apple

- www.miosito.it/catalogo-articoli/prodotti/informatica/accessori

- www.miosito.it/catalogo-articoli/prodotti/informatica

- www.miosito.it/catalogo-articoli

In realtà i rischi di penalizzazione, in queste condizioni, sono minimi
in quanto come indicato da Google stesso "si definisce contenuto
duplicato una porzione significativa di testo che risulta essere
identica, o quasi, ad un'altra che risiede nello stesso sito o in un
sito esterno"

Per causare quindi l'attivazione da parte di Google dei filtri
anti-duplicazione (con relative eventuali penalizzazioni) sarebbe
necessario che la maggior parte del testo presente nella scheda prodotto
sia riportato anche nelle varie Pagine di Categoria in cui risulterebbe
presente lo stesso articolo (ipotesi questa difficilmente praticabile).

In ogni caso per evitare qualsiasi tipo di problema è sempre meglio,
come detto, generare l' url delle pagine prodotto con il solo permalink
dell'articolo.

**ATTENZIONE! Il formato definito mediante il parametro "Formato
Permalink Scheda Articolo", verrà utilizzato dall'applicativo per
gestire i collegamenti automatici alle varie Pagine Prodotto. In ogni
caso le pagine prodotto risponderanno sempre ad entrambe le tipologie di
url.**

Questo modo di operare di Passweb, consente, da una parte, di passare da
un tipo di formato ad un altro senza incorrere in problemi di
indicizzazione legati ad errori 404 (pagina non trovata). Se infatti,
per qualche ragione, le varie pagine prodotto fossero state indicizzate
con il percorso completo delle categorie merceologiche, passando poi al
solo permalink dell'articolo i risultati di ricerche organiche
effettuate sui vari motori di ricerca che riportano ancora il vecchio
formato del url, verranno comunque reindirizzati alla corretta pagina
prodotto (senza generare errori 404 e senza costringere l'amministratore
del sito a crearsi appositi alias per ogni singolo articolo).

D'altra parte occorre anche considerare che il fatto di avere una pagina
che risponde comunque a due url differenti potrebbe portare nuovamente
al problema iniziale dei contenuti duplicati su pagine diverse, in
quanto, in questo modo, lo stesso esatto contenuto risulterebbe essere
presente agli indirizzi
"www.miosito.it/catalogo-articoli/prodotti/informatica/accessori/apple/magic-mouse"
e **"**www.miosito.it/magic-mouse ", che, agli occhi di uno spider,
risultano essere a tutti gli effetti due pagine distinte.

Passweb gestisce comunque anche questo tipo di problema in due modi
distinti; da una parte "canonicalizzando" gli url e, nello specifico,
inserendo automaticamente all'interno della pagina prodotto il meta tag
**rel="canonical"** (come da specifiche Google) in modo tale da indicare
allo spider quale delle due diverse url che rimandano allo stesso
contenuto sia effettivamente quella da dover indicizzare.

In questo senso l' url canonico sarà costituito dal **"dominio primario
del sito più il formato dei permalink"** che si è scelto di utilizzare
per i prodotti gestiti all'interno del sito.

Dall'altra parte verranno anche generati, in maniera completamente
automatica, **dei redirect di tipo 301** in maniera tale da informare
gli spider della variazione effettuata e garantire così la corretta
indicizzazione delle relative pagine prodotto (evitando sia errori di
tipo 404 -- pagina non trovata -- che contenuti duplicati).

**NOTA BENE**: il problema dei contenuti duplicati all'interno di un
sito è comunque un problema molto più ampio, non si limita, ovviamente,
al solo formato dei permalink delle pagine prodotto e, per ottimizzare
l'indicizzazione delle proprie pagine web, deve quindi essere affrontato
e risolto in maniera adeguata dall'amministratore del sito.

**[FORMATO PERMALINK CONTENUTI CMS:]{.underline}**

consente di decidere come dovrà essere generato e gestito l' url delle
Pagine di dettaglio per i vari post CMS pubblicati all'interno del sito.

E' possibile selezionare uno dei seguenti valori:

- **Con il parametro nel Url:** in questo caso l' url delle pagine di
  dettaglio dei vari post CMS sarà del tipo

> *http://www.clobis.it/**dettaglio-notizia?a=the-divergent-series-allegiant***
>
> e conterrà quindi al suo interno il parametro di query string ?a=
> seguito dal titolo del post che si sta visualizzando

- **Senza il parametro nel Url:** selezionando questa opzione verrà
  visualizzato un ulteriore campo "**Usa un separatore**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\permalink_cms_usa_separatore.bmp](./assets/media/image30.png){width="5.792361111111111in"
height="3.5256944444444445in"}

> mediante il quale poter specificare se nella costruzione dell' url
> delle pagine di dettaglio dei vari post CMS, dovrà essere utilizzato o
> meno un apposito separatore
>
> Nel caso in cui si dovesse decidere di **utilizzare tale separatore**
> (parametro impostato sul valore SI) sarà poi necessario indicare, in
> corrispondenza del successivo parametro "**Segmento separatore tra
> Pagina e Titolo del CMS**" la stringa da utilizzare per la costruzione
> del url della pagina di dettaglio dei post CMS.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\permalink_cms_separatore.bmp](./assets/media/image31.png){width="5.792361111111111in"
height="3.5256944444444445in"}

> La stringa indicata verrà quindi inserita, tra il nome della "Pagina
> di Dettaglio" ed il "Titolo" del post visualizzato.
>
> Supponendo dunque di inserire all'interno di questo campo il valore
> "**news**" (opzione di default) e di aver indicato come pagina di
> dettaglio per i post CMS la pagina denominata "Dettaglio Notizia" l'
> url delle pagine di lettura dei vari post potrebbe essere del tipo
>
> *http://www.clobis.it/**dettaglio-notizia/news/the-divergent-series-allegiant***
>
> e sarà quindi privo di qualsiasi parametro di query string.
>
> Nel caso in cui si dovesse invece decidere di **non utilizzare alcun
> separatore** (parametro "Usa un separatore" impostato sul valore No)
> l' url delle pagine di lettura dei vari post CMS risulterebbe ancora
> più accorciato in quanto privo sia di qualsiasi parametro di query
> string sia di eventuali separatori.
>
> *http://www.clobis.it/**dettaglio-notizia/the-divergent-series-allegiant***
>
> In queste condizioni le regole di "Url Rewrite" dell'applicazione
> prenderanno in considerazione le pagine indicate come "**Pagina di
> lettura**" in corrispondenza delle varie categorie CMS

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\categoria_cms_pagina_lettura.bmp](./assets/media/image32.png){width="5.792361111111111in"
height="3.5256944444444445in"}

> Per maggiori informazioni relativamente a come poter associare una
> pagina di lettura ad una data categoria CMS si veda anche la sezione
> "*Sito -- Gestione CMS -- Gestione Categorie*" di questo manuale.
>
> **ATTENZIONE!** **Nel momento in cui si dovesse decidere di costruire
> l' url delle pagine di lettura dei vari post cms senza parametro di
> query string e anche senza separatore, è necessario associare a
> ciascuna delle Categorie CMS gestite all'interno del sito una
> specifica pagina di lettura, pagina questa che dovrà ovviamente
> contenere un componente "Dettaglio News".**
>
> In caso contrario infatti tentando di visualizzare il dettaglio di una
> specifica notizia potrebbe essere ritornato un errore 404 di pagina
> non trovata
>
> Allo stesso modo nel momento in cui si dovesse decidere, in queste
> condizioni, di creare una nuova pagina dettaglio cms, sarà poi
> necessario verificare, per prima cosa, di aver impostato tale pagina
> come pagina di lettura per tutte le categorie cms interessate.
> Successivamente, sarà anche necessario accedere alla sezione "*Sito --
> Preferenze -- SEO*" del Wizard e cliccare sul pulsante "**Rigenera URL
> Rewrite**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\rigenera_url_rewrite.bmp](./assets/media/image33.png){width="5.792361111111111in"
height="3.5256944444444445in"}

> in maniera tale da consentire all'applicazione di rigenerare, secondo
> le nuove impostazioni, le corrette url di lettura dei vari post cms
> pubblicati all'interno del sito.
>
> **ATTENZIONE!** La variazione del parametro "**Formato Permalink
> Contenuti CMS**" comporta il riavvio automatico del sito.

- **Solo con il path:** selezionando questa opzione l' url della pagina
  di dettaglio dei vari post CMS verrà costruito concatenando
  semplicemente il dominio del sito con il titolo dello specifico post e
  risulterà quindi essere del tipo

> *http://www.clobis.it/**the-divergent-series-allegiant***
>
> **ATTENZIONE!** In queste condizioni è di fondamentale importanza
> verificare che **i vari post siano associati a categorie per le quali
> è stata correttamente impostata una specifica pagina di lettura**
> (pagina questa che dovrà ovviamente contenere un componente "Dettaglio
> News")
>
> In caso contrario infatti l'applicazione non sarebbe in grado di
> determinare l' url del post e verrebbe quindi ritornato un errore 404
> (di pagina non presente).
>
> **Allo stesso modo, è di fondamentale importanza verificare anche che
> il path del post che si intende visualizzare non sia già stato
> utilizzato per identificare un'altra pagina del sito**. In questo
> senso infatti Passweb effettua un controllo solo ed esclusivamente sui
> path degli altri post CMS assegnando automaticamente un numero
> progressivo al loro url nel momento in cui dovessero essere presenti
> contenuti con lo stesso path (e quindi con lo stesso titolo).
>
> Nel momento in cui l' url di visualizzazione di un determinato post
> dovesse invece coincidere con quello di un'altra pagina del sito si
> generà un conflitto (determinato dal fatto di avere due pagine diverse
> con lo stesso url) e l'applicazione potrebbe non rispondere in maniera
> corretta.

**ATTENZIONE!** Per ottimizzare in termini SEO l'indicizzazione di
questo tipo di contenuti è consigliabile impostare il parametro in
oggetto sul valore "**Solo con il path**" o, al massimo, **"Senza il
parametro nel Url"** e **senza l'utilizzo di alcun separatore** (oltre a
non annidare troppo, all'interno della struttura del sito, la pagina di
lettura)

**Nel momento in cui si dovesse variare l'impostazione di questo
parametro, Passweb gestirà automaticamente un redirect 301 dei vecchi
url su quelli definiti dal nuovo formato in maniera tale da non generare
errori 404 e informare allo stesso tempo i vari spider relativamente al
coretto url che dovrà essere indicizzato per le pagine in questione.**

Inoltre al cambiamento del parametro sarà anche necessario pulire i
cookie del browser per poter visualizzare correttamente i vari post sul
front end del sito (una volta deciso il tipo di permalink da utilizzare
si consiglia quindi di non variare più il parametro in questione)

