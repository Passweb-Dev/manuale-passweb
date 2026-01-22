# GESTIONE MARKERS



La sezione **Gestione Markers** (visibile solo ed esclusivamente nel
caso in cui non sia stato selezionato il parametro "Visualizza solo i
punti vendita"), consente di definire e configurare in maniera manuale i
vari Marker che dovranno poi essere posizionati sulla mappa.

All'interno di questa sezione, sulla sinistra, verrà visualizzato
l'elenco dei vari Marker e dei relativi indirizzi attualmente codificati
e inseriti nella mappa; sulla destra verranno invece visualizzate le
caratteristiche e le proprietà del Marker attualmente selezionato in
elenco.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_marker_RES.bmp](./assets/media/image46.png){width="5.16875in"
height="3.123611111111111in"}

Per modificare uno di questi Marker sarà quindi sufficiente selezionarlo
e andare poi ad agire sui vari parametri presenti all'interno della
sezione "**Modifica Marker**".

Per eliminare uno dei Marker presenti in elenco sarà invece sufficiente
selezionarlo e cliccare sul relativo pulsante di eliminazione
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image16.png){width="0.18819444444444444in"
height="0.1951388888888889in"}).

Per aggiungere un nuovo Marker alla mappa sarà invece necessario
cliccare sul pulsante di aggiunta nuovo marker (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png){width="0.18819444444444444in"
height="0.18819444444444444in"} ). In questo modo verrà infatti
visualizzato, nella parte destra della sezione "Gestione Marker", il
form "**Nuovo Marker**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_map_nuovo_marker_res.bmp](./assets/media/image48.png){width="5.155555555555556in"
height="3.1104166666666666in"}

mediante il quale poter definire le caratteristiche e le proprietà del
Marker che si intende aggiungere sulla mappa. In particolare sarà
possibile specificare un valore per i seguenti campi:

- **Riferimento:** consente di specificare il tipo di dato che dovrà
  essere inserito nel successivo campo e necessario per identificare la
  posizione sulla cartina in cui collocare il marker in oggetto. E'
  possibile selezionare uno dei seguenti valori:

  - **Indirizzo:** in questo caso nel successivo campo "**Indirizzo**"
    sarà necessario specificare l'esatto indirizzo in corrispondenza del
    quale dovrà essere posizionato il Marker che si sta codificando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gmap_indirizzo_res.bmp](./assets/media/image49.png){width="5.155555555555556in"
height="3.1104166666666666in"}

- **Coordinate:** in questo caso nel successivo campo "**Coordinate**"
  sarà necessario indicare le esatte coordinate (Latitudine,
  Longitudine) in corrispondenza delle quali dovrà essere posizionato il
  Marker che si sta codificando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gmap_coordinate_res.bmp](./assets/media/image50.png){width="5.155555555555556in"
height="3.1104166666666666in"}

> **ATTENZIONE!** L'utilizzo delle coordinate geografiche oltre a
> rendere più preciso il posizionamento del marker sulla mappa potrebbe
> anche velocizzare il suo caricamento all'interno della pagina web.
>
> Per individuare le esatte coordinate geografiche (Latitudine e
> Longitudine) del punto in cui andrebbe posizionato il marker è
> sufficiente:

- inserire l'indirizzo desiderato direttamente all'interno di Google
  Maps (https://www.google.it/maps)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_pv_1.bmp](./assets/media/image51.png){width="3.798611111111111in"
height="2.3118055555555554in"}

- cliccare con il tasto destro del mouse sul marker posizionato da
  google all'interno della mappa e selezionare l'opzione "**Che cosa c'è
  qui?**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_pv_2.bmp](./assets/media/image52.png){width="3.798611111111111in"
height="2.3118055555555554in"}

- le coordinate in esame potranno quindi essere prelevate direttamente
  dal piccolo fumetto visualizzato ora nella parte bassa della google
  map

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gmap_pv_3.bmp](./assets/media/image53.png){width="3.798611111111111in"
height="2.3118055555555554in"}

> **NOTA BENE:** il posizionamento finale del Marker all'interno della
> mappa sulla base dell'indirizzo e/o delle coordinate impostate dipende
> da Google. Passweb, in questo senso, non ha quindi alcuna
> responsabilità.

- **Punto Vendita:** in questo caso sarà poi possibile selezionare dal
  sottostante menu a tendina (campo **Punto di Vendita**) uno qualsiasi
  dei Punti Vendita precedentemente codificati e **abilitati**
  all'interno della sezione "*Ordini -- Configurazione Punti Vendita*"
  del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gmap_selezione_pv_res.bmp](./assets/media/image54.png){width="5.1625in"
height="3.1166666666666667in"}

> **ATTENZIONE!** i Punti Vendita correttamente esportati all'interno
> del sito ma non ancora abilitati non potranno essere inseriti nella
> Google Map

- **Testo Marker:** consente di specificare il testo che verrà
  visualizzato nel fumetto del Marker. E' possibile utilizzare il
  corrispondente editor HTML per formattare e personalizzare il testo
  che dovrà essere inserito all'interno del fumetto oltre che per
  inserire nel fumetto stesso anche eventuali immagini.

> Per maggiori informazioni relativamente all'utilizzo di questo editor
> HTML si veda anche il relativo capitolo *("Live Editing per Varianti
> Responsive -- Contenuti -- Editor dei contenuti"*) di questo manuale.
>
> **ATTENZIONE!** Nel caso in cui il Marker inserito nella Google Map
> sia quello relativo ad uno dei punti vendita gestiti all'interno del
> sito, quanto inserito all'interno del campo in esame avrà priorità
> maggiore, e verrà quindi visualizzato all'interno del relativo
> fumetto, rispetto a quanto indicato nella descrizione del punto
> vendita stesso

- **Immagine:** consente di specificare un' immagine, selezionandola tra
  quelle presenti in "Gestione Risorse", da associare al Marker che si
  sta codificando. Nel caso in cui non venga specificata nessuna
  immagine il Marker utilizzerà l'immagine di default ( ).

> E' possibile indicare una delle immagini presenti nel database del
> sito oppure uno degli Attributi Immagine gestiti.

- **Marker Aperto:** consente di specificare se il fumetto associato al
  Marker che si sta realizzando dovrà essere, all'apertura della pagina
  in cui è stato inserito il componente Google Map, aperto oppure
  chiuso.

Il pulsante "**Aggiungi Elemento**" presente nella parte alta della
maschera consentirà di aggiungere il Marker appena codificato all'elenco
dei Marker presenti sulla mappa.

Il pulsante '**Salva**' consentirà invece di salvare tutte le modifiche
apportate al componente in oggetto.

**NOTA BENE**: la Google map vera e propria verrà visualizzata
unicamente all'interno del sito web. Sul Wizard, come mostrato, verrà
visualizzato solo segnaposto per indicare l'avvenuto inserimento del
componente all'interno della pagina.

