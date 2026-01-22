# DEFINIZIONE DEGLI ATTRIBUTI DI DEFAULT



Come evidenziato nel precedente capitolo di questo manuale un Tema altro
non è se non un insieme di Attributi mappati ciascuno con uno specifico
elemento (come può essere ad esempio un colore o un'immagine) che potrà
poi essere utilizzato all'interno del sito in fase di costruzione e
personalizzazione delle varie pagine web.

La prima cosa da fare, nel processo di creazione di un Tema, sarà dunque
quella di stabilire quali elementi dovranno essere trattati all'interno
del sito come Attributi del Tema e, ovviamente, quale dovrà essere il
loro valore di Default, ossia il valore che questi stessi Attributi
dovranno assumere, se utilizzati all'interno del sito, nel momento in
cui non dovesse essere applicato alcun Tema.

**ATTENZIONE! La creazione degli Attributi di Default potrebbe essere
fatta anche a posteriori, una volta completata cioè la realizzazione
dell'intero sito in maniera tale da "temizzare" anche quei siti nati
inizialmente senza il concetto dei Temi.**

**In questo caso sarà però necessario tornare poi, ad esempio, in ogni
singola proprietà CSS che si vuole rendere variabile in base al Tema e
sostituire al valore per essa impostato il relativo Attributo di
Default.**

Per definire gli Attributi di Default è necessario cliccare innanzitutto
sul pulsante "**Temi**" presente nel menu di "Editing Sito". In questo
modo verrà infatti visualizzato, immediatamente a fianco del menu di
Editing, un ulteriore box

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_editing_gestione_temi.bmp](./assets/media/image326.png){width="5.9631944444444445in"
height="3.4784722222222224in"}

all'interno del quale il campo:

- **Tema Selezionato**: consente di visualizzare e/o modificare
  selezionandolo dall'apposito menu a tendina il Tema attualmente
  applicato al sito

- **Gestisci Temi**: consente, se cliccato, di accedere alla sezione di
  creazione e gestione dei Temi.

Cliccando dunque su quest'ultimo pulsante verrà visualizzata la maschera
di "**Gestione Temi"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_3_res.bmp](./assets/media/image327.png){width="6.558333333333334in"
height="3.4784722222222224in"}

suddivisa in due distinte sezioni:

- **Attributi di Default**: consente di visualizzare e gestire l'insieme
  degli Attributi di Default che potranno poi essere utilizzati in fase
  di realizzazione e personalizzazione delle varie pagine web

- **Temi**: consente di creare nuovi Temi e/o di gestire quelli già
  realizzati

Dovendo ora definire dei nuovi Attributi di Default sarà quindi
necessario portarsi nella relativa sezione, cliccare sul pulsante
"**Nuovo Attributo**" presente nella contestuale barra degli strumenti,
e nella successiva maschera indicare un valore per i seguenti campi:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_4_res.bmp](./assets/media/image328.png){width="4.582638888888889in"
height="1.0430555555555556in"}

- **Nome Attributo:** consente di assegnare un nome allo specifico
  Attributo che si sta realizzando

- **Valore di default:** consente di assegnare all'Attributo che si sta
  realizzando il suo valore di Default.

Nel caso in cui l'Attributo dovesse essere utilizzato per mappare uno
specifico colore è possibile indicare il relativo codice (esadecimale o
rgb) in maniera manuale oppure selezionandolo dal picker visualizzabile
cliccando sul pulsante "**Seleziona Colore**"

Allo stesso modo nel momento in cui l'Attributo dovesse essere
utilizzato per mappare una specifica immagine il pulsante "**Seleziona
Risorsa**" permetterà di accedere direttamente alla sezione "**Gestione
Risorse**" del Sito in maniera tale da poter individuare più facilmente
la risorsa desiderata (ed il relativo percorso che verrà poi inserito
all'interno del campo "Valore di Default").

**ATTENZIONE! Per non compromettere la corretta visualizzazione del sito
il valore di default assegnato ad un Attributo deve essere coerente con
il tipo di Attributo in questione.**

**In questo senso si consiglia quindi di utilizzare sempre i relativi
pulsanti "Seleziona Colore" e "Seleziona Immagine"**

Una volta assegnato un nome all'Attributo e definito per esso il suo
valore di Default, il pulsante "**Inserisci**" presente nella parte alta
della maschera consentirà di salvarlo e di inserirlo nell'elenco
presente all'interno della sezione "Attributi di Default"

I pulsanti presenti nella barra degli strumenti di questa sezione
consentiranno rispettivamente di:

**Nuovo Attributo** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo_attributo_tema_res.bmp](./assets/media/image329.png){width="0.6194444444444445in"
height="0.17777777777777778in"} ): consente di creare un nuovo Attributo
di Default

**Modifica Attributo** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_attributo_tema_res.bmp](./assets/media/image330.png){width="0.68125in"
height="0.17777777777777778in"} ): consente di modificare l'Attributo di
Default attualmente selezionato in elenco

**ATTENZIONE! Una volta creato e definito un Attributo sarà poi
possibile modificare il valore di Default ad esso associato ma non il
suo nome**

**Elimina Attributo** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_attributo_tema_res.bmp](./assets/media/image331.png){width="0.6444444444444445in"
height="0.1840277777777778in"} ): Consente di eliminare l'Attributo
attualmente selezionato in elenco.

**ATTENZIONE! Nel momento in cui si dovesse decidere di eliminare un
Attributo sarà necessario, per ovvie ragioni, indicare anche uno
specifico valore da utilizzare laddove era stato precedentemente
inserito l'Attributo che si intende eliminare.**

Cliccando su questo pulsante verrà quindi visualizzata la sezione
"**Elimina Attributo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_8_res.bmp](./assets/media/image332.png){width="4.588888888888889in"
height="1.4659722222222222in"}

all'interno della quale il campo:

- **Sostituisci con:** consente di indicare manualmente il valore che
  dovrà essere sostituito all'interno del sito laddove era stato
  precedentemente utilizzato l'Attributo che ora si intende eliminare.

- **Sostituisci con Attributo:** consente di sostituire l'Attributo che
  si intende eliminare con uno degli altri Attributi gestiti
  selezionandolo dall'apposito menu a tendina.

**ATTENZIONE! Per non compromettere la corretta visualizzazione del sito
la sostituzione deve essere ovviamente coerente con il tipo di Attributo
che si intende eliminare**

Nel caso in cui si intenda dunque eliminare un Attributo utilizzato per
mappare un colore questo dovrà essere sostituito o con un altro
Attributo dello stesso tipo oppure con un codice colore valido.

Allo stesso modo nel momento in cui si dovesse decidere di eliminare un
Attributo precedentemente utilizzato per mappare un'Immagine, questo
dovrà essere sostituito con un altro Attributo dello stesso tipo o con
il percorso di un'immagine effettivamente gestita all'interno del sito
stesso.

**In questo senso, e per non compromettere la corretta visualizzazione
del sito, si consiglia quindi di utilizzare i relativi pulsanti
"Seleziona Colore" e "Seleziona Risorsa"**

**Applica Default** (
![Videate\\pulsante_applica_default_tema.bmp](./assets/media/image333.png){width="0.5763888888888888in"
height="0.14097222222222222in"} ): consente di applicare a tutti gli
Attributi utilizzati all'interno del sito il loro valore di Default
deselezionando, di fatto, un eventuale Tema precedentemente impostato.

