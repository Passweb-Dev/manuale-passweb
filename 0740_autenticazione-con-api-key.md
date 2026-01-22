# AUTENTICAZIONE CON API KEY



Nel momento in cui si dovesse optare per questo tipo di autenticazione,
i parametri di configurazione del portale dovranno essere quelli di
seguito indicati

![](./assets/media/image295.png)

- **Identificativo:** IMDB (o qualsiasi altra stringa utile a
  identificare il portale).

> Il valore indicato in questo campo dovrà poi essere utilizzato come
> valore del parametro **\_portalID** nella chiamata AJAX a
> "/effettuaChimataPortale"

- **Etichetta**: IMDB Movie (o qualsiasi altra stringa utile a
  identificare il portale)

- **Base URL**: https://api.themoviedb.org/3

> Il valore del Base Url può essere ricavato consultando gli esempi di
> chiamate API nella documentazione presente al seguente indirizzo
> <https://developer.themoviedb.org/reference/getting-started>
>
> Facendo riferimento, ad esempio, alla chiamata che ritorna i dettagli
> di un film dato un determinato id esterno documentata al seguente
> indirizzo <https://developer.themoviedb.org/reference/find-by-id> e
> del tipo
>
> https://api.themoviedb.org/3/find/tt5950044?external_source=imdb_id
>
> avremo che:

- **https://api.themoviedb.org/3** è il Base Url (da inserire in fase di
  configurazione del portale)

- **/find/** è il path dello specifico endpoint da contattare per
  ottenere le informazioni richieste e che dovrà quindi essere
  utilizzato come valore del parametro **\_path** nella chiamata AJAX a
  "/effettuaChimataPortale"

- **tt5950044** è il valore dell'id del film per cui si richiedono le
  informazioni

> Questo valore dovrà essere richiesto all'utente mediante un apposito
> form e dovrà poi essere utilizzato per costruire l'url completo della
> chiamata API

- **external_source** è un parametro di query string con valore
  **imdb_id**

> Questo parametro ed il relativo valore dovranno essere utilizzati come
> valori del parametro **\_queryString** nella chiamata AJAX a
> "/effettuaChimataPortale"

- **Tipologia di Autenticazione:** Api Key

- **Api Key:** valore indicato in corrispondenza del campo "Api Key"
  presente, come già detto, alla pagina "Impostazioni -- API" del
  proprio account sul portale terzo

- **Aggiungi a:** Query String

- **Nome Campo Query String:** api_key -- essendo proprio questo, come
  indicato al seguente indirizzo
  <https://developer.themoviedb.org/docs/authentication-application>, il
  nome del parametro da utilizzare in query string per la gestione della
  chiave api di autenticazione

