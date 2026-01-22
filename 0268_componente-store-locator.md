# COMPONENTE STORE LOCATOR



Il Componente Store Locator

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_store_locator.bmp](./assets/media/image55.png)

consente di inserire all'interno della pagina web un modulo suddiviso in
due distinte sezioni: da una parte una Google Map su cui poter
posizionare e localizzare N distinti elementi (es. i propri Punti
Vendita), dall'altra parte un elenco di questi stessi elementi,
dettagliato per Nome, Indirizzo, Descrizione ... , e un insieme di
controlli necessari per filtrare ed interagire con i rispettivi elementi
presenti sulla Mappa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\store_locator_1.bmp](./assets/media/image56.png)

**ATTENZIONE! Come già indicato per il componente Google Map, dal 16
Luglio 2018 è entrato in vigore un nuovo piano tariffario basato sul
consumo per Maps, Routes e Places.**

L'effettiva possibilità di utilizzare le Mappe Google all'interno del
proprio sito è quindi sottoposta al fatto di aver ottemperato a tutte le
richieste effettuate da Google stessa in merito alla fruizione di questo
tipo di servizio. Per maggiori informazioni in merito si veda anche la
sezione "*Sito -- Preferenze -- SEO Integrazioni -- Google Maps Api*" di
questo manuale.

Il componente ha attivi di default i servizi di geolocalizzazione per
cui, effettuando per la prima volta l'accesso alla pagina del sito
contenente lo Store Locator, il browser si preoccuperà di richiedere
all'utente l'autorizzazione ad utilizzare tali servizi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\store_locator_geolocalizzazione.bmp](./assets/media/image57.png)

Nel momento in cui l'utente dovesse acconsentire ad utilizzare questo
tipo di servizio, il campo indirizzo verrà automaticamente compilato con
l'indirizzo attuale dell'utente, indirizzo questo rilevato
automaticamente dal browser.

I singoli marker presenti sulla mappa, possono essere posizionati in tre
modi diversi:

- Indicando **l'indirizzo** in corrispondenza del quale dovrà essere
  posizionato il marker

- Indicando **le coordinate esatte** (latitudine e longitudine) del
  punto in cui dovrà essere posizionato il marker

- Sulla base dell' **indirizzo associato ad uno dei Punti Vendita
  gestiti all'interno del sito** e visualizzati all'interno della
  maschera "Lista dei Punti Vendita" del Wizard (menu "*Ordini -- Punti
  Vendita*")

**ATTENZIONE!** nel caso in cui il numero di marker gestiti dovesse
essere particolarmente elevato e questi siano stati posizionati sulla
mappa utilizzando il loro indirizzo, potrebbero verificarsi degli errori
di "OVER_QUERY_LIMIT" dovuti al numero eccessivo di chiamate fatte a
Google per geolocalizzare l\'indirizzo, numero questo da mettere sempre
in relazione alle chiamate effettivamente disponibili secondo i
parametri di configurazione del proprio account.

Per evitare questo tipo di problemi, in ogni caso, Passweb distribuirà
automaticamente le chiamate su di un intervallo di tempo più elevato
cosa questa che se da una parte può evitare i problemi di
"OVER_QUERY_LIMIT", dall'altra parte potrebbe ovviamente provocare un
rallentamento nel caricamento dei markers.

**Per questo motivo in caso di rallentamento evidente a causa del numero
eccessivo di marker da gestire, è fortemente consigliato di posizionare
i markers sulla mappa utilizzando direttamente le coordinate (latitudine
e longitudine) in modo tale da evitare chiamate a Google per
geolocalizzare automaticamente i vari indirizzi**.

Rispetto ai marker posizionabili su di una "normale" Google Map, nello
Store Locator sarà poi possibile definire per ciascuno di essi un numero
maggiore di informazioni (es. Immagine del punto vendita, Descrizione
del punto Vendita, Indirizzo del Punto Vendita, Link alla pagina di
dettaglio ecc...), informazioni queste che, oltre ad essere visualizzate
nel fumetto attivabile cliccando sul marker stesso, verranno inserite
anche nell'elenco dei punti vendita visualizzabile, a seconda delle
configurazioni impostate, a fianco, sopra o sotto la mappa stessa.

L'elenco dei punti vendita (o, in generale, degli elementi presenti
sulla mappa) potrà essere filtrato sulla base di determinate
**categorie** personalizzabili in fase di configurazione del componente.

Il campo "**Indirizzo**", presente anch'esso tra i controlli dello store
locator, consente invece di posizionare la mappa sull'indirizzo inputato
(posto ovviamente che sia un indirizzo valido e riconosciuto da Google).
Il pulsante "**Indicazioni**" consente invece di evidenziare sulla mappa
il percorso verso l'ultimo marker selezionato o, nel caso in cui non
fosse stato selezionato alcun marker, verso quello più vicino.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\store_locator_2.bmp](./assets/media/image58.png)

Cliccando infine su uno degli elementi (es. Punti vendita) presenti in
elenco lo stesso elemento verrà evidenziato anche sulla mappa mediante
l'apertura del relativo fumetto.

