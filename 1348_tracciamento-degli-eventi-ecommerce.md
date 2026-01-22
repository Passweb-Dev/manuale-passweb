# TRACCIAMENTO DEGLI EVENTI ECOMMERCE



Il Tag descritto nel precedente capitolo di questo manuale consente di
tracciare solo ed esclusivamente le informazioni di base secondo quella
che è la specifica configurazione attivata nella corrispondente
proprietà GA4.

Nel momento in cui l'esigenza dovesse essere quella di attivare il
monitoraggio ecommerce, come già avveniva nel caso di UA, anche questa
volta sarà necessario creare altri tag specifici per ciascun evento
ecommerce che si desidera effettivamente tracciare.

In GA4 infatti il processo di attivazione e gestione del tracciamento
ecommerce è stato, sotto certi punti di vista, semplificato nel senso
che essendo il data model del nuovo sistema di tracciamento incentrato
interamente sugli eventi, non sarà più necessario attivare determinate
configurazioni sul proprio account di Analytics per poter gestire anche
il monitoraggio ecommerce ma, molto più semplicemente, è sufficiente
tracciare anche quelli che sono i diversi eventi ecommerce esattamente
allo stesso modo in cui dovranno essere tracciati tutti gli altri eventi
di interesse per il proprio sito.

E' bene sottolineare comunque che, in GA4, gli eventi ecommerce
rientrano tra quelli definiti come "**Eventi Consigliati**", non sono
quindi raccolti da Google in maniera automatica ne possono essere
collezionati con l'attivazione di un semplice check come si fa invece
per gli "Eventi di misurazione avanzata". Sotto questo punto di vista
dunque, allo stesso modo di quanto avveniva in UA, anche in GA4 sarà
necessario implementare (direttamente all'interno del sito o mediante
GTM) il codice necessario per inviare a GA4 gli eventi ecommerce da
tracciare assieme sempre a tutti i parametri richiesti.

In questo senso GA4 permette di analizzare come l'utente interagisce con
il nostro store on line attraverso una serie di 15 eventi ecommerce
consigliati. A questo indirizzo
<https://support.google.com/analytics/answer/9267735?hl=it&ref_topic=9756175>
(sezione "Per le vendite online") è possibile trovare maggiori
informazioni relativamente a ciascuno di questi eventi.

Nei successivi capitoli vedremo un po' più nel dettaglio quali di questi
eventi possono effettivamente essere tracciati e quali sono e come sono
strutturati i data layer presenti in Passweb per ciascuno di questi
stessi eventi

Anche nel caso di GA4 infatti la corretta configurazione dei Tag per il
tracciamento degli eventi ecommerce, non potrà prescindere dall'utilizzo
di un ben preciso Data Layer da cui poter prelevare i dati da inviare ad
Analytics.

Detto quindi che **Passweb gestisce nativamente il Data Layer relativo
ai principali eventi ecommerce consigliati da Google**, è abbastanza
semplice comprendere come, effettivamente, potrebbe essere molto più
semplice, anziché creare e gestire tanti singoli Tag, sfruttare la
comunicazione diretta tra GA4 ed il sito Passweb e quindi le
funzionalità native dell'applicativo che, attraverso la selezione di
semplici Flag, consentono di attivare tracciare gli stessi eventi
ecommerce.

In ogni caso, per completezza di trattazione, di seguito verrà indicata
la procedura da seguire per creare i Tag necessari a tracciare con GTM
gli eventi ecommerce attualmente gestiti in Passweb in maniera tale da
replicare, per quanto possibile, quello che avverrebbe sfruttando la
comunicazione diretta con Analytics.

Si ricorda comunque che **il presente manuale non è una guida ufficiale
di GTM per cui le procedure e le schermate presenti in queste pagine
potrebbero non essere allineate con l'effettiva interfaccia e/o con le
attuali funzionalità di GTM per cui è sempre bene fare riferimento anche
alla specifica documentazione di prodotto facilmente reperibile in
rete**

##### IMPOSTAZIONE SITO PASSWEB PER IL TRCCIAMENTO ECOMMERCE AVANZATO

Il primo passo da fare per poter tracciare gli eventi ecommerce di un
sito Passweb con GTM e GA4 è indubbiamente quello di settare
correttamente i parametri di configurazione per abilitare il sito stesso
a questo tipo di tracciamento.

In questo senso sarà necessario portarsi nel tab "**Tracciamento Dati"**
presente alla pagina **Sito -- Preferenze** del Wizard e da qui:

- Verificare di NON aver attivato il tracciamento diretto Passweb -- GA4
  ( parametri "**Versione Google Analytics**" e "**Chiave Google
  Analytics**" presenti all'interno della sezione "Google Analytics"
  **non valorizzati**) in maniera tale da non creare duplicazione di
  dati

- Verificare di aver impostato correttamente i parametri relativi al
  monitoraggio ecommerce presenti all'interno della sezione "**Eventi
  Ecommerce per Google Analytics e Google Tag Manager**" (pagina "**Sito
  -- Preferenze**" del Wizard tab "**Tracciamento Dati**")

![](./assets/media/image46.png)

> sul valore "**Client**" o "**Entrambi**"
>
> **ATTENZIONE!** nel momento in cui alcuni dei parametri evidenziati in
> figura dovessero essere impostati sull'opzione "**Server**", per i
> corrispondenti eventi ecommerce non verrà popolato il data layer
> rendendo di fatto impossibile tracciare l'evento stesso mediante GTM

- Verificare di aver impostato il parametro "**Versione Data Layer**"
  presente all'interno della sezione "Google Tag Manager" sull'opzione
  Google Analytics 4 in maniera tale da gestire il Data Layer con i
  parametri richiesti effettivamente da GA4

![](./assets/media/image47.png)

- Verificare di aver impostato correttamente gli snippet di codice
  necessari per l'installazione del contenitore di GTM sulle pagine del
  proprio sito (campi "**Monitoraggio Google Tag Manager -- HEAD**" e
  "**Monitoraggio Google Tag Manager -- BODY**")

![](./assets/media/image48.png)

**ATTENZIONE!** a differenza di quanto avveniva per UA, non sarà
necessario impostare setting particolari sul proprio account GA4 per cui
una volta impostato correttamente il sito Passweb, potremo passare
tranquillamente alla creazione su GTM dei vari tag necessari per
tracciare i diversi eventi ecommerce.

##### CREZIONE DELLE VARIBILI IN USO AGLI EVENTI ECOMMERCE

Come già accennato anche all'interno di questo stesso manuale la
principale differenza tra UA e GA4 sta proprio nel diverso data-model
utilizzato dai due sistemi di tracciamento e, nello specifico, nel fatto
che GA4 è basato interamente sulla gestione degli eventi (ogni cosa in
GA4 viene tratto e gestito come un evento la pageview, il tempo medio
passato su una pagina, le interazioni con i social ...).

Sotto questo aspetto poi il nuovo sistema di tracciamento è molto più
flessibile e ha molte meno restrizioni rispetto al suo predecessore. Con
GA4 infatti non si è più legati ai soli 4 parametri standard (Event
Category, Event Action, Event Label, Event Value) che potevano essere
abbinati agli eventi di Universal Analytics ma, in base a quelli che
sono gli obiettivi di analisi, è ora possibile impostare tutti i
parametri utili a descrivere meglio il contesto in cui l'evento si è
verificato.

Considerando dunque che dovremo essere noi a definire esattamente la
struttura del tracking andando ad aggiungere nel tag di ogni evento i
vari parametri (necessari e opzionali), prima di passare ad esaminare
come dovranno essere effettivamente creati questi stessi tag è bene
definire le diverse variabili che utilizzeremo per acquisire i dati dal
data-layer e per valorizzare, di conseguenza, i parametri da passare poi
ad Analytics, il tutto ovviamente facendo sempre riferimento a quelli
che sono gli eventi e i parametri consigliati da Google stesso in merito
al tracciamento ecommerce
(<https://support.google.com/analytics/answer/9267735?hl=it&ref_topic=9756175> -
<https://developers.google.com/analytics/devguides/collection/ga4/reference/events>
)

###### VARIABILE "GA4 -- DLV ECOMMERCE.ITEMS"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.items

**Contenuto della variabile**: array di prodotti (item) collegati
all'evento

**Tag in cui utilizzare la variabile**: tutti i tag di tracciamento
ecommerce

La variabile in esame consente di prelevare dal data layer del relativo
evento l'elenco di prodotti (con relativi parametri) coinvolti
nell'evento stesso.

Se pensiamo, ad esempio, all'evento di visualizzazione di un elenco di
prodotti, grazie a questa variabile sarà possibile passare ad Analytics
tutti gli articoli presenti nell'elenco stesso e, per ciascuno di essi
anche le relative informazioni (codice prodotto, nome prodotto, prezzo
...). Se pensiamo invece all'evento di aggiunta in carrello la variabile
in esame consentirà di passare ad Analytics tutti i dati del prodotto
che è stato effettivamente aggiunto.

**ATTENZIONE!** Come indicato nella documentazione ufficiale di Google,
per ogni evento ecommerce che si desidera tracciare è necessario passare
ad Analytics l'elenco di prodotti coinvolti nell'elenco stesso.

In conseguenza di ciò la variabile "GA4 -- DLV ecommerce.items" verrà
inserita in tutti i tag di tracciamento ecommerce che andremo poi a
configurare.

Di seguito viene indicato il procedimento da seguire per poter creare la
variabile in questione:

1.  Accedere al pannello di amministrazione del proprio account GTM,
    sezione "**Variabili**" (menu di sinistra), e creare una nuova
    variabile cliccando sul pulsante "**Nuova**" presente in
    corrispondenza del box "**Variabili definite dall'utente**"

![](./assets/media/image49.png)

2.  Cliccare sul pulsante "**Scegli un tipo di variabile per iniziare
    l'installazione**" presente in corrispondenza del box
    "**Configurazione Variabile**"

![](./assets/media/image50.png)

> e selezionare, tra le varie proposte, l'opzione "**Variabile di
> livello dati**"

![](./assets/media/image51.png)

3.  Nella successiva maschera impostare i campi di configurazione della
    variabile come di seguito indicato

![](./assets/media/image52.png)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.items**"

- **Versione livello dati**: impostare sull'opzione "**Versione 2**"

4.  Assegnare un nome alla variabile (es. "**GA4 -- DLV
    ecommerce.items**") utilizzando l'apposito campo presente nella
    parte alta della pagina

![](./assets/media/image53.png)

> e cliccare sul pulsante "**Salva**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.EVENT_CATEGORY"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.event_category

**Contenuto della variabile**: valore del parametro "event_category"
presente nel relativo data layer.

**Tag in cui utilizzare la variabile**: tutti i tag di tracciamento
ecommerce

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.event_category"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.EVENT_ACTION"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.event_action

**Contenuto della variabile**: valore del parametro "event_action"
presente nel relativo data layer.

**Tag in cui utilizzare la variabile**: tutti i tag di tracciamento
ecommerce

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.event_action"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.EVENT_LABEL"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.event_label

**Contenuto della variabile**: valore del parametro "event_lebel"
presente nel relativo data layer.

**Tag in cui utilizzare la variabile**: tutti i tag di tracciamento
ecommerce

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.event_label"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.CURRENCY"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.currency

**Contenuto della variabile**: valore del parametro "currency" presente
nel relativo data layer.

Il parametro currency verrà valorizzato con il codice ISO della valuta
in uso agli articoli presenti in ordine

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.currency"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.AFFILIATION"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.affiliation

**Contenuto della variabile**: valore del parametro "affiliation"
presente nel relativo data layer.

Il parametro affiliation verrà valorizzato con quanto inserito in
corrispondenza del parametro "**Nome Sito**" (pagina "Sito --
Preferenze" del Wizard, tab "SEO")

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.affiliation"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.COUPON"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.coupon

**Contenuto della variabile**: codice dell' eventuale buono sconto
utilizzato per la transazione.

Per transazioni in cui non vengono utilizzati codici sconto sarà
valorizzato con la stringa "No"

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.coupon"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.COUPON_VALUE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.coupon_value

**Contenuto della variabile**: importo dell'articolo spesa utilizzato
per gestire il relativo codice sconto (tipicamente un valore negativo).

Per transazioni in cui non vengono utilizzati codici sconto sarà
impostato a 0

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.coupon_value"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.PROMOZIONE_NAME"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.promozione_name

**Contenuto della variabile**: nome associato in Passweb alla
"Promozione in Carrello" che è stata effettivamente applicata e che ha
determinato l'aggiunta in carrello del relativo articolo di tipo Spesa.

Per transazioni a cui non vengono applicate promozioni sarà valorizzato
con la stringa "No"

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.promozione_name"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.PROMOZIONE_VALUE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.promozione_value

**Contenuto della variabile**: importo dell'articolo spesa utilizzato
per gestire la relativa promozione in carrello (tipicamente un valore
negativo).

Per transazioni a cui non vengono applicate promozioni sarà impostato a
0

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.coupon_value"**

###### VARIABILE "GA4 -- DLV ECOMMERCE.SHIPPING"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.shipping

**Contenuto della variabile**: valore delle spese di spedizione.

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.shipping"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.PAYMENT"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.payment

**Contenuto della variabile**: valore delle spese di pagamento.

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.payment"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.TAX"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.tax

**Contenuto della variabile**: valore dell' IVA

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.tax"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.SPESE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.spese

**Contenuto della variabile**: totale spese (generalmente coincide con
il totale degli articoli spesa eventualmente presenti in ordine)

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.spese"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.TOTALE_DOCUMENTO"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.totale_documento

**Contenuto della variabile**: totale documento ivato

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.totale_documento"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.TOTALE_MERCE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.totale_merce

**Contenuto della variabile**: totale merce

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
view_cart, begin_checkout, add_shipping_info, add_payment_info, purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.totale_merce"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.TRANSACTION_ID"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.transaction_id

**Contenuto della variabile**: id della transazione passweb

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.transaction_id"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.VALUE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.value

**Contenuto della variabile**: totale della transazione

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.value"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.DISCOUNT_PWB"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.discount_pwb

**Contenuto della variabile**: valore ivato dello sconto assegnato al
relativo prodotto

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
add_to_cart e remove_from_cart

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.discount_pwb"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.SHIPPING_TIER"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.shipping_tier

**Contenuto della variabile**: descrizione del metodo di spedizione

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
add_shipping_info

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.shipping_tier"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.PAYMENT_TYPE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.payment_type

**Contenuto della variabile**: descrizione del metodo di pagamento

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
add_payment_info

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.payment_type"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.DATETIME"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.dateTime

**Contenuto della variabile**: data e ora evento

**Tag in cui utilizzare la variabile**: tutti i tag di tracciamento
ecommerce [tranne quelli relativi agli eventi di: search, login,
sign_up, generate_lead (per i quali andrà utilizzata la variabile
successiva)]{.underline}

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.dateTime"**"

###### VARIABILE "GA4 -- DLV DATETIME"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV DateTime

**Contenuto della variabile**: data e ora evento

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
search, login, sign_up, generate_lead

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**dateTime"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.GIFT_CARD"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.gift_card

- **Contenuto della variabile**: True o False a seconda del fatto che
  per il pagamento dell'ordine sia stato utilizzato o meno il credito
  presente in una Gift Card

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.gift_card"**"

###### VARIABILE "GA4 -- DLV ECOMMERCE.PUNTI_PREMIO"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV ecommerce.punti_premio

- **Contenuto della variabile**: True o False a seconda del fatto che
  per il pagamento dell'ordine siano stati utilizzati o meno dei punti
  premio

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
purchase

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**ecommerce.punti_premio"**"

###### VARIABILE "GA4 -- DLV LOGIN_SIGNUP_METHOD"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Login_SignUp_Method

**Contenuto della variabile**: descrizione del metodo utilizzato per
l'autenticazione/registrazione al sito

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
login/sign_up

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**authenticationMethod**"

###### VARIABILE "GA4 -- DLV NEWSLETTER_SUBSCRIPTION"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Newsletter_Subscription

**Contenuto della variabile**: iscrizione al sistema di newsletter in
uso al sito

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
sign_up

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**newsletter_subscription**"

###### VARIABILE "GA4 -- DLV FORM_NAME"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Form_Name

**Contenuto della variabile**: nome assegnato in passweb al componente
form

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
generate_lead

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**form_name**"

###### VARIABILE "GA4 -- DLV SEARCH_CATEGORY"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Search_Category

**Contenuto della variabile**: tipologia di ricerca effettuata
internamente al sito (Ricerca Ecommerce/Ricerca CMS/Ricerca Testuale)

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
di ricerca

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**search_category**"

###### VARIABILE "GA4 -- DLV SEARCH_NOMECOMPONENTE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Search_NomeComponente (es. GA4 --
DLV Search_Codice)

**Contenuto della variabile**: valore utilizzato per la ricerca

**Tag in cui utilizzare la variabile**: tag di tracciamento degli eventi
di ricerca

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**search_nomecomponente**" (es. "search_codice")

**ATTENZIONE!** di base dovrebbe essere creata una variabile di questo
tipo per ogni campo presente all'interno del pannello di ricerca
utilizzato all'interno del sito

###### VARIABILE "GA4 -- DLV PAGE_TYPE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Page_Type

**Contenuto della variabile**: Tipologia di pagina visitata

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
wdata_loaded

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**page_type**"

###### VARIABILE "GA4 -- DLV VISITOR_LOGIN_STATE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Visitor_Login_State

**Contenuto della variabile**: Stato dell'utente

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
wdata_loaded

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**visitor_login_state**"

###### VARIABILE "GA4 -- DLV VISITOR_TYPE"

**Tipologia della variabile**: variabile di livello dati

**Nome della variabile**: GA4 -- DLV Visitor_Type

**Contenuto della variabile**: Tipologia utente loggato

**Tag in cui utilizzare la variabile**: tag di tracciamento dell'evento
wdata_loaded

La procedura da seguire per creare la variabile in esame è esattamente
la stessa di quella indicata nel precedente capitolo "*Variabile GA4 --
DLV ecommerce.items*" con le uniche differenze relative ovviamente al
nome da assegnare alla variabile e al valore da assegnare al campo "Nome
varabile di livello dati" (punto 3)

- **Nome varabile di livello dati**: impostare sul valore
  "**visitor_type**"

##### ARRAY ITEMS

Come indicato nella documentazione ufficiale Google

(
<https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?client_type=gtm>
)

tutti gli eventi connessi con il tracciamento ecommerce richiedono
l'invio ad Analytics di un array di oggetti (items) contenenti
informazioni relative ai singoli prodotti (item) coinvolti nell'evento
in questione.

Di seguito viene riportato un esempio della struttura dell'array items
gestito nei data layer di Passweb con l'indicazione, nel dettaglio, di
quali parametri verranno effettivamente considerati e come questi
verranno eventualmente valorizzati per ogni articolo coinvolto

###### ESEMPIO ARRAY ITEMS GESTITO NEI DATA LAYER DEGLI EVENTI PASSWEB

*items: \[*

*{*

*item_id: "Prod01A",*

*item_name: "Magic Mouse",*

*affiliation: "Store Clobis",*

*coupon: "Promo2022",*

*currency: "EUR",*

*discount: 2.22,*

*index: 0,*

*item_brand: "Apple",*

*item_category: "Apple",*

*item_category2: "Accessori",*

*item_category3: "Informatica",*

*item_category4: null,*

*item_category5: null,*

*item_list_id: null,*

*item_list_name: null,*

*item_variant: null,*

*location_id: null,*

*price: 59.99,*

*quantity: 3*

*},*

*...*

*{*

*item_id: "Prod35N,*

*item_name: "Felpa Nike",*

*affiliation: "Store Clobis",*

*coupon: "Promo2022",*

*currency: "EUR",*

*discount: 3.33,*

*index: 12,*

*item_brand: "Nike",*

*item_category: "Nike",*

*item_category2: "Felpe",*

*item_category3:"Abbigliamento",*

*item_category4: "Uomo",*

*item_category5: "Collezione_2022",*

*item_list_id: null,*

*item_list_name: null,*

*item_variant: "nero",*

*location_id: null,*

*price: 20.99,*

*quantity: 1*

*}*

*\]*

###### PARAMETRI ARTICOLO (ITEM) 

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
> item_category5 essendo nulli non verranno inseriti nel datlayer

- **item_list_id**: parametro non gestito

- **item_list_name**: valorizzato solo per gli eventi **view_item_list**
  e **view_cart** con il nome assegnato in Passweb al componente che
  individua la lista di articoli in cui il prodotto in esame è
  contenuto. Per tutti gli altri eventi ecommerce il parametro
  item_list_name non è gestito (e non verrà quindi inserito nel
  datalayer)

- **item_variant**: valorizzato solo per articoli a taglie/colori con il
  valore della relativa taglia/colore. Per articoli semplici il
  parametro item_variant assumerà sempre il valore null e non verrà
  quindi inserito nel datalyer

- **price**: prezzo di acquisto (**ivato**) dell'articolo in esame (al
  netto di eventuali sconti applicati all'articolo stesso)

##### IMPRESSIONE PRODOTTI -- VIEW_ITEM_LIST

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento delle impressioni generate dalla
visualizzazione di articoli presenti all'interno di componenti quali il
"Catalogo Ecommerce", le "Offerte / novità", gli "Abbinati" ecc... e la
procedura da seguire per creare, in GTM, un tag utile ad effettuare
questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'view_item_list',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Impression Product',*

*event_label: 'Vista Prodotti in Offerta',*

*currency: 'EUR',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56'*

*items: \[*

*{*

*item_id: 'Prod01A',*

*item_name: 'Magic Mouse',*

*currency: 'EUR',*

*discount: 2.22,*

*index: 1,*

*item_brand: "Apple",*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_list_name: 'Prodotti in Offerta',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*},*

*....*

*{*

*..parametri articolo N ...*

*}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Impression Product

- **event_label**: Vista + Nome assegnato in Passweb al componente che
  individua l'elenco di prodotti,

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**view_item_list**" presente alla pagina
  "***Sito Preferenze***" del Wizard, tab "***Tracciamento Dati***"
  sezione "***Parametro value eventi Analytics e Tag Manager***". Per
  maggiori informazioni in merito si veda anche quanto indicato
  all'interno del relativo capitolo di questo manuale ("*Sito --
  Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la visualizzazione
di una pagina con componenti quali il "Catalogo Ecommerce", le "Offerte
/ novità", gli "Abbinati" ecc...

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![Videate\\gtm_94.bmp](./assets/media/image55.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: view_item_list

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image56.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image57.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![Videate\\gtm_97.bmp](./assets/media/image59.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![Videate\\gtm_98.bmp](./assets/media/image63.png)

- **Nome Evento**: impostare su "***view_item_list***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -
    view_item_list**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 - View Item
    List**) operando dall'apposito campo presente nella parte alta della
    maschera

![Videate\\gtm_99.bmp](./assets/media/image64.png)

> e, infine, salvare il Tag cliccando sul pulsante "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

**ATTENZIONE!** La procedura appena descritta può essere utilizzata per
creare anche un qualsiasi altro Tag di tracciamento degli eventi
ecommerce con le uniche differenze rappresentate, ovviamente, dal nome
dell'evento da tracciare ed eventualmente dai parametri associati
all'evento stesso

##### CLICK PRODOTTO -- SELECT_ITEM

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare il click per andare poi a
visualizzare il dettaglio di un prodotto e la procedura da seguire per
creare, in GTM, un tag utile ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'select_item',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Click sul Prodotto',*

*event_label: 'Click del prodotto Magic Mouse,*

*content_type: 'product',*

*currency: 'EUR',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: 'Prod01A',*

*item_name: 'Magic Mouse',*

*currency: 'EUR',*

*discount: 2.22,*

*index: 1,*

*item_brand: "Apple",*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Click sul prodotto

- **event_label**: Click sul prodotto + Titolo del prodotto clicclato

- **content_type**: product

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**select_item**" presente alla pagina
  "***Sito Preferenze***" del Wizard, tab "***Tracciamento Dati***"
  sezione "***Parametro value eventi Analytics e Tag Manager***". Per
  maggiori informazioni in merito si veda anche quanto indicato
  all'interno del relativo capitolo di questo manuale ("*Sito --
  Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima il click per
visualizzare il dettaglio di un prodotto (partendo ad esempio dalla
cella dell'articolo stesso presente in catalogo)

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image65.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: select_item

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image66.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image67.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image68.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image69.png)

- **Nome Evento**: impostare su "***select_item***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event - select_item**")
    e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 - Select
    Item**) operando dall'apposito campo presente nella parte alta della
    maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### IMPRESSIONE PRODOTTO -- VIEW_ITEM

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare l'impressione generata dalla
visualizzazione del dettaglio di un prodotto e la procedura da seguire
per creare, in GTM, un tag utile ad effettuare questo tipo di
tracciamento

###### DATA LAYER

*{*

*event: 'view_item',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'View Detail Product',*

*event_label: 'Dettaglio del prodotto Magic Mouse,*

*currency: 'EUR',*

*value: 59.99,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: 'Prod01A',*

*item_name: 'Magic Mouse',*

*currency: 'EUR',*

*discount: 2.22,*

*index: 1,*

*item_brand: "Apple",*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 1*

*}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: View Detail Product

- **event_label:** Dettaglio del prodotto + Titolo del prodotto

- **currency:** codice ISO della valuta in uso al prodotto

- **value:** prezzo di vendita dell'articolo (valore di Default) oppure
  il valore personalizzato impostato per il parametro "**view_item**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la visualizzazione
di una scheda prodotto

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image70.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: view_item

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image71.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image72.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image73.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image74.png)

- **Nome Evento**: impostare su "***view_item***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event - view_item**") e
    cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 - View
    Item**) operando dall'apposito campo presente nella parte alta della
    maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### AGGIUNTA IN CARRELLO -- ADD_TO_CART

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'aggiunta di un prodotto in
carrello e la procedura da seguire per creare, in GTM, un tag utile ad
effettuare questo tipo di tracciamento

###### DATA LAYER

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

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: addToCart

- **event_label:** Aggiunto al Carrello il prodotto + Titolo del
  prodotto

- **currency:** codice ISO della valuta in uso al prodotto

- **value:** quantità con cui l'articolo è stato aggiunto in carrello
  (valore di Default), il corrispondente valore monetario (prezzo
  ivato), oppure il valore personalizzato impostato per il parametro
  "**GA4 --add_to_cart**" presente alla pagina "***Sito Preferenze***"
  del Wizard, tab "***Tracciamento Dati***" sezione "***Parametro Value
  eventi Analytics e Tag Manager***".

> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del relativo capitolo di questo manuale ("*Sito --
> Preferenze -- Tracciamento Dati*")

- **discount_pwb**: valore ivato dell'eventuale sconto relativo al
  prodotto aggiunto in carrello

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" l'aggiunta di un
articolo in carrello

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image75.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: add_to_cart

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image76.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image77.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: discount_pwb

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.discount_pwb**" precedentemente
  creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image78.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image79.png)

- **Nome Evento**: impostare su "***add_to_cart***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    add_to_cart**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Add To
    Cart**) operando dall'apposito campo presente nella parte alta della
    maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### RIMOZIONE DAL CARRELLO -- REMOVE_FROM_CART

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento della rimozione di un prodotto
dal carrello e la procedura da seguire per creare, in GTM, un tag utile
ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'remove_from_cart',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'removeFromCart',*

*event_label: 'Rimosso dal Carrello il prodotto Magic Mouse,*

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

*item_brand: "Apple",*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: removeFromCart

- **event_label:** Rimosso dal Carrello il prodotto + Titolo del
  prodotto

- **currency:** codice ISO della valuta in uso al prodotto

- **value:** quantità rimossa dal carrello (valore di Default), il
  corrispondente valore monetario (prezzo ivato), oppure il valore
  personalizzato impostato per il parametro "**remove_from_cart**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **discount_pwb**: valore ivato dell'eventuale sconto relativo al
  prodotto rimosso dal carrello

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la rimozione di un
articolo dal carrello

###### CREAZIONE DEL TAG 

- Accedere al proprio Account di Google Tag Manager, portarsi nella
  dashboard di gestione del Contenitore su cui si desidera operare e
  cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

- Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
  l'installazione**" presente all'interno del box "**Configurazione
  Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

- Selezionare tra quelli proposti il tag "**Google Analytics: evento
  GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

- Nella successiva maschera di configurazione del tag impostare i due
  parametri "Tag di configurazione" e "Nome evento" come nella figura di
  seguito riportata.

![](./assets/media/image80.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: remove_from_cart

<!-- -->

- A questo punto dovremo andare a definire i parametri da passare ad
  Analytics per l'evento in esame. Aprire quindi la sezione "**Parametri
  evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image81.png)

- Aggiungere i nuovi parametri completando i campi "Nome parametro" e
  "Valore" come nella figura di seguito riportata

![](./assets/media/image82.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: discount_pwb

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.discount_pwb**" precedentemente
  creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale
>
> recedenti capitoli di questo manuale

- Una volta completata la configurazione del Tag dovremo ora andare ad
  impostare l'Attivatore mediante il quale decidere quando e come questo
  stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image83.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

- Nella maschera di creazione del nuovo Attivatore cliccare su "**Scegli
  un tipo di trigger per iniziare l'installazione**" presente
  all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

- Nella successiva maschera impostare i parametri di configurazione
  dell'attivatore come nella figura di seguito riportata

![](./assets/media/image84.png)

- **Nome Evento**: impostare su "***remove_from_cart***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

<!-- -->

- Assegnare un nome all'Attivatore (es. "**GA4 Event --
  remove_from_cart**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

- Una volta completata anche la configurazione dell'Attivatore assegnare
  un nome al Tag che stiamo creando (es. **GA4 -- Remove From Cart**)
  operando dall'apposito campo presente nella parte alta della maschera
  e, infine, salvare il Tag cliccando sul pulsante "**Salva**"

- Verificare in modalità **Anteprima** il corretto funzionamento del Tag

- Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### AGGIUNTA ALLA WISHLIST -- ADD_TO_WISHLIST

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'aggiunta di un prodotto alla
wishlist e la procedura da seguire per creare, in GTM, un tag utile ad
effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'add_to_wishlist',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'addToWishlist',*

*event_label: 'Aggiunto alla Wishlist il prodotto Magic Mouse,*

*currency: 'EUR',*

*value: 3,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

*{*

*item_id: 'Prod01A',*

*item_name: 'Magic Mouse',*

*currency: 'EUR',*

*discount: 2.22,*

*index: 1,*

*item_brand: "Apple",*

*item_category: 'Apple',*

*item_category2: 'Accessori',*

*item_category3: 'Informatica',*

*item_variant: 'eventuale variante del prodotto',*

*price: 59.99,*

*quantity: 3*

*}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: addToWishlist

- **event_label:** Aggiunto alla Wishlist il prodotto + Titolo del
  prodotto

- **currency:** codice ISO della valuta in uso al prodotto

- **value:** quantità aggiunta in wishlist (valore di Default), il
  corrispondente valore monetario (prezzo ivato), oppure il valore
  personalizzato impostato per il parametro "**add_to_wishlist**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" l'aggiunta di un
articolo alla Wishlist

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image85.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: add_to_wishlist

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image86.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image87.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image88.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image89.png)

- **Nome Evento**: impostare su "***add_to_wishlist***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    add_to_wishlist**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Add To
    Wishlist**) operando dall'apposito campo presente nella parte alta
    della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### VISUALIZZAZIONE CARRELLO -- VIEW_CART

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'evento di visualizzazione
del carrello e la procedura da seguire per creare, in GTM, un tag utile
ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'view_cart',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'View Cart',*

*event_label: 'Vista Carrello',*

*currency: 'EUR',*

*spese:12,*

*tax:25.2,*

*totale_documento:87.7,*

*totale_merce:50.3,*

*shipping: 3,*

*payment: 10,*

*coupon: 'eventuale codice del coupon applicato',*

*coupon_value: 'eventuale importo del coupon',*

*promozione_name: 'eventuale nome della promo applicata',*

*promozione_value: 'eventuale importo della promo applicata',*

*value: 158.8,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

> *{*
>
> *item_id: "Prod01A",*
>
> *item_name: "Magic Mouse",*
>
> *currency: "EUR",*
>
> *discount: 2.22,*
>
> *index: 1,*

*item_brand: "Apple",*

> *item_category: "Apple",*
>
> *item_category2: "Accessori",*
>
> *item_category3: "Informatica",*
>
> *item_list_name: 'Carrello',*
>
> *item_variant: 'eventuale variante del prodotto',*
>
> *price: 59.99,*
>
> *quantity: 3*
>
> *},*
>
> *....*
>
> *{*
>
> *...parametri articolo N...*
>
> *}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: View Cart

- **event_label:** Vista + Nome del componente Carrello

- **currency:** codice ISO della valuta in uso ai prodotti in carrello

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in carrello)

- **tax**: totale iva in carrello

- **totale_documento**: totale carrello ivato

- **totale_merce**: totale merce carrello

- **shipping:** eventuale importo delle spese di spedizione

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **value:** totale carrello (valore di Default) oppure il valore
  personalizzato impostato per il parametro "**view_cart**" presente
  alla pagina "***Sito Preferenze***" del Wizard, tab "***Tracciamento
  Dati***" sezione "***Parametro value eventi Analytics e Tag
  Manager***". Per maggiori informazioni in merito si veda anche quanto
  indicato all'interno del relativo capitolo di questo manuale ("*Sito
  -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la visualizzazione
del carrello

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image90.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: view_cart

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image91.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image92.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: spese

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.spese**" precedentemente creata

- **Nome parametro**: tax

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.tax**" precedentemente creata

- **Nome parametro**: totale_documento

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_documento**" precedentemente
  creata

- **Nome parametro**: totale_merce

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_merce**" precedentemente
  creata

- **Nome parametro**: shipping

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping**" precedentemente creata

- **Nome parametro**: payment

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment**" precedentemente creata

- **Nome parametro**: coupon

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon**" precedentemente creata

- **Nome parametro**: coupon_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon_value**" precedentemente
  creata

- **Nome parametro**: promozione_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_name**" precedentemente
  creata

- **Nome parametro**: promozione_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_value**" precedentemente
  creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image93.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image94.png)

- **Nome Evento**: impostare su "***view_cart***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -- view_cart**")
    e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- View
    Cart**) operando dall'apposito campo presente nella parte alta della
    maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### INIZIO CHECKOUT -- BEGIN_CHECKOUT

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'inizio della fase di
checkout e la procedura da seguire per creare, in GTM, un tag utile ad
effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'begin_checkout',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Step Checkout -- Begin',*

*event_label: 'Avvio Checkout',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*payment: 10,*

*coupon: 'eventuale codice del coupon applicato',*

*coupon_value: 'eventuale importo del coupon',*

*promozione_name: 'eventuale nome della promo applicata',*

*promozione_value: 'eventuale importo della promo applicata',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

> *{*
>
> *item_id: "Prod01A",*
>
> *item_name: "Magic Mouse",*
>
> *currency: "EUR",*
>
> *discount: 2.22,*
>
> *index: 1,*

*item_brand: "Apple",*

> *item_category: "Apple",*
>
> *item_category2: "Accessori",*
>
> *item_category3: "Informatica",*
>
> *item_list_name: 'Carrello',*
>
> *item_variant: 'eventuale variante del prodotto',*
>
> *price: 59.99,*
>
> *quantity: 3*
>
> *},*
>
> *....*
>
> *{*
>
> *...parametri articolo N...*
>
> *}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Step Checkout - Begin

- **event_label:** Avvio Checkout

- **currency:** codice ISO della valuta in uso ai prodotti in carrello

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in ordine)

- **tax**: totale iva documento

- **totale_documento**: totale documento ivato

- **totale_merce**: totale merce

- **shipping:** eventuale importo delle spese di spedizione

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **value:** 1 (valore di Default), totale merce ivato oppure il valore
  personalizzato impostato per il parametro "**begin_checkout**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" l'inizio della
procedura di checkout

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image95.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: begin_checkout

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image96.png)

6.  Aggiungere i nuovi parametri completando i campi "Nome parametro" e
    "Valore" come nella figura di seguito riportata

![](./assets/media/image97.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: spese

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.spese**" precedentemente creata

- **Nome parametro**: tax

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.tax**" precedentemente creata

- **Nome parametro**: totale_documento

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_documento**" precedentemente
  creata

- **Nome parametro**: totale_merce

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_merce**" precedentemente
  creata

- **Nome parametro**: shipping

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping**" precedentemente creata

- **Nome parametro**: payment

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment**" precedentemente creata

- **Nome parametro**: coupon

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon**" precedentemente creata

- **Nome parametro**: coupon_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon_value**" precedentemente
  creata

- **Nome parametro**: promozione_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_name**" precedentemente
  creata

- **Nome parametro**: promozione_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_value**" precedentemente
  creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image98.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image99.png)

- **Nome Evento**: impostare su "***begin_checkout***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    begin_checkout**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Begin
    Checkout**) operando dall'apposito campo presente nella parte alta
    della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### INFORMAZIONI DI SPEDIZIONE -- ADD_SHIPPING_INFO

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'inserimento, durante la fase
di checkout, delle spese di spedizione e la procedura da seguire per
creare, in GTM, un tag utile ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'add_shipping_info',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Aggiunto Metodo di Spedizione',*

*event_label: 'Add Shipping Info Bartolini',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*shipping_tier: 'Bartolini',*

*payment: 10,*

*coupon: 'eventuale codice del coupon applicato',*

*coupon_value: 'eventuale importo del coupon',*

*promozione_name: 'eventuale nome della promo applicata',*

*promozione_value: 'eventuale importo della promo applicata',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

> *{*
>
> *item_id: "Prod01A",*
>
> *item_name: "Magic Mouse",*
>
> *currency: "EUR",*
>
> *discount: 2.22,*
>
> *index: 1,*

*item_brand: "Apple",*

> *item_category: "Apple",*
>
> *item_category2: "Accessori",*
>
> *item_category3: "Informatica",*
>
> *item_list_name: 'Carrello',*

*item_variant: 'eventuale variante del prodotto',*

> *price: 59.99,*
>
> *quantity: 3*
>
> *},*
>
> *....*
>
> *{*
>
> *...parametri articolo N...*
>
> *}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Aggiunto Metodo di Spedizione

- **event_label:** Add Shipping Info + Descrizione del metodo di
  spedizione selezionato

- **currency:** codice ISO della valuta in uso ai prodotti in carrello

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in ordine)

- **tax**: totale iva documento

- **totale_documento**: totale documento ivato

- **totale_merce**: totale merce

- **shipping:** eventuale importo delle spese di spedizione

- **shipping_tier:** descrizione del metodo di spedizione selezionato

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **value:** 1 (valore di Default), totale merce ivato oppure il valore
  personalizzato impostato per il parametro "**add_shipping_info**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la conferma della
selezione del metodo di spedizione

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image100.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: add_shipping_info

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image101.png)

6.  Aggiungere i nuovi parametri completando, per ciascuno di essi i
    campi "Nome parametro" e "Valore" come nella figura di seguito
    riportata

![](./assets/media/image102.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

- **Nome parametro**: shipping_tier

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping_tier**" precedentemente
  creata

- **Nome parametro**: shipping

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: spese

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.spese**" precedentemente creata

- **Nome parametro**: tax

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.tax**" precedentemente creata

- **Nome parametro**: totale_documento

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_documento**" precedentemente
  creata

- **Nome parametro**: totale_merce

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_merce**" precedentemente
  creata

- **Nome parametro**: payment

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment**" precedentemente creata

- **Nome parametro**: coupon

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon**" precedentemente creata

- **Nome parametro**: coupon_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon_value**" precedentemente
  creata

- **Nome parametro**: promozione_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_name**" precedentemente
  creata

- **Nome parametro**: promozione_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_value**" precedentemente
  creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image103.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image104.png)

- **Nome Evento**: impostare su "***add_shipping_info***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    add_shipping_info**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Add
    Shipping Info**) operando dall'apposito campo presente nella parte
    alta della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### INFORMAZIONI DI PAGAMENTO -- ADD_PAYMENT_INFO

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per consentire il tracciamento dell'inserimento, durante la fase
di checkout, della modalità di pagamento e la procedura da seguire per
creare, in GTM, un tag utile ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'add_payment_info',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Aggiunto Metodo di Pagamento',*

*event_label: 'Add Payment Info PayPal',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*payment: 10,*

*payment_type: 'PayPal'*

*coupon: 'eventuale codice del coupon applicato',*

*coupon_value: 'eventuale importo del coupon',*

*promozione_name: 'eventuale nome della promo applicata',*

*promozione_value: 'eventuale importo della promo applicata',*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

> *{*
>
> *item_id: "Prod01A",*
>
> *item_name: "Magic Mouse",*
>
> *currency: "EUR",*
>
> *discount: 2.22,*
>
> *index: 1,*

*item_brand: "Apple",*

> *item_category: "Apple",*
>
> *item_category2: "Accessori",*
>
> *item_category3: "Informatica",*
>
> *item_list_name: 'Carrello',*

*item_variant: 'eventuale variante del prodotto',*

> *price: 59.99,*
>
> *quantity: 3*
>
> *},*
>
> *....*
>
> *{*
>
> *...parametri articolo N...*
>
> *}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Aggiunto Metodo di Pagamento

- **event_label:** Add Payment Info + Descrizione del metodo di
  pagamento selezionato

- **currency:** codice ISO della valuta in uso ai prodotti in carrello

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in ordine)

- **tax**: totale iva documento

- **totale_documento**: totale documento ivato

- **totale_merce**: totale merce

- **shipping:** eventuale importo delle spese di spedizione

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **payment_type:** descrizione del pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **value:** 1 (valore di Default), totale merce ivato oppure il valore
  personalizzato impostato per il parametro "**add_payment_info**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" la conferma della
selezione della modalità di pagamento

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image105.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: add_payment_info

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image106.png)

6.  Aggiungere i nuovi parametri completando, per ciascuno di essi i
    campi "Nome parametro" e "Valore" come nella figura di seguito
    riportata

![](./assets/media/image107.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

- **Nome parametro**: payment_type

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment_type**" precedentemente
  creata

- **Nome parametro**: payment

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment**" precedentemente creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: spese

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.spese**" precedentemente creata

- **Nome parametro**: tax

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.tax**" precedentemente creata

- **Nome parametro**: totale_documento

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_documento**" precedentemente
  creata

- **Nome parametro**: totale_merce

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_merce**" precedentemente
  creata

- **Nome parametro**: shipping

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping**" precedentemente creata

- **Nome parametro**: coupon

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon**" precedentemente creata

- **Nome parametro**: coupon_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon_value**" precedentemente
  creata

- **Nome parametro**: promozione_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_name**" precedentemente
  creata

- **Nome parametro**: promozione_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_value**" precedentemente
  creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> Un discorso diverso, in questo senso, potrebbe essere fatato per il
> parametro "value", che potrebbe rivelarsi particolarmente utile nel
> momento in cui volessimo attribuire un valore monetario allo specifico
> evento. Tale valore potrebbe essere prelevato direttamente dal Data
> Layer di Passweb (e quindi potrebbe essere assegnato direttamente dal
> Wizard del sito) oppure potrebbe anche essere impostato direttamente
> in fase di configurazione del parametro senza ricorrere all'utilizzo
> della variabile "GA4 DLV -- ecommerce.value"
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image108.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image109.png)

- **Nome Evento**: impostare su "***add_payment_info***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    add_payment_info**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Add
    Payment Info**) operando dall'apposito campo presente nella parte
    alta della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### ACQUISTO -- PURCHASE

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare il completamento di un ordine e la
procedura da seguire per creare, in GTM, un tag utile ad effettuare
questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'purchase',*

*ecommerce: {*

*event_category: 'Ecommerce Avanzato',*

*event_action: 'Transaction',*

*event_label: 'Acquisto confermato + 1658',*

*transaction_id: 1658,*

*affiliation: 'Store Clobis',*

*currency: 'EUR',*

*spese:13,*

*tax: 85.78,*

*totale_documento: 517.69,*

*totale_merce: 418.91,*

*shipping: 3,*

*payment: 10,*

*shipping_tier: 'Bartolini',*

*payment_type: 'PayPal',*

*coupon: 'Promo 2022',*

*coupon_value: '-15.10,*

*promozione_name: 'Promo Telefoni',*

*promozione_value: '-105.10,*

*value: 130.54,*

*gift_card: 'True',*

*punti_premio: 'False',*

*dateTime:'11/10/2022, 14:54:56',*

*items: \[*

> *{*
>
> *item_id: "Prod01A",*
>
> *item_name: "Magic Mouse",*
>
> *currency: "EUR",*
>
> *discount: 2.22,*
>
> *index: 1,*

*item_brand: "Apple",*

> *item_category: "Apple",*
>
> *item_category2: "Accessori",*
>
> *item_category3: "Informatica",*
>
> *item_variant: 'eventuale variante del prodotto',*
>
> *price: 59.99,*
>
> *quantity: 3*
>
> *},*
>
> *....*
>
> *{*
>
> *...parametri articolo N...*
>
> *}*

*\]*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **event_category**: Ecommerce Avanzato

- **event_action**: Transaction

- **event_label:** Acquisto confermato + id transazione Passweb

- **transaction_id:** id della transazione Passweb

> **ATTENZIONE!** l'id della transazione (essendo ricollegabile allo
> specifico utente) può essere considerato come un dato di
> identificazione personale. In conseguenza di ciò nel momento in cui
> tale informazione dovesse essere inviata ad Analytics è necessario
> accertarsi di aver gestito in maniera corretta le richieste preventive
> di consenso e di aver inserito tutto il necessario nelle varie
> informative privacy presenti sul sito

- **affiliation:** valore del parametro "**Nome Sito**" (pagina "Sito --
  Preferenze" del Wizard, tab "SEO").

- **currency:** codice ISO della valuta in uso ai prodotti presenti in
  elenco

- **spese**: totale spese (generalmente coincide con il totale degli
  articoli spesa eventualmente presenti in ordine)

- **tax**: totale iva documento

- **totale_documento**: totale documento ivato

- **totale_merce**: totale merce

- **shipping:** eventuale importo delle spese di spedizione

- **shipping_tier:** descrizione del metodo di spedizione selezionato

- **payment:** eventuale costo aggiuntivo sul pagamento selezionato

- **payment_type:** descrizione del pagamento selezionato

- **coupon**: presente solo nel caso in cui sia stato applicato un Buono
  Sconto e valorizzato con il nome di quello stesso Buono Sconto

- **coupon_value**: presente solo nel caso in cui sia stato applicato un
  Buono Sconto e valorizzato con il valore del relativo sconto

- **promozione_name**: presente solo nel caso in cui sia stata applicata
  una Promozione e valorizzato con il nome di quella stessa Promo

- **promozione_value**: presente solo nel caso in cui sia stata
  applicata una Promozione e valorizzata con il valore del relativo
  sconto

- **gift_card:** "True / False" a seconda del fatto che per il pagamento
  dell'ordine sia stato utilizzato o meno il credito presente in una
  Gift Card

- **punti_premio:** "True / False" a seconda del fatto che per il
  pagamento dell'ordine siano stati utilizzati o meno dei punti premio

- **dateTime:** data e ora in cui si è verificato l'evento

- **value:** totale documento (valore di Default) oppure il valore
  personalizzato impostato per il parametro "**begin_checkout**"
  presente alla pagina "***Sito Preferenze***" del Wizard, tab
  "***Tracciamento Dati***" sezione "***Parametro value eventi Analytics
  e Tag Manager***". Per maggiori informazioni in merito si veda anche
  quanto indicato all'interno del relativo capitolo di questo manuale
  ("*Sito -- Preferenze -- Tracciamento Dati*")

- **items:** array dei prodotti presenti in elenco.

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" il processo di
checkout concludendo un ordine in maniera positiva

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image110.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: purchase

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image111.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image112.png)

> **[PARAMETRI OBBLIGATORI]{.underline}**

- **Nome parametro**: items

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.items**" precedentemente creata

- **Nome parametro**: transaction_id

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.transaction_id**" precedentemente
  creata

- **Nome parametro**: tax

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.tax**" precedentemente creata

- **Nome parametro**: spese

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.spese**" precedentemente creata

- **Nome parametro**: shipping

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping**" precedentemente creata

- **Nome parametro**: shipping_tier

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.shipping_tier**" precedentemente
  creata

- **Nome parametro**: payment

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment**" precedentemente creata

- **Nome parametro**: payment_type

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.payment_type**" precedentemente
  creata

- **Nome parametro**: totale_documento

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_documento**" precedentemente
  creata

- **Nome parametro**: totale_merce

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.totale_merce**" precedentemente
  creata

- **Nome parametro**: value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.value** precedentemente creata

- **Nome parametro**: currency

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.currency**" precedentemente creata

- **Nome parametro**: coupon

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon**" precedentemente creata

- **Nome parametro**: coupon_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.coupon_value**" precedentemente
  creata

- **Nome parametro**: promozione_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_name**" precedentemente
  creata

- **Nome parametro**: promozione_value

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.promozione_value**" precedentemente
  creata

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo, oltre al parametro items volendo, potremmo decidere di
> passare ad Analytics anche i seguenti parametri

- **Nome parametro**: event_action

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_action**" precedentemente
  creata

- **Nome parametro**: event_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_category**" precedentemente
  creata

- **Nome parametro**: event_label

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.event_label**" precedentemente
  creata

- **Nome parametro**: affiliation

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.affiliation**" precedentemente
  creata

- **Nome parametro**: gift_card

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.gift_card**" precedentemente creata

- **Nome parametro**: punti_premio

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.punti_premio**precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV ecommerce.dateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image113.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image114.png)

- **Nome Evento**: impostare su "***purchase***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -- purchase**") e
    cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 --
    Purchase**) operando dall'apposito campo presente nella parte alta
    della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### RICERCA -- SEARCH

**ATTENZIONE!** Come già evidenziato in merito all'integrazione diretta
Passweb -- Analytics **le ricerche interne al sito dovranno essere
trattate come dei normali eventi e, in queste condizioni, potranno
essere registrate anche nel momento in cui dovessimo decidere di non
abilitare il corrispondente evento di misurazione avanzata**

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare gli eventi di ricerca interna al
sito e la procedura da seguire per creare, in GTM, un tag utile ad
effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'search',*

*search_category: 'Ricerca ECommerce',*

*search_Nome_Tracciamento: valore utilizzato per la ricerca,*

*dateTime:'11/10/2022, 14:54:56',*

*ecommerce: {*

*value: 1*

*}*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **search_category:** Ricerca Ecommerce / Ricerca Testuale / Ricerca
  CMS

> **ATTENZIONE!** il parametro search_category assumerà uno dei tre
> valori sopra indicati in base alla tipologia del componente utilizzato
> per effettuare la ricerca sul sito

![](./assets/media/image115.png)

- **search_Nome_Tracciamento:** valore utilizzato per la ricerca

> dove
>
> **Nome_Tracciamento** coincide esattamente con quanto inserito nella
> maschera di configurazione del relativo componente di ricerca in
> corrispondenza del campo "Nome Tracciamento" (il tutto riportato in
> minuscolo)

![](./assets/media/image116.png)

> **ATTENZIONE!** Eventuali spazi presenti all'interno del campo
> evidenziato in figura verranno sostituiti dal carattere \_
>
> Nel momento in cui il campo in esame dovesse essere lasciato vuoto, al
> suo posto verrà utilizzato il nome (tutto in minuscolo) assegnato al
> componente
>
> Nel Data Layer verrà quindi inserito un parametro di questo tipo per
> ciascuno dei campi utilizzati (e quindi correttamente valorizzati) per
> effettuare la ricerca. Il valore assunto da questi stessi parametri
> potrà variare, ovviamente, in relazione al tipo di campo utilizzato
> per la ricerca
>
> Nel momento in cui all'interno del pannello di ricerca dovesse essere
> inserito, ad esempio, un componente di tipo "Filtro Checkbox", il
> valore che esso potrà assumere sarà solamente 1 e questo si potrà
> verificare solo se, in fase di ricerca , il check in esame dovesse
> essere effettivamente selezionato
>
> Supponendo dunque di utilizzare un pannello di ricerca di tipo
> Ecommerce con all'interno:

- un componente "Filtro Testo" con "Nome Tracciamento = Codice"

- un componente "Filtro Checkbox" con "Nome Tracciamento =
  Disponibilità"

- un componente "Filtro TreeView" con "Nome Tracciamento = Categoria
  Merceologica"

> e di effettuare una ricerca con il check relativo al campo
> "Disponibilità" selezionato e con il campo relativo al "Codice"
> valorizzato con la stringa "prod01A", il corrispondente evento
> "*search*" inviato a GA4 avrà (come nell'esempio sopra indicato) i due
> parametri addizionali

- *search_codice: 'prod01A'*

- *search_disponibilita: 1*

<!-- -->

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**GA4 -- search**" presente alla pagina
  "***Sito Preferenze***" del Wizard, tab "***Tracciamento Dati***"
  sezione "***Parametro Value eventi Analytics e Tag Manager***". Per
  maggiori informazioni in merito si veda anche quanto indicato
  all'interno del relativo capitolo di questo manuale ("*Sito --
  Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima", alcune ricerche
interne al sito

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image117.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: login

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image118.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image119.png)

> **ATTENZIONE!** i parametri di tipo search_nomeComponente dipendono
> ovviamente (sia dal punto di vista del nome che del numero) da quelli
> che sono i campi presenti all'interno del pannello di ricerca che si
> ha intenzione di tracciare
>
> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo potremmo decidere di passare ad Analytics anche il seguente
> parametro

- **Nome parametro**: search_category

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Search_Category**" precedentemente creata

- **Nome parametro**: search_nomeComponente -- dove ovviamente
  nomeComponente varia in base al nome assegnato allo specifico campo di
  ricerca presente nel pannello che si intende tracciare

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  corrispondente variabile "**GA4 -- DLV nomeComponente**"
  precedentemente creata (la variabile in questione deve, ovviamente,
  essere quella corrispondente al campo di ricerca cui fa riferimento il
  parametro in esame)

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV DateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image120.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image121.png)

- **Nome Evento**: impostare su "***search***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -- search**") e
    cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 --
    Purchase**) operando dall'apposito campo presente nella parte alta
    della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### AUTENTICAZIONE AL SITO -- LOGIN

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare l'autenticazione al sito e la
procedura da seguire per creare, in GTM, un tag utile ad effettuare
questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'login',*

*authenticationMethod: 'Sito'/ 'Facebook' / 'Google',*

*dateTime:'11/10/2022, 14:54:56',*

*value: 0*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **authenticationMethod:** stringa identificativa del metodo utilizzato
  per effettuare l'autenticazione al sito. Può assumere uno dei seguenti
  valori:

  - **Sito:** valore assegnato nel caso in cui l'autenticazione venga
    effettuata mediante un account registrato sul sito

  - **Facebook/Twitter/Google/PayPal ...**: valore assegnato nel caso in
    cui l'autenticazione venga effettuata con un social

- **dateTime:** data e ora in cui si è verificato l'evento

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" il processo di
autenticazione al sito

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image122.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: login

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image123.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image124.png)

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo potremmo decidere di passare ad Analytics anche il seguente
> parametro

- **Nome parametro**: method

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Login_SignUp_Method**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV DateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image125.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image126.png)

- **Nome Evento**: impostare su "***login***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -- login**") e
    cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 --
    Purchase**) operando dall'apposito campo presente nella parte alta
    della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### REGISTRAZIONE AL SITO -- SIGN_UP

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare la registrazione al sito e la
procedura da seguire per creare, in GTM, un tag utile ad effettuare
questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'sign_up,*

*authenticationMethod: 'Sito'/ 'Facebook' / 'Google',*

*form_name: 'Form Registrazione ',*

*newsletter_subscription: 'true / false',*

*dateTime:'11/10/2022, 14:54:56', ...*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **authenticationMethod:** stringa identificativa del metodo utilizzato
  per effettuare la registrazione al sito. Può assumere uno dei seguenti
  valori:

  - **Sito:** valore assegnato nel caso in cui la registrazione venga
    effettuata mediante un account registrato sul sito

  - **Facebook/Twitter/Google/PayPal ...**: valore assegnato nel caso in
    cui la registrazione venga effettuata tramite social

- **form_name:** Form + nome assegnato in passweb al componente form

- **newsletter_subscription:** true o false a seconda del fatto che
  l'utente abbia o meno deciso, in fase di registrazione, di iscriversi
  anche al sistema di newsletter (false a default)

- **dateTime:** data e ora in cui si è verificato l'evento

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima" il processo di
registrazione al sito

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image127.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: search

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image128.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image129.png)

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo potremmo decidere di passare ad Analytics anche il seguente
> parametro

- **Nome parametro**: method

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Login_SignUp_Method**" precedentemente creata

- **Nome parametro**: newsletter_subscription

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Newsletter_Subscription**" precedentemente
  creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV - DateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image130.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image131.png)

- **Nome Evento**: impostare su "***sign_up***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event -- sing_up**") e
    cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 -- Sign_Up**)
    operando dall'apposito campo presente nella parte alta della
    maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### COMPLETAMENTO FORM -- GENERATE_LEAD

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare il completamento di un form nativo e
la procedura da seguire per creare, in GTM, un tag utile ad effettuare
questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'generate_lead',*

*form_name: 'Form Contatti'*

*dateTime:'11/10/2022, 14:54:56', ...*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **form_name:** Form + nome assegnato in passweb al componente form

- **dateTime:** data e ora in cui si è verificato l'evento

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima", la compilazione
di un form nativo

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "Tag di configurazione" e "Nome evento" come nella figura
    di seguito riportata.

![](./assets/media/image132.png)

- **Tag di configurazione**: selezionare dal relativo menu a tendina il
  "Tag di configurazione GA4" precedentemente creato (per maggiori
  informazioni si veda quanto indicato all'interno del capitolo "*GTM e
  GA4 -- Installazione di GA4 con Google Tag Manager* ")

- **Nome evento**: generate_lead

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi Riga**"

![](./assets/media/image133.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image134.png)

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo potremmo decidere di passare ad Analytics anche il seguente
> parametro

- **Nome parametro**: form_name

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Form_Name**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV DateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image135.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image136.png)

- **Nome Evento**: impostare su "***generate_lead***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    generate_lead**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 --
    Generate_Lead**) operando dall'apposito campo presente nella parte
    alta della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

##### EVENTO CUSTOM -- WDATA_LOADED

Di seguito verrà riportato un esempio del Data Layer utilizzato da
Passweb per permettere di tracciare l'evento custom wdata_loaded, evento
questo che verrà generato a seguito di ogni vista ad una qualsiasi
pagina del sito e la procedura da seguire per creare, in GTM, un tag
utile ad effettuare questo tipo di tracciamento

###### DATA LAYER

*{*

*event: 'wdata_loaded,*

*page_type: 'store_cart'*

*visitor_login_state: 'not-logged'*

*visitor_type: 'privato'*

*dateTime:'11/10/2022, 14:54:56',*

*}*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **page_type:** Tipologia di pagina visitata.

> Il valore assegnato a questo parametro potrà quindi variare in
> relazione alla pagina visitata secondo il seguente schema:

- **store_root** 🡪 Home Page del sito

- **store_cart** 🡪 Pagina Carrello

- **store_checkout** 🡪 Pagina di Checkout (Ordine)

- **store_booking** 🡪 Pagina di Prenotazione (per siti Ho.Re.Ca.)

- **store_productpage** 🡪 Pagine Prodotto (Generica)

- **registration** 🡪 Pagina Registrazione (Nuovo Account)

- **profile** 🡪 Pagina Profilo (Dati Utente)

- **store_orders** 🡪 Pagina Ordini

- **store_page** 🡪Pagine Catalogo (pagine "azzurre")

- **product_page** 🡪 Pagina Prodotto di Categoria (pagine "rosse")

- **wishlist** 🡪 Pagina Wishlist

- **rma** 🡪 Pagina Reso Merce

- **giftregistry** 🡪 Pagina Lista Regalo

- **giftcard** 🡪 Pagina Gift Card

- **rewardpoints** 🡪 Pagina Punti Utente

- **page** 🡪 Pagina Generica (pagine "bianche")

<!-- -->

- **visitor_login_state**: stato dell'utente che visita il sito.

> Il valore assegnato a questo parametro varierà in relazione al fatto
> che l'utente abbia o meno effettuato l'accesso al sito secondo il
> seguente schema:

- **logged-in** 🡪 valore assegnato al parametro nel caso in cui l'utente
  abbia già effettuato il login al sito

- **not-logged** 🡪 valore assegnato al parametro nel caso in cui
  l'utente non abbia ancora effettuato il login al sito

<!-- -->

- **visitor_type**: tipologia dell'utente autenticato

> Il parametro in esame assumerà un valore **solo dopo che l'utente che
> visita il sito ha effettuato il login** e potrà assumere i seguenti
> valori:

- **privato** 🡪 valore assegnato al parametro nel caso in cui l'utente
  autenticato sia un "Privato"

- **azienda** 🡪 valore assegnato al parametro nel caso in cui l'utente
  autenticato sia un' "Azienda"

<!-- -->

- **dateTime:** data e ora in cui si è verificato l'evento

Per verificare i dati effettivamente presenti in questo Data Layer si
consiglia di simulare su GTM, in modalità "Anteprima", la visita ad una
qualsiasi pagina del sito sia come utente non autenticato che come
utente autenticato

###### CREAZIONE DEL TAG 

1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png)

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png)

3.  Selezionare tra quelli proposti il tag "**Google Analytics: evento
    GA4**"

![Videate\\gtm_93.bmp](./assets/media/image54.png)

4.  Nella successiva maschera di configurazione del tag impostare i due
    parametri "ID Misurazione" e "Nome evento" come nella figura di
    seguito riportata.

![](./assets/media/image137.png)

- **ID Misurazione**: indicare l'ID Misurazione dello stream di dati di
  Google Analytics a cui si desidera inviare i dati

- **Nome evento**: wdata_loaded

5.  A questo punto dovremo andare a definire i parametri da passare ad
    Analytics per l'evento in esame. Aprire quindi la sezione
    "**Parametri evento**" e cliccare sul pulsante "**Aggiungi
    parametro**"

![](./assets/media/image138.png)

6.  Aggiungere i parametri correlati all'evento completando, per
    ciascuno di essi i campi "Nome parametro" e "Valore" come nella
    figura di seguito riportata

![](./assets/media/image139.png)

> **[PARAMETRI OPZIONALI]{.underline}**
>
> Considerando la struttura del Data Layer esaminata nel precedente
> capitolo potremmo decidere di passare ad Analytics anche il seguente
> parametro

- **Nome parametro**: page_type

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Page_Type**" precedentemente creata

- **Nome parametro**: visitor_login_state

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Visitor_Login_State**" precedentemente creata

- **Nome parametro**: visitor_type

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV Visitor_Type**" precedentemente creata

- **Nome parametro**: dateTime

- **Valore**: cliccare sul pulsante di selezione delle variabili " (
  ![Videate\\gtm_selezione_variabili.bmp](./assets/media/image58.png) ) e selezionare tra quelle proposte la
  variabile "**GA4 -- DLV DateTime**" precedentemente creata

> Ovviamente nel momento in cui il valore assegnato nel Data Layer di
> Passweb ai parametri opzionali sopra indicati non dovesse essere utile
> al tipo di tracciamento che vogliamo effettivamente realizzare e ai
> dati che vogliamo quindi riportare nei report di Analytics, questi
> stessi parametri (tutti o in parte) potrebbero anche non essere
> inseriti nella configurazione del tag.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla creazione
> delle suddette variabili si veda quanto indicato nei precedenti
> capitoli di questo manuale

7.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![](./assets/media/image140.png)

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png)

8.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png)

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png)

9.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![](./assets/media/image141.png)

- **Nome Evento**: impostare su "***wdata_loaded***"

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

10. Assegnare un nome all'Attivatore (es. "**GA4 Event --
    wdata_loaded**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

11. Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GA4 --
    Wdata_Loaded**) operando dall'apposito campo presente nella parte
    alta della maschera e, infine, salvare il Tag cliccando sul pulsante
    "**Salva**"

12. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

13. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore

