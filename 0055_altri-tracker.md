# ALTRI TRACKER



All'interno di questa sezione è possibile **abilitare il tracciamento di
determinati dati Ecommerce con strumenti di terze parti diversi da
Google Analytics e/o Google Tag Manager.**

Come visto nei precedenti capitoli di questo manuale grazie
all'integrazione nativa tra Passweb e Google Analytics è possibile
utilizzare questo specifico strumento di tracciamento in maniera molto
semplice inserendo la Chiave di Monitoraggio nell'apposito campo e
selezionando determinati parametri come ad esempio quelli relativi alla
gestione dei dati dell' Ecommerce Avanzato e/o quello relativo al
tracciamento dei termini di ricerca.

Una volta settati questi semplici parametri l'utente non dovrà, a meno
di specifiche necessità, inserire nessun codice javascript di
tracciamento in quanto sarà Passweb stesso a preoccuparsi di inserire il
codice corretto nelle apposite pagine, di valorizzare correttamente
tutte le variabili richieste da Google Analytics e di inviare ad
Analytics stesso tutti i dati corretti.

**ATTENZIONE!** Per maggiori informazioni in merito a Google Analytics
si consiglia di consultare la relativa sezione di questo manuale
(*Google Analytics*) e soprattutto la relativa documentazione presente
in rete e direttamente raggiungibile anche dall'interno della
piattaforma stessa

Un discorso del tutto analogo vale anche per l'integrazione nativa tra
Passweb e Google tag Manager (GTM). Anche in questo caso infatti
l'utente dovrà semplicemente preoccuparsi di inserire nell'apposito
campo lo snippet di codice fornito direttamente da GTM. Sarà poi Passweb
a preoccuparsi di creare e popolare in maniera opportuna la variabile
**dataLayer** richiesta da GTM per effettuare lo specifico tracciamento
impostato, e di inviare i relativi dati al sistema di tracciamento.

In realtà essendo GTM un sistema di tracciamento più generalista
rispetto a Google Analytics, in queste condizioni la configurazione
potrebbe essere un po' più complessa dipendentemente dal tipo di
risultato che si vuole raggiungere ma, in ogni caso, si tratta sempre di
configurazioni da effettuare direttamente sull'interfaccia web di GTM.

**ATTENZIONE!** Per maggiori informazioni relativamente alla
configurazione e all'utilizzo di Google Tag manager si veda anche la
relativa sezione di questo manuale (Google Tag Manager) e soprattutto la
relativa documentazione presente disponibile in rete

Nel caso in cui, invece, l'esigenza dovesse essere quella di tracciare
determinate informazioni Ecommerce, come ad esempio l'impressione dei
prodotti piuttosto che la visita di una scheda prodotto o
l'aggiunta/rimozione di articoli in carrello utilizzando uno strumento
di tracciamento diverso da Google Analytics e/o da Google Tag Manager
(es. Pixel di Facebook, Trova Prezzi, Zanox ecc...), e quindi non
integrato nativamente in Passweb, l'operazione sarà comunque possibile
ma saranno necessarie specifiche competenze tecniche.

In queste condizioni sarà infatti necessario, per prima cosa,
selezionare il parametro "**Tracciamento dati Ecommerce**" presente
all'interno della sezione "**Altri Tracker**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\altri_tracker.bmp](./assets/media/image205.png){width="5.792361111111111in"
height="3.422222222222222in"}

**Una volta attivato questo parametro, indipendentemente dal fatto di
utilizzare o meno anche GTM, Passweb si occuperà comunque di creare una
variabile dataLayer (che poi è la stessa richiesta da GTM) e di
popolarla in maniera opportuna con tutta una serie di dati Ecommerce
necessari per effettuare diversi tipi di tracciamento**.

**In queste condizioni, inoltre, Passweb metterà a disposizione dello
sviluppatore anche tutta una serie di funzioni javascript native in
grado di analizzare la variabile dataLayer e di prelevare i dati
corretti da inviare poi al sistema di tracciamento**

L'amministratore / sviluppatore del sito dovrà quindi preoccuparsi di:

- Inserire nelle apposite pagine lo snippet di codice (javascript)
  necessario per consentire al sito di inviare i dati di tracciamento
  allo strumento preposto. Questo snippet, generalmente, viene fornito
  direttamente dallo strumento di tracciamento che si intende adottare
  (es. Pixel di Facebook, Trovaprezzi, Zanox ecc...)

- Utilizzare le funzioni javascript messe a disposizione nativamente da
  Passweb per prelevare i dati corretti da inviare poi al sistema di
  tracciamento.

La logica di funzionamento, dunque, è la stessa utilizzata anche da
Google Analytics e/o da Google Tag Manager solo che essendo questi due
strumenti integrati nativamente in Passweb è Passweb stesso che, in
quelle condizioni, che si preoccupa di eseguire quanto indicato ai punti
precedenti sollevando quindi l'amministratore / sviluppatore del sito
dall'incombenza di dover scrivere specifico codice javascript.

Di seguito viene fornito un elenco delle funzioni di callback javascript
utilizzabili in Passweb ai fini dell'integrazione con sistema di
tracciamento di terze parti ed alcuni semplici esempi relativi a come
poter utilizzare queste stesse funzioni.

- **PWT_AddToCart() --** funzione per gestire il tracciamento
  dell'evento "Aggiungi in Carrello"

- **PWT_RemoveFromCart() --** funzione per gestire il tracciamento
  dell'evento "Rimuovi dal Carrello"

- **PWT_ViewDetailProduct() --** funzione per gestire il tracciamento
  della Visualizzazione di una Scheda Prodotto

- **PWT_TransactionPurchase() --** funzione per gestire il tracciamento
  della finalizzazione di un acquisto

- **PWT_StepTransactionPurchase() --** funzione per gestire il
  tracciamento degli steps (inizio, spedizione ...) del checkout.

- **PWT_ViewImpression() --** funzione per gestire il tracciamento della
  vista di un elenco di prodotti

- **PWT_ViewCart() --** funzione per gestire il tracciamento del
  carrello

- **PWT_ClickProduct() --** funzione per gestire il tracciamento
  dell'evento di click su di un prodotto

- **PWT_SearchTerms()** **--** funzione per gestire il tracciamento dei
  termini di ricerca

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELL'EVENTO DI AGGIUNTA IN CARRELLO

Per gestire il tracciamento dell'evento di rimozione articoli dal
carrello verso un sistema di terze parti (diverso da Google Analytics) è
possibile utilizzare la seguente funzione di callback javascript:

function **PWT_AddToCart(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **product** - \>                                

                          id                      Identificativo prodotto
                                                  Passweb

                          code                    Codice prodotto
                                                  Gestionale

                          name                    Titolo prodotto

                          brand                   Marca prodotto

                          category                Categoria merceologica
                                                  prodotto

                          variant                 Variante prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          quantity                Quantità del prodotto

                          coupon                  Voucher associato al
                                                  prodotto

                          position                Posizione del prodotto

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE**! La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

Di seguito viene fornito un esempio di utilizzo della funzione in
oggetto in relazione al tracciamento mediante Pixel di Facebook:

function PWT_AddToCart(result){

fbq(\'track\', \'AddToCart\', {

currency:result.currency,

content_type:\'product\',

contents: \[

{

> id: result.product.id,
>
> quantity: result.product.quantity,
>
> item_price: result.product.price

}

\],

});

}

**ATTENZIONE!** Nel caso in cui si decida di utilizzare un componente
HTML la funzione in oggetto andrà racchiusa all'interno di un apposito
tag \< script \>

**ATTENZIONE!** Per implementare correttamente il tracciamento dei dati
con il Pixel di Facebook la funzione sopra indicata da sola non è
sufficiente. Occorre inserire anche lo snippet di codice necessario per
consentire al sito di inviare correttamente i dati di tracciamento. Per
maggiori informazioni in merito si rimanda alla specifica documentazione
presente su facebook (
<https://www.facebook.com/business/help/952192354843755> )

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELL'EVENTO RIMUOVI DAL CARRELLO

Per gestire il tracciamento dell'evento di aggiunta in carrello verso un
sistema di terze parti (diverso da Google Analytics) è possibile
utilizzare la seguente funzione di callback javascript:

function **PWT_RemoveFromCart(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **product** - \>                                

                          id                      Identificativo prodotto
                                                  Passweb

                          code                    Codice prodotto
                                                  Gestionale

                          name                    Titolo prodotto

                          brand                   Marca prodotto

                          category                Categoria merceologica
                                                  prodotto

                          variant                 Variante prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          quantity                Quantità del prodotto

                          coupon                  Voucher associato al
                                                  prodotto

                          position                Posizione del prodotto

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE**! La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELLA VISUALIZZAZIONE DI UNA SCHEDA PRODOTTO

Per gestire il tracciamento della visualizzazione di una scheda prodotto
verso un sistema di terze parti (diverso da Google Analytics) è
possibile utilizzare la seguente funzione di callback javascript:

function **PWT_ViewDetailProduct(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **product** - \>                                

                          id                      Identificativo prodotto
                                                  Passweb

                          code                    Codice prodotto
                                                  Gestionale

                          name                    Titolo prodotto

                          category                Categoria merceologica
                                                  prodotto

                          variant                 Variante prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          priceText               Prezzo testuale del
                                                  prodotto

                          quantity                Quantità del prodotto,
                                                  di default 1

                          currency                Codice ISO della valuta

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELLA FINALIZZAZIONE DI UN ACQUISTO

Per gestire il tracciamento della finalizzazione di un acquisto verso un
sistema di terze parti (diverso da Google Analytics) è possibile
utilizzare la seguente funzione di callback javascript:

function **PWT_TransactionPurchase(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------- ----------------- ----------------- ------------------
  **purchase** - \>                                     

                    **actionField**                     
                    **-\>**                             

                                      id                Identificativo
                                                        Ordine

                                      affiliation       Nome del sito

                                      revenue           Totale numerico
                                                        dell'Ordine

                                      shipping          Totale numero
                                                        delle spese di
                                                        spedizione
                                                        dell'Ordine

                                      tax               Totale numero
                                                        delle tasse
                                                        dell'Ordine

                                      coupon            Codice del voucher
                                                        utilizzato
                                                        nell'Ordine

                                      costumerId        Identificativo
                                                        Utente dell'Ordine

                                      email             Email Utente
                                                        dell'Ordine

                    **products** \[                     
                    \] **-\>**                          

                                      id                Identificativo
                                                        prodotto Passweb

                                      code              Codice prodotto
                                                        Gestionale

                                      name              Titolo prodotto

                                      category          Categoria
                                                        merceologica
                                                        prodotto

                                      price             Prezzo numerico
                                                        del prodotto

                                      quantity          Quantità del
                                                        prodotto

                                      variant           Variante prodotto

  **currency**                                          Codice ISO della
                                                        valuta

  **lang**                                              Codice ISO della
                                                        lingua del sito
  ----------------- ----------------- ----------------- ------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DEGLI STEPS (INIZIO, SPEDIZIONE ...) DEL CHECKOUT.

Per gestire il tracciamento degli step del checkout verso un sistema di
terze parti (diverso da Google Analytics) è possibile utilizzare la
seguente funzione di callback javascript:

function **PWT_StepTransactionPurchase(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------- ----------------- ----------------- ------------------
  **stepName**                                          Nome dello Step

  **checkout** **-                                      
  \>**                                                  

                    **actionField**                     
                    **-\>**                             

                                      step              Numero dello Step

                                      option            Valore indicato
                                                        nello Step

                    **products** \[                     
                    \] **-\>**                          

                                      id                Identificativo
                                                        prodotto Passweb

                                      code              Codice prodotto
                                                        Gestionale

                                      name              Titolo prodotto

                                      category          Categoria
                                                        merceologica
                                                        prodotto

                                      price             Prezzo numerico
                                                        del prodotto

                                      quantity          Quantità del
                                                        prodotto

                                      variant           Variante prodotto

                                      currency          Codice ISO della
                                                        valuta

  **currency**                                          Codice ISO della
                                                        valuta

  **lang**                                              Codice ISO della
                                                        lingua del sito
  ----------------- ----------------- ----------------- ------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELLA VISTA DI UN ELENCO DI PRODOTTI

Per gestire il tracciamento degli step della vista di un elenco di
prodotti verso un sistema di terze parti (diverso da Google Analytics) è
possibile utilizzare la seguente funzione di callback javascript:

function **PWT_ViewImpression(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **listName**                                    Nome della Lista

  **products** \[ \] **-                          
  \>**                                            

                          code                    Codice prodotto
                                                  Gestionale

                          name                    Titolo prodotto

                          category                Categoria merceologica
                                                  prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          quantity                Quantità del prodotto

                          currency                Codice ISO della valuta

                          id                      Identificativo prodotto
                                                  Passweb

                          brand                   Marca del Prodotto

                          position                Posizione del prodotto
                                                  all'interno dell'elenco

                          priceText               Prezzo testuale del
                                                  prodotto

                          lang                    Codice ISO della lingua
                                                  del sito

                          list                    Nome della Lista

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DEL CARRELLO

Per gestire il tracciamento della visualizzazione della pagina Carrello
verso un sistema di terze parti (diverso da Google Analytics) è
possibile utilizzare la seguente funzione di callback javascript:

function **PWT_ViewCart(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **listName**                                    Carrello

  **products** \[ \]                              
  **-\>**                                         

                          code                    Codice prodotto
                                                  Gestionale

                          name                    Titolo prodotto

                          category                Categoria merceologica
                                                  prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          quantity                Quantità del prodotto

                          currency                Codice ISO della valuta

                          id                      Identificativo prodotto
                                                  Passweb

                          brand                   Marca del Prodotto

                          position                Posizione del prodotto
                                                  all'interno dell'elenco

                          priceText               Prezzo testuale del
                                                  prodotto

                          lang                    Codice ISO della lingua
                                                  del sito

                          list                    Nome della Lista

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DELL'EVENTO DI CLICK SU DI UN PRODOTTO

Per gestire il tracciamento dell'evento di click su di un prodotto verso
un sistema di terze parti (diverso da Google Analytics) è possibile
utilizzare la seguente funzione di callback javascript:

function **PWT_ClickProduct(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------- ----------------------- -----------------------
  **product** **-\>**                             

                          code                    Codice prodotto
                                                  Gestionale

                          id                      Identificativo prodotto
                                                  Passweb

                          name                    Titolo prodotto

                          category                Categoria merceologica
                                                  prodotto

                          price                   Prezzo numerico del
                                                  prodotto

                          quantity                Quantità del prodotto

  **currency**                                    Codice ISO della valuta

  **lang**                                        Codice ISO della lingua
                                                  del sito
  ----------------------- ----------------------- -----------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### FUNZIONE PER GESTIRE IL TRACCIAMENTO DEI TERMINI DI RICERCA

Per gestire il tracciamento di un termine di ricerca verso un sistema di
terze parti (diverso da Google Analytics) è possibile utilizzare la
seguente funzione di callback javascript:

function **PWT_SearchTerms(result)**{ }

dove il parametro **result** è un oggetto con la seguente struttura

  ----------------------------------- -----------------------------------
  searchCategory                      Categoria di Ricerca (possibili
                                      valori: Ricerca Testuale, Ricerca
                                      ECommerce, Ricerca Cms)

  searchTerms                         Termini di Ricerca utilizzati

  lang                                Codice ISO della lingua del sito
  ----------------------------------- -----------------------------------

**ATTENZIONE!** La funzione in esame può essere implementata agendo
direttamente dalla sezione Javascript del layout di sito

##### TRACCIAMENTO VERSO TROVAPREZZI

Supponiamo di voler integrare il nostro sito Ecommerce con il sistema di
tracciamento ordini messo a disposizione da trovaprezzi.it.

Dando un'occhiata alla relativa documentazione messa a disposizione da
trovaprezzi.it troveremo immediatamente che le operazioni da eseguire
per abilitare questo tipo di tracciamento sono sostanzialmente due:

- Reperire la propria chiave merchant comunicando a trovaprezzi.it
  l'indirizzo della pagina del sito cui viene ricondotto l'utente dopo
  aver completato un acquisto

> (es. http://www.urlsito.it/store/cart/checkout/success)

- Inserire nella sezione \< head \> della pagina di cui al punto
  precedente il seguente codice di monitoraggio inserendo al posto dei
  parametri indicati tra /\* \*/ il valore della propria chiave merchant
  e ovviamente i dati dell'ordine che si intende tracciare (quindi
  l'email del cliente che ha effettuato l'ordine, i codici dei prodotti
  in ordine, il totale del carrello ecc...)

\<script type=\"text/javascript\"
src=\"https://tracking.trovaprezzi.it/javascripts/tracking.min.js\"
async=\"true\"\>\</script\>

\<script type=\"text/javascript\"\>

> window.\_tt = window.\_tt \|\| \[\];
>
> window.\_tt.push({ event: \"setAccount\", id: **/\* chiavemerchant
> \*/** });
>
> window.\_tt.push({ event: \"setOrderId\", order_id: **/\* idordine
> \*/** });
>
> window.\_tt.push({ event: \"setEmail\", email: **/\* emailcliente
> \*/** });
>
> window.\_tt.push({ event: \"addItem\", sku: **/\* sku \*/**,
> product_name: **/\* nomeprodotto \*/** });
>
> window.\_tt.push({ event: \"setAmount\", amount: **/\* totalecarrello
> \*/** });
>
> window.\_tt.push({ event: \"orderSubmit\"});

\</script\>

Ora per quel che riguarda il secondo punto, il codice di monitoraggio
sopra indicato andrà inserito nella sezione "**Documento**" all'interno
della voce di menu "**Ordini -- Gestione Ordini -- Configurazione
Ordini**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\altri_tracker2.bmp](./assets/media/image206.png){width="5.99375in"
height="3.5256944444444445in"}

Per quel che riguarda lo script, il parametro **/\* chiavemerchant \*/**
andrà sostituito con la chiave fornita da trovaprezzi.it una volta
comunicatogli l'indirizzo della pagina del proprio sito cui viene
ricondotto un utente dopo aver completato l'ordine.

Per le altre variabili, Passweb viene incontro allo sviluppatore
mettendogli a disposizione alcune variabili in grado di popolare
correttamente le variabili da passare allo script di Trovaprezzi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\altri_tracker3.bmp](./assets/media/image207.png){width="4.856944444444444in"
height="2.045138888888889in"}

Nello specifico le variabili sono:

- **\$texts_documentid\$** (Identificativo Passweb) **--** Restituisce
  l'id dell'ordine

- **\$billing_email\$** (Email) **--** Restituisce l'email associata
  all'ordine

- **\$documentItems (CICLO Articoli documento) --** Restituisce un array
  contenente gli articoli dell'ordine. Gli elementi di questo array
  saranno:

  - **Sku --** il codice dell'articolo viene popolato dalla variabile
    **\$it.entryCode\$** (Codice)

  - **product_name --** il nome dell'articolo **\$it.entryTitle\$**
    (Titolo)

- **\$totalamount\$** (Totale documento numerico)**--** Restituisce il
  totale dell'ordine

Tenendo conto di quanto detto, il codice da incollare nella sezione
"Documento", al fine di poter integrare il proprio sito con il sistema
di tracciamento offerto da trovaprezzi.it sarà:

\<script type=\"text/javascript\"
src=\"https://tracking.trovaprezzi.it/javascripts/tracking.min.js\"
async=\"true\"\>\</script\>

\<script type=\"text/javascript\"\>

window.\_tt = window.\_tt \|\| \[\];

window.\_tt.push({ event: \"setAccount\", id: \'CHIAVE MERCHANT\' });

window.\_tt.push({ event: \"setOrderId\", order_id:
\'\$texts_documentid\$\' });

window.\_tt.push({ event: \"setEmail\", email: \'\$billing_email\$\' });

\$documentItems:{

window.\_tt.push({ event: \"addItem\", sku: \'\$it.entryCode\$\',
product_name: \'\$it.entryTitle\$\' });

}\$;

window.\_tt.push({ event: \'setAmount\', amount: \'\$totalamount\$\' });

window.\_tt.push({ event: \"orderSubmit\"});

\</script\>

dove, ovviamente, dovremo preoccuparci soltanto di inserire la nostra
specifica chiave merchant.

##### TRACCIAMENTO VERSO -- ZANOX

Il processo di integrazione tra il proprio sito ed il sistema di
tracciamento Ecommerce messo a disposizione da Zanox
(<http://www.zanox.com/it/>) è sostanzialmente analogo a quello
esaminato nel precedente capitolo e relativo all'integrazione con il
sistema di tracciamento di trovaprezzi.it.

A differenza di trovaprezzi.it che offre la possibilità di tracciare
solo ed esclusivamente i dati relativi agli ordini effettuati
all'interno del sito, la piattaforma Zanox offre invece la possibilità
di monitorare diverse informazioni Ecommerce come ad esempio le ricerche
effettuate all'interno del sito piuttosto che l'aggiunta e la rimozione
di articoli in carrello o ancora la visita delle varie schede prodotto.

Anche in questo caso si tratterà comunque di:

- Reperire, per prima cosa, dalla documentazione messa a disposizione da
  Zanox stesso, lo snippet di codice di monitoraggio che dovrà essere
  inserito nella sezione \< head \> delle varie pagine del sito in
  relazione alla specifica informazione che si intende tracciare.

- Selezionare il parametro "Tracciamento Dati Ecommerce" presente nella
  sezione "Sito -- Preferenze" del Wizard

- Implementare delle funzioni javascript necessarie per analizzare la
  variabile dataLayer creata da Passweb, prelevare da essa i dati
  Ecommerce da monitorare e assicurarsi di inserire questi stessi dati
  nello snippet di codice di monitoraggio in maniera tale che possano
  poi essere inviati correttamente alla piattaforma di tracciamento.

In merito a quest'ultimo punto è bene poi sottolineare come Zanox
richieda necessariamente di creare, valorizzare ed inviare delle
variabili ben precise in relazione alla specifica informazione che si
intende tracciare.

Per inviare informazioni relativamente alle ricerche effettuate
all'interno del sito, ad esempio, sarà necessario utilizzare la
variabile "zx_search_query", mentre per inviare informazioni
relativamente al totale di un ordine sarà necessario utilizzare la
variabile "zx_total_amount".

Come già per trovaprezzi.it, anche nel caso di Zanox, Passweb viene
incontro allo sviluppatore mettendogli a disposizione tutta una serie di
funzioni javascript native in grado di analizzare la variabile dataLayer
prelevando i dati corretti da inviare poi al sistema di tracciamento.

Di seguito viene fornito un elenco delle funzioni javascript
utilizzabili in Passweb ai fini dell'integrazione con il sistema di
tracciamento Ecommerce messo a disposizione da Zanox ed alcuni semplici
esempi relativi a come poter utilizzare queste stesse funzione per
valorizzare le variabili richieste espressamente da questa piattaforma
di monitoraggio:

**TRACCIAMENTO DELLE RICERCHE:**

[Funzioni disponibili]{.underline}

- **PW_Zanox.GetSearchQuery():** Restituisce la query string della
  ricerca

[Esempio di integrazione:]{.underline}

\<script type=\"text/javascript\"\>

var **zx_search_query** = PW_Zanox.GetSearchQuery();

\</script\>

**TRACCIAMENTO VISTA SCHEDA PRODOTTO:**

[Funzioni disponibili]{.underline}

- **PW_Zanox.GetViewProductIdentifier()**: Restituisce il codice
  dell'articolo

- **PW_Zanox.GetViewProductName()**: Restituisce il nome del prodotto

- **PW_Zanox.GetViewProductDescription()**: Restituisce la descrizione
  del prodotto

- **PW_Zanox.GetViewProductCategory()**: Restituisce la categoria del
  prodotto

- **PW_Zanox.GetViewProductBrand()**: Restituisce il brand del prodotto

- **PW_Zanox.GetViewProductPrice()**: Restituisce il prezzo in formato
  descrittivo

- **PW_Zanox.GetViewProductAmount()**: Restituisce il prezzo in valore
  numerico

- **PW_Zanox.GetViewProductCurrency()**: Restituisce il currency code

- **PW_Zanox.GetViewProductLang()**: Restituisce la lingua di
  visualizzazione del prodotto

[Esempio di integrazione:]{.underline}

\<script type=\"text/javascript\"\>

var zx_identifier = PW_Zanox.GetViewProductIdentifier();

var zx_fn = PW_Zanox.GetViewProductName();

var zx_description = PW_Zanox.GetViewProductDescription();

var zx_category = PW_Zanox.GetViewProductCategory();

var zx_brand = PW_Zanox.GetViewProductBrand();

var zx_price = PW_Zanox.GetViewProductPrice();

var zx_amount = PW_Zanox.GetViewProductAmount();

var zx_currency = PW_Zanox.GetViewProductCurrency();

var zx_url = \"\";

var zx_photo = \"\";

var zx_language = PW_Zanox.GetViewProductLang();

\</script\>

**TRACCIAMENTO CARRELLO:**

[Funzioni disponibili]{.underline}

- **PW_Zanox.GetCartProducts()**: Restituisce un array con gli articoli
  presenti nel carrello

  - identifier: Restituisce il codice dell'articolo

  - amount: Restituisce il prezzo

  - quantity: Restituisce la quantità

  - currency: Restituisce la currency

[Esempio di integrazione:]{.underline}

\<script type=\"text/javascript\"\>

var zx_products = \[\];

var prd = PW_Zanox.GetCartProducts();

for(index = 0 ; index \< prd.length, index++){

zx_products.push({ identifier: prd\[index\].identifier, amount:
prd\[index\].amount, quantity: prd\[index\].quantity, currency:
prd\[index\].currency });

}

\</script\>

**TRACCIAMENTO DELLA CONFERMA DELL'ORDINE**

[Funzioni disponibili]{.underline}

- **PW_Zanox.GetTransactionItems()**: Restituisce gli articoli
  dell'ordine

  - **identifier**: Restituisce il codice dell'articolo

  - **amount**: Restituisce il prezzo

  - **quantity**: Restituisce la quantità

  - **currency**: Restituisce la currency

- **PW_Zanox.GetTransactionOrderId()**: Restituisce l'identificativo
  dell'ordine

- **PW_Zanox.GetTransactionTotalAmount()**: Restituisce il totale
  dell'ordine

- **PW_Zanox.GetTransactionCurrency()**: Restituisce la currency
  dell'ordine

- **PW_Zanox.GetTransactionLang()**: Restituisce la lingua degli
  articoli

[Esempio di integrazione:]{.underline}

\<script type=\"text/javascript\"\>

var zx_products = \[\];

var prd = PW_Zanox.GetTransactionItems();

for(index = 0; index \< prd.length; index++){

zx_products.push({ identifier: prd\[index\].identifier, amount:
prd\[index\].amount, currency: prd\[index\].currency, quantity:
prd\[index\].quantity });

}

var zx_transaction = PW_Zanox.GetTransactionOrderId();

var zx_total_amount = PW_Zanox.GetTransactionTotalAmount();

var zx_total_currency = PW_Zanox.GetTransactionCurrency();

var zx_language = PW_Zanox.GetTransactionLang();

\</script\>

