# ORDINI



Il tab "**Ordini**" visibile solo dopo aver configurato e salvato i
parametri presenti all'interno del tab "Configurazione", consente di
configurare e gestire la generazione del feed utilizzato per condividere
con Clerk informazioni relative agli ordini presenti all'interno del
proprio sito Ecommerce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_feed_ordini.bmp](./assets/media/image11.png)

In questo senso dunque il parametro:

**Data Import Ordini**: consente di visualizzare ed eventualmente
reimpostare la data di ultima generazione del feed. Tale campo verrà
quindi aggiornato in maniera automatica a seguito di ogni generazione
del feed (indipendentemente dal fatto che questo avvenga automaticamente
alla sincronizzazione o in maniera manuale cliccando sull'apposito
pulsante)

**ATTENZIONE!** all'interno del feed verranno inseriti solo ed
esclusivamente gli ordini con data successiva a quella indicata
all'interno di questo campo

**Considera articoli padre nel tracciamento**: se selezionato, nel
momento in cui dovessero essere presenti in ordine degli articoli figli
di struttura, verrà comunque inserito nel feed, e inviato anche via API,
il codice del relativo articolo padre (il prezzo cosniderato sarà invece
sempre quello dell'articolo figlio).

**ATTENZIONE!** questo flag dovrebbe essere attivato solo nel caso in
cui si sia deciso di impostare i moduli Clerk (Search e Reccomendations)
eventualmente implementati all'interno del sito per visualizzare, in
relazione ad articoli strutturati, i soli articoli padre (per maggiori
informazioni in merito si veda anche quanto indicato nel successivo
capitolo "*Tracciamento Sito*" di questo manuale)

**Genera Feed alla Sincronizzazione**: consente, se selezionato, di
generare automaticamente il feed ad ogni sincronizzazione sito --
gestionale (Standard o Totale).

**ATTENZIONE!** **se generato in maniera automatica** (dunque a seguito
di una sincronizzazione) all'interno del feed verranno inseriti
solamente gli Ordini:

- con data successiva a quella indicata in corrispondenza del campo
  "Data Import Ordini"

- che non sono stati già inviati a Clerk (via API) o che non sono già
  stati inseriti in un feed precedente

- che si trovano nello stato di Memorizzato, Sospeso o Evaso

**URL Feed**: consente di visualizzare l'url di pubblicazione del feed,
quello che dovrà poi essere inserito all'interno del campo "JSON Orders
URL" alla pagina "**Data -- Configuration**" dello store Clerk con cui
si desidera effettuare l'integrazione (per maggiori informazioni in
merito si veda anche quanto indicato all'interno del precedente capitolo
"*Sincronizzazione Dati*")

Il pulsante "**Genera Feed**" presente nella parte bassa della maschera
consente invece di avviare manualmente la generazione del relativo feed.

**ATTENZIONE!** **se generato in maniera manuale** all'interno del feed
verranno inseriti tutti gli Ordini:

- con data successiva a quella indicata in corrispondenza del campo
  "Data Import Ordini" indipendentemente dal fatto che siano o meno già
  stati inviati a Clerk (via API) o che siano o meno già stati inseriti
  in un feed precedente

- che si trovano nello stato di Memorizzato, Sospeso o Evaso

In sostanza dunque, una volta che un ordine è stato inserito in un feed,
potrà essere inserito anche in un feed generato successivamente solo se
questo verrà creato in maniera manuale

Ora, riguardo la generazione del feed Ordini e, in generale, riguardo le
modalità con cui Passweb può inviare a Clerk informazioni relativamente
agli ordini effettuati all'interno del sito, è bene fare alcune
considerazioni di fondamentale importanza in maniera tale da avere ben
chiaro il flusso da seguire per condividere con Clerk questo tipo di
informazioni.

Innanzitutto va detto che, come evidenziato anche nel precedente
capitolo di questo manuale, Passweb può condividere con Clerk
informazioni relative agli ordini effettuati all'interno del sito in due
modi diversi:

- Mediante la creazione del feed Ordini (che Clerk andrà poi a leggersi
  ad intervalli di tempo regolari)

- Mediante apposite chiamante API che, al verificarsi di determinati
  eventi, inseriranno direttamente i dati degli ordini nel database di
  Clerk

Per ogni ordine inserito nel feed verranno prese in considerazione le
seguenti informazioni:

- id Passweb dell'Ordine

- elenco dei prodotti in ordine indicando per ciascuno di essi:

  - id Passweb dell'articolo -- nel caso di articoli figli di struttura
    sarà inserito l'id dell'articolo figlio o quello dell'articolo padre
    a seconda dell'impostazione settata per il parametro "**Considera
    articoli padre nel tracciamento**"

  - quantità in ordine

  - prezzo ivato

- data dell'ordine

- id Passweb del cliente intestatario del documento

- email del cliente intestatario del documento

- stato impostato a:

  - "Confirmed" per ordini in stato Memorizzato

  - "Cancelled" per ordini in stato Sospeso

  - "Delivered" per ordini in stato Evaso

Per ogni ordine inviato via API verranno prese in considerazione le
stesse informazioni ad eccezione dello stato. Inoltre per gli ordini
inviati via API verrà preso in considerazione anche "vistor id" ossia un
identificativo del dispositivo da cui è stato effettuato l'ordine (per
maggiori informazioni in merito si veda anche quanto indicato nel
successivo capitolo "*Privacy e GDPR*" di questo manuale)

**ATTENZIONE!** i totali dell'ordine presenti su Clerk verranno
calcolati da Clerk stesso sulla base dei prezzi e della quantità dei
singoli articoli presenti nel documento (e non saranno comprensivi
ovviamente di eventuali costi di spedizione o spese accessorie presenti
nel piede del documento gestionale)

A seconda della modalità utilizzata (feed o API) cambieranno invece i
dati relativi alla sorgente (colonna "Source") e all'impatto (colonna
"Clerk.io impact") registrati da Clerk in corrispondenza di questi
stessi ordini.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_feed_ordini_2.bmp](./assets/media/image12.png)

Nello specifico:

- Gli ordini acquisti mediante import del feed verranno registrati su
  Clerk con sorgente "**Synced**" e avranno impatto nullo

- Gli ordini inviati mediante chiamate API verranno invece registrati su
  Clerk con sorgente "**Tracked**" e potranno avere un impatto nullo o
  diverso da 0 a seconda del fatto che gli articoli in ordine siano
  stati "trovati" o meno dai moduli Clerk (Ricerca, Raccomandazioni,
  Chat ...) implementati all'interno del sito.

Inoltre gli ordini "**Synced**" potranno eventualmente essere
sovrascritti e aggiornati a seguito di una nuova importazione del
relativo feed. Gli ordini "**Tracked**" invece, una volta registrati,
non potranno poi più essere modificati.

**In sostanza dunque l'importazione ordini mediante feed dovrebbe essere
effettuata in fase iniziale per il primo popolamento del database di
Clerk con tutti gli ordini presenti all'interno del sito ecommerce e,
successivamente, come backup per eventuali ordini che per qualche
ragione non sono stati inviati via API.**

Una volta attivata l'integrazione con Clerk i nuovi ordini dovrebbero
invece essere inviati via API in modo tale da poter registrare anche
l'impatto prodotto su di essi dai moduli Clerk.

Altra cosa importante da mettere in evidenza, vista la gestione degli
stati dell'ordine di Passweb, è che ovviamente non avrebbe alcun senso
inviare a Clerk, ad esempio, ordini in stato di "Pagamento non
confermato" per cui **sia in fase di generazione feed che in fase di
invio dati via API verranno presi in considerazione sempre e soltanto
Ordini in stato Memorizzato, Sospeso ed Evaso**

**ATTENZIONE!** Ordini in uno stato diverso dai tre sopra indicati, così
come Bolle e Fatture non verranno mai inseriti nel feed Ordini e non
verranno mai inviati a Clerk neppure via API

In considerazione di quanto detto fino ad ora lo scambio dati tra
Passweb e Clerk relativamente agli ordini presenti sul sito dovrà
avvenire come di seguito indicato:

- In fase iniziale per popolare il database di Clerk con gli ordini
  presenti all'interno del sito sarà necessario individuare ed inserire
  all'interno del campo "**Data Import Ordini"** una data di partenza
  per la generazione del feed.

> Dipendentemente dal numero di ordini presenti all'interno del proprio
> sito, le dimensioni di questo primo feed potrebbero essere piuttosto
> grandi e questo potrebbe ovviamente impattare sul tempo impiegato da
> Clerk per importare e analizzare poi i relativi dati. In questo senso
> il consiglio è quello di non inserire mai all'interno del feed ordini
> più vecchi di uno o due anni.

- Una volta impostata la data di partenza sarà necessario procedere ad
  una prima generazione manuale del feed all'interno del quale verranno
  quindi inseriti tutti gli ordini attualmente presenti sul sito con
  data successiva a quella indicata e in stato Memorizzato, Sospeso o
  Evaso.

> Considerando che questi ordini sono stati fatti prima
> dell'integrazione con Clerk è corretto che vengano inseriti nel feed e
> che vengano quindi registrati su Clerk con sorgente "Synced" e impatto
> nullo

- Terminata la generazione del feed la data presente all'interno del
  campo "Data Import Ordini" verrà automaticamente aggiornata alla data
  attuale e gli ordini presenti all'interno del feed verranno marcati
  come già inviati a Clerk e non verranno quindi più inseriti nei feed
  generati automaticamente a seguito di una sincronizzazione.

- A questo punto, posto ovviamente di aver impostato in maniera corretta
  tutta l'integrazione Passweb -- Clerk, sarà possibile attivare il flag
  "**Genera Feed alla sincronizzazione**" e lasciare che sia quindi
  Passweb a generare di volta in volta il feed Ordini che, se tutto
  funziona correttamente dovrebbe risultare sempre vuoto o quanto meno
  contenere solo quei pochi ordini che per qualche ragione non sono
  stati inviati via API

- Una volta attivata l'integrazione infatti i nuovi ordini effettuati
  all'interno del sito verranno inviati a Clerk via API in maniera tale
  da poterne registrare anche l'impatto.

> Nello specifico la chiamata API per l'invio del nuovo ordine verrà
> effettuata a seguito di una sincronizzazione parziale in maniera tale
> da essere certi di inviare a Clerk solo ordini in stato Memorizzato e
> di evitare, invece, l'invio di quelli in stato di "Pagamento non
> confermato" per i quali non si sa ancora se dovranno o meno essere
> inseriti a gestionale.
>
> Se la chiamata API va a buon fine l'ordine verrà registrato su Clerk,
> verrà marcato come già inviato a Clerk, e non verrà quindi più
> inserito nel feed ordini generato automaticamente alla prossima
> sincronizzazione standard
>
> Se per qualche ragione invece la chiamata API non dovesse andare a
> buon fine, l'ordine resterebbe marcato come "non inviato a Clerk" e
> verrebbe quindi eventualmente rivalutato per un invio via API durante
> la prossima sincronizzazione parziale scatenata ad esempio da un
> eventuale nuovo ordine effettuato sul sito prima dell'avvio della
> sincronizzazione standard.
>
> Se poi anche nelle successive sincronizzazioni parziali le chiamate
> API dovessero continuare ad avere dei problemi, gli ordini resteranno
> marcati come "non inviati a Clerk", verranno quindi inseriti nel feed
> generato automaticamente alla prima sincronizzazione standard utile e
> verranno importati su Clerk con sorgente "Synced" (in questo caso si
> perderà quindi l'impatto prodotto per essi da Clerk).

- Infine se fosse necessario, per una qualsiasi ragione, riallineare le
  due basi dati, per importare ordini presenti in Passweb ma non in
  Clerk sarà sufficiente effettuare una nuova generazione manuale del
  feed ordini con una data di partenza precedente a quella degli ordini
  non presenti su Clerk.

**ATTENZIONE!** considerando che i nuovi ordini verranno inviati a Clerk
via API non sarà necessario inserire nella pagina di conferma ordine lo
snippet di codice indicato nella documentazione Clerk per il
tracciamento lato client di questi stessi ordini (tracciamento questo
che tra l'altro prenderebbe in considerazione per forza di cose anche
ordini in stato di "Pagamento non confermato")

Infine un'ultima considerazione da fare è quella che riguarda la
creazione del feed ordini nel caso di siti in multilingua. In queste
condizioni infatti il consiglio è quello di creare su Clerk uno store
per ciascuna lingua gestita sul sito e su Passweb, ovviamente, un
Account Clerk per ciascuno Store marcando anche uno di questi account
come account di default

Il feed ordini verrà poi generato tenendo in considerazione la Nazione
selezionata dall'utente stesso in fase di registrazione al sito (o
quella eventualmente associata nella sua anagrafica gestionale nel caso
in cui l'utente dovesse essere stato importato direttamente da Mexal).
Dalla Nazione verrà poi ricavata la lingua e in base alla lingua
l'ordine verrà inserito in uno store piuttosto che in un altro

Supponendo dunque:

- di avere il sito in tre lingue, italiano francese e inglese

- di gestire all'interno del sito 4 distinti paesi Italia, Francia,
  Inghilterra e Spagna

- di aver creato tre store distinti all'interno di Clerk

- di aver configurato su Passweb 3 Account Clerk con le corrette
  impostazioni di lingua e valuta

- di aver impostato l'account in lingua italiana come account di default

In queste condizioni gli ordini verranno divisi nei feed dei vari
account Clerk presenti su Passweb come di seguito indicato:

- Gli ordini essere effettuati da un utente che risulta associato, nella
  sua anagrafica al paese Italia verranno inseriti nel feed dell'Account
  Clerk per cui è stata impostata la lingua italiana

- Gli ordini essere effettuati da un utente che risulta associato, nella
  sua anagrafica al paese Francia verranno inseriti nel feed
  dell'Account Clerk per cui è stata impostata la lingua francese

- Gli ordini essere effettuati da un utente che risulta associato, nella
  sua anagrafica al paese Inghilterra o ad esempio al paese Stati Uniti
  d'America, verranno inseriti nel feed dell'Account Clerk per cui è
  stata impostata la lingua inglese

- Gli ordini essere effettuati da un utente che risulta associato, nella
  sua anagrafica al paese Spagna verranno inseriti nel feed dell'Account
  Clerk per cui è stata impostata la lingua italiana (che è quello di
  default)

Per maggiori informazioni relativamente all'integrazione Passweb --
Clerk nel caso di siti multilingua si veda anche quanto indicato nel
relativo capitolo ("*Passweb e Clerk -- Integrazione -- Multilingua*")
di questo manuale

