# FASE 3 -- ANTEPRIMA DI PUBBLICAZIONE DEL CONTENITORE



Una volta aggiunti al Contenitore tutti i Tag di cui abbiamo bisogno,
potremmo passare ora alla sua pubblicazione in maniera tale da avviare
il sistema di raccolta dati.

Nel caso in cui dovessimo però aver dei dubbi in merito a quanto fatto e
dovessimo pensare che qualcosa nella creazione del Contenitore e/o nella
configurazione di un Tag sia andato storto, prima di pubblicare il
Contenitore e di metterlo quindi in produzione, potremmo anche
utilizzare una funzionalità di GTM estremamente importante, vale a dire
la modalità "**Anteprima**"

La visualizzazione in anteprima ci permette infatti di eseguire un
controllo di qualità verificando come il nostro sito si comporterà nel
momento in cui il Contenitore in esame dovesse essere effettivamente
pubblicato e quali Tag si attiveranno o meno durante la navigazione e
l'interazione con il sito

Per attivare questo tipo di modalità è sufficiente accedere alla
dashboard di gestione del Contenitore e cliccare sul pulsante
"**Anteprima**" presente nella parte alta della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_25a.bmp](./assets/media/image27.png)

In alternativa è anche possibile accedere alla sezione "**Versioni**"
dell'interfaccia web di GTM, individuare la versione dello specifico
Contenitore su cui si desidera operare e selezionare dal menu
**"Azioni"** la voce **Anteprima**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_26a.bmp](./assets/media/image28.png)

In ogni caso dopo aver avviato la modalità Anteprima ci verrà chiesto di
connettere una pagina del nostro sito a GTM mediante Tag Assistant (di
cui è presente anche un'apposita estensione per Chrome o per i browser
WebKit)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_26b.bmp](./assets/media/image29.png)

Una volta indicata la pagina del sito da collegare cliccando sul
pulsante "**Connect**" verrà aperto un nuovo tab del browser con la
pagina indicata e verrà stabilita la connessione tra quella specifica
sessione di visita e Google Tag Manager

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_26c.bmp](./assets/media/image30.png)

Tornando invece nel tab relativo a Tag Assistant e Tag Manager avremo la
possibilità di visualizzare una console contenente informazioni
dettagliate sul Contenitore che dovrebbe essere pubblicato all'interno
del sito e sui Tag in esso contenuti, compreso il loro stato di
attivazione (Tags Fired o Tags not Fired).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_27a.bmp](./assets/media/image31.png)

**ATTENZIONE!** La Console evidenziata in figura verrà visualizzata solo
ed esclusivamente sullo stesso browser utilizzato per gestire GTM. In
queste condizioni dunque il Tag non è ancora pubblicato e le normali
visite al sito effettuate da browser diversi da quello in cui si sta
gestendo GTM non invieranno alcun tipo di dati.

Cliccando su uno di questi Tag sarà possibile visualizzare informazioni
dettagliate sulle sue proprietà e sui suoi attivatori

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_29a.bmp](./assets/media/image32.png)

Per maggiori informazioni sulle funzionalità di anteprima e debug e
sulla relativa console si consiglia di fare riferimento alla specifica
documentazione di GTM presente in rete.

**ATTENZIONE! Prima di pubblicare un Contenitore occorre anche
accertarsi che altri script, eventualmente presenti nelle pagine del
sito e che fanno riferimento al tracciamento di funzionalità gestite ora
con GTM, siano stati opportunamente rimossi (evitando così che gli
stessi dati vengano tracciati due volte).**

**Se ad esempio, avessimo deciso di implementare Google Analytics
inserendo il relativo codice di monitoraggio direttamente all'interno
della pagina web (mediante l'apposita funzionalità Passweb) e,
successivamente, avessimo deciso di inserire uno o più Tag Google
Analytics anche all'interno del Contenitore gestito da GTM, gli stessi
dati verranno tracciati due volte falsando quindi, in maniera anche
abbastanza netta, tutte le statistiche di Google Analytics**

**NOTA BENE:** Nel caso in cui si decida di gestire l'integrazione tra
il proprio sito e Google Analytics mediante l'apposita funzionalità
nativa di Passweb, è indispensabile non attivare lo stesso tipo di
tracciamento anche in GTM e viceversa

