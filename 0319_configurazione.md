# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image189.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile settare i
principali parametri di configurazione.

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

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico

**ATTENZIONE!** Per maggiori informazioni relativamente al parametro
**Statico** si veda anche quanto indicato all'interno del capitolo
"*Configurazione Componenti -- Caratteristiche generali* --
*Staticizzazione e caricamento asincrono*" di questo manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Immagine Segnaposto / Segnaposto Smartphone / Segnaposto Tablet**:
consente di indicare una specifica immagine da utilizzare, alle diverse
risoluzioni (desktop, smartphone e tablet), prima che lo slider venga
effettivamente inizializzato via javascript.

**ATTENZIONE!** Il campo in esame non è multilingua per cui l'immagine
utilizzata come segnaposto sarà sempre la stessa per ciascuna delle
lingue gestite all'interno del sito

Le risorse gestite attraverso questi segnaposto possono diventare di
fondamentale importanza nel momento in cui l'immagine presente nella
prima slide del componente dovesse essere individuata come il Largest
Contentful Paint (LCP) della pagina.

Considerando infatti che il componente in esame necessita
obbligatoriamente di apposite funzioni javascript per poter operare in
maniera corretta, se l'immagine presente nella prima slide dovesse
essere effettivamente individuata come il LCP, il fatto di dover
attendere l'inizializzazione del componente via javascript, prima di
poterla avere disponibile nella pagina, potrebbe aumentare i tempi di
caricamento del LCP. L'utilizzo delle immagine segnaposto consente
invece di visualizzare l'immagine individuata come LCP prima ancora che
lo slider venga inizializzato via javascript ottimizzando quindi i tempi
di caricamento del relativo Core web Vital.

**ATTENZIONE!** In queste condizioni è ovviamente di fondamentale
importanza che l'immagine utilizzata come segnaposto sia esattamente la
stessa o che abbia quanto meno le stesse esatte dimensioni dell'immagine
che verrà poi effettivamente visualizzata nella prima Slide del
componente (in maniera tale da evitare effetti grafici indesiderati che
potrebbero portare anche ad un aumento del Cumulative Layout Shift, un
altro dei Core Web Vitals valutati da Google)

**Autoplay:** consente di decidere se abilitare o meno l'autoplay dello
slider.

Se impostato sul valore "**Si avvia lo slider al caricamento**", al
caricamento della pagina web verrà attivato lo scorrimento automatico
delle varie Slide.

Se impostato a **NO** per passare da una Slide all'atra sarà necessario
cliccare su uno dei controlli di scorrimento abilitati.

**Tempo di pausa per autoplay (ms)**: visibile solo nel caso in cui il
precedente parametro "Autoplay" sia stato impostato sul valore "SI avvia
lo slider al caricamento". Consente di impostare l'intervallo di tempo
(in millisecondi) che dovrà intercorrere tra il passaggio da una Slide
all'altra.

**Numero di Righe:** consente di impostare il numero di righe su cui
dovranno essere disposti i contenuti dello Slider.

**Numero di Slide da Mostrare:** consente di definire il numero
complessivo di Slide da visualizzare contemporaneamente all'interno
dello Slider

![](./assets/media/image190.png)

**Numero di Slide da Scrollare:** consente di definire il numero di
slide da scrollare tra un passaggio e l'altro. Supponendo dunque di
impostare questo parametro sul valore 3 le Slide presenti all'interno
del componente si sposteranno 3 alla volta. Nel caso in cui l'esigenza
dovesse invece essere quella di spostare un elemento alla volta il
parametro andrà ovviamente impostato sul valore 1.

**Controlli di Scorrimento:** consente di selezionare il tipo di
controllo che dovrà essere abilitato sul componente per consentire
all'utente di passare da una slide all'altra. E' possibile selezionare
uno dei seguenti valori:

- **Solo barra di scorrimento veloce:** in queste condizioni verrà
  abilitata una piccola barra contenente tanti pallini quante sono le
  sezioni scrollabili dello slider

![](./assets/media/image191.png)

- **Solo pulsanti:** in queste condizioni verranno abilitate due piccoli
  pulsanti per il passaggio alla slide precedente / successiva

![](./assets/media/image192.png)

- **Pulsanti e Barra di Scorrimento veloce:** in queste condizioni
  verranno attivati sul componente sia la barra di scorrimento veloce
  che i pulsanti per il passaggio alla slide precedente / successiva

**Visualizza Anteprima:** consente di decidere se visualizzare o meno,
oltre allo slider, anche l'anteprima dell'immagine attualmente
selezionata.

![](./assets/media/image193.png)

**ATTENZIONE!** Nel momento in cui si dovesse decidere di visualizzare
sia lo slider che l'anteprima, ogni singola miniatura presente
all'interno dello slider rappresenterà, in un certo senso, un controllo
di scorrimento. Cliccando infatti su una di queste miniature verrà
immediatamente visualizzata la corrispondente anteprima.

**Simulazione Slide Infinte:** consente di stabilire quello che dovrà
essere il comportamento del componente nel momento in cui verrà
raggiunta l'ultima slide. E' possibile selezionare una delle seguenti
opzioni:

- **NO**: in queste condizioni una volta raggiunta l'ultima Slide il
  componente si bloccherà e non ci sarà nessun passaggio verso altre
  Slide

- **SI**: in queste condizioni, una volta raggiunta l'ultima slide il
  componente ripartirà automaticamente dalla prima entrando dunque in un
  ciclo infinito

**Effetto dissolvimento:** consente di impostare l'animazione che dovrà
essere attivata al passaggio da una slide all'altra. E' possibile
selezionare uno dei seguenti valore:

- **SI**: in queste condizioni il passaggio da una slide all'altra
  avverrà con un'animazione di fade

- **NO**: in queste condizioni il passaggio da una slide all'altra
  avverrà con una semplice animazione di scorrimento da sinistra verso
  destra piuttosto che da destra verso sinistra.

**Effetto di comparsa della slide:** visibile solo nel caso in cui il
precedente parametro "Effetto dissolvimento" sia stato impostato sul
valore NO. Consente di impostare la velocità di esecuzione dell'effetto
di scorrimento che regola il passaggio da una slide all'altra. E'
possibile selezionare uno dei seguenti valori:

- **Entra lenta e accelera nel finale**

- **Entra lenta, accelera e rallenta nel finale**

- **Entra veloce e rallenta nel finale**

- **Velocità costante**

**Orientamento Slider:** consente di decidere se disporre lo slider in
orizzontale piuttosto che in verticale

**Scorrimento -- Posizione di partenza delle slide all'interno dello
slider**: consente di definire quella che dovrà essere la posizione di
partenza delle slide all'interno dello slider. E' possibile selezionare
uno dei seguenti valori:

- **Allineate al margine sinistro dello slider:** in queste condizioni
  la prima slide, tra quelle visibili all'interno dello slider, si
  disporrà allineata al margine sinistro dello slider stesso

![](./assets/media/image194.png)

- **Centrate**: in queste condizioni le slide visibili all'interno dello
  slider si disporranno in maniera tale da essere centrate rispetto allo
  slider stesso

![](./assets/media/image195.png)

**Altezza adattiva della slide:** se impostato a SI ogni singola slide
adatterà automaticamente la sua altezza in base ai suoi contenuti. Al
contrario se impostato NO tutte le slide avranno un altezza fissa.

**Tempo di animazioni (ms):** consente di impostare la durata (in
millisecondi) dell'effetto di transizione utilizzato per il passaggio da
una slide all'altra.

**Ferma il loop al passaggio del mouse/tap**: consente, se selezionato,
di bloccare il passaggio automatico da una slide all'altra (Autoplay =
SI) nel momento in cui si dovesse posizionare il mouse sul
componente[.]{.underline}

Una volta settati i parametri di configurazione del Componente sarà poi
necessario, ovviamente, definire i contenuti di ogni singola Slide
agendo, in questo senso, dalla sezione "Gestione Contenuti" presente
nella maschera di configurazione di questa specifica tipologia di
componenti.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

