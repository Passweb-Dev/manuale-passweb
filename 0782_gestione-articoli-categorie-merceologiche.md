# GESTIONE ARTICOLI -- CATEGORIE MERCEOLOGICHE



**ATTENZIONE!** le prestazioni dell'applicativo potrebbero essere
condizionate dall'utilizzo di un numero eccessivo di Categorie
Merceologiche. **In questo senso in fase di categorizzazione degli
articoli è consigliato restare sempre al di sotto delle 1200 Categorie
Merceologiche.** Per visualizzare il numero complessivo di Categorie
attualmente in uso all'interno del sito è possibile accedere alla pagina
"Gestione Articoli" del Wizard.

In Passweb è possibile gestire, per ogni singola categoria merceologica,
alcune informazioni addizionali che possono andare da una specifica
descrizione, un'immagine o le etichette in lingua, ad informazioni quali
Keywords, Description, Meta Tag, Title ecc... utili ad una corretta
indicizzazione della corrispondente Pagina Catalogo.

Selezionando infatti una delle categorie merceologiche presenti
all'interno dell'albero posto nella sezione sinistra della pagina, si
attiveranno, nella contestuale barra degli strumenti determinati
pulsanti attraverso i quali poter gestire, in maniera manuale o
automatica, questo tipo di informazioni

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_catalogo3.bmp](./assets/media/image168.png)

Selezionando invece la cartella radice ("**Catalogo Ecommerce**")
comparirà un ulteriore pulsante mediante il quale poter convertire
automaticamente in formato .webp tutte le immagini relative ad articoli
e/o categorie merceologiche pubblicate all'interno del sito

##### CATEGORIA MERCEOLOGICA -- ANAGRAFICA 

Per poter accedere all' Anagrafica Passweb di una determinata Categoria
Merceologica è sufficiente selezionare la Categoria stessa all'interno
dell'albero posto sulla sinistra della maschera "Gestione Articoli" e
cliccare poi sul pulsante "**Modifica**" presente nella contestuale
barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Modifica
Categoria Articolo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_categoria_articolo2.bmp](./assets/media/image169.png)

suddivisa in tre distinte sezioni, "**Informazioni Generali**", "**Seo
-- SiteMap**" e "**Marketplace**"

###### INFORMAZIONI GENERALI

I parametri presenti all'interno della sezione **Informazioni Generali**
consentono di gestire informazioni di carattere descrittivo per la
relativa Categoria Merceologica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_categoria_articolo2.bmp](./assets/media/image169.png)

Nello specifico il campo:

- **Codice:** consente di visualizzare il codice gestionale associato
  alla corrispondente Categoria Merceologica. Il campo è in sola
  visualizzazione; per modificare il valore presente all'interno di
  questo campo è quindi necessario agire direttamente all'interno del
  gestionale

- **Nome:** consente di personalizzare, in tutte le lingue gestite
  all'interno del sito, l'etichetta identificativa del nome della pagina
  e della corrispondente categoria merceologica.

> Il valore di questo campo corrispondente alla lingua Italiana,
> inizialmente, è prelevato direttamente dal campo "**Descrizione**"
> della relativa anagrafica della categoria merceologica del gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\anagrafica_gruppo_merceologico.bmp](./assets/media/image170.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_anagrafica_gruppo_merceologico.bmp](./assets/media/image171.png)

> **NOTA BENE:** a differenza del valore in italiano, il "Nome Pagina"
> in lingua può essere gestito e variato solo ed esclusivamente
> all'interno del Wizard di Passweb
>
> In particolare il fatto di prelevare o meno questo valore direttamente
> dal gestionale alla sincronizzazione dipende dal fatto di aver
> flaggato o meno il parametro **"Tabella Categorie Merceologiche"**
> presente all'interno della sezione **"Aggiornamento descrizioni in
> italiano dal gestionale"** all'interno della pagina **"Parametri di
> sincronizzazione"** del Wizard (per maggiori informazioni in merito si
> veda la corrispondente sezione di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sincronizzazione_categorie_merceologiche.bmp](./assets/media/image172.png)

> **NOTA BENE:** nel caso in cui sia stato selezionato il parametro
> **"Tabella Categorie Merceologiche"** sopra evidenziato, il valore
> prelevato dal gestionale alla sincronizzazione andrà a sovrascrivere
> eventuali valori inseriti per il campo in oggetto direttamente
> all'interno del Wizard di Passweb.

- **Posizione nel menu Categoria:** consente di assegnare alla
  corrispondente Pagina Catalogo uno specifico numero d'ordine. Tale
  numero verrà poi utilizzato per ordinare le voci di eventuali menu di
  categoria articoli per i quali il parametro "Campo di Ordinamento" è
  stato impostato sul valore "Personalizzato"

> **NOTA BENE:** per maggiori informazioni relativamente alle diverse
> possibili modalità di ordinamento dei menu di categoria articoli
> generati in automatico sulla base delle categorie merceologiche di
> Mexal, si veda anche la sezione "Live Editing -- Lista Componenti
> Ecommerce -- Componente Menu Categoria" di questo manuale.

- **Descrizione:** consente di associare alla categoria merceologica
  corrispondente alla Pagina Catalogo attualmente selezionata una
  specifica descrizione. Tale descrizione potrà poi essere visualizzata
  all'interno del componente ecommerce **"Lista Categorie"**

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente ecommerce **"Lista Categorie"** si rimanda alla
> relativa sezione di questo manuale

- **Set di Attributi:** consente di associare agli articoli/servizi
  appartenenti alla categoria merceologica attualmente selezionata, uno
  specifico Set di Attributi, selezionandolo tra quelli codificati
  all'interno della corrispondente sezione del Wizard.

> **L'associazione di un Set di Attributi ad una specifica categoria
> merceologia è un passaggio di fondamentale importanza all'interno del
> processo di categorizzazione degli articoli e indispensabile ai fine
> della creazione, per gli articoli di questa stessa categoria
> merceologica, di una loro anagrafica Passweb**
>
> Tale associazione, volendo, può essere fatta direttamente anche in
> fase di codifica dello specifico set di attributi (per maggiori
> informazioni in merito si veda anche la relativa sezione di questo
> manuale "*Catalogo -- Gestione Attributi Articolo -- Set di
> Attributi*")
>
> **ATTENZIONE! Nel caso di articoli associati a più categorie
> merceologiche verrà considerato il set di attributi relativo alla
> categoria merceologica principale, vale a dire quella associata
> all'articolo stesso direttamente all'interno del relativo gestionale
> Passepartout**
>
> **NOTA BENE:** per maggiori informazioni relativamente alla creazione
> e alla gestione di Attributi Articolo e/o al processo di
> categorizzazione degli articoli si veda anche la sezione "Catalogo --
> Gestione Attributi Articoli" di questo manuale.

- **Set di Opzioni:** consente di indicare, per gli articoli/servizi
  appartenenti alla categoria merceologica attualmente selezionata, uno
  specifico Set di Opzioni di personalizzazione, selezionandolo tra
  quelli codificati all'interno della corrispondente sezione del Wizard.

> **ATTENZIONE!** L'associazione del Set di Opzioni impostata a livello
> di singola categoria merceologica verrà effettivamente applicata solo
> ed esclusivamente alla sincronizzazione in relazione a eventuali nuovi
> articoli appartenenti alla categoria merceologica in esame.
>
> Nel caso in cui l'esigenza dovesse essere quella di associare un Set
> di Opzioni agli articoli già presenti sul sito, sarà necessario agire
> direttamente dall'Anagrafica Passweb dello specifico articolo oppure
> utilizzare il pulsante **"Associa il set agli articoli"** (maschera di
> configurazione del relativo Set).
>
> **ATTENZIONE! Nel caso di articoli associati a più categorie
> merceologiche verrà considerato il set di opzioni relativo alla
> categoria merceologica principale, vale a dire quella associata
> all'articolo stesso direttamente all'interno del relativo gestionale
> Passepartout**
>
> Si ricorda inoltre che l'effettiva associazione di un Set di Opzioni
> avviene a livello di articolo per cui il Set impostato direttamente
> sull'anagrafica del singolo prodotto avrà sempre priorità rispetto a
> quanto indicato a livello di categoria merceologica a meno,
> ovviamente, di non utilizzare il pulsante "Applica il set agli
> articoli" cosa questa che potrebbe resettare eventuali impostazioni
> precedentemente applicate a livello di singolo articolo
>
> Per maggiori informazioni relativamente alle opzioni di
> personalizzazione articolo si veda anche il corrispondente capitolo di
> questo manuale ("*Catalogo -- Opzioni Articoli*")

###### SEO -- SITEMAP

La sezione "**SEO -- SiteMap"** consente invece di gestire,
rispettivamente, i parametri necessari per una corretta indicizzazione
della corrispondente Pagina Catalogo e quelli attraverso cui poter
decidere se la Pagina stessa dovrà o meno comparire all'interno della
SiteMap del sito, ed eventualmente, con che priorità e con che frequenza
di aggiornamento.

**ATTENZIONE! I parametri presenti all'interno di questa sezione possono
essere visualizzati, ma in sola lettura, anche dalle proprietà della
corrispondente Pagina Catalogo**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\seo_categoria.bmp](./assets/media/image173.png)

Nello specifico il campo:

- **Title** (Titolo Pagina)**:** consente di indicare, in ciascuna delle
  lingue gestite all'interno del sito, uno specifico titolo per la
  pagina che si sta realizzando, valore questo che verrà poi utilizzato
  a livello HTML, per generare il \<Title\> di pagina.

> E' possibile indicare esattamente (con una semplice stringa di testo)
> il Title da utilizzare oppure, volendo, è anche possibile costruire
> questo Title utilizzando i segnaposto messi a disposizione da Passweb
> e visualizzati cliccando sull'apposito pulsante presente
> immediatamente al di sotto del campo di input.
>
> **ATTENZIONE!** dipendentemente dall'impostazione settata per il
> parametro "**Gestione Title**" (sezione "*Sito -- Preferenze -- SEO*"
> del Wizard) quanto inserito all'interno di questo campo potrà essere
> utilizzato per valorizzare il segnaposto {pageName} oppure potrà
> essere utilizzato esattamente come Title della specifica pagina
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Sito -- Preferenze -- SEO Nome del Sito e
> Configurazione Tag Title*" di questo manuale

- **Keywords Meta:** consente di specificare, per ciascuna delle lingue
  gestite all'interno del sito le parole chiave (corrispondenti al
  contenuto del Meta tag HTML KEYWORDS) relative alla categoria
  merceologica che si sta considerando e che verranno utilizzate per
  fornire informazioni relative a questa stessa pagina agli utenti o ai
  motori di ricerca.

> E' possibile indicare esattamente le Keywords da utilizzare (mediante
> semplici stringhe di testo separate da ,) oppure, volendo, è possibile
> costruire queste Keyword utilizzando i segnaposto messi a disposizione
> da Passweb e visualizzati cliccando sull'apposito pulsante posto
> immediatamente al di sotto del campo di input.
>
> Per maggiori informazioni relativamente all'utilizzo dei segnaposto si
> veda anche quanto indicato all'interno del capitolo "*Sito --
> Preferenze -- SEO Keywords Description*" di questo manuale

- **Description Meta:** consente di specificare, per ciascuna delle
  lingue gestite all'interno del sito la descrizione (corrispondente al
  contenuto del Meta tag HTML DESCRIPTION) relativa alla categoria
  merceologica che si sta considerando e che verrà utilizzata per
  fornire informazioni relative a questa stessa pagina agli utenti o ai
  motori di ricerca.

> E' possibile indicare esattamente la Description da utilizzare per la
> pagina in esame (mediante semplice stringa di testo) oppure, volendo,
> è possibile costruire queste Description utilizzando i segnaposto
> messi a disposizione da Passweb e visualizzati cliccando sull'apposito
> pulsante posto immediatamente al di sotto del campo di input.
>
> **ATTENZIONE!** dipendentemente dall'impostazione settata per il
> parametro "**Gestione Description**" (sezione "*Sito -- Preferenze --
> SEO*" del Wizard) quanto inserito all'interno di questo campo potrà
> essere utilizzato come Description specifica per la pagina in esame
> oppure potrà andare ad integrare quanto indicato in corrispondenza del
> campo "**Formato Description Pagina Catalogo**"
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Sito -- Preferenze -- SEO Keywords
> Description*" di questo manuale

- **Meta Tags:** consente di inserire nella sezione \<head\> della
  pagina, dei Meta Tags aggiuntivi, non presenti nativamente in Passweb,
  e relativi quindi a specifiche esigenze dell'utente.

> **ATTENZIONE!** A differenza dei precedenti campi "Keywords" e
> "Description" in cui è necessario inserire solamente il contenuto del
> relativo meta tag (ossia le specifiche keywords e/o la specifica
> description) **all'interno di questo campo occorre inserire invece
> l'intero markup relativo al meta tag che si desidera utilizzare**. Per
> maggiori informazioni in merito si veda anche il capitolo "*Pagine
> Generiche*" di questo manuale.
>
> Il pulsante **"Aggiungi segnaposto"** consente di inserire, nella
> definizione del meta tag, dei segnaposto che verranno poi valorizzati
> automaticamente da Passweb.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\anagrafica_categoria2.bmp](./assets/media/image174.png)

> Sono gestiti i seguenti segnaposto:

- **Url sito:** il segnaposto verrà sostituito a runtime con il domino
  del sito (es. www.miosito.it)

- **Url pagina:** il segnaposto verrà sostituito a runtime con l' url
  della relativa pagina web, esclusi eventuali parametri di query string
  (es. www.miosito.it\\catalogo-articoli)

- **Url pagina completo della stringa di Query:** il segnaposto verrà
  sostituito a runtime con l' url competo della relativa pagina web (es.
  www.miosito/cms/blog/dettaglio-post?a=phasellus-fringilla)

- **Titolo Pagina:** il segnaposto verrà sostituito a runtime con lo
  stesso valore utilizzato per il meta tag \< title \>

> Per inserire un nuovo segnaposto è sufficiente posizionare il cursore
> nella posizione in cui questo dovrà essere effettivamente inserito,
> cliccare sul pulsante "Aggiungi segnaposto" e selezionare dal relativo
> menu contestuale la tipologia di segnaposto da inserire.
>
> **NOTA BENE:** oltre che a livello di singola pagina i Meta Tag
> possono essere aggiunti e gestiti anche a livello di Layout Sito. Per
> maggiori informazioni in merito si vedano anche le sezioni "Live
> Editing -- Layout" e "Live Editing -- Pagine -- Pagine Generiche" di
> questo manuale

- **SiteMap:** consente di decidere se la pagina in oggetto dovrà o meno
  essere inclusa nella SiteMap del sito generata dinamicamente
  dall'applicazione.

- **ChangeFrequency:** consente di impostare, per la pagina in oggetto,
  il valore del campo della SiteMap utilizzato per informare il motore
  di ricerca relativamente alla frequenza di aggiornamento dei contenuti
  della pagina stessa.

- **Priority:** consente di impostare, per la pagina in oggetto, il
  valore del campo della SiteMap utilizzato per informare il motore di
  ricerca relativamente alla priorità assegnata ai contenuti della
  pagina stessa.

> **ATTENZIONE!** Nel caso in cui per i tre parametri sopra indicati non
> sia stato specificato alcun valore, verrà considerato il valore
> assegnato, allo stesso parametro, nella sezione "**SiteMap Pagine**"
> del menu "**Sito -- Preferenze**" del Wizard
>
> **Nel caso in cui i parametri in esame non siano stati opportunamente
> valorizzati neppure all'interno del menu "Sito -- Preferenze" del
> Wizard, la pagina in oggetto sarà sempre inserita nella SiteMap con le
> seguenti impostazioni: "ChangeFrequency = Settimanale" e "Priority =
> 0.8"**
>
> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> della SiteMap del sito si veda anche la sezione "Sito -- Preferenze --
> SiteMap Pagine" di questo manuale.

Una volta impostati questi parametri il pulsante **"Salva"** presente
nella parte bassa della maschera confermerà le variazioni eventualmente
apportate.

**ATTENZIONE! eventuali modifiche apportate ai parametri presenti
all'interno della sezione "Seo -- SiteMap" saranno propagate anche alle
corrispondenti pagine di categoria di ogni singola Variante Sito
attualmente gestita. Questi stessi dati verranno inoltre utilizzati
anche in fase di creazione delle nuove pagine in presenza di una nuova
Categoria Merceologica o di una nuova Variante Sito.**

###### MARKETPLACE

All'interno della sezione **Marketplace** è possibile definire la
corrispondenza tra la Categoria Merceologica Mexal / Ho.Re.Ca.
attualmente considerata e la relativa Categoria utilizzata all'interno
di uno dei marketplace integrati con il proprio sito Ecommerce

Per maggiori informazioni relativamente alle possibili integrazioni tra
Passweb ed uno dei marketplace gestiti (Google, Facebook, Magento
Prestashop ecc...) si veda anche la sezione *"Marketplace -- Altri
Marketplace"* di questo manuale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\categoria_merceologica_marketplace.bmp](./assets/media/image175.png)

I campi presenti all'interno di questa sezione consentono quindi di:

- **Google Product Category --** visualizzato solo nel caso in cui sia
  stata correttamente attivata l' integrazione con il Merchant Center di
  Google o il Business Manager di Facebook.

> Consente di indicare la Categoria Merceologica Google che dovrà
> corrispondere alla Categoria Mexal / Ho.Re.Ca. attualmente considerata
>
> Il campo in questione è un campo ad autocompletamento per cui
> iniziando a digitare alcuni caratteri verranno automaticamente
> visualizzate le categorie merceologiche predisposte direttamente da
> Google e coerenti con quanto digitato dall'utente.
>
> Sarà quindi sufficiente selezionare, tra quelle proposte, l'opzione
> desiderata in maniera tale da inserire all'interno del campo il
> percorso completo della categoria merceologica Google da utilizzare
> per mappare l'attuale categoria merceologica Mexal / Ho.Re.Ca.

- **Magento Product Category --** visualizzata solo nel caso in cui sia
  stata correttamente attivata l' integrazione Passweb -- Magento

> Consente di indicare le **Categorie Merceologiche** cui potranno
> essere associati, su Magento, gli articoli appartenenti alla Categoria
> Mexal / Ho.Re.Ca. attualmente considerata (per maggiori informazioni
> in merito si veda anche quanto indicato all'interno della sezione
> "*Marketplace -- Altri Marketplace -- Magento -- Specifiche
> addizionali -- Categories*" di questo manuale)
>
> Il campo in questione è un campo ad autocompletamento che accetta
> valori multipli, per cui iniziando a digitare alcuni caratteri
> (relativamente a quella che dovrà essere la categoria merceologica su
> Magento) verrà visualizzato automaticamente lo schema delle categorie
> merceologiche create e gestite sulla piattaforma terza (e coerenti
> ovviamente con quanto digitato dall'utente)
>
> Sarà quindi sufficiente selezionare, tra quelle proposte, l'opzione
> desiderata in maniera tale da inserire all'interno del campo il
> percorso completo della categoria merceologica Magento da utilizzare
> per mappare l'attuale categoria Mexal / Ho.Re.Ca.
>
> **ATTENZIONE!** **su Magento uno stesso articolo potrà appartenere,
> contemporaneamente, a più categorie merceologiche.**
>
> Una volta individuata e selezionata la prima categoria merceologica
> comparirà quindi un nuovo campo ad autocompletamento mediante il quale
> poter selezionare un ulteriore categoria.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\categoria_merceologica_marketplace2.bmp](./assets/media/image176.png)

> Inoltre considerando che **l'integrazione Passweb -- Magento lavora a
> livello di singola Store View** (e quindi a livello di singola lingua)
> per poter visualizzare le categorie merceologiche in una determinata
> lingua sarà necessario aver configurato un Account di integrazione con
> la Store View Magento utilizzata per gestire la stessa lingua.
>
> Supponiamo, ad esempio, di aver attivato in Passweb la lingua inglese
> avendo però configurato un unico Account di integrazione
> corrispondente alla Store View Magento in Italiano. In queste
> condizioni nel momento in cui tenteremo di inserire dei valori
> all'interno del campo "Magento Product Category" per la lingua inglese
> otterremo il messaggio "Marketplace non gestito"

- **Prestashop Product Category Default --** visualizzata solo nel caso
  in cui sia stata correttamente attivata l' integrazione Passweb
  Prestashop

> Consente di indicare la **Categoria Merceologica principale** cui
> potranno essere associati, su Prestashop, gli articoli appartenenti
> alla Categoria Mexal / Ho.Re.Ca. attualmente considerata (per maggiori
> informazioni in merito si veda anche quanto indicato all'interno della
> sezione "*Marketplace -- Altri Marketplace -- Prestashop -- Specifiche
> obbligatorie -- Category Default*" di questo manuale)
>
> Anche in questo caso il campo in questione è un campo ad
> autocompletamento per cui, iniziando a digitare alcuni caratteri
> (relativamente a quella che dovrà essere la categoria merceologica su
> Prestashop), verrà visualizzato automaticamente lo schema delle
> categorie merceologiche create e gestite sulla piattaforma terza (e
> coerenti ovviamente con quanto digitato dall'utente)
>
> Sarà quindi sufficiente selezionare, tra quelle proposte, l'opzione
> desiderata in maniera tale da inserire all'interno del campo il
> percorso completo della categoria merceologica Prestashop da
> utilizzare per mappare l'attuale categoria Mexal / Ho.Re.Ca.
>
> **ATTENZIONE!** Nel caso di siti multilingua, considerando che la
> traduzione del nome delle categorie avviene direttamente all'interno
> di Prestashop, sarà sufficiente indicare un valore per la sola lingua
> italiana

- **Prestashop Product Category --** visualizzata solo nel caso in cui
  sia stata correttamente attivata l' integrazione Passweb Prestashop

> Consente di indicare le **Categorie Merceologiche secondarie** cui
> potranno essere associati, su Prestashop, gli articoli appartenenti
> Categoria Mexal / Ho.Re.Ca. attualmente considerata (per maggiori
> informazioni in merito si veda anche quanto indicato all'interno della
> sezione "*Marketplace -- Altri Marketplace -- Prestashop -- Specifiche
> addizionali -- Categories*" di questo manuale)
>
> Il campo in questione è un campo ad autocompletamento che accetta
> valori multipli, per cui iniziando a digitare alcuni caratteri
> (relativamente a quella che dovrà essere la categoria merceologica su
> Prestashop) verrà visualizzato automaticamente lo schema delle
> categorie merceologiche create e gestite sulla piattaforma terza (e
> coerenti ovviamente con quanto digitato dall'utente)
>
> Sarà quindi sufficiente selezionare, tra quelle proposte, l'opzione
> desiderata in maniera tale da inserire all'interno del campo il
> percorso completo della categoria merceologica Magento da utilizzare
> per mappare l'attuale categoria Mexal / Ho.Re.Ca.
>
> Una volta individuata e selezionata la prima categoria merceologica
> comparirà un nuovo campo ad autocompletamento mediante il quale poter
> selezionare un' ulteriore categoria.

##### CATEGORIA MERCEOLOGICA -- IMMAGINI 

E' possibile associare ad ogni singola Categoria Merceologica due
distinte immagini, immagini queste che potranno poi essere utilizzate
all'interno del sito mediante i Componenti Ecommerce "**Lista
Categorie**", "**Scheda Categoria**" e "**Menu Categorie**".

Per poter effettuare questa associazione è sufficiente selezionare la
Categoria Merceologica desiderata all'interno dell'albero posto sulla
sinistra della maschera "Gestione Articoli" e cliccare poi sul pulsante
"**Risorse**" in maniera tale da accedere alla maschera di gestione
delle due immagini.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\immagine_categoria.bmp](./assets/media/image177.png)

All'interno di questa maschera, la sezione:

- **Risorsa Lista Categorie:** consente di associare alla categoria
  merceologica attualmente selezionata l'immagine da poter poi
  utilizzare all'interno del sito mediante i Componenti Ecommerce
  "**Lista Categorie**" e/o "**Scheda Categoria**"

- **Risorsa Menu Categoria:** consente di associare alla categoria
  merceologica attualmente selezionata l'immagine da poter poi
  utilizzare all'interno del sito mediante il Componente Ecommerce
  "**Menu Categorie**".

**ATTENZIONE!** sono accettate solo ed esclusivamente immagini di peso
inferiore a 1 MB

Per maggiori informazioni relativamente a come utilizzare queste
immagini all'interno del sito si vedano anche le sezioni *"Varianti Sito
Responsive -- Lista Componenti Ecommerce -- Componenti Interni ai
Componenti Ecommerce -- Componente Immagine (Lista Categorie e Scheda
Categoria)"* e *"Varianti Sito Responsive -- Lista Componenti Ecommerce
-- Componente Menu Categoria - Configurazione"* di questo manuale.

##### CATEGORIA MERCEOLOGICA -- IMPORTAZIONE / ESPORTAZIONE MASSIVA DEI DATI

Oltre a poter gestire i dati delle varie Categorie Merceologiche in
maniera manuale, entrando cioè direttamente nell'Anagrafica di ogni
singola Categoria come descritto nei precedenti capitoli di questo
manuale, Passweb consente anche di effettuare un'importazione massiva,
tramite file, di questi stessi dati in maniera tale da poter assegnare
in blocco a due o più Categorie Merceologiche tutte le informazioni del
caso.

In questo senso dunque il pulsante "**Importa**" nella barra degli
strumenti dell'albero delle Categorie Merceologiche presente all'interno
della maschera "Gestione Articoli", consente di importare tramite file
tutti i dati normalmente presenti, per una data Categoria Merceologica,
all'interno della maschera "Modifica Categoria Articolo -- Informazioni
Generali" precedentemente analizzata.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**File Dati Categorie**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_categorie_importazione_dati1.bmp](./assets/media/image178.png)

all'interno della quale poter configurare l'importazione dei dati in
oggetto. In particolare il campo

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  i dati che dovranno essere importati e associati alle rispettive
  Categorie Merceologiche

- **Lingua:** consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta,
consentendo a Passweb di associare alle rispettive Categorie
Merceologiche i dati presenti all'interno del file di importazione, è
necessario che il file stesso soddisfi determinate regole. Nello
specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

- L'intestazione, ossia la prima riga del file, deve necessariamente
  contenere l'elenco dei nomi dei campi che dovranno poi essere
  valorizzati con i dati presenti all'interno del file tesso. **Il nome
  dei campi non è case sensitive**

> Supponendo di aver scelto come carattere separatore il ;
> l'intestazione del file dovrà avere una struttura del tipo
>
> **NOME CAMPO1;NOME CAMPO2; .....;NOME CAMPON**
>
> Allo stesso modo le righe dei dati dovranno avere una struttura del
> tipo
>
> **VALORE1;VALORE2;....;VALOREN**

- Il primo campo del file dovrà essere obbligatoriamente il **Codice
  della Categoria Merceologica**. La presenza di questo campo è
  ovviamente **indispensabile** in quanto è quella che assicurerà poi
  l'associazione dei dati alle relative Categorie Merceologiche.

> **NOTA BENE:** se all'interno del file da importare non è presente il
> Codice della Categoria e/o se i codici inseriti all'interno di questo
> campo non coincidono con quelli effettivamente presenti all'interno
> del sito la procedura di import non valorizzerà, ovviamente, alcun
> campo dati
>
> Il codice della Categoria Merceologia può essere reperito direttamente
> all'interno del gestionale oppure nell'Anagrafica Passweb della
> Categoria stessa.

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.**

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso da
> virgolette.
>
> Inoltre nel caso in cui il valore di un campo abbia al suo interno
> elementi racchiusi da doppi apici sarà necessario racchiudere tra
> virgolette oltre all'interno campo anche questi stessi elementi.
>
> Supponendo, ad esempio, di aver scelto come carattere separatore il ;
> e di voler importare un file csv con i soli campi CODICE CATEGORIA e
> DESCRIZIONE, potrebbero configurarsi le seguenti casistiche:
>
> 1 -- Il campo DESCRIZIONE non contiene il carattere ; 🡪 il valore di
> questo campo **NON dovrà essere racchiuso da virgolette**
>
> **CAT01;Descrizione CAT01**
>
> 2 -- Il campo DESCRIZIONE contiene il carattere ; 🡪 il valore di
> questo campo **dovrà essere racchiuso da virgolette**
>
> **CAT01;"Descrizione CAT01 contenente un ; che deve essere gestito"**
>
> 3 -- Il campo DESCRIZONE contiene dei doppi apici 🡪 sarà necessario
> racchiudere tra virgolette **sia l'intero campo che l'elemento
> presente al suo interno e racchiuso da doppi apici**
>
> **CAT01;"il campo descrizione contiene ""doppi apici"" che devono
> essere gestiti"**
>
> 4 -- Il campo DESCRIZONE contiene un new line (ritorno a capo) 🡪 il
> valore di questo campo **dovrà essere racchiuso da virgolette**
>
> **CAT01;"il campo descrizione contiene un**
>
> **new line che deve essere gestito"**
>
> **ATTENZIONE!** Eventuali descrizioni delle Categorie Merceologiche
> non devono essere necessariamente allineate tutte su una riga, possono
> essere utilizzati dei new line (ritorno a capo) facendo però
> attenzione a racchiudere il valore di questi campi da doppi apici

Di seguito viene riportato un elenco di tutti i campi gestibili per ogni
singola Categoria Merceologica, e che potranno quindi essere valorizzati
in maniera massiva attraverso questa procedura, oltre ad un esempio di
creazione del file di importazione

- **codice**: codice della categoria -- corrisponde al campo .....
  presente nella maschera "Modifica Categoria Articolo -- Informazioni
  Generali"

- **orderPosition**: posizione nel menù di categoria -- corrisponde al
  campo "**Posizione nel Menu di Categoria**" presente nella maschera
  "Modifica Categoria Articolo -- Informazioni Generali"

- **nome**: nome, nella lingua indicata nel form di importazione, della
  categoria -- corrisponde al campo "**Nome**" presente nella maschera
  "Modifica Categoria Articolo -- Informazioni Generali"

- **descrizione**: descrizione, nella lingua indicata nel form di
  importazione, della categoria -- corrisponde al campo
  "**Descrizione**" presente nella maschera "Modifica Categoria Articolo
  -- Informazioni Generali"

- **title**: valore che dovrà assumere il tag \< title \>, nella lingua
  indicata nel form di importazione, per la relativa pagina di categoria

- **metaKeywords**: keywords meta, nella lingua indicata nel form di
  importazione, delle relative pagine di categoria

- **metaDescription**: description meta, nella lingua indicata nel form
  di importazione, delle relative pagine di categoria

- **metaTag**: tag meta, nella lingua indicata nel form di importazione,
  delle relative pagine di categoria

- **setOpzioni**: nome del Set di Opzioni di personalizzazione da
  associare alla categoria merceologica in esame

**[ESEMPIO -- CARATTERE SEPARATORE ; - LINGUA DI IMPORTAZIONE
ITALIANO]{.underline}**

codice;orderPosition;nome;descrizione;title;metaKeywords;metaDescription;metatag;setOpzioni

cat01;1;Nome-Informatica;Sommario-Prodotti di Informatica;Informatica;Pc
Desktop Accessori;;"\<link rel=""canonical""
href=""<http://www.miosito.com>"" /\>;setInformatica"

cat02;2;Nome-Fotografia;Sommario-Prodotti di Fotografia;Fotografia;;I
migliori prodotti fotografici;

cat03;3;Nome-Intrattenimento;Sommario-Prodotti di
Intrattenimento;Intrattenimento;Serie Tv Film Musica;Il grande
Intrattenimento; "\<link rel=""canonical""
href=""<http://www.miosito.com>"" /\>;setIntrattenimento"

**ATTENZIONE!! La procedura di import sovrascriverà eventuali dati già
presenti all'interno del sito**

**ATTENZIONE! Il valore del campo "descrizione" andrà ovviamente ad
incidere sul permalink delle relative pagine di categoria**

Al termine della procedura di importazione verrà inviata una mail di
notifica all'indirizzo impostato nella sezione "Posta/SMS" del Wizard
contenente i dettagli relativi all'esito della procedura di import.

Tale messaggio potrà inoltre essere consultato anche all'interno della
sezione "Posta/SMS -- Log Mail" del Wizard.

Il pulsante **Esporta**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image136.png) ) consente invece di esportare **in
formato .csv** l'elenco delle Categorie Merceologiche attualmente
gestite all'interno del proprio sito con le relative informazioni
anagrafiche.

Cliccando su questo pulsante verrà visualizzata la maschera
"**Esportazione Dati Categorie**" all'interno della quale poter
configurare l'esportazione dei dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_categorie_esportazione_dati.bmp](./assets/media/image179.png)

Nel caso di sito in multilingua è possibile selezionare, tra quelle
attualmente gestite, la lingua in relazione alla quale dovranno essere
esportati i dati delle Categorie (campo **Lingua**)

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che dovrà essere utilizzato
all'interno del file di esportazione come separatore per i vari campi.

I campi presenti all'interno del file di esportazione saranno
esattamente quelli esaminati in precedenza e gestibili nella
corrispondente procedura di importazione più l'identificativo Passweb
della relativa Categoria

**ATTENZIONE!** in fase di importazione dati il campo chiave rimane
comunque il codice della relativa categoria merceologica

##### CATEGORIA MERCEOLOGICA -- IMPORTAZIONE MASSIVA DELLE IMMAGINI DI CATEGORIA

Oltre a poter importare in maniera massiva mediante file .csv i dati
delle varie Categorie Merceologiche gestite all'interno del sito,
Passweb implementa anche un'analoga procedura di import tramite file
delle Immagini da associare a queste stesse Categorie Merceologiche.

Per poter avviare tale procedura è sufficiente cliccare sul pulsante
"**Imp. Risorse**" nella barra degli strumenti dell'albero delle
Categorie Merceologiche presente all'interno della maschera "Gestione
Articoli",

In questo modo verrà infatti visualizzata la maschera "**File Risorse
Categorie**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\categorie_importazione_immagini1.bmp](./assets/media/image180.png)

all'interno della quale poter indicare **il percorso di un file .zip**
appositamente creato e contenente tutte le Immagini da associare alle
varie Categorie Merceologiche oltre, ovviamente, ad un file .csv
mediante il quale poter indicare quale immagine associare a quale
categoria.

**ATTENZIONE!** sono accettate solo ed esclusivamente immagini di peso
inferiore a 1 MB

Il campo **Separatore** consente di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che è stato utilizzato
all'interno del file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta e
le varie immagini possano essere associate alle relative categorie
merceologiche, dovranno essere rispettate delle regole ben precise.

All'interno del file .zip dovranno essere presenti:

- **tutte le immagini** da associare alle Categorie Merceologiche
  gestite all'interno del sito

- **un file csv** appositamente realizzato e necessario per indicare
  quale immagine associare a quale categoria.

Nello specifico poi per quel che riguarda il file csv:

- l'intestazione, ossia la prima riga del file, dovrà contenere i
  seguenti campi (nell'ordine indicato): **codice, risorsa,
  risorsamenu**

- per ogni record del file dovranno quindi essere inserite le seguenti
  informazioni (nell'ordine indicato):

  - codice: **codice della categoria merceologica**

  - risorsa: **nome del file con relativa estensione** da associare alla
    categoria merceologica e da utilizzare poi all'interno del
    componente "Lista Categorie"

  - risorsamenu: **nome del file con relativa estensione** da associare
    alla categoria merceologica e da utilizzare poi all'interno del
    componente "Menu Categorie"

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione

**[ESEMPIO -- CARATTERE SEPARATORE UTILIZZATO = ;]{.underline}**

codice;risorsa;risorsamenu

Cat01;Immagine-Cat01.jpg;Immgine-Cat01-menu.jpg

Cat02;Immagine-Cat02.jpg;Immgine-Cat02-menu.jpg

Cat03;Immagine-Cat03.jpg;Immgine-Cat03-menu.jpg

**ATTENZIONE! E' necessario effettuare direttamente lo zip delle risorse
grafiche e del file csv e non della cartella contenente tali file. Nel
caso in cui si dovesse infatti effettuare lo zip della cartella
contenente le risorse grafiche e il file csv la procedura di
importazione e associazione delle risorse non potrà terminare in maniera
corretta.**

**NOTA BENE:** per l'upload multiplo di risorse sono gestiti unicamente
file .zip. Non sono ammessi quindi altri formati di compressione (es.
file .rar).

Durante l\'importazione il file .zip verrà decompattato e le singole
risorse verranno associate alle relative categorie merceologiche secondo
quanto indicato nel file csv.

**ATTENZIONE!** Nel caso in cui all'interno del file .zip siano presenti
dei file con lo stesso nome già presenti all'interno del sito, questi
ultimi verranno sovrascritti.

Infine nel caso in cui durante la decompattazione dell'archivio
compresso si dovesse raggiungere il limite dello spazio su disco
(secondo quanto indicato dal contratto), le restanti risorse non
verranno importate.

##### CONVERSIONE IMMAGINI IN FORMATO WEBP

Il pulsante **Converti in .webp** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_converti_webp.bmp](./assets/media/image181.png) ) visibile solo selezionando la cartella radice
"**Catalogo Ecommerce**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\img_articoli_conversione_webp.bmp](./assets/media/image182.png)

consente di avviare manualmente la procedura di conversione in formato
.webp **di tutte le immagini relative ad articoli e categorie
merceologiche** gestite all'interno del sito.

Cliccando su questo pulsante verrà quindi visualizzata la maschera
"**Conversione in .webp**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversione_webp_articoli.bmp](./assets/media/image183.png)

all'interno della quale poter impostare la qualità da utilizzare nel
processo di conversione (ovviamente più alto sarà il grado di qualità
impostata maggiore sarà il peso della relativa immagine .webp) e, una
volta fatto questo, avviare il processo cliccando sul pulsante "**Avvia
conversione**".

La procedura di conversione potrebbe richiedere diversi minuti in base
la numero complessivo di immagini da gestire.

Chiudendo la finestra prima dell'avvenuta conversione di tutte le
immagini, la procedura andrà comunque avanti ma non avremo più modo di
sapere l'esatto momento in cui l'operazione stessa sarà completata.

**ATTENZIONE!** La conversione in webp delle immagini articolo e di
categoria è un prerequisito indispensabile da soddisfare prima di poter
attivare correttamente il parametro "**Attiva Controllo su formato
immagini .webp e .jp2**" presente alla pagina "*Sito -- Preferenze -
SEO*"

In questo senso infatti è bene sottolineare che:

- nel momento in cui si dovesse decidere di attivare il parametro
  "Attiva Controllo su formato immagini .webp e .jp2" presente alla
  pagina "*Sito -- Preferenze - SEO*" del Wizard senza aver prima
  convertito tutte le immagini relative ai prodotti e alle categorie
  merceologiche gestite all'interno del sito in formato webp, queste
  stesse immagini, sul front end, potrebbero anche non essere
  visualizzate in maniera corretta (generando quindi degli errori 404)

- nel momento in cui il parametro "Attiva Controllo su formato immagini
  .webp e .jp2" presente alla pagina "*Sito -- Preferenze - SEO*" del
  Wizard sia già stato attivato in maniera corretta, ogni qualvolta si
  andranno ad aggiungere nuove immagini articolo (mediante
  sincronizzazione o direttamente dal Wizard non fa differenza) Passweb
  si preoccuperà di convertirle automaticamente in formato .webp.

In queste condizioni dunque la possibilità di lanciare manualmente una
conversione di tutte le immagini articolo e di categoria in formato webp
dovrebbe servire solo ed esclusivamente per risolvere eventuali problemi
(dovuti ad esempio alla mancata conversione automatica di una nuova
immagine articolo importata a seguito di una sincronizzazione).

Per maggiori informazioni in merito all'utilizzo del parametro "Attiva
Controllo su formato immagini .webp e .jp2" si veda anche quanto
indicato nel relativo capitolo ("*Sito -- Preferenze -- SEO Caricamento
Pagina*") di questo manuale

