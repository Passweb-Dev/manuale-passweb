# GESTIONE DELLE CHIAMATE



Come indicato nei precedenti capitoli di questo manuale una volta
completata l'integrazione con un determinato portale, per effettuare le
chiamate agli endpoint da esso esposti sarà necessario utilizzare gli
strumenti di editing avanzato messi a disposizione da Passweb (Layout di
pagina o Componente HTML) per effettuare chiamate Ajax in POST all'url

**/effettuaChiamataPortale**

indicando anche i seguenti parametri:

- **\_portalID -- obbligatorio**: identificativo del portale cui dovrà
  essere indirizzata la chiamata API.

> E' il valore inserito, in fase di configurazione del portale, in
> corrispondenza del campo "**Identificativo**" (per maggiori
> informazioni in merito si veda quanto indicato nel precedente capitolo
> di questo manuale)

- **\_path -- obbligatorio**: path dello specifico endpoint cui dovrà
  essere inoltrata la chiamata API.

> E' il percorso dell'endpoint da chiamare al netto del Base Url
> indicato, in fase di configurazione del portale, in corrispondenza
> dell'omonimo campo e al netto anche di eventuali parametri di query
> string

- **\_method -- obbligatorio**: metodo della chiamata API da
  implementare (es. GET, POST ...)

<!-- -->

- **\_queryString -- opzionale**: nel caso in cui la chiamata API
  dovesse utilizzare determinati parametri di query string dovranno
  essere inseriti in corrispondenza di questo parametro con notazione
  {chiave1:valore1,chiave2:valore2 ...}

- **\_body** -- **opzionale**: testo in formato JSON con eventuali
  ulteriori dati da passare nel body della chiamata API al relativo
  endpoint

**ATTENZIONE!** a differenza dei parametri sopra indicati, che
ovviamente potranno variare a seconda dei casi, il parametro url da
passare alla chiamata AJAX dovrà essere sempre e soltanto
**/effettuaChiamataPortale.**

Nel momento in cui l'url indicato non dovesse essere questo, le chiamate
API non potranno essere inoltrate da Passweb allo specifico portale

Relativamente al formato dei risultati ritornati occorre tenere presente
che **la chiamata a "/effettuaChiamataPortale" restituisce sempre un
oggett**o formato da:

- **status**: codice di stato. Campo numerico. Il valore del campo è 500
  se si è verificato un errore, 200 se la chiamata è stata effettuata
  correttamente

- **response**: campo stringa. Se il codice di stato è 500, questo campo
  contiene il dettaglio dell'errore. Se il codice di stato è 200, il
  campo contiene invece il json restituito dalla Web Api in formato
  stringa.

Fatte queste considerazioni di fondamentale importanza e chiariti quelli
che sono i parametri da dover/poter passare dalla chiamata AJAX
effettuata lato client all' url "**/effettuaChiamataPortale**", vediamo
ora un semplice esempio di come poter effettivamente implementare questo
tipo di chiamate.

