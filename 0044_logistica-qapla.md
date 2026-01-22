# LOGISTICA -- QAPLA'



Qaplà ( <https://www.qapla.it> ) è un sistema integrato che permette di
gestire le spedizioni dalla stampa dell\'etichetta, fino alla notifica
di consegna e che si rivela particolarmente utile per quegli shop online
che vogliono prendere il controllo del loro "ultimo miglio", aggregando
informazioni di tracking da diversi corrieri nazionali e internazionali,
raccogliendo informazioni in real time sulle spedizioni e fornendo
comunicazioni dirette ai clienti.

Grazie ai servizi offerti da questa piattaforma è possibile:

- Stampare le etichette per i principali corrieri, come BRT, GLS, SDA,
  TNT, DHL, UPS, Crono, Nexive e Fercam ...

- Monitorare tutte le spedizioni con un unico pannello di controllo in
  maniera tale da avere sempre la situazione sotto controllo e poter
  dare ai clienti tutte le informazioni sull'avanzamento della
  spedizione in tempo reale grazie anche ad una tracking page
  personalizzata.

- Inviare Mail, SMS e notifiche di consegna inserendo così, anche nelle
  mail sullo stato di avanzamento della spedizione, specifiche proposte
  commerciali (Coupon di sconto, banner o link ad offerte speciali,
  articoli consigliati ...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_1.bmp](./assets/media/image121.png)

##### INTEGRAZIONE PASSWEB -- QAPLA'

Per poter realizzare l'integrazione tra il proprio sito Ecommerce e la
piattaforma Qaplà, abilitando così il trasferimento automatico degli
ordini da Passweb verso la piattaforma terza, è necessario disporre di
apposite Api Key prelevabili direttamente dal back end di Qaplà.

Una volta attivato il proprio account sarà quindi necessario:

- effettuare l'accesso al relativo pannello di controllo, portarsi
  all'interno della sezione "*Canali*"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_2.bmp](./assets/media/image122.png)

> e cliccare sul pulsante "**Configura**" presente in corrispondenza del
> proprio canale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_2_1.bmp](./assets/media/image123.png)

- Copiare le chiavi presenti in corrispondenza dei campi "**API Key
  Privata**" e "**API Key Pubblica**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_2a.bmp](./assets/media/image124.png)

> e incollarle rispettivamente all'interno dei campi "**Qaplà API Key
> Privata**" e "**Qaplà API Key Pubblica**" presenti alla pagina "*Sito
> -- Preferenze -- Integrazioni*" del Wizard (sezione "**Logistica
> Qaplà**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_3.bmp](./assets/media/image125.png)

Infine, considerando che l'integrazione Passweb -- Qaplà sfrutta anche i
WebHook messi a disposizione da questa stessa piattaforma per ottenere
informazioni relativamente al tracking e alla generazione delle
spedizioni, per completare la configurazione sarà necessario impostare
correttamente, all'interno del pannello di controllo di Qaplà i suddetti
WebHook.

In questo senso quindi, sarà necessario portarsi all'interno della
sezione "**Aggiornamenti - WebHook**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_4.bmp](./assets/media/image126.png)

e attivare sia il Webhook relativo alla "**notifica tracking
spedizioni**" che quello relativo alla "**notifica generazione
spedizioni**" (parametro "Attivazione" sul valore "Attiva") e inserire
nei due campi URL i seguenti indirizzi:

- Webhook di notifica tracking spedizioni 🡪 URL =
  <https://www.nomesito.it/WebHookQaplaShipment>

- Webhook di notifica generazione spedizioni 🡪 URL =
  <https://www.nomesito.it/WebHookQaplaOrder>

Terminati questi semplici passaggi l'integrazione Passweb -- Qaplà
potrebbe ritenersi conclusa e ogni ordine che dovesse trovarsi, in
Passweb, nello stato di:

- **Memorizzato**

- **Modificato**

- **Sospeso**

- **Annullato**

verrà inviato, in fase di sincronizzazione, anche a Qaplà.

In queste condizioni, dunque, nel momento in cui dovesse essere
effettuato un nuovo ordine all'interno del sito, e questo stesso
documento dovesse essere inserito correttamente all'interno del
gestionale, passando quindi dallo stato di "Nuovo" a quello di
"Memorizzato", al termine del processo di sincronizzazione l'ordine in
esame verrà inviato anche a Qaplà.

**ATTENZIONE!** anche ordini provenienti da marketplace esterni come
Amazon e eBay una volta acquisiti da Passweb e inseriti nel gestionale
si troveranno nello stato di "Memorizzato" e potrebbero quindi, in fase
di sincronizzazione, essere inviati a Qaplà

**Questo potrebbe causare un problema di duplicazione dei documenti nel
momento in cui, anche su Qaplà, dovesse essere attiva l'integrazione con
lo stesso Marketplace gestito da Passweb**. In questo caso infatti lo
stesso ordine potrebbe essere riportato su Qaplà sia dall'integrazione
diretta Qaplà -- Amazon / eBay, sia dall'integrazione Passweb -- Qaplà.

In conseguenza di ciò, nel momento in cui si dovesse decidere di
utilizzare l'integrazione diretta Qaplà -- Amazon /eBay per gestire la
logistica degli ordini acquisiti da questi marketplace, sarà necessario
accertarsi di aver deselezionato, in fase di configurazione
dell'integrazione Passweb -- Qaplà, i check "**Invia gli ordini MFN di
Amazon a Qaplà**" e "**Invia gli ordini eBay a Qaplà**" presenti
all'interno della sezione **"Logistica Qaplà**" (sezione "*Sito --
Preferenze*")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_amazon_ebay.bmp](./assets/media/image127.png)

- **Invia gli ordini MFN di Amazon a Qaplà:** consente, se selezionato,
  di inviare a Qaplà, in fase di sincronizzazione, anche gli ordini in
  stato "Memorizzato" provenienti da Amazon a patto che siano di tipo
  **MFN** (con logistica cioè a carico del venditore)

> **ATTENZIONE!** gli ordini Amazon di tipo **AFN** (con logistica
> gestita direttamente da Amazon) non verranno mai inviati a Qaplà
> indipendentemente dal loro stato
>
> Nel momento in cui dovesse essere attiva l'integrazione diretta Qaplà
> -- Amazon, per evitare duplicazione di documenti il parametro in esame
> dovrà essere deselezionato
>
> **ATTENZIONE!** La disattivazione di questo parametro non andrà ad
> influire in alcun modo sull'integrazione Passweb -- Amazon. Passweb
> continuerà quindi ad acquisire normalmente gli ordini Amazon evitando
> però di inviarli anche a Qaplà

- **Invia gli ordini di eBay a Qaplà:** consente, se selezionato, di
  inviare a Qaplà, in fase di sincronizzazione, anche gli ordini in
  stato "Memorizzato" provenienti da eBay

> Nel momento in cui dovesse essere attiva l'integrazione diretta Qaplà
> -- eBay, per evitare duplicazione di documenti, il parametro in esame
> dovrà essere deselezionato
>
> **ATTENZIONE!** La disattivazione di questo parametro non andrà ad
> influire in alcun modo sull'integrazione Passweb -- eBay. Passweb
> continuerà quindi ad acquisire normalmente gli ordini eBay evitando
> però di inviarli anche a Qaplà

Infine, è bene considerare, come precedentemente evidenziato, che
verranno inviati a Qaplà anche ordini in stato "**Sospeso**" e
"**Annullato**". Ciò significa dunque che, una volta importato l'ordine
all'interno del gestionale, se questo dovesse poi subire delle modifiche
prima che venga creata la spedizione (e prima quindi che venga generata
la relativa bolla o fattura) queste stesse modifiche verranno riportate,
in fase di sincronizzazione, non solo all'interno di Passweb ma anche
sui relativi documenti Qaplà che potranno quindi essere modificati sia
in termini di contenuto che in termini di Stato.

**ATTENZIONE!** Al termine della sincronizzazione verrà inviata, all'
amministratore del sito, una specifica mail per informarlo relativamente
al passaggio di determinati ordini sulla piattaforma terza

##### DATI DELLA SPEDIZIONE

Per ogni ordine inviato da Passweb a Qaplà verranno trasferite alla
piattaforma terza determinate informazioni, alcune sempre presenti e
indispensabili per poter creare poi la relativa spedizione, altre invece
opzionali e legate essenzialmente a specifiche impostazioni di
configurazione del proprio sito Ecommerce.

Tra le informazioni "obbligatorie" trasmesse a Qaplà ad ogni ordine,
troveremo ovviamente:

- Cliente intestatario dell'ordine (Nome / Cognome / Ragione Sociale)

- Indirizzo mail del cliente intestatario

- Indirizzo di spedizione

- Elenco articoli in ordine

- Stato Ordine

- Totale Ordine

Queste informazioni potranno essere visualizzate su Qaplà nella maschera
contenente l'elenco di tutti gli ordini acquisiti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_lista_ordini.bmp](./assets/media/image128.png)

e, ovviamente nella maschera di dettaglio del relativo documento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_6.bmp](./assets/media/image129.png)

Tra le informazioni "opzionali" potremo invece trovare il peso degli
articoli in ordine, opzioni di consegna al piano, opzioni di
assicurazione, etichette personalizzate utili a capire come dovrà poi
essere gestita la relativa spedizione ecc...

In particolare:

- Nel momento in cui l'esigenza dovesse essere quella di inviare a Qaplà
  anche il peso (singolo e totale) degli articoli presenti in ordine,
  sarà necessario gestire questo tipo di informazione, per ogni singolo
  prodotto, mediante il corrispondente campo presente nell'anagrafica
  Passweb dell'articolo stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_8.bmp](./assets/media/image130.png)

> Gestendo quindi il peso degli articoli mediante il campo evidenziato
> in figura, sulla piattaforma terza sarà poi possibile visualizzare,
> per ogni ordine, il peso complessivo dei prodotti presenti all'interno
> di quello stesso documento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_9.bmp](./assets/media/image131.png)

> Aprendo il dettaglio dell'ordine sarà invece possibile visualizzare,
> nella parte bassa, il peso dei singoli articoli.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_10.bmp](./assets/media/image132.png)

> Per maggiori informazioni relativamente a come poter gestire, in
> Passweb, il peso dei vari articoli si veda anche quanto indicato
> all'interno del capitolo "*Catalogo -- Gestione Articoli -- Articoli
> -- Anagrafica Articolo / Servizio -- Anagrafica Passweb --
> Spedizione*" di questo manuale

- Per quel che riguarda invece eventuali etichette personalizzate
  piuttosto che opzioni di consegna al piano, di preavviso telefonico,
  di consegna al sabato ecc... occorre sottolineare che lato Passweb
  questo tipo di informazione è legata al metodo di trasporto piuttosto
  che a eventuali spese accessorie e/o allo specifico pagamento
  selezionato dall'utente in fase di checkout. Lato Qaplà l'effettiva
  gestione di queste informazioni dipende invece dallo specifico
  corriere che verrà poi utilizzato per gestire la spedizione.

> In sostanza dunque, su Passweb, in fase di configurazione di un metodo
> di trasporto piuttosto che di una spesa accessoria o di un pagamento
> sarà possibile definire anche eventuali informazioni aggiuntive da
> passare a Qaplà per la gestione della spedizione nel momento in cui
> l'utente dovesse effettivamente selezionare per il proprio ordine
> quella specifica modalità di trasporto, quella specifica spesa
> accessoria e/o quello specifico pagamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_11.bmp](./assets/media/image133.png)

> **ATTENZIONE!** Come indicato, lato Qaplà, la gestione di queste
> informazioni dipenderà invece dal corriere effettivamente utilizzato
> per gestire la spedizione (al momento solo BRT o GLS) per cui le
> informazioni passate da Passweb verranno effettivamente visualizzate
> nel back end di Qaplà solo nel momento in cui si dovesse scegliere di
> effettuare la spedizione con uno dei corrieri in grado di gestire
> quella specifica informazione
>
> Per maggiori informazioni relativamente a come poter associare ad un
> determinato metodo di trasporto piuttosto che ad una spesa accessoria
> o ad un pagamento informazioni aggiuntive sulla spedizione di Qaplà,
> si veda anche quanto indicato nei relativi capitoli di questo manuale
> (es. "*Ordini -- Metodi di Trasporto -- Trasporti di tipo Passweb --
> Qaplà*")

##### GESTIONE NUMBER TRACKING

Nel momento in cui si dovesse decidere di attivare l'integrazione
Passweb -- Qaplà utilizzando quindi la piattaforma terza per la gestione
delle spedizioni, sarà poi Qaplà stesso a preoccuparsi di inserire nel
dettaglio dell'ordine visualizzabile sul sito Ecommerce il number
tracking e il link di collegamento alla specifica pagina web in cui
l'utente potrà monitorare lo stato della sua spedizione.

**ATTENZIONE!** Per consentire a Qaplà di inserire nel dettaglio del
documento Passweb il number Tracking della relativa spedizione è di
fondamentale importanza configurare correttamente, sulla piattaforma
terza, i relativi Webhook (si veda quanto indicato in merito nel
precedente capitolo "Integrazione Passweb -- Qaplà")

Sfruttando dunque i WebHook precedentemente configurati, quando su Qaplà
verrà creata, a partire da un determinato ordine la relativa spedizione,
Qaplà stesso, in maniera completamente automatica, comunicherà al sito
Ecommerce la nuova condizione **inserendo sul relativo documento
Passweb:**

- la sigla del corriere utilizzato (es. BRT)

- il Tracking Number assegnato all'ordine direttamente su Qaplà (es.
  987654321987)

- il link di collegamento alla tracking page personalizzata (Segui la
  spedizione) gestibile direttamente dalla piattaforma Qaplà e
  all'interno della quale l'utente potrà controllare in ogni momento lo
  stato esatto della sua spedizione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\qapla_7.bmp](./assets/media/image134.png)

**ATTENZIONE!** Impostando in fase di configurazione del sito anche al
chiave pubblica di Qaplà, il link di tracciamento della spedizione verrà
visualizzato su Passweb non appena il sito avrà ricevuto la
corrispondente chiamata Webhook.

In questa fase la spedizione potrebbe ancora non essere effettivamente
presente su Qaplà **per cui potrebbero verificarsi situazioni in cui,
per un breve lasso di tempo, cliccando sul link di tracciamento l'utente
ottenga come risposta da Qaplà che la spedizione in questione non è
ancora presente.**

Altra cosa di fondamentale importanza da tenere in considerazione
inoltre, è che nel momento in cui si dovesse decidere di gestire le
spedizioni tramite Qaplà il fatto di aver configurato o meno alla pagina
**"Configurazione Ordini"** del Wizard un determinato attributo per
gestire il tracking number (parametro "**Attributo del Number
Tracking**") non verrà poi preso in considerazione

In queste condizioni infatti l'assegnazione del Tracking Number e il
link di collegamento alla pagina di tracciamento della spedizione
verranno gestiti direttamente da Qaplà e sarà Qaplà stessa ad inserire
automaticamente queste informazioni sull'ordine Passweb.

**ATTENZIONE! Allo stato attuale il Tracking Number inserito da Qaplà
sul documento Passweb non viene trasferito in Mexal.**

Se l'esigenza dovesse quindi essere quella di avere anche sul documento
Mexal l'indicazione del Tracking Number tale informazione andrà poi
inserita in maniera manuale.

Infine, nel caso in cui si decida di gestire tutte le comunicazioni
relative alla spedizione direttamente da Qaplà, è consigliabile,
ovviamente, disattivare le analoghe comunicazioni (mail di evasione)
gestite direttamente da Passweb e/o da MailChimp in maniera tale da non
inviare più volte al cliente lo stesso tipo di comunicazione.

