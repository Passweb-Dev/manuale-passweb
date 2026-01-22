# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e di configurazione**

![](./assets/media/image199.png)

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
essere reso statico

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

**Tipo:** consente di indicare la tipologia del pannello di ricerca che
si sta realizzando specificando quindi anche la funzione che tale
pannello dovrà espletare. Nel caso specifico tale parametro dovrà
ovviamente essere impostato sul valore **"Ricerca Testuale"**

**Colore di Sfondo Valore Attivo:** consente di impostare il colore di
sfondo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

**Colore del Testo Valore Attivo:** consente di impostare il colore del
Testo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

**Identificatore:** consente di legare tra loro due o più pannelli di
ricerca in maniera tale da poterli poi gestire come se fossero il
medesimo pannello.

Il campo è **numerico** ed opzionale per cui andrà valorizzato solo ed
esclusivamente nel momento in cui sia effettivamente necessario legare
tra loro due o più pannelli distinti.

Supponiamo, ad esempio, di dover fare in modo che il filtro impostato in
un pannello di ricerca presente nella Home Page del sito sia mantenuto
anche all'interno di un altro pannello di ricerca (ovviamente dello
stesso tipo), collocato, ad esempio, in una diversa posizione della
pagina "Risultati Ricerca".

Considerando che i due pannelli di ricerca sono due distinti componenti
Passweb, e **NON** lo stesso componente distribuito sulle due diverse
pagine, l'unica possibilità che avremo per soddisfare questa esigenza
sarà quella di impostare il campo "Identificatore" di entrambi i
pannelli sullo stesso valore numerico (es. 1).

Ovviamente il pannello in Home Page dovrà essere configurato in maniera
tale che la sua destinazione sia la pagina "Risultati Ricerca", mentre
quello presente all'interno della pagina "Risultati Ricerca" dovrà
essere configurato per restare in quella stessa pagina

In queste condizioni nel momento in cui un utente del sito dovesse
effettuare una ricerca partendo dal pannello presente in Home Page verrà
poi ricondotto alla pagina "Risultati Ricerca" dove, oltre a
visualizzare il risultato della ricerca effettuata, si ritroverà anche,
nel pannello presente in questa pagina gli stessi valori del filtro
impostato nel pannello della Home Page

**ATTENZIONE!** I pannelli di ricerca collegati unicamente mediante il
parametro "Identificatore" restano sempre e comunque componenti distinti
per cui eventuali modifiche (grafiche e/o di configurazione) effettuate
per uno di essi non verranno riportate automaticamente anche sugli altri

**Ricerca Iniziale:** consente di dichiarare il filtro che dovrà essere
applicato in maniera automatica ogni volta in cui l'utente effettuerà
l'accesso ad una pagina del sito in cui è contenuto il pannello di
ricerca in questione.

Per maggiori informazioni relativamente a come poter determinare
l'effettivo valore da inserire all'interno di questo campo si veda anche
il successivo capitolo "*Querystring di ricerca -- Applicazione di un
filtro iniziale*" di questo manuale.

**Destinazione:** consente di impostare la specifica pagina di
destinazione all'interno della quale dovranno essere visualizzati i
risultati della ricerca effettuata. E' possibile decidere di rimanere
all'interno della stessa pagina (opzione "Rimani su questa pagina")
oppure selezionare una pagina specifica dal sottostante albero delle
pagine (opzione **"Rimanda alla pagina"**).

**In ogni caso affinché questo tipo di ricerca possa funzionare in
maniera corretta, è indispensabile che nella pagina di destinazione sia
presente il componente "Risultati Ricerca sul Sito".**

**ATTENZIONE!** L'applicazione automatica di un filtro iniziale
(parametro "**Ricerca Iniziale**") non produrrà mai un cambio di pagina.
Questo tipo di filtri quindi, verranno applicati sempre e soltanto alla
pagina in cui si trova il pannello in questione

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- Il pannello di ricerca (Campi)

- Il pulsante per avviare la ricerca (Submit)

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, **il
Componente "Ricerca sul Sito" può essere considerato a tutti gli effetti
come un "Componente di tipo Contenitore".**

Nel caso specifico ovviamente all'interno del pannello di ricerca potrà
essere inserito unicamente un componente di tipo "Campo Testo", in tutto
e per tutto simile al componente "Campo Testo" che può essere inserito
all'interno di un componente "Form", e che metterà dunque a disposizione
dell'utente un semplice campo di input in cui l'utente stesso potrà
digitare lo specifico testo da ricercare.

