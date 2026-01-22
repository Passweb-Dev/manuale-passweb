# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_tag_cloud_res.bmp](./assets/media/image28.png){width="4.623611111111111in"
height="3.084722222222222in"}

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

**Numero di Tag visualizzati:** consente di specificare il numero
massimo di Tag che dovranno essere visualizzati all'interno della
nuvola.

**Dimensione minima/massima Font:** come precedentemente evidenziato
all'interno di questo componente verrà visualizzato un elenco pesato dei
tag maggiormente utilizzati all'interno del sito. Il peso dei vari tag,
inteso esclusivamente come frequenza di utilizzo di questi stessi tag
all'interno del sito, è reso con caratteri di dimensioni diverse, il che
significa quindi che più grande è il carattere, maggiore è la frequenza
con cui il relativo Tag è stato utilizzato all'interno del sito.

In questo senso dunque, il parametro "Dimensione minima/massima Font"
consente di specificare il font minimo e massimo da utilizzare per la
visualizzazione rispettivamente dei Tag meno e più usati all'interno del
sito.

**Visualizza anche i contenuti interni a una Gerarchia di Contenuti:**
selezionando questo parametro l'evidenziazione all'interno del
calendario dei giorni in corrispondenza dei quali sono state pubblicate
delle notizie, terrà conto anche dei contenuti interni ad eventuali
notizie strutturate presenti in archivio.

> **NOTA BENE:** il valore assegnato a questo parametro deve essere
> coerente con quello assegnato allo stesso parametro del corrispondente
> componente "Archivio News".

**Pagina di Destinazione per l'Archivio News:** nel momento in cui un
utente dovesse cliccare su di uno qualsiasi dei Tag presenti all'interno
di questo componente, verrà automaticamente ricondotto ad uno specifico
archivio di notizie già filtrate sulla base dello specifico Tag
selezionato. Il parametro in oggetto consente quindi di selezionare la
specifica pagina del sito cui verrà ricondotto l'utente dopo selezionato
uno specifico tag all'interno della nuvola, e che dovrà, ovviamente,
contenere un componente CMS "Archivio News" con il parametro "Abilita
Tag" selezionato.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> del componente "Archivio News" e dei suoi componenti interni si
> rimanda alla relativa sezione di questo manuale.

**Categoria Radice:** consente di specificare, selezionandola dal
sottostante albero delle categorie, la specifica categoria di News in
relazione alla quale dovranno essere visualizzati i Tag presenti
all'interno della nuvola.

> In queste condizioni dunque, nel caso in cui si dovesse selezionare,
> ad esempio, la categoria "Sport" all'interno della nuvola verrebbero
> visualizzati solo ed esclusivamente i tag associati ai post della
> Categoria "Sport" e ad eventuali sue sottocategorie.
>
> **NOTA BENE:** nel caso in cui si desideri ottenere una nuvola di tag
> che tenga conto di tutte le news pubblicate all'interno del sito
> indipendentemente dalla loro categoria di appartenenza, il parametro
> "Categoria Radice" andrà impostato sul valore "Categorie CMS"

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

