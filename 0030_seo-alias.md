# SEO -- ALIAS



La sezione "**Alias**", presente all'interno del menu **"Preferenze
--SEO"** consente di abilitare / disabilitare la generazione automatica,
da parte dell'applicativo, degli Alias (redirect di tipo 301) relativi
sia alle pagine generiche che alle pagine prodotto e necessari per
evitare eventuali errori di tipo 404 (pagina non trovata) che potrebbero
pregiudicare un corretto posizionamento del proprio sito web.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\seo_alias.bmp](./assets/media/image45.png){width="5.792361111111111in"
height="3.5256944444444445in"}

Per maggiori informazioni relativamente agli Alias di Pagina e/o agli
Alias Articolo si veda anche la sezione "*Sito -- Gestione Alias*" di
questo manuale.

**Generazione Automatica:** selezionando questo parametro l'applicativo
verrà abilitato per la creazione e la gestione automatica sia degli
Alias di Pagina che degli Alias Articolo.

**ATTENZIONE! Nella generazione automatica degli Alias verranno
considerate solo ed esclusivamente le pagine della Variante attualmente
online.**

**Si consiglia quindi di non attivare la generazione automatica quando
il sito è ancora in fase di sviluppo ma solo nel momento in cui il sito
verrà messo in produzione e potrà quindi iniziare ad essere
correttamente indicizzato.**

**In caso contrario (generazione automatica degli Alias con sito in
sviluppo e quindi ancora soggetto a frequenti cambiamenti nei nomi di
pagina) si correrebbe il rischio di generare tutta una serie di Alias
inutili che potrebbero pregiudicare le prestazioni del sito
rallentandone la navigazione.**

Una volta selezionato il parametro "Generazione Automatica", Passweb si
prenderà carico di generare automaticamente dei nuovi Alias al
verificarsi delle seguenti condizioni:

1.  **Viene modificato il nome di una pagina esistente**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_nome_pagina.bmp](./assets/media/image46.png){width="4.032638888888889in"
height="2.584722222222222in"}

> Al salvataggio del nuovo nome, Passweb creerà automaticamente il
> relativo Alias di Pagina in maniera tale che eventuali url già
> indicizzati con il vecchio nome non producano un errore 404 ma
> riportino correttamente l'utente sulla stessa pagina del sito.
>
> Nel caso di siti in multilingua l'Alias verrà creato, ovviamente, per
> la lingua corrispondente a quella per cui è stato modificato il nome
> della pagina in esame.
>
> In queste condizioni va inoltre sottolineato che:

- Nel caso in cui la pagina alla quale viene modificato il nome abbia
  anche delle pagine figlie, verranno generati automaticamente anche
  tutti gli Alias ad esse relativi. Ciò significa dunque che, se si
  dovesse modificare, ad esempio, il nome della Pagina Negozio verranno
  creati automaticamente anche gli Alias di Pagina per tutte le
  Categorie merceologiche attualmente gestite all'interno del sito (in
  queste condizioni, e dipendentemente dal numero di pagine figlie
  presenti, il salvataggio potrebbe richiedere qualche secondo in più).

- Nel caso in cui la pagina alla quale viene modificato il nome dovesse
  essere la pagina "Prodotto" generica e si sia scelto di utilizzare,
  relativamente agli url delle pagine prodotto, il permalink con il
  percorso di categoria, verranno generati automaticamente anche tutti
  gli **Alias Articolo** relativi ai prodotti gestiti all'interno del
  sito e non associati a nessuna categoria merceologica (oltre
  ovviamente agli Alias di Pagina relativi alle pagine figlie della
  pagina Prodotto)

2.  **Viene modificato all'interno della sezione "Gestione Articoli" del
    Wizard il nome di una categoria merceologica**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_nome_categoria.bmp](./assets/media/image47.png){width="5.99375in"
height="3.6430555555555557in"}

> Indipendentemente dal fatto che la variazione al nome della Categoria
> Merceologica, già gestita all'interno del sito, avvenga mediante
> l'apposito form oppure mediante l'import di un file csv, al
> salvataggio del nuovo nome per la categoria in oggetto, verrà creato
> automaticamente anche il relativo **Alias di Pagina**.
>
> In queste condizioni va inoltre sottolineato che:

- Nel caso in cui la Categoria Merceologica in esame dovesse avere delle
  sotto categorie, verranno creati automaticamente anche tutti gli Alias
  di Pagina ad esse relativi.

- Nel caso in cui si sia scelto di utilizzare, relativamente agli url
  delle pagine prodotto, il permalink con il percorso di categoria,
  verranno creati automaticamente anche tutti gli **Alias Articolo**
  relativi ai prodotti associati all'interno del gestionale alle
  Categorie Merceologiche oggetto della variazione.

3.  **Viene modificata all'interno del gestionale la descrizione di una
    Categoria Merceologica**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_nome_categoria_mexal.bmp](./assets/media/image48.png){width="4.428472222222222in"
height="2.8118055555555554in"}

> Nel caso in cui sia stato selezionato il parametro "**Tabella
> Categorie Merceologiche**" in relazione al campo "**Aggiornamento**
> **descrizioni in italiano dal Gestionale"** della maschera
> "**Parametri Sincronizzazione"** del Wizard, in fase di
> sincronizzazione verranno creati automaticamente tutti gli Alias di
> Pagina relativi alle Categorie Merceologiche per cui è stata
> effettivamente variata la descrizione.
>
> In queste condizioni va inoltre sottolineato che:

- Nel caso in cui le Categorie Merceologiche in esame dovessero avere
  delle sotto categorie, verranno creati, automaticamente, in fase di
  sincronizzazione, anche tutti gli Alias di Pagina ad esse relativi.

- Nel caso in cui si sia scelto di utilizzare, relativamente agli url
  delle pagine prodotto, il permalink con il percorso di categoria,
  verranno creati automaticamente, in fase di sincronizzazione, anche
  tutti gli **Alias Articolo** relativi ai prodotti associati
  all'interno del gestionale alle Categorie Merceologiche oggetto della
  variazione.

4.  **Si è scelto di generare il permalink delle pagine prodotto
    utilizzando come tipo di dato l'opzione "Descrizione Gestionale" e
    viene modificata all'interno del gestionale la descrizione di uno
    degli articoli gestiti all'interno del sito.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_descrizione_articolo_mexal.bmp](./assets/media/image35.png){width="4.695138888888889in"
height="2.454861111111111in"}

> In queste condizioni, in fase di sincronizzazione, una volta rilevata
> la nuova descrizione verrà automaticamente creato il relativo Alias
> Articolo.

5.  **Si è scelto di generare il permalink delle pagine prodotto
    utilizzando come tipo di dato l'opzione "Attributo Gestionale" e
    viene modificato, sul gestionale, il valore dell'attributo
    selezionato.**

> In queste condizioni, in fase di sincronizzazione, una volta rilevato
> il nuovo valore per l'attributo in esame verrà automaticamente creato
> il relativo Alias Articolo
>
> Per maggiori informazioni relativamente alla gestione degli attributi
> articolo si veda anche il relativo capitolo di questo manuale.

6.  **Viene modificato il valore del campo "Titolo" presente all'interno
    dell'Anagrafica Passweb di un determinato prodotto**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\permalink_passweb.bmp](./assets/media/image41.png){width="5.99375in"
height="3.6430555555555557in"}

> **ATTENZIONE! Il campo "Titolo" presente nell'Anagrafica Passweb di un
> determinato articolo può essere modificato solo ed esclusivamente nel
> caso in cui si stia operando su di un sito Ecommerce collegato ad uno
> dei gestionali Ho.Re.Ca. oppure nel caso in cui si sita operando su di
> un sito Ecommerce collegato a Mexal e contemporaneamente si sia scelto
> di gestire il permalink delle pagine prodotto utilizzando come tipo di
> dato l'opzione "Passweb"**
>
> In queste condizioni, indipendentemente dal fatto che la variazione
> sia avvenuta operando manualmente all'interno della relativa
> Anagrafica Passweb oppure a seguito dell'importazione di un file csv,
> al salvataggio del nuovo valore verrà creato automaticamente il
> relativo Alias Articolo.

7.  **Viene modificato il tipo di dato utilizzato per gestire il
    permalink delle pagine prodotto**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\permalink_prodotti_passweb.bmp](./assets/media/image42.png){width="5.746527777777778in"
height="3.49375in"}

> **ATTENZIONE! La variazione del parametro in oggetto di per se non
> apporta nessuna cambiamento al "Titolo" degli Articoli gestiti
> all'interno del sito e/o al loro permalink. Affinchè il cambiamento
> abbia effetto sarà necessario lanciare anche una sincronizzazione
> completa.**
>
> In queste condizioni in fase di sincronizzazione (completa) verranno
> automaticamente creati tutti gli Alias Articolo determinati dal
> cambiamento del valore per il parametro in oggetto.
>
> Per maggiori informazioni relativamente alla personalizzazione del
> permalink delle pagine prodotto si veda anche il precedente capitolo
> ("*SEO -- Titolo Permalink*") di questo manuale

Gli Alias generati automaticamente dal sistema saranno visibili e
gestibili dalla relativa sezione del Wizard ("***Sito -- Gestione
Alias***") e si differenzieranno da quelli creati manualmente
dall'utente in base al contenuto della colonna "**Automatico**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_e_manuali.bmp](./assets/media/image49.png){width="5.99375in"
height="3.6430555555555557in"}

In ogni caso gli Alias generati in automatico dal sistema potranno
essere gestiti liberamente e potranno quindi essere eliminati e/o
modificati anche in maniera manuale.

Ovviamente nel momento in cui dovesse essere apportata, in maniera
manuale, una variazione ad un Alias creato automaticamente dal sistema,
al salvataggio della modifica l'Alias stesso non sarà più colorato in
blu e non avrà più l'opzione "A" (automatico) come identificativo
all'interno della griglia.

Per maggiori informazioni relativamente a questa sezione del Wizard si
veda anche il relativo capitolo ("*Sito -- Gestione Alias*") di questo
manuale

**ATTENZIONE! Nella generazione automatica degli Alias di Pagina e/o
degli Alias Articolo vengono sempre effettuati i seguenti controlli:**

- Nel caso in cui sia presente, tra quelli già gestiti, un Alias
  relativo al nuovo slug di pagina o di articolo questo verrà eliminato

- Nel caso in cui non sia presente, tra quelli già gestiti, un Alias di
  pagina o di articolo corrispondente al vecchio slug di pagina, questo
  verrà correttamente creato

Per comprendere meglio il funzionamento di questi controlli si consideri
anche il seguente esempio:

[ESEMPIO]{.underline}

Supponiamo di avere a che fare con un albero di pagine di questo tipo\_

Home

\| \_\_ Azienda

\|\_\_ Contatti

In queste condizioni, la pagina contatti è raggiungibile, inizialmente,
con lo slug "**azienda/contatti**"

Supponiamo ora di aver abilitato la generazione automatica degli Alias e
di rinominare la pagina "Contatti" in "Contattaci"

Una volta effettuata la modifica la stessa pagina sarà quindi
raggiungibile con il nuovo slug "**azienda/contattaci**"

In queste condizioni in fase di generazione automatica dell'Alias di
Pagina verrà verificato, per prima cosa, se è già presente, tra quelli
attualmente gestiti, un Alias di Pagina di tipo redirect con url
"azienda/contattaci" (corrispondente quindi al nuovo slug) e, in caso
affermativo, tale Alias verrà eliminato (in caso contrario infatti la
pagina Contattaci non sarebbe ovviamente raggiungibile con il nuovo slug
essendo questo gestito da uno specifico Alias)

Successivamente verrà verificato se esiste già, tra quelli attualmente
gestiti, un Alias di Pagina di tipo redirect con url "azienda/contatti"
(corrispondente quindi al vecchio slug). In caso affermativo non verrà
creato alcun Alias essendo quello necessario per gestire il cambio di
nome apportato alla pagina in questione già presente; in caso negativo
invece l'Alias di Pagina verrà correttamente creato.

