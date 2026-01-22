# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image6.png)

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
tipo di componente per fare in modo che vengano poi visualizzati
eventuali nuovi post inseriti dal back end del sito sarà necessario
rigenerare il codice HTML del componente

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

**Pagina di Destinazione per il Dettaglio News:** consente di
selezionare la pagina del sito che dovrà essere utilizzata come pagina
di visualizzazione per il dettaglio della news selezionata.

Ovviamente affinché il dettaglio della News possa essere consultato in
maniera corretta, nella pagina di destinazione dovrà essere presente il
Componente "**Dettaglio News**" (con al suo interno il Componente
"**Articolo**")

**ATTENZIONE!** Nel momento in cui la pagina di destinazione dovesse
coincidere con la stessa pagina in cui è presente anche il componente
Archivio News, il contenuto della news selezionata verrà caricato,
all'interno del componente "Dettaglio News", tramite javascript in
maniera tale da evitare il reload dell'intera pagina.

In queste condizioni per gestire correttamente le statistiche su
Analytics relativamente alle visite ricevute dai contenuti CMS sarà
necessario utilizzare Tag Manager configurando correttamente Google Tag
Manager\'s History Change trigger. Ogni volta che viene caricato un
contenuto tramite javascript viene infatti modificato l' url del browser
tramite history.pushState.

**Numero di News per pagina:** consente di specificare l'esatto numero
di notizie che dovranno essere visualizzate all'interno di ogni singola
pagina del componente.

**Numero di colonne:** le news presenti all'interno del componente
verranno visualizzate in una griglia responsiva paginata. Mediante
questo parametro è possibile impostare il numero di colonne e dunque il
numero di news che dovranno essere visualizzate all'interno di ogni
singola riga della griglia

**ATTENZIONE!** indipendentemente dal numero di news che si è scelto di
visualizzare all'interno del componente, per risoluzioni **inferiori ai
992 px** verranno sempre visualizzate 2 news per riga.

Analogamente per risoluzioni **inferiori a 768 px** la griglia si
linearizzerà mostrando una sola news per ogni riga

**Formato data:** permette di impostare un particolare formato della
Data di Pubblicazione tra quelli proposti.

**Dove vuoi visualizzare la paginazione?:** consente di indicare dove
posizionare la paginazione

**Numero di Pagine:** consente di impostare, selezionandolo dal relativo
menu a tendina, il numero di pagine che dovranno essere visualizzate nei
controlli di paginazione. Ovviamente oltre al numero indicato
all'interno di questo campo nei controlli di paginazione saranno sempre
visibili anche la prima e l'ultima pagina disponibili.

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Dove vuoi visualizzare la Paginazione" sia stato impostato su di un
valore diverso da "Non Visualizzare".**

**Paginazione con Precedente e Successivo:** se selezionato, nei
controlli di paginazione, verranno visualizzati anche i pulsanti
"Precedente" e "Successivo".

**Questo campo viene visualizzato solo nel caso in cui il parametro
"Dove vuoi visualizzare la Paginazione" sia stato impostato su di un
valore diverso da "Non Visualizzare".**

**Tipo di Paginazione per dispositivi desktop (**\>= **992px):**
consente di definire il tipo di paginazione da utilizzare, per il
componente in oggetto, su dispositivi desktop (risoluzione maggiore o
uguale a 992px)

E' possibile selezionare uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scroll bar per visualizzare i
  risultati presenti all'interno della nuova pagina)

- **A richiesta:** selezionando questa tipologia di paginazione verrà
  visualizzato sopra e/o sotto il componente (dipendentemente da come è
  stato impostato il precedente parametro "Visualizza Paginazione") un
  pulsante "**Mostra Altri Risultati**" che l'utente dovrà utilizzare
  per richiedere la visualizzazione delle news presenti nelle successive
  pagine del catalogo.

- **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
  paginazione le news distribuite all'interno delle varie pagine,
  verranno visualizzate automaticamente mano a mano che l'utente
  scorrerà la pagina web verso l'alto

**Tipo di Paginazione per dispositivi mobile (\<** **992px):** consente
di definire il tipo di paginazione da utilizzare, per il componente in
oggetto, su dispositivi mobile (risoluzione minore a 992px). E'
possibile selezionare uno dei seguenti valori:

- **A richiesta:** selezionando questa tipologia di paginazione verrà
  visualizzato sopra e/o sotto il componente (dipendentemente da come è
  stato impostato il precedente parametro "Visualizza Paginazione") un
  pulsante "**Mostra Altri Risultati**" che l'utente dovrà utilizzare
  per richiedere la visualizzazione delle news presenti nelle successive
  pagine del catalogo.

- **Scroll infinito (Lazy Loading):** selezionando questa tipologia di
  paginazione le news distribuite all'interno delle varie pagine,
  verranno visualizzate automaticamente mano a mano che l'utente
  scorrerà la pagina web verso l'alto

**Categoria Radice:** consente di selezionare dal sottostante albero
delle categorie, la specifica categoria di News che dovranno essere
visualizzate all'interno del componenti in oggetto.

> **NOTA BENE:** per maggiori informazioni relativamente a come creare e
> gestire le varie categorie di News si rimanda alla relativa sezione di
> questo manuale (Live Editing per Varianti Responsive -- Gestione CMS
> -- Gestione Categorie).

Nel caso in cui, dunque, all'interno del componente debbano essere
presenti tutte le notizie pubblicate all'interno del sito,
indipendentemente dalla loro specifica categoria di appartenenza, sarà
sufficiente o non selezionare nessun categoria oppure selezionare la
radice dell'albero (Categorie CMS)

**Propaga il filtro sulla Categoria anche sui Contenuti Interni:** se
selezionato, consente di propagare il filtro sulla categoria di News,
impostato attraverso il precedente parametro, anche ai singoli
componenti inseriti e gestiti all'interno dell'Archivio considerato.

Supponiamo di voler visualizzare all'interno del nostro Archivio News i
soli post appartenenti alla categoria "Notizie ed Eventi" e di aver per
questo correttamente settato il precedente parametro "Categoria Radice".

Supponiamo inoltre di aver inserito all'interno dell'Archivio un
componente "Indice Libro" con al suo interno un contenuto strutturato su
N livelli la cui radice appartiene alla categoria "Notizie ed Eventi".

Supponiamo infine che alcuni elementi del contenuto strutturato
appartengano alla categoria "Notizie ed Eventi" ed altri no.

In queste condizioni nel caso in cui il parametro in oggetto sia stato
selezionato, all'interno dell'indice libro verranno visualizzati solo ed
esclusivamente quegli elementi interni al contenuto strutturato
associati alla categoria "Notizie ed Eventi".

Nel caso in cui il parametro in oggetto non sia stato selezionato,
verranno invece visualizzati all'interno dell'Indice Libro tutti i suoi
elementi interni indipendentemente dalla loro specifica categoria di
appartenenza.

**Ignora le Pagine di Lettura di Categoria nei links:** consente di
ignorare eventuali pagine di Lettura per il dettaglio delle News
impostate specificatamente sulle singole categorie di appartenenza delle
News stesse.

Per ogni singola categoria di News, volendo, è infatti possibile
definire una specifica pagina del sito da utilizzare come pagina per la
visualizzazione del dettaglio delle notizie appartenenti a quella stessa
categoria.

Supponendo dunque di aver impostato una pagina di questo tipo, ad
esempio per la categoria "Notizie ed Eventi", e di non aver selezionato
il parametro "Ignora le Pagine di Lettura di Categoria nei links", nel
caso in cui un utente dovesse poi cliccare sul titolo o sull'immagine di
una notizia presente all'interno dell'Archivio considerato, ed
appartenente a questa stessa categoria, per consultare il dettaglio
della notizia selezionata verrebbe ricondotto alla pagina di lettura
impostata sulla categoria (indipendentemente dunque da quanto impostato
per il parametro "Pagina di Destinazione per il Dettaglio News"
dell'archivio considerato).

Nel caso in cui invece in queste stesse condizioni fosse stato
selezionato il parametro "Ignora le Pagine di Lettura di Categoria nei
links" cliccando sul titolo o sull'immagine di una notizia presente
all'interno dell'Archivio considerato, ed appartenente alla categoria
"Notizie ed Eventi", per consultare il dettaglio della notizia
selezionata l'utente verrebbe ricondotto alla pagina impostata come
"Pagina di Destinazione per il Dettaglio News" per l'Archivio
considerato (indipendentemente, questa volta, da eventuali pagine di
lettura impostate specificatamente sulla categoria di appartenenza della
News)

**Abilita Filtro Data:** se selezionato consentirà poi di filtrare le
varie notizie presenti in Archivio secondo quella che è la loro data di
pubblicazione. Nel momento in cui, dunque, un utente dovesse cliccare
sulla data di pubblicazione di una specifica notizia, l'archivio
mostrerebbe tutte le notizie pubblicate in quella specifica data.

**Abilita Filtro Autore:** se selezionato consentirà poi di filtrare le
varie notizie presenti in Archivio secondo quella che è il loro autore.
Nel momento in cui, dunque, un utente dovesse cliccare sul nome di un
autore di una specifica notizia, l'archivio mostrerebbe tutte le notizie
pubblicate da quello specifico autore.

**Abilita Filtro Tag:** se selezionato consentirà poi di filtrare le
varie notizie presenti in Archivio sulla base dei loro Tag Associati.
Nel momento in cui, dunque, un utente dovesse cliccare su di un
qualsiasi Tag associato ad una qualsiasi notizia presente in archivio
l'archivio stesso mostrerebbe tutte le notizie con associate lo stesso
Tag.

**Abilita Filtro Categoria:** se selezionato consentirà poi di filtrare
le varie notizie presenti in Archivio secondo quella che è la loro
categoria di appartenenza. Nel momento in cui, dunque, un utente dovesse
cliccare sul nome di una qualsiasi Categoria associata ad una qualsiasi
notizia presente in archivio, l'archivio stesso mostrerebbe solo ed
esclusivamente le notizie di quella stessa categoria.

**Abilita Filtro Full Text:** se selezionato consentirà poi di ricercare
le varie notizie presenti in Archivio mediante l'utilizzo di un
componente "**Ricerca sul sito**" opportunamente configurato.

Nel momento in cui dunque si volesse realizzare un apposito pannello di
ricerca per consentire all'utente di effettuare ricerche personalizzate
sulle News presenti in Archivio, diventerebbe di fondamentale importanza
selezionare questo parametro, rendendo di fatto il corrispondente
archivio filtrabile sulla base delle ricerche effettuate dai singoli
utenti.

> **NOTA BENE:** nel caso in cui questo parametro non sia stato
> selezionato, ogni ricerca realizzata attraverso un componente "Ricerca
> sul sito" configurato per agire su questo stesso Archivio, non
> produrrà alcun risultato.

**Abilita Filtri Multipli:** se selezionato consentirà di applicare
all'Archivio più filtri contemporaneamente. Tali filtri verranno
considerati in and tra loro.

Una volta applicato uno qualsiasi dei filtri sopra indicati, questo
stesso filtro potrà essere rimosso cliccando sul corrispondente pulsante
**"Rimuovi Filtro"**

![](./assets/media/image7.png)

**Visualizza anche i contenuti interni a una Gerarchia di Contenuti:**
se selezionato consentirà di visualizzare all'interno del corrispondente
archivio anche i contenuti interni ad ogni singola notizia strutturata.
In caso contrario, in relazione alle notizie strutturate, verranno
visualizzate, in Archivio, le sole radici.

**Visualizzazione Risultati:** se selezionato, consentirà di
visualizzare, nella parte bassa del componente, una stringa di testo
contenente il numero complessivo dei risultati che soddisfano la ricerca
effettuata.

Il testo di questa stringa può essere modificato e personalizzato alla
sezione \"Gestione Testi/Messaggi del Sito\" agendo sui testi del
componente in oggetto.

**Ordinamento:** consente di stabilire la modalità secondo cui dovranno
essere ordinate le notizie o i post presenti all'interno del componente
considerato. E' possibile selezionare uno dei seguenti valori:

- **In base al numero di Visualizzazioni:** selezionando questa opzione
  i post presenti in Archivio verranno ordinati, in maniera decrescente,
  in base al numero di visualizzazioni ricevute.

> In queste condizioni il primo post ad essere visualizzato sarà dunque
> quello che ha ricevuto più visualizzazioni in assoluto
>
> **ATTENZIONE!** Per ottenere una visualizzazione dovrà essere
> consultato il dettaglio del relativo post.
>
> La comparsa del post all'interno del componente "Archivio News" non
> incrementa quindi in alcun modo il numero di visualizzazioni ottenute

- **Per data decrescente (prima i più recenti):** selezionando questa
  opzione i post presenti all'interno dell'Archivio verranno ordinati,
  in maniera decrescente, in base alla loro data di pubblicazione

- **Per data crescente (prima i più vecchi):** selezionando questa
  opzione i post presenti all'interno dell' Archivio verranno ordinati,
  in maniera crescente, in base alla loro data di pubblicazione

- **In base al campo "Posizione":** selezionando questa opzione i post
  presenti all'interno dell'Archivio verranno ordinati sulla base del
  valore presente all'interno del loro campo "Posizione"

> **NOTA BENE:** per maggiori informazioni relativamente a come
> associare una specifica data di pubblicazione o uno specifico valore
> per il campo "Posizione" ad un contenuto CMS, si veda anche la sezione
> "Sito -- Gestione CMS" di questo manuale.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Archivio News" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore".** Sarà infatti
possibile inserire al suo interno dei campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Una volta inserito il Componente all'interno della pagina, per poterne
poi personalizzare i contenuti sarà necessario attivare la modalità di
gestione dei componenti, portarsi sul Componente in esame e, alla
comparsa del R.O.C. cliccare sull'icona "**Accedi ai componenti
interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Archivio News" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il layout del
  componente. Per maggiori informazioni relativamente all'utilizzo di
  questi componenti si vedano le corrispondenti sezioni di questo
  manuale.

- **Componenti CMS:** contiene quei componenti necessari a visualizzare
  all'interno del componente in oggetto i singoli elementi componenti
  una notizia (Titolo, Autore, Sommario, Articolo ecc ...).

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i componenti CMS interni ad un componente "Archivio News" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti CMS -- Componenti Interni ai Componenti
> CMS).

L'inserimento di questi componenti all'interno del Componente Archivio
News avviene utilizzando le solite tecniche di interazione con l'editor
(Drag and Drop o Point and Click) già esaminate all'interno di questo
manuale (per maggiori informazioni si rimanda allo specifico capitolo di
questo manuale).

In ogni caso, comunque, l' Archivio News sarà costituito da un certo
numero di celle (una per ogni notizia pubblicata al suo interno). **I
vari componenti (siano essi Componenti Comuni o Componenti CMS)
utilizzati per costruire il proprio archivio potranno essere inseriti
indistintamente all'interno di una qualsiasi di queste celle (penserà
poi l'applicazione a ripeterli, in maniera completamente automatica,
all'interno di tutte le altre celle dell'archivio)**

