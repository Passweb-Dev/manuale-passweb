# PAGINE



Il tab "**Pagine**" visibile solo dopo aver configurato e salvato i
parametri presenti all'interno del tab "Configurazione", consente di
configurare e gestire la generazione del feed utilizzato per condividere
con Clerk informazioni relative ai post CMS e ai testi pubblicati nelle
varie pagine del proprio sito.

![](./assets/media/image20.png)

In questo senso dunque il parametro:

**Genera Feed alla Sincronizzazione**: consente, se selezionato, di
generare automaticamente il feed ad ogni sincronizzazione sito --
gestionale (Standard o Totale).

**URL Feed**: consente di visualizzare l'url di pubblicazione del feed,
quello che dovrà poi essere inserito all'interno del campo "JSON Pages
URL" alla pagina "**Data -- Configuration**" dello store Clerk con cui
si desidera effettuare l'integrazione (per maggiori informazioni in
merito si veda anche quanto indicato all'interno del precedente capitolo
"*Sincronizzazione Dati*")

Il pulsante "**Genera Feed**" presente nella parte bassa della maschera
consente invece di avviare manualmente la generazione del relativo feed.

Considerando che questa tipologia di feed serve, essenzialmente, a
gestire i diversi contenuti testuali che posson essere inseriti nelle
varie pagine del sito, al suo interno potremo trovare due diverse
tipologie di elementi:

- testi pubblicati in una qualsiasi pagina mediante il componente
  "**Paragrafo**" e marcati in maniera specifica (campo "**Considera nel
  feed pagine**") per essere inseriti all'interno di questo feed

![](./assets/media/image21.png)

> Per maggiori informazioni sul componente "Paragrafo" si veda anche
> quanto indicato nel relativo capitolo di questo manuale ("*Componenti
> Comuni -- Componente Paragrafo -- Configurazione*")

- post CMS pubblicati all'interno del sito

> **ATTENZIONE!** Eventuali post creati all'interno del Wizard ma non
> ancora pubblicati sul sito non verranno presi in considerazione in
> fase di generazione del feed

Nello specifico poi per ogni singolo elemento (pagina / post cms)
presente all'interno del feed verranno gestite le seguenti informazioni:

- id Pagina / codice post CMS

- type: tipologia di contenuto. Impostato su:

  - page per i testi pubblicati in una determinata pagina mediante
    componente Paragrafo e marcati per essere inseriti anche in questo
    feed

  - blog per i post CMS pubblicati all'interno del sito

- title: titolo della pagina / titolo del post CMS

- text: valorizzato per i testi generici con il "Contenuto" del relativo
  componente paragrafo, per i post CMS con quanto inserito all'interno
  del campo "Articolo" (in sostanza il dettaglio testuale del post)

- categories_cms: nome delle categorie associate al post CMS

**ATTENZIONE!** **il feed delle pagine conterrà ovviamente sempre e
comunque tutti i testi marcati per essere inseriti in questo stesso feed
e tutti i post cms effettivamente pubblicati all'interno del sito**

Nel caso dei siti multilingua i campi presenti all'interno del feed (es.
"text") verranno valorizzati nella lingua impostata in fase di
configurazione del relativo account Clerk

