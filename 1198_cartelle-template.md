# CARTELLE TEMPLATE



Le "**Cartelle Template**" sono quelle identificate all'interno
dell'albero dall'icona colorata di blu e:

![](./assets/media/image87.png)

- **possono essere create e gestite unicamente** **da utenti di tipo
  COMMERCIALISTA**

- **possono essere create soltanto a livello 0 ossia come cartelle
  figlie della radice "Documenti"**

**Un Template, di base, altro non è se non una struttura di cartelle che
verrà poi automaticamente replicata per tutti gli utenti di tipo AZIENDA
visibili dall'utente COMMERCIALISTA e collocati quindi ad un più basso
livello della sua gerarchia**.

Per creare questo tipo di cartelle sarà necessario, per prima cosa,
selezionare la radice "**Documenti**" e cliccare poi sul pulsante di
creazione di una Nuova Cartella, esattamente allo stesso modo di quanto
si farebbe nel momento in cui l'esigenza dovesse essere quella di creare
una nuova cartella Standard.

In questo caso però, essendo l'utente in questione di tipo
COMMERCIALISTA, ed essendo la nuova cartella creata a livello 0 nella
sua maschera di creazione sarà presente anche il parametro
"**Prototipo**"

![Videate\\area_riservata_documenti_crea_template_passcomm.bmp](./assets/media/image88.png)

Selezionando tale parametro verrà automaticamente nascosta la sezione
"Utenti e Gruppi" e, di fatto, scomparirà quindi la possibilità di
definire i possibili utenti da associare alla cartella stessa. In queste
condizioni sarà poi l'applicazione a preoccuparsi di creare in
automatico tutte le cartelle derivanti dal Template associandogli anche
i relativi utenti e permessi.

In particolare, nel momento in cui dovessimo poi andare a creare una
nuova cartella all'interno di una cartella di tipo Template, al
salvataggio l'applicazione si preoccuperà di verificare la presenza di
utenti di tipo AZIENDA che l'utente COMMERCIALISTA attualmente loggato è
in grado di gestire e, nel caso, replicherà per ognuno di essi la stessa
struttura di cartelle presente all'interno della cartella Template
creando anche, se necessario, una prima cartella padre di tipo Azienda
con nome **"Sigla Azienda -- Ragione Sociale"**, per utenti Passcom di
tipo AZIENDA, oppure con nome **"Nome Utente"** per utenti NON Passcom
di tipo AZIENDA.

**ATTENZIONE!** **le cartelle di tipo Template possono essere create
soltanto al primo livello della struttura ossia immediatamente al di
sotto del livello "Documenti". La propagazione della struttura di
cartelle presenti nel Template verso le altre cartelle di tipo Azienda
avrà origine solamente nel momento in cui verranno create nuove sotto
cartelle della cartella Template.**

Mentre le cartelle di tipo Template sono proprietarie dello specifico
utente che le ha create, e potranno quindi essere gestite ed
eventualmente modificate solamente da lui, **le cartelle di tipo Azienda
originate da un Template saranno visibili ed accessibili, oltre che dai
rispettivi utenti ad esse associati dall'applicazione, anche da tutti
gli utenti collocati, nella struttura gerarchia dei gruppi, ad un
livello superiore rispetto a quello in cui si trovano i rispettivi
utenti di tipo AZIENDA**.

Inserendo quindi all'interno di una cartella di tipo Template delle
nuove sottocartelle, queste verranno automaticamente aggiunte anche
all'interno delle relative cartelle di tipo Azienda. **Lo stesso
discorso non vale per i documenti che, ovviamente, non dovranno essere
inseriti all'interno delle cartelle di tipo Template ma bensì
all'interno delle corrispondenti cartelle di tipo Azienda**.

In effetti mentre la struttura delle cartelle deve essere la stessa per
tutte le Cartelle Azienda, i documenti in esse presenti, generalmente
saranno diversi per ogni singolo utente.

Volendo è possibile creare cartelle template anche partendo da un
archivio compresso (file .zip) appositamente creato operando, in questo
senso, esattamente allo stesso modo di come si farebbe per le cartelle
Standard

Se successivamente alla creazione di una cartella di tipo Template,
dovesse essere aggiunto un nuovo utente di tipo AZIENDA, tra quelli
gestibili dal creatore della cartella Template, verrebbe automaticamente
creata anche per esso la relativa cartella di tipo Azienda con
all'interno la stessa struttura di cartelle presenti nella cartella di
tipo Template.

**ATTENZIONE! Nel caso in cui l'utente di tipo COMMERCIALISTA decida di
eliminare una o più cartelle presenti all'interno della cartella di tipo
Template, verranno automaticamente eliminate anche le relative cartelle
di tipo Azienda e gli eventuali documenti in esse contenuti.**

**ATTENZIONE:** non è possibile eliminare una cartella di tipo Template
se al suo interno sono presenti delle sotto cartelle

Infine, selezionando la radice di un Template, si abiliterà nella barra
degli strumenti il pulsante **Copia Template**
(![Videate\\ar_pulsante_copia_template_passcom.bmp](./assets/media/image89.png) )

**Copia Template**
(![Videate\\ar_pulsante_copia_template_passcom.bmp](./assets/media/image89.png) ): consente di effettuare una copia
integrale della struttura di cartelle presenti nel Template attualmente
selezionato.

> **NOTA BENE:** questo pulsante verrà abilitato solo ed esclusivamente
> nel caso in cui sia stata selezionata la cartella radice di un
> Template

Cliccando dunque su questo pulsante **oltre a replicare l'intera
struttura del template verranno create anche le relative cartelle
Aziendali** (proprio come se fosse creato da zero un nuovo Template)
assegnando, al primo livello, lo stesso nome della cartella originaria
con in più il prefisso "copia".

In ogni caso il nome di ogni singola cartella Template potrà poi essere
modificato selezionando la cartella stessa e cliccando sul pulsante
"Proprietà" presente nella barra degli strumenti.

