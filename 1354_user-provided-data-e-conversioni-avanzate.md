# USER PROVIDED DATA E CONVERSIONI AVANZATE



Oltre ai dati esaminati nei precedenti capitoli di questo manuale
indispensabili, come visto, per poter implementare mediante Google Tag
Manager un tracciamento ecommerce avanzato per il proprio sito web,
Passweb offre la possibilità di inserire all'interno del proprio
dataLayer anche tutti i dati utente di prima parte necessari per poter
attivare sia in Google Analytics ma soprattutto in Google AdWords la
gestione degli User Provided Data e delle Conversioni Avanzate
(**enhanced conversion**)

Per poter inserire questo tipo di dati all'interno del dataLayer di
Passweb è sufficiente attivare il parametro "**Raccolta Dati Utente nel
Data Layer**" presente alla pagina "**Sito -- Preferenze**" del Wizard
(tab "**Tracciamento Dati**" sezione "**Google Tag Manager**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_attivazione_upd_1.bmp](./assets/media/image199.png)

Da un punto di vista tecnico infatti l'attivazione del parametro
evidenziato in figura comporterà l'inserimento nel dataLayer, per ogni
evento Ecommerce gestito, anche di una sezione **user_data** del tipo di
quella di seguito indicata

*user_data: {*

*sha256_email_address: valore hashato della mail utente ,*

*sha256_phone_number: valore hashato del telefono utente,*

*address: {*

*sha256_first_name: valore hashato del nome utente,*

*sha256_last_name: valore hashato del cognome / ragione sociale utente,*

*street: indirizzo utente (via),*

*city: indirizzo utente (città),*

*postal_code: indirizzo utente (CAP),*

*country: indirizzo utente (Nazione)*

*}*

*}*

In considerazione di ciò in corrispondenza, ad esempio, di un evento di
tipo *add_to_cart* il dataLayer generato da Passweb avrà una struttura
del tipo di quella di seguito indicata:

*{*

*event: 'add_to_cart',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'addToCart',*

*event_label: 'Aggiunto al Carrello il prodotto Magic Mouse,*

*currency: 'EUR',*

*value: 3,*

*discount_pwb: 2.22,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: 'Prod01A',*

*item_name: 'Magic Mouse',*

*currency: 'EUR',*

*discount: 2.22,*

*index: 1,*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*}*

*\]*

*},*

***user_data {***

***sha256_email_address: valore hashato della mail utente,***

***sha256_phone_number:*** ***valore hashato del telefono utente,***

***address: {***

***sha256_first_name: valore hashato del nome utente,***

***sha256_last_name: valore hashato del cognome / ragione sociale
utente,***

***street: \"via ernani 8\",***

***city:\"Rimini\",***

***postal\_ code: \"47922\",***

***country: \"Italy\"***

***}***

***}***

*}*

Inoltre occorre anche sottolineare che

- nel dataLayer dei diversi eventi gestiti da Passweb, la sezione
  *user_data* sarà presente solo nel momento in cui a visitare la pagina
  o ad eseguire una determinata azione dovesse essere un utente
  autenticato

- nel momento in cui un utente dovesse effettuare un ordine da "Ospite"
  con il checkout in un unico step, la sezione "*user_data*" potrà
  essere inserita, ovviamente, solo nel dataLayer dell'evento di
  ***purchase*** che, in queste condizioni, sarà quindi l'unico evento
  lato client in relazione al quale poter gestire i dati utente
  necessari per il tracciamento della conversione avanzata

- nel momento in cui un utente dovesse effettuare un ordine da "Ospite"
  con il checkout a step multipli, la sezione "*user_data*" potrà essere
  inserita, in tutti gli eventi del checkout relativi agli step
  successivi al primo (in cui l'utente di fatto si registra) e quindi
  oltre all'evento di ***purchase***, in queste condizioni i dati utente
  necessari per il tracciamento delle conversioni avanzate potranno
  essere prelevati anche in relazione agli eventi di
  ***add_shipping_info*** e ***add_payment_info***

- relativamente agli eventi di "*sign_up*" la sezione "*user_data*"
  verrà inserita nel dataLayer dell'evento stesso e conterrà,
  ovviamente, i dati inseriti dall'utente in fase di registrazione.
  Nello specifico, in questo caso all'interno della sezione
  "*user_data*" del dataLayer verrà inserito solamente l'indirizzo mail

- relativamente agli eventi di "*generate_lead*" la sezione
  "*user_data*" verrà inserita nel dataLayer dell'evento stesso e come
  dati potrà avere solamente l'indirizzo mail di chi ha compilato il
  form (quindi del lead).

> In questo senso sarà quindi di fondamentale importanza inserire
> all'interno del form un campo di tipo Email obbligatorio che l'utente
> dovrà valorizzare con il proprio indirizzo mail e, in fase di
> configurazione, impostare il parametro **Id/Name** del campo in
> oggetto sul valore "**email**"

- i parametri mail, telefono, ... saranno hashati come richiesto da
  google e verranno effettivamente inseriti nel dataLayer solo se il
  loro valore non dovesse essere nullo (nel caso in cui, ad esempio, per
  un dato utente non dovessimo avere disponibile il telefono il
  parametro *sha256_phone_number* non sarà inserito nel dataLayer)

Ora, il fatto di avere a disposizione nel dataLayer i dati utente, come
noto, non comporta assolutamente che queste informazioni vengano poi
passate anche a Google Analytics, a Google Ads o ad un qualsiasi altro
sistema di terze parti.

Per fare in modo che questi dati possano essere trasmessi a queste
piattaforme e che possano quindi essere utilizzati per la gestione delle
conversioni avanzate dovranno infatti essere configurati in maniera
opportuna anche i relativi Tag di tracciamento.

In questo senso la prima cosa da fare sarà quindi quella di creare,
all'interno di Google Tag Manager le variabili necessarie per poter
accedere ai dati utente presenti nel dataLayer di Passweb.

Nei successivi capitoli di questo manuale vedremo dunque come poter
creare queste variabili e come configurare i Tag di tracciamento
presenti all'interno di Google Tag Manager per fare in modo che i dati
utente prelevati dal sito possano essere trasmessi alla piattaforma
collegata (AdWords piuttosto che Google Analytics).

