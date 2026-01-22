# BRAINTREE -- ATTIVAZIONE PAGAMENTO PAY PAL



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui si dovesse decidere di abilitare, tra le opzioni messe a
disposizione da Braintree, il pagamento mediante PayPal non sarà
sufficiente attivare l'apposito flag all'interno di Passweb ma, affinché
tutto possa funzionare in maniera adeguata, sarà necessario configurare
correttamente il pagamento PayPal anche all'interno del backoffice di
Braintree secondo quanto indicato al seguente link
<https://developer.paypal.com/braintree/articles/guides/fraud-tools/basic/avs-cvv-rules>

In questo senso Braintree mette a disposizione due diversi metodi per
testare il pagamento mediante PayPal:

- **Mocked PayPal testing:** metodo di default.

> Più semplice da attivare inquanto non prevede il collegamento con
> account di test PayPal ma, per contro, non consente, ovviamente, di
> testare l'integrazione completa tra Braintree e PayPal

- **Linked PayPal testing:** richiede delle operazioni aggiuntive, tra
  cui la configurazione di un account developer e Sandbox di PayPal da
  collegare alla Sandbox di Braintree ma, proprio per questo, consente
  di testare in tutti gli aspetti la completa integrazione tra le due
  piattaforme

Nel seguito di questo capitolo vedremo più nel dettaglio la procedura da
seguire per attivare la fase di test in modalità "**Linked PayPal
testing**" dando per scontato di avere già a disposizione un account
developer di PayPal su cui poter operare (per maggiori informazioni in
merito a come poter attivare e gestire un Account sandbox di PayPal si
faccia riferimento anche ai precedenti capitoli di questo manuale)

**ATTEZIONE!** Va da sé ovviamente che per poter attivare su Braintree,
in ambiente di produzione, il pagamento mediante PayPal sarà necessario
disporre anche di un account PayPal di produzione perfettamente
funzionante

- Effettuare il login al proprio account developer di PayPal e accedere
  alla sezione "**Sandbox accounts**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_1.bmp](./assets/media/image80.png){width="5.370138888888889in"
height="3.234027777777778in"}

- Creare un account sandbox di tipo **Business** selezionando anche lo
  stesso paese scelto in fase di creazione dell'account sandbox di
  Braintree

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_2.bmp](./assets/media/image81.png){width="5.370138888888889in"
height="3.234027777777778in"}

- Accedere quindi alla sezione "**Apps & Credentials**" selezionando
  l'apposita voce di menu presente anche in testata e procedere poi alla
  creazione di una nuova APP cliccando sul relativo pulsante "**Create
  App**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_3.bmp](./assets/media/image82.png){width="5.370138888888889in"
height="3.234027777777778in"}

- In fase di creazione dell'APP flaggare la tipologia "**Merchant**" e
  selezionare anche dal relativo menu a tendina il sandbox Account
  creato al punto precedente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_4.bmp](./assets/media/image83.png){width="5.370138888888889in"
height="3.234027777777778in"}

- Completata la creazione dell'App verremo ricondotti automaticamente
  alla sua pagina di dettaglio dove ci verranno mostrate le credenziali
  API (Client ID e Secret key) relative a questa stessa APP, credenziali
  che dovremo annotarci da qualche parte perché ci verranno poi
  richieste anche all'interno di Braintree per completare il
  collegamento tra le due piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_5.bmp](./assets/media/image84.png){width="5.370138888888889in"
height="3.234027777777778in"}

- Effettuare ora l'autenticazione al proprio account sandbox di
  Braintree aprire il menu delle impostazioni (icona raffigurante una
  piccola rotellina posta in testata) e selezionare la voce "Processing"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_6.bmp](./assets/media/image85.png){width="5.370138888888889in"
height="3.234027777777778in"}

- All'interno della sezione Payment Methods cliccare sul link "**Link
  Sandbox**" presente in corrispondenza della sezione "PayPal"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_7.bmp](./assets/media/image86.png){width="5.370138888888889in"
height="3.234027777777778in"}

- Inserire nel relativo form i dati richiesti (**Email**, **Client ID**
  e **Secret ID**) relativi all'account Sandbox di PayPal creato nei
  precedenti passaggi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_paypal_8.bmp](./assets/media/image87.png){width="5.370138888888889in"
height="3.234027777777778in"}

> Cliccando quindi sul pulsante **Link PayPal SandBox** avremo
> completato il collegamento tra le due piattaforme e, in fase di test,
> potremo quindi verificare l'intero flusso del pagamento Braintree
> mediante PayPal
>
> **ATTENZIONE!** Essendo il tutto creato in ambiente Sandbox, in fase
> di pagamento dovremo utilizzare, chiaramente, delle credenziali di
> test
>
> **ATTENZIONE!** Gli stessi passaggi andranno eseguiti allo stesso modo
> anche per collegare i relativi ambienti (Braintree e PayPal) di
> produzione

