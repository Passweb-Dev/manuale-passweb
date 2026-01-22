# INSERIMENTO SUL GESTIONALE DI ORDINI CON ASSOCIATO UN SET DI OPZIONI



Confermando un ordine con associato un determinato Set di Opzioni, le
informazioni aggiuntive inserite dall'utente in fase di checkout,
potranno essere inserite anche nelle mail gestite in automatico da
Passweb oltre che, ovviamente, nel relativo documento gestionale.

Nello specifico, per fare in modo che questo tipo di dato venga inserito
nelle varie mail di ordine gestite in automatico da Passweb sarà
necessario accertarsi di aver gestito correttamente, nel "Dettaglio"
della corrispondente e-mail, i segnaposto presenti all'interno della
sezione "**Campi Opzioni Documento**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_opzioni_documento.bmp](./assets/media/image711.png)

**ATTENZIONE!** per maggiori informazioni in merito alla
personalizzazione delle mail di Ordini/Bolle/Fatture si rimanda a quanto
indicato all'interno del capitolo "*Ordini -- Configurazioni Ordini --
Documento -- Personalizzazione del template di Ordini / Bolle /
Fatture*" di questo manuale

Per quel che riguarda invece **l'inserimento di queste informazioni nel
corrispondente documento gestionale è bene sottolineare che, come per le
custom option, anche in questo caso le informazioni aggiuntive verranno
gestite mediante l'inserimento, nel corpo del documento, di apposite
note precedute a default, questa volta, dai caratteri #@**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opzioni_ordine_gestionale.bmp](./assets/media/image712.png)

Volendo è anche possibile indicare una serie di caratteri differenti da
anteporre alle note utilizzate per gestire queste opzioni di
personalizzazione agendo, in questo senso, mediante il parametro
"**Prefisso Opzioni Documento**" presente alla pagina "Configurazione
Ordini" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordini_prefisso_opzioni.bmp](./assets/media/image713.png)

**ATTENZIONE! E' di fondamentale importanza non variare in alcun modo
sul gestionale le informazioni contenute nelle note relative alle
opzioni di personalizzazione**

La forma e la struttura di tali note è infatti indispensabile, in fase
di rilettura del documento, per poter mantenere anche sulla versione web
di documenti evasi e/o modificati le stesse opzioni di personalizzazione
presenti nel documento sorgente.

Nel momento in cui all'interno del gestionale si dovessero variare le
note relative alle opzioni di personalizzazione in oggetto, quando poi
l'ordine verrà riportato su Passweb (a seguito ad esempio della sua
evasione) le informazioni in esso presenti potrebbero non combaciare più
con quelle presenti nel documento originale, senza contare poi che, in
caso di riordino a partire da documenti che sono stati modificati lato
gestionale, potrebbero presentarsi dei problemi relativi alle opzioni di
personalizzazione in esso presenti.

**Nel caso in cui l'esigenza dovesse essere quella di non far comparire
nella stampa dei documenti queste note "particolari" sarà necessario
configurare correttamente la relativa modulistica grafica**

In Mexal, ad esempio, sarà necessario portarsi all'interno del menu
"**Servizi -- Personalizzazioni -- Modulistica documenti grafica**",
selezionare la sigla del documento interessato (es OC) e cliccare sul
pulsante "Invio" aprendo così l'editor di modifica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stampe_grafiche_mexal.bmp](./assets/media/image714.png)

Sarà quindi necessario inserire all'interno dell'elemento **"Riga
Descrittiva**" l'espressione che consente di non stampare, nel relativo
documento, le righe di tipo nota che iniziano con determinati caratteri.

Considerando, ad esempio, i caratteri utilizzati a default per marcare
queste note, l'espressione da inserire sarà la seguente:

**IIF(LEFT\$(\_mmdee,2)=\"#@\",\"\",\_mmdee)**

In questo modo nella stampa del documento le righe relative a note che
iniziano con i caratteri "#@" verranno sostituite da righe vuote.

Volendo poi è possibile migliorare ulteriormente il risultato ottenuto
evitando anche di stampare eventuali righe vuote.

Per far questo sarà necessario effettuare un doppio clic sul testo "Riga
Descrittiva" e selezionare all'interno della successiva maschera
"Proprietà sezione" il parametro "**No stampa righe non valorizzate**"

Per maggiori informazioni relativamente alla gestione della modulistica
grafica si rimanda ai manuali dei relativi prodotti.

