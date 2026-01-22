# CONFIGURAZIONE



In ActiveCampaign è possibile attivare due diverse tipologie di
monitoraggio:

- **Monitoraggio lato client**: consente di tracciare unicamente le
  visite alle pagine del sito. Richiede l'inserimento di un apposito
  snippet di codice e può quindi essere facilmente implementato
  all'interno del proprio sito Passweb

- **Monitoraggio lato client**: consente di tracciare eventi custom.
  Richiede di interagire con le API messe a disposizione da
  ActiveCampaign utilizzato un linguaggio lato server. **NON è
  implementato nativamente in Passweb**

Nel momento in cui l'esigenza dovesse essere quindi quella di attivare
il tracciamento lato client, per monitorare le pagine visitate dagli
utenti del sito e collegare eventuali automazioni a queste visite, sarà
necessario

- Accedere alla pagina "**Sito -- Monitoraggio del sito**" del proprio
  account ActiveCampaign e attivare il relativo switch presente
  all'interno della sezione "Monitoraggio del sito"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_attivazione_monitoraggio_client.bmp](./assets/media/image18.png){width="5.5in"
height="3.4743055555555555in"}

- Inserire l'url del proprio sito (nel formato sitoweb.it, quindi senza
  indicazione del protocollo http/https e senza www) all'interno del
  campo "**Aggiungi URL del sito Web**" presente all'interno della
  sezione "**Whitelist e codice di installazione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_whitelist_monitoraggio.bmp](./assets/media/image19.png){width="5.5in"
height="3.4743055555555555in"}

> Verificare anche il check "**Includi tutte le pagine del sito Web**"
> sia correttamente selezionato. Tale opzione consente infatti di
> mettere in whitelist l'intero sito e di poter quindi tracciare le
> visite ad una qualsiasi pagina.

- Copiare lo snippet di codice presente in corrispondenza del campo
  "**Codice di localizzazione**" ed inserirlo, come indicato, nel piede
  di ogni pagina del sito che si intende tracciare.

> Per far questo è possibile utilizzare un componente HTML all'interno
> del quale inserire il codice prelevato da ActiveCampaign e collegare
> poi questo stesso componente ad ogni pagina del sito oppure, molto più
> semplicemente, è possibile inserire lo snippet di codice in
> corrispondenza del campo "**Code Snippet -- FOOTER**" presente alla
> pagina "**Sito -- Preferenze**" del Wizard (sezione
> "**Integrazioni**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_integrazione_codice_monitoraggio.bmp](./assets/media/image20.png){width="5.5in"
height="3.4479166666666665in"}

> **ATTENZIONE!** come indicato nella relativa documentazione di
> ActiveCampaign **la piattaforma non supporta l'inserimento del codice
> di monitoraggio mediante piattaforme di gestione dei tag (es. Google
> Tag Manager)** per cui tale script deve necessariamente essere
> inserito direttamente sul sito Passweb
>
> Altra considerazione di fondamentale importanza da fare è che, come
> precedentemente evidenziato, il sistema di tracciamento di
> ActiveCampaign è a tutti gli effetti un sistema di profilazione degli
> utenti
>
> In conseguenza di ciò nel momento in cui si dovesse decidere di
> integrarlo sarà necessario, da una parte, fornire nelle Norme sulla
> gestione della privacy e dei cookie, un'informativa adeguata circa
> l'utilizzo di questa piattaforma e dei dati che con essa vengono
> raccolti e, dall'altra parte, verificare di aver gestito in maniera
> corretta la richiesta di consenso preventivo come effettivamente
> previsto dalla normativa GDPR

Per maggiori informazioni relativamente al codice di monitoraggio di
ActiveCampaign si consiglia di fare sempre riferimento alla specifica
documentazione di prodotto (es.
[https://help.activecampaign.com/hc/it/articles/221542267-Una-panoramica-del-Monitoraggio-del-sito](https://help.activecampaign.com/hc/it/articles/221542267-Una-panoramica-del-Monitoraggio-del-sito#01H7DD6NXCQN0MXNCZGNW9H76Y) -
<https://help.activecampaign.com/hc/it/articles/221493708-Come-configurare-il-Monitoraggio-del-sito>
)

