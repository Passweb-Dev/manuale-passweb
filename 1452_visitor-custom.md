# VISITOR: CUSTOM



Questa impostazione è quella che consente di tracciare i visitatori del
sito e le relative sessioni utilizzando degli ID personalizzati (quindi
non generati direttamente da Clerk) su cui poter avere il pieno
controllo.

Dipendentemente da come verranno generati ed utilizzati questi
identificativi potrà cambiare il funzionamento dell'applicativo in
relazione all'integrazione con Clerk e, ovviamente, anche quello che
dovrà essere poi gestito a livello di GDPR.

In questo senso l'integrazione Passweb -- Clerk utilizza la modalità
*Custom* combinata con la modalità *visitor: null* per garantire che
tutti i moduli Clerk eventualmente implementati all'interno del sito,
possano continuare a funzionare (ovviamente in maniera limitata) anche
nel caso in cui l'utente dovesse decidere di non prestare i relativi
consensi restando comunque pienamente conformi a quanto richiesto dal
GDPR.

Nel momento in cui l'utente dovesse invece prestare tutti i consensi del
caso, l'impostazione *Custom* e gli id visitatore generati direttamente
da Passweb consentiranno di ottenere risultati più precisi rispetto, ad
esempio, a quelli ottenibili con l'impostazione *visitor: 'persistent'*
anche in considerazione del fatto che questi stessi id saranno
effettivamente unici per dispositivo, superando quindi i problemi,
precedentemente evidenziati, relativamente alla condivisione dello
stesso id da parte di utenti che dovessero trovarsi a navigare sullo
stesso sito, dalla stessa rete, con dispositivi dello stesso tipo e con
lo stesso browser.

Detto ciò per poter attivare questa impostazione sarà necessario, dal
punto di vista tecnico, inserire all'interno dello script di
configurazione di Clerk il segnaposto "**Tipo di visitatore**" (
**{clerk_visitor_type} )** evitando di indicare in maniera specifica
altre opzioni per il parametro visitor.

Lo script di configurazione di Clerk dovrà quindi essere di questo tipo:

*\<!\-- Start of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

*\<script type=\"text/javascript\"\>*

*(function(w,d){*

*var
e=d.createElement(\'script\');e.type=\'text/javascript\';e.async=true;*

*e.src=\'https://cdn.clerk.io/clerk.js\';*

*var
s=d.getElementsByTagName(\'script\')\[0\];s.parentNode.insertBefore(e,s);*

*w.\_\_clerk_q=w.\_\_clerk_q\|\|\[\];w.Clerk=w.Clerk\|\|function(){w.\_\_clerk_q.push(arguments)};*

*})(window,document);*

*Clerk(\'config\', {*

*key:* *\'{clerk_public_key}\',*

*collect_email: true,*

***{clerk_visitor_type}***

*});*

*\</script\>*

*\<!\-- End of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

In queste condizioni l'applicativo si comporterà come di seguito
indicato:

- Al primo accesso al sito da parte di un nuovo visitatore, lo script di
  configurazione di Clerk verrà eseguito sostituendo il segnaposto
  *{clerk_visitor_type}* con l'impostazione ***visitor: null*** mettendo
  quindi l'applicativo nelle condizioni di non generare automaticamente
  nessun id di sessione e di non inviare quindi a Clerk nessun dato di
  questo tipo.

> Contestualmente, la presenza del segnaposto *{clerk_visitor_type}*
> nello script di configurazione, provocherà anche la creazione da parte
> di Passweb di un cookie di prima parte denominato '**PWB-CI'**
> contenente una stringa identificativa del dispositivo di navigazione
> utilizzato dall'utente (in sostanza dunque un client-id).
>
> Tale stringa:

- verrà generata in maniera assolutamente casuale

- non sarà in alcun modo riconducibile ad altri dati personali
  dell'utente

- non verrà utilizzata per una profilazione dettagliata o per un
  tracciamento cross site

- verrà rigenerata regolarmente ogni 30 giorni

> In sostanza dunque il cookie PWB-CI potrebbe tranquillamente essere
> considerato come un cookie tecnico utilizzabile per distinguere
> sessioni di navigazione anonime e contenente un dato (client-id)
> pseudonimizzato.
>
> Sulla base di quanto detto può essere effettivamente corretto, in
> queste condizioni, eseguire lo script di configurazione di Clerk senza
> doverlo necessariamente sottoporre all'accettazione preventiva dei
> cookie (impostazione *visitor: null*) e allo stesso modo può anche
> essere considerato corretto installare, senza consenso preventivo, il
> cookie PWB-CI (cookie tecnico contenente un dato pseudonimizzato).
>
> In ogni caso, come per il *visitor: 'auto'* sarà comunque necessario:

- informare l'utente tramite Privacy Policy relativamente al fatto che
  il sito sta trattando dei dati pesudonimi (es. "utilizziamo un cookie
  tecnico per distinguere sessioni anonime per un massimo di 30 giorni")

- avere una base legale adeguata (preferibilmente Legittimo Interesse)

<!-- -->

- Nel momento in cui l'utente dovesse poi decidere di non accettare i
  cookie analitici, oppure nel caso in cui all'interno del sito non
  dovesse essere utilizzata nessuna delle CMP (es. Iubenda) integrate
  con Passweb per la gestione del consenso preventivo, tutto continuerà
  a funzionare esattamente come per il primo accesso.

> Lo script di configurazione di Clerk continuerà quindi ad essere
> eseguito in modalità *visitor: null* e, in conseguenza di ciò
> eventuali moduli Clerk implementati all'interno del sito (es. Ricerca,
> Raccomandazioni ...) continueranno a funzionare in modalità "limitata"
> secondo quanto descritto nel precedente capitolo di questo manuale

- Nel caso in cui l'utente dovesse invece prestare il consenso per
  l'utilizzo dei cookie analitici il comportamento dell'applicativo sarà
  completamente differente. In questo caso infatti:

  - verrà installato nel browser dell'utente un nuovo cookie denominato
    '**clerk-visitor-id'** (come nel caso di *visitor: 'persistent'*)
    della durata di 60 giorni in cui verrà memorizzato un visitor id di
    16 caratteri costruito da Passweb sulla base dell'indirizzo IP
    dell'utente che sta navigando il sito, dello user agent del browser
    utilizzato, della data e del client-id presente all'interno del
    cookie PWB-CI

  - lo script di configurazione di Clerk non verrà più eseguito in
    modalità *visitor: null* ma bensì con l'opzione

> ***visitor: 'xxxxx'***
>
> dove xxxxx sarà esattamente il visitor id presente all'interno del
> cookie 'clerk-visitor-id'

- le chiamate API generate da Raccomandazioni Clerk implementate
  all'interno del sito mediante il componente "Popolarità Prodotto"
  utilizzeranno come visitor id, quando necessario, il valore presente
  all'interno del cookie 'clerk-visitor-id'

Sulla base di quanto visto fino ad ora dovrebbero essere abbastanza
chiare le principali differenze e i principali vantaggi che si possono
avere adottando questo tipo di gestione rispetto a quanto avviene, ad
esempio, con l'impostazione *visitor: 'presistent',* vale a dire:

- il fatto di non dover sottoporre lo script di configurazione di Clerk
  al consenso preventivo (grazie all'impostazione iniziale *visitor:
  null*) garantisce, a differenza di quanto avveniva nel caso di
  *visitor: 'persistent'*, che i moduli Clerk eventualmente presenti
  all'interno del sito (es. Ricerca) possano funzionare (in modalità
  "limitata") anche nel momento in cui l'utente non dovesse prestare
  alcun consenso

- il visitor id generato da Passweb, memorizzato all'interno del cookie
  'clerk-visitor-id' ed utilizzato in tutte le chiamate Clerk sia lato
  client che lato server (ovviamente solo nel caso in cui l'utente abbia
  prestato i relativi consensi) garantisce non solo che i prodotti
  visualizzati all'interno delle varie Raccomandazioni Clerk siano
  effettivamente coerenti con i dati di navigazione dell'utente (come
  avveniva anche nel caso di *visitor: 'persistent'*), ma anche che, per
  come viene generato, (ossia sulla base anche del client-id presente
  all'interno del cookie "PWB-CI" che abbiamo visto essere unico per
  dispositivo) che questo sia effettivamente unico per ogni dispositivo
  di navigazione e quindi che non si verifichino (come nel caso di
  *visitor: 'persistent'* o *visitor: 'auto'*) condivisioni di id tra
  utenti che navigano sullo stesso sito, dalla stessa rete con
  dispositivi dello stesso tipo e con lo stesso browser.

**ATTENZIONE! in ogni caso il consiglio è sempre quello di verificare
direttamente con il supporto Clerk o con il proprio DPO che la soluzione
adottata sia effettivamente conforme a quanto richiesto dal GDPR**

