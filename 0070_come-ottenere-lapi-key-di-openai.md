# COME OTTENERE L'API KEY DI OPENAI



Come già indicato all'interno del precedente capitolo di questo manuale
per poter utilizzare il modulo di intelligenza artificiale (Passweb AI)
è necessario da una parte acquistarlo all'interno di Passstore e,
dall'altra parte, disporre di un account OpenAI abilitato all'utilizzo
della API, con un metodo di pagamento correttamente configurato ed un
credito residuo maggiore di 0€

In questo senso dunque è molto importante non fare confusione, in fase
di creazione del proprio account, tra il piano di Chat GPT Plus e
l'accesso alle API di OpenAI.

Chat GPT Plus e le API OpenAI sono infatti due sistemi completamente
diversi, con due diverse modalità di utilizzo e due diversi piani di
pagamento.

Nello specifico Chat GPT Plus è un piano di abbonamento mensile che
permette di utilizzare GPT-4 esclusivamente nell'interfaccia web di Chat
GPT o nella relativa app e non può essere sfruttato in alcun modo per
sviluppare applicazioni o integrazioni esterne

**ATTENZIONE! Chat GPT Plus non consente di utilizzare le API di
OpenAI**

Le API di OpenAI consentono invece di integrare i diversi modelli di
intelligenza artificiale sviluppati dall'azienda all'interno di
applicazioni o di siti web di terze parti mediante l'utilizzo di
un'apposita API key.

In questo caso inoltre il sistema non prevede un piano di abbonamento
mensile, i costi variano infatti in base all'utilizzo che viene fatto
del servizio e dipendono quindi dalla quantità di dati scambiati, nello
specifico, dal numero di token utilizzati ossia dal volume di testo che
il motore di intelligenza artificiale dovrà andare a processare e questo
comprende sia il testo utilizzato da per formulare le domande che quello
utilizzato dall'AI per produrre poi le risposte.

Ovviamente i due sistemi (Chat GPT Plus e le API di Open AI) non sono
alternativi tra loro e, se necessario, possono tranquillamente essere
attivati ed utilizzati contemporaneamente considerando anche che
verranno poi fatturati su due canali diversi e con due modalità
differenti

Per maggiori informazioni relativamente ai due sistemi e ai relativi
costi di attivazione e gestione si consiglia comunque di fare sempre
riferimento al sito di OpenAI (<https://openai.com/>)

Detto questo, **nel momento in cui l'esigenza dovesse essere
esclusivamente quella di utilizzare i modelli di intelligenza
artificiale di Chat GPT all'interno del proprio sito Passweb, sarà
sufficiente attivare l'accesso alle API di OpenAI in maniera tale da
ottenere l'Api Key da inserire poi nei parametri di configurazione del
modulo Passweb.**

In questo senso sarà quindi necessario:

- Accedere all'indirizzo <https://platform.openai.com/>, cliccare sul
  pulsante "**Sign up**" posto nella parte alta della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_1.bmp](./assets/media/image360.png)

> e completare poi la creazione dell'account inserendo tutti i dati
> richiesti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_2.bmp](./assets/media/image361.png)

> Ovviamente nel caso in cui si dovesse disporre già di un account
> OpenAI non sarà necessario crearne uno nuovo ma sarà sufficiente
> effettuare l'accesso con le proprie credenziali

- Una volta creato l'account ed effettuato l'accesso portarsi
  all'interno della sezione "**API keys**" e cliccare sul pulsante
  "**Create new secret key**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_3.bmp](./assets/media/image362.png)

- Nella successiva maschera assegnare un nome all'API key che si sta
  creando e associarla anche ad uno specifico progetto.

> OpenAI consente infatti di gestire all'interno del proprio account più
> progetti differenti e di assegnare quindi a ciascuno di essi e/o a
> specifici team di utenti chiavi di configurazione differenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_4.bmp](./assets/media/image363.png)

- Mantenere selezionata l'opzione "**All**" in corrispondenza della voce
  "**Permission**" e cliccare quindi sul pulsante "**Create secret
  key**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_5.bmp](./assets/media/image364.png)

- Considerando che l'API key appena creata è l'elemento grazie al quale
  poter accedere programmaticamente alle API di OpenAI, e quindi di
  interagire con i vari modelli di intelligenza artificiale (producendo
  di fatto dei costi per il proprietario dell'account), nella successiva
  maschera verrà chiaramente indicato di non condividere la chiave in
  oggetto con nessuno e verrà indicato anche che, per ragioni di
  sicurezza la chiave appena generata non sarà più visibile all'interno
  del proprio account per cui nel momento in cui dovessimo perderla
  saremo poi costretti ad eliminarla e a crearne una nuova

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_6.bmp](./assets/media/image365.png)

> In considerazione di ciò **è quindi indispensabile, prima di chiudere
> la maschera evidenziata in figura, copiare la chiave appena generata e
> salvarla in un posto a noi accessibile in maniera tale da poterla poi
> riprendere quando dovremo inserirla in fase di configurazione del
> modulo Passweb AI**

Considerando che, come precedentemente indicato, l'utilizzo delle API di
Open AI è soggetto ad un piano di pagamento a consumo, la creazione
dell'API key non è di per sé sufficiente a rendere il modulo Passweb AI
effettivamente utilizzabile.

Per completare il processo di attivazione sarà infatti necessario
inserire all'interno del proprio account OpenAI anche un metodo di
pagamento valido

Per inserire un nuovo metodo di pagamento è necessario portarsi
all'interno della sezione "**Billing**" e cliccare sul pulsante "**Add
payment details**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_7.bmp](./assets/media/image366.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_8.bmp](./assets/media/image367.png)

Una volta inseriti i dati della carta di credito e codificato quindi il
metodo di pagamento, sarà poi necessario utilizzare tale metodo per
caricare sull'account un credito maggiore di 0€

![Videate\\account_openai_9.bmp](./assets/media/image368.png)

All'interno del proprio account OpenAI, infine, sarà sempre possibile
tenere sotto controllo gli importi relativi ai costi attualmente
sostenuti (sezione "**Usage**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_10.bmp](./assets/media/image369.png)

E, volendo, sarà possibile impostare anche eventuali limiti di utilizzo
per non incorre in fatture impreviste (sezione "Limits")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_openai_11.bmp](./assets/media/image370.png)

Per maggiori informazioni relativamente a questo tipo di procedure si
rimanda alla documentazione della specifica piattaforma

Completata l'attivazione dell'account OpenAI e ottenuta l'API key
necessaria per l'integrazione potremo passare alla configurazione del
modulo Passweb AI

