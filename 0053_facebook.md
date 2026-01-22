# FACEBOOK



All'interno della sezione "**Facebook Pixel -- Conversion API**" è
possibile attivare il sistema di tracciamento mediante di Facebook, sia
lato client che lato server.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_pixel_facebook.bmp](./assets/media/image200.png){width="5.740277777777778in"
height="3.623611111111111in"}

Nello specifico il campo:

- **Access Token:** consente di inserire il token di accesso generato
  direttamente all'interno del Business Manager di Facebook in fase di
  attivazione delle Conversion API e necessario per poter attivare il
  tracciamento lato server

> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> attivare unicamente il tracciamento lato client (mediante Pixel) il
> campo in questione deve essere lasciato vuoto

- **Pixel ID:** consente di inserire l'id del Pixel di Facebook generato
  direttamente all'interno del Business Manager e indispensabile per
  poter attivare sia il tracciamento lato client che quello lato server

- **Codice di Test:** consente di inserire il "**test_event_code**"
  prelevabile direttamente dal Business Manager di Facebook e
  indispensabile per poter testare il corretto tracciamento degli eventi
  server

> **ATTENZIONE!** il "test_event_code" inserito all'interno di questo
> campo serve unicamente per testare il corretto funzionamento del
> tracciamento lato server e, in ogni caso, deve essere rimosso una
> volta verificato che tutto funzioni come deve
>
> Per maggiori informazioni relativamente a come poter testare il
> tracciamento Facebook lato server e/o client, si veda anche quanto
> indicato nel relativo capitolo di questo manuale ("*Facebook Pixel e
> Conversion API -- Verifica del tracciamento*")

- **Tracciamento Client:** consente, se selezionato, di attivare il
  tracciamento lato client. Ovviamente affinché questo tipo di
  tracciamento possa effettivamente essere attivato sarà necessario aver
  valorizzato in maniera corretta anche il campo "Pixel ID"

> **ATTENZIONE!** Passweb implementa già, in maniera nativa, gli snippet
> di codice necessari per tracciare determinati eventi standard (es.
> PageView, Acquisto, Aggiunta al carrello, Aggiunta alla Wishlist ...)
> per cui una volta selezionato il parametro in esame e inserito il
> Pixel ID all'interno del relativo campo, di base, **non saranno
> necessarie ulteriori azioni** (per maggiori informazioni in merito si
> veda anche quanto indicato all'interno del capitolo *"Facebook Pixel e
> Conversion API -- Tracciamento lato Client Facebook Pixel"* di questo
> manuale)
>
> In ogni caso, potrebbero comunque configurarsi delle situazioni tali
> da rendere necessario il fatto di dover apportare delle
> personalizzazioni al codice di tracciamento. In queste condizioni sarà
> sufficiente inserire lo snippet di tracciamento all'interno del
> successivo campo "Codice di tracciamento" apportando qui tutte le
> modifiche richieste.
>
> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> gestire unicamente il tracciamento lato server (in maniera tale, ad
> esempio, da evitare qualsiasi rischio in merito alla deduplicazione
> degli eventi) il parametro in esame non dovrà mai essere selezionato

- **Codice di tracciamento --** visibile solo dopo aver attivato il
  precedente parametro "Tracciamento Client"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\facebook_codice_di_tracciamento.bmp](./assets/media/image201.png){width="5.636111111111111in"
height="3.4868055555555557in"}

> Consente di impostare manualmente lo snippet di codice necessario per
> attivare il tracciamento lato client di Facebook.
>
> **ATTENZIONE!** Nel caso in cui non ci sia la necessità di
> personalizzare il codice di tracciamento è sufficiente attivare il
> precedente parametro "Tracciamento Client" vuoto il campo "Codice di
> tracciamento"
>
> Nel momento in cui dovesse essere invece necessario apportare delle
> personalizzazioni al codice di tracciamento (ad esempio per poterlo
> utilizzare in maniera corretta assieme ad una piattaforma CMP non
> integrata nativamente in Passweb) sarà sufficiente copiare lo snippet
> di codice direttamente dal proprio account Facebook, incollarlo
> all'interno del campo in oggetto e apportare qui tutte le
> personalizzazioni richieste.
>
> In queste condizioni si consiglia comunque di inserire il proprio
> Pixel ID all'interno del relativo campo Passweb e modificare poi lo
> script di tracciamento inserendo al posto del Pixel ID il seguente
> segnaposto

- **\$PIXEL_ID\$** - sostituito a runtime con quanto inserito
  all'interno del campo Passweb **Pixel ID**

> Inoltre, per poter consentire a Passweb, anche in queste condizioni,
> di inviare a Facebook gli stessi dati che vengono inviati nel momento
> in cui si dovesse gestire tutto in maniera nativa, sarà necessario
> inserire nello snippet di tracciamento, subito dopo il Pixel ID anche
> il seguente segnaposto

- **\$FB_PARAMS\$ -** necessario per consentire a Passweb di inviare a
  Facebook anche tutti i parametri gestiti e collegati allo specifico
  evento tracciato

> In definitiva dunque, posto di aver inserito il Pixel ID all'interno
> del relativo campo Passweb, lo snippet da inserire all'interno del
> campo "Codice di tracciamento" dovrà essere del tipo di quello qui di
> seguito indicato
>
> *\< script \>*
>
> *!function (f, b, e, v, n, t, s) {*
>
> *if (f.fbq) return; n = f.fbq = function () {*
>
> *n.callMethod ?*
>
> *n.callMethod.apply(n, arguments) : n.queue.push(arguments)*
>
> *};*
>
> *if (!f.\_fbq) f.\_fbq = n; n.push = n; n.loaded = !0; n.version =
> \'2.0\';*
>
> *n.queue = \[\]; t = b.createElement(e); t.async = !0;*
>
> *t.src = v; s = b.getElementsByTagName(e)\[0\];*
>
> *s.parentNode.insertBefore(t, s)*
>
> *}(window, document, \'script\',*
>
> *\'https://connect.facebook.net/en_US/fbevents.js\');*
>
> *fbq(\'init\', \'**\$PIXEL_ID\$**\' **\$FB_PARAMS\$**);*
>
> *fbq(\'track\', \'PageView\', {}, { \'eventID\': \'FB_EVENT_ID\' });*
>
> *\</script\>*
>
> *\<!\--\<noscript\>\<img height=\"\"1\"\" width=\"\"1\"\"
> style=\"\"display:none\"\"*
>
> *src=\"\"https://www.facebook.com/tr?id=\$PIXEL_ID\$&ev=PageView&noscript=1&eid=FB_EVENT_ID\"\"*
>
> */\>\</noscript\>\--\>*
>
> *\<!\-- End Meta Pixel Code \--\>*
>
> **ATTENZIONE!** verificare sempre che lo script sopra evidenziato sia
> effettivamente lo stesso presente anche all'interno del backoffice del
> proprio account Facebook

- **Abilita eventi custom:** consente, se selezionato, di attivare il
  tracciamento (lato server e/o client in base alle impostazioni settate
  per i precedenti parametri) dei seguenti eventi personalizzati:

  - SelectItem -- Selezione prodotto

  - ViewItemList -- Visualizzazione elenco prodotti

  - ViewCart -- Visualizzazione carrello

  - RemoveFromCart -- Rimozione dal carrello

  - AddShippingInfo -- Aggiunta informazioni di spedizione

Per maggiori informazioni in merito al sistema di tracciamento messo a
disposizione da facebook si veda anche quanto indicato nel capitolo
"**Facebook Pixel e Conversion API**" di questo manuale.

