# TRACCIAMENTO DELLO USER ID



Come già indicato in altri capitoli di questo manuale il tracciamento
mediante User id consente di associare i visitatori del sito ad un
identificatore univoco che dovrà essere assegnato agli utenti stessi
direttamente dall'applicativo, tipicamente mediante il processo di login
ed è sicuramente il metodo di identificazione più accurato tra quelli di
disponibili in GA4 (gli atri sono Google Signals ed il classico Client
id) inquanto consente di riconoscere e seguire facilmente l'utente in
maniera cross device e cross platform.

Per maggiori informazioni relativamente all'utilizzo dello User id in
GA4 è possibile fare riferimento a quanto indicato all'interno del
capitolo *"Google Analytics -- Google Analytics 4 -- Universal Analytics
e GA4 Principali differenze -- Privacy e Raccolta dei dati -- User ID"*
(per approfondire l'argomento si consiglia comunque di fare sempre
riferimento alla documentazione ufficiale messa a disposizione da Google
o alle numerose guide dedicate presenti in rete)

**ATTENZIONE!** attivando il tracciamento mediante User ID si ha anche
la responsabilità di garantire che l\'utilizzo dell' ID utente sia
conforme ai Termini di servizio di Google Analytics. Non vanno quindi
utilizzate informazioni che consentono l'identificazione personale e,
allo stesso modo, sarà necessario, da una parte, fornire nelle Norme
sulla gestione della privacy del proprio sito un'informativa adeguata
circa l'utilizzo degli identificatori e, dall'altra parte, verificare di
aver gestito in maniera adeguata la richiesta di consenso preventivo per
il tracciamento.

In ogni caso **Lo User ID non deve contenere in alcun modo informazioni
che una terza parte potrebbe utilizzare per determinare l'identità di un
utente**.

Di seguito verrà illustrata la procedura da seguire per poter tracciare
lo User id in GA4 mediante GTM. Si tratta essenzialmente di 4 semplici
step:

- Step 1: configurare la proprietà GA4 per la raccolta dati mediante
  User id

- Step 2: Inserire lo User id nei Data Layer gestiti da Passweb

- Step 3: Creare una variabile di livello dati per memorizzare lo User
  id

- Step 4: Inserire lo User id come parametro del Tag di configurazione
  di GA4

##### STEP 1: CONFIGURARE LA PROPRIETA' DI GA4 PER LA RACCOLTA DATI MEDIANTE USER ID

In GA4 la raccolta dei dati mediante User ID dipende dal metodo
utilizzato da Analytics stesso per associare gli eventi agli utenti,
metodo questo che può essere impostato all'interno della sezione
"**Identità Report**" presente nell'interfaccia di amministrazione della
relativa proprietà GA4

![](./assets/media/image142.png)

GA4 imposta a default l'Identificazione nei report sull'opzione
"**Sfumato**" il che significa che verranno valutati, nell'ordine, i
seguenti metodi di identificazione degli utenti: prima di tutto lo User
ID poi i Google Signals, l'ID Dispositivo (Client ID) e infine i Modelli
automatici

In queste condizioni dunque, nel momento in cui lo User ID dovesse
essere effettivamente disponibile questo verrà utilizzato come metodo di
identificazione degli utenti per tutti i rapporti di GA4. Se non
presente verranno invece utilizzati i Google Signals e a seguire Client
ID e Modelli Automatici

Allo stesso modo impostando l'Identificazione nei report sull'opzione
"**In osservazione**" verranno valutati, nell'ordine, i seguenti metodi
di identificazione degli utenti: prima di tutto lo User ID poi i Google
Signals, l'ID Dispositivo (Client ID). Non verranno invece presi in
considerazione i Modelli Automatici.

In sostanza dunque per configurare la proprietà GA4 per la raccolta dati
mediante User id è sufficiente verificare che l'Identificazione nei
report sia stata impostata su una delle due opzioni: "Sfumato" (opzione
abilitata a default) oppure "In osservazione"

##### STEP 2: INSERIRE LO USER ID NEI DATA LAYER GESTITI DA PASSWEB

Il secondo passaggio è quello che prevede l'inserimento nei Data Layer
gestiti da Passweb dello User id che Passweb stesso assegna
automaticamente a tutti gli utenti che hanno effettuato l'autenticazione
sul sito.

Per fare questo è sufficiente selezionare il parametro "**Usa User_id
nel Data Layer**" presente alla pagina "**Sito -- Preferenze**" del
Wizard (tab "**Tracciamento Dati**" sezione "**Google Tag Manager**")
come nella figura di seguito riportata

![](./assets/media/image143.png)

**ATTENZIONE!** prima di attivare, lato Passweb, il tracciamento
mediante User ID è necessario accertarsi bene di gestire in maniera
corretta la richiesta agli utenti di tutti i consensi necessari, di aver
sistemato in maniera adeguata l'informativa privacy in uso sul sito e,
in generale, di soddisfare tutto quanto richiesto dal GDPR in merito di
trattamento dei dati

A questo punto è anche possibile verificare il corretto inserimento del
parametro "user_id" nei Data Layer di Passweb utilizzando la modalità
"Anteprima" di GTM e andando ad esaminare il push dei dati inseriti da
Passweb nel Data Layer di uno degli eventi tracciati all'interno del
proprio sito

![](./assets/media/image144.png)

##### STEP 3: CREARE UNA VARIABILE DI LIVELLO DATI PER MEMORIZZARE LO USER ID

Un volta abilitata la proprietà GA4 per la raccolta dati tramite User id
e impostato il proprio sito Passweb in modo tale da inserire nei Data
Layer generati in corrispondenza dei vari eventi anche il parametro
"User_id", dovremo ora fare in modo che GTM possa recuperare questo dato
dai rispettivi Data Layer.

In questo senso andremo quindi a creare un'apposita variabile, in
maniera del tutto analoga a quanto già fatto per le altre variabili
create per il tracciamento degli eventi ecommerce, mappandola, questa
volta ovviamente, sul parametro "User_id"

Seguendo dunque la stessa procedura indicata nel precedente capitolo
"*Variabile GA4 -- DLV ecommerce.items*" creare ora una nuova variabile
di livello dati con le seguenti caratteristiche:

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV user_id

**Contenuto della variabile**: identificativo utente assegnato
automaticamente da Passweb a tutti gli utenti che fanno login sul sito

**Tag in cui utilizzare la variabile**: tag di configurazione di GA4
oppure Tag del singolo evento per cui si desidera tracciare lo User_id

**Nome varabile di livello dati**: impostare sul valore "**user_id"**"

![](./assets/media/image145.png)

##### STEP 4: INSERIRE LO USER ID COME PARAMETRO DEL TAG DI CONFIGURAZIONE DI GA4

Una volta acquisito lo User id anche in GTM l'ultimo passaggio sarà ora
quello che prevede di inviare il dato a GA4 e per far questo sarà
sufficiente inserirlo come parametro aggiuntivo nella configurazione del
Tag per cui si vuole tracciare anche questo tipo di dato.

In questo senso la cosa importante da sottolineare è che se l'esigenza
dovesse essere quella di tracciare lo User id in relazione ad un singolo
evento (es. purchase) sarebbe sufficiente inserirlo come parametro
aggiuntivo nella configurazione del singolo Tag.

Nel momento in cui invece l'esigenza dovesse essere quella di
**raccogliere lo User id in relazione a tutti gli eventi tracciati
(opzione questa consigliata) sarà sufficiente inserirlo come parametro
aggiuntivo nel Tag di configurazione di GA4** e questo verrà
automaticamente inserito anche in tutti gli altri eventi.

Supponendo dunque di voler soddisfare quest'ultima casistica apriamo il
Tag di configurazione di GA4, apriamo la sezione "**Campi da
impostare**" e clicchiamo sul pulsante "**Aggiungi Riga**" come nella
figura di seguito riportata

![](./assets/media/image146.png)

Aggiungere quindi il nuovo parametro completando i campi "Nome
parametro" e "Valore" come nella figura di seguito riportata

![](./assets/media/image147.png)

- **Nome parametro**: user_id

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV user_id**" precedentemente creata (Step 3)

##### VERIFICA DELLA CONFIGURAZIONE

Una volta completati tutti e 4 gli Step indicati nei precedenti capitoli
possiamo ora andare a verificare il corretto passaggio dei dati dal
nostro sito alla relativa proprietà di GA4.

Per far questo è sufficiente ancora una volta utilizzare la modalità
"Anteprima" di GTM e la Debug View di GA4.

In particolare, una volta avviata la modalità "Anteprima" di GTM sarà
necessario portarsi nel tab in cui è stato aperto il nostro sito,
effettuare l'autenticazione con un utente registrato e navigare il sito
in maniera tale da produrre l'attivazione di alcuni eventi ecommerce e
dei relativi Tag di tracciamento (es. view_item_list).

Fatto questo dovremo portarci nella Debug View di GA4 e verificare che
tra parametri arrivati con l'evento tracciato ci sia anche lo user_id
come nella figura di seguito riportata

![](./assets/media/image148.png)

##### UTILIZZARE LO USER ID NEI REPORT

Una volta verificato che lo User id assegnato da Passweb agli utenti che
effettuato il login viene correttamente passato ad Analytics resta ora
da capire come poter effettivamente visualizzare ed utilizzare questo
dato nei vari report.

In questo senso è bene sottolineare due cose di fondamentale importanza

- Lo user_id in GA4 è una dimensione predefinita per cui può
  effettivamente essere inserita e gestita nei vari report

- A default GA4 non consente di visualizzare esattamente il valore dello
  user_id ma consente di distinguere solamente tra gli utenti che hanno
  o non hanno effettuato l'autenticazione al sito

Inoltre, nei pochi report standard attualmente presenti in GA4 questo
dato non è presente per cui dovrà essere, eventualmente, inserito nei
report customizzati che ogni utente può costruirsi all'interno della
sezione "**Esplora**"

![](./assets/media/image149.png)

Per far questo sarà quindi necessario creare un nuovo report
personalizzato o, eventualmente, accedere ad uno di quelli già creati e
cliccare sul pulsante + accanto alla voce "**Dimensioni**" evidenziata
in figura

![](./assets/media/image150.png)

in maniera tale da aprire, nella parte destra dello schermo, l'elenco
delle dimensioni disponibili che possono effettivamente essere aggiunte
al report che stiamo esaminando.

Come detto lo user_id è una dimensioni predefinita in GA4 per cui
dovremo semplicemente aprire la sezione "**Utente**" evidenziata in
figura, spuntare la voce "**Accesso eseguito con lo User-ID**" e
cliccare sul pulsante "**Importa**" presente nella parte alta della
maschera

![](./assets/media/image151.png)

Fatto questo troveremo ora la dimensione appena selezionata assieme a
tutte le atre presenti nella relativa colonna e che possono
effettivamente essere inserite nel report che stiamo esaminando

![](./assets/media/image152.png)

Sarà quindi sufficiente selezionare questa dimensione e trascinarla tra
le righe o le colonne gestite nel report

![](./assets/media/image153.png)

Fatto questo il report verrà rielaborato in tempo reale mostrando quindi
anche (laddove presente) il dato relativo alla dimensione appena
inserita

![](./assets/media/image154.png)

**ATTENZIONE!** Come precedentemente evidenziato questa dimensione non
ci consente di visualizzare esattamente l'id assegnato all'utente in
Passweb ma offre solo un valore booleano che ci consente di distinguere,
ad esempio, tra gli eventi che hanno effettivamente uno user_id
associato perché generati da utenti che hanno fatto login sul sito e
quelli che invece non lo hanno perché generati da utenti non autenticati

Nel momento in cui l'esigenza dovesse essere invece quella di
visualizzare in determinati report esattamente lo user_id assegnato in
Passweb ai vari utenti (in sostanza lo stesso valore che possiamo vedere
nella Debug View), potremmo comunque pensare di passare questo valore ad
Analytics anche attraverso un ulteriore parametro (es. passweb_user_id)
in maniera tale da poter creare poi una dimensione personalizzate
(ovviamente con ambito "Utente") da inserire in tutti i report in cui
questo dato risulta effettivamente necessario.

Per maggiori informazioni relativamente alla creazione di report custom,
di dimensioni custom ecc... si consiglia di fare sempre riferimento alla
documentazione ufficiale messa a disposizione da Google o alle numerose
guide presenti in rete.

