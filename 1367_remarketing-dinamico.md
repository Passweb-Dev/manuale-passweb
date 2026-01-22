# REMARKETING DINAMICO



Il Remarketing è una strategia di digital marketing che permette di
mostrare annunci pubblicitari a utenti che hanno già visitato un sito
web. L'obiettivo principale è riportare questi utenti sul sito per
completare una determinata azione che può essere, ad esempio, un
acquisto, una registrazione, la compilazione di un form ecc...

Esistono due principali tipologie di Remarketing: standard e dinamico.

Il **Remarketing Standard** consente di mostrare annunci display
generici (principalmente banner) agli utenti che hanno già visitato il
sito

Il **Remarketing Dinamico** invece è una sorta di upgrade del
Remarketing Standard perché consente di mostrare agli utenti che hanno
già visitato il sito non più degli annunci generici ma annunci
personalizzati relativi esattamente ai prodotti che questi stessi utenti
hanno effettivamente visualizzato sul sito.

Per comprendere meglio la differenza tra queste due tipologie di
Remarketing possiamo considerare l'esempio di un utente che arriva sul
nostro sito e visita, ad esempio, la pagina prodotto di una specifica
scarpa da running.

Implementando il Remarketing Standard quando, nei giorni successivi,
quello stesso utente navigherà altri siti potrà visualizzare banner
pubblicitari che lo invitano a tornare sul nostro sito e che comunque
non avranno alcun riferimento alle scarpe da running che aveva
visualizzato il giorno prima.

Con il Remarketing Dinamico invece quando l'utente nei giorni successivi
navigherà altri siti potrà visualizzare annunci pubblicitari relativi
proprio a quello specifico paio di scarpe visualizzato il giorno prima
magari con anche uno sconto personalizzato per incentivarlo
all'acquisto.

In sostanza dunque, il Remarketing Dinamico può rivelarsi molto più
efficace rispetto a quello standard soprattutto per i siti B2C con
cataloghi di prodotti particolarmente numerosi, dove con il solo
remarketing standard si correrebbe il rischio di visualizzare agli
utenti annunci pubblicitari di prodotti che, alla fine, non sono
esattamente quelli per cui quegli stessi utenti erano finiti sul nostro
sito.

Dal punto di vista tecnico l'implementazione del Remarketing Dinamico è
un po' più complessa e richiede ovviamente l'invio a Google Ads di una
quantità maggiore di dati.

Considerando infatti che non verrà mostrato a tutti gli utenti lo stesso
annuncio pubblicitario (come nel Remarketing Standard) ma annunci con
contenuti diversi a seconda di quello che lo specifico utente ha
effettivamente fatto o visto sul nostro sito, sarà necessario,
ovviamente, tracciare e inviare a Google Ads questo tipo di
informazioni.

Nello specifico gli eventi di remarketing da tracciare saranno:

- **view_item_list**

- **view_item**

- **add_to_cart**

- **purchase**

e, in corrispondenza di ciascuno di essi dovranno essere inviate a
Google Ads informazioni dettagliate relative a tutti i prodotti
coinvolti in questi stessi eventi.

In questo senso, in realtà, sarà sufficiente inviare a Google Ads, oltre
ad un valore monetario da assegnare al relativo evento (valore questo
che coinciderà, tipicamente, con la somma dei prezzi ivati di tutti i
prodotti coinvolti), anche:

- il codice identificativo di ogni singolo prodotto coinvolto in quello
  stesso evento

- l'indicazione di dove Google dovrà andare poi a reperire autonomamente
  le informazioni (titolo, prezzo, sconto, descrizione ...) sui prodotti
  coinvolti nell'evento e che saranno quindi oggetto dei vari annunci
  pubblicitari.

Nello specifico, il parametro da utilizzare per indicare a Google dove
andare a reperire le informazioni sui prodotti inseriti nei vari annunci
pubblicitari è '**google_business_vertical**' e, nel caso di siti
ecommerce, questo parametro dovrà essere valorizzato con la stringa
'**retail'**.

Questa particolare configurazione indica a Google di prelevare le
informazioni di cui a bisogno, relativamente ai prodotti coinvolti negli
annunci di remarketing dinamico, direttamente all'interno di Google
Merchant Center.

Considerando quanto appena detto è quindi abbastanza semplice
comprendere che per **poter gestire in maniera corretta il Remarketing
Dinamico non sarà sufficiente inviare ad Ads, in corrispondenza degli
eventi indicati** **i dati richiesti, ma sarà necessario gestire in
maniera corretta anche un catalogo prodotti all'interno del Merchant
Center, in quanto sarà proprio all'interno del Merchant Center che
Google andrà a reperire in maniera automatica (utilizzando come chiave
l'id prodotto passato ad Ads) tutte le informazioni necessarie per
gestire poi le varie campagne dei prodotti coinvolti nel Remarketing
Dinamico**

**ATTENZIONE!** per poter gestire correttamente il Remarketing Dinamico
è necessario disporre di un Catalogo prodotti all'interno di Google
Merchant Center

Ovviamente l'account del Google Merchant Center dovrà essere lo stesso
utilizzato per Google Ade e, altrettanto chiaramente, il codice dei
prodotti pubblicati all'interno del Merchant Center dovrà essere lo
stesso di quello passato dal sito a Google Ads al verificarsi dei
diversi eventi di Remarketing Dinamico.

Ora al netto del Catalogo prodotti presente all'interno del Merchant
Center, catalogo questo che può tranquillamente essere creato con le
funzionalità disponibili all'interno Wizard (per maggiori informazioni
in merito si veda quanto indicato all'interno del capitolo "*Marketplace
-- Altri Marketplace -- Google Merchant* " di questo manuale), il data
layer gestito da Passweb, è strutturato e contiene già tutte le
informazioni necessarie per poter attivare, all'interno di Google Tag
Manager, la gestione del Remarketing Dinamico.

Nei successivi capitoli di questo manuale vedremo dunque, un po' più nel
dettaglio, la struttura del data layer di Passweb e come poter gestire i
dati in esso presenti per configurare correttamente in GTM i Tag di
Remarketing Dinamico.

