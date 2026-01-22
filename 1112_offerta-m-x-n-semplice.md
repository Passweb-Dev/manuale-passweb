# OFFERTA M X N SEMPLICE



Utilizzando questo tipo di Promozione è possibile configurare delle
offerte di tipo M x N (il classico 3x2) dove M indica quanti articoli
devono essere acquistati per aver diritto allo sconto e N quanti degli M
articoli acquistati verranno poi effettivamente pagati.

E' possibile mettere in promozione singoli articoli (Tabella "**Articoli
in Promozione**") oppure intere categorie di articoli (Tabella
**"Articoli appartenenti alle categorie"**)

![](./assets/media/image553.png)

**ATTENZIONE! In queste condizioni, il programma crea un'offerta M x N
diversa per ogni articolo inserito.**

Supponiamo, ad esempio, di aver impostato questa promozione per
configurare un 3x2.

Inserendo in ordine gli articoli "After Shave Hugo Boss", "Acqua di Giò"
e "Armani Mania" (tutti associati alla Promozione in esame) l'offerta
verrà applicata solo ed esclusivamente nel momento in cui il cliente
dovesse acquistare 3 "After Shave Hugo Boss", o 3 "Acqua di Giò" o 3
"Armani Mania".

L'offerta **non** verrà invece applicata se si dovessero acquistare, ad
esempio, 2 "Acqua di Giò" e 1 "Armani Mania".

Per realizzare un'offerta dove il cliente possa acquistare, a scelta,
sia "Acqua di Giò" che "Armani Mania" ottenendo, comunque, il diritto
allo sconto, è necessario utilizzare delle Promozioni di tipo **"M x N
Articoli Misti"** (per maggiori informazioni in merito a questo tipo di
Promozione si veda anche il successivo capitolo di questo manuale.);

I due campi presenti in corrispondenza del parametro "**Parametri M x
N**" permettono di definire esattamente tanto il numero di articoli che
devono essere acquistati per poter applicare la promozione quanto quelli
che verranno poi effettivamente pagati.

![](./assets/media/image554.png)

In particolare il campo:

- **M:** permette di impostare il numero di articoli che devono essere
  acquistati affinchè il cliente abbia diritto allo sconto

- **N:** permette di impostare il numero esatto di articoli che il
  cliente dovrà effettivamente pagare

Il campo "**Valore / Percentuale**" presente immediatamente al di sotto
della tabella "Articoli appartenenti alle categorie" consente invece, di
definire esattamente come dovranno essere trattati gli M -- N articoli
oggetto della promozione.

![](./assets/media/image555.png)

Non è detto, infatti, che tali articoli debbano per forza di cose essere
gratuiti. Ad essi potrebbe tranquillamente essere applicata una certa
percentuale di sconto come, allo stesso modo, questi articoli potrebbero
essere inseriti in ordine con un certo prezzo fisso. Tutto ciò lo si
stabilisce, appunto dal campo "**Valore / Percentuale**"

Supponiamo, ad esempio, di voler realizzare un classico 3 x 2 dove il
terzo articolo in ordine sia gratuito. Per ottenere questo tipo di
risultato sarà necessario selezionare, per il campo in esame, l'opzione
"**Percentuale**" ed inserire poi nel campo sottostante il valore 100.

![](./assets/media/image556.png)

In queste condizione al terzo articolo verrà quindi applicato uno sconto
del 100%.

Se si volesse invece realizzare una Promozione in cui il terzo articolo
in ordine venga acquistato a metà prezzo sarà ovviamente necessario
selezionare per il parametro in esame, ancora una volta, l'opzione
"Percentuale" inserendo però nel successivo campo il valore 50.

Se invece l'esigenza dovesse essere quella di configurare un 3x2 in cui
il terzo articolo debba sempre essere pagato 5 €, sarà necessario
selezionare, per il parametro in esame, l'opzione **Valore** inserendo
poi il valore 5 nel successivo campo.

![](./assets/media/image557.png)

In queste condizioni il terzo articolo verrà pagato sempre 5 €,
indipendentemente da quello che possa essere il suo effettivo prezzo di
listino.

**ATTENZIONE!** Il parametro **"Numero massimo applicazioni offerta"**
che, lato gestionale, consente di definire quante volte l'offerta possa
essere applicata prima che si disattivi in automatico, **non è
attualmente gestito all'interno del sito, dove la promozione potrà
quindi essere disattivata solo in maniera manuale oppure in base al suo
intervallo di validità.**

Dopo aver codificato questa Promozione ed averla esportata all'interno
del sito, prima di poterla effettivamente utilizzare sarà necessario,
ovviamente, attivarla e questo potrà essere fatto direttamente dalla
maschera "Lista delle Promozioni", selezionandola in elenco e cliccando
sul pulsante "**Attiva Promozione**" oppure agendo dal parametro
"**Attivo**" presente nella maschera di configurazione della Promozione
stessa.

![](./assets/media/image558.png)

Il campo **Descrizione** presente all'interno della maschera di
configurazione della promozione consente di specificare, in tutte le
lingue attualmente gestite all'interno del sito, un testo descrittivo
della promozione in oggetto, testo questo che verrà poi mostrato
all'interno del componente "**Carrello Custom**" al verificarsi delle
seguenti condizioni:

- Il carrello non è vuoto

- La promozione in oggetto non è ancora stata applicata perché non sono
  ancora state soddisfatte le condizioni di applicabilità della
  promozione stessa definite all'interno del gestionale relativamente
  agli articoli e/o alle categorie di articoli coinvolte.

Il parametro in oggetto consente quindi di definire un testo mediante il
quale poter informare l'utente del sito che, al verificarsi di
specifiche condizioni (da dettagliare all'interno del testo stesso)
potrà beneficiare di determinate promozioni.

In questo senso, cliccando sul pulsante "**Aggiungi Segnaposto**", sarà
possibile inserire all'interno del testo il seguente placeholder:

- **Sconto**: consente di inserire all'interno del testo il segnaposto
  {discount} che verrà poi sostituito, sul front end del sito, dal
  valore dello sconto (in percentuale o in valuta) di cui l'utente potrà
  beneficiare al verificarsi delle condizioni di applicabilità della
  promozione in esame (promozione che dovrà ovviamente prevedere
  l'applicazione di un determinato sconto)

**ATTENZIONE! Gli sconti dovuti all'applicazione di questo tipo di
Promozioni verranno applicati, all'interno del sito, sempre e comunque a
livello di Carrello mediante l'inserimento di un relativo Abbuono**

![](./assets/media/image540.png)

In queste condizioni non sarà ovviamente possibile visualizzare gli
sconti dovuti alla promozione ne in Catalogo ne tanto meno all'interno
delle varie schede prodotto.

L'Abbuono dovuto all'applicazione della Promozione verrà infatti
visualizzato soltanto in Carrello oltre che, ovviamente, in fase di
Checkout ordine.

Relativamente alle condizioni di applicabilità di questo tipo di
Promozioni occorre fare un'ulteriore considerazione molto importante.

**Nel caso in cui gli articoli coinvolti nella Promozione siano gestiti
con un unità di misura diversa da pz**, la promozione verrà applicata
sul sito, in maniera leggermente diversa a quanto avviene sul
gestionale.

In queste condizioni (articoli con unità di misura diversa da pz)
infatti, **sul gestionale**, la promozione verrà applicata solo nel
momento in cui all'interno del documento venissero inserite **righe
articolo distinte**. Il 3x2, ad esempio, potrà essere applicato solo se
nel conto cassa sono presenti 3 righe articolo distinte; non verrebbe
invece applicato se fosse presente una sola riga articolo con quantità
impostata a 3.

**Sul sito invece, in queste stesse condizioni,** la Promozione verrà
applicata semplicemente nel momento in cui la quantità sulla singola
riga articolo soddisfa quanto indicato per la promozione, come del resto
avverrà anche per articoli gestiti con unità di misura uguale a pz.

Sul sito infatti non è possibile creare più righe distinte per lo stesso
articolo in ordine; aggiungendo in carrello, anche in momenti diversi,
lo stesso articolo verrà sempre incrementata la quantità attualmente
presente sulla stessa, singola, riga articolo.

Lato gestionale, infine, nel momento in cui si andrà a caricare, in
cassa, l'ordine nato all'interno del sito web, lo sconto, dovuto alla
promozione e **applicato sul sito a livello di Carrello** mediante un
relativo **Abbuono,** verrà riportato all'interno del campo **Sconto**

![](./assets/media/image542.png)

**ATTENZIONE!** Le Promozioni di tipo **Offerte M x N semplice** sono
considerate tra l'elenco delle Promozioni da poter escludere nel caso di
applicazione di eventuali Buoni Sconto.

Ciò significa dunque che nel momento in cui un dato utente dovesse
trovarsi applicata questo tipo di promozione, e fosse anche in possesso
di un Codice Sconto ancora valido, potrebbe essere possibile fare in
modo che l'applicazione del Buono Sconto annulli automaticamente
l'applicazione della Promozione.

Per maggiori informazioni sull'utilizzo dei Buoni Sconto e sulla
possibilità di escludere o meno determinate promozioni all'applicazione
dei Buoni Sconto si veda anche il capitolo "*Ordini -- Configurazione
Promozioni -- Buoni Sconto*" di questo manuale.

