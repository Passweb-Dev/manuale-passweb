# GESTIONE CONTENUTI



La sezione "**Gestione Contenuti**", presente nella maschera di
configurazione del componente "Ordine Custom (Checkout)", consente di
definire e gestire i contenuti del componente in oggetto permettendoci
di stabilire esattamente il numero di colonne in cui dovrà essere
suddivisa ogni singola riga articolo.

![](./assets/media/image290.png)

In particolare dunque nella parte sinistra di questa sezione è
visualizzato l'elenco delle colonne attualmente gestite per ogni singola
riga articolo.

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Aggiungi colonna** (
  ![](./assets/media/image14.png) ): consente di aggiungere una nuova
  colonna.

- **Elimina scheda** (
  ![](./assets/media/image165.png) ): consente di eliminare la colonna
  attualmente selezionata in elenco.

- **Sposta su / giù**
  (![](./assets/media/image166.png) ): consente di riordinare tra loro le
  varie colonne presenti all'interno del componente spostando verso
  l'alto o il basso la colonna attualmente selezionata in elenco.

Nella parte destra della sezione "**Gestione Contenuti**" è invece
possibile definire le proprietà e le caratteristiche della colonna
attualmente selezionata. In particolare è possibile impostare un valore
per i seguenti campi:

**Titolo:** consente di impostare l'etichetta identificativa della
specifica colonna.

**Funzionamento:** consente di definire il modo in cui potranno essere
organizzati e gestiti i contenuti all'interno della specifica colonna.

In questo senso è possibile selezionare uno dei seguenti valori:

![](./assets/media/image291.png)

- **Contenuto:** impostando il parametro "Funzionamento" su questo
  valore sarà poi necessario inserire il contenuto della relativa
  colonna agendo **direttamente da questa stessa maschera** e
  utilizzando per questo il corrispondente editor HTML

> Per maggiori informazioni relativamente all'utilizzo di questo editor
> HTML si veda anche il relativo capitolo *("Live Editing per Varianti
> Responsive -- Contenuti -- Editor dei contenuti"*) di questo manuale.
>
> In queste condizioni inoltre il campo **"Eventuale Immagine"**
> consente di selezionare un'immagine da associare al testo inserito
> all'interno del precedente campo. Cliccando infatti sul pulsante
> **"Seleziona Risorsa"** si verrà ricondotti alla maschera di "Gestione
> Risorse" attraverso cui poter selezionare dall'elenco (o caricarla
> ex-novo dal proprio computer) l'immagine desiderata. La piccola x
> eventualmente posta a fianco del pulsante "Seleziona Risorsa"
> consentirà di azzerare il campo eliminando quindi l'associazione con
> la risorsa precedentemente selezionata.
>
> Una volta impostati i contenuti desiderati, il pulsante **"Aggiungi
> Elemento",** nella parte bassa della maschera, consentirà di
> aggiungere la colonna appena editata al Componente che si sta
> realizzando.
>
> **ATTENZIONE! In queste condizioni i valori inseriti all'interno dei
> campi "Contenuto" e "Immagine" verranno replicati e saranno quindi
> sempre gli stessi per ogni singola riga articolo presente in ordine**

- **Contenitore:** impostando il parametro "Funzionamento" su questo
  valore la colonna che si sta realizzando verrà considerata come un
  vero e proprio contenitore di componenti.

> **In questo caso sarà quindi possibile inserire all'interno della
> colonna non solo del semplice testo accompagnato eventualmente da
> un'immagine ma anche dei veri e propri componenti di tipo Ecommerce,
> permettendoci dunque di contestualizzare le informazioni visualizzate
> all'interno di ogni singola riga articolo presente in ordine.**
>
> **L'inserimento di questi componenti non potrà però avvenire
> direttamente da questa maschera di configurazione, come nel caso
> precedente, ma, trattandosi di veri e propri componenti Passweb, dovrà
> necessariamente avvenire in modalità "Live Editing" utilizzando le
> solite tecniche di Drag and Drop**.
>
> In sostanza dunque, nelle condizioni indicate, il componente "Ordine
> Custom" diventerà a tutti gli effetti un vero e proprio **Componente
> di tipo Contenitore** e andrà quindi trattato e gestito come tale.
>
> Per poter inserire dei contenuti all'interno delle colonne gestite in
> questo modo, sarà quindi necessario attivare la modalità di gestione
> dei componenti, portarsi col mouse sul componente Ordine Custom e,
> alla comparsa del R.O.C., cliccare sull'icona '**Accedi ai componenti
> interni**'.
>
> Nello specifico sarà possibile inserire all'interno del Ordine Custom
> due diverse tipologie di componenti:

- **Componenti Comuni:** si tratta di semplici componenti di tipo
  Paragrafo, Immagine, HTML o Contenitore il cui contenuto non potrà
  ovviamente essere contestualizzato in base alla specifica riga
  articolo e verrà quindi replicato in maniera identica per ogni singolo
  articolo presente in carrello

- **Componenti Ecommerce:** si tratta di veri e propri componenti
  Ecommerce mappati con i corrispondenti campi del gestionale (es.
  descrizione articolo, immagine articolo, prezzo, attributi articolo
  ecc...) ed in grado dunque di contestualizzare le relative
  informazioni in base allo specifico articolo presente in carrello.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> dei Componenti di tipo Contenitore si veda anche il corrispondente
> capitolo di questo manuale ("Live Editing per Varianti Responsive --
> Componenti -- Componenti di tipo Contenitore")
>
> Infine, nelle condizioni sopra indicate, sarà anche possibile
> assegnare ad ogni singola colonna una specifica immagine di sfondo
> agendo in questo senso dal relativo parametro **"Immagine di Sfondo
> Sezione"**

![](./assets/media/image168.png)

> **ATTENZIONE!** Aggiungendo o eliminando un componente dal dettaglio
> del documento questo verrà automaticamente aggiunto o eliminato anche
> dal riepilogo eventualmente visualizzato nella fase iniziale del
> checkout. Allo stesso modo aggiungendo o eliminando componenti dal
> riepilogo questi verranno automaticamente aggiunti o eliminati anche
> dal dettaglio del documento (per maggiori informazioni in merito si
> veda quanto indicato nel precedente capitolo di questo manuale)

**Visibile da:** consente di impostare la visibilità **dell'intera
colonna** in oggetto a livello di gruppi utente, potendo quindi decidere
quali utenti potranno o meno visualizzarla (volendo sarà poi possibile
dettagliare maggiormente questo tipo di informazione agendo sui permessi
di visibilità dei singoli componenti presenti all'interno della
colonna).

Impostando questo parametro sul valore **"Tutti"** l'intera colonna sarà
quindi visibile a tutti i visitatori del sito.

Impostando invece il parametro sul valore **"Solo i gruppi
Specificati"** verranno visualizzati tutti i gruppi utente appositamente
creati all'interno della corrispondente sezione "*Utenti -- Gruppi
Utenti Sito*" del Wizard. **In queste condizioni la colonna in oggetto
potrà quindi essere visibile ai soli utenti appartenenti ai gruppi
selezionati**.

Per maggiori informazioni relativamente alla creazione dei Gruppi Utente
si veda la corrispondente sezione "Utenti -- Gruppi Utenti Sito" di
questo manuale.

**Larghezza Colonna:** consente di impostare la larghezza della colonna
in esame definendo, come al solito, quante delle 12 sezioni in cui
risulta essere suddivisa la riga articolo dovranno essere occupate da
questa stessa colonna

