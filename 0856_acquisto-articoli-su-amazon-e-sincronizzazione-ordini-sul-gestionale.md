# ACQUISTO ARTICOLI SU AMAZON E SINCRONIZZAZIONE ORDINI SUL GESTIONALE



Come evidenziato nei precedenti capitoli di questo manuale, volendo, è
possibile configurare l'integrazione Passweb -- Amazon in maniera tale
da importare all'interno del proprio sito Ecommerce, e da qui sul
gestionale Passepartout, gli ordini effettuati direttamente sul relativo
marketplace.

**ATTENZIONE!** Verranno importati da Amazon solo ed esclusivamente gli
ordini che si trovano in uno degli stati indicati nel box di destra
della sezione "**Stati Ordine**" presente nella maschera di
configurazione del proprio Account Amazon (tab "Ordini"). Per maggiori
informazioni sugli stati dell'ordine in Amazon si rimanda alla relativa
documentazione

Per abilitare questo tipo di gestione è necessario impostare il
parametro "**Creare ordini in Passweb**", presente nella maschera di
configurazione dell'Account Amazon (tab "Ordini"), sul valore **SI**

![](./assets/media/image288.png)

In questo caso inoltre è possibile impostare anche il sezionale del
gestionale in cui dovranno essere memorizzati gli ordini provenienti da
Amazon (**Sezionale degli Ordini**) e il codice Mastro in cui
memorizzare i nuovi clienti acquisiti a seguito di ordini effettuati
direttamente su un marketplace (**Codici Mastro dei Clienti**).

Ovviamente è consigliabile definire uno specifico sezionale per gli
ordini provenienti da Amazon in maniera tale da poterli poi distinguere
facilmente da quelli effettuati direttamente sul sito Ecommerce o, ad
esempio, su eBay.

**ATTENZIONE!** **Nel caso in cui l'utente che ha effettuato l'ordine su
Amazon abbia utilizzato un indirizzo mail già presente nel database di
Passweb** (perché già registrato anche sul sito Ecommerce e,
probabilmente, già presente anche sul gestionale), in fase di
importazione ordine verrà agganciata l'Anagrafica di tale utente senza
però sovrascriverne i dati.

In queste condizioni dunque non verrà creata nessuna nuova Anagrafica
Utente. L'indirizzo di spedizione merce presente sul documento importato
da Amazon sarà quello definito e selezionato dall'utente stesso
direttamente all'interno di Amazon.

Nel caso in cui tale indirizzo non dovesse essere presente tra gli
indirizzi già associati all'utente, verrà creato in Passweb e, laddove
possibile, anche all'interno del gestionale un nuovo indirizzo di
spedizione.

Nel caso in cui invece **l'utente che ha effettuato l'ordine su Amazon
abbia utilizzato un indirizzo mail non ancora presente nel database di
Passweb,** in fase di importazione ordine verrà creata una nuova
Anagrafica con i dati (es. indirizzo di spedizione) prelevati
direttamente dall'Account Amazon del compratore. Tale Anagrafica verrà
poi creata, ovviamente, anche all'interno del gestionale contestualmente
con l'inserimento del nuovo ordine.

**ATTENZIONE!** I **nuovi utenti acquisiti a seguito di ordini
effettuati su Amazon** (tipicamente utenti occasionali) non avranno modo
di accedere automaticamente al sito Passweb. Per poter effettuare
acquisti direttamente sul sito Ecommerce tali utenti dovranno quindi
effettuare una nuova registrazione all'interno dello stesso sito
Ecommerce oppure, dovranno essergli assegnate, e comunicate, delle
credenziali di accesso operando direttamente all'interno dei relativi
campi del gestionale.

La sincronizzazione Ordini tra Passweb ed Amazon può avvenire in due
modi diversi:

- **Manualmente**, cliccando sul pulsante **Sincro Ordini** (
  ![](./assets/media/image45.png) ) presente nella barra degli strumenti
  della maschera "**Gestione Account**" dopo aver selezionato uno degli
  Account presenti in elenco.

> **ATTENZIONE!** In queste condizioni verranno importati solo ed
> esclusivamente gli ordini effettuati sui marketplace collegati
> all'Account selezionato
>
> Terminata l'importazione in Passweb verrà lanciata automaticamente una
> sincronizzazione parziale (non scalata dal monte sincronizzazioni
> previste da contratto) in maniera tale da inserire immediatamente i
> nuovi ordini Amazon anche all'interno del gestionale.
>
> **ATTENZIONE!** Il processo di importazione ordini da Amazon potrebbe
> richiedere diversi minuti. Si consiglia quindi di non eseguire una
> nuova sincronizzazione prima di aver ricevuto la mail di avvenuta
> sincronizzazione relativa a quella eventualmente in corso

- **Automaticamente:**

  - a seguito di ogni Sincronizzazione "Sito -- Gestionale",
    indipendentemente dal fatto che tale sincronizzazione sia stata
    lanciata in maniera manuale o schedulata.

> In questo caso la sincronizzazione ordini riguarderà i marketplace
> collegati a tutti gli Account Amazon gestiti

- secondo la schedulazione (mensile, settimanale, giornaliera, oraria
  ...) impostata nella maschera di configurazione dello specifico
  Account Amazon all'interno della sezione "**Schedulazione**".

> In questo caso, ovviamente, la sincronizzazione ordini riguarderà solo
> ed esclusivamente i Marketplace collegati all'account Amazon in cui è
> stata impostata la relativa schedulazione
>
> **ATTENZIONE!** il processo automatico di importazione ordini da
> Amazon viene lanciato, cronologicamente, prima di eventuali
> sincronizzazioni Sito -- Gestionale in maniera tale da poter poi
> importare sul gestionale stesso anche i nuovi ordini effettuati su
> Amazon.
>
> Nel caso in cui in fase di sincronizzazione dovessero essere importati
> ordini da Amazon verrà anche inviata un'apposita mail di notifica con
> tutti i dettagli dell'operazione.

**ATTENZIONE!** In tutti gli ordini importati da Amazon verrà inserita
automaticamente una nota di corpo contenente la data e l'identificativo
assegnati all'ordine su Amazon

![](./assets/media/image289.png)

Si ricorda inoltre che le spese di trasporto relative ad ordini
provenienti da Amazon sono gestite mediante appositi articoli di tipo
Spesa inserti nel corpo del documento.

In questo senso è quindi consigliabile gestire specifici articoli spesa
in maniera tale da poter facilmente individuare che l'articolo spesa in
esame è stato inserito per gestire le spese di trasporto.

**ATTENZIONE**! Si ricorda che Amazon a differenza di eBay non mette a
disposizione dell'utente un ambiente di test per cui tutte le operazioni
del caso potranno essere provate e testate utilizzando unicamente
pubblicazioni reali sul relativo Marketplace Amazon.

