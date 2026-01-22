# CARATTERISTICHE E LIMITI PRINCIPALI DELL'INTEGRAZIONE



- Allo stato attuale l'integrazione prevede la gestione delle seguenti
  tipologie di prodotti Prestashop:

  - Prodotti Semplici

  - Prodotti con combinazioni

> corrispondenti, di base, ad articoli Mexal di tipo A semplici, a
> confezione, a taglie / colori, e/o strutturati (articoli figlio). Non
> sono quindi gestiti Campionari, DBA ...

- A livello di dati articolo lo scambio di informazioni tra Passweb e
  Prestashop può avvenire via API oppure mediante la creazione e lo
  scambio di appositi file CSV. A livello di importazione ordini invece
  l'integrazione Passweb -- Prestashop può avvenire unicamente via API.

> In ogni caso se si dovesse optare per una pubblicazione articoli via
> API (considerando le limitazioni del caso) o si dovesse decidere di
> attivare e gestire anche l'importazione ordini da Prestashop verso il
> gestionale Passepartout sarà di fondamentale importanza verificare il
> corretto funzionamento delle API Prestashop. Nel momento in cui,
> infatti, tali API non dovessero essere contattabili in maniera
> corretta o dovessero ritornare degli errori il processo di
> integrazione risulterebbe compromesso.
>
> **Tali problemi vanno necessariamente risolti lato Prestashop e in
> questo senso Passepartout non fornisce alcun tipo di assistenza**

- Considerando quanto indicato al punto precedente il Connettore
  potrebbe non essere compatibile con eventuali servizi Cloudflare (o
  simili) presenti sulla piattaforma terza. Il trasferimento dati via
  API richiede infatti che venga mantenuta aperta e attiva una
  connessione tra il Connettore Passweb e la piattaforma terza per tutto
  il tempo necessario al trasferimento delle informazioni. Servizi come
  Cloudflare potrebbero invece, per loro stessa natura, interrompere
  questa connessione dopo un intervallo prestabilito di tempo impedendo,
  di fatto, il completamento delle operazioni e ritornando un apposito
  messaggio di Timeout

- Il processo di pubblicazione degli articoli via API dipende
  ovviamente, oltre che dalle elaborazioni interne a Passweb, anche dai
  tempi di risposta delle relative API.

> Ipotizzando un tempo di pubblicazione del singolo articolo attorno ai
> 5 secondi la pubblicazione di 1000 articoli impiegherebbe un tempo
> pari all\'incirca a 1.5 ore. Nel momento in cui i tempi di
> pubblicazione del singolo articolo dovessero raddoppiare passando a 10
> secondi la pubblicazione di 1000 articoli impiegherebbe all\'incirca
> un tempo pari a 3 ore.

- **Considerando che in fase di pubblicazione articoli via API si va ad
  agire direttamente sulle anagrafiche di prodotti presenti
  nell'ambiente di produzione della piattaforma terza, è buona norma
  effettuare backup periodici di queste informazioni (mediante ad
  esempio le apposite funzioni Prestashop di export dati in csv),
  soprattutto nel momento in cui si dovesse decidere di gestire
  determinate informazioni direttamente da Prestashop, in maniera tale
  da poter poi facilmente ripristinare tali dati nel momento in cui
  dovessero verificarsi problemi o sovrascritture di dati
  indesiderate.**

- L'integrazione non prevede la creazione automatica di categorie
  merceologiche. Queste devono già essere presenti su Prestashop e
  devono poi essere mappate correttamente con le categorie presenti in
  Passweb (ed esportate dal gestionale). In assenza di mapping sulle
  categorie gli articoli possono passare correttamente su Prestashop ma
  risulteranno non associati a nessuna categoria e quindi potrebbero non
  essere visibili sul front end

- Dipendentemente dalle configurazioni settate per l'Account e per le
  Inserzioni di pubblicazione, le Categorie merceologiche (primarie e
  secondarie) definite sul gestionale Passepartout (o su Passweb) e le
  relative associazioni con i prodotti potranno andare o meno a
  sovrascrivere i corrispondenti dati presenti sulla piattaforma terza.

- L'integrazione non prevede la creazione di nuovi campi (es. Features)
  legati alle anagrafiche articolo Prestashop. Tali campi devono già
  essere presenti su Prestashop. In determinate situazione
  l'integrazione può aggiungere valori a questi elementi ma di base si
  limita ad agganciare elementi e valori che devono essere già presenti
  (nelle diverse lingue) su Prestashop. L'aggancio avviene indicando
  esattamente lo stesso valore già presente sulla piattaforma terza.

- **In merito agli ordini acquisiti da Prestashop occorre sempre
  ricordare che il numero di decimali e le tipologie di arrotondamento
  in uso sulla piattaforma esterna potrebbero non coincidere con i
  decimali e gli arrotondamenti utilizzati dai gestionali Passepartout
  (il calcolo dell'IVA, ad esempio, è gestito direttamente da Mexal e
  non è possibile modificare o personalizzare questo tipo di algoritmo).
  In conseguenza di ciò potrebbero verificarsi situazioni in cui i
  totali del documento Prestashop differiscano di alcuni centesimi
  rispetto a quelli del documento gestionale**

- I campi SDI e PEC necessari per attivare la fatturazione elettronica
  sui gestionali Passepartout non sono campi standard di Prestashop per
  cui è assolutamente indispensabile che tali campi, se gestiti, possano
  poi essere accessibile in lettura / scrittura mediante API standard e,
  nello specifico, mediante una delle seguenti Risorse

  - Addresses

  - Customers

> Nel caso in cui i campi Prestashop utilizzati per gestire SDI e PEC
> non siano accessibili tramite API Standard, Passweb non avrà modo di
> accedere a queste informazioni.

- Eventuali sconti presenti sul documento Prestashop verranno gestiti
  con l'inserimento nel documento gestionale di appositi articoli spesa
  a quantità -1 e con valore negativo

- Considerata l'impossibilità di agire via API sulle singole righe del
  documento Prestashop, l'evasione parziale di un singolo ordine non è
  gestita

- Il "Fatturare A" è gestito secondo le specifiche indicate all'interno
  del capitolo "*Marketplace -- Altri Marketplace -- Prestashop --
  Codifica automatica di nuove anagrafiche utente -- Fatturare a*" di
  questo manuale

- L'associazione e l'aggiornamento delle immagini articolo da Passweb a
  Prestashop, richiede la pubblicazione via API e funziona in maniera
  posizionale. In altri termini dunque l'immagine prodotto prelevata dal
  gestionale sarà la prima immagine associata in Prestashop al relativo
  articolo; la prima immagine secondaria eventualmente prelevata da
  gestionale sarà la seconda immagine associata su Prestashop e via di
  seguito.

> In considerazione di ciò **si consiglia di non adottare mai una
> gestione mista** (alcune immagini sul gestionale e altre caricate
> direttamente da Prestashop).
>
> Allo stesso modo una volta importate le immagini dal gestionale queste
> non dovrebbero poi essere cambiate di posizione operando direttamente
> all'interno di Prestashop
>
> **ATTENZIONE! Nel momento in cui non dovesse essere rispettato quanto
> sopra indicato in fase di pubblicazione delle immagini articolo si
> potrebbero verificare sovrascritture e / o eliminazioni indesiderate
> delle risorse attualmente presenti su Prestashop**
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
  cliente da Prestashop verso il gestionale Passepartout. Allo stesso
  modo non è gestita l\'esportazione diretta dei clienti presenti nelle
  anagrafiche del gestionale verso la piattaforma terza.

- Eventuali nuove anagrafiche utente verranno create all\'interno del
  corrispondente gestionale Passepartout solo in fase di importazione
  ordini prelevando i dati necessari (indirizzo di fatturazione,
  indirizzo di spedizione \...) direttamente dalle informazioni presenti
  sull'ordine acquisito

- La distinzione tra Utente Privato e Utente Azienda avverrà sulla base
  del campo Prestashop presente nell' indirizzo di fatturazione e
  utilizzato per gestire la partita IVA (campo "Numero IVA")

