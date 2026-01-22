# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_lista_news_res.bmp](./assets/media/image3.png)

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

**Intestazione:** consente di indicare, in tutte le lingue attualmente
gestite all'interno del sito, un paragrafo che verrà poi visualizzato,
sul front end del sito, come intestazione del componente in esame.

**Tipologia Visualizzazione:** consente di definire la tipologia del
contenitore delle news che dovrà essere pubblicato all'interno del sito.

E' possibile selezionare uno dei seguenti valori:

- **Griglia:** selezionando questa opzioni le news presenti all'interno
  del componente verranno visualizzate in una griglia paginata

- **Slider:** selezionando questa opzione le news presenti all'interno
  del componente verranno disposte su di un\'unica riga all'interno di
  uno slider a scorrimento orizzontale.

**Autoplay (solo per configurazioni di tipo Slider):** consente di
decidere se abilitare o meno l'autoplay dello slider.

Se impostato sul valore "**Si avvia lo slider al caricamento**", al
caricamento della pagina web verrà attivato lo scorrimento automatico
delle varie Slide.

Se impostato a **NO** per passare da una Slide all'atra sarà necessario
cliccare su uno dei controlli di scorrimento abilitati.

**ATTENZIONE!** una volta abilitato l'autoplay, occorre comunque
ricordare che nel momento in cui l'utente dovesse decidere di cliccare
sui pulsanti di controllo, lo scorrimento automatico verrà arrestato.

**Tempo di pausa per autoplay (ms)**: visibile solo nel caso in cui il
precedente parametro "Autoplay" sia stato impostato sul valore "SI avvia
lo slider al caricamento".

Consente di impostare l'intervallo di tempo (in millisecondi) che dovrà
intercorrere tra il passaggio da una Slide all'altra.

**Tempo di animazione (solo per configurazioni di tipo Slider):**
consente di impostare la durata, in millisecondi, dell\'animazione di
passaggio da una slide all'altra.

**Posizionamento bottoni Slider (solo per configurazioni di tipo
Slider):** consente di decidere, selezionando una delle possibili
combinazioni presenti all'interno del corrispondente menu a tendina,
dove dovranno essere collocati i pulsanti di scorrimento dello slider.

**Pagina di Destinazione per il Dettaglio News:** consente di
selezionare la pagina del sito che dovrà essere utilizzata come pagina
di visualizzazione per il dettaglio della news selezionata.

Ovviamente affinché il dettaglio della News possa essere consultato in
maniera corretta, nella pagina di destinazione dovrà essere presente il
Componente "**Dettaglio News**" (con al suo interno il Componente
"**Articolo**")

**ATTENZIONE!** Nel momento in cui la pagina di destinazione dovesse
coincidere con la stessa pagina in cui è presente anche il componente
Lista News, il contenuto della news selezionata verrà caricato,
all'interno del componente "Dettaglio News", tramite javascript in
maniera tale da evitare il reload dell'intera pagina.

In queste condizioni per gestire correttamente le statistiche su
Analytics relativamente alle visite ricevute dai contenuti CMS sarà
necessario utilizzare Tag Manager configurando correttamente Google Tag
Manager\'s History Change trigger. Ogni volta che viene caricato un
contenuto tramite javascript viene infatti modificato l' url del browser
tramite history.pushState.

**Pagina di Destinazione Archivio News:** consente di selezionare la
pagina del sito che dovrà essere destinata a contenere l'archivio
all'interno del quale poter ricercare le varie notizie. Ovviamente
all'interno di questa stessa pagina dovrà poi essere necessariamente
presente il componente CMS "Archivio News".

In relazione ai due campi sopra indicati occorre fare alcune
considerazioni di fondamentale importanza e valide, in generale, per
tutti i componenti CMS gestiti all'interno del sito.

Per poter sfruttare appieno tutte le potenzialità della componentistica
CMS messa a disposizione da Passweb, sarà indispensabile gestire
all'interno del sito, almeno una pagina "Dettaglio" e una pagina
"Archivio" in cui inserire i corrispondenti componenti CMS.

La prima (pagina Dettaglio) consentirà infatti di visualizzare il
dettaglio delle varie notizie selezionate dall'utente all'interno del
sito. In questo senso, volendo sarebbe possibile gestire anche solo
un'unica pagina di questo tipo, in cui inserire cioè il componente
"Dettaglio News", in quanto il contenuto di questo stesso componente
varierà poi in maniera dinamica ed in base alla specifica notizia di cui
l'utente del sito a richiesto di visualizzare il dettaglio (in sostanza
potremmo tranquillamente paragonare la pagina dettaglio CMS alla pagina
Prodotto di un sito e-commerce).

La seconda (pagina Archivio) consentirà invece di gestire, attraverso il
corrispondente componente "Archivio News" un vero e proprio archivio di
tutte le notizie pubblicate all'interno del sito. In questo senso poi,
come indicato nella corrispondente sezione di questo manuale è possibile
gestire sia un unico archivio contenente tutte le notizie pubblicate
all'interno del sito, sia un singolo archivio per ogni singola categoria
di News.

In ogni caso comunque va detto che i vari elementi che potranno poi
essere inseriti all'interno di un componente "Lista News" piuttosto che
di un componente "Archivio News" (Titolo, Autore, Categorie o Tag
associati ecc ...) hanno associati specifici automatismi gestiti
dall'applicazione e tali per cui, ad esempio, cliccando sul nome
dell'autore del post, l'utente del sito potrebbe essere automaticamente
ricondotto alla corrispondente pagina Archivio, ritrovandosi già
impostato, sul componente "Archivio News" presente all'interno di questa
pagina, un filtro per autore e visualizzando dunque solo ed
esclusivamente le notizie redatte da quello specifico autore. Per queste
ragioni è indispensabile, come detto, gestire all'interno del sito,
almeno una pagina "Dettaglio" e una pagina "Archivio".

**Categorie Associate:** permette di selezionare la o le categorie di
News che dovranno essere visualizzate all'interno della Lista in
oggetto.

**Numero di News da Visualizzare:** consente di specificare il numero
esatto di notizie che dovranno essere visualizzate all'interno della
lista in oggetto. Tali notizie verranno poi ordinate sulla base della
loro specifica data di pubblicazione ponendo prima quelle con date più
recenti

**Formato data:** permette di impostare un particolare formato della
Data di Pubblicazione tra quelli proposti.

**Visualizza anche i contenuti interni a una Gerarchia Contenuti:** come
descritto all'interno della sezione "*Live Editing per Varianti
Responsive -- Gestione CMS -- Gestione Contenuti*" di questo manuale,
Passweb consente di creare sia delle semplici notizie, prive dunque di
una qualsiasi struttura, sia delle notizie più complesse e distribuite
dunque su di una generica gerarchia a N livelli. In questo senso il
parametro in oggetto consentirà di visualizzare o meno all'interno della
lista solo le radici di eventuali contenuti strutturati o anche i
singoli elementi componenti la struttura stessa.

**Numero di colonne:** le news presenti all'interno del componente
verranno visualizzate in una griglia responsiva NON paginata. Mediante
questo parametro è possibile impostare il numero di colonne e dunque il
numero di news che dovranno essere visualizzate all'interno di ogni
singola riga della griglia

**ATTENZIONE!** indipendentemente dal numero di news che si è scelto di
visualizzare all'interno del componente, per risoluzioni **inferiori ai
992 px** verranno sempre visualizzate 2 news per riga.

Analogamente per risoluzioni **inferiori a 768 px** la griglia si
linearizzerà mostrando una sola news per ogni riga

**Ordinamento:** consente di stabilire la modalità secondo cui dovranno
essere ordinate le notizie o i post presenti all'interno del componente
considerato. E' possibile selezionare uno dei seguenti valori:

- **In base al numero di Visualizzazioni:** selezionando questa opzione
  i post presenti all'interno della Lista verranno ordinati, in maniera
  decrescente, in base al numero di visualizzazioni ricevute.

> In queste condizioni il primo post ad essere visualizzato in lista
> sarà dunque quello che ha ricevuto più visualizzazioni in assoluto
>
> **ATTENZIONE!** Per ottenere una visualizzazione dovrà essere
> consultato il dettaglio del relativo post.
>
> La comparsa del post all'interno del componente "Lista News" non
> incrementa quindi in alcun modo il numero di visualizzazioni ottenute

- **Per data decrescente (prima i più recenti):** selezionando questa
  opzione i post presenti all'interno della Lista verranno ordinati, in
  maniera decrescente, in base alla loro data di pubblicazione

- **Per data crescente (prima i più vecchi):** selezionando questa
  opzione i post presenti all'interno della Lista verranno ordinati, in
  maniera crescente, in base alla loro data di pubblicazione

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
**il Componente "Lista News" può essere considerato a tutti gli effetti
come un "Componente di tipo Contenitore".** Sarà infatti possibile
inserire al suo interno dei campi che, per poter esser gestiti
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

In particolare all'interno di un componente di tipo "Lista News" sarà
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
> i componenti CMS interni ad un componente "Lista News" si veda la
> corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti CMS -- Componenti Interni ai Componenti
> CMS).

L'inserimento di questi componenti all'interno del Componente Lista News
avviene utilizzando le solite tecniche di interazione con l'editor (Drag
and Drop o Point and Click) già esaminate all'interno di questo manuale
(per maggiori informazioni si rimanda allo specifico capitolo di questo
manuale).

In ogni caso, comunque, la Lista News sarà costituita da un certo numero
di celle (una per ogni notizia pubblicata al suo interno). **I vari
componenti (siano essi Componenti Comuni o Componenti CMS) utilizzati
per costruire la propria lista potranno essere inseriti indistintamente
all'interno di una qualsiasi di queste celle (penserà poi l'applicazione
a ripeterli, in maniera completamente automatica, all'interno di tutte
le altre celle della lista)**

