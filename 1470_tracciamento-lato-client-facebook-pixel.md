# TRACCIAMENTO LATO CLIENT -- FACEBOOK PIXEL



Come già indicato nei precedenti capitoli di questo manuale, per poter
implementare in maniera corretta il tracciamento lato Client è
necessario utilizzare il Pixel di Facebook (o Pixel Meta), uno strumento
questo, indispensabile per raccogliere i dati relativi alle diverse
azioni compiute dai visitatori del sito ed inviarli poi, mediante
apposite istruzioni javascript, ai server di Facebook

Il pixel di Facebook, che di fatto dunque, altro non è se non un
particolare snippet di codice javascript, consente di rilevare e
tracciare eventi come:

- La visualizzazione di pagina

- L'aggiunta / rimozione di articoli in carrello

- La conferma di un acquisto

- ...

**ATTENZIONE! Il pixel di Facebook, e quindi il tracciamento lato
client, è basato sull'utilizzo di appositi cookie che verranno
installati sul browser degli utenti. In conseguenza di ciò, come già per
Google Analytics, nel momento in cui si dovesse decidere di gestire
questo tipo di tracciamento sarà necessario attivare anche tutte le
relative misure richieste dal GDPR**

Di seguito viene descritta la procedura necessaria per creare un Pixel
di Facebook è installarlo all'interno del proprio sito Passweb.

- Accedere al proprio Account **Business Manager**, aprire il menu
  "**Tutti gli Strumenti**" e selezionare la voce "**Gestione Eventi**"

![Videate\\facebook_tracciamento_client_1.bmp](./assets/media/image1.png){width="5.2340277777777775in"
height="3.532638888888889in"}

> **ATTENZIONE!** il Pixel di Facebook, così come l'Access Token
> necessario per attivare le Conversion API, può essere generato
> unicamente all'interno del Business Manager di Facebook. Il fatto
> dunque di disporre di un proprio Business Manager è un prerequisito
> indispensabile per attivare sia il tracciamento lato client che quello
> lato server
>
> Per maggiori informazioni relativamente a come attivare un proprio
> Business Manager creando il relativo account si consiglia di fare
> riferimento alla documentazione ufficiale presente sui siti di
> Facebook

- Una volta effettuato l'accesso alla sezione "Gestione Eventi" cliccare
  sul pulsante verde raffigurante un piccolo + (**Collega origini dei
  dati**)

![Videate\\facebook_tracciamento_client_2.bmp](./assets/media/image2.png){width="5.2340277777777775in"
height="3.532638888888889in"}

- Nella successiva maschera di collegamento dell'origine dati
  selezionare l'opzione "**Web**" e cliccare sul pulsante "**Collega**"

![Videate\\facebook_tracciamento_client_3.bmp](./assets/media/image3.png){width="3.5388888888888888in"
height="1.6104166666666666in"}

- Assegnare quindi un nome al pixel e cliccare infine sul pulsante
  "**Crea Pixel**"

![Videate\\facebook_tracciamento_client_4.bmp](./assets/media/image4.png){width="2.4479166666666665in"
height="1.4347222222222222in"}

- Una volta completata la creazione del Pixel, portarsi all'interno
  della sezione "**Impostazioni**"

![Videate\\facebook_tracciamento_client_5.bmp](./assets/media/image5.png){width="5.2340277777777775in"
height="3.532638888888889in"}

> copiare quindi l'Id presente in corrispondenza della sezione "**Id del
> pixel**" evidenziata in figura, e incollarlo all'interno del campo
> "**Pixel ID**" presente nella sezione "**Facebook Pixel -- Conversion
> API**" alla pagina "**Sito -- Preferenze**" del Wizard (tab
> "**Tracciamento Dati**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\facebook_tracciamento_client_6.bmp](./assets/media/image6.png){width="5.792361111111111in"
height="3.50625in"}

- Completare quindi l'attivazione del tracciamento lato client per il
  proprio sito Passweb verificando di aver correttamente selezionando il
  parametro "**Tracciamento Client**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\facebook_tracciamento_client_7.bmp](./assets/media/image7.png){width="5.792361111111111in"
height="3.50625in"}

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
**attivare solamente il tracciamento mediante Facebook Pixel** sarà
sufficiente flaggare il parametro "**Tracciamento Client**" e inserire
nel campo "**Pixel ID**" l'id del pixel precedentemente creato

In realtà, come precedentemente indicato, la creazione del Pixel di
Facebook, di per sé, non sarebbe sufficiente a completare
l'implementazione del tracciamento lato client. Oltre a questo sarebbe
infatti indispensabile inserire e gestire all'interno del proprio sito
anche i diversi snippet di codice javascript necessari per inviare ai
server di facebook tutte le informazioni raccolte dal pixel stesso in
merito a quello che gli utenti stanno facendo all'interno nostro sito.

In questo senso è bene quindi sottolineare che **Passweb implementa già,
in maniera nativa, gli snippet di codice necessari per tracciare i
seguenti eventi standard:**

- PageView -- Visualizzazione di pagina

- ViewContent -- Visualizzazione dei contenuti

- AddToCart -- Aggiunta al carrello

- AddToWishlist -- Aggiunta alla Wishlist

- AddPaymentInfo -- Aggiunta delle informazioni di pagamento

- InitiateCheckout -- Inizio di acquisto

- Purchase -- Acquisto

- Search -- Ricerca

- CompleteRegistration -- Registrazione

- Lead -- Acquisizione Contatto

**ATTENZIONE!** Un elenco completo di tutti gli eventi standard gestiti
da Facebook può essere visualizzato al seguente link

<https://developers.facebook.com/docs/meta-pixel/implementation/conversion-tracking#standard-events>

Il parametro "**Abilita eventi custom**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\facebook_eventi_custom.bmp](./assets/media/image8.png){width="5.792361111111111in"
height="3.50625in"}

consente invece, se selezionato, di attivare anche il tracciamento dei
seguenti eventi personalizzati:

- SelectItem -- Selezione prodotto

- ViewItemList -- Visualizzazione elenco prodotti

- ViewCart -- Visualizzazione carrello

- RemoveFromCart -- Rimozione dal carrello

- AddShippingInfo -- Aggiunta informazioni di spedizione

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri, e
quindi alle singole informazioni, passate a facebook con ciascuno degli
eventi sopra indicati si veda anche quanto riportato nel successivo
capitolo "*Eventi e Parametri*" di questo manuale

Nel momento in cui l'esigenza dovesse essere, dunque, quella di
**tracciare, lato client, uno degli eventi sopra indicati**, una volta
selezionato il parametro "**Tracciamento client**" (ed eventualmente
anche quello "**Abilita eventi custom**") e inserito l'id del pixel,
secondo quanto precedentemente evidenziato**, non saranno necessarie
ulteriori azioni** e il nostro sito inizierà già a tracciare questi
stessi eventi.

**ATTENZIONE!** una volta attivato il tracciamento lato client seguendo
la procedura appena descritta verificare anche di non aver inserito in
maniera manuale, da qualche altra parte del sito, il codice di
tracciamento fornito da facebook (ad esempio quello relativo al
tracciamento delle visualizzazioni di pagina). In caso contrario infatti
gli stessi eventi e/o le stesse visite al sito potrebbero essere
conteggiati più di una sola volta.

**Anche dal punto di vista del GDPR il tracciamento lato client di
Facebook è già integrato nativamente con le diverse piattaforme CMP
(Iubenda, Cookiebot ...) attivabili in Passweb**. Ciò significa dunque
che, come per il tracciamento mediante Google Analytics, anche in questo
caso, nel momento in cui la piattaforma utilizzata per gestire i cookie
e i vari consensi GDPR dovesse essere, ad esempio, Iubenda, gli snippet
di codice necessari per l'installazione dei cookie e l'invio dei dati
statistici e di profilazione ai server di facebook verranno
effettivamente attivati solo nel caso in cui l'utente che naviga il sito
abbia effettivamente prestato tutti i consensi necessari.

**ATTENZIONE! nel caso in cui l'esigenza dovesse essere invece quella di
tracciare un evento (standard o custom) diverso da quelli
precedentemente indicati, sarà necessario gestire l'evento stesso in
maniera manuale inserendo quindi all'interno del sito tutto il codice
necessario per fare in modo che l'evento stesso venga correttamente
registrato ed inviato a facebook.**

Per maggiori informazioni relativamente agli eventi gestiti da Facebook
si consiglia sempre di fare riferimento alla relativa documentazione
ufficiale (
<https://www.facebook.com/business/m/one-sheeters/facebook-pixel-events>
)

