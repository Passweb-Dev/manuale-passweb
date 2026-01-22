# GESTIONE LINEE ARTICOLO



La funzionalità **"Gestione linee articolo"** consente di attivare una
particolare modalità di gestione a seguito della quale articoli
appartenenti a linee diverse genereranno ordini distinti (uno per ogni
linea articolo presente in carrello).

Per poter attivare questa particolare modalità di gestione sarà
necessario, per prima cosa, codificare le diverse Linee Articolo cui
dovranno poi essere associati i vari prodotti agendo, per questo, dalla
sezione "**Catalogo -- Gestione Articoli -- Linee**" del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_linee_articolo.bmp](./assets/media/image133.png)

Per maggiori informazioni in merito a come poter codificare una nuova
linea articolo si veda anche la sezione *"Catalogo -- Gestione Articoli
Linee Articolo"* di questo manuale

Una volta codificate tali linee sarà poi necessario portarsi nell'
Anagrafica Passweb (sezione "Informazioni Generali") dell'articolo che
si vuol associare ad una specifica linea e in corrispondenza del campo
**Gestione Linee Articolo** selezionare dal box di sinistra la linea
desiderata e inserirla nel box di destra cliccando per questo sul
pulsante raffigurante una piccola freccia verde rivolta verso destra.

Una volta attivata questa particolare modalità di gestione, all'interno
del sito, in fase di acquisto, **un utente avrà la possibilità di
inserire in carrello anche articoli appartenenti a linee differenti;
confermando il carrello l'applicazione si preoccuperà poi di verificare
l'appartenenza o meno di ogni singolo articolo ad una specifica linea e
di generare, conseguentemente, un distinto ordine per ogni singola linea
presente in carrello.**

In particolare, in fase di conferma ordine, verrà visualizzato,
immediatamente al di sopra dei vari step necessari per la conferma del
documento, l'elenco delle linee presenti.

Cliccando sull'etichetta identificativa di una specifica linea l'utente
avrà quindi la possibilità di confermare il documento contenente solo
gli articoli appartenenti a quella specifica linea. Alla conferma
dell'ordine, se sono presenti altre linee, l'utente verrà riportato
nuovamente alla pagina di checkout per procedere con l'ordine relativo
alla linea successiva.

Nel caso in cui tutti gli articoli presenti in carrello appartengano
dunque ad una specifica linea l'applicazione si preoccuperà di generare
ordini distinti, uno per ogni singola linea, suddividendo gli articoli,
per ogni singolo ordine, in maniera del tutto automatica.

Nel caso in cui, invece, vengano inseriti in carrello, assieme ad
articoli appartenenti ad una specifica linea, anche articoli non
appartenenti a nessuna linea o articoli appartenenti contemporaneamente
a più linee, l'applicazione si preoccuperà, anche questa volta, di
suddividere automaticamente gli articoli nei diversi ordini con
l'obbiettivo, inoltre, di generare il minor numero possibile di
documenti.

In questo senso verrà quindi applicata la seguente logica:

- verranno ordinate, per prima cosa, le varie linee in base al numero di
  articoli (tra quelli presenti in carrello) appartenenti alla specifica
  linea. **Nel caso in cui ci siano più linee con lo stesso numero di
  articoli tali linee verranno ordinate per codice linea**;

- dopo aver ordinato le varie linee l'applicazione si preoccuperà di
  predisporre un primo documento per la prima linea in elenco.
  All'interno di questo documento verranno inseriti tutti gli articoli
  presenti in carrello appartenenti a quella specifica linea,
  indipendentemente dal fatto che tali articoli appartengano,
  eventualmente, anche ad altre linee;

- verrà, a questo punto, analizzata la seconda linea in elenco e, nel
  caso in cui tra gli articoli rimasti in carrello, ci siano ancora
  articoli appartenenti a tale linea, verrà predisposto un documento
  anche per essa. Anche in questo caso all'interno di questo documento
  verranno inseriti gli articoli appartenenti alla specifica linea,
  indipendentemente dal fatto che appartengano, eventualmente, anche ad
  altre linee. Nel caso in cui invece, tra quelli rimasti in carrello
  non ci siano più articoli appartenenti alla linea in esame (perché ad
  esempio tali articoli appartenevano anche alla linea precedente e sono
  quindi già stati inseriti all'interno del primo documento), per essa
  non verrà predisposto nessun documento e l'applicazione passerà a
  processare, seconda la stessa logica, la successiva linea in elenco;

- gli articoli presenti in carrello e non appartenenti a nessuna linea
  verranno automaticamente inseriti dall'applicazione all'interno
  dell'ordine con il maggior numero di articoli.

Un'altra cosa di fondamentale importanza da tenere in considerazione,
riguarda poi l'utilizzo delle linee articolo in relazione a promozioni
che prevedono l'aggiunta di articoli in carrello.

In questo senso, infatti, occorre ricordare che **inizialmente**, **in
fase di suddivisione degli articoli nei singoli ordini (determinati
dalle linee articolo) non verranno considerati i prodotti che sono stati
aggiunti al carrello a seguito dell'applicazione di eventuali
promozioni.**

**ATTENZIONE!** Questo non significa però che eventuali promozioni che
prevedono l'aggiunta di articoli in carrello siano incompatibili con
l'utilizzo delle linee articolo.

**Tali promozioni infatti verranno rivalutate ed applicate solo dopo che
l'ordine iniziale sarà stato splittato nei singoli documenti e solo ed
esclusivamente sulla base dei prodotti effettivamente presenti in
ciascuno di essi.**

In questa fase inoltre non verrà presa in considerazione l'appartenenza
degli articoli oggetto della promozione ad eventuali linee, per cui
all'ordine relativo ad una specifica linea potranno tranquillamente
essere aggiunti anche articoli omaggio che non appartengono a quella
stessa linea.

**ATTENZIONE!** Questo tipo di comportamento si rende necessario in
conseguenza del fatto che non esiste nessun vincolo che possa obbligare
in qualche modo l'utente a chiudere tutti i singoli ordini generati a
seguito dell'appartenenza degli articoli in carrello a diverse linee.

In queste condizioni infatti se i prodotti omaggio venissero già
considerati in fase creazione dei singoli ordini secondo la loro
appartenenza ad eventuali linee, potrebbero anche verificarsi casi in
cui l'utente si ritrovi ad usufruire di omaggi che di fatto non gli
spettano in quanto generati da uno degli N ordini prodotti dalle linee
articolo che l'utente stesso potrebbe poi decidere di non portare a
termine.

Per comprendere meglio questa casistica supponiamo che sul sito sia
attiva una promozione che preveda l'aggiunta in omaggio dell' Articolo Y
appartenente alla linea A, nel momento in cui si dovesse decidere di
acquistare l'Articolo X appartenente alla linea B. In queste condizioni
se venisse considerata l'appartenenza alle linee articolo anche dei
prodotti omaggio già in fase di creazione dei singoli documenti si
verrebbero a creare due distinti ordini, uno con l'articolo Y
(appartenente alla linea A) e uno con l'articolo X (appartenente alla
linea B) e l'utente potrebbe benissimo decidere di chiudere solo
l'ordine con l'articolo Y usufruendo di fatto della promozione anche
senza acquistare effettivamente l'articolo X.

La logica applicata da Passweb a questa casistica fa si invece che venga
prodotto un singolo documento (relativo alla linea B) contenente
l'articolo X e l'omaggio a lui legato (articolo Y) indipendentemente dal
fatto che tale omaggio non appartenga alla linea dell'ordine.

Per quel che riguarda i pagamenti, infine, è bene ricordare che in fase
di conferma ordine verranno proposti all'utente i pagamenti associati
alla specifica linea di appartenenza del documento che si sta generando,
più quelli non associati ad alcuna linea.

Nel caso in cui, dunque, l'esigenza sia quella di proporre all'utente
tutte le modalità di pagamento attivate, non andrà creata nessuna
associazione tra le modalità di pagamento e le linee articolo.

> **NOTA BENE:** se associato ad una Linea Articolo, il pagamento
> abituale, verrà gestito esattamente come un qualsiasi altro pagamento,
> e verrà quindi proposto all'utente solo ed esclusivamente nel caso di
> conferma di un ordine per la Linea in questione.

**ATTENZIONE!** nel caso di conferma di un orine con articoli
appartenenti a più linee, e nel caso in cui queste linee siano le stesse
per tutti gli articoli, all'utente verranno proposte tutte le modalità
di pagamento associate a queste linee, oltre, ovviamente, alle modalità
di pagamento non associate ad alcuna linea.

Alcuni esempi chiariscono meglio i concetti espressi fino a questo
momento.

**ESEMPIO 1**

Supponiamo che nel carrello siano presenti i seguenti articoli:

  -----------------------------------------------------------------------
                           **LINEA1**                   **LINEA2**
  ------------- --------------------------------- -----------------------
    **ART1**                    X                 

    **ART2**                    X                            X

    **ART3**                                                 X

    **ART4**                                      

    **ART5**                    X                 
  -----------------------------------------------------------------------

In queste condizioni, seguendo la logica sopra evidenziata,
l'applicazione ordinerà le varie linee presenti in carrello nel seguente
modo:

- LINEA1 (3 articoli)

- LINEA2 (2 articoli)

L'utente, in questo caso, dovrà quindi procedere con la generazione di
due ordini distinti. All'interno del primo ordine, relativo alla LINEA1,
verranno inseriti gli articoli: ART1, ART2, ART4, ART5. All'interno del
secondo ordine, relativo invece alla LINEA2, verrà inserito il solo
articolo ART3.

Nell'elenco dei pagamenti verranno mostrate tutte le modalità associate
alla linea in corso più quelle che non sono assegnate a nessuna linea
(anche il pagamento abituale viene gestito con la stessa logica).

**ESEMPIO 2**

Supponiamo che nel carrello siano presenti i seguenti articoli:

  -----------------------------------------------------------------------
                           **LINEA1**                   **LINEA2**
  ------------- --------------------------------- -----------------------
    **ART1**                    X                            X

    **ART2**                    X                            X
  -----------------------------------------------------------------------

Considerando che, in queste condizioni, le due linee presenti in
carrello contengo entrambe lo stesso numero di articoli, preverrà, tra
esse, l'ordinamento per codice linea.

- LINEA1 (2 articoli)

- LINEA2 (2 articoli)

Verrà quindi generato un solo ordine relativo alla LINEA1 contenente
entrambi gli articoli presenti in carrello.

Nell'elenco dei pagamenti verranno mostrate tutte le modalità associate
alla LINEA1, alla LINEA2 e quelle che non sono assegnate a nessuna linea
(anche il pagamento abituale viene gestito con la stessa logica)

**ESEMPIO 3**

Supponiamo che nel carrello siano presenti i seguenti articoli:

  ---------------------------------------------------------------------------------
                **LINEA1**      **LINEA2**    **LINEA3**   **LINEA4**   **LINEA5**
  ---------- ----------------- ------------- ------------ ------------ ------------
   **ART1**          X               X                                 

   **ART2**          X               X                                 

   **ART3**                                       X            X       

   **ART4**                                       X            X       

   **ART5**                                                                 X
  ---------------------------------------------------------------------------------

In queste condizioni, l'applicazione ordinerà le varie linee presenti in
carrello nel seguente modo:

- LINEA1 (2 articoli)

- LINEA2 (2 articoli)

- LINEA3 (2 articoli)

- LINEA4 (2 articoli)

- LINEA5 (1 articolo)

L'utente dovrà quindi procedere, questa volta, con la generazione di tre
ordini distinti. All'interno del primo ordine, relativo alla LINEA1,
verranno inseriti gli articoli: ART1, ART2. All'interno del secondo
ordine, relativo alla LINEA3, verranno inseriti gli articoli: ART3,
ART4. All'interno del terzo e ultimo ordine, relativo alla LINEA5, verrà
infine inserito il solo articolo ART5.

**Gli articoli ART1 e ART2 vengono associati alla LINEA1 in quanto
questa linea precede alfabeticamente la LINEA2.**

**Gli articoli ART3 e ART4 vengono associati alla LINEA3 in quanto
questa linea precede alfabeticamente la LINEA4.**

I pagamenti visualizzati per il primo ordine saranno quelli relativi sia
alla LINEA1 che alla LINEA2, in quanto tutti gli articoli dell'ordine
appartengono ad entrambe le linee, più quelli non appartenenti a nessuna
linea.

I pagamenti visualizzati per il secondo ordine saranno quelli relativi
sia alla LINEA3 che alla LINEA4, in quanto tutti gli articoli
dell'ordine appartengono ad entrambe le linee, più quelli non
appartenenti a nessuna linea.

I pagamenti visualizzati per il terzo ordine saranno quelli relativi
alla LINEA5, più quelli non appartenenti a nessuna linea.

