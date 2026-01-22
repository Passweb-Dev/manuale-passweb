# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_cms0_res.bmp](./assets/media/image38.png)

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

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

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
ovviamente essere impostato sul valore **"Ricerca sul CMS"**

> **NOTA BENE:** una volta impostata la tipologia del pannello di
> ricerca che si intende realizzare e confermato il componente, tale
> tipologia non potrà più essere modificata.

**Colore di Sfondo Valore Attivo:** consente di impostare il colore di
sfondo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

**Colore del Testo Valore Attivo:** consente di impostare il colore del
Testo che verrà utilizzato per i campi di ricerca quando il filtro è
attivo

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
risultati del filtro impostato. E' possibile decidere di rimanere
all'interno della stessa pagina (opzione **"Rimani su questa pagina"**)
oppure selezionare una pagina specifica dal sottostante albero delle
pagine (opzione **"Rimanda alla pagina"**).

**ATTENZIONE! Affinché la ricerca possa funzionare in maniera corretta,
è indispensabile che nella pagina di destinazione sia presente un
componente CMS "Archivio News" con il parametro "Abilita Filtro
FullText" selezionato, oppure un componente "Risultati ricerca sul sito"
con abilitata la ricerca sui contenuti CMS.**

Nel primo caso il risultato sarà quello di visualizzare all'interno del
Componente "Archivio News" le sole notizie che soddisfano il filtro
impostato.

Nel secondo caso i risultati del filtro impostato verranno invece
visualizzati all'interno del componente "Risultati Ricerca sul sito".

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

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Ricerca sul Sito" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore".** Sarà infatti
possibile inserire al suo interno dei campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Per poter costruire quindi il proprio filtro di ricerca sarà necessario,
innanzitutto, attivare la modalità di gestione dei componenti. Occorrerà
poi portarsi sul Componente di ricerca presente nella pagina e, alla
comparsa del R.O.C. cliccare sull'icona "**Accedi ai componenti
interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Ricerca CMS" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale

- **Componenti per il Form:** contiene i componenti che potranno essere
  inseriti all'interno del componente "Ricerca" per poter realizzare e
  definire il proprio filtro.

Nel caso si decida di inserire all'interno del pannello di ricerca un
componente "Campo Testo", questo metterà a disposizione dell'utente un
semplice campo di input in cui l'utente stesso potrà digitare la stringa
di testo da ricercare.

**Nel caso in cui si decida di inserire all'interno di una Ricerca CMS
componenti quali "Campo Radio", "Campo Lista Checkbox" o "Campo Lista
Valori", sarà poi necessario mappare questi stessi elementi con
specifiche categorie CMS**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_cms_check_res.bmp](./assets/media/image39.png)

In questo modo **se (e soltanto se)** la ricerca CMS è utilizzata in
unione con un componente "Risultati Ricerca sul sito", oltre a digitare
il testo da ricercare l'utente avrà anche la possibilità di selezionare
diverse opzioni per effettuare un pre-filtro sulla tipologia di
risultato che intende ottenere.

