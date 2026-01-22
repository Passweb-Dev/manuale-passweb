# CARRELLI ABBANDONATI



All'interno di questa sezione è possibile visualizzare informazioni
dettagliate relativamente a quelli che sono stati, in relazione alla
Variante e all'intervallo di tempo considerato, i Carrelli Abbandonati.

![](./assets/media/image11.png)

**ATTENZIONE! Per Carrelli Abbandonati si intendono quelle sessioni
durante le quali un determinato utente è arrivato ad inserire uno o più
articoli in carrello senza poi concludere effettivamente l'ordine**

In particolare nel momento in cui un utente dovesse aggiungere un primo
articolo in Carrello questo verrà immediatamente considerato come
"**Carrello Attivo**" e verrà quindi visualizzato e conteggiato tra
quelli presenti nel relativo report presente all'interno della sezione
"**Statistiche -- Ecommerce -- Carrelli Attivi**" del Wizard oltre che
nei relativi indicatori della Dashboard

Tale carrello rimarrà come Attivo almeno per i prossimi 30 minuti.

Trascorsi poi **30 minuti di inattività**, dove inattività significa che
non sono state apportate modifiche alle quantità o al numero di articoli
in carrello e che, ovviamente, il carrello stesso non è stato
finalizzato in ordine, allora il Carrello in esame passerà da Attivo ad
**Abbandonato** e verrà quindi visualizzato e conteggiato tra quelli
presenti all'interno di questa sezione del Wizard

Il grafico presente nella parte alta della pagina mostra l'andamento nel
tempo del numero di carrelli abbandonati registrati dal sito.

La tabella presente nella parte bassa

![](./assets/media/image12.png)

consente invece di ottenere informazioni più dettagliate su ogni singolo
carrello abbandonato.

Nello specifico infatti, per ogni singolo elemento presente in griglia
verranno visualizzate le seguenti informazioni:

- **Id:** codice identificativo del relativo carrello all'interno del
  database di Passweb

- **Utente:** Nome e Cognome / Ragione Sociale dell'utente (**se
  autenticato**) che ha generato il relativo carrello abbandonato

- **Email:** indirizzo Email dell'utente (**se autenticato**) che ha
  generato il relativo carrello abbandonato

- **Numero:** numero degli articoli presenti all'interno del relativo
  carrello abbandonato

- **Quantità:** somma delle quantità di tutti gli articoli presenti
  all'interno del relativo carrello abbandonato

- **Coupon:** codice dell'eventuale Buono Sconto utilizzato nel relativo
  carrello abbandonato

- **Subtotale:** importo totale del relativo carrello abbandonato.

> **ATTENZIONE!** Da questi importi sono escluse eventuali spese
> accessorie (es. spese di spedizione, spese sui pagamenti ecc...)
> generate dai relativi preventivi eventualmente effettuati dall'utente
> all'interno della stessa pagina carrello.

- **Data:** data di creazione del relativo carrello abbandonato

Cliccando su uno qualsiasi degli elementi presenti in griglia sarà poi
possibile visualizzare, ed eventualmente stampare (pulsante "Stampa") il
dettaglio del relativo carrello abbandonato.

![](./assets/media/image13.png)

**ATTENZIONE!** Nel dettaglio dei carrelli abbandonati non verranno
indicati i dati relativi ad eventuali spese accessorie (es. spese di
spedizione, spese sui pagamenti ecc...) generate dai relativi preventivi
eventualmente effettuati dall'utente all'interno della stessa pagina
carrello

Il pannello di ricerca presente nella parte alta della pagina consente
inoltre di filtrare i carrelli abbandonati presenti in elenco sulla base
del loro codice identificativo (campo "**Id**"), del fatto che il
carrello sia stato generato da un utente autenticato o meno (parametro
**"Solo Visitatori Autenticati"**) oppure sulla base del Nome / Ragione
Sociale / Email dello specifico utente che lo ha generato (campo
"**Nome/Ragione Sociale/Email**")

Il pulsante "**Esporta**" consente invece di esportare all'interno di un
apposito file .csv, relativamente ai dati attualmente presenti in
griglia (e quindi eventualmente filtrati rispetto al totale dei dati
stessi) diversi tipi di informazioni:

![](./assets/media/image14.png)

- **Elenco Carrelli**: viene generato ed esportato un csv in cui ogni
  singolo record è relativo ad uno specifico carrello abbandonato. Per
  ogni carrello abbandonato sono esportate le seguenti informazioni:

  - **ID** = codice identificativo del relativo carrello all'interno del
    database di Passweb

  - **Indirizzo IP** = Indirizzo IP della macchina client dell'utente
    che ha generato il relativo carrello abbandonato

  - **Codice Utente** = codice conto nell\'anagrafica utenti o codice
    contatto dell'utente cha ha generato il relativo carrello
    abbandonato

  - **Nome/Ragione Sociale** = nome e cognome o ragione sociale
    dell\'utente che ha generato il relativo carrello abbandonato

  - **Email** = indirizzo email dell\'utente che ha generato il relativo
    carrello abbandonato

  - **N. Articoli** = numero degli articoli presenti nel relativo
    carrello abbandonato

  - **Qta Articoli** = somma delle quantità degli articoli presenti nel
    relativo carrello abbandonato

  - **Coupon** = codice dell'eventuale Buono Sconto utilizzato nel
    relativo carrello abbandonato

  - **Sub Totale** = importo totale del relativo carrello abbandonato

> **ATTENZIONE!** Da questi importi sono escluse eventuali spese
> accessorie (es. spese di spedizione, spese sui pagamenti ecc...)
> generate dai relativi preventivi eventualmente effettuati dall'utente
> all'interno della stessa pagina carrello.

- **Valuta** = valuta gestita nel relativo carrello abbandonato

- **Data** = data di creazione del relativo carrello abbandonato

<!-- -->

- **Elenco Righe**: viene generato un csv in cui ogni singolo record
  rappresenta una delle righe articolo presente all'interno dei carrelli
  abbandonati.

> **ATTENZIONE! Nel momento in cui uno stesso articolo fosse presente in
> due carrelli abbandonati diversi, nel csv di esportazione verranno
> inserite due righe distinte.**
>
> Per ogni articolo sono esportate le seguenti informazioni:

- **ID Carrello** = codice identificativo del carrello, all'interno del
  database di Passweb, cui appartiene il relativo articolo

- **Codice** = codice dell'articolo articolo presente nel corrispondente
  carrello abbandonato

- **Qta** = quantità articolo presente nel corrispondente carrello
  abbandonato

- **Importo** = totale della riga articolo presente nel corrispondente
  carrello abbandonato

- **Valuta** = valuta in uso all'interno del corrispondente carrello
  abbandonato

- **Codice Utente** = codice conto nell\'anagrafica utenti o codice
  contatto dell'utente che ha generato il carrello abbandonato cui
  appartiene il relativo articolo

- **Nome/Ragione Sociale** = nome e cognome o ragione sociale
  dell\'utente che ha generato il carrello abbandonato cui appartiene il
  relativo articolo

- **Email** = indirizzo email dell\'utente che ha generato il carrello
  abbandonato cui appartiene il relativo articolo

- **Data** = data di creazione della riga del relativo carrello
  abbandonato

<!-- -->

- **Elenco Articoli e Quantità**: viene generato un csv in cui ogni
  singolo record rappresenta un articolo presente all'interno di uno
  qualsiasi dei carrelli abbandonati (informazioni raggruppate per
  articolo).

> **ATTENZIONE! Nel momento in cui uno stesso articolo fosse presente in
> due carrelli abbandonati diversi, nel csv di esportazione verrà
> inserita un\'unica riga. I dati presenti all'interno del file saranno
> quindi raggruppati per codice articolo**
>
> Per ciascuno dei record presenti all'interno del file saranno presenti
> le seguenti informazioni:

- **Codice** = codice dell'articolo che compare in almeno uno dei
  carrelli abbandonati

- **Referenze** = numero delle righe dei carrelli abbandonati in cui è
  presente il relativo articolo

- **Qta** = somma delle quantità di tutte le righe dei carrelli
  abbandonati in cui è presente il relativo articolo

<!-- -->

- **Elenco Articoli e Utenti**: viene generato un csv analogo al
  precedente in cui però le informazioni non sono raggruppate solamente
  per articolo ma anche per utente.

> **ATTENZIONE! In queste condizioni dunque nel momento in cui uno
> stesso articolo fosse presente in due carrelli abbandonati diversi,
> entrambi generati dallo stesso utente nel csv di esportazione verrà
> inserita un\'unica riga.**
>
> **Nel caso in cui invece uno stesso articolo fosse presente in due
> carrelli abbandonati diversi generati anche da utenti diversi nel csv
> di esportazione verranno inseriti due record distinti**
>
> Per ciascuno dei record presenti all'interno del file saranno presenti
> le seguenti informazioni:

- **Codice** = codice dell'articolo che compare in almeno uno dei
  carrelli abbandonati di un dato utente

- **Referenze** = numero delle righe dei carrelli abbandonati da un
  determinato utente in cui è presente il relativo articolo

- **Qta** = somma delle quantità di tutte le righe dei carrelli
  abbandonati da un determinato utente in cui è presente il relativo
  articolo

- **Codice Utente** = codice conto nell\'anagrafica utenti o codice
  contatto dell'utente che ha generato il carrello abbandonato cui
  appartiene il relativo articolo

- **Nome/Ragione Sociale** = nome e cognome o ragione sociale
  dell\'utente che ha generato il carrello abbandonato cui appartiene il
  relativo articolo

- **Email** = indirizzo email dell\'utente che ha generato il carrello
  abbandonato cui appartiene il relativo articolo

<!-- -->

- **File Import Carrello:** consente di esportare gli articoli dei
  carrelli abbandonati attualmente presenti in elenco all'interno di un
  file .csv il cui formato è esattamente quello richiesto dalla
  procedura di "**Import articoli in Carrello tramite File**" (per
  maggiori informazioni in merito a questa procedura si veda anche la
  sezione "*Varianti Sito Responsive -- Lista Componenti Ecommerce --
  Componente Carrello Custom -- Aggiunta Articoli in Carrello tramite
  File*" di questo manuale).

> Il file così esportato avrà come intestazione i campi "**codice**",
> "**quantità**" e "**taglia**" (non vengono quindi considerati ed
> esportati dati relativi a prezzi e/o sconti).
>
> **ATTENZIONE!** Nel file verranno inseriti i dati delle righe articolo
> presenti in tutti i carrelli abbandonati attualmente presenti in
> elenco ad eccezione di:

- **articoli spesa**

- **articoli padri di struttura (configurati in relazione ad articoli
  figli non presenti sul sito)**

- **articoli presenti nel carrello abbandonato a seguito
  dell'applicazione di eventuali promozioni**

- **box configurabili**

- **articoli componenti di un campionario (box) non configurabile. In
  questo caso verrà aggiunto, ovviamente, il solo articolo
  campionario(box)**

**ATTENZIONE!** tutti i dati presenti all'interno di questa sezione del
Wizard sono relativi solo ed esclusivamente ai carrelli abbandonati a
partire dalla data in cui tale funzionalità risulta essere
effettivamente disponibile

