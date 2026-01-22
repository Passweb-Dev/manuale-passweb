# 3 -- ACQUISTO DELLA GIFT CARD (TRATTAMENTO O RICARICA PROMOZIONE) SUL FRONT END DEL SITO



Sulla base di quanto indicato nel precedente capitolo di questo manuale,
dovrebbe ormai essere evidente che l'acquisto di una Gift Card di tipo
HoReCa (ossia l'acquisto di un Trattamento e/o di un articolo di tipo
"Ricarica Promozione"), se portato a termine, e quindi pagato, in
maniera corretta **porterà sempre alla creazione, in Beauty, di un
corrispondente "Buono Sconto"** che poi, a seconda dei casi, potrà
essere utilizzato solo per il pagamento di un determinato Trattamento
oppure per pagare interamente o anche solo parzialmente un Trattamento
qualsiasi.

Nello specifico dunque, a fronte dell'inserimento sul gestionale di un
ordine web contenente l'acquisto di un Trattamento verrà generato su
Beauty, in maniera completamente automatica, un nuovo Buono Sconto:

- relativo al trattamento acquistato **(1)** -- (pulsante "**Avanzate**"
  nella maschera di dettaglio del Buono Sconto per accedere maschera
  "**Dati ulteriori buono sconto**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_buono_sconto_beauty.bmp](./assets/media/image346.png){width="5.695138888888889in"
height="3.2729166666666667in"}

- con importo (**ivato**) pari all'importo del Trattamento stesso
  **(2)**

> **ATTENZIONE!** L'importo del Buono Sconto creato su Beauty è sempre
> iva inclusa

- con scadenza determinata da quanto impostato in fase di configurazione
  della Gift Card HoReCa all'interno del campo "Durata (giorni)" **(3)**

- con Serie e Codice determinati sulla base di quanto impostato, lato
  gestionale, in fase di configurazione del codice a barre in uso ai
  Buoni Sconto **(4)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_buono_sconto_beauty_2.bmp](./assets/media/image347.png){width="4.071527777777778in"
height="1.7659722222222223in"}

A fronte invece dell'inserimento sul gestionale di un ordine web
contenente l'acquisto di un articolo di tipo "Ricarica Promozione" verrà
generato su Beauty, in maniera completamente automatica, un nuovo Buono
Sconto

- non associato a specifici articoli **(1) -** (pulsante "**Avanzate**"
  nella maschera di dettaglio del Buono Sconto per accedere maschera
  "**Dati ulteriori buono sconto**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_buono_sconto_beauty_3.bmp](./assets/media/image348.png){width="5.643055555555556in"
height="3.3444444444444446in"}

- con importo (**ivato**) pari al valore (ivato) della ricarica
  acquistata **(2)**

> **ATTENZIONE!** Anche in questo caso l'importo del Buono Sconto creato
> su Beauty è sempre iva inclusa

- con scadenza determinata da quanto impostato in fase di configurazione
  della Gift Card HoReCa all'interno del campo "Durata (giorni)" **(3)**

- con Serie e Codice determinati sulla base di quanto impostato, lato
  gestionale, in fase di configurazione del codice a barre in uso ai
  Buoni Sconto **(4)**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_buono_sconto_beauty_4.bmp](./assets/media/image349.png){width="4.071527777777778in"
height="1.7659722222222223in"}

In entrambi i casi il campo "Cliente" presente nella maschera di
configurazione del Buono Sconto verrà valorizzato, ovviamente, con il
nominativo dell'utente che ha effettuato l'acquisto sul web.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_12.bmp](./assets/media/image350.png){width="4.071527777777778in"
height="1.7659722222222223in"}

**ATTENZIONE!** Il fatto che nel campo "Cliente" del Buono Sconto sia
indicato l'utente che ha effettuato l'acquisto sul web non significa che
il Buono Sconto in questione potrà essere utilizzato solo da
quell'utente.

**Ciò che determina infatti la possibilità di utilizzare, almeno
all'interno del sito, un determinato Buono Sconto è il codice della Gift
Card di tipo HoReCa**, codice questo che coincide esattamente con il
Codice a barre del corrispondente Buono Sconto generato su Beauty e che
potrà essere visualizzato anche sul Wizard di Passweb all'interno della
pagina "*Utenti -- Gift Card -- Codici*"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_13.bmp](./assets/media/image351.png){width="5.370138888888889in"
height="3.292361111111111in"}

**ATTENZIONE!** i codici relativi alla Gift Card di tipo Ho.Re.Ca sono
creati in maniera completamente automatica solo ed esclusivamente a
fronte dell'inserimento nel gestionale di un ordine contenente
l'acquisto di un Trattamento o di una Ricarica Promozione e quindi solo
dopo la creazione del relativo Buono Sconto Beauty.

**Non è quindi possibile creare in maniera manuale, operando
direttamente dal Wizard di Passweb, codici di Gift Card di tipo HoReCa**

In sostanza dunque una volta creato il Buono Sconto, Beauty provvederà a
comunicare a Passweb il relativo codice a barre (campo "**Codice a
barre**" nella maschera di configurazione del Buono Sconto) e solo a
questo punto Passweb avrà a disposizione tutte le informazioni
necessarie poter creare, a sua volta, il Codice Gift Card, per poterlo
attivare e per poterlo inserire tra quelli presenti all'interno della
maschera precedentemente evidenziata.

Creato il Codice Gift Card Passweb si preoccuperà poi di inserirlo anche
nella mail di Attivazione (posto che nel template di questa mail sia
stato correttamente inserito il relativo segnaposto) e di inviare
all'acquirente questa stessa mail.

Una volta ottenuto il Codice Gift Card, l'utente potrà quindi decidere
di utilizzarlo, nei tempi e nei modi corretti, per se stesso ad esempio
in fase di pagamento della prenotazione via web di un determinato
Trattamento.

D'altra parte nulla vieta che un determinato Trattamento possa essere
acquistato con l'intenzione di regalarlo poi a qualcun altro.

In questo caso una volta ottenuto il Codice Gift Card l'acquirente non
dovrà far altro che far pervenire questo stesso codice, secondo le
modalità e i canali da lui ritenuti più opportuni (mail, sms, biglietto
regalo ...), a chi ne dovrà effettivamente beneficiare.

**ATTENZIONE! l'invio del Codice Gift Card all'effettivo beneficiario è
a carico dell'acquirente e non può essere effettuato in maniera
automatica da Passweb**

Per maggiori informazioni relativamente a come poter effettivamente
utilizzare un Codice Gift Card in fase di pagamento della prenotazione
di un Trattamento si veda anche quanto indicato nel successivo capitolo
di questo manuale.

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
gestire delle informazioni aggiuntive sull'acquisto di un Trattamento o
di una Ricarica Promozione, come potrebbe essere, ad esempio, il
nominativo della persona a cui destinare il relativo Codice Sconto e/o
un eventuale nota sarà necessario attivare per quel tipo di trattamento
e/o per quel tipo di ricarica promozione il modulo aggiuntivo delle
Custom Option

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_14.bmp](./assets/media/image352.png){width="5.370138888888889in"
height="3.292361111111111in"}

In queste condizioni eventuali informazioni aggiuntive verranno inserite
nel corpo del relativo documento gestionale (secondo le normali modalità
di gestione delle Custom Option) e anche nel campo "Descrizione"
presente nella maschera del Buono Sconto Beauty generato a seguito
dell'acquisto di quel determinato Trattamento o di quella determinata
Ricarica Promozione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_15.bmp](./assets/media/image353.png){width="3.2465277777777777in"
height="2.1951388888888888in"}

Per maggiori informazioni relativamente all'utilizzo delle Custom Option
si veda quanto indicato nel relativo capitolo di questo manuale
("*Catalogo -- Opzioni Articoli*")

Un'ultima considerazione di fondamentale importanza da fare riguarda poi
la modalità di acquisto che dovrà essere effettivamente attivata sul
sito in relazione ai Trattamenti e alle Ricariche Promozionali.

Sulla base di quanto detto fino a questo momento è ormai chiaro infatti
che l'inserimento su Beauty di un ordine web contenente questo tipo di
prodotto e la conseguente creazione del relativo buono sconto genererà
poi anche la creazione, lato Passweb, dei relativi codici Gift Card e il
loro invio (tramite mail di Attivazione) ai relativi acquirenti, i quali
una volta in possesso di questi codici potranno immediatamente
utilizzarli all'interno del sito per usufruire dei relativi sconti.

**In questo senso dunque è di fondamentale importanza essere certi che
gli ordini inseriti nel gestionale siano stati correttamente pagati e
per far questo sarà necessario accertarsi che le uniche modalità di
pagamento effettivamente attive per i Trattamenti e/o per le Ricariche
Promozionali siano mediante Carta di Credito**

In caso contrario potrebbero anche verificarsi situazioni in cui un
utente si possa trovare ad utilizzare un Buono Sconto prima ancora di
averne effettivamente pagato l'importo.

Inoltre occorre anche tenere ben presente che, **lato gestionale,
possono esserci dei problemi nel momento in cui si tenti di fiscalizzare
un unico ordine contenente sia Trattamenti che articoli di tipo
"Ricarica Promozione"**

In conseguenza di tutto ciò sarà necessario considerare le seguenti
casistiche:

- se la configurazione del sito **dovesse prevedere unicamente
  l'acquisto (oltre che la prenotazione) di Trattamenti** sarà
  sufficiente verificare che le sole modalità di pagamento
  effettivamente attive sul sito siano mediante Carta di Credito.

- se la configurazione del sito **dovesse prevedere l'acquisto sia di
  Trattamenti che di articoli di tipo "Ricarica Promozione" occorrerà
  attivare la gestione delle Linee Articolo** creando, nello specifico,
  2 linee distinte, una per i Trattamenti e una per le "Ricariche
  Promozione".

> In questo modo, se necessario, sarà poi possibile spezzare l'acquisto
> in più ordini differenti contenenti solo Trattamenti e solo "Ricariche
> Promozione" evitando così problemi di fiscalizzazione dei relativi
> Buoni Sconto
>
> In questo caso inoltre sarà anche necessario verificare che le sole
> modalità di pagamento effettivamente attive sul sito siano mediante
> Carta di Credito

- se la configurazione del sito **dovesse prevedere l'acquisto
  contemporaneo di Trattamenti, Ricariche Promozioni e anche Articoli
  "tradizionali"** (pagabili quindi anche con modalità diverse dalla
  carta di credito) **occorrerà attivare la gestione delle Linee
  Articolo creando, nello specifico, 3 distinte linee**, una per i
  Trattamenti, una per le Ricariche Promozione una per gli Articoli
  tradizionali.

> In questo caso inoltre sarà necessario verificare anche di aver
> attivato per le linee relative ai Trattamenti e alle Ricariche
> Promozione solamente pagamenti online mentre per le Linea relativa
> agli articoli tradizionali sarà possibile attivare anche altre
> modalità di pagamento

Infine, come per le Gift Card Virtuali, un ordine contenente unicamente
l'acquisto di un Trattamento o di una Ricarica Promozione non necessita,
ovviamente, di spedizioni di alcun tipo per cui in fase di Checkout la
sezione relativa alla selezione della modalità di spedizione verrà
automaticamente nascosta.

