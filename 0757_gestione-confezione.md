# GESTIONE CONFEZIONE



La sezione "**Gestione Confezioni**", presente all'interno della
maschera "**Configurazione Catalogo Mexal / Ho.Re.Ca.**" consente di
decidere come dovranno essere gestiti all'interno del sito quelli che,
lato gestionale, sono articoli gestiti a Confezione.

In questo senso è bene ricordare che:

- In Mexal, per poter gestire un articolo a Confezioni è necessario
  impostare il parametro "**Confezione**" presente nella maschera
  "**Altri Dati Anagrafici**" del singolo articolo sul valore
  "**Confezione (=)**" indicando poi nel successivo campo la quantità di
  articoli che dovrà effettivamente essere presente all'interno della
  singola confezione.

![](./assets/media/image14.png)

- Nei gestionali Ho.Re.Ca., per poter gestire un articolo a Confezioni è
  necessario impostare il parametro "**Tipo Confezione**" presente
  all'interno del Tab "**Alias e Fornitori**" dell'anagrafica articolo,
  sul valore "**Confezione**" indicando poi nel successivo campo "**qta.
  conf.**" la quantità di articoli che dovrà effettivamente essere
  presente all'interno della singola confezione

![](./assets/media/image15.png)

Nell'esempio indicato in figura l'articolo in esame verrà venduto
all'interno del gestionale a confezioni di 3 unità ciascuna.

**ATTENZIONE! Tale quantità, comunque, è semplicemente propositiva e
potrà quindi essere modificata secondo le specifiche esigenze
dell'utente.**

In queste condizioni, **lato Passweb,** la quantità effettivamente
acquistabile per l'articolo in esame dipende invece dal fatto che ad
effettuare l'ordine sia un utente Privato oppure un utente di tipo
Azienda e, soprattutto, da come sono stati impostati i relativi
parametri "**Aggiungi al carrello**" presente all'interno della sezione
"**Gestione Confezioni**"

![](./assets/media/image16.png)

Nello specifico dunque, il parametro:

**Aggiungi al Carrello Privati:** consente di decidere come dovranno
essere gestiti sul sito ecommerce, nel caso in cui ad effettuare
l'ordine sia un utente Privato , quelli che all'interno del gestionale
sono articoli a confezione.

**Aggiungi al Carrello Aziende:** consente di decidere come dovranno
essere gestiti sul sito ecommerce, nel caso in cui ad effettuare
l'ordine sia un utente di tipo Azienda, quelli che all'interno del
gestionale sono articoli a confezione.

In entrambi i casi è possibile selezionare uno dei seguenti valori:

- **Quantità Singola:** selezionando questa opzione, lato Passweb,
  l'articolo verrà gestito sempre e comunque come articolo singolo
  indipendentemente dunque dalle eventuali impostazioni settate lato
  gestionale per il campo "Confezione". In queste condizioni inoltre gli
  eventuali pulsanti incrementali (+/-) presenti ad esempio in
  corrispondenza del componente "Aggiungi in carrello" andranno ad
  aumentare / diminuire la quantità indicata sempre e soltanto di un
  unità alla volta

- **Quantità Singola incrementale:** selezionando questa opzione si avrà
  lo stesso comportamento del caso precedente (Quantità Singola) ma con
  una diversa gestione dei pulsanti incrementali (+/-). In questo caso
  infatti tali pulsanti andranno ad aumentare / diminuire la quantità
  del prodotto di un valore pari esattamente a quello indicato per la
  confezione presente sul gestionale

> Supponendo quindi di aver impostato, lato gestionale, nel campo
> relativo alla Confezione il valore 3, l'utente si troverà all'interno
> del sito il campo quantità, presente in corrispondenza del pulsante di
> aggiunta in carrello, impostato inizialmente sul valore 1.
>
> In questo caso però nel momento in cui dovesse cliccare sul pulsante +
> la quantità indicata aumenterà di 3 unità alla volta passando ad
> esempio da 1 a 3, a 6 a 9 ...

- **Quantità Propositiva:** in queste condizioni, lato Passweb,
  l'articolo verrà gestito esattamente come avviene all'interno del
  gestionale. Ciò significa dunque che la quantità indicata inizialmente
  sarà solo propositiva per cui l'utente potrà poi acquistare l'articolo
  desiderato nella quantità da lui scelta. In queste condizioni inoltre
  gli eventuali pulsanti incrementali (+/-) presenti ad esempio in
  corrispondenza del componente "Aggiungi in carrello" andranno ad
  aumentare / diminuire la quantità indicata sempre e soltanto di un
  unità alla volta

> Supponendo quindi di aver impostato, lato gestionale, nel campo
> relativo alla Confezione il valore 3, l'utente si troverà all'interno
> del sito il campo quantità, presente in corrispondenza del pulsante di
> aggiunta in carrello, anch'esso impostato inizialmente sullo stesso
> valore.
>
> L'utente avrà comunque la libertà di modificare tale valore secondo le
> sue specifiche esigenze e potrà quindi acquistare l'articolo in esame
> in quantità 1,2, 3,4, 5 ecc...
>
> Nel momento in cui dovesse cliccare sul pulsante + la quantità
> indicata aumenterà di un'unità alla volta passando ad esempio da 3 a 4
> a5 ...

- **Quantità propositiva incrementale:** selezionando questa opzione si
  avrà lo stesso comportamento del caso precedente (Quantità
  propositiva) ma con una diversa gestione dei pulsanti incrementali
  (+/-). In questo caso infatti tali pulsanti andranno ad aumentare /
  diminuire la quantità del prodotto di un valore pari esattamente a
  quello indicato per la confezione presente sul gestionale.

> Supponendo quindi di aver impostato, lato gestionale, nel campo
> relativo alla Confezione il valore 3, l'utente si troverà ancora una
> volta il campo quantità, presente in corrispondenza del pulsante di
> aggiunta in carrello, anch'esso impostato inizialmente sul valore 3 e
> come prima avrà comunque la libertà di modificare tale valore secondo
> le sue specifiche esigenze.
>
> In questo caso però nel momento in cui dovesse cliccare sul pulsante +
> la quantità indicata aumenterà di 3 unità alla volta passando ad
> esempio da 3 a 6 a 9 ...

- **Quantità Bloccata:** in queste condizioni lato Passweb, l'utente
  avrà l'obbligo di indicare all'interno del campo quantità, presente in
  corrispondenza del pulsante di aggiunta in carrello, una quantità
  multipla della confezione indicata all'interno del gestionale.

> Supponendo quindi di aver impostato, anche in questo caso lato
> gestionale, nel campo relativo alla Confezione il valore 3,
> all'interno del sito l'utente si troverà il campo quantità
> inizialmente valorizzato sullo stesso valore ma, a differenza del caso
> precedente in queste condizioni tale valore potrà essere modificato
> solo ed esclusivamente con un multiplo di 3.
>
> L'articolo potrà quindi essere acquistato solo ed esclusivamente in
> quantità 3, 6, 9, 12, ecc...
>
> Nel caso in cui l'utente dovesse inserire una quantità non ammessa
> (es. 4 o 5) verrà visualizzato un apposito messaggio di errore e
> l'articolo non verrà aggiunto in carrello.

![](./assets/media/image17.png)

> E' possibile personalizzare il messaggio di errore alla sezione
> "Testi/Messaggi Sito" del Wizard selezionando il componente "Aggiunta
> al Carrello" e agendo sul campo "Confezione Bloccata".
>
> **ATTENZIONE!** In queste condizioni i pulsanti incrementali
> eventualmente presenti a fianco del campo quantità aumenteranno e/o
> diminuiranno la quantità dell'articolo di un valore pari alla
> confezione indicata per l'articolo in esame all'interno del gestionale

- **Quantità Bloccata con aggiornamento delle quantità:** anche in
  queste condizioni, come nel caso precedente , l'utente avrà l'obbligo
  di indicare all'interno del campo quantità, presente in corrispondenza
  del pulsante di aggiunta in carrello, una quantità multipla della
  confezione indicata all'interno del gestionale.

> A differenza del caso precedente però, nel momento in cui l'utente
> dovesse inserire una quantità non corretta tale quantità verrebbe
> automaticamente aggiornata **al valore superiore più prossimo a quello
> inserito**.
>
> Supponendo quindi, come nei casi precedenti, di aver impostato lato
> gestionale una confezioni pari a 3, nel momento in cui l'utente
> dovesse tentare di acquistare, sul sito, l'articolo in esame in
> quantità 4, tale quantità verrà automaticamente impostata sul valore
> 6.

**ATTENZIONE!** In fase di verifica della disponibilità articolo,
qualora l'articolo non fosse disponibile e si gestisse la confezione
bloccata (siti ecommerce Mexal), la quantità verrebbe aggiornata in
automatico **al valore inferiore più prossimo a quello disponibile**.

**ATTENZIONE!** Le impostazioni settate per i due parametri sopra
esaminati varranno, a livello globale, per tutti gli articoli gestiti
all'interno del sito come articoli a confezione.

In ogni caso, una volta impostato il comportamento a livello generale,
sarà comunque possibile modificare la gestione a confezioni del singolo
articolo, agendo mediante gli stessi parametri presenti nell'Anagrafica
Passweb dell'articolo stesso

![](./assets/media/image18.png)

In questo caso però è bene ricordare che **le variazioni apportate ai
parametri in oggetto all'interno della sezione "Gestione Confezioni"
della maschera "Configurazione Catalogo" andranno a sovrascrivere
eventuali impostazioni precedentemente settate in maniera specifica per
il singolo articolo (impostazioni queste che dovranno quindi essere,
eventualmente ridefinite)**

**Totale Quantità articoli:** consente di decidere come dovrà essere
gestita la confezione in fase di calcolo della quantità degli articoli
presenti in carrello.

E' possibile selezionare uno dei seguenti valori:

- **Considera le unità in confezione:** selezionando questa opzione in
  fase di calcolo della quantità degli articoli presenti in carrello
  verrà considerato, in relazione ad articoli gestiti a confezione, il
  totale delle unità presenti in ciascuna confezione.

> Supponendo dunque di aver inserito in carrello 4 confezioni da 7 pezzi
> ciascuna, il totale articoli ammonterà, in queste condizioni a 28
> unità.

- **Considera i colli:** selezionando questa opzione in fase di calcolo
  della quantità degli articoli presenti in carrello verrà considerato,
  in relazione ad articoli gestiti a confezione, il numero dei colli.

> Supponendo dunque di aver inserito in carrello 4 confezioni da 7 pezzi
> ciascuna, il totale articoli ammonterà, in queste condizioni a sole 4
> unità.

**ATTENZIONE!** Le impostazioni settate per il parametro "Totale
Quantità Articoli", e conseguentemente il fatto di considerare nel
calcolo del totale degli articoli presenti in carrello, il numero dei
colli piuttosto che i singoli articoli presenti in ciascuna confezione,
andrà ad impattare, ovviamente, anche su eventuali scaglioni definiti in
base al totale degli articoli presenti in carrello e utilizzati, ad
esempio, per gestire eventuali Spese di spedizione e/o eventuali Spese
accessorie.

**ATTENZIONE!** Si ricorda che in Ho.Re.Ca. non è prevista la gestione
dei colli, per cui in fase di ordine all'interno del sito sarà
possibile, ad esempio, acquistare 4 confezioni di un determinato
prodotto da 7 pezzi ciascuna ma nel momento in cui l'ordine verrà poi
inserito nel gestionale in corrispondenza della relativa riga del
documento verrà inserita una quantità di prodotto pari a 28 unità.

**Confezione Web Singola -- solo Ecommerce Mexal:** consente di decidere
come dovrà essere gestito l'articolo a catalogo nel momento in cui il
campo "Confezione" collegato alla funzionalità Mexal "Gestione
Confezione" dovesse essere impostato sul valore 1 (per maggiori
informazioni relativamente alla funzionalità Mexal "Gestione Confezioni"
si veda anche la sezione *"Configurazione Gestionale -- Mexal
Configurazione Gestionale -- Mexal Attivazione Passweb -- Funzionalità
Mexal Articoli -- Gestione Multipli e Confezioni"* di questo manuale)

![](./assets/media/image19.png)

E' possibile selezionare uno dei seguenti valori:

- **Quantità**: selezionando questa opzione tutti gli articoli a
  catalogo per i quali il campo "Confezione" collegato alla funzionalità
  Mexal "Gestione Confezione" risulti essere impostato sul valore 1,
  verranno gestiti come articoli singoli (senza indicazione dei colli).

> Ciò significa dunque che, lato Mexal, nella riga dell'ordine
> l'articolo verrà inserito sempre e comunque nella quantità indicata
> dall'utente in fase di acquisto senza indicare nessun collo

- **Confezione:** selezionando questa opzione tutti gli articoli a
  catalogo per i quali il campo "Confezione" collegato alla funzionalità
  Mexal "Gestione Confezione" risulti essere impostato sul valore 1
  verranno gestiti come articoli a colli di 1 pezzo ciascuno.

> In queste condizioni dunque, se l'utente dovesse indicare, in fase di
> acquisto sul sito di voler acquistare per l'articolo in esame una
> quantità pari a 3, sulla riga d'ordine del documento Mexal verrà
> inserita una quantità pari a 3x1 ossia 3 colli dell'articolo da un
> pezzo ciascuno

**ATTENZIONE!** Nel caso in cui si dovesse variare la configurazione del
parametro "Confezione Web Singola", affinchè tale variazione venga
correttamente applicata, sarà necessario variare, lato gestionale, gli
articoli coinvolti e lanciare una nuova sincronizzazione Sito --
Gestionale.

