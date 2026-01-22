# SIMULATORE DI PAGAMENTO



Come evidenziato nel precedente capitolo di questo manuale, e come già
avviene per altre modalità di pagamento analoghe, anche Pago Light mette
a disposizione degli utenti un simulatore di pagamento che, oltre ad
essere visualizzato direttamente in fase di checkout, volendo, può
essere inserito anche all'interno della pagina prodotto.

Ovviamente, in fase di checkout l'importo su cui verrà effettuata la
simulazione di rateizzazione sarà il totale ordine; se inserito
all'interno della pagina prodotto invece l'importo considerato sarà il
prezzo dello specifico articolo.

**ATTENZIONE!** Il simulatore di pagamento è gestito direttamente da
Pago Light e viene iniettato sulle pagine del sito Passweb mediante un
apposito snippet di codice.

Per attivare il simulatore di Pago Light è necessario inserire
correttamente lo snippet di configurazione, fornito direttamente dalla
piattaforma terza, all'interno del campo "**Script simulatore di
pagamento**" presente tra i parametri di configurazione del relativo
Gateway

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pago_light_simulatore_1.bmp](./assets/media/image147.png)

In questo senso i due pulsanti **"Script Default Pagolight Standard"** e
**"Script Default Pagolight PRO"** consentono di inserire all'interno
del campo in esame i relativi snippet di codice necessari per attivare
sia il Simulatore Standard sia quello PRO

**ATTENZIONE!** gli snippet di codice utilizzati per gestire il
simulatore possono variare nel corso del tempo essendo gestiti
direttamente da PagoLight. **Si consiglia quindi di verificare sempre
che lo script inserito in automatico da Passweb sia effettivamente
quello attualmente utilizzato da PagoLight** e di apportare, nel caso,
le modifiche necessario (per maggiori informazioni in merito è
necessario rivolgersi direttamente all'assistenza di PagoLight)

**ATTENZIONE!** Il simulatore attivato deve essere ovviamente coerente
con la tipologia di contratto effettivamente sottoscritta con Pagolight

[**SIMULATORE STANDARD**]{.underline}

Consente di visualizzare all'interno del sito (pagina Prodotto e Pagina
Checkout) solo alcune informazioni generiche relative al pagamento in
oggetto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_simulatore_standard.bmp](./assets/media/image148.png)

Dal punto di vista della sua configurazione vanno considerati con
particolare attenzione i due parametri di seguito indicati:

- **data-heidipay-minorAmount:** consente di indicare l'importo che
  dovrà essere passato al Widget di Pagolight per calcolare eventuali
  simulazioni di rateizzazione.

> Considerando che l'importo da rateizzare, ovviamente, potrà variare in
> relazione al totale dello specifico ordine e/o al prezzo dello
> specifico prodotto, **il parametro in questione dovrà essere
> valorizzato con il segnaposto "Prezzo"** selezionabile dal relativo
> menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_prezzo.bmp](./assets/media/image149.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_prezzo_2.bmp](./assets/media/image150.png)

- **data-heidipay-term:** consente di indicare il numero massimo di rate
  che verranno poi effettivamente proposte all'utente in fase di
  pagamento sulla piattaforma terza.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_rate.bmp](./assets/media/image151.png)

> Il numero indicato in corrispondenza di questo parametro, verrà poi
> visualizzato sul simulatore nel front end del sito web

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_rate_2.bmp](./assets/media/image152.png)

> e dovrà, ovviamente, coincidere con il numero massimo di rate
> effettivamente proposte in fase di pagamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_rate_3.bmp](./assets/media/image153.png)

[**SIMULATORE PRO**]{.underline}

Consente di mostrare, direttamente all'interno del proprio sito web, le
diverse possibili opzioni di rateizzazione che verranno poi
effettivamente proposte anche in fase di pagamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_simulatore_pro.bmp](./assets/media/image154.png)

Dal punto di vista della sua configurazione vanno considerati con
particolare attenzione i parametri di seguito indicati:

- **data-heidipay-minorAmount:** consente di indicare l'importo che
  dovrà essere passato al Widget di Pagolight per calcolare eventuali
  simulazioni di rateizzazione.

> Considerando che l'importo da rateizzare, ovviamente, potrà variare in
> relazione al totale dello specifico ordine e/o al prezzo dello
> specifico prodotto, **il parametro in questione dovrà essere
> valorizzato con il segnaposto "Prezzo"** selezionabile dal relativo
> menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_segnaposto_prezzo.bmp](./assets/media/image149.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_pro_segnaposto_prezzo_2.bmp](./assets/media/image155.png)

- **data-heidipay-apiKey:** consente di inserire l'api key necessaria
  per il corretto funzionamento del simulatore pro.

> **ATTENZIONE!** la chiave da inserire all'interno del parametro in
> questione deve essere richiesta direttamente a Pago Light

- **data-heidipay-allowedterms:** consente di indicare i diversi
  possibili numeri di rate che dovranno essere utilizzati in fase di
  simulazione della rateizzazione.

> E' possibile utilizzare il segnaposto "**Numero di rate**"
> selezionabile dal relativo menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_pro_segnaposto_rate_2.bmp](./assets/media/image156.png)

> che verrà poi sostituito a runtime con quanto inserito all'interno del
> campo "**Numero di rate**" presente tra i parametri di configurazione
> del gateway precedentemente analizzati
>
> **ATTENZIONE!** i numeri di rate utilizzati dal simulatore dovranno,
> ovviamente, essere gli stessi che verranno poi effettivamente proposti
> all'utente in fase di pagamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_pro_segnaposto_rate_3.bmp](./assets/media/image157.png)

- **data-heidipay-pricing-structure-code:** consente di inserire il
  "Codice Tabella" necessario per il corretto funzionamento del
  simulatore.

> **ATTENZIONE!** il codice tabella da inserire all'interno del
> parametro in questione deve essere richiesta direttamente a Pago Light
>
> E' possibile utilizzare il segnaposto "**Codice Tabella**"
> selezionabile dal relativo menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagolight_pro_segnaposto_tabella_2.bmp](./assets/media/image158.png)

> che verrà poi sostituito, a runtime, con quanto inserito all'interno
> del campo "**Codice Tabella**" presente tra i parametri di
> configurazione del gateway precedentemente analizzati

