# FUNZIONE JAVASCRIPT PER L'APPLICAZIONE DI UN FILTRO ARTICOLI



Nel momento in cui l'esigenza dovesse essere quella di utilizzare il
componente "Catalogo Ecommerce" e/o il componente "Risultati Ricerca
Ecommerce" per visualizzare al loro interno un insieme di articoli
(ovviamente tra quelli gestiti all'interno del sito) di cui si conosce
il codice, sarà possibile utilizzare la funzione javascript

**Site.catalog.ApplyFilterByFields(filterId,elencoCodice,componentsClass,location)**

che di fatto andrà ad applicare uno specifico filtro al/ai componenti
indicati e che richiede i seguenti parametri di input:

- **filterId:** valore intero che non deve coincidere con l'id di un
  eventuale altro filtro. Può essere impostato ad esempio a -1

- **elencoCodice:** elenco dei codici articolo relativi ai prodotti che
  dovranno essere visualizzati all'interno del componente nel formato

> *{codice: \[\'PROD72A\',\'PROD66B\',\'PROD64G\'\]}*
>
> dove:
>
> *\'PROD72A\', \'PROD66B\' ...*sono i codici articolo, separati da ,
> dei prodotti da visualizzare all'interno del componente

- **componentsClass:** classi CSS dei componenti cui dovrà essere
  applicato il filtro di visualizzazione degli articoli nel formato

> *\['classeCss1','classeCss2'...\]*
>
> E' possibile indicare la classe Passweb dei componenti interessati
> (es. '*ecCatalogComp*') oppure una qualsiasi delle classi custom ad
> essi assegnate.
>
> **ATTENZIONE!** si ricorda che gli unici componenti Passweb cui può
> essere applicato un filtro articoli sono il "**Catalogo Ecommerce**"
> (classe '***ecCatalogComp*''**), i "**Risultati Ricerca Ecommerce**"
> (classe '***ecCatalogsearchresultsboxComp***') e i pannelli di
> "**Ricerca Ecommerce**" (classe '***ecCatalogsearchandfilterComp**'*)

- **location - opzionale:** percorso relativo della pagina del sito dove
  si trova il componente cui dovrà essere applicato il filtro di
  visualizzazione dei prodotti.

> **ATTENZIONE!** nel momento in cui si dovesse decidere di utilizzare
> anche il parametro location, una volta eseguita la funzione e
> applicato quindi il corrispondente filtro, sarà necessario poi gestire
> manualmente l'indirizzamento alla relativa pagina
>
> Al contrario nel caso in cui il parametro location non dovesse essere
> utilizzato, una volta eseguita la funzione, il filtro verrà
> automaticamente applicato alla pagina corrente
>
> Ovviamente, affinché il filtro possa funzionare in maniera corretta, è
> indispensabile che nella pagina di destinazione (sia essa quella
> corrente o una pagina diversa) sia effettivamente presente il
> componente o i componenti con la classe indicata in corrispondenza del
> parametro "componentsClass"

**[Esempio:]{.underline}**

Site.catalog.ApplyFilterByFields(-1, *{codice:
\['prod01','prod02'\]}*,\['filtroJS','pannelloREc'\])

Eseguendo questa funzione verrà applicato, nella pagina corrente ai
componenti cui sono state assegnate le classi custom *'filtroJS'* o
*'pannelloREc',* il filtro di visualizzazione relativo ai soli due
prodotti di codice *'prod01'* e *'prod02'*

Nel momento in cui l'esigenza dovesse essere invece quella di resettare
il filtro di visualizzazione attualmente applicato ad uno dei componenti
Passweb che ammettono effettivamente l'applicazione dei filtri articolo,
sarà sufficiente utilizzare la stessa funzione javascript appena
analizzata passando però, in corrispondenza del parametro
'**elencoCodice'**, un array vuoto

*{codice: \[\]}*

**[Esempio:]{.underline}**

Site.catalog.ApplyFilterByFields(-1,
*{codice:\[\]}*,\['filtroJS','pannelloREc'\])

Eseguendo questa funzione verranno resettati i filtri articolo
precedentemente applicati ai componenti cui sono state assegnate le
classi custom *'filtroJS'* o *'pannelloREc'*
