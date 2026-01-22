# ORDINI CON OPZIONI DI PERSONALIZZAZIONE ARTICOLO



Alla conferma dell'ordine i valori selezionati dall'utente relativamente
alle opzioni di personalizzazione dei vari articoli verranno inseriti
nelle mail gestite in automatico da Passweb oltre che, ovviamente, nel
relativo documento gestionale.

Nello specifico per poter garantire una corretta gestione, anche lato
Mexal / Ho.Re.Ca. delle opzioni di personalizzazione, queste verranno
riportate **tramite apposite note di riga, precedute, a default, dai
caratteri "##"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\custom_option_ordine.bmp](./assets/media/image658.png){width="5.969444444444444in"
height="2.8958333333333335in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\custom_option_ordine_retail.bmp](./assets/media/image659.png){width="4.472222222222222in"
height="2.9694444444444446in"}

Volendo è anche possibile indicare una serie di caratteri differenti da
anteporre alle note di riga utilizzate per gestire le opzioni di
personalizzazione agendo, in questo senso, mediante il parametro
"**Prefisso Opzioni Articolo**" presente alla pagina "Configurazione
Ordini" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordini_prefisso_opzioni.bmp](./assets/media/image660.png){width="5.6194444444444445in"
height="3.423611111111111in"}

**ATTENZIONE! E' di fondamentale importanza non variare in alcun modo
sul gestionale le informazioni contenute nelle note relative alle
opzioni di personalizzazione degli articoli**

La forma e la struttura di tali note è infatti indispensabile, in fase
di rilettura del documento, per poter mantenere anche sulla versione web
di documenti evasi e/o modificati le stesse opzioni di personalizzazione
presenti nel documento sorgente.

Nel momento in cui all'interno del gestionale si dovessero variare le
note relative alle opzioni di personalizzazione degli articoli, quando
poi l'ordine verrà riportato su Passweb (a seguito ad esempio della sua
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\stampe_grafiche_mexal.bmp](./assets/media/image661.png){width="5.214583333333334in"
height="2.748611111111111in"}

Sarà quindi necessario inserire all'interno dell'elemento **"Riga
Descrittiva**" l'espressione che consente di non stampare, nel relativo
documento, le righe di tipo nota che iniziano con determinati caratteri.

Considerando, ad esempio, i caratteri utilizzati a default per marcare
queste note, l'espressione da inserire sarà la seguente:

**IIF(LEFT\$(\_mmdee,2)=\"##\",\"\",\_mmdee)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\stampe_grafiche_mexal2.bmp](./assets/media/image662.png){width="5.214583333333334in"
height="2.748611111111111in"}

In questo modo nella stampa del documento le righe relative a note che
iniziano con i caratteri "##" verranno sostituite da righe vuote.

Volendo poi è possibile migliorare ulteriormente il risultato ottenuto
evitando anche di stampare eventuali righe vuote.

Per far questo sarà necessario effettuare un doppio clic sul testo "Riga
Descrittiva" e selezionare all'interno della successiva maschera
"Proprietà sezione" il parametro "**No stampa righe non valorizzate**"

![Videate\\stampe_grafiche_mexal2.bmp](./assets/media/image663.png){width="5.214583333333334in"
height="2.748611111111111in"}

Per maggiori informazioni relativamente alla gestione della modulistica
grafica si rimanda ai manuali dei relativi prodotti.

