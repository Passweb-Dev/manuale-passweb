# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_calendario_res.bmp](./assets/media/image25.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico.

Ovviamente nel momento in cui si dovesse decidere di staticizzare questo
tipo di componente, per fare in modo che, a seguito dell'inserimento da
back end di nuovi contenuti, i dati visualizzati dal componente siano
effettivamente quelli corretti sarà necessario rigenerare il codice HTML
del componente

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Pagina di Destinazione per l'Archivio News:** come precedentemente
evidenziato, nel momento in cui un utente dovesse cliccare su di una
qualsiasi delle date evidenziata all'interno del calendario, verrà
automaticamente ricondotto ad uno specifico archivio di notizie già
filtrate sulla base della data selezionata. Il parametro in oggetto
consente quindi di selezionare la specifica pagina del sito cui verrà
ricondotto l'utente dopo aver cliccato su di una specifica data
all'interno del calendario, e che dovrà, ovviamente, contenere un
componente CMS "Archivio News" con il parametro "Abilita Filtro Data"
selezionato.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Archivio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.

**Categoria Radice:** consente di specificare, selezionandola dal
sottostante albero delle categorie, la specifica categoria di News in
relazione alla quale dovranno essere evidenziate all'interno del
calendario le date di pubblicazione dei vari post.

In queste condizioni dunque, nel caso in cui si dovesse selezionare, ad
esempio, la categoria "Sport" all'interno del Calendario verrebbero
evidenziati solo ed esclusivamente i giorni in cui sono state pubblicate
all'interno del sito delle notizie appartenenti alla Categoria "Sport" e
ad eventuali sue sottocategorie.

> **NOTA BENE:** nel caso in cui si desideri ottenere un Calendario che
> tenga conto delle date di pubblicazione di tutte le news pubblicate
> all'interno del sito indipendentemente dalla loro categoria di
> appartenenza, il parametro "Categoria Radice" andrà impostato sul
> valore "Categorie CMS"

Oltre ad essere un filtro verso la pagina di destinazione per l'Archivio
News, definita in fase di configurazione del componete e a consentire
quindi all'utente di filtrare le varie news presenti in archivio secondo
quello che è la loro data di pubblicazione, il componente "Calendario"
accetta esso stesso dei filtri di visualizzazione.

Questo significa dunque che inserendo questo componente, ad esempio,
all'interno di una pagina Archivio (ossia di una pagina contenente il
componente "Archivio News"), nel momento in cui si dovessero applicare
dei filtri, per Autore, per Tag, per Categoria di News ecc ... a questo
archivio, questi stessi filtri potrebbero influenzare anche il
componente "Calendario" che potrebbe quindi ritrovarsi, ad esempio, ad
evidenziare soltanto le date in relazione alle quali sono state
pubblicate delle notizie per quello specifico autore o per quella
specifica categoria.

In questo senso dunque il parametro:

**Abilita Filtro Autore:** se selezionato renderà il corrispondente
componente "Calendario" filtrabile per Autore. In queste condizioni
dunque, nel momento in cui il componente dovesse essere inserito
all'interno di una pagina Archivio e all'Archivio News dovesse essere
applicato un filtro per Autore, anche il componente Calendario si
troverebbe ad evidenziare solo ed esclusivamente i giorni in relazione
ai quali sono state pubblicate all'interno del sito delle notizie di
quello stesso autore.

**Abilita Filtro Tag:** se selezionato renderà il corrispondente
componente "Calendario" filtrabile per Tag. In queste condizioni dunque,
nel momento in cui il componente dovesse essere inserito all'interno di
una pagina Archivio e all'Archivio News dovesse essere applicato un
filtro per Tag, anche il componente Calendario si troverebbe a
visualizzare solo ed esclusivamente i giorni in relazione ai quali sono
state pubblicate all'interno del sito delle notizie con quello specifico
Tag associato.

**Abilita Filtro Categoria:** se selezionato renderà il corrispondente
componente "Calendario" filtrabile per Categoria di News. In queste
condizioni dunque, nel momento in cui,il componente dovesse essere
inserito all'interno di una pagina Archivio e all'Archivio News dovesse
essere applicato un filtro per Categoria, anche il componente Calendario
si troverebbe a visualizzare solo ed esclusivamente i giorni in
relazione ai quali sono state pubblicate all'interno del sito delle
notizie appartenenti a quella specifica categoria di News.

**Abilita Filtro FullText:** se selezionato renderà il componente
"Calendario" filtrabile sulla base di specifiche ricerche effettuate
dall'utente utilizzando un apposito pannello di ricerca (componente
"Ricerca sul Sito" configurato per effettuare ricerche CMS). In queste
condizioni dunque sarebbe possibile, ad esempio, ricercare tutti i post
presenti in Archivio che contengono al parola "iOS" ed evidenziare nel
corrispondente Calendario tutti i giorni in relazione ai quali sono
stati pubblicati all'interno del sito dei post contenenti questa stessa
stringa.

**Visualizza anche i contenuti interni a una Gerarchia di Contenuti:**
selezionando questo parametro l'evidenziazione all'interno del
calendario dei giorni in corrispondenza dei quali sono state pubblicate
delle notizie, terrà conto anche dei contenuti interni ad eventuali
notizie strutturate presenti in archivio.

> **NOTA BENE:** il valore assegnato a questo parametro deve essere
> coerente con quello assegnato allo stesso parametro del corrispondente
> componente "Archivio News".

**Formato Mese:** consente di specificare il formato di visualizzazione
del nome del mese posto nella parte alta del calendario scegliendolo tra
la forma **Standard** (es. Novembre) e la forma **Abbreviata** (es. Nov)

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

