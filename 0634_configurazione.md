# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image2.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** permette di inserire un nome per il campo che si sta editando;

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Cosa vuoi mostrare?**: consente di definire il tipo di dato che dovrà
essere pubblicato all'interno del sito mediante il componente in
oggetto.

E' possibile selezionare una delle seguenti opzioni:

- **Promozioni**: in queste condizioni il componente mostrerà le
  Promozioni appositamente configurate all'interno della corrispondente
  sezione del gestionale ("*Marketing -- Promozioni*")

![](./assets/media/image3.png)

> Nello specifico all'interno del componente in oggetto **verranno
> visualizzate solo ed esclusivamente le Promozioni Welcome che
> soddisfano le seguenti specifiche:**

- **Sono Promozioni Attive**

- **Hanno il check "Visualizza in homepage" correttamente selezionato**

- **Hanno una data di fine validità (campo "Prenotabile al") maggiore o
  uguale alla Data odierna**

> Per ciascuna delle Promozioni presenti all'interno del componente
> verranno poi visualizzate le seguenti informazioni:

- Nome

- Descrizione

- Codice

- Immagine

- Periodo di Validità

- Link di collegamento al dettaglio sulla corrispondente pagina del
  Booking Engine

> **ATTENZIONE!** per quel che riguarda il **Nome** e la **Descrizione**
> della specifica Promozione verranno visualizzati, in relazione anche
> alle lingue gestite (tanto sul sito quanto su Welcome), i testi
> presenti all'interno della sezione "**Traduzioni**"

![](./assets/media/image4.png)

**Tipologia di visualizzazione:** consente di definire come dovranno
essere mostrati gli elementi presenti all'interno del componente.

E' possibile selezionare uno dei seguenti valori:

- **Slider:** selezionando questa opzione gli elementi presenti
  all'interno del componente verranno disposti su di un\'unica riga
  all'interno di uno slider a scorrimento orizzontale.

![](./assets/media/image5.png)

- **Griglia:** selezionando questa opzione gli elementi presenti
  all'interno del componente verranno visualizzati all'interno di una
  griglia responsiva, organizzata su di un certo numero di colonne
  impostabili mediante i successivi parametri presenti all'interno di
  questa stessa maschera di configurazione

![](./assets/media/image6.png)

**Numero di Elementi da Visualizzare -- (solo per configurazioni di tipo
Slider):** consente di impostare il numero massimo di slide che dovranno
essere visualizzate contemporaneamente.

**ATTENZIONE!** indipendentemente dal valore impostato all'interno del
parametro in oggetto, per risoluzioni inferiori a 1200px e 992px
verranno visualizzate rispettivamente due e una sola slide alla volta (è
comunque possibile variare questo comportamento di default a livello di
codice CSS)

**Posizione bottoni Slider -- (solo per configurazioni di tipo
Slider):** consente di decidere, selezionando una delle possibili
combinazioni presenti all'interno del corrispondente menu a tendina,
dove dovranno essere collocati i pulsanti di scorrimento dello slider.

**Autoplay -- (solo per configurazioni di tipo Slider):** consente di
decidere se abilitare o meno l'autoplay dello slider.

Se impostato sul valore "**Si avvia lo slider al caricamento**", al
caricamento della pagina web verrà attivato lo scorrimento automatico
delle varie Slide.

Se impostato a **NO** per passare da una Slide all'atra sarà necessario
cliccare su uno dei controlli di scorrimento abilitati.

**ATTENZIONE!** una volta abilitato l'autoplay, occorre comunque
ricordare che nel momento in cui l'utente dovesse decidere di cliccare
sui pulsanti di controllo, lo scorrimento automatico verrà arrestato.

**Tempo di pausa per autoplay (ms) -- (solo per configurazioni di tipo
Slider)**: visibile solo nel caso in cui il precedente parametro
"Autoplay" sia stato impostato sul valore "Si avvia lo slider al
caricamento".

Consente di impostare l'intervallo di tempo (in millisecondi) che dovrà
intercorrere tra il passaggio da una Slide all'altra.

**Tempo di animazione (ms) -- (solo per configurazioni di tipo
Slider):** consente di impostare la durata, in millisecondi,
dell\'animazione di passaggio da una slide all'altra.

**Numero di elementi in ogni riga -- (solo per configurazioni di tipo
Griglia):** consente di impostare il numero di colonne e quindi il
numero di promozioni che dovranno essere visualizzate per singola riga.

In relazione a questo parametro vanno fatte poi alcune considerazioni di
fondamentale importanza legate al comportamento responsivo del
componente.

In particolare dunque è bene ricordare che:

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  la griglia, indipendentemente dal numero di promozioni che si è scelto
  di visualizzare all'interno di ogni singola riga, per risoluzioni:

  - **inferiori ai 1200 px** verranno visualizzate automaticamente 3
    promozioni per riga

  - **inferiori ai 992 px** verranno visualizzate automaticamente 2
    promozioni per riga

  - **Inferiori ai 768** px verrà visualizzate automaticamente una sola
    promozione per riga

- Nel caso in cui sia stata impostata come tipologia di visualizzazione
  lo slider, indipendentemente dal numero di articoli che si è scelto di
  visualizzare all'interno della singola riga, per risoluzioni
  **inferiori ai 992 px** lo slider mostrerà sempre e soltanto un solo
  articolo alla volta

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

