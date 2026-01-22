# TRACCIAMENTO SITO



Oltre alla condivisione dei dati via feed un altro punto cardine di
tutto l'ecosistema Clerk è, ovviamente, il tracciamento in tempo reale
del comportamento utente. L'IA di Clerk infatti apprende continuamente
da quello che gli utenti fanno sul sito, i prodotti che visitano, quelli
che mettono in carrello, gli ordini portati a termine ....

Tracciare questi comportamenti quindi è di fondamentale importanza per
consentire a Clerk di fare previsioni accurate e di mostrare anche
statistiche dettagliate relativamente all'impatto che i suggerimenti
forniti da questo sistema hanno effettivamente prodotto sugli ordini
effettuati all'interno del sito (cosa questa di fondamentale importanza
inquanto aiuta l'amministratore a capire quanto effettivamente Clerk può
essergli utile)

Dal punto di vista tecnico il sistema di tracciamento di Clerk può
operare sia lato client (via javascript) che lato server (attraverso
apposite chiamate API) in modo tale da coprire tutte le casistiche
possibili.

Il tracciamento lato client è gestito interamente dalla libreria
Clerk.js, la stessa da cui dipende di fatto il corretto funzionamento di
tutti i moduli Clerk implementati all'interno del sito mediante
Injection o Embedding del codice (es. moduli di ricerca, chat,
raccomandazioni ...) per cui, sotto questo punto di vista, è tutto
automatico e non dovremo preoccuparci di nulla se non di assicurarci di
aver configurato correttamente l'inizializzazione di questo script (per
maggior informazioni in merito si veda anche quanto indicato nel
precedente capitolo "*Integrazione -- Configurazione Parametri Store*"
di questo manuale).

Oltre a questo vanno però considerate anche altre cose di fondamentale
importanza. Innanzitutto l'integrazione Passweb -- Clerk prevede anche,
come visto, la possibilità di implementare le Raccomandazioni mediante
l'utilizzo di un componente nativo di Passweb che, in questo senso, non
ha nulla a che vedere con lo script Clerk.js.

Oltre a questo ci sono poi anche altri eventi che possono verificarsi
all'interno del sito (es. completamento di un ordine, aggiunta di
articoli in carrello ...), che non sono gestiti automaticamente dalla
libreria Clerk.js e che possono richiedere quindi o l'utilizzo di un
tracciamento lato server o comunque un intervento da dover eseguire
manualmente sulle pagine del sito

In generale quindi i punti chiave da prendere in considerazione nel
sistema di tracciamento implementato da Clerk sono quelli di seguito
indicati:

**CLICK SU PRODOTTI PRESENTI ALL'INTERNO DEI MODULI IMPLEMENTATI
ALL'INTERNO DEL SITO (SEARCH, RACCOMANDAZIONI, CHAT ...)**

Il click su di un prodotto suggerito da Clerk all'interno di una
raccomandazione piuttosto che di un risultato di ricerca o di una Chat,
è il punto di ingresso che consente poi all'amministratore del sito,
grazie alle statistiche presenti nelle varie Dashboard del proprio
account Clerk, di capire esattamente quanto Clerk stesso può aiutarlo ad
aumentare le vendite.

In questo senso infatti se un utente dovesse cliccare su di un prodotto
suggerito da Clerk e, successivamente dovesse poi chiudere un ordine con
all'interno quello stesso prodotto, il tracciamento del click iniziale
consentirà a Clerk di sapere che quella vendita è stata generata da un
suo suggerimento, di capire anche lo specifico elemento che ha generato
quel suggerimento (lo slider di una ben precisa raccomandazione,
piuttosto che un modulo di ricerca o un suggerimento in Chat), di
calcolare l'impatto che quell'articolo a prodotto sul valore complessivo
dell'ordine e di mostrare all'amministratore tutti questi dati
all'interno di specifiche Dashboard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracciamento_clerk_1.bmp](./assets/media/image65.png){width="5.428472222222222in"
height="3.33125in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracciamento_clerk_2.bmp](./assets/media/image66.png){width="5.428472222222222in"
height="3.33125in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tracciamento_clerk_3.bmp](./assets/media/image67.png){width="5.428472222222222in"
height="3.3375in"}

Dal punto di vista tecnico il modo in cui tracciare questi click può
variare a seconda di come viene implementato il singolo modulo
all'interno del proprio sito, nello specifico:

- Nel caso in cui il modulo sia stato implementato mediante Injection o
  Embedding del codice il tracciamento del click sarà gestito lato
  client in maniera automatica dalla libreria Clerk.js

- Nel caso in cui si dovesse invece ricorrere ad un'implementazione via
  API, Clerk.js, tipicamente, non potrà intervenire (o almeno non in
  maniera completa) per cui sarà necessario tracciare anche i vari click
  lato server

Riportando quanto detto nell'ambito dell'integrazione Passweb -- Clerk,
per quel che riguarda i moduli Search e Chat non ci sono problemi nel
senso che questi possono essere implementati solo con Injection o
Embedding e quindi il tracciamento del click sugli articoli mostrati al
loro interno sarà completamente automatico.

Per quel che riguarda le Raccomandazioni invece, come visto, queste
potranno essere implementate mediante injection / embedding del codice
(e anche in questo caso tutto verrebbe gestito automaticamente da
Clerk.js) oppure possono essere implementate utilizzando anche un
componente nativo di Passweb (Popolarità Prodotto) che utilizzerà per
questo apposite chiamate API.

**Anche in questo caso comunque non ci si dovrà preoccupare di nulla
inquanto l'integrazione prevede anche il tracciamento lato server dei
click effettuati sugli articoli mostrati all'interno di questi
componenti Passweb.**

L'unica cosa da prendere in considerazione è il fatto che, operando
mediante injection o embedding l'impatto di una vendita verrà
eventualmente associato al nome o alla label assegnata direttamente
all'interno di Clerk allo specifico modulo di ricerca o allo specifico
slider di raccomandazione che ha prodotto quella stessa vendita.

Nel momento in cui la vendita avrà invece origine dal click su di un
prodotto presente all'interno di un componente "Popolarità Prodotto" di
Passweb (configurato per visualizzare delle raccomandazioni Clerk) non
si avrà, ovviamente, un elemento corrispondente su Clerk cui assegnare
l'impatto della vendita. Per risolvere questo problema sia in fase di
richiesta dei dati che in fase di tracciamento del click verrà passata a
Clerk un'etichetta con il nome del componente Passweb per cui, alla
fine, l'impatto della vendita su Clerk verrà assegnato proprio alla
label indicata e quindi allo specifico componente Passweb che l'ha
prodotta.

**COMPLETAMENTO DI UN ORDINE**

Ovviamente, affinché quanto indicato al punto precedente possa
funzionare in maniera corretta sarà necessario tracciare non solo il
click sul suggerimento offerto da Clerk ma anche l'ordine effettuato poi
dall'utente.

Il completamento dell'ordine però non ha un interazione diretta con un
modulo Clerk per cui il suo tracciamento dovrà essere effettuato,
sostanzialmente, allo stesso modo di come avviene il normale
tracciamento di un ordine verso, ad esempio, Google Analytics.

Da questo punto di vista infatti Clerk offre sia la possibilità di
tracciare il completamento dell'ordine lato client mediante
l'inserimento di un apposito script nella pagina di completamento
dell'ordine
(<https://help.clerk.io/it/integrations/any-webshop/get-started/> -
sezione "Aggiungi Tracciamento delle vendite"), sia la possibilità di
tracciare questo evento lato server.

In questo senso, come già visto anche nel precedente capitolo
"*Integrazione -- Ordini*", l'integrazione Passweb -- Clerk prevede già
il tracciamento degli ordini lato server mediante apposite chiamate API
per cui, come già per il tracciamento dei click, anche in questo caso
l'utente non dovrà preoccuparsi di nulla oltre al fatto di configurare
correttamente l'integrazione tra le due piattaforme

**ATTENZIONE! considerando che il tracciamento dei nuovi ordini viene
effettuato in automatico da Passweb lato server, non è necessario
inserire nella pagina di conferma ordine lo snippet di codice indicato
nella documentazione Clerk per il tracciamento lato client di questi
stessi ordini**

In relazione al tracciamento degli ordini c'è poi un'altra
considerazione molto importante da fare che riguarda, nello specifico,
la gestione degli articoli strutturati.

Considerando infatti come viene gestita questa particolare tipologia di
prodotti, nel momento in cui si dovesse decidere di visualizzare
all'interno dei moduli Clerk (ricerca o raccomandazioni non fa
differenza) solamente i padri di struttura potremmo ritrovarci in una
condizione tale per cui il click iniziale sul prodotto presente nel
modulo Clerk non corrisponda poi all'articolo effettivamente acquistato
dall'utente.

In questo caso infatti cliccando sull'articolo padre suggerito da Clerk
l'utente verrà ricondotto nella relativa pagina prodotto dove dovrà
impostare la configurazione desiderata individuando e mettendo in
carrello di fatto non l'articolo padre ma uno specifico articolo figlio.
Andando quindi a concludere l'ordine, l'articolo acquistato non
risulterà essere stato suggerito da Clerk (perché il click iniziale è
stato sull'articolo padre mentre quello acquistato e uno degli articoli
figlio) per cui l'impatto registrato ed assegnato a Clerk in questo caso
sarà nullo, anche se di fatto l'acquisto è stato originato proprio da
uno dei suoi suggerimenti.

Per far fronte a questa situazione è necessario agire sul parametro
"**Considera articoli padre nel tracciamento**" presente nella maschera
di configurazione dell'Account Clerk configurato sul backend di Passweb
(tab Ordini)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_feed_ordini_articoli_padre.bmp](./assets/media/image68.png){width="5.428472222222222in"
height="3.33125in"}

Attivando questo parametro infatti Passweb si comporterà come di seguito
indicato:

- cliccando su di un articolo padre presente in uno dei suggerimenti
  Clerk verrà correttamente registrato il click sul codice di questo
  stesso articolo

- l'utente verrà ricondotto nella pagina prodotto del padre dove dovrà
  configurare un articolo figlio (quindi con codice diverso da quello
  del padre)

- selezionata la configurazione desiderata metterà in carrello lo
  specifico articolo figlio e andrà poi a concludere l'ordine

- in fase di invio dell'ordine a Clerk (o in fase di creazione del feed
  json) Passweb verificherà il valore del parametro "Considera articoli
  padre nel tracciamento" e, trovandolo attivato, invece di inviare a
  Clerk il codice dell'articolo figlio effettivamente inserito in ordine
  invierà quello del corrispondente articolo padre. Il prezzo inviato a
  Clerk sarà invece sempre quello dell'articolo figlio effettivamente
  acquistato

In questo modo avremo perfetta corrispondenza tra il click iniziale e il
codice articolo inserito in ordine per cui Clerk riuscirà a registrare
correttamente il fatto che la vendita è stata originata da un suo
suggerimento calcolandone anche il relativo impatto.

Il risvolto negativo, in tutto ciò, è rappresentato ovviamente dal fatto
che nel dettaglio dell'ordine presente su Clerk sarà indicato il codice
dell'articolo padre per cui, lato Clerk, non avremo più traccia (se non
per il prezzo) dell'articolo figlio effettivamente acquistato.

**ATTENZIONE! questa opzione dovrà essere attivata solo ed
esclusivamente nel momento in cui si sia deciso di visualizzare
all'interno dei suggerimenti Clerk (sia quelli iniettati / embeddati che
quelli gestiti con il componente "Popolarità Prodotto") i soli articoli
padri di struttura**

Di contro ovviamente, lasciando il parametro "Considera articoli padre
nel tracciamento" deselezionato, per essere sicuri di avere poi
un'esatta corrispondenza tra il click iniziale e il codice articolo
effettivamente inserito in ordine dovremo assicurarci di visualizzare in
tutti i moduli Clerk (sia quelli iniettati / embeddati che quelli
gestiti con il componente "Popolarità Prodotto") i soli articoli figlio.

**TRACCIAMENTO DELLE PAGINE PRODOTTO**

Oltre ai click sui suggerimenti offerti e al completamento di un ordine,
a Clerk può servire conoscere anche quelli che sono i prodotti
visualizzati dagli utenti indipendentemente dal fatto che la visita alla
pagina prodotto sia stata originata o meno da uno dei suoi suggerimenti.

Come per il completamento dell'ordine anche la visualizzazione di una
pagina prodotto può non avere interazione diretta con un modulo Clerk
per cui questo tipo di tracciamento non potrà essere gestito
automaticamente da Clerk.js.

In questo senso dunque il suggerimento (indicato direttamente dalla
documentazione Clerk
<https://help.clerk.io/it/integrations/any-webshop/get-started/> ) è
quello di **inserire in tutte le pagine prodotto il seguente snippet di
codice**

\<span

class=\"clerk\"

data-api=\"log/product\"

data-product=\"**{{SKU}}**\"\>

\</span\>

dove {{SKU}} è il segnaposto del "**Codice Articolo**" disponibile nella
maschera di configurazione del componente HTML che dovrà essere
utilizzato per inserire nelle varie pagine prodotto lo snippet in esame

**AGGIUNTA ARTICOLI IN CARRELLO**

L'aggiunta di articoli in carrello è un altro evento che può essere
tracciato, anche se tale evento verrà considerato più che altro
nell'ambito dell'integrazione con il modulo Email che, come indicato nei
precedenti capitoli, al momento, non prevede però integrazioni native
con il sito Passweb.

In ogni caso una volta attivato il modulo Clerk l'evento di aggiunta in
Carrello verrà automaticamente inviato a Clerk (via javascript) secondo
quanto descritto nella relativa documentazione (
<https://docs.clerk.io/docs/clerkjs-shopping-cart> ) per cui, anche in
questo caso, l'utente non dovrà preoccuparsi di nulla.

