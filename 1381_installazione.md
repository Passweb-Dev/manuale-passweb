# INSTALLAZIONE



Come evidenziato nel precedente capitolo di questo manuale uno dei
vantaggi principali di Matomo rispetto a Google Analytics, soprattutto
in ottica privacy e GDPR, è indubbiamente quello di poterlo installare
su di un server proprietario mantenendo sempre il controllo totale dei
dati raccolti ed evitando anche di inviarli a terze parti, come avviene
invece nel caso di Google Analytics.

In questo senso, volendo essere più precisi, è bene sottolineare che
esistono due diverse versioni di questo software, o meglio due diverse
modalità di installazione:

![Videate\\matomo_5.bmp](./assets/media/image5.png)

- una versione gratuita, **On Premise**

> Questa configurazione richiede l'installazione, su di un server
> proprietario (o quanto meno all'interno di uno spazio di hosting
> appositamente abilitato e configurato) di tutto quanto richiesto da
> Matomo (php, MySQL ...) per poter funzionare in maniera corretta,
> oltre ovviamente all'installazione del software stesso.
>
> Il software in se non ha alcun costo (essendo open source sotto
> licenza GPL) per cui le uniche spese da sostenere in questa
> configurazione saranno legate al costo del server, o dell'abbonamento
> al servizio di hosting (condiviso o dedicato) che andremo ad
> utilizzare per installare tutti i servizi.
>
> Avendo il pieno controllo del database e del software non ci saranno
> limiti sulla quantità di dati che potranno essere salvati (ovviamente
> moli di dati importanti andranno poi gestite in maniera adeguata) e
> allo stesso modo avremo la possibilità di personalizzare l'interfaccia
> grafica e le funzionalità dello strumento secondo le specifiche
> esigenze del caso ricorrendo ai diversi plugin disponibili nel
> relativo marketplace
>
> Di contro, chiaramente, questo tipo di configurazione richiede
> determinate conoscenze tecniche sia per quel che riguarda l'effettiva
> installazione di tutto il necessario (anche se in realtà questo
> potrebbe essere effettuato in maniera piuttosto semplice utilizzando
> strumenti automatici come Softaculus messi a disposizione dai vari
> servizi di hosting) sia anche poi per una corretta gestione di tutto
> il sistema (aggiornamenti compresi) una volta portato in produzione.
>
> **ATTENZIONE!** Nel momento in cui si dovesse decidere di utilizzare
> la versione On Premise di Matomo optando anche per l'utilizzo di un
> determinato servizio di hosting è consigliabile verificare,
> innanzitutto, che il provider scelto (es. Aruba) offra effettivamente
> un hosting compatibile con Matomo (dotato quindi di php e MySQL) e
> magari anche strumenti come **Softaculous** (già integrati nel
> relativo cPanel) che consentono effettivamente di gestire
> l'installazione di tutto l'ambiente in maniera automatica con pochi
> click
>
> Per maggiori informazioni in merito alle procedure di installazione On
> Premise di Matomo è possibile fare riferimento ad una delle tante
> guide disponibili in rete (es.
> <https://supporthost.com/it/installare-matomo/> )

- una versione a pagamento, **Cloud**

> In questo caso è possibile disporre di un ambiente già tutto
> configurato e pronto all'uso. Il software può essere utilizzato quindi
> come un semplice servizio e l'unica cosa richiesta, esattamente come
> Google Analytics, sarà quella di inserire lo script di tracciamento
> all'interno del proprio sito.
>
> Anche in questo caso il software in se non avrà un costo specifico ma
> verranno utilizzati i server di Matomo (localizzati in Europa) per
> archiviare i dati e questo comporterà ovviamente la sottoscrizione di
> un abbonamento mensile o annuale di importo variabile in relazione al
> traffico generato e quindi alla quantità di dati raccolti e
> immagazzinati.
>
> Per maggiori informazioni relativamente alle modalità di installazione
> e di utilizzo di Matomo, oltre che ovviamente per informazioni più
> dettagliate sui costi dell'abbonamento al servizio cloud, sulle
> modalità di utilizzo del servizio e di calcolo dei dati inviati è
> necessario fare riferimento direttamente al sito ufficiale della
> piattaforma <https://matomo.org/pricing/>

**ATTENZIONE! Indipendentemente dalla versione utilizzata (On Premise o
Cloud) l'integrazione con Passweb presuppone che Matomo sia già
installato e che possa quindi funzionare in maniera corretta.
Passepartout non offre servizi di hosting per Matomo e non fornisce
assistenza in merito all'installazione e all'utilizzo di questo
prodotto.**

