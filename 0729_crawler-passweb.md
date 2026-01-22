# CRAWLER PASSWEB



Come già evidenziato nei precedenti capitoli di questo manuale il
processo di creazione della cache non è istantaneo ma è un processo che
avviene in maniera automatica mano a mano che il sito riceve delle
visite.

In conseguenza di ciò i benefici apportati da questo sistema potrebbero
anche non essere immediatamente visibili per determinati utenti e / o
per determinate pagine.

In questo senso Passweb offre all'amministratore del sito la possibilità
di lanciare un Crawler automatico che andrà a scansionare determinate
pagine del sito simulando quelle che potrebbero essere delle visite
effettuate da utenti non autenticati e permettendo così alla cache di
costruirsi prima ancora che le pagine interessate vengano effettivamente
visualizzate da utenti reali.

Il Crawler Passweb potrà essere lanciato in maniera manuale cliccando
sul pulsante "**Avvia Crawler**" presente all'interno della maschera
"**Gestione Cache**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\crawler_passweb_1.bmp](./assets/media/image271.png)

oppure potrà anche essere lanciato in automatico da Passweb al termine
di ogni sincronizzazione sito -- gestionale (sia Standard che Totale)
**a patto però di aver attivato il flush automatico della cache**

Il pulsante "**Log Crawler**" presente sempre nella parte bassa della
pagina "Gestione Cache" consente invece di scaricare un file di log
contenente i dettagli relativi alle pagine visitate dal Crawler Passweb
durante l'ultima scansione del sito. Inoltre all'termine della scansione
verrà anche inviata una mail con l'esito dell'operazione all'indirizzo
impostato all'interno della pagina "Posta / SMS" del Wizard

In relazione all'utilizzo del Crawler messo a disposizione da Passweb
occorre fare un paio di osservazioni di fondamentale importanza. Nello
specifico è bene sottolineare che:

- **Il Crawler Passweb non eseguirà mai una scansione completa del sito
  ma si limiterà a visitare le pagine prodotto, con un massimo di 100,
  risultanti dal filtro articoli impostato in corrispondenza del
  parametro "Filtro Articoli Crawler"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\crawler_passweb_filtro_articoli.bmp](./assets/media/image272.png)

> Considerando infatti che un sito Ecommerce potrebbe avere anche
> migliaia di pagine e che il processo di scansione dovrebbe comunque
> essere eseguito in un tempo limitato (il che implica il fatto di
> visitare le pagine interessate con una frequenza piuttosto elevata),
> effettuando il crawling dell'intero sito il carico cui si troverebbe
> sottoposto il server web potrebbe essere particolarmente elevato
> provocando quindi un degradamento delle performance non solo per il
> sito in esame ma anche per tutti gli altri siti presenti sullo stesso
> server web (si ricorda infatti che, di base, i siti Passweb sono
> gestiti in hosting condiviso).
>
> Per evitare questo tipo di problemi è stato quindi imposto il limite
> delle 100 pagine prodotto per ogni scansione effettuata.

- **Per i siti multilingua, in fase di Crawling, verranno considerati
  solamente gli url delle pagine prodotto nella lingua di default del
  sito.**

> Ciò significa dunque che nel momento in cui la lingua di default del
> sito dovesse essere, ad esempio, l'italiano, le richieste effettuate
> dal Crawler Passweb verranno gestite come se fossero effettuate da un
> browser con la lingua impostata su "it-IT" e andranno quindi a
> generare la cache solamente per le corrispondenti pagine prodotto in
> italiano.

