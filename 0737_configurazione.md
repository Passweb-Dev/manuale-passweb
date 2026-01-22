# CONFIGURAZIONE



La sezione "**Portali --** **Configurazione**" del Wizard consente di
configurare e gestire le integrazioni tra il proprio sito Passweb ed un
generico portale esterno che espone endpoint interrogabili mediante
apposite chiamate API.

Effettuando l'accesso a questa sezione verrà quindi visualizzata la
maschera "**Portali**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_configurazione.bmp](./assets/media/image283.png){width="5.856944444444444in"
height="3.571527777777778in"}

contenente l'elenco dei portali attualmente integrati con il proprio
sito Ecommerce. I pulsanti presenti nella barra degli strumenti
consentono rispettivamente di:

- **Elimina Portale (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_portale.bmp](./assets/media/image284.png){width="0.5972222222222222in"
  height="0.18819444444444444in"} **):** consente di eliminare il
  portale attualmente selezionato in elenco

- **Modifica Portale** **(**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_portale.bmp](./assets/media/image285.png){width="0.6430555555555556in"
  height="0.18819444444444444in"} **):** consente di modificare i
  parametri di configurazione necessari per l'integrazione tra Passweb
  ed il portale attualmente selezionato in elenco

- **Aggiungi Portale** **(**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_portale.bmp](./assets/media/image286.png){width="0.675in"
  height="0.1951388888888889in"} **):** consente di configurare
  l'integrazione tra Passweb ed un nuovo portale

Cliccando su quest'ultimo pulsante verrà infatti visualizzata la
maschera "**Nuovo Portale**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_nuovo_portale.bmp](./assets/media/image287.png){width="5.856944444444444in"
height="3.571527777777778in"}

all'interno della quale poter specificare tutti i parametri di
configurazione necessari per attivare la comunicazione tra le due
piattaforme.

In questo senso il parametro:

**Identificativo:** consente di assegnare al portale che si sta
configurando uno specifico id che dovrà poi essere utilizzato anche
nelle chiamate Ajax da effettuare per interrogare i relativi endpoint

**Etichetta:** consente di assegnare al portale che si sta configurando
un'etichetta descrittiva utile per distinguerlo dagli altri portali
presenti in elenco

**Base URL:** consente di indicare il base url ossia l'indirizzo
principale (la "radice") dell'API su cui vengono poi costruite tutte le
chiamate ai vari endpoint.

Generalmente contiene il **protocollo** (es. https), il **domino** (es.
api.example.com) e spesso anche un **prefisso di percorso** (es.
/api/v1/).

Nel momento in cui, ad esempio, le chiamate API da implementare
dovessero essere del tipo

*https://api.example.com/v1/users*

*https://api.example.com/v1/orders*

il Base URL da inserire all'interno del campo in oggetto sarà
***https://api.example.com/v1/*** mentre ***users*** e ***orders***
saranno i due diversi endpoint da interrogare da interrogare.

**Tipologia di autenticazione**: consente di indicare, selezionandola
dal relativo menu a tendina, la specifica tipologia di autenticazione da
utilizzare per abilitare la comunicazione tra le due piattaforme
(ovviamente la scelta dipenderà dalle possibilità offerte dalla
piattaforma con cui si deve effettuare l'integrazione)

È possibile selezionare una delle seguenti opzioni:

- **No Authentication:** in questo caso la comunicazione tra le due
  piattaforme avverrà senza alcun meccanismo di autenticazione (opzione
  ovviamente più semplice ma meno sicura)

- **Basic Authentication:** selezionando questa opzione la comunicazione
  tra le due piattaforme avverrà utilizzando il meccanismo della "Basic
  Authentication". È il meccanismo più semplice di autenticazione http
  in cui vengono richiesti una username ed una password codificate poi
  in base64 ed inserite nell'header "Authorization" della richiesta
  inviata ai vari endpoint.

> In queste condizioni, in fase di configurazione del portale, sarà
> quindi necessario indicare anche i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_basic_authentication.bmp](./assets/media/image288.png){width="5.856944444444444in"
height="3.571527777777778in"}

- **Username**: username di accesso all' account abilitato all'utilizzo
  delle API. Spesso coincide con il client_id

- **Password**: password di accesso all' account abilitato all'utilizzo
  delle API. Spesso coincide con il cosiddetto client_secret

> Generalmente questo tipo di autenticazione non prevede scadenza delle
> credenziali e, ovviamente, nel momento in cui un utente
> malintenzionato dovesse intercettare l'header della richiesta potrebbe
> risalire alla credenziali utilizzate per l'autenticazione ai servizi
> API sul portale esterno. In conseguenza di ciò il consiglio, prima di
> utilizzare questo tipo di autenticazione, è sempre quello di
> verificare quanto meno che la comunicazione tra le due piattaforme
> avvenga in HTTPS

- **Authentication with Token:** selezionando questa opzione la
  comunicazione tra le due piattaforme avverrà utilizzando un token di
  autorizzazione (al posto di username e password della Basic
  Authentication) che dovrà poi essere inserito direttamente nell'
  Authorization header delle chiamate

> In queste condizioni, in fase di configurazione del portale, sarà
> quindi necessario indicare anche i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_token_authentication.bmp](./assets/media/image289.png){width="5.856944444444444in"
height="3.571527777777778in"}

- **Bearer Token**: token di autorizzazione per le chiamate API generato
  sulla piattaforma terza

> **ATTENZIONE!** il token inserito in corrispondenza di questo campo
> verrà memorizzato nel database di Passweb e verrà utilizzato
> unicamente nelle chiamate server to server tra le due piattaforme per
> ottenere i dati richiesti

- **API Key:** selezionando questa opzione la comunicazione tra le due
  piattaforme avverrà utilizzando un meccanismo di autenticazione basato
  su di un API Key da generare sulla piattaforma terza, che tipicamente
  serve alla piattaforma stessa per identificare da chi arrivano le
  varie chiamate e che, lato Passweb, potrà essere inserita o in query
  string o in uno specifico header delle richieste che verranno poi
  inviate al portale in questione

> In queste condizioni, in fase di configurazione del portale, andranno
> quindi specificati anche i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_api_key_authentication.bmp](./assets/media/image290.png){width="5.856944444444444in"
height="3.571527777777778in"}

- **API Key**: consente di indicare la chiave API, da generare sulla
  piattaforma terza, che dovrà poi essere utilizzata per consentire la
  comunicazione tra le due piattaforme.

- **Aggiungi a**: consente di decidere dove e come dovrà essere
  utilizzata la chiave api indicata in corrispondenza del precedente
  parametro.

> E' possibile selezionare una delle seguenti opzioni:

- **Header**: in questo caso la chiave api verrà inserita in uno
  specifico header delle richieste inviate alla piattaforma terza.

> L'header da utilizzare potrà essere selezionato tra quelli indicati in
> corrispondenza del successivo parametro "**Nome Header**"

- **Query String**: in questo caso la chiave api verrà gestita
  direttamente come parametro di query string nell' url della richiesta
  API inviata alla piattaforma terza.

> Il parametro da utilizzare in query string per gestire questa chiave
> api dovrà essere indicato in corrispondenza del successivo campo
> "**Nome Campo Query String**"
>
> Ovviamente a livello di sicurezza, tra le due opzioni sopra citate, è
> sempre preferibile utilizzare (se la piattaforma terza offre questa
> possibilità) l'inserimento dell' api key in uno specifico header delle
> richieste. Se inserita in query string infatti l' api key potrebbe poi
> comparire nei log dei server, nei browser history, nei referrer
> inviati ad altri siti ... con un elevato rischio di esposizione. Nel
> momento in cui dovesse invece essere passata in un header delle
> richieste (più comune nelle API moderne), l' api key non resterebbe
> salvata in log o history del browser permettendo quindi di rispettare
> meglio le convenzioni di sicurezza (gli header sono pensati proprio
> per metadati come le credenziali).
>
> In generale occorre comunque evidenziare che l' api key generalmente è
> una stringa statica, che non scade automaticamente e che può quindi
> essere usata fintanto che non venga rigenerata in maniera manuale.
> Inoltre, come detto, consente di identificare l'app o l'utente che
> effettua la chiamata ma, di solito, a differenza di meccanismi di
> autenticazione più sicuri come OAuth2 non gestisce ruoli complessi o
> permessi granulari

- **OAuth2:** selezionando questa opzione la comunicazione tra le due
  piattaforme avverrà utilizzando lo standard OAuth2, un protocollo che
  definisce un insieme di flussi per ottenere token in modo sicuro e
  regolamentato.

> In sostanza OAuth2 è uno standard che utilizza comunque dei token ma
> stabilisce anche dove chiedere il token di autenticazione, quali
> parametri inviare (grant_type, client_id, scope, ecc.), come gestirne
> la scadenza e come poterlo rinnovare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_oauth2_client_credentials.bmp](./assets/media/image291.png){width="5.856944444444444in"
height="3.571527777777778in"}

> Dal punto di vista implementativo supporta diversi scenari
> (grant_type) che, lato Passweb, possono essere specificati in
> corrispondenza del parametro "**Tipo OAuth2**".
>
> In questo senso è possibile selezionare una delle seguenti opzioni:

- **Client Credentials**: nello standard OAuth2 il flusso "Client
  Credentials" (generalmente il più semplice da implementare) prevede di
  effettuare una chiamata POST ad un Authorization Server passandogli
  determinati parametri necessari per consentirgli di validare la
  chiamata in ingresso.

> In queste condizioni, in fase di configurazione del portale, andranno
> quindi specificati anche i seguenti parametri:

- **Client Id:** generalmente è l'id dell'applicazione realizzata sulla
  piattaforma terza per gestire questo tipo di integrazione

- **Client Secret:** generalmente è la password dell'applicazione
  realizzata sulla piattaforma terza per gestire questo tipo di
  integrazione

- **Access Token Url:** url del Authorization Server cui verrà inviata
  la richiesta per ottenere l'Access Token

- **Scope di utilizzo del token:** elenco degli scope/permessi per cui
  dovrà essere generato l'Access Token e su cui l'Access Token potrà poi
  effettivamente essere utilizzato.

> **ATTENZIONE!** gli scope/permessi da inserire in questo campo
> potranno variare (anche come notazione) in relazione alla specifica
> piattaforma con cui si deve realizzare l'integrazione. Devono quindi
> essere reperiti direttamente sulla documentazione fornita dalla
> piattaforma terza e, nel momento in cui dovesse essere necessario
> gestire più di uno scope/permesso, questi dovranno essere separati da
> uno spazio
>
> Nel momento in cui l'Authorization Server dovesse validare in maniera
> corretta, sulla base dei parametri ricevuti, la chiamata che gli è
> stata inoltrata, risponderà a sua volta inviando, tipicamente in
> formato JSON, un Access Token (assieme ad altre informazioni),
> generalmente privo di scadenza, che sarà poi quello da utilizzare per
> effettuare le chiamate ai vari endpoint che, a questo punto, potranno
> a loro volta restituire i dati richiesti.
>
> Ovviamente l'Access Token restituito dalla piattaforma terza verrà
> memorizzato nel database di Passweb e verrà utilizzato unicamente
> nelle chiamate server to server tra le due piattaforme per ottenere i
> dati richiesti
>
> Non sarà quindi in alcun modo visibile all'interno del Wizard ne tanto
> meno dovrà essere utilizzato nelle chiamate AJAX effettuate lato
> client.
>
> Dal punto di vista della sicurezza va considerato che un Access Token
> privo di scadenza è ovviamente meno sicuro di uno con validità
> limitata nel tempo e che dovrà quindi essere periodicamente rigenerato
> (come avviene nel flusso di OAuth2 con Refresh Token)

- **Password**: nello standard OAuth2 il flusso "Password" è un flusso
  ormai poco usato perché meno sicuro ma ancora supportato da diversi
  servizi. La logica di base è la stessa del flusso "Client
  Credentials", la minor sicurezza deriva dal fatto che in questo caso
  per poter ottenere l' Access Token è necessario disporre non solo del
  Client Id e del Client Secret, che tipicamente sono legati ad
  un'applicazione creata sulla piattaforma terza, ma anche Username e
  Password che sono legati invece proprio all'account dell'Utente su
  questa stessa piattaforma.

> In queste condizioni, in fase di configurazione del portale, andranno
> quindi specificati i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_oauth2_password.bmp](./assets/media/image292.png){width="5.856944444444444in"
height="3.571527777777778in"}

- **Username:** generalmente è lo username dell'account utente sulla
  piattaforma terza

- **Password:** generalmente è la password dell'account utente sulla
  piattaforma terza

- **Client Id:** generalmente è l'id dell'applicazione realizzata sulla
  piattaforma terza per gestire questo tipo di integrazione

- **Client Secret:** generalmente è la password dell'applicazione
  realizzata sulla piattaforma terza per gestire questo tipo di
  integrazione

- **Access Token Url:** url del Authorization Server cui verrà inviata
  la richiesta per ottenere l'Access Token

- **Scope di utilizzo del token:** elenco degli scope/permessi per cui
  dovrà essere generato l'Access Token e su cui l'Access Token potrà poi
  effettivamente essere utilizzato.

> **ATTENZIONE!** gli scope/permessi da inserire in questo campo
> potranno variare (come notazione) in relazione alla specifica
> piattaforma con cui si deve realizzare l'integrazione. Devono quindi
> essere reperiti direttamente sulla documentazione fornita dalla
> piattaforma terza e, nel momento in cui dovesse essere necessario
> gestire più di uno scope/permesso, questi dovranno essere separati da
> uno spazio
>
> Anche in questo caso l'Access Token (solitamente privo di scadenza)
> restituito dalla piattaforma terza verrà memorizzato nel database di
> Passweb e verrà utilizzato unicamente nelle chiamate server to server
> tra le due piattaforme per ottenere i dati richiesti

- **Refresh Token:** diversamente dai flussi "Client Credentials" e
  "Password", nello standard OAuth2 il flusso "Refresh Token" prevede di
  gestire, sostanzialmente, due diversi token: il solito Access Token
  che dovrà essere utilizzato nelle chiamate ai singoli endpoint per
  ottenere i dati richiesti e che, a differenza dei casi precedenti
  questa volta avrà una validità limitata (a seconda del livello di
  sicurezza adottato dalla piattaforma terza, può andare da poche ore a
  diversi giorni) e un Refresh Token che rimarrà valido invece a lungo
  termine (tipicamente anche settimane o mesi) da utilizzare nel momento
  in cui l' Access Token dovesse risultare scaduto per poterne generare
  uno nuovo.

> In queste condizioni, in fase di configurazione del portale, andranno
> quindi specificati i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_oauth2_refresh_token.bmp](./assets/media/image293.png){width="5.856944444444444in"
height="3.571527777777778in"}

- **Client Id:** generalmente è l'id dell'applicazione realizzata sulla
  piattaforma terza per gestire questo tipo di integrazione

- **Client Secret:** generalmente è la password dell'applicazione
  realizzata sulla piattaforma terza per gestire questo tipo di
  integrazione

- **Auth Url:** url della piattaforma terza cui verrà ridiretto l'utente
  in fase di generazione del Refresh Token

- **Access Token Url:** url del Authorization Server cui verrà inviata
  la richiesta per ottenere l'Access Token

- **Scope di utilizzo del token:** elenco degli scope/permessi per cui
  dovrà essere generato l'Access Token e su cui l'Access Token potrà poi
  effettivamente essere utilizzato.

> **ATTENZIONE!** gli scope/permessi da inserire in questo campo
> potranno variare (come notazione) in relazione alla specifica
> piattaforma con cui si deve realizzare l'integrazione. Devono quindi
> essere reperiti direttamente sulla documentazione fornita dalla
> piattaforma terza e, nel momento in cui dovesse essere necessario
> gestire più di uno scope/permesso, questi dovranno essere separati da
> uno spazio
>
> Una volta inseriti i parametri richiesti per avviare la procedura di
> autenticazione sarà necessario, in questo caso, cliccare sul pulsante
> "**Genera Token**" presente nella parte bassa della maschera.
>
> In questo modo infatti l'utente verrà ricondotto all'indirizzo
> specificato in corrispondenza del parametro "**Auth Url**" dove,
> tipicamente, gli verrà mostrata una maschera di login relativa
> all'applicazione creata sulla piattaforma terza per gestire l'accesso
> mediante OAuth2.
>
> Dovrà quindi inserire le credenziali del proprio account e accettare
> l'assegnazione dei permessi richiesti.
>
> A questo punto la piattaforma terza provvederà a rilasciare sia
> l'Access Token che il Refresh Token il quale, come detto, avrà una
> scadenza a lungo termine e potrà quindi essere riutilizzato
> automaticamente, nel momento in cui l'Access Token risulterà scaduto
> per generarne uno nuovo.
>
> **ATTENZIONE!** anche se a lunga durata, il Refresh Token avrà
> comunque una data di scadenza oltre la quale non potrà più essere
> utilizzato per generare nuovi Access Token. In queste condizioni sarà
> quindi necessario effettuare nuovamente la procedura di autenticazione
> mediante il pulsante "**Genera Token**" in maniera tale da poter
> generare un nuovo Refresh Token.
>
> Ovviamente sia il Refresh Token che i vari Access Token verranno
> memorizzati nel database di Passweb e utilizzati unicamente nelle
> chiamate server to server tra le due piattaforme per ottenere i dati
> richiesti

**ATTENZIONE!** indipendentemente dalla tipologia di autenticazione che
si deciderà di adottare, i parametri richiesti (client_id,
client_secret, api key, token ...) così come i token ottenuti in
risposta dai vari Authorization Server, verranno memorizzati nel
database di Passweb, saranno utilizzati unicamente nella chiamata server
to server e, per ragioni di sicurezza, non dovranno mai, ovviamente,
essere inseriti nelle chiamate AJAX effettuate lato client.

