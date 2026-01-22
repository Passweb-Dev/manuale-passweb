# INTERFACCIA UTENTE



Una volta configurata l'integrazione tra le due piattaforme, il passo
successivo sarà quello di gestire la logica e l'interfaccia da
utilizzare per lo scambio di dati tra le due piattaforme.

Supponendo dunque di voler implementare la chiamata API documentata
all'indirizzo <https://developer.themoviedb.org/reference/find-by-id>
dovremo costruire un form che possa permettere all'utente di indicare
l'id del film per il quale vuole richiedere delle informazioni e la
sorgente esterna a cui appartiene questo id

In questo senso potremmo quindi utilizzare un componente HTML
all'interno del quale inserire il seguente codice

\<!\-- FORM INSERIMENTO DATI\--\>

*\<h2 class=\"titoloSezione\"\>*

*Ricerca Movie su TMDB*

*\</h2\>*

*\<form id=\"tmdbForm\"\>*

*\<div id=\"wrapperCampiRicerca\" class=\"wrCampiRicerca\"\>*

*\<div class=\"campiAPI\"\>*

*\<div id=\"wrapperIdMovie\"\>*

*\<label class=\"labelTMDB\"\>Id Film\</label\>*

*\<input type=\"text\" id=\"inputIdMovie\" class=\"inputTMDB\"
name=\"inputIdMovie\" placeholderder=\"- Inserisci id Film -\"\>*

*\</div\>*

*\<div id=\"wrapperExtSrc\"\>*

*\<label class=\"labelTMDB\"\>Sorgente Esterna\</label\>*

*\<select class=\"selectTMDB\" id=\"selectExtSrc\" \>*

*\<option value=\"\"\>\</option\>*

*\<option value=\"imdb_id\"\>imdb_id\</option\>*

*\<option value=\"tvdb_id\"\>tvdb_id\</option\>*

*\<option value=\"wikidata_id\"\>wikidata_id\</option\>*

*\<option value=\"youtube_id\"\>youtube_id\</option\>*

*\</select\>*

*\</div\>*

*\</div\>*

*\</div\>*

*\<button id=\"avviaRicerca\"\> Cerca \</button\>*

\</form\>

Oltre al form di inserimento dati dovremo poi gestire anche i risultati
ottenuti dalla chiamata API.

Potremmo quindi pensare di utilizzare un altro componente HTML
all'interno del quale inserire una div che andremo poi a popolare con i
risultati ottenuti dalla chiamata

*\<h2 class=\"titoloSezione\"\>*

*Risultati Ricerca*

*\</h2\>*

*\<div id=\"risultatiTMDB\"\>*

*\</div\>*

In questo modo, al netto di eventuali personalizzazioni grafiche che
potranno essere gestite, ad esempio, dalla sezione CSS del layout di
pagina, otterremo da una parte un form con i due campi che consentono
all'utente di indicare l'id del film per il quale vuole ricevere delle
informazioni e la sorgente esterna da cui è stato prelevato quello
stesso id. Dall'altra parte avremo invece la div con
*id=\"risultatiTMDB",* inizialmente vuota all'interno della quale
dovremo poi inserire e visualizzare le informazioni ottenute a seguito
della chiamata API

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_esempio_utilizzo_4.bmp](./assets/media/image297.png)

