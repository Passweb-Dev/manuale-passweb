# IMPLEMENTAZIONE E GESTIONE DELLA CHIAMATA API



Una volta definita e implementata l'interfaccia da utilizzare per lo
scambio di dati tra le due piattaforme, il passo successivo sarà quello
di implementare la chiamata API e gestire la relativa risposta inserendo
nella pagina web i dati richiesti.

In questo senso la prima cosa da fare sarà quella di analizzare la
struttura della chiamata che dovrà effettivamente essere inoltrata al
portale esterno, struttura questa che, come indicato nella relativa
documentazione ( <https://developer.themoviedb.org/reference/find-by-id>
) dovrà essere del tipo

**GET -
https://api.themoviedb.org/3/find/{external_id}?external_source={external_source}**

dove

- **GET** è metodo da utilizzare per la chiamata API

- **https://api.themoviedb.org/3** è il Base Url inserito sul Wizard di
  Passweb in fase di configurazione del portale

- **/find** è il path dell'endpoint cui inviare la richiesta dati

- **{external_id}** è l'id del film inserito dall'utente all'interno del
  form di richiesta dati e che dovrà essere inserito direttamente nel
  url di richiesta come parte dell'endpoint da contattare

- **external_source={external_source}** è un parametro di query string
  da inserire anch'esso nel url di richiesta e da valorizzare con il
  tipo di sorgente esterna indicata dall'utente in fase di
  configurazione del form

Ora, sulla base di quanto indicato nei precedenti capitoli di questo
manuale, per consentire a Passweb di inoltrare al portale esterno una
chiamata in GET di questo tipo, dovremo utilizzare, inserendola ad
esempio nel Layout di pagina (sezione Javascript), una funzione analoga
a quella di seguito indicata

*function testPortale(id,extSrc){*

*\$.ajax({*

*type: \"POST\",*

***url: \"/effettuaChiamataPortale\"**,*

*data:JSON.stringify({*

*\_**portalID**: \"IMDB\",*

*\_**path**:\"/find/\" + id,*

***\_method**: \"GET\",*

***\_queryString**: { external_source: extSrc },*

*}),*

*contentType: \"application/json\",*

*dataType: \"json\",*

*error: function(error) {*

*console.log(\'error\');*

*},*

*success: function (data) {*

*var risposta = JSON.parse(data.response);*

*renderRisultati(risposta)*

*console.log(risposta);*

*}*

*});*

*}*

Tale funzione accetta in ingresso due parametri (id e extSrc) che
dovranno essere i valori inseriti dall'utente in fase di compilazione
del form di richiesta dati ed effettua una chiamata AJAX in POST all'
url ***\"/effettuaChiamataPortale"*** passandogli i seguenti parametri

- *\_**portalID**: \"IMDB\"* -- È il valore inserito, in fase di
  configurazione del portale, in corrispondenza del campo
  "**Identificativo**"

- *\_**path**:\"/find/\" + id --* È il path dello specifico endpoint cui
  inoltrare la richiesta costruito come somma delle stringhe "/find" +
  id del film inserito dall'utente in fase di compilazione del form.

- ***\_method**: \"GET\"* -- È il metodo che Passweb dovrà utilizzare
  per effettuare la chiamata API al portale esterno

- ***\_queryString**: { external_source: extSrc } --* È il parametro di
  query string da inerire nel url di richiesta valorizzato con la
  sorgente indicata dall'utente in fase di compilazione del form di
  richiesta dati

Nel momento in cui la chiamata API dovesse dare esito positivo
(*success*) verrà invocata la funzione *renderRisultati(risposta)*
passandogli come parametro l'oggetto contenente i dati ottenuti dal
portale esterno

Per completare il processo e visualizzare all'interno della pagina web i
dati richiesti dall'utente dovremo quindi:

- Impostare la logica necessaria per prelevare dal form di richiesta
  dati le informazioni inserite dall'utente e passarle come parametri
  alla funzione *testPortale(id,extSrc)* appena analizzata

- Implementare la funzione *renderRisultati(response)* che dovrà
  occuparsi di analizzare i dati presenti nell'oggetto che gli viene
  passato come parametro e inserirli poi all'interno della pagina web in
  maniera tale che l'utente possa visualizzarli

Per il primo punto potremmo inserire, sempre nel layout di pagina
(sezione Javascript) il seguente snippet di codice

*/\*\* Gestione Form \*/*

*\$(document).ready(function() {*

*\$(\"#avviaRicerca\").on(\"click\", function(e) {*

*e.preventDefault(); // evita che il form faccia il submit tradizionale*

*// recuperiamo i valori dai campi del form*

*var id = \$(\"#inputIdMovie\").val().trim();*

*var extSrc = \$(\"#selectExtSrc\").val();*

*// chiamiamo la funzione testPortale () passandogli come parametri i
valori recuperati dal form*

*testPortale(id, extSrc);*

*});*

*});*

Per quel che riguarda invece la funzione *renderRisultati(response)* che
come detto deve occuparsi di analizzare i dati presenti nell'oggetto che
gli viene passato come parametro e inserirli poi all'interno della
pagina web, potremo pensare di inserire, sempre nel layout di pagina, il
seguente codice

*function renderRisultati(response) {*

*// svuotiamo il div che dovrà contenere i risultati della richiesta*

*\$(\"#risultatiTMDB\").empty();*

*// controlliamo se nell'oggetto passato alla funzione ci sono dei
risultati e in caso positivo costruiamo l'html con i dati richiesti
prelevati da questo oggetto*

*if (response.movie_results && response.movie_results.length \> 0) {*

*response.movie_results.forEach(function(movie) {*

*var html = \`*

*\<div class=\"movie-card\"\>*

*\<h2\>\${movie.title} (\${movie.release_date})\</h2\>*

*\<img src=\"https://image.tmdb.org/t/p/w200\${movie.poster_path}\"*

*alt=\"\${movie.title}\"\>*

*\<p\>\<strong\>Titolo originale:\</strong\>
\${movie.original_title}\</p\>*

*\<p\>\<strong\>Lingua:\</strong\> \${movie.original_language}\</p\>*

*\<p\>\<strong\>Voto medio:\</strong\> \${movie.vote_average}
(\${movie.vote_count} voti)\</p\>*

*\<p\>\${movie.overview}\</p\>*

*\</div\>*

*\`;*

*// inseriamo l'html con i dati richiesti nella div corrispondente
all'interno della pagina web*

*\$(\"#risultatiTMDB\").append(html);*

*});*

*} else {*

*\$(\"#risultatiTMDB\").html(\"\<p\>Nessun risultato trovato.\</p\>\");*

*}*

*}*

In questo modo cliccando sul pulsante "Cerca" verrà eseguita la funzione
*testPortale* che consentirà a Passweb di effettuare la chiamata API al
portale esterno utilizzando i dati inseriti dall'utente all'interno del
Form. Una volta ottenuti i dati richiesti, verrà eseguita la funzione
*renderRisultati* che si occuperà di visualizzare i dati richiesti
all'interno della pagina web

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_esempio_utilizzo_5.bmp](./assets/media/image298.png)

**ATTENZIONE!** quanto indicato all'interno di questi capitoli è un
semplice esempio di come poter utilizzare l'integrazione tra Passweb ed
un portale esterno che espone endpoint interrogabili mediante apposite
chiamate API. I parametri di integrazione con il portale, la logica di
gestione delle chiamate API così come quella di gestione e di
visualizzazione dei risultati dovranno, ovviamente, essere implementati
di volta in volta secondo quelle che sono le specifiche esigenze del
caso e secondo quelle che sono le possibilità offerte dal portale con
cui si desidera realizzare l'integrazione
