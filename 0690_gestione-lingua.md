# GESTIONE LINGUA



La pagina "**Gestione Lingua**" **accessibile solo nel caso di siti
Ecommerce collegati a Mexal**, consente di associare ad ogni lingua
gestita all'interno del sito uno specifico codice della "Tabella Lingue
Estere" di Mexal in maniera tale da consentire a Passweb di poter
prelevare, direttamente dal gestionale, le descrizioni in lingua degli
articoli presenti all'interno del negozio web.

**NOTA BENE:** l'attivazione di una o più lingue estere, e la
conseguente realizzazione di un sito in multilingua, dipende da quanto
impostato in "Sito -- Gestione Lingue del Sito"; per i dettagli relativi
a questa operazione si rimanda quindi alla specifica sezione di questo
manuale.

Considerando che Passweb non dispone di un dizionario integrato, nel
caso di siti in multilingua, le pagine del sito ed i relativi componenti
in lingua andranno, generalmente, editati in maniera manuale. Nel caso
ad esempio di un sito in italiano e inglese, il contenuto di un
componente "Paragrafo", ad esempio, dovrà essere inserito dall'utente
sia in lingua italiana che in lingua inglese.

Possono fare eccezione a questa regola le descrizioni degli articoli
presenti all'interno del negozio web. **Passweb infatti gestisce
eventuali descrizioni in lingua opportunamente inserite, per i singoli
articoli, all\'interno del gestionale.**

Questo significa dunque che nel caso in cui si decidesse di inserire
all'interno del sito, laddove possibile, il componente E-Commerce
**"Titolo"**, e nel caso in cui si fosse deciso di utilizzare come tipo
di dato per generare il "Titolo" degli articoli l'opzione "Descrizione
Gestionale", alla sincronizzazione verrebbero presi, per il campo in
esame, anche gli eventuali valori in lingua e **tale campo potrebbe
quindi visualizzare, in maniera del tutto automatica, valori diversi a
seconda della diversa lingua di visualizzazione del sito**.

**NOTA BENE:** per maggiori informazioni relativamente alla gestione del
Componente E-Commerce "Titolo" si veda anche il capitolo di questo
manuale relativo ai componenti E-Commerce.

Per poter fare in modo che avvenga tutto ciò occorrerà, per prima cosa,
lato Mexal attivare una o più lingue estere e associare una o più
descrizioni in lingua ai vari articoli. Fatto questo occorrerà poi, lato
Passweb, stabilire una corrispondenza tra le lingue abilitate e gestite
all'interno del sito e le lingue abilitate e gestite all'interno di
Mexal. La sincronizzazione successiva a queste due operazioni consentirà
a Passweb di prelevare da Mexal le corrette descrizioni in lingua dei
vari articoli e di visualizzare quindi il valore del campo "Titolo" in
maniera diversa a seconda della diversa lingua di visualizzazione del
sito.

Per associare all\'interno del gestionale una o più descrizioni in
lingua ai vari articoli occorre:

- Settare l\'apposito parametro di magazzino **\"Descrizioni in lingua
  straniera\"** che consente di stabilire il numero di lingue (compreso
  tra 2 e 9), e conseguentemente il numero di descrizioni articolo in
  lingua estera, che sarà poi possibile editare

![](./assets/media/image158.png)

- Attivare le lingue che si intende gestire associando semplicemente
  un\'etichetta agli slot della **\"Tabella Lingue Estere\"**
  *(Magazzino - Tabelle Aziendali - Lingue Straniere)* di Mexal

![](./assets/media/image159.png)

- Associare la descrizione in lingua ai singoli articoli all\'interno
  della loro anagrafica, compilando i vari campi della maschera
  **\"Descrizioni in lingue\"** accessibile premendo F2 sul campo
  \"Descr\"

![](./assets/media/image160.png)

I valori inseriti in questo campo saranno poi quelli visualizzati
all\'interno del sito web nelle corrispondenti pagine in lingua.

Per maggiori informazioni relativamente all'attivazione e alla gestione
delle lingue estere in Mexal si rimanda al relativo manuale.

Per stabilire una corrispondenza tra le lingue abilitate e gestite
all'interno del sito e le lingue abilitate e gestite all'interno di
Mexal, occorre invece agire direttamente all'interno di Passweb dalla
pagina **"Gestione Lingua"**. All'interno di questa pagina verrà infatti
visualizzata la maschera, **"Gestione delle Lingue Estere",** qui di
seguito riportata

![](./assets/media/image161.png)

attraverso la quale poter realizzare l'associazione in oggetto.

All'interno di questa maschera verrà infatti visualizzato l'elenco delle
lingue gestite in Passweb ed in cui è stato dunque realizzato il sito
web.

Per poter completare l'associazione "Lingua Mexal -- Lingua Passweb"
sarà sufficiente indicare per ciascuna lingua gestita all'interno del
sito, selezionandolo dal relativo menu a tendina, il numero della lingua
corrispondente all'interno della "Tabella Lingue Estere" di Mexal.

**ATTENZIONE! Per i siti multilingua collegati a Mexal la Descrizione in
Italiano, eventualmente utilizzata per generare il Titolo dell'articolo
ed il corrispondente permalink, e normalmente inserita all'interno del
campo "Descrizione" dell'Anagrafica Articolo, potrebbe anche essere
inserita in uno dei campi relativi alle lingue aggiuntive gestite in
Mexal stesso.**

![](./assets/media/image162.png)

Una scelta di questo tipo potrebbe rivelarsi particolarmente utile in
quanto consentirebbe di definire, direttamente all'interno del
gestionale e senza il bisogno di creare apposite videate aggiuntive, una
descrizione articolo "SEO Friendly" che ben si sposa cioè con quelle che
possono essere esigenze tipicamente web lasciando inalterata la
"Descrizione principale" nell'Anagrafica Articolo che, al contrario,
potrebbe invece essere stata creata secondo altre logiche puramente
gestionali che poco anche a che vedere con il posizionamento di una
pagina web.

**ATTENZIONE! Per adottare questa soluzione è necessario aver mappato
anche la lingua Italiana con una delle lingue "Extra" abilitate e
gestite all'interno del gestionale**

![](./assets/media/image163.png)

Nel caso in cui non dovesse essere effettuato questo tipo di Mapping il
Titolo degli Articoli ed il loro permalink verrà generato sempre e
soltanto sulla base del campo Descrizione presente in Anagrafica
Articolo.

