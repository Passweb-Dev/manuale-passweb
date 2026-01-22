# ATTIVAZIONE API PRESTASHOP



Come evidenziato nei precedenti capitoli di questo manuale a livello di
dati articolo lo scambio di informazioni tra Passweb e Prestashop può
avvenire via API oppure mediante la creazione e lo scambio di appositi
file CSV. A livello di importazione ordini invece l'integrazione Passweb
-- Prestashop può avvenire unicamente via API.

In ogni caso, indipendentemente dalla particolare metodologia di
pubblicazione articoli adottata e/o dal fatto di voler gestire o meno
anche l'importazione ordini, occorre considerare sempre che Passweb
necessita comunque di connettersi via API alla relativa installazione
Prestashop quanto meno per poter leggere informazioni fondamentali per
una corretta configurazione dell'Account (es. store e lingue in uso
all'installazione Prestashop) e per poter poi creare e gestire
correttamente le varie Inserzioni.

**In conseguenza di ciò diventa dunque obbligatorio e di fondamentale
importanza attivare e configurare correttamente le API Prestashop**.

Nel seguito di questo capitolo vedremo quindi la procedura da seguire
per poter attivare queste API e come poter prelevare tutte le
informazioni necessarie per poter poi configurare l'integrazione tra le
due piattaforme.

- La prima cosa da fare sarà quella di accedere alla propria
  installazione Prestashop con le credenziali di amministratore e
  portarsi poi all'interno della sezione "**Parametri Avanzati -
  Webservice**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_1.bmp](./assets/media/image585.png){width="4.967361111111111in"
height="3.532638888888889in"}

- Una volta effettuato l'accesso a questa sezione, verificare che
  l'interruttore "**Attiva servizio Web Prestashop**" sia impostato sul
  valore SI e, successivamente, cliccare sul pulsante "**Aggiungi una
  nuova chiave di servizio**" presente nella parte alta della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_2.bmp](./assets/media/image586.png){width="4.967361111111111in"
height="3.532638888888889in"}

- Assegnare una Descrizione alla chiave che si sta configurando, in
  maniera tale da poterla poi distinguere da eventuali altre chiavi
  presenti sulla propria installazione Prestashop (campo "**Descrizione
  Chiave**" all'interno della sezione "**Account Servizio web**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_3.bmp](./assets/media/image587.png){width="4.967361111111111in"
height="3.532638888888889in"}

> e cliccare poi sul pulsante "**Genera**" per generare l'Api Key che
> dovremo utilizzare per integrare le due piattaforme

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_4.bmp](./assets/media/image588.png){width="4.967361111111111in"
height="3.532638888888889in"}

- Impostare quindi la sezione "**Permessi**" come evidenziato in figura
  (lo schema di permessi considerato è relativo al caso generale ed è
  utile quini per attivare sia la pubblicazione articoli via API che
  l'importazione ordini)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_5.jpg](./assets/media/image589.jpeg){width="3.4868055555555557in"
height="4.434722222222222in"}

> **Metodi GET --** Intera colonna
>
> **Metodi PUT --** Attivare le seguenti risorse:

- categories

- combinations

- customers

- customizations

- images

- product_customization_fields

- product_feature_values

- product_features

- product_option_values

- product_options

- product_suppliers

- products

- order_carriers

- orders

- specific_prices

- stock_availables

> **Metodi POST --** Attivare le seguenti risorse:

- categories

- combinations

- customers

- customizations

- images

- manufacturers

- product_customization_fields

- product_feature_values

- product_features

- product_option_values

- product_options

- product_suppliers

- products

- specific_prices

> **Metodi DELETE --** Attivare le seguenti risorse:

- categories

- combinations

- customers

- customizations

- images

- orders

- order_histories

- product_customization_fields

- product_feature_values

- product_features

- product_option_values

- product_options

- product_suppliers

- specific_prices

> **ATTENZIONE!** Nel momento si dovesse decidere di non attivare il
> metodo DELETE per una delle risorse indicate (per essere certi ad
> esempio del fatto di non eliminare mai la relativa informazione
> presente su Prestashop) occorrerà poi verificare che questo non
> precluda il normale funzionamento dell'integrazione creando di fatti
> altri problemi non previsti
>
> **Metodi HEAD --** Attivare le seguenti risorse:

- categories

- combinations

- customers

- customizations

- images

- product_customization_fields

- product_feature_values

- product_features

- product_option_values

- product_options

- product_suppliers

- specific_prices

- stock_availables

> **ATTENZIONE! Lo schema di permessi potrebbe variare in relazione al
> metodo di pubblicazione articoli che si decide di adottare e/o in
> relazione al fatto di attivare o meno anche la gestione e
> l'importazione degli ordini effettuati sulla piattaforma terza**

- Una volta impostati i permessi come indicato, verificare che lo Stato
  di attivazione della chiave appena configurata sia effettivamente
  impostato sul valore SI

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prestashop_6.bmp](./assets/media/image590.png){width="4.967361111111111in"
height="3.532638888888889in"}

> e cliccare quindi sul pulsante "**Salva**", posto nella parta bassa
> della pagina, per salvare la chiave precedentemente generata con lo
> schema di permessi settato.

Al termine della procedura appena descritta è possibile verificare il
corretto accesso alle API Prestashop seguendo una delle procedure di
seguito indicate:

**[TEST 1]{.underline}**

- Aprire un browser all'indirizzo www.nomesitoprestashop.it/api

- Verrà visualizzata una maschera di richiesta delle credenziali di
  accesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\connessione_web_prestashop.bmp](./assets/media/image591.png){width="4.298611111111111in"
height="3.1166666666666667in"}

- Inserire all'interno del campo "Nome Utente" la chiave di accesso
  precedentemente configurata, lasciare il campo Password vuoto e
  cliccare su "Accedi"

- Nel caso in cui le API di Prestashop siano state correttamente
  configurate e siano effettivamente contattabili e utilizzabili da
  Passweb, verrà visualizzata una pagina del tipo di quella qui di
  seguito evidenziata contenente la struttura dei relativi webserivices

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\connessione_web_prestashop_2.bmp](./assets/media/image592.png){width="4.909027777777778in"
height="2.7465277777777777in"}

**[TEST 2]{.underline}**

Nel caso in cui il test precedente non dovesse dare esito positivo
eseguire questo test:

1.  Aprire un browser all'indirizzo
    [http://www.sito_prestashop.it/api?ws=chiave_di_accesso]{.underline}
    dove

    a.  [www.sito_prestashop.it]{.underline} = indirizzo del proprio
        sito prestashop

    b.  chiave_di_accesso = chiave di accesso precedentemente
        configurata

2.  Se le API di prestashop sono state configurate correttamente e sono
    effettivamente accessibili verrà visualizzata una pagina del tipo di
    quella qui di seguito evidenziata contenente la struttura dei
    relativi webserivices

![Videate\\connessione_web_prestashop_2.bmp](./assets/media/image593.png){width="4.909027777777778in"
height="2.7465277777777777in"}

**[TEST 3]{.underline}**

In alternativa ai TEST1 e TEST2 è possibile anche utilizzare un client
API come **Postman**
([[https://www.postman.com]{.underline}](https://www.postman.com)).
Questo strumento richiede maggiori conoscenze tecniche ma essendo uno
strumento esterno a Passweb consente di verificare la correttezza delle
chiamate e la presenza di eventuali errori in risposta che sono
indipendenti da Passweb

**ATTENZIONE!** Nel caso in cui la procedura di autenticazione appena
descritta non dovesse dare esito positivo e non si riuscisse quindi a
visualizzare la struttura dei Webservices Prestashop neppure Passweb
riuscirà a connettersi con il relativo sito e non sarà quindi possibile
attivare l'integrazione via API.

**Allo stesso modo la presenza di eventuali errori in risposta dalle API
Prestashop (verificabili anche con strumenti esterni come Postman)
potrebbero invalidare questo tipo di integrazione tra le due
piattaforme.**

In queste condizioni sarà necessario contattare l'assistenza del proprio
sito Prestashop e risolvere il problema prima di poter procedere con
l'integrazione. **Passepartout non fornisce alcun tipo di assistenza in
questo senso**

