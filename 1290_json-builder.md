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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder.bmp](./assets/media/image5.png){width="5.370138888888889in"
height="3.636111111111111in"}

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
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_pulisci_struttura.bmp](./assets/media/image10.png){width="0.8444444444444444in"
height="0.24027777777777778in"} ): consente di azzerare la struttura
dati che si sta realizzando

**Esporta JSON** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_json.bmp](./assets/media/image11.png){width="0.7854166666666667in"
height="0.24027777777777778in"} ): consente di esportare la struttura
dati in esame all'interno di un file JSON

**Importa JSON da file** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_json.bmp](./assets/media/image12.png){width="1.0256944444444445in"
height="0.23402777777777778in"} ): consente di creare automaticamente
una struttura dati più o meno complessa importandola direttamente da un
file JSON correttamente strutturato.

**Aggiungi nodo** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_nodo.bmp](./assets/media/image13.png){width="0.83125in"
height="0.24027777777777778in"} ): consente di aggiungere alla struttura
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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_campi_nodo.bmp](./assets/media/image14.png){width="5.370138888888889in"
height="3.636111111111111in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_array.bmp](./assets/media/image15.png){width="5.370138888888889in"
height="3.636111111111111in"}

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
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_stringa.bmp](./assets/media/image16.png){width="0.66875in"
> height="0.2013888888888889in"} ).
>
> Cliccando su questo pulsante sarà quindi possibile aggiungere
> all'array, in maniera manuale, i singoli elementi impostando un
> mapping specifico per ciascuno di essi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_array_2.bmp](./assets/media/image17.png){width="5.370138888888889in"
height="3.636111111111111in"}

- **Oggetto**: da selezionare nel caso in cui la proprietà da inserire
  nel JSON-LD dovesse essere gestita come un oggetto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_oggetto.bmp](./assets/media/image18.png){width="5.532638888888889in"
height="3.415277777777778in"}

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
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_proprieta.bmp](./assets/media/image19.png){width="0.7465277777777778in"
> height="0.2013888888888889in"} ) grazie al quale poter aggiungere, in
> maniera manuale, le singole proprietà dell'oggetto effettuando anche
> per ciascuna di esse uno specifico mapping con i Campi o gli Attributi
> Passweb da cui prelevare i relativi valori.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_oggetto_2.bmp](./assets/media/image20.png){width="5.370138888888889in"
height="3.636111111111111in"}

> **ATTENZIONE!** se necessario è possibile creare anche strutture dati
> più complesse come ad esempio, un oggetto di array o un oggetto di
> oggetti

- **Array di oggetti**: da selezionare nel caso in cui la proprietà da
  inserire nel JSON-LD dovesse essere gestita come un array di oggetti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_array_oggetti_0.bmp](./assets/media/image21.png){width="5.350694444444445in"
height="3.623611111111111in"}

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
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_elemento_1.bmp](./assets/media/image22.png){width="0.7534722222222222in"
> height="0.2013888888888889in"} ) grazie al quale poter aggiungere, in
> maniera manuale, i singoli oggetti all'array.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_array_oggetti_2.bmp](./assets/media/image23.png){width="5.350694444444445in"
height="3.623611111111111in"}

> I due pulsante "**Aggiungi proprietà**" (
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_proprieta.bmp](./assets/media/image19.png){width="0.7465277777777778in"
> height="0.2013888888888889in"} ) e "**Rimuovi proprietà**" (
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_rimuovi_proprieta.bmp](./assets/media/image24.png){width="0.7208333333333333in"
> height="0.2076388888888889in"} ) consentiranno invece di definire la
> struttura e mappare con i relativi Campi / Attributi Passweb le
> proprietà di ogni oggetto dell'Array

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_json_builder_array_oggetti.bmp](./assets/media/image25.png){width="5.350694444444445in"
height="3.623611111111111in"}

Per quel che riguarda invece **la tipologia di campo Passweb** **con cui
poter mappare le varie proprietà** è possibile selezionare una delle
seguenti opzioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json-ld_campi_passweb.bmp](./assets/media/image26.png){width="5.350694444444445in"
height="3.623611111111111in"}

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

