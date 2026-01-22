# TRACCIAMENTO DATI



All'interno di questa sezione è possibile:

- Marcare / Smarcare l'ordine in esame come esportato su Google Ads
  nell'ambito della procedura di import delle conversioni offline

- Visualizzare alcuni dati utilizzati per il tracciamento dell'ordine in
  esame ed inviati quindi a sistemi quali Google Analytics, Google Ads o
  Facebook

![](./assets/media/image680.png)

Nello specifico dunque il parametro:

- **Esportato su Google Ads**: consente, se attivato, di marcare
  l'ordine in esame come già esportato su Google Ads evitando quindi di
  inserirlo nel file di esportazione che potrà poi essere prodotto
  automaticamente da Passweb nell'ambito della procedura di import delle
  conversioni offline (per maggiori informazioni in merito a questo tipo
  di procedura si veda quanto indicato all'interno del capitolo "*Google
  Ads User Provided Data e Conversioni Avanzate -- Import delle
  conversioni offline*" di questo manuale)

> **ATTENZIONE!** la stessa operazione può essere fatta anche in maniera
> massiva su più ordini contemporaneamente operando direttamente dalla
> maschera "**Lista Ordini**" mediante i pulsanti "**Esportato su Ads**
> / **Non Esportato su Ads**"

- **AdPersonalization / AdStorage / AnalyticsStorage /
  FunctionalityStorage / SecurityStorage / PersonalizationStorage --**
  dato in sola visualizzazione**:**

> Consente di visualizzare lo stato del relativo consenso (Granted o
> Denied) prestato dall'utente nel momento in cui è stato effettuato il
> relativo ordine (**richiede ovviamente l'attivazione e la gestione
> della Consent Mode**).
>
> **ATTENZIONE!** nel momento in cui non dovesse essere implementato
> l'utilizzo della consent mode i suddetti consensi verranno impostati a
> default su "**Denied**"

- **Client ID --** dato in sola visualizzazione: consente di
  visualizzare il Client ID dell'utente che ha effettuato l'ordine in
  esame

> Il Client ID è un identificatore univoco utilizzato da Google
> Analytics e assegnato a ciascun utente che visita il sito web. E'
> legato allo specifico dispositivo e allo specifico browser e viene
> infatti memorizzato all'interno di un cookie (\_ga) salvato da Google
> proprio sul browser utilizzato dall'utente per visualizzare la pagina
> web.
>
> Potrebbero quindi verificarsi anche situazioni in cui due diversi
> ordini effettuati dallo stesso utente presentino due valori diversi
> per il Client ID (ad esempio perché i due ordini sono stati effettuati
> utilizzando browser o dispositivi differenti)
>
> Ovviamente nel caso in cui l'utente non dovesse aver prestato il
> relativo consenso per il tracciamento, il cookie di Google non potrà
> essere salvato e quindi eventuali ordini effettuati da questo stesso
> utente saranno privi di questo valore

- **Session ID** -- dato in sola visualizzazione: consente di
  visualizzare l'Id di sessione assegnato da Google alla visita durante
  la quale l'utente ha effettuato l'ordine in esame.

> Una sessione rappresenta un insieme di interazioni (ad esempio,
> visualizzazioni di pagina, eventi, acquisti) che un utente compie sul
> sito web, inizia quando l'utente accede al sito e può terminare ad
> esempio dopo 30 minuti di inattività, per cui tipicamente ordini
> diversi dello stesso utente avranno Session ID differenti
>
> Come per il Client ID anche il Session ID viene salvato in un cookie
> da Google e quindi nel momento in cui l'utente non dovesse aver
> prestato i relativi consensi per il tracciamento il campo in esame
> risulterà vuoto

- **Session Number** -- dato in sola visualizzazione: consente di
  visualizzare il Session Number associato da Google alla sessione di
  vista durante la quale l'utente ha effettuato l'ordine in esame.

> Il Session Number rappresenta il numero progressivo di sessioni che un
> utente ha avviato sul sito. Questo numero viene incrementato ogni
> volta che un utente inizia una nuova sessione ed è collegato al Client
> ID per mantenere un conteggio unico per ogni utente.
>
> Come per i precedenti valori anche il Session Number viene salvato in
> un cookie da Google e quindi nel momento in cui l'utente non dovesse
> aver prestato i relativi consensi per il tracciamento il campo in
> esame risulterà vuoto

- **GCLID** -- dato in sola visualizzazione

> Il GCLID (Google Click Identifier) è un identificatore univoco che
> Google utilizza per tracciare i click sugli annunci Google Ads. Viene
> aggiunto automaticamente agli URL come parametro quando è abilitato in
> Google Ads il tracciamento automatico (opzione questa che dovrebbe
> essere sempre attivata). Serve per collegare i dati dei click sugli
> annunci Google alle conversioni e ad altre azioni monitorate da
> strumenti come Google Ads e Google Analytics.
>
> Grazie al GCLID è quindi possibile associare il click di un utente su
> di un annuncio a: una campagna, una parola chiave, un tipo di
> dispositivo, l'orario del click permettendo quindi di misurare le
> performance degli annunci e le conversioni.
>
> Come per i precedenti valori anche il GCLID viene salvato in un cookie
> da Google. A differenza di quanto avveniva per i precedenti parametri,
> per fare in modo che il GCLID sia effettivamente valorizzato è
> necessario non solo che l'utente abbia prestato tutti i consensi del
> caso per il tracciamento ma anche che la visita al sito sia partita,
> ovviamente, da un annuncio Google Ads
>
> **ATTENZIONE!** il valore del GLID potrà o meno essere inserito nel
> file prodotto da Passweb, in relazione al processo di import delle
> conversioni offline, in base al valore parametro "**Inserisci GCLID
> export CSV**" presente alla pagina "Sito -- Preferenze" del Wizard
> (tab "Tracciamento Dati" sezione "Google Ads")
>
> Per maggiori informazioni in merito all'import delle conversioni
> offline si veda anche quanto indicato all'interno del relativo
> capitolo di questo manuale ( "*Google Ads User Provided Data e
> Conversioni Avanzate -- Import delle conversioni offline*")

- **FBP** -- dato in sola visualizzazione

> Utilizzato da Meta (Facebook) per il tracciamento degli utenti quando
> si implementa il Facebook Pixel o la Conversion API. Serve a
> identificare gli utenti e a migliorare l\'attribuzione delle azioni di
> marketing, come gli acquisti o le registrazioni. E', in sostanza, il
> corrispondente del Client ID nell'ambito del sistema di tracciamento
> di Facebook.
>
> E' salvato in un cookie del browser (fbp) e quindi come per tutti gli
> altri parametri nel momento in cui l'utente non dovesse aver prestato
> i relativi consensi per il tracciamento il campo in esame risulterà
> vuoto

- **FBC** -- dato in sola visualizzazione

> Utilizzato da Meta (Facebook) per il tracciamento delle conversioni
> quando si implementa il Facebook Pixel o la Conversion API. E', in
> sostanza, il corrispondente del GCLID nell'ambito del sistema di
> tracciamento di Facebook e serve quindi per collegare i dati dei click
> sugli annunci Facebook alle conversioni e ad altre azioni monitorate
> all'interno del proprio Business Manager
>
> E' salvato in un cookie del browser (fbc) e, proprio come il GCLID,
> affinché questo parametro sia effettivamente valorizzato è necessario
> non solo che l'utente abbia prestato tutti i consensi del caso per il
> tracciamento ma anche che la visita al sito sia partita, ovviamente,
> da un annuncio su Facebook.

