# PARAMETRI ARTICOLO (ITEM)



- **item_id**: codice articolo

- **quantity**: per gli eventi **add_to_cart**, **remove_from_cart**,
  **add_to_wishlist** verrà valorizzato con l'effettiva quantità con cui
  l'articolo in esame viene effettivamente aggiunto/rimosso dal
  carrello/wishlist. Per gli eventi **begin_checkout** e **purchase**
  verrà valorizzato con l'effettiva quantità dell'articolo in ordine. In
  tutti gli altri eventi ecommerce verrà valorizzato a default con il
  valore 1

- **item_name**: titolo articolo

- **affiliation**: valorizzato solo per l'evento **purchase** con quanto
  inserito in corrispondenza del parametro "**Nome Sito**" (pagina "Sito
  -- Preferenze" del Wizard, tab "SEO"). Per tutti gli altri eventi
  ecommerce il parametro affiliation non è gestito

- **currency**: codice ISO della valuta in uso all' articolo

- **discount**: valore dell'eventuale sconto applicato all'articolo

- **index**: posizione occupata dell'articolo nel corrispondente elenco
  di prodotti

- **item_brand**: brand (marca) dell'articolo. Il valore di questo
  parametro dipende dalle impostazioni settate all'interno del Wizard in
  corrispondenza del campo "**Parametro Brand**" (menu "**Sito --
  Preferenze**", tab "**Tracciamento Dati**", sezione "**Parametri
  personalizzabili Google Analytics**")

> Nello specifico può essere valorizzato con:

- il valore impostato all'interno del gestionale nel campo "**Natura**"
  del relativo articolo

- il valore impostato all'interno del gestionale nel campo "**Categoria
  Statistica**" del relativo articolo

- il valore impostato in uno specifico **Attributo Passweb**

<!-- -->

- **item_category/2/3/4/5**: categorie merceologiche di appartenenza del
  corrispondente prodotto.

> [Esempio]{.underline}:
>
> Nell'ipotesi in cui il prodotto in esame appartenga alla seguente
> struttura gerarchica di categorie merceologiche
>
> **Informatica/Accessori/Apple**
>
> i parametri **item_category** verranno valorizzati come di seguito
> indicato:

- item_category: "Apple",

- item_category2: "Accessori"

- item_category3: "Informatica"

> In queste condizioni quindi i parametri item_category4 e
> item_category5 essendo nulli non verranno passati ad Analytics

- **item_list_id**: parametro non gestito

- **item_list_name**: valorizzato solo per gli eventi **view_item_list**
  e **view_cart** con il nome assegnato in Passweb al componente che
  individua la lista di articoli in cui il prodotto in esame è
  contenuto. Per tutti gli altri eventi ecommerce il parametro
  item_list_name non è gestito (e non verrà quindi passato ad analytics)

- **item_variant**: valorizzato solo per articoli a taglie/colori con il
  valore della relativa taglia/colore. Per articoli semplici il
  parametro item_variant essendo nullo non verrà passato ad Analytics

- **price**: prezzo di acquisto (**ivato**) dell'articolo in esame (al
  netto di eventuali sconti applicati all'articolo stesso)

