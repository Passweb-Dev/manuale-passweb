# ANONIMIZZAZIONE DEI DATI



Prima di prendere in considerazione il discorso relativo
all'anonimizzazione è bene fare innanzitutto una premessa su quelli che
sono i dati che possono effettivamente essere raccolti utilizzando
Matomo.

In questo senso, come indicato anche nella documentazione ufficiale
(<https://matomo.org/faq/general/faq_18254/>), utilizzando il tracker
javascript di Matomo verranno raccolte, a default, le seguenti
informazioni:

- Indirizzo IP dell'utente (anonimizzato o meno in base alle
  impostazioni settate)

- User ID (opzionale)

- Titolo della pagina visualizzata

- URL della pagina visualizzata

- Risoluzione dello schermo

- Ora nel fuso orario dell'utente locale

- File cliccati e scaricati

- Collegamenti a un dominio esterno su cui è stato fatto click (Outlink)

- Tempo di generazione delle pagine

- Posizione dell'utente: paese, regione, città, latitudine e longitudine
  approssimative ( in base alle impostazioni di Geolocalizzazione
  settate)

- Lingua principale del browser utilizzato

- User Agent del browser utilizzato

In aggiunta a quanto sopra indicato, nei cookie di prima parte
installati da Matomo, verranno memorizzati anche i seguenti dati:

- ID visitatore, univoco casuale

- Ora della prima visita dell'utente

- Ora della visita precedente dell'utente

- Numero di visite dell'utente

Infine altri dati (questa volta opzionali) che potrebbero essere
raccolti utilizzando Matomo potrebbero essere:

- Dimensioni e variabili personalizzate

- Campagne

- Dati di ricerche effettuate all'interno del sito

- Dati Ecommerce

- Interazioni sui form

- Interazioni sui video

- ...

Ora dipendentemente dalla tipologia di dati raccolti, o meglio,
dipendentemente dal fatto di voler acquisire o meno informazioni di
identificazione personale, oltre che ovviamente dal fatto implementare o
meno un tracciamento che faccia effettivamente uso dei cookie, potremmo
anche trovarci in una situazione in cui l'utilizzo di Matomo potrebbe
non essere sottoposto al GDPR e potrebbe quindi avvenire anche senza la
necessità di richiedere esplicito consenso agli utenti.

Come vedremo meglio nel relativo capitolo di questo manuale (*"Matomo --
Privacy e GDPR -- Tracciamento senza richiesta di consenso"*) una
condizione imprescindibile affinché possa effettivamente configurarsi
una situazione di questo tipo è quella di non raccogliere assolutamente
nessuna informazione di identificazione personale.

**Nel momento in cui dovesse essere raccolta anche una sola informazione
di carattere personale sarà necessario richiedere preventivamente il
consenso agli utenti accertandosi di non tracciare nessun dato nel caso
in cui l'utente dovesse negare tale consenso**

**ATTENZIONE!** Per maggiori informazioni in merito a quelli che possono
o meno essere considerati effettivamente dati di identificazione
personale si consiglia di chiedere sempre un parere al proprio team
legale o perlomeno di fare riferimento a quanto indicato in proposito
dal Garante.

A questo indirizzo <https://matomo.org/faq/general/faq_18254/> è
possibile trovare alcune indicazioni relativamente a quelli che possono
essere considerati dati di identificazione personale (PII).

Ora, se per i dati opzionali come possono essere lo User Id, le Custom
Dimension, le HBeatmaps, le registrazioni di sessioni di navigazione ...
non ci sono grossi problemi nel senso che per non raccogliere questo
tipo di dati è sufficiente non attivare le relative funzionalità, per
quei dati considerati come informazioni di identificazione personale che
vengono raccolti a default da Matomo il discorso invece è leggermente
diverso.

In questo caso infatti non è possibile evitare di raccogliere il dato
ma, a differenza di quanto avviene con Google Analytics, Matomo mette a
disposizione degli utenti tutta una serie di funzionalità attraverso cui
poter anonimizzare questi stessi dati in maniera tale da non poterli più
utilizzare per risalire all'identità dei singoli utenti

Per attivare e gestire l'anonimizzazione di questi dati è sufficiente
agire dalla sezione "**Rendi anonimi i dati**" presente all'interno del
menu "**Privacy**" nella pagina di **Amministrazione** della propria
installazione Matomo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_10.bmp](./assets/media/image10.png)

I parametri presenti all'interno del box "**Rendi anonimi i Dati di
Tracciamento**" consentono rispettivamente di:

- **Rendi anonimi gli IP dei visitatori**: consente, se selezionato, di
  attivare l'anonimizzazione degli indirizzi IP.

> E' possibile decidere quanti bytes degli indirizzi IP dovranno essere
> nascosti (ad esempio 2 bytes, l'impostazione consigliata,
> trasformerebbe l'indirizzo IP 192.168.100.1 in 192.168.xxx.xxx)
>
> Volendo è anche possibile rafforzare la privacy degli utenti decidendo
> di estendere l'anonimizzazione degli indirizzi IP anche ad eventuali
> plugin che ne dovessero fare uso (parametro "Usa gli indirizzi IP
> anonimi quando si arricchiscono le visite" impostato su SI).
>
> Ovviamente, in queste condizioni si garantisce una maggior privacy
> agli utenti ma, di contro, si avrà una minor accuratezza, ad esempio,
> nella geolocalizzazione degli utenti.

- **Sostituisci l'ID Utente con uno pseudonimo:** consente se
  selezionato di sostituire l'id utente con uno pseudonimo generato
  utilizzando una funzione di hash criptata

> **ATTENZIONE!** come indicato nella descrizione di questo parametro la
> sostituzione con uno pseudonimo non è la stessa cosa dell'anonimato.
> In termini GDPR: lo pseudonimo di un ID Utente conta ancora come un
> dato personale.

- **Rendi anonimo l'ID dell'Ordine:** consente, se selezionato, di
  anonimizzare gli id degli ordini effettuati all'interno del sito e
  registrati da Matomo (siti ecommerce).

- **Forza il tracciamento senza i cookies:** consente di attivare la
  modalità di tracciamento cookieless (senza utilizzo dei cookie)

- **Rendi anonimo il referrer:** offre diverse opzioni per poter
  anonimizzare in maniera più o meno forte l' url referrer ossia l' url
  a partire dal quale l'utente è atterrato sul nostro sito

Nell'ottica di voler anonimizzare completamente tutti i possibili dati
di identificazione personale potrebbe quindi essere necessario:

- Anonimizzare gli indirizzi IP mascherando almeno 2 o 3 bytes di tali
  indirizzi

- Estendere l'utilizzo di IP anonimi anche ad altri plugin (es. plugin
  di geolocalizzazione)

- Mascherare ID Utente e ID Ordine

- Abilitare il tracciamento cookieless

- Anonimizzare l'url referrer mantenendo il solo dominio del sito
  (opzione "Mantieni solo il dominio dell'URL di un referrer")

In tutto ciò ovviamente, occorre considerare anche il lato negativo
della medaglia.

Se da una parte, infatti, l'anonimizzazione dei dati potrebbe portare
anche, assieme al verificarsi di altre condizioni, a poter implementare
un sistema di tracciamento senza la necessità di richiedere il consenso
agli utenti rimanendo comunque conformi al GDPR, dall'altra parte va
anche considerato che questa anonimizzazione porterà sicuramente ad
avere una minor accuratezza dei dati raccolti, in termini ad esempio di
tracciamento degli utenti cross device, di geolocalizzazione, di profilo
degli utenti con le varie operazioni da essi effettuate ...

In sostanza dunque starà a chi utilizza Matomo decidere se configurarlo
in maniera tale da poter effettivamente implementare il tracciamento
senza alcun tipo di richiesta e senza quindi correre il rischio di
perdere tutti i dati degli utenti che dovessero poi negare il proprio
consenso, pagando però il prezzo di avere dei dati globali meno accurati
e precisi, oppure se decidere di raccogliere anche informazioni di
carattere personale implementando quindi tutte le richieste di consenso
previste dal GDPR, correndo il rischio di avere alla fine meno dati su
cui ragionare ma sicuramente più precisi e accurati.

