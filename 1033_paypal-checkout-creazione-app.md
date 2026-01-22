# PAYPAL CHECKOUT -- CREAZIONE APP



Come indicato nel precedente capitolo di questo manuale, per poter
attivare in maniera corretta il metodo di pagamento **PayPal Checkout**
sarà necessario soddisfare alcuni requisiti di fondamentale importanza.

Nello specifico sarà necessario:

- Disporre di un proprio account sull'ambiente developer di PayPal
  [**https://developer.paypal.com**](https://developer.paypal.com)

- Creare un APP da cui poter prelevare i parametri di configurazione

- Attivare apposti webhooks

Di seguito viene quindi indicata la procedura da seguire per ottenere
quanto richiesto.

1.  Accedere all'indirizzo <https://developer.paypal.com> ed effettuare
    l'accesso con il proprio account PayPal.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login51.bmp](./assets/media/image170.png){width="4.980555555555555in"
height="3.4347222222222222in"}

2.  Una volta effettuato l'accesso verremo ricondotti nella
    **Dashboard** da dove dovremo poi cliccare sul pulsante "A**pps &
    Credentials**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login53a1.bmp](./assets/media/image171.png){width="5.486805555555556in"
height="3.3569444444444443in"}

> in maniera tale da accedere alla sezione di creazione e gestione delle
> proprie App

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login53.bmp](./assets/media/image172.png){width="5.486805555555556in"
height="3.3569444444444443in"}

> dove avremo la possibilità di creare App sia nell'ambiente **Sandbox**
> di test che in quello **Live** di produzione. Ovviamente il tutto
> dovrà essere coerente con quanto impostato sul pagamento Passweb in
> corrispondenza del parametro "**Ambiente del Gateway**".
>
> In fase di sviluppo sarà quindi necessario da una parte impostare tale
> parametro sul valore "**Test**" e dall'altra parte creare in PayPal un
> APP in ambiente **Sandbox**.
>
> Allo stesso modo nel momento in cui si deciderà di passare in
> produzione sarà necessario da una parte impostare il parametro Passweb
> "Ambiente del Gateway" sul valore "**Produzione**" e dall'altra parte
> creare in PayPal un APP in ambiente **Live**

3.  Selezionare quindi, mediante l'apposito controllo l'ambiente
    desiderato e cliccare poi sul pulsante "**Create app**"

4.  Assegnare un nome all'app e cliccare sul pulsante "**Create app**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout.bmp](./assets/media/image173.png){width="5.220833333333333in"
height="3.1951388888888888in"}

> **ATTENZIONE!** Lavorando in ambiente "Sandbox" sarà necessario
> indicare in questa fase anche un account Sandbox Business
> appositamente creato

5.  Completata la creazione dell'APP verremo automaticamente ricondotti
    ad una pagina di dettaglio di questa stessa APP da cui poter
    prelevare i valori richiesti (**Client ID** e **Secret**) per
    attivare correttamente la modalità di pagamento in esame sul nostro
    sito Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout2.bmp](./assets/media/image174.png){width="5.220833333333333in"
height="3.1951388888888888in"}

6.  Copiare quindi quanto indicato all'interno del campo **Client ID**
    ed incollarlo nel corrispondente campo della sezione
    "**Configurazione Parametri del Gateway**" nella maschera di
    configurazione del pagamento Passweb.

> Allo stesso modo copiare quanto indicato all'interno del campo
> **Secret** (cliccando preventivamente sul pulsante "Show") e
> incollarlo nel campo "**Secret Stringa**" della sezione
> "**Configurazione Parametri del Gateway**" nella maschera di
> configurazione del pagamento Passweb.

7.  Sempre nella pagina di dettaglio dell'APP portarsi all'interno della
    sezione relativa alle Features dell'APP e verificare che sia tutto
    impostato come in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout3.bmp](./assets/media/image175.png){width="5.220833333333333in"
height="3.1951388888888888in"}

8.  A questo punto sarà necessario attivare i webhooks richiesti.
    Restando quindi ancora una volta nella maschera di dettaglio
    dell'APP portarsi all'interno della sezione "**Sandbox / Live
    Webhooks**" e cliccare sul pulsante "**Add Webhook**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout4.bmp](./assets/media/image176.png){width="5.220833333333333in"
height="3.201388888888889in"}

9.  Inserire quindi all'interno del campo "**Webhook URL**" il seguente
    indirizzo:

> **https://\<urlsito\>/store/cart/checkout/paypal/webhooks**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout5.bmp](./assets/media/image177.png){width="4.967361111111111in"
height="3.363888888888889in"}

> **ATTENZIONE!** l'attivazione dei webhooks richiede necessariamente la
> presenza di un certificato SSL sul proprio sito

10. All'interno della sezione "**Event types**" flaggare invece le
    seguenti tipologie di eventi:

    a.  **Checkout order approved**

    b.  **Checkout order completed**

    c.  **Checkout order saved**

    d.  **Checkout order voided**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout6.bmp](./assets/media/image178.png){width="5.220833333333333in"
height="3.201388888888889in"}

e.  **Payment authorization created**

f.  **Payment authorization voided**

g.  **Payment capture completed**

h.  **Payment capture denied**

i.  **Payment capture pending**

j.  **Payment capture refunded**

k.  **Payment capture reversed**

l.  **Payment order cancelled**

m.  **Payment order created**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\app_payapl_checkout7.bmp](./assets/media/image179.png){width="5.220833333333333in"
height="3.201388888888889in"}

11. Salvare l'APP cliccando sul pulsante "Save" presente a fondo pagina

