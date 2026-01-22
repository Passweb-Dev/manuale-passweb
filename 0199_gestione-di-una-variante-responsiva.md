# GESTIONE DI UNA VARIANTE RESPONSIVA



Nel momento in cui l'esigenza dovesse essere quella di gestire le
proprietà e i parametri di configurazione di una Variante Responsiva
sarà necessario accedere alla maschera "**Gestione Varianti**" cliccando
per questo sul pulsante **Gestione Varianti**
(![Videate\\pulsante_gestione_varianti_me.bmp](./assets/media/image8.png){width="0.8208333333333333in"
height="0.26875in"} ) presente nel menu di Editing del Sito o, in
alternativa, sul corrispondente pulsante presente nella Barra degli
Strumenti del Live Editing
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\barra_strumenti_gestione_varianti.bmp](./assets/media/image2.png){width="0.34305555555555556in"
height="0.2013888888888889in"})

Una volta effettuato l'accesso a questa maschera troveremo infatti,
nella parte destra, l'elenco delle Varianti Sito attualmente codificate
e gestite all'interno del proprio ambiente di sviluppo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_4_res.bmp](./assets/media/image9.png){width="4.410416666666666in"
height="2.0520833333333335in"}

Per ogni Variante Sito gestita è indicato:

- il suo Codice identificativo

- il suo Colore identificativo

- se la Variante è Online (colore di sfondo verde chiaro)

- il suo Nome descrittivo

- il codice del Layout di Sito ad essa associato

- il numero di Pagine presenti nella Variante

Selezionando una specifica Variante tra quelle presenti in elenco
verranno visualizzati, nella barra degli strumenti, una serie di
pulsanti identificativi delle varie azioni che potranno essere
effettuate sulla Variante stessa.

Nello specifico il pulsante:

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image10.png){width="0.3506944444444444in"
height="0.18680555555555556in"} ): consente di eliminare la Variante
Sito attualmente selezionata in elenco. **Non è possibile eliminare la
Variante Sito attualmente Online**.

> **NOTA BENE:** l'eliminazione di una Variante Sito NON comporta
> l'automatica eliminazione delle risorse grafiche utilizzate per la
> creazione della Variante stessa, risorse queste che potrebbero, in
> effetti, essere in comune anche ad altre Varianti ancora gestite.

Per eliminare quindi eventuali risorse grafiche utilizzate solo ed
esclusivamente per una specifica Variante non più gestita, recuperando
così spazio disco, sarà necessario agire manualmente dalla sezione
"Gestione Risorse del Sito"

**Copia** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_copia.bmp](./assets/media/image11.png){width="0.32083333333333336in"
height="0.18680555555555556in"} ): consente di effettuare una copia
della Variante Sito attualmente selezionata in elenco.

In fase di copia, prima dell'avvio della procedura, verrà visualizzata
una maschera all'interno della quale poter indicare:

![Videate\\copia_variante_cartella_destinazione_res.bmp](./assets/media/image12.png){width="5.627083333333333in"
height="1.5298611111111111in"}

- **Cartella:** consente di indicare una specifica cartella in cui
  verranno eventualmente copiate tutte le risorse utilizzate dalla
  variante di origine.

> **ATTENZIONE!** nel caso in cui non dovesse essere indicata nessuna
> cartella all'interno del campo in esame, **la variante di origine e
> quella di copia condivideranno, ovviamente, le stesse risorse**.

- **Non considerare le pagine di categoria (se hanno la stessa
  grafica):** consente di decidere se, in fase di copia della Variante,
  dovrà essere considerata o meno ogni singola pagina di Categoria e
  ogni singola pagina Prodotto con la relativa grafica e i relativi
  componenti

> In particolare nel caso in cui il parametro in oggetto dovesse essere:

- **Deselezionato**: in fase di copia verrà considerata ogni singola
  pagina Prodotto e ogni singola pagina di Categoria presente nella
  Variante di origine con la relativa grafica e i relativi componenti.
  **Questa configurazione dovrebbe quindi essere presa in considerazione
  solo nel caso in cui nella Variante sorgente dovessero essere
  effettivamente gestiti componenti o grafiche diverse per le diverse
  pagine di Categoria o per le diverse pagine Prodotto**

> **ATTENZIONE!** In queste condizioni l'operazione di copia impiegherà
> più tempo e, nel momento in cui la Variante sorgente dovesse avere un
> numero di pagine particolarmente elevato (dell'ordine delle migliaia)
> l'operazione di copia potrebbe anche dare dei problemi

- **Selezionato**: in fase di copia verranno considerate nella Variante
  sorgente, per quel che riguarda le pagine di categoria soltanto la
  pagina "Negozio" e per quel che riguarda le pagine Prodotto solo la
  pagina Prodotto "generica". In conseguenza di ciò nella Variante di
  copia tutte le pagine di Categoria si ritroveranno ad avere la stessa
  grafica e gli stessi componenti della pagina Negozio e, allo stesso
  modo, tutte le pagine Prodotto si ritroveranno ad avere la stessa
  grafica e gli stessi componenti della pagina Prodotto "generica".

> Va da se che tale opzione dovrebbe quindi essere presa in
> considerazione nel caso in cui nella Variante sorgente si sia deciso
> di utilizzare per tutte le pagine di categoria la stessa grafica e gli
> stessi componenti della pagina Negozio e per tutte le pagine Prodotto
> la stessa grafica e gli stessi componenti presenti anche nella pagina
> Prodotto "generica"
>
> **ATTENZIONE!** In queste condizioni l'operazione di copia sarà molto
> più veloce.

**Accedi Wizard** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_accedi_variante_res.bmp](./assets/media/image13.png){width="0.6194444444444445in"
height="0.2013888888888889in"} ): consente di caricare all'interno del
proprio ambiente di sviluppo la Variante Sito attualmente selezionata in
elenco in modo tale da poterne gestire struttura, grafica e contenuti
utilizzando per questo i normali strumenti messi a disposizione dal
Wizard di Passweb.

> **NOTA BENE:** la Variante Sito caricata all'interno del proprio
> ambiente di sviluppo non deve necessariamente coincidere con quella
> attualmente pubblicata (Variante Sito online)

**Accedi Sito** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_accedi_da_sito_res.bmp](./assets/media/image14.png){width="0.5145833333333333in"
height="0.2013888888888889in"} ): consente di visualizzare lato
front-end, come sarebbe dunque per un normale visitatore del sito, la
Variante attualmente selezionata, senza però portarla Online.

Cliccando su questo pulsante verrà infatti aperta una nuova finestra del
browser all'interno della quale verrà caricata la Variante sito
selezionata in elenco in maniera tale da poter avere un'idea chiara di
quello che sarebbe il risultato finale nel momento in cui questa stessa
Variante dovesse effettivamente essere portata Online.

Per poter ottenere questo risultato verranno opportunamente settate da
Passweb tutte le variabili di sessione del browser necessarie per poter
effettivamente simulare quello che sarebbe il risultato finale. In
queste condizioni dunque anche dopo aver chiuso la finestra del browser
aperta automaticamente da Passweb, se si tentasse di aprire manualmente,
sullo stesso PC e con lo stesso browser, il sito, quello che verrebbe
visualizzato sarebbe ancora la Variante offline precedentemente
selezionata che, generalmente, non coincide con quella effettivamente
Online.

> **NOTA BENE:** il pulsante "Accedi da Sito" si limita soltanto a
> **simulare** quello che sarebbe il risultato finale nel momento in cui
> la Variante selezionata dovesse essere portata Online.

Per evitare quindi di fare confusione all'utente tra Variante online e
offline, verrà visualizzato, nella parte basse del browser un piccolo
banner per indicare in maniera esplicita che quella che si sta
attualmente visualizzando è una Variante offline.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_offline.bmp](./assets/media/image15.png){width="5.514583333333333in"
height="3.2465277777777777in"}

Nel momento in cui l'esigenza dovesse essere quella di tornare a
visualizzare la Variante Online sarà quindi necessario effettuare una
delle azioni di seguito indicate:

- Aprire il sito con un altro browser

- Attendere lo scadere della sessione del browser precedentemente
  utilizzato

- Cliccare nuovamente sul pulsante "Accedi Sito" dopo aver selezionato
  la Variante Online

- Chiudere il browser pulire la cache (facendo attenzione a selezionare
  anche l'opzione che prevede di eliminare anche i cookie) e solo a
  questo punto aprire nuovamente il sito

**Link Variante** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_link_variante.bmp](./assets/media/image16.png){width="0.5597222222222222in"
height="0.2013888888888889in"} ): visibile solo nel caso in cui la
Variante selezionata in elenco non sia quella online.

Consente di generare e copiare in clipboard il link di visualizzazione
della variante attualmente selezionata in elenco (analogo al pulsante
"Accedi Sito").

Tale link potrà poi essere fornito ad eventuali utenti che dovessero
avere la necessità di visualizzare lato front end una determinata
Variante offline ma che, per una qualche ragione, non possono accedere
al Wizard ed utilizzare, in questo senso, il pulsante "Accedi Sito"
precedentemente analizzato

**ATTENZIONE! Il link generato mediante il pulsante in esame ha una
validità massima di 24 ore**

In conseguenza di ciò nel momento in cui il link in questione dovesse
essere utilizzato dopo 24 ore dalla sua generazione, non consentirà più
di accedere alla visualizzazione della Variante offline per cui è stato
generato

**Online** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_online_variante_res.bmp](./assets/media/image17.png){width="0.35833333333333334in"
height="0.20902777777777778in"} ): consente di portare online e quindi
di pubblicare a tutti gli effetti la Variante Sito attualmente
selezionata in elenco.

Nel momento in cui dunque una specifica Variante dovesse essere portata
online la Variante Sito che fino a quel momento era nello stato Online
verrà automaticamente posta Offline e al pari delle altre Varianti che
si trovano in questo stato potrà essere visualizzata e gestita solo ed
esclusivamente all'interno del proprio ambiente di sviluppo.

Le Varianti Sito attualmente online verranno visualizzate nella parte
alta dell'elenco e saranno evidenziate in verde

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_11_res.bmp](./assets/media/image18.png){width="5.097222222222222in"
height="2.477777777777778in"}

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image19.png){width="0.3958333333333333in"
height="0.18680555555555556in"} ): consente di accedere all'anagrafica
della Variante Sito attualmente selezionata in elenco. Cliccando su
questo pulsante verrà visualizzata la maschera "**Modifica Variante
Sito**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_6_res.bmp](./assets/media/image20.png){width="6.627083333333333in"
height="4.059722222222222in"}

all'interno della quale oltre a poter variare, eventualmente, i
parametri impostati in fase di creazione della Variante stessa, sarà
possibile impostare anche altri parametri fondamentali per un corretto
funzionamento del sito.

Per maggiori informazioni in merito si vedano i successivi capitoli di
questo manuale.

**NOTA BENE:** i parametri presenti all'interno della maschera
"**Modifica Variante Sito**" sono riferiti, ovviamente, alla Variante
Sito attualmente selezionata e come tali verranno quindi applicati solo
ed esclusivamente nel momento in cui la Variante stessa verrà
effettivamente portata on line

