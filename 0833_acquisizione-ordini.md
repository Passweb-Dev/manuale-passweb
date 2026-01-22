# ACQUISIZIONE ORDINI



Come evidenziato nei precedenti capitoli di questo manuale, volendo è
possibile configurare l'integrazione Passweb -- eBay in maniera tale da
importare all'interno del proprio sito Ecommerce, e da qui sul
gestionale Passepartout, gli ordini effettuati direttamente sui
marketplace.

**ATTENZIONE! Verranno importati da eBay solo ed esclusivamente gli
ordini in stato Completed.** Per maggiori informazioni sugli stati
dell'ordine in eBay si rimanda alla relativa documentazione

(http://developer.ebay.com/devzone/xml/docs/reference/ebay/types/OrderStatusCodeType.html)

Per abilitare questo tipo di gestione è necessario impostare il
parametro "**Creare ordini in Passweb**", presente nella maschera di
configurazione dell'Account eBay, sul valore **SI**

![](./assets/media/image165.png)

In questo caso inoltre è possibile impostare anche il sezionale del
gestionale in cui dovranno essere memorizzati gli ordini provenienti da
eBay (**Sezionale degli Ordini**) e il codice Mastro in cui memorizzare
i nuovi clienti acquisiti a seguito di ordini effettuati direttamente su
un marketplace (**Codici Mastro dei Clienti**).

Ovviamente è consigliabile definire uno specifico sezionale per gli
ordini provenienti da eBay in maniera tale da poterli poi distinguere
facilmente da quelli effettuati direttamente sul sito Ecommerce o, ad
esempio, su Amazon.

**ATTENZIONE!** **Nel caso in cui l'utente che ha effettuato l'ordine su
eBay abbia utilizzato un indirizzo mail già presente nel database di
Passweb** (perché già registrato anche sul sito Ecommerce e,
probabilmente, già presente anche sul gestionale), in fase di
importazione ordine verrà agganciata l'Anagrafica di tale utente senza
però sovrascriverne i dati.

In queste condizioni dunque non verrà creata nessuna nuova Anagrafica
Utente. L'indirizzo di spedizione merce presente sul documento importato
da eBay sarà quello definito e selezionato dall'utente stesso
direttamente all'interno di eBay. Nel caso in cui tale indirizzo non
dovesse essere presente tra gli indirizzi già associati all'utente,
verrà creato in Passweb e, laddove possibile, anche all'interno del
gestionale un nuovo indirizzo di spedizione.

Nel caso in cui invece **l'utente che ha effettuato l'ordine su eBay
abbia utilizzato un indirizzo mail non ancora presente nel database di
Passweb,** in fase di importazione ordine verrà creata una nuova
Anagrafica con i dati (es. indirizzo di spedizione) prelevati
direttamente dall'Account eBay del compratore. Tale Anagrafica verrà poi
creata, ovviamente, anche all'interno del gestionale contestualmente con
l'inserimento del nuovo ordine.

**ATTENZIONE!** I **nuovi utenti acquisiti a seguito di ordini
effettuati su eBay** (tipicamente utenti occasionali) non avranno modo
di accedere automaticamente al sito Passweb. Per poter effettuare
acquisti direttamente sul sito Ecommerce tali utenti dovranno quindi
effettuare una nuova registrazione all'interno dello stesso sito
Ecommerce oppure, dovranno essergli assegnate, e comunicate, delle
credenziali di accesso operando direttamente all'interno dei relativi
campi del gestionale.

L'importazione su Passweb degli ordini effettuati su uno dei marketplace
eBay, infine, può avvenire in due modi diversi:

- **Manualmente**, cliccando sul pulsante **Sincro Ordini** (
  ![](./assets/media/image45.png) ) presente nella barra degli strumenti
  della maschera "**Lista degli Account eBay**" dopo aver selezionato
  uno degli Account presenti in elenco.

> **ATTENZIONE!** In queste condizioni verranno importati solo ed
> esclusivamente gli ordini effettuati sui marketplace collegati
> all'Account selezionato
>
> Terminata l'importazione in Passweb verrà lanciata automaticamente una
> sincronizzazione parziale (non scalata dal monte sincronizzazioni
> previste da contratto) in maniera tale da inserire immediatamente i
> nuovi ordini eBay anche all'interno del gestionale.
>
> **ATTENZIONE!** Il processo di importazione ordini da eBay potrebbe
> richiedere diversi minuti. Si consiglia quindi di non eseguire una
> nuova sincronizzazione prima di aver ricevuto la mail di avvenuta
> sincronizzazione relativa a quella eventualmente in corso

- **Automaticamente** a seguito di ogni Sincronizzazione "Sito --
  Gestionale", indipendentemente dal fatto che tale sincronizzazione sia
  stata lanciata in maniera manuale o schedulata.

> **ATTENZIONE!** L'importazione automatica degli ordini effettuati su
> eBay potrà avvenire solo a seguito di Sincronizzazioni Totali o per
> Variati**. In queste condizioni inoltre verranno importati gli ordini
> effettuati sui marketplace collegati a tutti gli Account per i quali
> il parametro "Creare ordini in Passweb" è stato impostato a SI.**
>
> In realtà il processo automatico di importazione ordini da eBay viene
> lanciato, cronologicamente, prima della sincronizzazione Sito --
> Gestionale in maniera tale da poter poi importare sul gestionale
> stesso anche i nuovi ordini effettuati su eBay.
>
> Nel caso in cui in fase di sincronizzazione dovessero essere importati
> ordini da eBay verrà anche inviata un'apposita mail di notifica con
> tutti i dettagli dell'operazione.

**ATTENZIONE!** **In tutti gli ordini importati da eBay verrà inserita
automaticamente una nota di corpo contenente la data e l'identificativo
assegnati all'ordine su eBay**

![](./assets/media/image166.png)

Si ricorda inoltre che le spese di trasporto relative ad ordini
provenienti da eBay sono gestite mediante appositi articoli di tipo
Spesa inserti nel corpo del documento.

**In questo senso è quindi consigliabile gestire articoli spesa diversi
per ciascuna tipologia di spedizione abilitata su eBay in maniera tale
da poter facilmente distinguere, dalla descrizione di questi stessi
articoli spesa, la tipologia di spedizione selezionata dall'utente in
fase di acquisto su eBay**.

Per poter testare e verificare tutto il processo di acquisizione ordini
è possibile utilizzare appositi Account di Test di tipo Compratore
appositamente creati tanto nella Sandbox di eBay quanto in quella di
PayPal.

Utilizzando l'Account eBay di tipo Compratore sarà infatti possibile
autenticarsi direttamente sulla Sandbox di eBay, selezionare gli
articoli pubblicati in questo ambiente tramite il sito Passweb ed
effettuare l'acquisto.

In fase di checkout sarà invece possibile selezionare come modalità di
pagamento PayPal (posto ovviamente di averla abilitata in fase di
configurazione dell'Inserzione). In questo modo si verrà ricondotti
automaticamente alla Sandbox di PayPal stesso dove utilizzando il
relativo account di test sarà possibile completare l'acquisto e
verificare quindi anche il processo di acquisizione del nuovo ordine sul
sito Passweb.

Per maggiori informazioni relativamente alla creazione di Utenti
Compratore nelle Sandbox di eBay e PayPal si vedano anche i relativi
capitoli di questo manuale.

**ATTENZIONE! Tutti gli ordini acquisiti dai marketplace eBay possono
essere visualizzati e gestiti all'interno della sezione "Catalogo --
eBay - Ordini" del Wizard**

Per maggiori informazioni in merito alla gestione di questi ordini e ai
loro possibili stati si veda anche il successivo capitolo di questo
manuale.

