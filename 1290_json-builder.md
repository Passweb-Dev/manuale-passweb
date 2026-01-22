# JSON-BUILDER



Come già evidenziato nei precedenti capitoli di questo manuale i check
presenti in corrispondenza del parametro "**Proprietà gestite**"
(pannello "**Dati Strutturati**") consentono di attivare solo una parte
delle proprietà disponibili per lo Schema Product, nello specifico,
quelle gestite in automatico da Passweb su cui l'utente non avrebbe
possibilità di intervento se non optando per un inserimento manuale di
tutto il JSON-LD all'interno di ogni singola scheda prodotto.

Nel momento in cui l'esigenza dovesse essere dunque quella di integrare
il JSON-LD gestito in automatico da Passweb aggiungendo altre proprietà,
relative sempre allo Schema Product, ma diverse da quello che può essere
il titolo, la descrizione, il prezzo, la disponibilità ecc... sarà
necessario utilizzare il JSON Builder presente all'interno della sezione
"**Struttura JSON-LD**" evidenziata in figura

![](./assets/media/image5.png)

Analizzando infatti il vocabolario di Schema.org in relazione alle
proprietà disponibili per lo Schema Product
(<https://schema.org/Product>), si nota facilmente come potremmo
trovarci a dover gestire delle proprietà semplici del tipo
"chiave:valore" ma anche delle proprietà rappresentate con strutture
dati più complesse come array, oggetti, array di oggetti. In questi casi
per non ottenere poi degli errori in fase di validazione del JSON-LD,
cosa questa che ci impedirebbe di comunicare correttamente al motore di
ricerca piuttosto che ad un qualunque altro sistema automatico le
informazioni sui prodotti presenti all'interno del sito, con tutte le
conseguenze del caso, dovremo integrare i dati gestiti in automatico da
Passweb replicando esattamente la struttura per essi richiesta dal
vocabolario di Schema.org.

La sezione "**Struttura JSON-LD**" sopra evidenziata consente proprio di
fare tutto ciò. L'unico vincolo, in questo senso, è rappresentato dal
fatto di non poter modificare o integrare le proprietà gestite
direttamente da Passweb

**ATTENZIONE!** tramite il Json Builder è possibile gestire solamente
proprietà a livello Product (inserite cioè nel JSON-LD allo stesso
livello di *\"@type\": \"Product\")* che non siano già gestite tramite
uno dei check presenti all'interno del pannello "Dati Strutturati"

I pulsanti presenti all'interno di questa sezione consentono
rispettivamente di:

**Pulisci Struttura** (
![](./assets/media/image10.png) ): consente di azzerare la struttura
dati che si sta realizzando

**Esporta JSON** (
![](./assets/media/image11.png) ): consente di esportare la struttura
dati in esame all'interno di un file JSON

**Importa JSON da file** (
![](./assets/media/image12.png) ): consente di creare automaticamente
una struttura dati più o meno complessa importandola direttamente da un
file JSON correttamente strutturato.

**Aggiungi nodo** (
![](./assets/media/image13.png) ): consente di aggiungere alla struttura
del JSON-LD un nuovo nodo di tipo radice che verrà quindi inserito allo
stesso livello di *\"@type\", \"name\", \"description\"* ... dopo quelle
che sono le proprietà gestite in automatico da Passweb

I campi visualizzati dopo aver cliccato su questo pulsante consentono di
indicare, rispettivamente:

- il nome della proprietà da codificare -- campo "**Elemento chiave**"

- la struttura dati con cui dovrà essere gestita (se è una proprietà
  semplice oppure se dovrà essere gestita come un oggetto, come un array
  ...) -- campo "**Tipo**"

- la tipologia di campo Passweb con cui dovrà eventualmente essere
  mappata -- campo "**Sorgente valore**"

- il valore personalizzato, il campo o l'attributo Passweb da cui
  dovranno essere prelevati i valori da assegnare, articolo per
  articolo, alla proprietà in esame -- campo "**Seleziona
  campo/attributo ...**"

Il campo "**Preview Json**" consente invece di visualizzare in tempo
reale la struttura dati che si sta realizzando.

**ATTENZIONE!** il vocabolario cui fare riferimento per sapere
esattamente quello che dovrà essere il nome da assegnare alla proprietà,
la struttura dati con cui dovrà essere gestita e i possibili valori che
dovrà assumere è, ovviamente, sempre quello di Schema.org

In particolare per quel che riguarda **le diverse tipologie di strutture
dati che potranno essere inserite all'interno del JSON-LD,** è possibile
selezionare una delle seguenti opzioni:

- **Valore Semplice**: da selezionare nel caso in cui la proprietà da
  inserire nel JSON-LD dovesse essere gestita con una struttura dati
  "semplice"

![](./assets/media/image14.png)

> del tipo
>
> ***"nome proprietà" : "valore"***
>
> In queste condizioni **valore** potrà essere sia un valore semplice
> (tipicamente una stringa) che un array (di stringhe o di numeri). In
> quest'ultimo caso, in particolare, sarà poi necessario mappare la
> proprietà in esame con un Campo o un Attributo Passweb a valori
> multipli

- **Array di stringhe / Array di numeri**: da selezionare nel caso in
  cui la proprietà da inserire nel JSON-LD dovesse essere gestita come
  un Array di stringhe / Array di numeri

![](./assets/media/image15.png)

> quindi con una struttura dati del tipo
>
> ***"nome proprietà":\['valore1','valore2', ...'valoreN'\]*** oppure
> ***"nome proprietà":\[numero1,numero2, ...numeroN\]***
>
> dove però gli elementi dell'array non possono essere prelevati da un
> unico Campo / Attributo Passweb a valori multipli, ma dovranno invece
> essere prelevati da singoli Campi / Attributi Passweb ad un solo
> valore ciascuno
>
> In questo caso infatti, una volta impostato il campo "**Tipo**"
> sull'opzione "**Array di stringhe**" o "**Array di numeri**" non
> verranno visualizzati gli ulteriori campi **"Sorgente valore**" e
> "**Seleziona campo/attributo ...**" e al loro posto comparirà invece
> il pulsante "**Aggiungi stringa / numero**" (
> ![](./assets/media/image16.png) ).
>
> Cliccando su questo pulsante sarà quindi possibile aggiungere
> all'array, in maniera manuale, i singoli elementi impostando un
> mapping specifico per ciascuno di essi

![](./assets/media/image17.png)

- **Oggetto**: da selezionare nel caso in cui la proprietà da inserire
  nel JSON-LD dovesse essere gestita come un oggetto

![](./assets/media/image18.png)

> e quindi con una struttura dati del tipo
>
> ***"nome proprietà" {***
>
> ***"proprietà oggetto\": "valore proprietà",***
>
> ***\"proprietà oggetto\": "valore proprietà",***
>
> ***\" proprietà oggetto\": "valore proprietà"***
>
> ***...***
>
> ***}***
>
> in cui la proprietà in esame potrà avere a sua volta diverse altre
> proprietà ognuna delle quali dovrà essere indicata con una sintassi
> del tipo ***"proprietà oggetto\": "valore proprietà"***
>
> Anche in questo caso dunque, selezionando come tipologia di struttura
> dati l'opzione "Oggetto", non verranno visualizzati immediatamente i
> campi **"Sorgente valore**" e "**Seleziona campo/attributo ...**" e al
> loro posto comparirà invece il pulsante "**Aggiungi proprietà**" (
> ![](./assets/media/image19.png) ) grazie al quale poter aggiungere, in
> maniera manuale, le singole proprietà dell'oggetto effettuando anche
> per ciascuna di esse uno specifico mapping con i Campi o gli Attributi
> Passweb da cui prelevare i relativi valori.

![](./assets/media/image20.png)

> **ATTENZIONE!** se necessario è possibile creare anche strutture dati
> più complesse come ad esempio, un oggetto di array o un oggetto di
> oggetti

- **Array di oggetti**: da selezionare nel caso in cui la proprietà da
  inserire nel JSON-LD dovesse essere gestita come un array di oggetti

![](./assets/media/image21.png)

> e quindi con una struttura dai del tipo
>
> ***"nome proprietà":\[***
>
> ***{***
>
> ***"nome proprietà\": "valore proprietà",***
>
> ***\" nome proprietà\": "tipo proprietà",***
>
> ***\" nome proprietà\": "tipo proprietà"***
>
> ***...***
>
> ***},***
>
> ***{***
>
> ***"nome proprietà\": "valore proprietà",***
>
> ***\" nome proprietà\": "tipo proprietà",***
>
> ***\" nome proprietà\": "tipo proprietà"***
>
> ***...***
>
> ***},***
>
> ***....***
>
> ***\]***
>
> Anche in questo caso una volta impostato il campo "**Tipo**"
> sull'opzione "**Array di oggetti**" comparirà il pulsante "**Aggiungi
> Elemento**" (
> ![](./assets/media/image22.png) ) grazie al quale poter aggiungere, in
> maniera manuale, i singoli oggetti all'array.

![](./assets/media/image23.png)

> I due pulsante "**Aggiungi proprietà**" (
> ![](./assets/media/image19.png) ) e "**Rimuovi proprietà**" (
> ![](./assets/media/image24.png) ) consentiranno invece di definire la
> struttura e mappare con i relativi Campi / Attributi Passweb le
> proprietà di ogni oggetto dell'Array

![](./assets/media/image25.png)

Per quel che riguarda invece **la tipologia di campo Passweb** **con cui
poter mappare le varie proprietà** è possibile selezionare una delle
seguenti opzioni:

![](./assets/media/image26.png)

- **Valore Personalizzato:** in questo caso sarà possibile indicare
  esplicitamente, all'interno del successivo campo di input
  ("**Inserisci valore**") il valore che dovrà assumere la proprietà in
  esame

> **ATTENZIONE!** in queste condizioni il valore indicato in
> corrispondenza dell'opzione "Personalizzato" sarà ovviamente lo stesso
> per tutti gli articoli presenti all'interno del sito
>
> Nel caso in cui l'esigenza dovesse essere quella di creare un qualcosa
> di più dinamico, dove la proprietà indicata possa assumere un valore
> diverso per ogni singolo prodotto, sarà quindi necessario optare per
> l'opzione "**Campo Articolo**" o "**Attributo**"

- **Campo Articolo:** in questo caso sarà possibile indicare il campo da
  cui prelevare il valore della proprietà in esame selezionandolo tra
  quelli dell'anagrafica articolo Passweb visualizzati in corrispondenza
  del campo "**Seleziona campo...**"

- **Attributo:** in questo caso sarà possibile indicare il campo da cui
  prelevare il valore della proprietà in esame selezionandolo tra gli
  Attributi Passweb visualizzati in corrispondenza del campo
  "**Seleziona attributo...**"

Nei successivi capitoli di questo manuale andremo ad esaminare due
semplici esempi di come poter utilizzare al meglio il Json Builder per
integrare il JSON-LD gestito in automatico da Passweb rispettivamente
con una proprietà "semplice" e con una proprietà gestita invece con una
struttura dati più complessa come quella di un oggetto.

