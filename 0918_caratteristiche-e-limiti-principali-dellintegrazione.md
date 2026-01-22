# CARATTERISTICHE E LIMITI PRINCIPALI DELL'INTEGRAZIONE



- Allo stato attuale l'integrazione prevede la gestione delle seguenti
  tipologie di prodotti Prestashop:

  - **Simple Product**

  - **Configurable Product**

> corrispondenti, di base, ad articoli Mexal di tipo A semplici, a
> confezione, a taglie / colori, e/o strutturati (articoli figlio). Non
> sono quindi gestiti Campionari, DBA ...

- A livello di dati articolo lo scambio di informazioni tra Passweb e
  Magento può avvenire via API oppure mediante la creazione e lo scambio
  di appositi file CSV. A livello di importazione ordini invece
  l'integrazione Passweb -- Magento può avvenire unicamente via API.

> In ogni caso se si dovesse optare per una pubblicazione articoli via
> API (considerando le limitazioni del caso) o si dovesse decidere di
> attivare e gestire anche l'importazione ordini da Magento verso il
> gestionale Passepartout sarà di fondamentale importanza verificare il
> corretto funzionamento delle API Magento. Nel momento in cui, infatti,
> tali API non dovessero essere contattabili in maniera corretta o
> dovessero ritornare degli errori il processo di integrazione
> risulterebbe compromesso.
>
> **Tali problemi vanno necessariamente risolti lato Magento e in questo
> senso Passepartout non fornisce alcun tipo di assistenza**

- Considerando quanto indicato al punto precedente il Connettore
  potrebbe non essere compatibile con eventuali servizi Cloudflare (o
  simili) presenti sulla piattaforma terza. Il trasferimento dati
  richiede infatti che venga mantenuta aperta e attiva una connessione
  tra il Connettore Passweb e la piattaforma terza per tutto il tempo
  necessario al trasferimento delle informazioni. Servizi come
  Cloudflare potrebbero invece, per loro stessa natura, interrompere
  questa connessione dopo un intervallo prestabilito di tempo impedendo,
  di fatto, il completamento delle operazioni e ritornando un apposito
  messaggio di Timeout

- Il processo di pubblicazione degli articoli sulla piattaforma terza
  dipende ovviamente, oltre che dalle elaborazioni interne a Passweb,
  anche dai tempi di risposta delle relative API.

> Ipotizzando un tempo di pubblicazione del singolo articolo attorno ai
> 5 secondi la pubblicazione di 1000 articoli impiegherebbe un tempo
> pari all\'incirca a 1.5 ore. Nel momento in cui i tempi di
> pubblicazione del singolo articolo dovessero raddoppiare passando a 10
> secondi la pubblicazione di 1000 articoli impiegherebbe all\'incirca
> un tempo pari a 3 ore.

- La chiamata API per la lettura dei prodotti gestita da Passweb
  utilizza un pageSize di 2000 (vengono quindi letti 2000 articoli alla
  volta). E' necessario quindi verificare che il corrispondente
  parametro Magento sia impostato su di un valore maggiore o uguale a
  2000.

- **Considerando che in fase di pubblicazione articoli via API si va ad
  agire direttamente sulle anagrafiche di prodotti presenti
  nell'ambiente di produzione della piattaforma terza, è buona norma
  effettuare backup periodici di queste informazioni, soprattutto nel
  momento in cui si dovesse decidere di gestire determinate informazioni
  direttamente da Magento, in maniera tale da poter poi facilmente
  ripristinare tali dati nel momento in cui dovessero verificarsi
  problemi o sovrascritture di dati indesiderate.**

- L'integrazione non prevede la creazione automatica di categorie
  merceologiche. Queste devono già essere presenti su Magento e devono
  poi essere mappate correttamente con le categorie presenti in Passweb
  (ed esportate dal gestionale). In assenza di mapping sulle categorie
  gli articoli possono passare correttamente su Magento ma risulteranno
  non associati a nessuna categoria e quindi potrebbero non essere
  visibili sul front end

- Dipendentemente dalle configurazioni settate per l'Account e per le
  Inserzioni di pubblicazione, le Categorie merceologiche definite sul
  gestionale Passepartout (o su Passweb) e le relative associazioni con
  i prodotti potranno andare o meno a sovrascrivere i corrispondenti
  dati presenti sulla piattaforma terza.

- L'integrazione non prevede la creazione di nuovi campi legati alle
  anagrafiche articolo di Magento. In determinate situazione
  l'integrazione può aggiungere valori a specifici elementi che, di base
  devono però essere già presenti sulla piattaforma terza.

- **In merito agli ordini acquisiti da Magento occorre sempre ricordare
  che il numero di decimali e le tipologie di arrotondamento in uso
  sulla piattaforma esterna potrebbero non coincidere con i decimali e
  gli arrotondamenti utilizzati dai gestionali Passepartout (il calcolo
  dell'IVA, ad esempio, è gestito direttamente da Mexal e non è
  possibile modificare o personalizzare questo tipo di algoritmo). In
  conseguenza di ciò potrebbero verificarsi situazioni in cui i totali
  del documento Magento differiscano di alcuni centesimi rispetto a
  quelli del documento gestionale**

- I campi SDI e PEC (come anche il campo relativo al codice fiscale)
  necessari per attivare la fatturazione elettronica sui gestionali
  Passepartout non sono campi standard di Magento per cui per poter
  gestire queste informazioni è necessario ricorrere a dei moduli
  aggiuntivi

> In questo senso, nella scelta del modulo da acquistare per gestire
> questo tipo di informazioni, è di fondamentale importanza ricordarsi
> che l'integrazione Passweb -- Magento si basa sulle API standard messe
> a disposizione da Magento stesso per cui **è assolutamente
> indispensabile che i campi SDI e PEC aggiunti dal modulo esterno siano
> poi accessibili in lettura / scrittura mediante queste stesse API**
> attraverso i metodi di seguito indicati:

- attributeMetadata/customer

- attributeMetadata/customer/custom

- attributeMetadata/customerAddress

- attributeMetadata/customerAddress/custom

> Nel caso in cui i campi Magento utilizzati per gestire SDI e PEC non
> siano accessibili tramite API Standard, Passweb non avrà modo di
> accedere a queste informazioni.

- Eventuali sconti presenti sul documento Magento verranno gestiti con
  l'inserimento nel documento gestionale di appositi articoli spesa a
  quantità -1 e con valore negativo

- Considerata l'impossibilità di agire via API sulle singole righe del
  documento Magento, l'evasione parziale di un singolo ordine non è
  gestita

- Il "Fatturare A" è gestito secondo le specifiche indicate all'interno
  del capitolo "*Marketplace -- Altri Marketplace -- Magento -- Codifica
  automatica di nuove anagrafiche utente -- Fatturare a*" di questo
  manuale

- Nel momento in cui si dovesse decidere di gestire le immagini dei
  prodotti dal relativo gestionale Passepartout queste potrebbero,
  dipendentemente da come verranno poi configurate le Inserzioni
  utilizzate per la pubblicazione, andare a sostituire eventuali
  immagini già presenti su Magento.

> **In tal senso si consiglia di non adottare mai una gestione mista**
> (alcune immagini sul gestione e altre caricate direttamente sulla
> piattaforma terza).
>
> Allo stesso modo una volta importate le immagini dal gestionale queste
> non dovrebbero poi essere cambiate di posizione operando direttamente
> all'interno di Magento.
>
> **ATTENZIONE! Nel momento in cui non dovesse essere rispettato quanto
> sopra indicato in fase di pubblicazione delle immagini articolo si
> potrebbero verificare sovrascritture e / o eliminazioni indesiderate
> delle risorse attualmente presenti su Magento**
>
> Se la logica adottata da Passweb non dovesse essere adatta a
> soddisfare le esigenze del caso, e si dovesse quindi decidere di
> gestire le immagini articolo dalla piattaforma terza sarà allora
> necessario verificare di non avere inserito le immagini lato
> gestionale o, in alternativa, di aver correttamente selezionato, in
> fase di configurazione dell'Account di integrazione, il parametro
> "**Escludi Feed Immagini**" (sezione "**Articoli**") in maniera tale
> da inibire completamente la trasmissione di questo tipo di risorse dal
> gestionale Passepartout verso la piattaforma terza
>
> **ATTENZIONE!** La gestione delle immagini articolo direttamente sul
> gestionale potrebbe, per ovvie ragioni, rallentare il processo di
> pubblicazione (via API) degli articoli. **Laddove possibile è
> auspicabile quindi gestire queste immagini direttamente sulla
> piattaforma terza**

- Non è gestito un processo diretto di acquisizione delle anagrafiche
  cliente da Magento verso Mexal. Allo stesso modo non è gestita
  l\'esportazione diretta dei clienti presenti nelle anagrafiche del
  gestionale verso la piattaforma terza.

- Eventuali nuove anagrafiche utente verranno create all\'interno del
  corrispondente gestionale Passepartout solo in fase di importazione
  ordini prelevando i dati necessari (indirizzo di fatturazione,
  indirizzo di spedizione \...) direttamente dalle informazioni presenti
  sull'ordine acquisito

- La distinzione tra Utente Privato e Utente Azienda avverrà sulla base
  del campo Magento presente nell' indirizzo di fatturazione (Billing
  Address) e utilizzato per gestire la partita IVA (campo VAT)

