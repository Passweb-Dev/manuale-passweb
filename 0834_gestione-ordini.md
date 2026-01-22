# GESTIONE ORDINI



All'interno della sezione **"Catalogo -- eBay - Ordini"** è possibile
visualizzare e gestire tutti gli ordini acquisiti direttamente dal
Marketplace a seguito di sincronizzazioni manuali e/o automatiche

I pulsanti presenti nella barra degli strumenti della maschera "**Lista
Ordini**" consentono di gestire i diversi stati del documento e di
comunicare eventuali variazioni al relativo Marketplace.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_gestione_ordini_0.bmp](./assets/media/image167.png){width="5.889583333333333in"
height="3.428472222222222in"}

**Parametri Ordine** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_parametri_ordine.bmp](./assets/media/image168.png){width="0.5520833333333334in"
height="0.15555555555555556in"} ): consente di impostare una o più
causali, opportunamente definite all' interno del gestionale, ed
utilizzate per marcare come "**Annullati**" gli ordini provenienti dal
Marketplace.

**ATTENZIONE! le causali impostate all'interno di questa sezione sono
valide a livello generale per tutti gli ordini presenti in elenco.**

![Videate\\ebay_gestione_ordini_1.bmp](./assets/media/image169.png){width="5.889583333333333in"
height="3.428472222222222in"}

E' possibile annullare un ordine indicando due diverse motivazioni,
corrispondenti ciascuna ad una delle causali impostate all'interno della
maschera di seguito evidenziata

- **L\'acquirente ha richiesto di annullare l\'ordine o c\'è un problema
  con l\'indirizzo dell\'acquirente:** consente di definire la causale
  di annullamento utilizzata all'interno del gestionale per marcare il
  relativo ordine come Annullato in conseguenza del fatto che
  "*l'acquirente ha richiesto di annullare l'ordine oppure si è
  verificato un problema di spedizione*".

- **Ho esaurito l\'oggetto o l\'oggetto è danneggiato:** consente di
  definire la causale di annullamento utilizzata all'interno del
  gestionale per marcare il relativo ordine come Annullato in
  conseguenza del fatto che "*i prodotti in ordine sono esauriti o
  danneggiati*".

**ATTENZIONE!** Nel caso di **siti Ecommerce collegati a Mexal** è
necessario indicare, nei due campi sopra evidenziati, il codice delle
relative Causali. Nel caso invece di **siti Ecommerce collegati ad uno
dei gestionali Ho.Re.Ca** il nome di queste stesse causali.

Annullando un ordine all'interno del gestionale e utilizzando, allo
stesso tempo, una delle due causali sopra indicate, sarà quindi
possibile comunicare automaticamente, in fase di sincronizzazione Sito
-- Gestionale, il cambio di stato anche al relativo Marketplace.

**Annulla** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_annulla.bmp](./assets/media/image170.png){width="0.2986111111111111in"
height="0.16875in"} ): consente di porre l'ordine attualmente
selezionato in elenco nello stato di "**In Attesa di Annullo**"
indicando anche la motivazione per cui l'ordine in esame è stato
annullato

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Annulla"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà visualizzata la maschera "**Parametri
di Annullamento dell'Ordine**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_gestione_ordini_2.bmp](./assets/media/image171.png){width="5.811805555555556in"
height="3.428472222222222in"}

all'interno della quale poter indicare, selezionandola dall'apposito
menu a tendina (campo **Motivo di Annullamento**), la motivazione per
cui si desidera annullare quello specifico ordine.

**ATTENZIONE!** Una volta impostato un "Motivo di Annullamento" l'ordine
sarà posto, come detto, nello stato di "**In Attesa di Annullo**" ma non
verrà comunicato nulla al relativo marketplace dove l'ordine manterrà,
quindi, il suo stato originario.

In queste condizioni per completare l'annullamento dell'ordine sarà
necessario eseguire manualmente la procedura di "Aggiornamento Ordini"
sul Marketplace (pulsante **Aggiorna Ordini**) oppure attendere la
prossima sincronizzazione "Sito -- Gestionale".

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Annullato**" anche all'interno del proprio sito Passweb. Lato
gestionale l'ordine manterrà invece il suo stato originale (essendo
l'annullamento partito dal sito Passweb) e sarà quindi necessaria una
sincronizzazione per allineare lo stato del documento anche sul
gestionale.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Annullo**" e provvederà ad effettuare il cambio di stato sia verso il
marketplace che verso il gestionale in maniera del tutto automatica.

In entrambi i casi dunque al termine della sincronizzazione l'ordine
sarà in stato "**Annullato**" sul gestionale, sul sito Passweb e sul
relativo Marketplace.

**ATTENZIONE!** Per maggiori informazioni sulle procedure di
annullamento di un ordine eBay si veda anche il successivo capitolo di
questo manuale (*Stati Ordine eBay*)

**Spedizione** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mp_pulsante_spedizione.bmp](./assets/media/image172.png){width="0.38333333333333336in"
height="0.1625in"} ): consente di porre l'ordine attualmente selezionato
in elenco nello stato di "**In Attesa di Spedizione**"

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Spedizione"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Parametri della Spedizione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_parametri_spedizione.bmp](./assets/media/image173.png){width="5.889583333333333in"
height="3.428472222222222in"}

all'interno della quale poter impostare:

- **Vettore:** consente di impostare, selezionandolo dal relativo menu a
  tendina, il Vettore eBay utilizzato per effettuare la spedizione
  relativamente all'ordine in questione.

> **ATTENZIONE!** All'interno del campo "Vettore" verranno visualizzati
> solo ed esclusivamente quei metodi di trasporto configurati come
> Vettori eBay e per i quali è stato quindi valorizzato, in fase di
> configurazione, il relativo campo "**Vettore eBay**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_parametri_spedizione_2.bmp](./assets/media/image174.png){width="5.616666666666666in"
height="3.4611111111111112in"}

> Per maggiori informazioni in merito si veda anche la sezione "*Ordini
> -- Configurazione Metodi di trasporto*" di questo manuale.

- **Data di Inizio Trasporto:** consente di impostare la data di inizio
  trasporto relativamente all'ordine in questione.

- **Number Tracking:** consente di impostare il Number Tracking
  assegnato dallo spedizioniere alla spedizione che si sta effettuando.

**ATTENZIONE!** Nel caso in cui **il processo di spedizione parta dal
gestionale** mediante la valorizzazione dei relativi campi, tutti e tre
i parametri presenti all'interno di questa maschera saranno in sola
visualizzazione.

Una volta impostati questi parametri cliccando sul pulsante "Salva"
l'ordine passerà in stato di "**In Attesa di Spedizione**" ma non verrà
comunicato nulla al relativo marketplace dove l'ordine manterrà, quindi,
il suo stato originario.

In queste condizioni per completare il processo di spedizione
dell'ordine sarà necessario eseguire manualmente la procedura di
"Aggiornamento Ordini" sul Marketplace (pulsante **Aggiorna Ordini**)
oppure attendere la prossima sincronizzazione "Sito -- Gestionale".

**ATTENZIONE!** Per effettuare il cambio di stato da "In Attesa di
Spedizione" a "Spedito" è necessario che tutti e tre i campi "Vettore",
"Data Inizio Trasporto" e "Number Tracking" siano stati correttamente
valorizzati. Nel caso in cui anche uno soltanto di questi non dovesse
essere valorizzato l'ordine rimarrà sempre nello stato di "In Attesa di
Spedizione"

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Spedito**" anche all'interno del proprio sito Passweb. Lato
gestionale non verrà apportata ancora nessuna modifica all'ordine e sarà
quindi necessaria una sincronizzazione per allineare lo stato del
documento anche sul gestionale.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Spedizione**", provvederà ad effettuare il cambio di stato (che passerà
quindi a "**Spedito**") anche verso il marketplace e inserirà lato
gestionale il vettore la data di inizio trasporto e, dove possibile,
anche il Number Tracking impostati all'interno del sito.

Nello specifico **Vettore, Data di Inizio Trasporto** e **Number
Tracking** verranno inseriti nei relativi campi presenti nel piede del
documento

![Videate\\ebay_parametri_spedizione_3.bmp](./assets/media/image175.png){width="5.961111111111111in"
height="2.584722222222222in"}

![Videate\\ebay_parametri_spedizione_3a.bmp](./assets/media/image176.png){width="5.480555555555555in"
height="2.8048611111111112in"}

Per i siti Ecommerce collegati a Mexal, nel momento in cui il Number
Tracking dovesse essere gestito con un Attributo Ordine, il codice di
spedizione verrà ovviamente inserito all'interno dell'apposito campo
della videata riportabile utente utilizzata per gestire l'attributo in
esame.

In tutti i casi, comunque, al termine della sincronizzazione l'ordine
sarà in stato "**Spedito**" sul marketplace a all'interno del proprio
sito Passweb mentre all'interno del gestionale saranno stati valorizzati
i campi del Vettore, della Data di Inizio Trasporto e del Number
Tracking.

**ATTENZIONE!** Affinchè i valori inseriti da Passweb siano
correttamente visibili nel piede dei documenti Mexal, è necessario che
il parametro di magazzino "**Memorizza data e ora inizio trasporto**"
sia stato correttamente selezionato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\memorizza_data_spedizione.bmp](./assets/media/image177.png){width="4.2340277777777775in"
height="3.363888888888889in"}

Nel caso in cui il parametro in oggetto non fosse stato selezionato,
Data e ora di inizio trasporto impostate da Passweb potranno essere
visibili all'interno di bolle e/o fatture ma non all'interno di ordini.

Per maggiori informazioni sulle procedure di spedizione di un ordine
eBay si veda anche il successivo capitolo di questo manuale (*Stati
Ordine eBay*)

**Pagamento** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_pulsante_pagamento.bmp](./assets/media/image178.png){width="0.3958333333333333in"
height="0.15555555555555556in"} ): consente di porre l'ordine
attualmente selezionato in elenco nello stato di "**In Attesa di
Pagamento**"

**ATTENZIONE! Le impostazioni settate mediante il pulsante "Pagamento"
valgono solo ed esclusivamente per l'ordine attualmente selezionato in
elenco**

Cliccando su questo pulsante verrà visualizzata la maschera "**Parametri
Pagamento Ordine**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_parametri_pagamento.bmp](./assets/media/image179.png){width="5.889583333333333in"
height="3.428472222222222in"}

all'interno della quale l'utente avrà la possibilità di modificare lo
stato dell'ordine in relazione al suo avvenuto pagamento

Nello specifico impostando il parametro **Pagato** sul valore:

- **SI**: l'ordine verrà posto nello stato di "**In Attesa di
  Pagamento**"

In queste condizioni per completare il processo di pagamento dell'ordine
sarà necessario eseguire manualmente la procedura di "Aggiornamento
Ordini" sul Marketplace (pulsante **Aggiorna Ordini**) oppure attendere
la prossima sincronizzazione "Sito -- Gestionale".

Nel primo caso (pulsante **Aggiorna Ordini**) verrà comunicato il cambio
di stato al relativo Marketplace e l'ordine passerà nello stato di
"**Pagato**" anche all'interno del proprio sito Passweb.

Nel secondo caso, durante la prossima sincronizzazione Sito Gestionale,
Passweb verificherà la presenza di un ordine in stato "**In Attesa di
Pagamento**" e provvederà ad effettuare il cambio di stato (che passerà
quindi a "**Pagato**") anche verso il marketplace.

**ATTENZIONE**! **Gli stati "In Attesa di Pagamento" e "Pagato" non
hanno un corrispettivo gestionale per cui possono essere gestiti solo
all'interno di questa sezione del Wizard di Passweb oltre a poter essere
comunicati anche al relativo Marketplace eBay.**

Il fatto di poter porre un ordine in stato di "In Attesa di Pagamento",
o "Pagato" può essere particolarmente utile in relazione a quegli ordini
eBay che non vengono pagati immediatamente mediante carta di credito ma
per i quali è stata abilitata e scelta un'altra tipologia di pagamento.

**Aggiorna Ordini** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiorna_ordini.bmp](./assets/media/image180.png){width="0.5256944444444445in"
height="0.15555555555555556in"} ): consente di eseguire, in maniera
manuale, la procedura di aggiornamento dello stato ordini dal proprio
sito Passweb verso i relativi Marketplace eBay.

**ATTENZIONE!** La procedura "Aggiorna Ordini" eseguita da questa
sezione del Wizard funziona esclusivamente dal sito Passweb verso i
Marketplace e non ha alcuna influenza sul gestionale.

Per maggiori informazioni relativamente ai vari cambi di stato e a come
poter comunicare tali informazioni ai relativi marketplace si veda anche
il successivo capitolo ("*Stati Ordine eBay*") di questo manuale.

