# REGOLE DI RACCOLTA PUNTI



Una volta definiti i parametri di configurazione generali del sistema di
raccolta punti, il passo immediatamente successivo è quello che prevede
di definire nei dettagli le regole secondo cui gli utenti del sito
potranno poi accumulare i vari punti.

In questo senso sarà quindi necessario accedere alla maschera "Raccolta
Punti" precedentemente analizzata, selezionare tra quelle presenti in
elenco la raccolta in relazione alla quale dover definire le relative
regole e cliccare poi sul pulsante "**Regole Punti**" presente nella
contestuale barra degli strumenti

In questo modo si avrà infatti accesso alla maschera "**Lista Regole
Punti**" contenente l'elenco di tutte le regole definite per la raccolta
in esame.

![](./assets/media/image372.png)

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Attiva / Disattiva Regola** (
![](./assets/media/image373.png) /
![](./assets/media/image374.png) **):** consente di attivare / disattivare la regola
attualmente selezionata in elenco

**Copia Regola** (
![](./assets/media/image375.png) )**:** consente di copiare la regola
attualmente selezionata in elenco

**Elimina Regola** (
![](./assets/media/image80.png) )**:** consente di eliminare la regola
attualmente selezionata in elenco

**Modifica Regola** (
![](./assets/media/image79.png) )**:** consente di modificare la regola attualmente
selezionata in elenco

**Aggiungi Regola** (
![](./assets/media/image376.png) )**:** consente di creare una nuova
regola di accumulo punti

Cliccando su quest'ultimo pulsante verrà infatti aperta la maschera
"**Nuova Regola**"

![](./assets/media/image377.png)

all'interno della quale poter impostare tutti i parametri di
configurazione della regola che si intende creare.

Nello specifico il parametro:

**Nome:** consente di assegnare un nome alla regola che si sta
codificando in maniera tale da poterla poi distinguere tra tutte le
altre presenti in elenco

**Azione:** consente di definire l'azione che dovrà essere effettuata
all'interno del sito per poter applicare la regola in questione. E'
possibile selezionare una delle seguenti opzioni:

- **Ordine:** in queste condizioni la regola in esame verrà applicata in
  fase di acquisto e dunque nel momento in cui un utente dovesse
  chiudere un nuovo ordine

- **Registrazione:** in queste condizioni la regola in esame verrà
  applicata in fase di registrazione al sito e dunque nel momento in cui
  un utente dovesse creare il proprio account di accesso

**Valuta di riferimento -- solo se "Azione = Ordine"**: consente di
indicare, selezionandola dal relativo menu a tendina, la valuta in cui
dovranno essere considerati gli importi indicati nei vari parametri di
configurazione della regola stessa.

**Gestione Limite -- solo se "Azione = Ordine":** consente di indicare
se i valori impostati all'interno dei campi:

- Limite Minimo del totale merce

- Limite Massimo del totale merce

- Y per regole di accumulo del tipo "Assegna X Punti per ogni Y del
  totale merce"

dovranno essere considerati o meno comprensivi di IVA

**Limite Minimo / Massimo del totale merce -- solo se "Azione =
Ordine":** valore del totale merce al di sotto / al di sopra del quale
la regola in oggetto non ha validità. Nel caso in cui il totale merce
del documento dovesse essere dunque minore / maggiore del valore
indicato all'interno di questo campo, la corrispondente regola non verrà
mai applicata.

Inoltre, occorre considerare che gli importi indicati in corrispondenza
di questi parametri determineranno anche la visualizzazione o meno del
componente "Punti" eventualmente inserito nelle singole celle articolo
piuttosto che direttamente nelle varie schede prodotto (per maggiori
informazioni in merito si veda anche quanto indicato nel capitolo
"*Lista componenti ecommerce -- Componenti interni ai componenti
ecommerce -- Punti*" di questo manuale)

**ATTENZIONE!** l'importo indicato all'interno di questi campi verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**NOTA BENE:** nel caso in cui l'utente che effettua l'ordine abbia una
valuta diversa da quella specificata all'interno del campo "Valuta di
riferimento" gli importi dei limiti minimo e massimo specificati
all'interno dei relativi campi verranno convertiti nella valuta in uso
dal cliente.

**Periodo di validità:** consente di impostare l'intervallo temporale
entro cui la regola in oggetto verrà ritenuta valida.

**ATTENZIONE!** Regole scadute (con "Data Fine" inferiore alla data
odierna) così come Regole non ancora iniziate (con "Data Inizio"
superiore alla data odierna,) non verranno mai applicate.

**Priorità:** intero a base 1. Consente di specificare l'ordine in cui
dovranno essere valutate le regole definite per il sistema di raccolta
punti in esame.

**L'ordinamento è ascendente e regole prive di priorità verranno
valutate per ultime.**

Supponendo di aver codificato tre distinte regole A, B e C
rispettivamente con priorità 2, 1 e 3 nel momento in cui tali regole
dovessero poi essere applicate (perché l'utente ha concluso un ordine o
si è registrato al sito), verranno valutate per prima cosa le condizioni
di applicabilità della regola B (che ha priorità 1), poi quelle della
regola A (che ha priorità 2) ed infine quelle della regola C (che ha
priorità 3).

**ATTENZIONE!** le regole di accumulo punti possono essere cumulabili
tra loro. In virtù di questo fatto, nel momento in cui, per l'esempio
sopra considerato, dovessero essere soddisfatte le condizioni di
applicabilità di tutte e tre le regole A, B e C l'utente andrà ad
accumulare i punti stabiliti da ciascuna di queste stesse regole.

**Interrompi esecuzione regole:** se selezionato consente di
interrompere, a partire dalla regola in oggetto, la valutazione delle
condizioni di applicabilità di eventuali altre regole con grado di
priorità superiore.

Tale parametro consente quindi di definire il livello di sovrapposizione
e di cumulabilità delle diverse regole definite per il sistema di
raccolta punti in questione.

Per comprendere meglio la funzione e l'importanza di questo parametro
supponiamo, ad esempio, di aver codificato tre distinte regole A, B e C
rispettivamente con priorità 2, 1 e 3 che dovranno essere applicate in
fase di ordine e supponiamo inoltre di aver selezionato il parametro in
oggetto per la regola A.

In queste condizioni nel momento in cui l'utente effettuerà l'ordine sul
sito verranno valutate per prima cosa le condizioni di applicabilità
della regola B (che ha priorità 1) e, se soddisfatte, verranno caricati
sull'anagrafica del cliente i punti stabiliti dalla regola stessa.
Considerando poi che per la regola B non è stato selezionato il
parametro "Interrompi esecuzione regole" verranno valutate anche le
condizioni di applicabilità della regola A (che ha priorità 2) e, se
soddisfatte, verranno caricati sull'anagrafica del cliente anche i punti
stabiliti dalla regola A.

Per la regola A è stato inoltre selezionato il parametro "Interrompi
esecuzione regole" il che farà terminare, esattamente in questo punto,
il processo di valutazione delle condizioni di applicabilità di altre
regole con priorità maggiore a 2.

In conseguenza di ciò le condizioni di applicabilità della regola C (che
ha priorità 3) non verranno neppure valutate. E' possibile quindi
affermare che, in queste condizioni, la regola C non potrà mai essere
cumulabile alle regole A e B.

Considerando infine che per la regola C non è stato selezionato il
parametro di interruzione tale regola potrebbe invece essere cumulabile
con eventuali ulteriori regole di priorità maggiore o uguale a 3.

**Attivo:** consente, se selezionato, di attivare la regola in esame

**Scadenza**: consente di impostare la tipologia di scadenza che dovrà
essere considerata per i punti accumulati mediante la regola in esame.
E' possibile selezionare una delle seguenti opzioni:

- **Fissa**: in queste condizioni i punti accumulati mediante la regola
  in esame avranno una scadenza fissa alla data indicata nel successivo
  campo "Data di Scadenza". Oltre tale data i punti in questione non
  saranno quindi più utilizzabili.

- **Variabile**: in queste condizioni i punti accumulati mediante la
  regola in esame scadranno esattamente (e non saranno quindi più
  utilizzabili) N giorni dopo che sono stati accumulati, dove N è
  esattamente il numero indicato in corrispondenza del successivo
  parametro "**Durata (giorni)**"

**ATTENZIONE!** la scadenza dei punti accumulati non ha nulla a che
vedere con il periodo di validità della relativa regola di raccolta.

In conseguenza di ciò i punti accumulati potrebbero tranquillamente
essere utilizzati anche nel momento in cui la regola secondo cui sono
stati raccolti non dovesse essere più valida

**Data di Scadenza:** consente di indicare la data di scadenza dei punti
accumulati mediante la regola in esame. Oltre tale data i punti in
questione non saranno quindi più utilizzabili

**Durata (gironi) -- solo se "Scadenza = Variabile":** consente di
indicare il numero esatto dei giorni, a partire dalla data di accumulo,
dopo i quali i punti verranno ritenuti scaduti e non potranno quindi più
essere utilizzati

**Descrizione -- solo se "Azione = Ordine":** consente di specificare,
in tutte le lingue attualmente gestite all'interno del sito, un testo
descrittivo della regola di raccolta punti in oggetto, testo questo che
verrà poi mostrato all'interno dei componenti "**Carrello Custom**" e/o
"**Carrellino**" al verificarsi delle seguenti condizioni:

- Il carrello non è vuoto

- La regola di raccolta punti in oggetto non è ancora stata applicata
  perché il Totale Merce non rientra ancora nel range di applicabilità
  della regola stessa (campi "Limite Minimo e Massimo del totale merce")

- La regola di raccolta punti in oggetto non è ancora stata applicata
  perché non sono ancora state soddisfatte le condizioni di
  applicabilità della regola stessa.

> Per maggiori informazioni in merito alle condizioni di applicabilità
> di una specifica regola di raccolta punti si veda anche il successivo
> capitolo di questo manuale "Regole di raccolta punti -- Condizioni"

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
visualizzare, per la stessa Regola di Raccolta Punti, due Descrizioni
differenti, una all'interno della pagina Carrello e una all'interno del
componente Carrellino, sarà necessario, per prima cosa, impostare i
relativi messaggi in maniera tale da poterli identificare univocamente,
ad esempio mediante l'assegnazione di apposite classi CSS.
Successivamente sarà poi possibile nasconderli o visualizzarli secondo
le specifiche esigenze del caso, attraverso l'applicazione di semplici
regole CSS

Grazie a questo parametro è quindi possibile definire un testo mediante
il quale poter informare l'utente del sito che, al verificarsi di
specifiche condizioni (da dettagliare all'interno del testo stesso)
potrà accumulare un determinato numero di punti da riutilizzare poi per
successivi ordini.

![](./assets/media/image378.png)

Il pulsante "**Aggiungi Segnaposto**"

![](./assets/media/image379.png)

consente di inserire all'interno della descrizione della specifica
regola, anche i seguenti Placeholder:

- **Limite minimo**: consente di inserire all'interno del testo il
  segnaposto \$min_limit\$ che verrà poi sostituito, sul front end del
  sito, dall'importo in valuta relativo al limite minimo del totale
  merce che sarà necessario raggiungere per poter attivare la regola in
  esame (campo Limite Minimo del totale merce)

- **Limite massimo**: consente di inserire all'interno del testo il
  segnaposto \$max_limit\$ che verrà poi sostituito, sul front end del
  sito, dall'importo in valuta relativo al limite massimo del totale
  merce oltre il quale non sarà più possibile attivare la regola in
  esame (campo Limite Massimo del totale merce)

- **Differenza Limite Minimo**: consente di inserire all'interno del
  testo il segnaposto \$min_limit_diff\$ che verrà poi sostituito, sul
  front end del sito, con il valore della differenza tra il totale
  carrello dell' utente (ivato o non ivato a seconda di quanto impostato
  in corrispondenza del parametro "Gestione Limite") e il limite minimo
  di applicabilità della regola in esame.

> **ATTENZIONE!** nel caso in cui la "Differenza Limite Minimo" dovesse
> essere negativa (perché il totale in carrello supera il limite minimo
> impostato per la promozione) il valore di questo segnaposto non verrà
> visualizzato
>
> Nel momento in cui l'esigenza dovesse essere quella di nascondere, nel
> caso in cui la differenza in oggetto dovesse essere negativa, non solo
> il valore ma anche un eventuale testo utilizzato come label per il
> valore stesso il tutto andrà racchiuso all'interno del segnaposto
> "**Se differenza Limite Minimo**"

- **Se differenza Limite Minimo:** consente di inserire all'interno del
  testo il seguente segnaposto condizionale:

> \$if(min_limit_diff)\$
>
> -- Testo da visualizzare nel caso in cui la "Differenza limite minino"
> dovesse avere un valore positivo --
>
> \$else\$
>
> -- Testo da visualizzare nel caso in cui la "Differenza limite minino"
> dovesse avere un valore negativo --
>
> \$endif\$
>
> In queste condizioni dunque quanto inserito tra le istruzioni
> \$if(min_limit_diff)\$ e \$else\$ verrà visualizzato solo nel caso in
> cui la differenza tra il totale in carrello e il limite minimo
> impostato per la regola di raccolta punti dovesse essere un valore
> positivo (condizioni di limite minimo non soddisfatta).
>
> Quanto inserito invece tra le istruzioni \$else\$ e \$endif\$ verrà
> visualizzato solo nel caso in cui la differenza tra il totale in
> carrello e il limite minimo impostato per la regola di raccolta punti
> dovesse essere un valore negativo (condizioni di limite minimo
> soddisfatta)

- **Punti**: consente di inserire del all'interno del testo il
  segnaposto \$points\$ che verrà poi sostituito, sul front end del
  sito, dal numero di punti che potranno essere accumulati a seguito
  dell'applicazione della regola in esame

**Zone Associate:** consente di definire, selezionandole tra quelle
definite all'interno della sezione "**Ordini -- Zone**" del Wizard, le
eventuali Zone di Spedizione in corrispondenza delle quali la Regola di
raccolta punti potrà effettivamente essere applicata

**ATTENZIONE!** nel caso in cui il campo in esame dovesse essere
lasciato vuoto la Regola di raccolta punti sarà sempre valida
indipendentemente da quello che potrebbe essere l'indirizzo di
spedizione associato all'utente che naviga il sito

Per associare una nuova Zona alla Regola di raccolta punti che si sta
realizzando sarà sufficiente cliccare sul pulsante "**Aggiungi una
zona**" ed inserirla quindi all'interno del corrispondente riquadro

![](./assets/media/image380.png)

Il campo "Aggiungi una zona" è ad autocompletamento per cui iniziando a
digitare il nome della Zona che si intende associare alla Regola verrà
aperto un elenco contenente tutte le possibili Zone di spedizione
definite all'interno della corrispondente sezione del Wizard (per
maggiori informazioni relativamente a come codificare una Zona di
spedizione utilizzabile poi a livello di Regole punti si veda quanto
indicata all'interno del capitolo "*Ordini -- Zone*" di questo manuale)

![](./assets/media/image381.png)

Nel momento in cui digitando il nome della Zona non dovesse essere
proposta nessuna opzione, significa che la Zona indicata non è tra
quelle codificate all'interno della relativa sezione del Wizard e che
quindi **non dovrà essere associata alla Regola in esame**

**ATTENZIONE! associando alla Regola di raccolta punti una o più Zone di
spedizione, questa potrà poi essere applicata solo nel momento in cui
l'indirizzo di spedizione dell'utente dovesse effettivamente rientrare
in una delle Zone indicate**

In questo senso è bene quindi ricordare che l'indirizzo di spedizione in
base al quale decidere se applicare o meno una regola di raccolta punti
con delle zone associate, verrà valutato in maniera diversa a seconda
del fatto che l'utente stesso abbia o meno effettuato il login al sito e
a seconda anche di quello che sta effettivamente facendo sul sito.

In particolare:

- **Utenti non autenticati**: per questa tipologia di utenti l'indirizzo
  di spedizione verrà valutato prendendo in considerazione solamente la
  Nazione di appartenenza dell'utente, Nazione questa che verrà
  determinata, in prima istanza, sulla base della lingua impostata sul
  browser utilizzato per navigare il sito. Nel caso in cui tale lingua
  dovesse essere priva dell'indicazione dello specifico paese, la
  provenienza del visitatore verrà determinata sulla base del suo
  indirizzo IP.

> **ATTENZIONE! La corrispondenza Indirizzo IP -- Paese di provenienza è
> determinata automaticamente da Passweb sulla base di un servizio
> gratuito di tipo "light" la cui precisione potrebbe non essere quindi
> garantita al 100% soprattutto in virtù di eventuali riassegnazioni
> degli indirizzi IP da parte dei vari provider.**
>
> Se poi il paese ricavato dalle impostazioni del browser o
> dall'indirizzo IP non dovesse essere tra quelli attualmente gestiti
> all'interno del sito, la Nazione di appartenenza dell'utente verrà
> automaticamente impostata sul Paese di Default (per maggiori
> informazioni in merito all'associazione degli utenti non autenticati
> ad una determinata Nazione si veda anche quanto indicato all'interno
> della sezione "*Configurazione -- Parametri Paese Lingua e Valuta --
> Gestione Paese*" di questo manuale)
>
> Una cosa di fondamentale importanza da tenere in considerazione è che
> non avendo a disposizione, in queste condizioni, un indirizzo completo
> e potendo far riferimento soltanto alla Nazione, le Zone di spedizione
> che verranno effettivamente considerate in fase di validazione della
> Regola punti saranno soltanto quelle in cui è stato gestito l'intero
> paese.
>
> In conseguenza di ciò, se il paese di appartenenza dell'utente non
> autenticato dovesse essere, ad esempio, l'Italia e tra le Zone
> associate alla Regola dovessero esserci soltanto Zone per cui è stata
> definita non solo la Nazione Italia ma anche specifiche Regioni,
> Provincie, Località o Cap, queste non verranno validate e, di
> conseguenza, la Regola non verrà applicata.
>
> Al contrario, se tra le Zone associate alla Regola dovesse essercene
> una definita solo per la Nazione Italia allora questa verrebbe
> validata e la Regola sarebbe quindi applicata

- **Utenti autenticati**: nel momento in cui un utente dovesse
  effettuare l'autenticazione al sito, l'indirizzo di spedizione
  valutato per determinare se una Regola di raccolta punti dovrà o meno
  essere applicata sarà, in prima istanza, il suo indirizzo primario

- **Utilizzo del componente "Selezione Indirizzo"**: l'indirizzo di
  spedizione valutato per determinare se una Regola di raccolta punti
  dovrà o meno essere applicata sarà quello eventualmente impostato
  mediante il componente in esame (per maggiori informazioni
  relativamente all'utilizzo del componente "Selezione Indirizzi" si
  rimanda a quanto indicato all'interno del capitolo "*Componenti
  Ecommerce -- Componente Selezione Indirizzo*" di questo manuale)

- **Checkout**: in fase di checkout verrà valutato, ovviamente,
  l'indirizzo di spedizione effettivamente impostato dall'utente
  all'interno del relativo step

Oltre a questi parametri di configurazione generale, potrebbe poi essere
necessario specificare anche:

- una o più condizioni che dovranno essere obbligatoriamente soddisfatte
  affinché la regola in oggetto possa effettivamente essere ritenuta
  valida -- **sezione Condizioni**

- la logica di funzionamento della regola (e quindi in che modo dovranno
  essere caricati i punti) -- sezione **Azione**

- gli specifici Gruppi Utente la regola in esame potrà effettivamente
  essere ritenuta valida -- sezione **Gruppi**

Per maggiori informazioni in merito si vedano i successivi capitoli di
questo manuale.

##### CONDIZIONI

All'interno della sezione "**Condizioni**" è possibile definire una o
più condizioni che dovranno essere obbligatoriamente soddisfatte
affinché la regola in oggetto possa effettivamente essere ritenuta
valida.

**ATTENZIONE! La sezione "Condizioni" è visibile solo ed esclusivamente
per regole configurate con il parametro "Azione = Ordine"**

Prima di poter definire delle nuove condizioni è necessario effettuare
almeno un salvataggio della regola in questione

![](./assets/media/image382.png)

Una vota salvata la regola si attiverà infatti, come mostrato in figura,
un nuovo pulsante mediante il quale poter gestire, attraverso l'apposita
maschera, l'inserimento di una nuova condizione.

![](./assets/media/image383.png)

Per ogni condizione è possibile impostare un valore per i seguenti
parametri:

**Nome:** nome identificativo della condizione che si sta codificando

**Filtro Articoli:** consente di impostare un determinato filtro
articoli. Per maggiori informazioni in merito alla creazione di un
filtro articoli si veda anche la sezione "*Utenti -- Gruppi Utenti Sito
-- Filtri Utente e Filtri Articolo -- Filtri Articolo*" di questo
manuale.

Impostando, sulla condizione in esame, un filtro articoli, la regola in
oggetto potrà essere applicata solo ed esclusivamente nel caso in cui
gli articoli in ordine soddisfino tale filtro.

In questo senso poi occorre sottolineare che, **relativamente agli
articoli di tipo Campionario**, la validazione del filtro impostato
verrà fatta prendendo in considerazione l'articolo Campionario in sé
piuttosto che i singoli Componenti dipendentemente da come è stato
impostato il parametro "**Gestione Articoli Box**" alla pagina
"**Configurazione Catalogo**" del Wizard.

In particolare nel caso in cui il parametro in questione dovesse essere
impostato sul valore:

- **Considera il Box** -- **opzione di default**: verrà preso in
  considerazione soltanto l'articolo Campionario.

> In questo caso dunque, la condizione di applicabilità della Regola
> Punti verrà validata, se l'articolo Campionario in sé dovesse
> effettivamente soddisfare il filtro impostato, indipendentemente dal
> fatto che i suoi componenti possano poi soddisfare o meno lo stesso
> filtro

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, la condizione di applicabilità della Regola
> Punti verrà eventualmente validata prendendo in considerazione i
> componenti del Campionario ma non l'articolo Campionario in sé che,
> quindi, potrebbe anche non soddisfare il filtro impostato.

**Filtro carrello:** consente di impostare un filtro sulla quantità /
numero di articoli presenti in carrello a livello globale o di singola
riga, e/o sulla base del fatto che gli articoli in carrello abbiano o
meno uno sconto già applicato. Di base quindi lavorando sul "Filtro
Carrello" sarà possibile:

- decidere se la Regola Punti dovrà essere applicata solo nel momento in
  cui tutte le righe articolo presenti in carrello dovessero soddisfare
  un eventuale "Filtro Articoli" o anche se solo una certa percentuale
  di esse dovesse essere effettivamente sufficiente per fare scattare la
  promozione.

- decidere se la Regola Punti dovrà essere applicata considerando tutti
  gli articoli presenti in carrello che soddisfano un eventuale "Filtro
  Articoli", oppure solo quelli che, oltre a soddisfare un eventuale
  "Filtro Articoli", risultino anche privi di eventuali altri sconti già
  applicati.

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

- **Quantità in carrello:** permette di definire una condizione sulla
  **quantità complessiva di articoli presenti in carrello**. Supponendo
  quindi di impostare un filtro del tipo "Quantità in carrello maggiore
  di 5" la regola in esame verrà considerata valida solo ed
  esclusivamente nel caso in cui la quantità complessiva di articoli in
  carrello dovesse essere maggiore di 5. Tale condizione potrebbe quindi
  essere soddisfatta inserendo in carrello un solo articolo in quantità
  6 o, ad esempio, due distinti articoli ciascuno in quantità 3.

- **Elementi in carrello:** permette di definire una condizione sul
  **numero complessivo di articoli presenti in carrello**. Supponendo
  quindi di impostare un filtro del tipo "Elementi in Carrello maggiore
  di 2" la regola in esame verrà considerata valida solo ed
  esclusivamente nel caso in cui siano stati inseriti in carrello almeno
  3 distinti articoli indipendentemente dalla quantità acquistata per
  ognuno di essi.

> **ATTENZIONE!** **Nel caso in cui, sulla condizione in esame, sia
> stato impostato anche un Filtro Articoli, nella valutazione del filtro
> sulle quantità e/o sul numero di articoli presenti in carrello
> verranno considerati solo ed esclusivamente gli articoli che
> soddisfano il filtro impostato.**
>
> Di base dunque se dovessimo trovarci in una situazione mista in cui
> sono presenti in carrello sia prodotti che soddisfano un eventuale
> Filtro Articoli sia prodotti che non lo soddisfano, nel momento in cui
> quelli che lo soddisfano dovessero soddisfare anche eventuali
> condizioni impostate sulla quantità o sul numero di elementi, allora
> la regola verrebbe correttamente applicata.
>
> Diversamente se l'esigenza dovesse essere quella di non applicare la
> regola in una situazione mista, in cui ci ritroviamo in carrello
> prodotti che soddisfano il Filtro Articoli ma anche prodotti che non
> lo soddisfano, sarà necessario utilizzare allora per il Filtro
> Carrello l'opzione "Percentuale Elementi in Carrello"

- **Elementi distinti in Carrello**: stesso funzionamento della
  condizione "Elementi in carrello" con la particolarità però di
  considerare eventuali righe che fanno riferimento allo stesso articolo
  come un unico elemento in carrello.

> Supponendo dunque di impostare un filtro del tipo "Elementi distinti
> in carrello maggiore di 2" la regola in esame verrà considerata valida
> solo nel caso in cui dovessero essere presenti in carrello almeno 3
> righe di articoli questa volta **tutti diversi tra loro.**

- **Percentuale Elementi in Carrello**: permette di indicare la
  percentuale di articoli presenti in carrello che dovranno soddisfare
  un eventuale condizione di Filtro Articoli affinché la regola in esame
  possa effettivamente essere applicata.

> Nel momento in cui l'esigenza dovesse essere dunque quella di bloccare
> la regola in una situazione mista e applicarla solo ed esclusivamente
> nel caso in cui tutti gli articoli presenti in carrello dovessero
> soddisfare un'eventuale condizioni di Filtro Articoli, sarà allora
> necessario impostare un Filtro Carrello del tipo "**Percentuale
> elementi in carrello = 100**"

![](./assets/media/image384.png)

> In queste condizioni se dovessimo avere in carrello anche un solo
> articolo che non soddisfa la condizione impostata all'interno del
> campo "Filtro Articoli" la regola, indipendentemente da tutto il
> resto, non verrà applicata.
>
> Allo stesso modo se l'esigenza dovesse essere quella di applicare la
> regola quando almeno il 50% delle righe articolo presenti in carrello
> dovessero soddisfare la condizione di Filtro Articoli, sarà allora
> necessario impostare un Filtro Carrello del tipo "**Percentuale
> elementi in carrello maggiore o uguale 50**"
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere impostato nessun
> Filtro Articoli la "Percentuale elementi in carrello" sarà ovviamente
> sempre uguale a 100

- **Percentuale Quantità in Carrello**: permette di indicare quanti
  articoli in percentuale, rispetto alla quantità totale di prodotti
  presenti in carrello, dovranno soddisfare un eventuale condizione di
  Filtro Articoli, affinché la regola in esame possa effettivamente
  essere applicata

> Supponendo dunque che l'esigenza sia quella di dover applicare la
> Regola Punti solo nel momento in cui almeno il 30% della quantità
> complessiva di articoli presenti in carrello appartenga alla categoria
> 24 ("Outlet Uomo"), dovremmo configurare una condizione di
> applicabilità del tipo di quella rappresentata in figura

![](./assets/media/image385.png)

> In questo modo infatti se dovessimo trovarci ad avere in carrello una
> quantità complessiva di 5 prodotti di cui 4 (quindi 80% del totale)
> appartenenti ad una categoria diversa dalla 24 ed uno solo (quindi il
> 20% del totale) appartenente alla categoria 24, la condizione
> impostata non risulterebbe soddisfatta e la Regola Punti, di
> conseguenza, non verrebbe applicata.
>
> Se invece, in queste stesse condizioni, dovessimo trovarci ad avere in
> carrello una quantità complessiva di 6 prodotti di cui sempre 4 (ossia
> il 67% del totale) appartenenti ad una categoria diversa dalla 24 e i
> restanti 2 (quindi il 33% del totale) appartenenti invece alla
> categoria 24, la condizione impostata sarebbe verificata e, di
> conseguenza, la Regola Punti verrebbe applicata

- **Quantità in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verrà valutata la quantità di riga per ogni
  singolo prodotto che soddisfa l'eventuale filtro impostato. Supponendo
  dunque di considerare una configurazione del tipo di quella
  rappresentata in figura

![Videate\\promozioni_riga.bmp](./assets/media/image386.png)

> la Regola Punti verrà effettivamente applicata solo nel momento in cui
> in carrello dovessimo avere almeno un articolo il cui codice inizia
> con AGLIANIC e la sua quantità di riga dovesse essere maggiore o
> uguale a 2
>
> Nelle condizioni indicate con i seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   1

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> la Regola Punti non verrebbe quindi applicata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due e nessuno di
> essi ha in riga una quantità maggiore o uguale a 2
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> la Regola Punti verrebbe correttamente applicata perché uno dei due
> prodotti che soddisfano il filtro articoli impostato
> (AGLIANICVULDON99) ha effettivamente una quantità di riga uguale a 2

- **Quantità Massima in Riga:** permette di definire una condizione
  sulla quantità di articoli presenti nelle singole righe del carrello.
  Nello specifico, in questo caso, verranno valutati tutti i prodotti
  che soddisfano l'eventuale filtro impostato e tra questi verrà preso
  in considerazione solo quello con la quantità in riga più alta. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata la promozione verrebbe applicata altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\promozioni_riga_2.bmp](./assets/media/image387.png)

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Regola Punti non verrebbe applicata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il primo ma tale quantità
> (2) non soddisfa comunque la condizione impostata (maggiore o uguale a
> 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   4

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Regola Punti verrebbe correttamente applicata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il secondo
> (AGLIANICVULROI01) e tale quantità (4) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Quantità Minima in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verranno valutati tutti i prodotti che
  soddisfano l'eventuale filtro impostato e tra questi verrà preso in
  considerazione solo quello con la quantità in riga più bassa. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata la promozione verrebbe applicata altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\promozioni_riga_3.bmp](./assets/media/image388.png)

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Regola Punti non verrebbe applicata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) ma tale quantità (1) non soddisfa comunque la
> condizione impostata (maggiore o uguale a 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   3

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> la Regola Punti verrebbe correttamente applicata perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) e tale quantità (3) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Sconto in Riga**: permette di definire una condizione di
  applicabilità della Regola Punti che tenga conto di tutti gli articoli
  presenti in carrello che soddisfano un eventuale "Filtro Articoli", o
  solo di quelli che, oltre a soddisfare un eventuale "Filtro Articoli",
  risultino anche privi di eventuali altri sconti già applicati.

> **ATTENZIONE! l'opzione "Sconto in Riga" è di tipo Stringa**
>
> In conseguenza di ciò per creare una condizione che verrà validata
> solo nel caso in cui i prodotti in carrello che soddisfano un
> eventuale "Filtro Articoli" risultino essere anche privi di altri
> sconti già applicati, **il campo "Valore" della condizione "Sconto in
> Riga" dovrà essere lasciato vuoto (**Valore = Stringa vuota).
>
> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\promozioni_sconto_in_riga.bmp](./assets/media/image389.png)

> la condizione in esame verrà validata e la relativa Regola Punti
> applicata solo nel caso in cui tutti gli articoli presenti in carrello
> (**Percentuale Elementi in Carrello = 100**) appartengano alla
> categoria 24 e siano tutti privi di sconto (**Sconto in Riga = stringa
> vuota**)
>
> Al contrario, se anche tutti gli articoli presenti in carrello
> appartenessero effettivamente alla categoria 24 ma anche uno solo di
> essi avesse già uno sconto applicato (perché ad esempio importato dal
> gestionale) la condizione non verrebbe validata e, di conseguenza, la
> relativa Regola Punti non verrebbe applicata.
>
> **ATTENZIONE!** **si ricorda che nel caso di articoli box (campionari
> standard e configurabili) il prezzo del box stesso viene determinato
> sommando il prezzo dei singoli componenti al netto di eventuali sconti
> ad essi applicati**
>
> In sostanza dunque ad articoli Campionario non verrà mai applicato
> direttamente un determinato sconto.
>
> Nel momento in cui l'esigenza dovesse essere quindi quella di
> considerare non lo sconto dell'articolo campionario in sé ma quello
> eventualmente applicato ai suoi componenti sarà necessario verificare
> di aver correttamente impostato il parametro "**Gestione Articoli
> Box**" presente alla pagina "**Configurazione Catalogo**" del Wizard
> sul valore "**Considera i componenti del Box**".
>
> Per maggiori informazioni in merito a questo parametro si veda anche
> quanto indicato nel relativo capitolo di questo manuale ("*Catalogo --
> Configurazione Parametri Catalogo - Catalogo Mexal / Ho.Re.Ca. --
> Gestione Carrello*")

**Filtro Totale:** consente di impostare un Filtro mediante il quale
poter decidere se la regola dovrà essere applicata o meno in relazione a
determinati Totali del documento.

**ATTENZIONE!** l'importo indicato nelle condizioni di filtro dovrà
essere espresso nella valuta definita all'intero del campo **"Valuta di
Riferimento"** presente tra i parametri di configurazione della regola
in esame

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

- **Totale merce ivato / non ivato:** consente di impostare una
  condizione di applicabilità della regola basata sul Totale merce ivato
  / non ivato del carrello.

> Supponendo quindi di impostare un filtro del tipo "**Totale merce
> ivato maggiore o uguale 50**" la regola verrà applicata solo nel caso
> in cui il totale merce ivato in carrello sia effettivamente maggiore o
> uguale a 50€

- **Subtotale merce ivato / non ivato:** consente di impostare una
  condizione di applicabilità basata sulla somma dei Totali di Riga
  ivati / non ivati dei soli prodotti in carrello che soddisfano un'
  eventuale condizione di Filtro Articoli impostata per la regola stessa

> **ATTENZIONE!** Nel momento in cui non dovesse essere presente nessun
> Filtro Articoli anche in questo caso verrà preso in considerazione,
> ovviamente, il Totale merce ivato / non ivato dell'interno carrello

- **Percentuale subtotale merce ivato / non ivato:** consente di
  impostare una condizione di applicabilità basata sulla percentuale del
  subtotale merce (ivato /non ivato) dei soli prodotti in carrello che
  soddisfano un' eventuale condizione di Filtro Articoli in relazione a
  quello che è il totale merce (ivato / non ivato) complessivo
  dell'interno carello.

> Supponendo dunque di configurare una condizione di applicabilità del
> tipo di quella rappresentata in figura

![](./assets/media/image390.png)

> la Regola Punti in esame verrà applicata solo nel caso in cui
> dovessero essere presenti in carrello articoli della categoria 113 il
> cui totale merce, non ivato, risulti maggiore o uguale al 30% del
> totale merce, non ivato, dell'interno carrello

Nella definizione dei Filtri Articolo / Quantità / Totale è anche
possibile, volendo, concatenare tra loro due o più condizioni. Al
termine di ogni condizione, dopo aver impostato operatore relazionale e
relativo valore della condizione, verrà infatti visualizzata una "e",
corrispondente all'operatore logico "AND", e utilizzata, a default, per
concatenare tra loro eventuali ulteriori filtri che dovranno essere
considerati nella definizione della condizione da soddisfare per
l'effettiva applicazione della regola.

Cliccando su questo elemento verrà aperta una piccola finestra
all'interno della quale poter selezionare eventuali ulteriori operatori
logici. Le eventuali parentesi, poste prima o dopo questi operatori,
vanno utilizzate esattamente come avviene in algebra, per specificare
quali condizioni dovranno essere valutate prima e quali dopo.

![](./assets/media/image391.png)

Il parametro "**Gestione Condizioni**" permette di decidere, infine, se
la regola in esame dovrà essere ritenuta valida al verificarsi di tutte
le condizioni indicate oppure solamente di un determinato numero di
esse.

![](./assets/media/image392.png)

In particolare dunque impostando questo parametro sul valore:

- **Tutte le condizioni devono essere soddisfatte**: la regola verrà
  considerata valida solo ed esclusivamente nel momento in cui tutte le
  condizioni inserite siano state soddisfatte

- **Almeno X condizioni devono essere soddisfatte**: per poter
  considerare valida la regola in esame è sufficiente che siano
  soddisfatte almeno X condizioni di quelle indicate, dove X sarà
  esattamente il numero specificato in corrispondenza del successivo
  campo "**Numero condizioni (X)**"

**ATTENZIONE!** il numero di condizioni da verificare per poter
applicare la regola influisce anche sull' effettiva visibilità del
componente "Punti". Per maggiori informazioni in merito a questo
componente si veda anche quanto indicato all'interno del relativo
capitolo di questo manuale ("*Varianti Sito Responsive -- Lista
Componenti Ecommerce -- Componenti interni ai componenti ecommerce --
Punti*").

Supponendo dunque di avere a che fare con una regola costituita dalle
tre condizioni di seguito indicate:

- Articoli appartenenti alla categoria "Uomo"

- Quantità in carrello \>= 2

- Totale merce non ivato \>= 100€

e di avere impostato l'applicazione della regola al verificarsi di
almeno 2 delle suddette condizioni, il componente "Punti" inserito ad
esempio all'interno del "Catalogo Ecommerce" (dove viene considerato
sempre in quantità unitaria) verrà visualizzato solo in corrispondenza
di quegli articoli che appartengono effettivamente alla categoria "Uomo"
e il cui prezzo unitario non ivato risulti essere effettivamente
maggiore o uguale a 100€.

##### AZIONI

Una volta definite tutte le condizioni necessarie per poter
effettivamente ritenere valida la regola, occorre impostare, ovviamente,
la parte più importante della regola stessa ossia la sua logica di
funzionamento

Questo lo si fa agendo all'interno della sezione **Azione.**

![](./assets/media/image393.png)

In particolare il parametro:

**Tipo** consente di specificare come dovranno effettivamente essere
accumulati i vari punti. E' possibile selezionare una delle seguenti
opzioni:

- **Assegna X punti al Cliente:** selezionando questa opzione, nel
  momento in cui tutte le condizioni di applicabilità della regola
  dovessero essere soddisfatte, alla chiusura di un ordine verranno
  assegnati al cliente X punti, dove X è esattamente il numero indicato
  in corrispondenza del successivo parametro **X**

- **Assegna X punti per ogni Y del totale merce:** selezionando questa
  opzione, nel momento in cui tutte le condizioni di applicabilità della
  regola dovessero essere soddisfatte, alla chiusura di un ordine
  verranno assegnati al cliente X punti per ogni Y del totale merce dove
  X e Y sono esattamente i valori indicati in corrispondenza dei
  successivi parametri **X** e **Y.**

> **ATTENZIONE!** Il Totale Merce sulla base del quale calcolare i punti
> effettivamente accumulabili è quello determinato dai soli articoli che
> soddisfano eventuali filtri impostati sulla condizione di
> applicabilità della regola.
>
> In questo senso nel caso dei Campionari verrà considerato l'articolo
> in se piuttosto che i singoli componenti dipendentemente da come è
> stato impostato il parametro "**Gestione Articoli Box**" alla pagina
> "**Configurazione Catalogo**" del Wizard
>
> Infine, il totale merce verrà considerato comprensivo o meno di iva a
> seconda di quanto impostato per il parametro "**Gestione Limite**"
>
> **ATTENZIONE! In queste condizioni eventuali arrotondamenti nel
> calcolo del numero di punti da caricare per il cliente che sta
> effettuando l'ordine verranno considerati sempre per difetto**

**Base Calcolo -- solo per "Tipo = Assegna X punti per ogni Y del totale
merce":** consente di decidere se il Totale Merce da utilizzare per
determinare il numero di punti da assegnare al cliente dovrà essere
considerato o meno comprensivo di IVA

**Numero massimo di punti da assegnare -- solo per "Tipo = Assegna X
punti per ogni Y del totale merce"**: consente di definire un numero
massimo di punti da assegnare al cliente oltre il quale non si potrà mai
andare indipendentemente da quello che sarà poi l'effettivo totale merce
del documento.

##### GRUPPI

La sezione **Gruppi**, presente nella parte bassa della maschera,
consente infine di associare uno o più gruppi utente alla regola in
esame, definendo, quindi, per quali utenti la regola potrà
effettivamente essere applicata

![](./assets/media/image394.png)

Nel box sulla sinistra sono visualizzati tutti i gruppi utente
codificati all'interno della corrispondente sezione del Wizard (per
maggiori informazioni in merito si veda la sezione "*Utenti -- Gruppi
Utenti Sito*" di questo manuale). Per associare un gruppo utente alla
regola è sufficiente selezionarlo dall'elenco di sinistra ed inserirlo
in quello di destra cliccando sul pulsante raffigurante una piccola
freccia rivolta verso destra.

Allo stesso modo per eliminare l'associazione "Gruppo Utente -- Regola",
sarà sufficiente selezionare il gruppo desiderato dall'elenco di destra
ed eliminare l'associazione cliccando sul pulsante raffigurante una
piccola freccia rivolta verso sinistra.

**Una volta associato un gruppo di utenti ad una Regola, questa verrà
valutata ed eventualmente applicata solo nel momento in cui l'utente
beneficiario dei punti appartenga effettivamente ad uno dei gruppi
associati alla regola**

**ATTENZIONE!** Nel caso in cui alla regola non venga associato alcun
gruppo, questa potrà essere applicata (con i relativi limiti) ad un
qualsiasi utente del sito.

