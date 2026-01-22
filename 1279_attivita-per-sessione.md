# ATTIVITA' PER SESSIONE



Come indicato nel precedente capitolo di questo manuale ("*Visitatori*")
una volta effettuato l'accesso alle statistiche relative ai visitatori
del sito, volendo è possibile scendere ancora più in profondità andando
ad esaminare nel dettaglio quello che l'utente ha fatto durante ogni
singola sessione di navigazione.

Per far questo è sufficiente cliccare sull'Id della sessione interessata
presente in corrispondenza di ogni singola riga della tabella contente
l'elenco delle visite registrate dal sito nell'intervallo di tempo
selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attivita_per_sessione_1.bmp](./assets/media/image44.png)

In questo modo, infatti, verrà visualizzata la maschera "**Attività per
Sessione -- Id sessione**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attivita_per_sessione.bmp](./assets/media/image41.png)

all'interno della quale poter ottenere informazioni più dettagliate
relativamente alla sessione di navigazione in questione e alle pagine
effettivamente consultate dall'utente durante questa stessa sessione

In particolare, nella parte alta della pagina sarà possibile ottenere
informazioni relativamente a:

- **Ip**: indirizzo Ip della macchina client dell'utente che sta
  visitando il sito

- **Location:** zona geografica associata all'indirizzo Ip del computer
  su cui risiede il browser utilizzato per navigare il sito.

- **Browser:** browser, con relativa versione, utilizzato per navigare
  il sito

- **Risoluzione del browser:** risoluzione dello schermo impostata sul
  computer dell'utente che sta navigando il sito

- **User Agent:** dettaglio dello User Agent identificativo del browser
  utilizzato dall'utente per navigare il sito.

> Tecnicamente uno **User Agent** altro non è se non un'applicazione
> installata sul computer dell'utente che si connette ad un ben preciso
> processo server. Nello specifico, ovviamente, lo User Agent in
> questione è quello del browser utilizzato dall'utente per connettersi
> ad internet e navigare il nostro sito web. Quando l'utente effettua
> un'operazione di questo tipo il browser utilizzato invia al server su
> cui risiede il sito una stringa di testo utilizzata appunto per
> consentire al server stesso di identificarlo come Chrome piuttosto che
> come Edge, Safari ... e per fornirgli informazioni quali ad esempio la
> versione, il sistema operativo della macchina su cui è installato, la
> lingua, la risoluzione dello schermo ecc...

- **Referrer:** url di partenza utilizzato dall'utente per accedere al
  nostro sito ed iniziare dunque la sua sessione di navigazione.

> l'url Referrer è semplicemente l'URL di un elemento che conduce
> all'elemento corrente; nello specifico, ad esempio, il referrer di una
> pagina web del nostro sito può essere un'altra pagina web, di un altro
> sito, che ospita un link di collegamento al nostro oppure, più
> semplicemente, una pagina dei risultati di ricerca di Google.
>
> In sostanza, dunque, il referrer **rappresenta**, come detto, **il
> punto di parenza** **utilizzato dall'utente per accedere al nostro
> sito.**
>
> Tale informazione può quindi essere particolarmente utile per capire
> ad esempio se il nostro sito è o meno facilmente ricercabile
> all'interno dei vari motori di ricerca (referrer rappresentati da
> pagine di risultati dei motori di ricerca sono, in questo senso,
> informazioni molto indicative), se è pubblicizzato o meno da altri
> siti o se solitamente gli utenti accedono al sito digitandone
> direttamente l'indirizzo web nella barra del browser. In quest'ultimo
> caso il referrer sarebbe nullo e nel campo in questione verrebbe
> quindi riportato il dato n/d (non disponibile)

- **Permanenza sul sito:** consente di visualizzare la durata della
  sessione attualmente selezionata e quindi il tempo speso dall'utente
  all'interno del nostro sito.

La griglia presente nella parte bassa della maschera "Attività per
Sessione" consente invece di visualizzare il dettaglio della navigazione
effettuata dall'utente durante quella stessa sessione

![Videate\\statistiche_panoramica_4.bmp](./assets/media/image45.png)

Il pannello di ricerca presente immediatamente al di sopra della tabella
consente di filtrare i dai in griglia in base alla specifica attività
registrata.

**ATTENZIONE! Le attività tracciabili sono solo ed esclusivamente quelle
indicate in elenco ossia:**

- **Compilazione Form --** Attività registrata nel momento in cui
  l'utente compila uno dei form presenti all'interno del sito e
  realizzati mediante il relativo componente Passweb

- **Completamento Ordine --** Attività registrata nel momento in cui
  l'utente completa un ordine all'interno del sito

- **Completamento Registrazione --** Attività registrata nel momento in
  cui l'utente completa la Registrazione al sito

- **Completamento Reso --** Attività registrata nel momento in cui
  l'utente completa un Reso all'interno del sito

- **Inserimento in Carrello --** Attività registrata nel momento in cui
  l'utente aggiunge un articolo in Carrello

- **Inserimento Indirizzo di Spedizione -** Attività registrata nel
  momento in cui l'utente aggiunge un nuovo Indirizzo di Spedizione

- **Login --** Attività registrata nel momento in cui l'utente effettua
  l'autenticazione al sito

- **Login Social - --** Attività registrata nel momento in cui l'utente
  effettua l'autenticazione al sito utilizzando un suo profilo Social

- **Logout --** Attività registrata nel momento in cui l'utente effettua
  il logout dal sito

- **Modifica Indirizzo Spedizione -** Attività registrata nel momento in
  cui l'utente conferma eventuali modifiche ad uno dei suoi indirizzi di
  spedizione

- **Modifica Profilo -** Attività registrata nel momento in cui l'utente
  conferma eventuali modifiche apportate al suo Profilo

- **Pagina Non Trovata (404):** attività registrata nel momento in cui
  l'utente dovesse incorrere in un errore di tipo 404 -- Pagina Non
  Trovata -- Verrà registrato inoltre anche l' url della pagina che ha
  generato l'errore.

- **Rimozione dal Carrello --** Attività registrata nel momento in cui
  l'utente rimuove un articolo dal Carrello

- **Rimozione Indirizzo di Spedizione-** Attività registrata nel momento
  in cui l'utente elimina un suo Indirizzo di Spedizione

- **Visita Articolo CMS --** Attività registrata nel momento in cui
  l'utente visita una pagina di dettaglio di un contenuto CMS

- **Visita Pagina Catalogo --** Attività registrata nel momento in cui
  l'utente visita una Pagina Catalogo (pagina azzurra)

- **Visita Pagina Generica -** Attività registrata nel momento in cui
  l'utente visita una Pagina Generica (pagina bianca)

- **Visita Pagina Prodotto -** Attività registrata nel momento in cui
  l'utente visita una Pagina Prodotto (pagina rossa)

- **Visita Pagina -** Attività registrata nel momento in cui l'utente
  visita una qualsiasi Pagina del sito

Il pulsante "**Esporta**", consente, infine, di esportare i dati
attualmente presenti in griglia (e quindi eventualmente filtrati
rispetto al totale dei dati stessi) all'interno di un apposito file .csv

