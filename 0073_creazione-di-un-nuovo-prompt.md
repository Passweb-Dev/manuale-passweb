# CREAZIONE DI UN NUOVO PROMPT



Come indicato nel precedente capitolo di questo manuale un Prompt altro
non è se non un'istruzione, o meglio un insieme di istruzioni, da
fornire al modello di intelligenza artificiale per farle generare il più
rapidamente possibile dei contenuti che siano anche il più coerenti
possibile con lo specifico campo per cui è stata effettivamente
richiesta la generazione di questi stessi contenuti.

Per creare un nuovo Prompt potremmo partire da uno dei Prompt
predefiniti messi a disposizione da Passweb (per maggiori informazioni
in merito a questa possibilità si veda il successivo capitolo di questo
manuale) oppure potremmo anche decidere di crearne uno da zero.

In quest'ultimo caso, per creare da zero uno nuovo Prompt, sarà
sufficiente cliccare sul pulsante "**Aggiungi**" presente nella barra
degli strumenti della maschera "Prompt Template"

![](./assets/media/image383.png)

In questo modo verrà infatti visualizzata la maschera "**Nuovo
Template**"

![Videate\\passweb_ai_nuovo_prompt.bmp](./assets/media/image384.png)

all'interno della quale poter indicare un valore per i seguenti
parametri:

**Titolo**: consente di assegnare un nome al prompt che si sta
realizzando

**Descrizione**: consente di assegnare una descrizione al prompt che si
sta realizzando

**Modello:** consente di indicare, selezionandolo da un apposito menu a
tendina, il modello di AI da associare al prompt in esame e che verrà
quindi utilizzato per generare il relativo contenuto

**ATTENZIONE!** a seconda del modello selezionato, a fronte della stessa
domanda e quindi dello stesso prompt, si potranno ottenere risultati
diversi e, soprattutto, si dovranno anche sostenere costi diversi.

A titolo puramente esemplificativo vengono riportate di seguito alcune
caratteristiche dei vari modelli gestiti dal modulo Passweb. **In ogni
caso, per informazioni più dettagliate ed aggiornate, soprattutto sui
prezzi, si consiglia di fare sempre riferimento a quanto indicato
direttamente sul sito di OpenAI**

- **[GPT-4o]{.underline}**

> E' una versione ottimizzata di GPT-4, progettata per essere più veloce
> e meno costosa rispetto al modello GPT-4 standard.
>
> È stato ottimizzato per ridurre i tempi di risposta e le risorse
> computazionali, il che si traduce in costi inferiori per gli utenti
> API e migliori performance in termini di velocità.
>
> È particolarmente vantaggioso per applicazioni ad alto volume che
> richiedono una versione potente di GPT-4 ma a un costo più
> accessibile.
>
> GPT-4-turbo offre anche opzioni di contesto espanso (come le versioni
> da 8k e 32k token), consentendo di gestire conversazioni o documenti
> più lunghi.
>
> **Costo di GPT-4o**:

- 8K context (fino a circa 8.000 token): \$0.03 per 1k token (input) e
  \$0.06 per 1k token (output).

- 32K context (fino a circa 32.000 token): \$0.06 per 1k token (input) e
  \$0.12 per 1k token (output).

> **ATTENZIONE!** In considerazione di quanto detto GPT-4o è il modello
> consigliato per l'uso commerciale e quotidiano, poiché mantiene la
> potenza del modello GPT-4 con maggiore efficienza e costi ridotti ed è
> quindi anche **il modello che verrà utilizzato da Passweb come default
> nel momento in cui si dovesse utilizzare l'AI per generare contenuti a
> partire da campi cui non è stato associato nessun tipo di Template**

- **[GPT-3.5]{.underline}**

> E' la versione precedente di Chat GPT, meno preciso rispetto a GPT-4°
> e tende a commettere errori più spesso
>
> Anche se comunque sufficientemente potente, GPT-3.5 può mancare di
> dettagli o fraintendere richieste complesse.
>
> È meno capace nei compiti che richiedono ragionamenti complessi o
> multi-step. Sebbene sia comunque creativo, tende a fornire risposte
> più semplici e meno dettagliate rispetto a GPT-4o
>
> A un limite di contesto inferiore (circa 4,000 token) rispetto a
> GPT-4o, quindi può perdere parte del filo del discorso in
> conversazioni lunghe, costringendo spesso a riepilogare i dettagli in
> discussioni estese.
>
> A livello di costi è comunque più economico di GPT-4o per cui lo si
> può ritenere un ottimo modello per domande meno complesse, in cui il
> costo e la velocità sono più importanti della qualità e accuratezza
> delle risposte
>
> **Costo di GPT-3.5**:

- \$0.0015 per 1k token (input)

- \$0.002 per 1k token (output).

<!-- -->

- **[MODELLI PIÙ VECCHI (ES. GPT-3 - DAVINCI, CURIE, BABBAGE,
  ADA)]{.underline}**

> Sebbene meno avanzati rispetto a GPT-4 e GPT-3.5-turbo, OpenAI offre
> ancora alcuni dei modelli GPT-3 originali con prezzi variabili:

- Davinci: \$0.02 per 1k token (il più potente dei modelli GPT-3).

- Curie: \$0.002 per 1k token.

- Babbage: \$0.0005 per 1k token.

- Ada: \$0.0004 per 1k token (il modello più economico e rapido di
  GPT-3)

- ...

**Categoria**: consente di indicare la categoria di contenuto cui dovrà
essere associato il prompt in esame. E' possibile selezionare uno dei
seguenti valori

- **Prodotto:** in questo caso il prompt in esame potrà essere
  utilizzato per generare contenuti sui prodotti in vendita all'interno
  del sito e potrà quindi essere associato a determinati campi articolo

- **CMS**: in questo caso il prompt in esame potrà essere utilizzato per
  generare contenuti relativi ai post CMS pubblicati all'interno del
  sito e potrà quindi essere associato a determinati campi CMS

- **Generico**: in questo caso il prompt in esame potrà essere
  utilizzato per generare contenuti generici come ad esempio contenuti
  da inserire all'interno di un componente Paragrafo, codice CSS o
  Javascript da utilizzare nelle apposite sezioni dei layout in uso al
  sito o ancora codice HTML da utilizzare all'interno del relativo
  componente Passweb.

Come si può facilmente comprendere, a seconda della categoria
selezionata potranno cambiare anche i parametri di configurazione del
prompt come ad esempio i campi a cui potranno essere associati e su cui
si potranno effettivamente utilizzare per porre domande alla AI.

Una volta impostati quindi Titolo, Descrizione, Modello e Categoria
(tutti parametri obbligatori), cliccando sul pulsante "**Salva**"
verranno visualizzati altri parametri di configurazione del prompt,
coerenti con la categoria effettivamente selezionata, e anch'essi
indispensabili per completare la definizione del prompt stesso

![](./assets/media/image385.png)

In particolare dunque il parametro:

**Template di default -- disponibile solo per template di categoria
Prodotto o CMS**: consente, se selezionato, impostare il prompt in esame
come prompt di default per i campi cui verrà poi associato.

**ATTENZIONE!** il prompt di default è strettamente collegato alla
funzionalità "One Click" utilizzabile in fase di generazione dei
contenuti.

Per maggiori informazioni in merito si veda il relativo capitolo
("*Generazione di Contenuti One Click*") di questo manuale

**Campi di destinazione**: consente di selezionare i campi a cui
associare il prompt in esame.

I campi di ricerca presenti immediatamente al di sopra di entrambi i box
consentono, digitando almeno 3 caratteri, di filtrare gli elementi
presenti in elenco.

Per associare il prompt ad un determinato campo è sufficiente
selezionarlo dal box di sinistra ed inserirlo in quello di destra
cliccando sul pulsante raffigurante una piccola freccia verde.

Allo stesso modo per eliminare un'associazione "campo -- template" è
sufficiente selezionare il campo in esame dal box di destra e
reinserirlo in quello di sinistra cliccando sul pulsante raffigurante
una piccola freccia rossa

**ATTENZIONE!** i campi visualizzati in corrispondenza di questo
parametro variano in relazione alla specifica categoria assegnata al
prompt stesso.

In particolare i prompt della categoria "Prodotto" potranno essere
associati e potranno quindi essere utilizzati per generare il contenuto
dei seguenti campi:

- **Descrizione Articolo** -- campo "Descrizione" dell'anagrafica
  articolo Passweb

- **Descrizione Dettagliata** -- campo "Descrizione Dettagliata"
  dell'anagrafica articolo Passweb

- **Descrizione HTML / 2 / 3** -- campi Descrizione HTML, Descrizione
  HTML2 e Descrizione HTML3 dell'anagrafica articolo Passweb

- **Descrizione della categoria Merceologica** -- campo "Descrizione"
  dell'anagrafica Passweb delle categorie merceologiche

I prompt della categoria CMS potranno invece essere associati e quindi
utilizzati sui seguenti campi

- **Titolo** -- campo "Titolo" nella maschera di creazione di un
  contenuto CMS

- **Sommario** -- campo "Sommario" nella maschera di creazione di un
  contenuto CMS

- **Testo** -- campo "Contenuto" nella maschera di creazione di un
  contenuto CMS

- **Descrizioni 1 / 2 / 3** -- campi "Descrizione 1 / 2 / 3" nella
  maschera di creazione di un contenuto CMS (sezione "Ulteriori
  Contenuti")

- **Descrizione della categoria** -- campo "Descrizione" della categoria
  CMS

- **Tag Associati** -- campo "Tag Associati" nella maschera di creazione
  di un contenuto CMS (sezione "Associazioni").

> **ATTENZIONE!** In questo caso andrebbe poi chiesto all'AI di generare
> i valori separati da , in modo tale che questi possano poi essere
> inseriti come Tag distinti
>
> I prompt della categoria SEO potranno invece essere associati e quindi
> utilizzati sui seguenti campi:

- **Articolo -- Description Meta --** campo "Description Meta"
  dell'anagrafica articolo Passweb (sezione "SEO -- Sitemap")

- **Articolo -- Meta Keywords: --** campo "Keywords Meta"
  dell'anagrafica articolo Passweb (sezione "SEO -- Sitemap")

- **Articolo -- Title: --** campo "Title" dell'anagrafica articolo
  Passweb (sezione "SEO -- Sitemap")

- **Categoria -- Description Meta --** campo "Description Meta"
  dell'anagrafica Passweb delle categorie merceologiche (sezione "SEO --
  Sitemap")

- **Categoria -- Meta Keywords: --** campo "Keywords Meta"
  dell'anagrafica Passweb delle categorie merceologiche (sezione "SEO --
  Sitemap")

- **Categoria -- Title: --** campo "Title" dell'anagrafica
  dell'anagrafica Passweb delle categorie merceologiche (sezione "SEO --
  Sitemap")

- **CMS -- Description--** campo "Description Meta" di un contenuto CMS
  (sezione "SEO -- Sitemap")

- **CMS -- Keywords: --** campo "Keywords Meta" di un contenuto CMS
  (sezione "SEO -- Sitemap")

- **CMS -- Title: --** campo "Title" di un contenuto CMS (sezione "SEO
  -- Sitemap")

- **Pagina -- Description--** campo "Description" nella proprietà di una
  pagina generica

- **Pagina -- Keywords: --** campo "Keywords" nella proprietà di una
  pagina generica

- **Pagina -- Title: --** campo "Title" nella proprietà di una pagina
  generica

I prompt della categoria "Generica", infine, potranno essere associati e
quindi utilizzati sui seguenti campi:

- **Componente Paragrafo** -- campo "Contenuto" presente nella maschera
  di configurazione del componente "Paragrafo"

- **Componente HTML** -- campo "HTML" presente nella maschera di
  configurazione del componente "HTML"

- **Layout** -- sezioni CSS e Javascript presenti nella maschera di
  configurazione dei vari layout in uso al sito

**ATTENZIONE!** nel caso in cui il template in esame dovesse essere
stato impostato come Template di Default sarà obbligatorio accertarsi
che i campi ad esso associati non siano già stati utilizzati in un altro
Template di Default. **Ogni singolo campo potrà infatti avere un solo
Template di Default**

In ogni caso nel momento in cui si tentasse di associare ad uno stesso
campo a due diversi Template di Default, in fase di salvataggio verrà
visualizzato un apposito messaggio di errore.

**Prompt System**: consente di definire il prompt di sistema, vale a
dire, l'insieme delle istruzioni che il modello di AI selezionato dovrà
poi seguire nel generare il contenuto richiesto.

Le istruzioni in questione possono essere fornite in linguaggio naturale
e sono di fondamentale importanza per ottenere risposte che siano il più
possibile precise e coerenti con la tipologia di contenuto richiesto.

In questo senso Passweb fornisce già, per ogni template gestito, un
Prompt di sistema predefinito, che varia in relazione alla categoria,
che può essere applicato in un qualsiasi momento cliccando sul pulsante
"**Default**" presente immediatamente al di sotto del campo in esame e
che tende anche ad eliminare, dalla risposta fornita dal modello,
eventuale testo in eccesso e non necessario (come eventuali frasi
introduttive e conclusive) in maniera tale da limitare, per quando
possibile, i costi di utilizzo.

![](./assets/media/image386.png)

Nello specifico:

- per i template della categoria "**Prodotto**", cliccando sul pulsante
  "**Default**", verrà proposto il seguente prompt di sistema:

> "*Sei uno specialista di e-commerce che vende prodotti \[\[INDICARE LA
> TIPOLOGIA DI PRODOTTI VENDUTI\]\] e la tua specialità è scrivere
> descrizioni di prodotti persuasive e SEO-friendly. La descrizione
> risultante deve convincere gli utenti che stanno cercando di
> acquistare online, deve avere un numero massimo di parole di
> \[\[INDICARE IL NUMERO DESIDERATO\]\] parole, il tono della
> descrizione dovrà essere informativo ma persuasivo e lo stile di
> scrittura dovrà essere adattato a un pubblico di potenziali
> acquirenti. I paragrafi all\'interno di ciascuna descrizione devono
> essere facili da leggere e utilizzare spazi vuoti, punti, virgole ed
> elenchi per raggiungere questo obiettivo. È necessario fornire il
> contenuto \[\[in formato HTML senza delimitatori di codice come
> \`\`\`html\]\] \[\[in formato testuale senza l'utilizzo di codice
> HTML\]\]. Ricorda che lo scopo di questa descrizione è incentivare
> l'acquisto del prodotto. Per favore rispondi sempre con la risposta
> senza utilizzare frasi introduttive o conclusive, non ripetere le
> istruzioni, non ricordare le istruzioni precedenti, non scusarsi, non
> fare riferimento a te stesso in nessun momento e non fare
> supposizioni*."
>
> **ATTENZIONE!** considerando che, ovviamente, è impossibile definire
> un prompt di sistema immediatamente utilizzabile per tutte le
> tipologie di prodotto e per tutti i campi articolo in cui poter
> utilizzare le funzioni generative dell'AI, **il prompt di sistema
> della categoria "Prodotto" andrà di volta in volta adattato alle
> specifiche esigenze del caso.**
>
> In particolare nel prompt di sistema fornito da Passweb per i template
> della categoria "Prodotto", il testo racchiuso tra \[\[ \]\] andrà
> sostituito esattamente con la tipologia di prodotti venduti piuttosto
> che con il nome dello specifico articolo o ancora con l'eventuale
> numero massimo di caratteri da utilizzare per la risposta.
>
> Allo stesso modo nel momento in cui l'esigenza dovesse essere quella
> di ottenere delle risposte in formato HTML, nel prompt indicato andrà
> utilizzata la frase "*È necessario fornire il contenuto in formato
> HTML senza delimitatori di codice come \`\`\`html*"
>
> Nel momento in cui l'esigenza dovesse invece essere quella di ottenere
> delle risposte semplici in formato testuale andrà utilizzata la frase
> "*È necessario fornire il contenuto in formato testuale senza
> l'utilizzo di codice HTML*"

- per i template della categoria "**CMS**", cliccando sul pulsante
  "**Default**", verrà proposto il seguente prompt di sistema

> "*Sei uno scrittore esperto con la capacità di creare post di blog
> altamente coinvolgenti che catturino l'attenzione del tuo pubblico e
> offrano valore. Raccogli ispirazione da altri articoli di successo
> relativi allo stesso argomento per assicurarti di non tralasciare
> punti e sezioni importanti. Utilizza le migliori pratiche SEO per
> garantire un uso corretto delle parole chiave nei titoli.*
>
> *Rispondi fornendo il contenuto in formato HTML senza delimitatori di
> codice come \`\`\`html. Ricorda che lo scopo principale è quello di
> fornire contenuti sull'argomento indicato che possano rendere
> l'articolo facilmente rintracciabile. Per favore rispondi sempre con
> la risposta senza utilizzare frasi introduttive o conclusive, non
> ripetere le istruzioni, non ricordare le istruzioni precedenti, non
> scusarsi, non fare riferimento a te stesso in nessun momento e non
> fare supposizioni*."

- per i template della categoria "**SEO**", cliccando sul pulsante
  "**Default**", verrà proposto il seguente prompt di sistema

> "*Sei un esperto di pratiche SEO. Utilizza le migliori pratiche SEO
> per garantire risposte efficaci. Raccogli ispirazione da altri siti
> che risultano essere posizionati in maniera ottimale*
>
> *Per favore rispondi sempre con la risposta senza utilizzare frasi
> introduttive o conclusive, non ripetere le istruzioni, non ricordare
> le istruzioni precedenti, non scusarsi, non fare riferimento a te
> stesso in nessun momento e non fare supposizioni*"

- per i template della categoria "Generico", cliccando sul pulsante
  "Default" verrà proposto il seguente prompt di sistema

> *"Rispondi sempre solo con la risposta, senza frasi introduttive o
> conclusive. In caso di risposte HTML, rispondi sempre solo con il
> codice HTML senza delimitatori di codice come \`\`\`html***"**

Ovviamente tutti i prompt di sistema forniti da Passweb potranno sempre
essere personalizzati secondo le specifiche esigenze del caso.

Un'ultima considerazione di fondamentale importanza da fare è quella che
riguarda i siti multilingua. **Per questi siti, di base, sarà infatti
necessario impostare un prompt di sistema per ciascuna delle lingue
gestite**

Nel momento in cui l'esigenza dovesse essere, dunque, quella di generare
del contenuto sia in Italiano che in Inglese le istruzioni su come
rispondere dovranno essere fornite al modello di AI sia in Italiano che
in Inglese.

In realtà anche se **il consiglio è quello di definire sempre il prompt
di sistema nella specifica lingua di utilizzo**, volendo, anche per
l'inglese si potrebbe provare a scrivere comunque il prompt in lingua
Italiana, indicando però al modello di AI come istruzione aggiuntiva, di
rispondere in Inglese

Esempio:

"*Sei uno specialista di e-commerce che vende prodotti \[\[INDICARE LA
TIPOLOGIA DI PRODOTTI VENDUTI\]\] e la tua specialità è scrivere
descrizioni di prodotti persuasive. Il tuo compito è scrivere una
descrizione SEO-friendly per il prodotto \[\[NOME\]\]. La descrizione
risultante deve convincere gli utenti che stanno cercando di acquistare
un \[\[NOME\]\] online, deve avere un numero massimo di parole di
\[\[INDICARE IL NUMERO DESIDERATO\]\] parole, il tono della descrizione
dovrà essere informativo ma persuasivo e lo stile di scrittura dovrà
essere adattato a un pubblico di potenziali acquirenti. I paragrafi
all\'interno di ciascuna descrizione devono essere facili da leggere e
utilizzare spazi vuoti, punti, virgole ed elenchi per raggiungere questo
obiettivo. È necessario fornire il contenuto \[\[in formato HTML senza
delimitatori di codice come \`\`\`html\]\] \[\[in formato testuale senza
l'utilizzo di codice HTML\]\]. Ricorda che lo scopo di questa
descrizione è incentivare l'acquisto del prodotto. **Per favore rispondi
in Inglese**, senza utilizzare frasi introduttive o conclusive, non
ripetere le istruzioni, non ricordare le istruzioni precedenti, non
scusarsi, non fare riferimento a te stesso in nessun momento e non fare
supposizioni*."

**Prompt**: consente di impostare la domanda che dovrà poi essere
inoltrata al modello di intelligente artificiale.

Come per il prompt di sistema il consiglio, per i siti multilingua, è
sempre quello di impostare la domanda in ciascuna delle lingue
effettivamente gestite. Anche in questo caso però si potrebbe provare a
formulare la domanda sempre in italiano indicando poi al modello in
maniera esplicita di rispondere nella lingua desiderata.

Per i prompt della categoria "Prodotto" è possibile utilizzare, in fase
di compilazione della domanda uno dei segnaposto messi a disposizione da
Passweb.

![](./assets/media/image387.png)

I segnaposto inseriti verranno poi valorizzati in maniera dinamica, in
fase di generazione del contenuto, con il valore del corrispondente
campo dell'articolo in relazione al quale è stata posta la domanda

E' possibile utilizzare uno dei seguenti segnaposto:

- Codice Articolo

- Codice Alternativo

- Titolo Articolo

- Descrizione

- Descrizione Dettagliata

- Descrizione HTML / 2 / 3

- Attributi articolo

Infine, anche in questo caso Passweb mette già a disposizione
dell'utente, per ciascuna delle categorie gestite, una serie di prompt
predefiniti accessibili cliccando sul relativo pulsante (**Prompt
Predefiniti**) presente nella barra degli strumenti (per maggiori
informazioni in merito si veda il successivo capitolo di questo manuale)

