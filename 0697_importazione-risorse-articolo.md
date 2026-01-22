# IMPORTAZIONE RISORSE ARTICOLO



La procedura di **Importazione delle risorse articolo** è quella
particolare operazione che permette a Passweb di prelevare tutte le
risorse grafiche (immagini e schede tecniche) associate, direttamente
sul gestionale, agli articoli gestiti all'interno del sito.

**ATTENZIONE! A differenza dei dati aggiuntivi articolo, legati alle
Funzionalità Mexal e gestiti, all'interno di Mexal stesso, mediante
un'apposita videata aggiuntiva articolo per ognuno dei 9 possibili siti
collegati alla stessa azienda, le immagini e/o le schede tecniche
associate all'articolo direttamente da Mexal, sono uniche per tutti i
siti su cui lo stesso articolo verrà poi esportato**

Nel caso in cui l'esigenza dovesse essere quella di esportare uno stesso
articolo su più siti differenti e gestire su ognuno di essi immagini e/o
schede tecniche diverse sarà necessario, per forza di cose, associare le
diverse risorse all'articolo direttamente dal Wizard dei diversi siti.

Come per la sincronizzazione, anche la procedura di importazione delle
risorse articolo, può essere eseguita in maniera manuale oppure
automaticamente al termine di ogni sincronizzazione schedulata.

**ATTENZIONE! In ogni caso va sottolineato che la procedura di
Importazione Risorse NON andrà mai ad incidere in alcun modo sul monte
sincronizzazioni previste da contratto essendo questa una procedura
diversa da quella di sincronizzazione**

E' anche vero comunque che, se a seguito di una sincronizzazione
dovessero essere esportati sul sito **nuovi articoli** e, all'interno
del gestionale tali articoli avessero già delle risorse grafiche
associate, allora la sincronizzazione stessa oltre a portare sul sito
l'articolo con i relativi dati, si preoccuperà di prelevare ed esportare
anche tutte le risorse grafiche ad esso associate.

**In definitiva, dunque, questo tipo di operazione dovrà essere eseguita
ogni qual volta si aggiungano e/o si modifichino risorse grafiche ad
articoli già esportati e gestiti sul sito, in maniera tale da poter
prelevare solo queste risorse senza dover utilizzare le sincronizzazioni
previste da contratto.**

Per avviare la procedura di importazione delle risorse articolo in
maniera manuale è sufficiente cliccare sul pulsante "**Importa
Risorse**" presente, nella maschera di configurazione dei parametri di
sincronizzazione, all'interno della sezione **"Importazione Risorse
Articolo"**

![](./assets/media/image177.png)

Il campo **"Data di ultima importazione delle risorse articolo"**
consente di specificare una data a partire dalla quale dovrà essere
effettuata la ricerca, lato gestionale, di nuove immagini da importare.

**Impostata una data, verranno quindi importate tutte le risorse
grafiche associate agli articoli che risulteranno essere stati variati
in una data successiva a quella impostata**.

**ATTENZIONE!** da Docuvision verranno importate unicamente quelle
immagini che sono state caricate con data maggiore o uguale alla data
indicata all'interno di questo campo (data questa che verrà aggiornata
automaticamente al termine della procedura).

Nel caso in cui non venga specificata nessuna data, saranno importate
tutte le risorse articolo, indipendentemente dalla data in cui sono
state caricate (**in queste condizioni la procedura potrebbe impiegare
più tempo**).

Il campo "**Elenco Codici Articolo (csv-txt)**" consente invece di
importare un file csv / txt contenente l'elenco dettagliato dei soli
codici articolo per i quali dovranno essere importate le relative
risorse (immagini e schede tecniche)

**ATTENZIONE! Nel momento in cui l'esigenza dovesse essere quella di
importare un numero particolarmente elevato di risorse, andando così in
contro al rischio di avviare una procedura che potrebbe durare anche
parecchie ore, si consiglia di utilizzare il campo "Elenco Codici
Articolo (csv-txt)" in maniera tale da suddividere l'importazione in più
scaglioni distinti caratterizzati ciascuno da un minor numero di
articoli da processare (e quindi di risorse da importare)**

In questo modo si potrà avere un maggiore controllo sulla procedura di
importazione impattando in maniera minore anche sulle prestazioni del
sito.

In merito al campo in oggetto è bene sottolineare inoltre che:

- Nel file da importare i codici articolo **dovranno essere indicati
  senza separatore e su righe differenti**.

> [ESEMPIO]{.underline}
>
> Codice1
>
> Codice2
>
> Codice3

- Nel momento in cui si dovesse optare per un'importazione scaglionata
  delle risorse articolo **verrà comunque tenuto conto della "Data di
  Ultima importazione risorse articolo"** (se impostata)

- Nel momento in cui si dovesse optare per un'importazione scaglionata
  delle risorse articolo e tale procedura dovesse dare esito positivo,
  al termine verrà automaticamente ripristinata all'interno del campo
  "Data di Ultima importazione risorse articolo", la data che era
  presente in questo stesso campo prima di avviare la procedura di
  importazione (in modo tale da garantire il corretto funzionamento del
  successivo parametro "Importa risorse articoli solo se automatica")

Il parametro "**Importa risorse articoli (solo se automatica e Mexal \>=
2023H)**" presente solo per siti Ecommerce collegati a Mexal e valido
solo per versioni di Mexal successive alla 2023H

![](./assets/media/image178.png)

consente di automatizzare la procedura in esame.

Selezionando questo parametro infatti **a seguito di ogni
sincronizzazione schedulata** verrà eseguita automaticamente anche la
procedura di importazione risorse utilizzando come data di ultima
importazione quella indicata all'interno dell'apposito campo (data
questa che verrà poi aggiornata automaticamente al termine della
procedura stessa)

**ATTENZIONE! Nel caso in cui si dovesse decidere di gestire l'immagine
del prodotto direttamente sull'anagrafica articolo del gestionale è
consigliato lasciare il flag in esame deselezionato.**

**In caso contrario infatti una semplice variazione dell'anagrafica
articolo (F10) comporterebbe, in fase di sincronizzazione, il
trasferimento a Passweb dell'immagine anche se, di fatto, questa non è
stata variata rispetto all'ultima sincronizzazione**

Volendo, infine, è possibile richiamare la procedura di Importazione
Risorse anche da Mexal. Per maggiori informazioni in merito si veda
anche il successivo capitolo *"Sincronizzazione lanciata da Mexal"* di
questo manuale

In ogni caso, una volta lanciata la procedura di Importazione Risorse
l'esito verrà notificato via mail all'indirizzo indicato in
corrispondenza del campo **E-mail** presente all'interno della sezione
"**Parametri importazione risorse**"

![](./assets/media/image179.png)

**ATTENZIONE!** nel caso in cui il campo E-mail evidenziato in figura
non dovesse essere valorizzato, la mail di notifica verrà inviata
all'indirizzo indicato in corrispondenza del campo E-mail presente alla
pagina "**Account e-mail SMS**" del Wizard (menu "*Posta / SMS --
Impostazioni -- Configurazione*")

Infine, il pulsante "**Cancella Risorse Inesistenti**" (solo Ecommerce
Mexal) consente di eliminare automaticamente tutte le risorse non più
collegate, in Mexal, agli articoli attualmente gestiti all\'interno del
sito.

**ATTENZIONE!**: durante la procedura di cancellazione delle risorse
inesistenti **NON** verranno importate nuove risorse all'interno del
sito.

**NOTA BENE:** la procedura di importazione di nuove risorse articolo,
così come quella di eliminazione delle risorse inesistenti, non incide
sul numero di sincronizzazioni disponibili da contratto.

Per maggiori informazioni relativamente alle modalità di caricamento in
Docuvision delle immagini e delle schede articolo da utilizzare poi
all'interno del sito e-commerce, o per come fare a distinguere
l'Immagine del catalogo dalle Immagini (principale e secondarie) della
Scheda Prodotto, si veda anche la sezione "*Catalogo -- Configurazione
Parametri Catalogo -- Associazione delle immagini e delle schede
tecniche allo specifico articolo*" di questo manuale.

