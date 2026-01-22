# PARAMETRI DI INTEGRAZIONE



Per poter completare l'integrazione tra il proprio sito Ecommerce e la
piattaforma di pagamento Scalapay è necessario disporre di apposite
chiavi da inserire tra i parametri di configurazione del pagamento
Passweb.

Per ottenere queste chiavi sarà necessario:

1.  Completare la creazione del proprio account Scalapay

2.  Effettuare l'accesso alla piattaforma (
    <https://portal.scalapay.com/signup> ) utilizzando l'account appena
    creato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_5.bmp](./assets/media/image205.png){width="5.383333333333334in"
height="2.9743055555555555in"}

3.  Portarsi quindi all'interno della sezione "**Sviluppatore**"
    selezionando l'apposita voce di menu posta sulla sinistra della
    pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_scalapay_1.bmp](./assets/media/image206.png){width="5.201388888888889in"
height="3.50625in"}

> copiare la chiave presente in corrispondenza del campo "**Chiave
> API**" evidenziato in figura e inserirla nella maschera di
> configurazione del pagamento Passweb all'interno del campo "**Secret
> API Key**" (sezione "Configurazione Parametri del Gateway")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_6.bmp](./assets/media/image207.png){width="5.201388888888889in"
height="3.50625in"}

> **ATTENZIONE!** All'interno della "Secret Api Key" sono mappati i
> prodotti attivati in fase di sottoscrizione del relativo contratto ed
> è da questa chiave dunque che dipende l'effettiva possibilità, da
> parte del cliente, di suddividere poi il pagamento in 3 o in 4 rate

4.  Nel caso in cui **si sita utilizzando la versione v5 del widget di
    Scalapay** (parametro "**Versione Script = v5**"), per consentire un
    corretto funzionamento del relativo simulatore di pagamento, oltre
    alla Secret Api Key, sarà necessario impostare anche il "**Merchant
    Token**".

> In queste condizioni sarà quindi necessario copiare la stringa
> presente all'interno del campo "**Merchant Token**" presente sempre
> nella sezione "Sviluppatore" del proprio account Scalapay

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_8.bmp](./assets/media/image208.png){width="5.201388888888889in"
height="3.50625in"}

> e inserirla poi nell'omonimo campo presente nella maschera di
> configurazione del pagamento Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_9.bmp](./assets/media/image209.png){width="5.201388888888889in"
height="3.50625in"}

Come evidenziato nel precedente capitolo di questo manuale, infine,
Scalapay gestisce anche la modalità Server to Server mediante
l'attivazione di appositi WebHook.

Per attivare questa modalità sarà quindi necessario:

1.  Accedere, tramite il proprio account al Back Office di Scalapay,
    portarsi all'interno della sezione "**Sviluppatore**" e compilare il
    campo **Url Order Webhook** evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\scalapay_7.bmp](./assets/media/image210.png){width="5.201388888888889in"
height="3.50625in"}

> con il seguente indirizzo:
>
> **https://{www.miosito.it}/store/cart/checkout/scalapay/webhooks**
>
> dove, ovviamente, al posto di {www.miosito.it} andrà inserito l' url
> del proprio sito ecommerce

Una volta completata la creazione di questo end point la modalità Server
to Server sarà attiva e il gateway di Scalapay potrà quindi fornire una
risposta al sito ecommerce anche nel momento in cui l'utente dovesse
decidere, una volta completata la transazione, di chiudere il browser
senza tornare al sito.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di fare riferimento sempre alla
relativa manualistica di prodotto.

