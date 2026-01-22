# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico la sua maschera di gestione e configurazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componenti-googlemap_res.bmp](./assets/media/image37.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente stesso.

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

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente al parametro
> **Statico** si veda anche quanto indicato all'interno del capitolo
> "*Configurazione Componenti -- Caratteristiche generali* --
> *Staticizzazione e caricamento asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

All'interno della sotto sezione "**Parametri Google Map**" è possibile
gestire alcune opzioni di visualizzazione della mappa. Nello specifico
il parametro :

- **Zoom mappa:** consente di impostare il livello di ingrandimento
  sulla mappa. I valori consigliati sono da 10 a 15.

- **Tipo di Mappa:** consente di selezionare il tipo di mappa che dovrà
  essere utilizzato all'interno del componente. E' possibile selezionare
  uno dei seguenti valori:

  - **Stradale**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_stradale.bmp](./assets/media/image38.png)

- **Satellitare**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_satellitare.bmp](./assets/media/image39.png)

- **Terrestre**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_terrestre.bmp](./assets/media/image40.png)

- **Ibrida**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_ibrida.bmp](./assets/media/image41.png)

- **Punti di interesse:** consente di decidere quali punti di interesse
  (Attrazioni Turistiche, Commercianti, Edifici Governativi ecc...)
  dovranno o meno essere visualizzati all'interno della Google Map oltre
  ai marker appositamente impostati.

> **ATTENZIONE!** I punti di interesse verranno visualizzati solo nel
> caso in cui per la mappa sia stato selezionato il tema Standard

- **Tema:** consente di impostare, selezionandolo dall'apposito menu a
  tendina, uno specifico tema grafico da applicare alla Google Map

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_tema_grafico.bmp](./assets/media/image42.png)

All'interno della sotto sezione **"Gestione dei punti vendita"** è
possibile decidere di abilitare o meno, all'interno della corrispondente
Google Map, i soli punti vendita appositamente codificati mediante le
relative funzioni messe a disposizione da Passweb.

- **Visualizza solo i Punti Vendita:** consente di caricare
  automaticamente all'interno della Google Map i marker relativi a tutti
  i Punti Vendita attualmente codificati e gestiti all'interno del sito
  (per maggiori informazioni relativamente alla creazione e alla
  gestione dei Punti Vendita si veda anche la sezione *"Ordini --
  Configurazione Punti Vendita"* di questo manuale)

> **ATTENZIONE! Selezionando questa opzione i marker presenti
> all'interno della Google Map sono inseriti e gestiti automaticamente
> da Passweb. Non sarà quindi possibile inserire manualmente altri
> Marker e, in conseguenza di ciò, scomparirà anche, nella maschera di
> configurazione del componente, il tab "Gestione Markers"**
>
> In queste condizioni inoltre i marker presenti nella google map
> avranno l'icona standard e il contenuto del fumetto coinciderà
> esattamente con quanto impostato per la descrizione del relativo Punto
> Vendita

La sotto sezione **Parametri di Ricerca** permette infine di decidere se
abilitare o meno, ed eventualmente come configurarla, la funzionalità
della Google Map relativa al calcolo del percorso più breve tra un
indirizzo indicato dall'utente ed il marker presente sulla mappa ad esso
più vicino.

In particolare dunque il parametro:

- **Abilita Ricerca:** consente di abilitare all'interno della Google
  Map un campo di ricerca all'interno del quale l'utente potrà inserire,
  in maniera guidata, un indirizzo personalizzato. Il pulsante Ricerca
  posto accanto a questo campo consentirà poi all'utente di calcolare ed
  eventualmente visualizzare all'interno della Google Map il percorso
  più breve tra l'indirizzo da lui selezionato ed il Marker ad esso più
  vicino

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_ricerca_percorso.bmp](./assets/media/image43.png)

- **Visualizza il percorso più breve:** consente di visualizzare, se
  selezionato, una linea all'interno della Google Map che individua
  graficamente il percorso più breve tra l'indirizzo, indicato
  dall'utente all'interno dell'apposito pannello di ricerca, ed il
  marker, presente nella Google Map, ad esso più vicino

- **Visualizza il percorso testuale più breve:** consente di
  visualizzare, se selezionato, una descrizione testuale del percorso
  più breve tra l'indirizzo, indicato dall'utente all'interno
  dell'apposito pannello di ricerca, ed il marker, presente nella Google
  Map, ad esso più vicino

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_ricerca_percorso_testuale.bmp](./assets/media/image44.png)

- **Visualizza i marker più vicini:** se selezionato, consente di
  visualizzare tra i risultati la descrizione del Marker più vicino
  all'indirizzo impostato dall'utente all'interno dell'apposito campo di
  ricerca.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_ricerca_percorso_luoghi_vicini.bmp](./assets/media/image45.png)

Una volta settati i parametri di configurazione della Google Map sarà
poi necessario impostare i vari marker che dovranno essere visualizzati
all'interno della mappa agendo, in questo senso, dalla sezione "Gestione
Markers" presente nella maschera di configurazione di questa specifica
tipologia di componenti.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

