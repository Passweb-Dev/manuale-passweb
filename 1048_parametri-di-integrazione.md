# PARAMETRI DI INTEGRAZIONE



Per poter completare l'integrazione tra il proprio sito Ecommerce e la
piattaforma di pagamento Stripe è necessario disporre di apposite chiavi
da inserire tra i parametri di configurazione del pagamento Passweb.

Per ottenere queste chiavi sarà necessario:

1.  Completare la creazione del proprio account Stripe

2.  Effettuare l'accesso alla piattaforma
    (<https://dashboard.stripe.com/login> ) utilizzando l'account appena
    creato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_1.bmp](./assets/media/image219.png){width="5.2659722222222225in"
height="2.785416666666667in"}

3.  Portarsi quindi all'interno della sezione "**Sviluppatori -- Chiavi
    API**" selezionando l'apposita voce di menu posta sulla sinistra
    della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_2.bmp](./assets/media/image220.png){width="5.552083333333333in"
height="3.325in"}

4.  Copiare le chiavi presenti in corrispondenza dei campi "**Chiave
    Pubblica**" e "**Chiave Segreta**" ed incollarle nei relativi
    parametri di configurazione del pagamento Passweb (sezione
    "Configurazione Parametri del Gateway")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_3.bmp](./assets/media/image221.png){width="5.844444444444444in"
height="3.4479166666666665in"}

**ATTENZIONE!** le chiavi di configurazione (pubblica e segreta) da
inserire all'interno dei campi evidenziati in figura sono diverse a
seconda del fatto che si stia utilizzando l'ambiente di test o quello
live di produzione

In fase di test sarà quindi necessario impostare il parametro "Ambiente
del gateway" sul valore "**Test**" e verificare che le chiavi inserite
all'interno dei successivi campi siano effettivamente quelle di test.

Prima di passare in produzione sarà invece necessario impostare il
parametro "Ambiente del gateway" sul valore "**Produzione**" e
verificare che le chiavi inserite all'interno dei successivi campi siano
quelle prelevate dall'ambiente live di Stripe.

Per poter passare su Stripe dall'ambiente di test a quello live è
sufficiente agire dal relativo controllo presente nella parte alta della
pagina

**ATTENZIONE!** per poter passare all'ambiente live è necessario per
prima cosa terminare l'attivazione del proprio account inserendo anche
tutti i dati del conto bancario su cui verranno poi accreditati i
pagamenti

Come evidenziato nel precedente capitolo di questo manuale, infine,
Stripe gestisce anche la modalità Server to Server mediante
l'attivazione di appositi WebHook.

Per attivare questa modalità sarà quindi necessario:

1.  Accedere, tramite il proprio account Stripe, alla relativa
    applicazione di back end e portarsi all'interno della sezione
    "**Sviluppatore -- WebHook**" cliccando sull'apposita voce di menu
    posta sulla sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_5.bmp](./assets/media/image222.png){width="5.552083333333333in"
height="3.325in"}

2.  Cliccare quindi sul pulsante "**Aggiungi endpoint**" posto nella
    parte alta della pagina e compilare la successiva maschera di
    creazione come di seguito indicato:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_7.bmp](./assets/media/image223.png){width="5.552083333333333in"
height="3.325in"}

- **URL endpoint**: inserire all'interno del campo in questione il
  seguente url

> **https://{urlsito}/store/cart/checkout/stripe/webhooks**
>
> dove, ovviamente, al posto di {urlsito} andrà inserito l'indirizzo del
> proprio sito web

- **Descrizione:** associare all'endpoint che si sta realizzando una
  descrizione (es. Integrazione Passweb)

- **Eventi da inviare:** selezionare tra quelli proposti in elenco i
  seguenti eventi:

  - **checkout.session.completed**

  - **checkout.session.async_payment_succeeded**

  - **checkout.session.async_payment_failed**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stripe_7a.bmp](./assets/media/image224.png){width="5.552083333333333in"
height="3.325in"}

3.  Cliccare quindi sul pulsante "**Aggiungi endpoint**" per completare
    la creazione del relativo endpoint

Una volta completata la creazione di questo end point la modalità Server
to Server sarà attiva e il gateway di Stripe potrà quindi fornire una
risposta al sito ecommerce anche nel momento in cui l'utente dovesse
decidere, una volta completata la transazione, di chiudere il browser
senza tornare al sito ecommerce.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di utilizzare la specifica
manualistica.

