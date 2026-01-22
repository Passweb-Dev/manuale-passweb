# GESTIONE MARKERS



Per aggiungere nuovi Markers alla mappa è possibile operare in due modi
diversi:

- In maniera manuale operando direttamente dalla maschera di
  configurazione del componente e andando quindi a configurare uno a uno
  i vari Marker che si desidera aggiungere

- In maniera massiva mediante l'import di un file csv appositamente
  strutturato

Nel primo caso (inserimento manuale) per aggiungere un nuovo Marker sarà
sufficiente cliccare sul relativo pulsante di aggiunta ( ). presente
all'interno della sezione "**Gestione Markers**".

In questo modo verrà infatti visualizzato, nella parte destra della
maschera, il form "**Nuovo Marker**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\store_locator_marker_categorie_1.bmp](./assets/media/image65.png)

mediante il quale poter definire le caratteristiche e le proprietà
dell'elemento che si intende aggiungere sulla mappa. Sarà quindi
possibile specificare un valore per i seguenti campi:

**Riferimento:** consente di specificare il tipo di informazioni che
dovranno poi essere fornite per identificare la posizione sulla mappa in
corrispondenza della quale andare a posizionare il relativo marker.

E' possibile selezionare uno dei seguenti valori:

- **Coordinate:** in questo caso nel successivo campo "**Coordinate**"
  sarà necessario indicare le esatte coordinate (Latitudine,
  Longitudine) in corrispondenza delle quali dovrà essere posizionato il
  Marker che si sta codificando.

> **ATTENZIONE!** L'utilizzo delle coordinate geografiche oltre a
> rendere più preciso il posizionamento del marker sulla mappa potrebbe
> anche velocizzare il suo caricamento all'interno della pagina web.
>
> Come evidenziato nei precedenti capitoli di questo manuale infatti,
> nel caso in cui il numero di marker gestiti dovesse essere
> particolarmente elevato e questi siano stati posizionati sulla mappa
> utilizzando il loro indirizzo, potrebbero verificarsi degli errori di
> "OVER_QUERY_LIMIT" dovuti al numero eccessivo di chiamate fatte a
> Google per geolocalizzare l\'indirizzo, numero questo da mettere
> sempre in relazione alle chiamate effettivamente disponibili secondo i
> parametri di configurazione del proprio account.
>
> Per evitare questo tipo di problemi, in ogni caso, Passweb distribuirà
> automaticamente le chiamate su di un intervallo di tempo più elevato
> cosa questa che se da una parte può evitare i problemi di
> "OVER_QUERY_LIMIT", dall'altra parte potrebbe ovviamente provocare un
> rallentamento nel caricamento dei markers.
>
> **Per questo motivo in caso di rallentamento evidente a causa del
> numero eccessivo di marker da gestire, è fortemente consigliato di
> posizionare i markers sulla mappa utilizzando direttamente le
> coordinate (latitudine e longitudine) in modo tale da evitare chiamate
> a Google per geolocalizzare automaticamente i vari indirizzi**.
>
> Per maggiori informazioni relativamente a come poter individuare le
> esatte coordinate geografiche (Latitudine e Longitudine) del punto in
> cui andrebbe posizionato il marker si veda anche quanto indicato in
> merito alla configurazione del componente Google Map

- **Indirizzo:** in questo caso nel successivo campo "**Indirizzo**"
  sarà necessario specificare l'esatto indirizzo in corrispondenza del
  quale dovrà essere posizionato il Marker che si sta codificando.

> **ATTENZIONE!** il posizionamento di un marker sulla mappa mediante la
> definizione del suo indirizzo, richiede una chiamata alle API di
> Google per geolocalizzare l'indirizzo trasformandolo nelle coordinate
> corrette. Solo al termine di questa operazione il marker potrà essere
> effettivamente posizionato sulla mappa.

- **Punto Vendita:** in questo caso sarà poi possibile selezionare dal
  sottostante menu a tendina (campo **Punto di Vendita**) uno qualsiasi
  dei Punti Vendita codificati e **abilitati** all'interno della sezione
  "*Ordini -- Configurazione Punti Vendita*" del Wizard

**Marker Aperto:** consente di specificare se il fumetto associato al
Marker che si sta realizzando dovrà essere, all'apertura della pagina in
cui è stato inserito il componente Google Map, aperto oppure chiuso.

**Immagine marker mappa:** consente di specificare un' immagine da
associare al Marker che si sta codificando. Nel caso in cui non venga
specificata nessuna immagine il Marker utilizzerà l'immagine di default.

E' possibile indicare una delle immagini presenti nel database del sito
oppure uno degli Attributi Immagine attualmente gestiti.

All'interno della sezione "**Bottone e info text Marker**" è invece
possibile specificare alcune informazioni descrittive del marker che si
sta codificando, informazioni queste che verranno poi visualizzate nel
fumetto collegato al marker presente sulla mappa e nell'elenco presente
all'interno della colonna "Lista Comandi".

Sarà possibile indicare un valore per i seguenti campi

- **Nome:** titolo del marker (può essere ad esempio il nome dello
  specifico punto vendita)

- **Descrizione:** breve descrizione visualizzata immediatamente al di
  sotto del titolo del marker

- **Descrizione Indirizzo:** ulteriore descrizione utilizzabile per
  fornire maggiori informazioni riguardo l'ubicazione del marker.

- **Immagine marker bottone e info text:** consente di associare al
  marker in esame una specifica immagine che verrà poi visualizzati in
  corrispondenza del marker stesso sia all'interno del relativo fumetto
  che nell'elenco testuale dei vari marker presenti sulla mappa

**Pagina di destinazione:** visualizzato solo nel caso in cui il
parametro "Riferimento" sia impostato su "Indirizzo" oppure su
"Coordinate". Consente di collegare il marker in esame ad una specifica
pagina del sito utilizzabile, ad esempio, come "pagina di dettaglio" per
il relativo punto vendita.

Il link di collegamento alla pagina, il cui testo è personalizzabile
all'interno della sezione "Gestione Testi / Messaggi del sito", verrà
mostrato immediatamente al di sotto della "Descrizione Indirizzo"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\store_locator_marker_categorie_7.bmp](./assets/media/image66.png)

**ATTENZIONE!** Nel caso in cui il marker sulla mappa sia uno dei Punti
Vendita codificati all'interno della relativa sezione del Wizard il link
all'eventuale pagina di dettaglio verrà settato sulla base di quanto
inserito all'interno del campo "**Pagina Negozio per sito**" presente
nella maschera di configurazione del punto vendita stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\store_locator_marker_categorie_6.bmp](./assets/media/image67.png)

Per maggiori informazioni relativamente alla codifica e alla gestione
dei punti vendita si veda anche quanto indicato all'interno del relativo
capitolo di questo manuale ("*Ordini -- Punti Vendita*")

Infine, sempre all'interno del fumetto visualizzato in corrispondenza
dei marker posizionati sulla mappa, è presente anche il pulsante
"**Indicazioni Stradali**" (il cui testo è modificabile come al solito
all'interno della sezione "Testi/Messaggi del Sito") che consente di
simulare il click sul pulsante "Indicazioni" localizzato all'interno
della "Lista Comandi" avviando di fatto il calcolo del percorso da
seguire per andare dall'indirizzo indicato al marker corrispondente.

Il pulsante "**Aggiungi Elemento**" presente nella parte alta della
maschera consentirà di aggiungere il Marker appena codificato all'elenco
dei Marker presenti sulla mappa.

Nel caso in cui l'esigenza dovesse essere invece quella di importare
massivamente un numero elevato di Marker sarà sufficiente attivare la
relativa funzione cliccando sul pulsante "**Importa Marker**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_importa.bmp](./assets/media/image68.png)) presente, anch'esso nella barra
strumenti della sezione "**Gestione Markers**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\markers_importa_valori.bmp](./assets/media/image69.png)

In questo modo verrà infatti visualizzato, nella parte destra della
maschera, il form "**Importa Valori**" all'interno della quale poter
selezionare il file da importare.

Nello specifico, infatti , il campo:

- **File (csv-txt):** consente di selezionare il file txt o csv da
  uplodare e contenente l'elenco dei marker da posizionare sulla mappa

- **Lingua di riferimento**: consente di indicare la lingua del sito a
  cui dovranno fare riferimento i dati presenti all'interno del file di
  importazione. Nel caso di siti multilingua sarà necessario creare e
  uplodare file diversi per ciascuna delle lingue gestite

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

- **Elimina valori non presenti nel file**: consente di decidere se in
  fase di importazione dovranno o meno essere eliminati eventuali marker
  già inseriti sul componente ma non presenti nel file di importazione

**ATTENZIONE!** per fare in modo che la procedura di importazione
termini correttamente il file di importazione dovrà essere strutturto
come di seguito indicato:

La prima riga del file deve contenere, necessariamente, tutte le
intestazioni di colonna come di seguito indicato

*type;location;addressDesc;open;imageMap;buttonText;buttonDesc;buttonImage;page*

Gli ulteriori record del file dovranno invece avere in corrispondenza di
ciascuna colonna il relativo valore di configurazione del marker che si
intende inserire. Nello specifico in corrispondenza della colonna:

- **type -- campo obbligatorio -** andrà inserita la tipologia del
  marker che si intende inserire indicando:

  - **0** se il marker verrà gestito tramite Indirizzo

  - **1** se il marker verrà gestito tramite Coordinate (latitudine
    ,longitudine)

  - **2** se il marker verrà gestito tramite Punto vendita

- **Location -- campo obbligatorio --** andranno inseriti i valori di
  localizzazione del marker che si intende inserire. Ovviamente tali
  valori varieranno in base alla tipologia di marker che si è deciso di
  gestire e quindi in base al valore che si è indicato in corrispondenza
  della precedente colonna "type".

> In particolare se nella colonna type è stato indicato il valore:

- 0 🡪 nella colonna Location sarà necessario indicare **l'indirizzo
  completo** del marker (es. Via Flaminia 29, 47922 Rimini)

- 1 🡪 nella colonna Location sarà necessario indicare **le esatte
  coordinate** del marker (es. 49.32154767, 48.324657)

- 2 🡪 nella colonna Location sarà necessario indicare **l'id** punto
  vendita che rappresenta il marker da inserire. Tale identificativo può
  essere visualizzato sul Wizard all'interno della maschera "**Lista dei
  Punti Vendita**")

<!-- -->

- **addressDesc -- opzionale --** andrà inserita la descrizione
  dell'indirizzo

- **open** -- **opzionale --** andrà inserita l'indicazione necessaria
  per definire se il relativo Marker dovrà essere o meno aperto secondo
  questo schema:

  - **0** indica marker **chiuso**

  - **1** indica marker **aperto**

- **imageMap** -- **opzionale --** andrà indicato il path relativo o
  l'attributo tema dell\'immagine del marker sulla mappa.

- **buttonText** **-- opzionale --** andrà indicato il testo del bottone

- **buttonDesc -- opzionale --** andrà indicata la descrizione del
  bottone

- **buttonImage** -- **opzionale --** andrà il path relativo il path
  relativo o l'attributo tema dell\'immagine del bottone

- **page** -- **opzionale --** andrà indicato l' eventuale link all' id
  di pagina.

Il pulsante "**Esporta Marker**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_esporta.bmp](./assets/media/image70.png)) presente, anch'esso nella barra
strumenti della sezione "**Gestione Markers**" consente, invece, di
esportare i marker attualmente presenti in elenco all'interno di un file
.csv.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\markers_esporta_valori.bmp](./assets/media/image71.png)

Cliccando su questo pulsante verrà infatti visualizzato, nella parte
destra della maschera, il form "**Esporta Valori**" all'interno della
quale poter configurare il file che dovrà poi essere esportato.

Nello specifico, infatti , il campo:

- **Lingua di riferimento**: consente di indicare la lingua del sito a
  cui dovranno fare riferimento i dati presenti all'interno del file da
  esportare. Nel caso di siti multilingua sarà necessario effettuare
  esportazioni diverse per ciascuna delle lingue gestite

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere da utilizzare all'interno del file di
  esportazione come separatore per i vari campi

In questo senso, se si dovessero avere problemi nella creazione del file
csv da utilizzare per l'import massivo dei marker, si consiglia di
codificare manualmente almeno un paio di marker e successivamente
esportarli mediante l'apposita funzione in maniera tale da avere un
esempio chiaro di come procedere nella realizzazione del file csv di
import.

**ATTENZIONE!** l'import massivo dei marker mediante file csv non
gestisce l'associazione con le varie categorie. Tale operazione dovrà
quindi essere eseguita in maniera manuale secondo quanto indicato
all'interno del successivo capitolo di questo manuale.

Gli ulteriori pulsanti presenti all'interno della barra strumenti della
sezione "Gestione Markers" consentono infine di:

**Elimina**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image16.png)): consente di eliminare dalla mappa il
marker attualmente selezionato in elenco

**Copia Marker**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_copia.bmp](./assets/media/image72.png)): consente di creare un nuovo Marker
effettuando una copia di quello attualmente selezionato in elenco.

**Modifica Marker**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_modifica.bmp](./assets/media/image73.png)): consente di accedere in modifica al
form di configurazione del marker attualmente selezionato in elenco.

**Converti**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_converti.bmp](./assets/media/image74.png)): consente di convertire in blocco tutti
gli indirizzi dei marker attualmente presenti in elenco nelle relative
coordinate geografiche (latitudine e longitudine) in maniera tale
ottimizzare i tempi di caricamento della mappa all'interno della pagina
web.

