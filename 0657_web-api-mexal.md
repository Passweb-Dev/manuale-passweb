# WEB API MEXAL



Come evidenziato nei precedenti capitoli di questo manuale, volendo, è
possibile abilitare il proprio sito Passweb all'utilizzo delle Web API
Mexal. Per far questo sarà necessario:

- Verificare di aver attivato le relative API all'interno del gestionale
  (richiesta attivazione della suite MDS solo per versioni Mexal
  inferiori alla 2024D)

- Creare un utente gestionale abilitato all'utilizzo delle API e
  appartenente quindi al gruppo "**Servizi Web API**" (solo utenti di
  questo gruppo potranno infatti utilizzare i relativi servizi)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\webApi_1.bmp](./assets/media/image13.png){width="5.090972222222222in"
height="2.967361111111111in"}

Una volta attivato il servizio lato gestionale sarà poi necessario
portarsi sul Wizard del proprio sito Passweb alla pagina
"**Configurazione -- Configurazione Gestionale**" e impostare anche qui
i parametri richiesti all'interno della sezione Web API, parametri
questi che saranno diversi a seconda del fatto che Mexal sia installato
presso la Web Farm Passepartout o in locale presso il cliente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_conf_Mexal_webAPI_locale.bmp](./assets/media/image12.png){width="5.870138888888889in"
height="3.558333333333333in"}

In ogni caso si tratterà comunque di impostare un valore per i seguenti
campi:

- **Login API:** username dell'utente Mexal abilitato all'utilizzo delle
  Web Api

- **Password API:** password dell'utente Mexal abilitato all'utilizzo
  delle Web Api

- **Base Address WebApi -- solo per installazioni locali:** indirizzo
  del server mexal più la porta su cui è in ascolto il servizio Web Api

> I valori necessari per costruire il Base Address possono essere
> ricavati all'interno della maschera gestionale "**Configurazione
> webapi**" ("*Servizi -- Configurazioni -- Configurazione moduli -- Web
> Api*")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\webApi_2.bmp](./assets/media/image14.png){width="3.467361111111111in"
height="1.5326388888888889in"}

> Supponendo dunque che i valori presenti all'interno dei campi
> evidenziati in figura siano rispettivamente mrossi e 9104 il Base
> Address da inserire nel corrispondente campo Passweb sarà esattamente
> il seguente
>
> https://mrossi.passepartout.local:9104

**ATTENZIONE!** In ogni caso per maggiori informazioni relativamente al
Base Address e, più in generale, all'attivazione e all'utilizzo delle
API Mexal si consiglia di fare sempre riferimento alla relativa
documentazione di prodotto

Una volta completata l'attivazione lato gestionale e inseriti anche i
parametri richiesti nella relativa maschera Passweb, per richiamare le
Web Api di Mexal sarà sufficiente utilizzare gli strumenti di editing
avanzato di Passweb (Layout di pagina o Componente HTML) per effettuare
chiamate Ajax in POST al server Mexal richiamando il seguente url

**/callWebApiMexal**

indicando anche i seguenti parametri:

- **\_path**: percorso della Web Api Mexal da richiamare

- **\_method**: metodo della Web Api. I valori ammessi sono GET, POST,
  PUT e DEL (fare riferimento al manuale delle WebAPI).

- **\_body**: parametro opzionale. Testo in formato json con i dati da
  passare alla Web Api

**ATTENZIONE!** Per maggiori informazioni relativamente ai percorsi
delle singole Web Api e/o ai relativi metodi ammessi per le singole
chiamate si consiglia di fare sempre riferimento alla relativa
documentazione di prodotto

Relativamente al formato dei risultati ritornati occorre tenere presente
che **la chiamata a "/callWebApiMexal" restituisce sempre un oggett**o
formato da:

- **status**: codice di stato. Campo numerico. Il valore del campo è 500
  se si è verificato un errore, 200 se la chiamata è stata effettuata
  correttamente

- **response**: Campo stringa. Se il codice di stato è 500, questo campo
  contiene il dettaglio dell'errore. Se il codice di stato è 200, il
  campo contiene invece il json restituito dalla Web Api in formato
  stringa.

- **location**: Campo stringa. In caso di inserimento di una nuova
  entità, in questo campo viene indicato il path dell'entità appena
  creata

Di seguito vengono riportate, a titolo puramente esemplificativo, alcune
possibili chiamate alle Web Api Mexal effettuate utilizzando la libreria
jQuery disponibile nativamente all'interno di ogni sito Passweb

**ESEMPIO -- Lettura dei dati dell\'utente con codice conto 501.00001:**

*\$.ajax({*

*type: \"POST\",*

*url: \"/callWebApiMexal\",*

*data: {*

*\_path: \'/webapi/risorse/clienti/501.00001\',*

*\_method: \'GET\'*

*},*

*dataType: \"json\",*

*error: function (xhr, textStatus, errorThrown) {*

*alert(\'Errore Generico : \' + errorThrown);*

*},*

*success: function (result) {*

*switch(result.status)*

*{*

*case 200:*

*var cliente = JSON.parse(result.response);*

*alert(cliente.codice);*

*break;*

*case 500:*

*alert(\'Errore : \' + result.response);*

*break;*

*}*

*}*

*});*

**ESEMPIO -- Modifica dei dati dell\'articolo con codice
AGLIANICVULSIM03**

*var variazioni = {descrizione: \"Aglianico\"};*

*\$.ajax({*

*type: \"POST\",*

*url: \"/callWebApiMexal\",*

*data: {*

*\_path: \'/webapi/risorse/articoli/AGLIANICVULSIM03\',*

*\_method: \'PUT\',*

*\_body: JSON.stringify(variazioni)*

*},*

*dataType: \"json\",*

*error: function (xhr, textStatus, errorThrown) {*

*alert(\'Errore Generico : \' + errorThrown);*

*},*

*success: function (result) {*

*switch(result.status)*

*{*

*case 200:*

*alert(\'Modifica effettuata\');*

*break;*

*case 500:*

*alert(\'Errore : \' + result.response);*

*break;*

*}*

*}*

*});*

**ESEMPIO -- Creazione di un nuovo cliente con codifica automatica**

*var cliente = {*

*codice: \"501.AUTO\",*

*ragione_sociale:\"cliente 2 webapi REST\",*

*tp_nazionalita: \"I\",*

*cod_listino:2,*

*valuta:1*

*};*

*\$.ajax({*

*type: \"POST\",*

*url: \"/callWebApiMexal\",*

*data: {*

*\_path: \'/webapi/risorse/clienti\',*

*\_method: \'POST\',*

*\_body: JSON.stringify(cliente)*

*},*

*dataType: \"json\",*

*error: function (xhr, textStatus, errorThrown) {*

*alert(\'Errore Generico : \' + errorThrown);*

*},*

*success: function (result) {*

*switch(result.status)*

*{*

*case 200:*

*alert(\'Inserimento effettuato: \' + result.location);*

*break;*

*case 500:*

*alert(\'Errore : \' + result.response);*

*break;*

*}*

*}*

*});*

**ATTENZIONE! nell'header "Coordinate-Gestionale" che viene impostato in
automatico da Passweb per fare la richiesta alle Web API non viene
gestito il parametro "Magazzino".**

Si ricorda inoltre che le Web Api Mexal, se correttamente configurate,
verranno utilizzate anche:

- per eliminare automaticamente, in fase di sincronizzazione, eventuali
  documenti presenti su Passweb ma non più nel gestionale (perché ad
  esempio oggetto di fusione, di trasformazioni da preventivi ad ordine
  ...). Per maggiori informazioni in merito si veda anche quanto
  indicato all'interno del capitolo "*Ordini -- Ordini -- eliminazione
  automatica di documenti non più presenti a gestionale*" di questo
  manuale

- per abilitare la ricerca tra i documenti Docuvision presenti in area
  riservata. Per maggiori informazioni in merito si veda anche quanto
  indicato all'interno del capitolo "*Siti Ecommerce -- Area Riservata e
  B2B*" di questo manuale

