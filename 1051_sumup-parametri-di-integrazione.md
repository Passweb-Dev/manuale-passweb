# SUMUP -- PARAMETRI DI INTEGRAZIONE



Per poter completare l'integrazione tra il proprio sito Ecommerce e il
gateway di pagamento SumUp è necessario disporre di apposite chiavi da
inserire tra i parametri di configurazione del pagamento Passweb.

Per ottenere queste chiavi sarà necessario:

1.  Completare correttamente la creazione di un proprio merchant account
    sul portale di SumUp

2.  Accedere al portale di sviluppo di SumUp (
    <https://me.sumup.com/developers> ) con le credenziali dell'account
    appena creato. Dal manu Account, posto nella parte alta della pagina
    selezionare la voce "**OAuth2 Apps**"

![](./assets/media/image232.png)

> e cliccare quindi sul pulsante "**Create application**"

![](./assets/media/image233.png)

3.  Completare il form assegnando un nome all'applicazione e indicando
    l'url del proprio sito

![](./assets/media/image234.png)

> Cliccare quindi sul pulsante "**Register application**".

4.  Nella successiva maschera completare, eventualmente, la sezione
    "**Application consent screen**" con i dati opzionali richiesti

![](./assets/media/image235.png)

> Lasciare inalterata la sezione relativa agli Scopes

![](./assets/media/image236.png)

> e selezionare invece, nella sezione "**Restricted Scopes**" la voce
> payments

![](./assets/media/image237.png)

> Cliccare quindi sul pulsante "**Save**"

5.  Sempre all'interno della stessa pagina, all'interno della sezione
    "**Client Secret**", cliccare ora sul pulsante "**Create client
    secret**"

![](./assets/media/image238.png)

6.  Completare quindi il form di creazione delle credenziali come di
    seguito indicato:

![](./assets/media/image239.png)

- **Client name**: nome dell'applicazione per cui si stanno generando le
  credenziali Oauth (es. nome del sito)

- **Application type**: Web

- **Authorized redirect URL**: inserire il seguente url

> https://{urlsitoweb}/wizard/callbackpaymets/sumup
>
> dove ovviamente al posto {urlsitoweb\] andrà inserito l'indirizzo del
> proprio sito ecommerce

- **Authorized Javascript Origin (Facoltativo):** non compilare

> e cliccare sul pulsante "**Save**"

7.  Una volta completata correttamente la creazione delle credenziali
    Oauth verrà generato un file .json all'interno del quale saranno
    contenute le chiavi di integrazione da copiare e incollare nei
    parametri di configurazione del pagamento Passweb

> Per visualizzare queste chiavi sarà sufficiente cliccare sul "**Client
> name**" relativo al client secret appena creato

![](./assets/media/image240.png)

> e nella successiva maschera cliccare sul pulsante "**Download**"

![Videate\\sumup_7a.bmp](./assets/media/image241.png)

8.  Aprire quindi il file scaricato al punto precedente con un normale
    editor di testi (es. notepad)

![](./assets/media/image242.png)

> e copiare il valore dei parametri "**client_id**" e
> "**client_secret**" all'interno dei relativi campi presenti tra i
> parametri di configurazione del pagamento Passweb

![](./assets/media/image243.png)

9.  Completare quindi la configurazione del pagamento inserendo
    all'interno del campo "**Merchant Code**" l'identificativo merchant
    del proprio account SumUp, codice questo che può essere trovato
    nella Dashboard del proprio account Sum Up

![](./assets/media/image244.png)

nella parte alta della pagina immediatamente al di sotto del nome utente

![](./assets/media/image245.png)

**ATTENZIONE!** per maggiori informazioni relativamente a come poter
passare su SumUp dall'ambiente di test a quello di produzione si
consiglia di fare riferimento alla documentazione del relativo portale
e/o alla relativa assistenza

