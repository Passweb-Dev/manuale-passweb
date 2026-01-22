# GESTIONE ACCOUNT



Una volta effettuato l'accesso alla sezione "**Gestione Account**" verrà
visualizzata la maschera "**Lista degli Account**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\altri_mkt.bmp](./assets/media/image306.png)

contenente l'elenco degli Account relativi alle diverse piattaforme
attualmente collegate e integrate con il sito Ecommerce.

Per ogni Account presente in elenco è indicato:

- Il nome assegnato alla Account in fase di creazione -- campo
  **Descrizione**

- La piattaforma integrata con il sito Ecommerce mediante questo stesso
  Account -- campo "**Marketplace**"

- Se, in relazione all'account in esame, è stato abilitato o meno
  l'invio delle mail relative alle operazioni di pubblicazione articoli
  -- campo "**Invia Email**"

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

- **Elimina Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_account.bmp](./assets/media/image188.png) )**:** consente di eliminare l'account attualmente
  selezionato in elenco

- **Modifica Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_account.bmp](./assets/media/image189.png) )**:** consente accedere alle impostazioni di
  configurazione dell'Account selezionato in elenco.

- **Copia Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_copia_account.bmp](./assets/media/image307.png) )**:** consente copiare l'Account
  attualmente selezionato in elenco.

- **Aggiorna Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiorna_account.bmp](./assets/media/image308.png) )**:** consente di aggiornare l'account
  attualmente selezionato in elenco e tutta la relativa struttura dati

- **Sincro Ordini** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sincro_ordini_ebay.bmp](./assets/media/image45.png) ): consente di effettuare, nel caso in cui l'Account
  selezionato in elenco sia stato configurato per interagire con la
  piattaforma terza anche a livello di ordini, la sincronizzazione tra
  le due piattaforme (es. Passweb / Magento) importando quini in Passweb
  eventuali nuovi ordini acquisiti direttamente sulla piattaforma
  esterna.

> **ATTENZIONE!** la sincronizzazione tra Passweb e la piattaforma
> terza, con la conseguente eventuale importazione di nuovi ordini,
> **avverrà anche, in maniera automatica, a seguito di ogni
> "Sincronizzazione"** (totale o per variati, manuale o schedulata) tra
> il Sito ed il gestionale Passepartout
>
> Per maggiori informazioni in merito si veda anche il capitolo "*Altri
> Marketplace -- Magento / Prestashop -- Gestione Ordini -
> Sincronizzazione*" di questo manuale.

- **Sincro Clienti** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sincro_clienti.bmp](./assets/media/image309.png) ): consente di effettuare, la
  sincronizzazione tra le due piattaforme (es. Passweb / Magento)
  aggiornando con i dati prelevati dalla piattaforma esterna le
  anagrafiche **di tutti i clienti presenti su Passweb a seguito di
  ordini precedentemente importati da questa stessa piattaforma**.

> Ovviamente affinché la procedura funzioni correttamente è necessario
> che l'Account selezionato in elenco sia stato configurato per
> interagire con la piattaforma terza anche a livello di ordini
>
> **ATTENZIONE!** l'operazione di sincronizzazione dei clienti NON
> importa su Passweb, e conseguentemente sul gestionale, nuovi clienti
> dalla piattaforma esterna ma andrà solamente ad aggiornare le
> anagrafiche di tutti quei clienti che sono già presenti in Passweb.
> Eventuali nuovi clienti potranno quindi essere inseriti solo
> contestualmente all'acquisizione del loro primo ordine
>
> **ATTENZIONE!** La procedura lanciata cliccando sul pulsante in esame
> prenderà sempre in considerazione tutti i clienti inseriti su Passweb
> a seguito di ordini acquisiti dalla piattaforma terza per cui potrebbe
> anche impiegare diverso tempo. Si consiglia quindi di effettuare
> questa operazione solo nel momento in cui sia effettivamente
> necessario riallineare tutte le anagrafiche cliente.

- **Aggiungi Account** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_account.bmp](./assets/media/image310.png) )**:** consente di aggiungere e configurare un nuovo
  Account di integrazione

La prima cosa da fare per poter integrare Passweb con una delle
piattaforme gestite sarà dunque quella di cliccare sul pulsante
**"Aggiungi Account"**.

In questo modo verrà infatti visualizzata la maschera "**Dati Account**"
all'interno della quale poter selezionare, tra quelle proposte, la
specifica piattaforma da integrare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\altri_mkt_1.bmp](./assets/media/image311.png)

Una volta effettuata questa scelta e impostati i principali parametri di
configurazione, compariranno poi, dipendentemente dalla specifica
piattaforma che si è deciso di integrare, ulteriori sezioni all'interno
delle quali poter configurare in maniera più dettagliata altri aspetti.

Nello specifico la sezione

- **Metodi di pubblicazione:** disponibile solo per integrazioni con
  Prestashop e Magento

> Consente di decidere come dovranno essere pubblicati gli articoli
> all'interno della piattaforma terza (via API oppure mediante upload di
> appositi file csv)

- **Articoli:** consente di definire il magazzino gestionale da
  utilizzare nell'integrazione in esame.

> Nel caso di integrazioni con Prestashop o Magento consente di
> impostare anche altri parametri da tenere in considerazione in fase di
> pubblicazione articoli sulla piattaforma terza.

- **Marketplace:** disponibile solo per integrazioni con Google Shopping

> Consente di attivare e/o aggiornare la struttura dati dei marketplace
> verso cui dovranno poi essere esportati gli articoli

- **Ordini:** disponibile solo per integrazioni con Prestashop e Magento

> Consente di decidere se l'Account in esame dovrà o meno interagire con
> Passweb anche a livello di ordini

- **Clienti:** disponibile solo per integrazioni con Prestashop e
  Magento

> Consente di decidere se l'Account in esame dovrà o meno interagire con
> Passweb anche a livello di aggiornamento delle anagrafiche clienti

- **Schedulazione:** disponibile solo per integrazioni con Prestashop e
  Magento

> Consente di schedulare le operazioni di sincronizzazione (ordini e
> clienti) tra Passweb e la piattaforma esterna

- **Backup:** disponibile solo per integrazioni con Prestashop e Magento

> Consente, nel momento in cui dovesse essere utilizzata la
> pubblicazione via API, di visualizzare e gestire i backup effettuati
> da Passweb relativamente alle anagrafiche articolo dei prodotti
> presenti sulla piattaforma terza prima della pubblicazione effettuata
> da Passweb stesso

- **Download CSV:** disponibile solo per integrazioni con Prestashop e
  Magento

> Consente di effettuare un download manuale dei file CSV contenti i
> dati articolo che dovranno poi essere uplodati sulla piattaforma terza

**ATTENZIONE! La possibilità di interagire con la piattaforma esterna
anche a livello di ordini / clienti, così come la possibilità di
attivare uno o più marketplace dipende dalla specifica piattaforma con
cui si intende realizzare l'integrazione**

Per maggiori informazioni relativamente ai diversi parametri di
configurazione presenti all'interno delle sezioni sopra indicate si
rimanda a quanto indicato nei successivi capitoli di questo manuale

