# CONFIGURAZIONE ACCOUNT



Condizione **necessaria e indispensabile** per poter integrare il
proprio sito Passweb con la piattaforma Amazon è quella di **essere
registrati in Amazon Seller Central come Venditore Pro**.

Per realizzare questo tipo di integrazione Passweb utilizza le Amazon
Selling Partner API (SP-API)

La prima cosa da fare sarà quindi quella di recarsi al seguente
indirizzo <https://sellercentral.amazon.it/gp/homepage.html>,

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_1.bmp](./assets/media/image181.png){width="4.16875in"
height="2.9090277777777778in"}

cliccare sul pulsante "**Registrati ora**" e completare la creazione del
proprio Account Venditore, facendo attenzione, ancora una volta, al
fatto di creare un Account di tipo Professionale

**ATTENZIONE! Account Venditore di tipo Individuale non permettono di
realizzare l'integrazione tra il proprio sito Passweb e i marketplace
Amazon.**

Per maggiori informazioni relativamente alle diverse tipologie di
Account, alle relative modalità di creazione e ad eventuali costi di
gestione si rimanda alla specifica documentazione Amazon presente in
rete (es.
<https://services.amazon.it/servizi/vendita-su-amazon/caratteristiche-e-vantaggi.html>
).

Una volta in possesso di un Account Venditore di tipo Pro il passo
successivo è quello che prevede di autorizzare lo sviluppatore
"Passepartout" ad utilizzare questo stesso Account per pubblicare
articoli su uno dei Marketplaces Amazon.

Per fare questo è necessario agire dalla sezione "**Gestione Account**"
accessibile dalla voce di menu ***"*Catalogo -- Amazon*"*.**

All'interno di questa sezione verrà infatti visualizzata la maschera
"**Lista degli Account** **Amazon**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_11.bmp](./assets/media/image182.png){width="5.825in"
height="3.4090277777777778in"}

contenente l'elenco di tutti gli Account attualmente collegati al
proprio sito Ecommerce.

Il pulsante **"Aggiungi Account"** ( ) presente nella contestuale barra
degli strumenti, consente di avviare la procedura mediante la quale
concedere, allo sviluppatore "Passepartout", l'autorizzazione ad
utilizzare il proprio Account Venditore Pro per mettere in vendita su
uno o più Marketplace Amazon gli articoli presenti all'interno del sito
Ecommerce.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Dati Account**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_dati_account_api.bmp](./assets/media/image183.png){width="5.825in"
height="3.4090277777777778in"}

all'interno della quale dover impostare un valore per i seguenti campi:

- **Descrizione**: consente di associare all'account in esame una
  specifica descrizione in maniera tale da poterlo poi identificare
  nella lista degli Account attualmente configurati e gestiti
  all'interno del sito

- **Paese**: consente di specificare il paese, e quindi il marketplace,
  in relazione al quale creare l'account. Nel relativo menu a tendina
  verranno proposti solo ed esclusivamente i paesi relativi ai
  Marketplace attivi (per maggiori informazioni relativamente a come
  poter attivare uno specifico marketplace si veda anche quanto indicato
  nel successivo capitolo "*Marketplace*" di questo manuale)

> **ATTENZIONE!** E' necessario creare un account distinto per ogni
> singolo marketplace con cui si vuol interagire indipendentemente dal
> fatto che il marketplace in esame sia abilitato alla sola ricezione di
> nuovi ordini o anche alla pubblicazione di articoli

Dopo aver impostato i due campi sopra indicati sarà necessario cliccare
sul pulsante "**Genera Token**". In questo modo verrà infatti aperta la
pagina di accesso ad **Amazon Seller Central**.

![Videate\\amazon_1.bmp](./assets/media/image184.png){width="4.16875in"
height="2.9090277777777778in"}

dove sarà necessario autenticarsi utilizzando le credenziali
dell'Account Venditore Pro precedentemente registrato.

Una volta effettuata l'autenticazione verrà visualizzata la maschera
attraverso cui concedere all'applicazione Passepartout l'autorizzazione
ad utilizzare questo stesso Account per pubblicare articoli su uno dei
Marketplaces Amazon.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\autorizza_integrazione_passweb.bmp](./assets/media/image185.png){width="4.402777777777778in"
height="2.422222222222222in"}

Sarà quindi necessario selezionare il check evidenziato in figura e
cliccare poi sul relativo pulsante di conferma

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\Autorizza_integrazione_Passweb_accetta.bmp](./assets/media/image186.png){width="2.623611111111111in"
height="1.3701388888888888in"}

Confermata l'autorizzazione verremo automaticamente riportati indietro
sulla maschera di configurazione dell'Account Passweb dove troveremo ora
i campi **Token** e **Selling Partner ID** correttamente valorizzati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_dati_account_api2.bmp](./assets/media/image187.png){width="5.50625in"
height="3.5in"}

Arrivati a questo punto sarà necessario cliccare sul pulsante
"**Salva**" presente nella parte bassa della maschera in maniera tale da
salvare i parametri inseriti e visualizzare così altre due sezioni,
"**Articoli**" e "**Ordini**" all'interno delle quali poter configurare
in maniera più dettagliata altri aspetti dell'integrazione.

Per maggiori informazioni in merito a ciascuna di queste sezioni si
vedano i successivi capitoli di questo manuale.

I pulsanti presenti nella barra degli strumenti della maschera **"Lista
degli Account Amazon**" consentono, infine, di:

- **Elimina Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_account.bmp](./assets/media/image188.png){width="0.5194444444444445in"
  height="0.15555555555555556in"} )**:** consente di eliminare l'account
  attualmente selezionato in elenco.

- **Sincro Ordini** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sincro_ordini_ebay.bmp](./assets/media/image45.png){width="0.4479166666666667in"
  height="0.15555555555555556in"} ): consente, nel caso in cui l'Account
  selezionato in elenco sia stato configurato per interagire con Amazon
  anche a livello di ordini, di effettuare la sincronizzazione tra le
  due piattaforme importando quini in Passweb eventuali nuovi ordini, e
  relativi clienti, acquisiti direttamente sul marketplace Amazon.

> **ATTENZIONE!** la sincronizzazione tra Passweb e Amazon, con la
> conseguente eventuale importazione di nuovi ordini, **avverrà anche,
> in maniera completamente automatica, a seguito di ogni
> "Sincronizzazione Sito -- Gestionale"** (manuale o schedulata), e/o
> secondo quanto impostato nel Tab "**Schedulazione**" presente nella
> maschera di configurazione del relativo Account
>
> Per maggiori informazioni in merito si veda anche il capitolo
> "*Acquisto articoli su Amazon e sincronizzazione Ordini sul
> gestionale*" di questo manuale.

- **Modifica Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_account.bmp](./assets/media/image189.png){width="0.5652777777777778in"
  height="0.1625in"} )**:** consente accedere, in modifica, alle
  impostazioni di configurazione dell'Account selezionato in elenco.

