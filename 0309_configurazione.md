# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image163.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Caricamento Javascript**: se selezionato, consente di caricare il
  relativo componente in maniera asincrona al termine del caricamento
  della pagina web.

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Caricamento Javascript** e **Statico** si veda anche quanto indicato
> all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Staticizzazione e caricamento
> asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

- **Aspect Ratio:** consente di impostare, selezionandolo dal relativo
  menu a tendina, il rapporto larghezza/altezza del video

- **Sorgente:** consente di indicare la sorgente da cui prelevare il
  video. E' possibile selezionare uno dei seguenti valori:

  - **Youtube:** selezionando questa opzione il video da inserire
    all'interno del sito dovrà essere pubblicato su Youtube

  - **Vimeo:** selezionando questa opzione il video da inserire
    all'interno del sito dovrà essere pubblicato su Vimeo

  - **Custom:** selezionando questa opzione il video da inserire
    all'interno del sito potrà essere pubblicato su di una qualsiasi
    altra piattaforma (diversa da Youtube o Vimeo)

- **Link:** consente di indicare l' url dello specifico video che dovrà
  essere visualizzato all'interno del sito.

> Nel caso in cui la **Sorgente del video dovesse essere YouTube** per
> individuare l' url da inserire all'interno di questo campo sarà
> necessario:

- Accedere, su YouTube, alla pagina di visualizzazione del video e
  cliccare sul pulsante "**Condividi**"

![](./assets/media/image164.png)

- Selezionare dal corrispondente menu contestuale l'opzione
  "**Incorpora**"

![](./assets/media/image165.png)

- Prelevare, dal codice di incorporamento, il link del video di YouTube
  (valore dell' attributo src dell' iframe) e inserirlo come valore del
  parametro **Link** nella maschera di configurazione del componente
  Passweb

![](./assets/media/image166.png)

> In maniera del tutto analoga nel caso in cui la sorgente del video
> dovesse essere **Vimeo** sarà necessario:

- Accedere, su Vimeo, alla pagina di visualizzazione del video e
  cliccare sul pulsante "**Share**"

![](./assets/media/image167.png)

- Prelevare, dal codice di condivisione, il link del video di Vimeo
  (valore dell' attributo src dell' iframe) e inserirlo come valore del
  parametro **Link** nella maschera di configurazione del componente
  Passweb

![](./assets/media/image168.png)

I successivi parametri consentono di attivare o meno determinate
funzionalità sul player del video e possono variare in relazione alla
specifica piattaforma di pubblicazione adottata

- **Autoplay (Youtube e Vimeo):** consente, se selezionato, di avviare
  automaticamente il video al caricamento della pagina

- **Autopause (Vimeo):** consente, se selezionato, di bloccare
  automaticamente la riproduzione del video in esame nel momento in cui
  dovesse essere avviata, all'interno della stessa pagina, la
  riproduzione di un altro video

- **Controlli (Youtube):** consente di abilitare o meno all'interno del
  player la barra dei controlli. E' possibile selezionare uno dei
  seguenti valori:

  - Non visualizzare

  - Visualizza al play del video

  - Visualizza quando il video comincia la riproduzione

- **Disabilita tastiera (Youtube):** consente, se selezionato, di
  disabilitare i controlli da tastiera

- **Visualizza full screen (Youtube):** consente, se selezionato, di
  abilitare il pulsante per la visualizzazione a schermo intero

- **Loop (Youtube e Vimeo):** consente, se selezionato di fari ripartire
  automaticamente il video una volta terminato

- **Mostra video correlati (Youtube):** consente, se selezionato, di
  mostrare i video correlati al termine della riproduzione del video in
  esame

- **Mostra informazioni del Video (Youtube):** consente, se selezionato,
  di attivare il pulsante per la visualizzazione delle informazioni
  aggiuntive relative al video in esame

- **Attributi aggiuntivi:** consente di indicare eventuali attributi da
  aggiungere all' url del video che possono attivare o meno determinate
  funzionalità del player (utile soprattutto nel momento in cui il video
  dovesse essere pubblicato su piattaforme diverse da Youtube o Vimeo)

Il pulsante '**Salva**' presente nella parte alta della maschera
consentirà di salvare tutte le modifiche apportate al componente in
oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

