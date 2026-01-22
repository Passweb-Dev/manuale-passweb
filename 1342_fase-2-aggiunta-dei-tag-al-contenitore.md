# FASE 2 -- AGGIUNTA DEI TAG AL CONTENITORE



Arrivati a questo punto abbiamo creato il nostro Account GTM, il nostro
primo Contenitore e lo abbiamo anche installato in tutte le pagine del
sito Passweb.

Tale Contenitore però, allo stato attuale, è ancora completamente
inutile, sia perché non è ancora stato pubblicato sia, soprattutto,
perché non è ancora stato inserito al suo interno alcun Tag.

Il prossimo passo sarà quindi quello di inserire all'interno del
Contenitore tutti i Tag di cui abbiamo bisogno, in relazione ovviamente
a quelle che sono le necessità di analisi e tracciamento del nostro sito
e agli strumenti di terze parti che vogliamo utilizzare per questo tipo
di operazioni.

In questo senso, come evidenziato nei precedenti capitoli di questo
manuale, uno dei grandi vantaggi di GTM è rappresentato proprio dal
fatto che per aggiungere, modificare o eliminare Tag dal Contenitore
installato all'interno del nostro sito occorre operare direttamente
dall'interfaccia web di GTM (senza dover intervenire in modo diretto sul
codice sorgente delle pagine).

Nello specifico dunque, sarà necessario accedere al proprio Account GTM
e selezionare, tra quelli presenti all'interno della pagina **Account**,
il Contenitore all'interno del quale si desidera inserire nuovi Tag

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_12a.bmp](./assets/media/image13.png)

In questo modo verremo infatti ricondotti alla dashboard di gestione del
Contenitore selezionato da dove, oltre a verificare lo stato del
Contenitore stesso (pubblicato, non pubblicato, in anteprima ecc ...),
la sua versione e le attività recenti per esso eseguite, potremo
ovviamente procedere anche alla creazione di nuovi Tag.

Per questo sarà sufficiente cliccare sulla voce **Tag** presente nel
menu di sinistra

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_13a.bmp](./assets/media/image14.png)

e, successivamente sul pulsante "**Nuovo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_14a.bmp](./assets/media/image15.png)

In alternativa è anche possibile cliccare direttamente sulla voce
**"Aggiungi un nuovo Tag"** presente nella dashboard di gestione del
Contenitore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_15a.bmp](./assets/media/image16.png)

In entrambi i casi verremo comunque ricondotti alla maschera di
creazione del nuovo Tag

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_16a.bmp](./assets/media/image17.png)

dove dovremo assegnare un nome al Tag e, soprattutto, selezionare il
tipo di Tag da aggiungere al nostro contenitore ( e conseguentemente, lo
strumento di terze parti con cui vogliamo integrare il nostro sito e
verso il quale dovremo quindi inviare tutte le informazioni e i dati di
tracciamento richiesti).

In questo senso sarà quindi necessario cliccare sul pulsante "**Scegli
un tipo di tag per iniziare l'installazione**" e selezionare poi, tra
quelli proposti, lo specifico Tag da inserire

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_17a.bmp](./assets/media/image18.png)

**ATTENZIONE!** Nel caso in cui il Tag che si desidera inserire
all'interno del Contenitore non sia tra quelli predefiniti messi a
disposizione da GTM, è sempre possibile comunque inserire lo specifico
codice all'interno, ad esempio, di un "**Tag HTML personalizzato**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_18a.bmp](./assets/media/image19.png)

A seconda del tipo di Tag sarà poi necessario impostare anche altri
parametri di configurazione specifici per la particolare tipologia di
Tag selezionata

**ATTENZIONE! I parametri di configurazione di un Tag possono variare in
relazione alla specifica tipologia di Tag**

Nel caso in cui, ad esempio, si sia scelto di inserire nel Contenitore
un Tag per il monitoraggio di Google Analytics, sarà necessario, innanzi
tutto decidere se il Tag in questione dovrà essere quello relativo a
Universal Analytics, oppure uno di quelli relativi al nuovo Google
Analytics 4

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_19a.bmp](./assets/media/image20.png)

Nel momento in cui si dovesse optare, ad esempio, per il Tag di
Universal Analytics sarà poi necessario, indicare il "**Tipo di
Monitoraggio**" da implementare (Visualizzazioni di pagina, Eventi ...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_21a.bmp](./assets/media/image21.png)

l' **ID monitoraggio** della Proprietà di Analytics cui dovranno essere
spediti i dati (all'interno dell'apposito campo o nella relativa
Variabile) e anche tutta una serie di altri parametri di configurazione
relativi allo specifico monitoraggio che si vuole effettivamente
implementare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_20a.bmp](./assets/media/image22.png)

**ATTENZIONE!** I parametri di configurazione del Tag possono variare
anche in relazione alla "Tipologia di Monitoraggio" implementata

**ATTENZIONE!** Dipendentemente dal Tag selezionato e dalla particolare
configurazione impostata potrebbe essere necessario intervenire anche a
livello di Data Layer. Per maggiori informazioni in merito **si
consiglia dunque di fare sempre riferimento alla specifica
documentazione di GTM**

Una volta impostati correttamente i parametri di configurazione
richiesti dallo specifico Tag sarà poi necessario decidere quando questo
stesso Tag dovrà effettivamente essere attivato associandogli quindi un
ben preciso **Attivatore.**

In questo senso sarà sufficiente cliccare sul pulsante "**Scegli un
attivatore per attivare questo tag**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_22a.bmp](./assets/media/image23.png)

e selezionare poi, tra quelli proposti, l'attivatore da utilizzare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_22b.bmp](./assets/media/image24.png)

**ATTENZIONE!** Come evidenziato nei precedenti capitoli di questo
manuale ogni Tag deve avere associato almeno un Attivatore. Per maggiori
informazioni in merito agli Attivatori si consiglia di fare sempre
riferimento alla specifica documentazione di GTM

Una volta impostati anche gli Attivatori, il pulsante **"Salva"**
consente di creare definitivamente il Tag in esame inserendolo quindi
all'interno del nostro Contenitore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_22c.bmp](./assets/media/image25.png)

Il Tag così creato verrà ora visualizzato all'interno della sezione Tag
da dove potrà anche essere modificato in qualsiasi momento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_24a.bmp](./assets/media/image26.png)

