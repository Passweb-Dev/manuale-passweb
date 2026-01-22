# COMPONENTI E-COMMERCE -- IMMAGINE RAPPRESENTATIVA (IMMAGINI DELLA SCHEDA PRODOTTO)



Nel caso in cui il Componente Ecommerce **"Immagine Rappresentativa"**
venga inserito all'interno del Componente di primo livello **"Scheda
Prodotto"** questo consentirà di visualizzare, attraverso un'apposita
galleria, tutte le immagini (Principale e Secondarie) associate allo
specifico articolo.

Volendo sarà anche possibile attivare un effetto di zoom sull'immagine
attualmente visualizzata come immagine principale della galleria.

In relazione alle immagini associate ad ogni singolo prodotto presente
all'interno del sito va ricordato che queste possono essere gestite in
maniera differente a seconda del fatto di considerare siti collegati a
Mexal oppure ad uno dei gestionali Ho.Re.Ca.

**[SITI ECOMMERCE COLLEGATI A MEXAL]{.underline}**

In questo caso se l' "Immagine del Catalogo" dovesse essere gestita
direttamente nell'anagrafica gestionale dello specifico articolo,
allora:

- l' **Immagine Principale** della Scheda Prodotto corrisponderà
  all'Immagine associata in Docuvision allo specifico articolo con
  progressivo uguale a 1

- le **Immagini Secondarie** della Scheda Prodotto corrisponderanno
  invece alle immagini associate in Docuvision allo specifico articolo
  con progressivo maggiore di 1

Nel caso in cui, invece l' "Immagine del Catalogo" sia gestita,
anch'essa, attraverso Docuvision, allora:

- l'**Immagine Principale** della Scheda Prodotto corrisponderà
  all'Immagine associata in Docuvision allo specifico articolo con
  progressivo uguale a 2

- le **Immagini Secondarie** della Scheda Prodotto corrisponderanno
  invece alle immagini associate in Docuvision allo specifico articolo e
  con progressivo maggiore di 2

> **NOTA BENE:** per maggiori informazioni relativamente
> all'associazione dell'Immagine principale e delle Immagini secondarie
> della Scheda Prodotto allo specifico articolo, si rimanda al relativo
> capitolo di questo manuale.

**[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI
HO.RE.CA.]{.underline}**

In queste condizioni l'immagine principale della Scheda Prodotto potrà
essere associata allo specifico articolo, operando direttamente
all'interno del gestionale, unicamente attraverso il campo "Allegato".

Infine, indipendentemente dal tipo di gestionale considerato, nel
momento in cui ad un determinato articolo non dovesse essere associata
nessuna immagine (né tramite l'anagrafica dell'articolo stesso, né
tramite Docuvision e neppure operando direttamente dal backend di
Passweb), il componente "Immagine" inserito all'interno della scheda
prodotto potrà eventualmente visualizzare l'immagine caricata nel campo
"**Immagine catalogo di Default**" presente all'interno della sezione
"*Catalogo - Configurazione Parametri-- Parametri Immagini*" del Wizard

**ATTENZIONE!** Volendo è anche possibile gestire le immagini articolo
direttamente su Passweb caricandole all'interno della corrispondente
sezione del Wizard. Per maggior informazioni in merito si veda anche la
sezione *"Catalogo -- Configurazione Parametri Catalogo -- Gestione
Articoli -- Articoli"* di questo manuale.

Tipicamente la visualizzazione delle immagini articolo all'interno della
scheda prodotto potrebbe essere del tipo di quella evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scheda_prodotto_immagini_esempio.bmp](./assets/media/image467.png)

All'interno della scheda prodotto il Componente "Immagine
Rappresentativa" sarà quindi costituito da:

- Un' **Immagine Principale** le cui dimensioni massime coincidono con
  quelle impostate in corrispondenza del parametro **"Immagine
  principale della Scheda Prodotto",** presente nella maschera "**Lista
  delle tipologie di immagini nel Catalogo**" alla sezione "*Catalogo -
  Configurazione Parametri-- Parametri Immagini*" del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scheda_prodotto_immagini_esempio1.bmp](./assets/media/image468.png)

- una "**Galleria di immagini secondarie**" posizionata all'interno di
  uno Slider a scorrimento orizzontale o verticale, e costituita da
  tante miniature le cui dimensioni massime coincidono con quelle
  impostate per il parametro "**Immagini Secondarie della Scheda
  Prodotto**" presente nella maschera "**Lista delle tipologie di
  immagini nel Catalogo**" alla sezione "*Catalogo - Configurazione
  Parametri-- Parametri Immagini*" del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scheda_prodotto_immagini_esempio2.bmp](./assets/media/image469.png)

**ATTENZIONE! Nel caso in cui sia gestita una sola immagine per un
determinato articolo, verrà comunque creata una Galleria contenente
quest'unica immagine.**

Cliccando su una delle immagini articolo (sia essa l'immagine principale
o una qualsiasi delle immagini secondarie) verrà avviata un animazione
attraverso cui poter visualizzare la galleria delle immagini a schermo
intero.

Volendo, infine, dalla configurazione del componente sarà possibile
anche attivare un effetto di zoom sull'immagine principale della
galleria (per maggiori informazioni in merito alle opzioni di
configurazione del componente si veda il successivo capitolo di questo
manuale)

