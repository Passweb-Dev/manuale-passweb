# PAGAMENTI RICORRENTI



L'integrazione Passweb -- Nexi offre la possibilità di attivare anche
dei pagamenti ricorrenti che possono essere utilizzati, ad esempio, per
la vendita all'interno del sito di servizi in abbonamento.

In questo caso vanno però fatte immediatamente alcune considerazioni di
fondamentale importanza.

Nello specifico è bene sottolineare che:

- **Passweb gestisce solamente il primo pagamento della serie dei
  pagamenti ricorrenti (quello che di fatto attiva il servizio). Tutti i
  pagamenti successivi al primo, così come eventuali disdette, dovranno
  essere gestiti esternamente a Passweb utilizzando le API messe a
  disposizione da Nexi oppure configurando il tutto direttamente
  all'interno del backend di Nexi stesso**

> **ATTENZIONE!** per maggiori informazioni relativamente a come poter
> gestire all'interno del backend di Nexi i pagamenti ricorrenti si
> consiglia di fare riferimento alla documentazione del relativo portale
> essendo questa un'operazione completamente esterna a Passweb

- In conseguenza di quanto indicato al punto precedente tutti i
  pagamenti successivi al primo verranno visualizzati solo sul
  backoffice di Nexi e, in caso di cambio carta di credito, dovrà essere
  fatta nuovamente la procedura di acquisto del servizio partendo dal
  sito.

- Ogni pagamento ricorrente gestito da Nexi comporta la creazione,
  all'interno dell'ambiente di Nexi stesso, di un apposito contratto,
  con relativo numero identificativo (ovviamente univoco). Per poter
  gestire nel backoffice di Nexi i pagamenti ricorrenti successivi al
  primo sarà quindi indispensabile poter disporre del "Numero Contratto"
  creato in fase di attivazione del servizio

- Considerando che il primo pagamento, e quindi l'attivazione del
  servizio, verrà effettuato da Passweb, il "Numero Contratto"
  necessario per poter gestire i pagamenti successivi al primo dovrà
  essere inserito nell'ordine creato da Passweb e riportato poi sul
  gestionale

- **Tipicamente all'interno di Nexi dovrebbe essere creato un contratto
  differente per ogni servizio acquistato in modo tale che l'acquirente
  possa poi disdire, se necessario, un singolo abbonamento lasciandone
  invece attivi altri legati a servizi diversi da quello disdetto.** Per
  poter ottenere un risultato di questo tipo sarà quindi necessario
  configurare il sito in un certo modo, utilizzando (dipendentemente
  dalla tipologia di articoli venduti) le linee articolo, configurando
  se necessario due diversi pagamenti Nexi legati alle varie linee
  articolo che andremo a gestire e facendo anche in modo che ogni tutti
  servizi acquistabili con pagamenti ricorrenti possano effettivamente
  essere acquistati solo in quantità unitaria.

Fatte queste considerazioni di fondamentale importanza vediamo ora come
dover operare per poter gestire in maniera corretta, nell'integrazione
Passweb -- Nexi, i pagamenti ricorrenti.

La prima cosa da fare sarà sicuramente quella di impostare correttamente
i parametri di configurazione del gateway e in questo senso dovremo
quindi:

- Settare il parametro "**Soluzione**" presente alla pagina
  "**Configurazione del Metodo di Pagamento**" (tab "**Parametri
  Gateway**") sull'opzione "**Pagamento Ricorrente**"

- Settare in maniera corretta i parametri "**Alias**" e "**Chiave
  Segreta**" presenti all'interno della sezione "**Pagamento
  Ricorrente**" evidenziata in figura

![Videate\\nexi_pagamento_ricorsivo.bmp](./assets/media/image130.png)

> In questo senso, considerando che Passweb si occupa, come detto di
> gestire solo il primo pagamento **i valori da inserire all'interno dei
> campi Alias e Chiave Segreta saranno esattamente quelli che dovremmo
> inserire in corrispondenza di questi stessi campi nel caso di
> "Pagamenti Semplici"**
>
> Dal punto di vista tecnico, dunque, la differenza tra un "Pagamento
> Semplice" e un "Pagamento Ricorrente" sarà solamente la creazione
> all'interno di Nexi del contratto necessario per poter gestire poi
> tutti i pagamenti successivi al primo (operazione questa che, lo
> ricordiamo ancora una volta, dovrà essere gestita esternamente a
> Passweb).

A tal proposito il numero del contratto creato in Nexi a seguito
dell'acquisto di un servizio con pagamento ricorrente, numero questo
indispensabile, come detto, per poter gestire i pagamenti successivi al
primo mediate chiamate API (da realizzarsi esternamente a Passweb) o
direttamente dal backoffice di Nexi, potrà essere gestito in Passweb:

- Come segnaposto nella nota di testata dell'ordine su Mexal (campo
  "**Nota nuovo Ordine**" alla pagina "**Configurazione Parametri
  Ordine**" del Wizard )

![](./assets/media/image131.png)

> Utilizzando il segnaposto evidenziato in figura il codice contratto
> creato su Nexi verrà quindi riportato anche nella nota di testata
> dell'ordine inserito all'interno del gestionale

![](./assets/media/image132.png)

- Come segnaposto nel dettaglio documento (tab "**Documento**" alla
  pagina "**Configurazione Parametri Ordine**" del Wizard)

![](./assets/media/image133.png)

> Utilizzando il segnaposto evidenziato in figura il codice contratto
> creato su Nexi potrà quindi essere riportato anche nel dettaglio
> dell'ordine visualizzabile in area riservata, piuttosto che nel
> dettaglio dell'ordine presente nelle varie mail gestite da Passweb

- Come segnaposto per il parametro "**Dettaglio**" presente nella
  maschera di configurazione del pagamento

![](./assets/media/image134.png)

> Utilizzando il segnaposto evidenziato in figura il codice contratto
> creato su Nexi potrà quindi essere riportato anche nel dettaglio
> dell'ordine visualizzabile nella parte pubblica del sito

- nel dettaglio del documento visualizzabile direttamente all'interno
  del Wizard

![](./assets/media/image135.png)

- come campo presente nel tracciato record degli ordini esportati dal
  Wizard di Passweb

**ATTENZIONE!** il consiglio, in questo senso, è quello di inserire il
segnaposto "Numero Contratto Nexi" all'interno del campo "Nota nuovo
ordine" in maniera tale da avere disponibile questa informazione
direttamente all'interno del gestionale

Infine, un'ultima cosa di fondamentale importanza da tenere in
considerazione è, come già evidenziato, che all'interno di Nexi
tipicamente andrebbe creato un contratto differente per ogni servizio
acquistato in modo tale che l'acquirente possa poi disdire, se
necessario, un singolo abbonamento lasciandone invece attivi altri
legati a servizi diversi da quello disdetto.

Ora per poter ottenere un risultato di questo tipo sarà necessario:

- Gestire in maniera corretta le Linee Articolo.

> Nel momento in cui dovessero essere venduti all'interno del sito sia
> beni che servizi in abbonamento sarà di fondamentale importanza
> separare l'acquisto dei servizi dal quello dei prodotti utilizzando,
> per l'appunto, due diverse linee articolo. In queste condizioni sarà
> inoltre necessario gestire anche due diversi pagamenti, sempre legati
> a Nexi e, nello specifico: un "Pagamento Semplice" da utilizzare per
> la Linea Articolo dei prodotti e un "Pagamento Ricorrente" legato
> invece alla Linea Articolo dei servizi in abbonamento.
>
> Allo stesso modo nel caso in cui dovessero essere venduti servizi in
> abbonamento di tipo diverso, potrebbe essere necessario creare e
> gestire una distinta Linea Articolo per ognuno di essi

- Impostare sui servizi venduti in abbonamento (che dovranno comunque
  essere in Mexal articoli di tipo A) una quantità massima di vendita
  pari a 1, utilizzando per questo la funzionalità "**Quantità massima
  di vendita**" disponibile nelle videate aggiuntive articolo Mexal
  riservate a Passweb

![](./assets/media/image136.png)

> **ATTENZIONE!** per maggiori informazioni in merito alla funzionalità
> "Quantità massima di vendita" si veda quanto indicato all'interno del
> capitolo "*Configurazione -- Mexal Configurazione Gestionale --
> Attivazione Passweb -- Funzionalità Articoli -- Vendita Articoli per
> quantità massima*" di questo manuale.

- In realtà il fatto di importare per ogni singolo servizio venduto
  all'interno del sito una quantità massima di vendita parti ad 1 non ci
  mette completamente al sicuro in relazione al fatto che venga poi
  creato in Nexi un contratto per ogni singolo servizio acquistato.
  L'utente potrebbe infatti, in determinate condizioni, arrivare anche
  ad inserire in carrello due distinte righe dello stesso servizio
  (quindi della stessa Linea Articolo) e arrivare così a concludere un
  unico ordine con all'interno due distinti servizi in abbonamento
  creando però, all'interno di Nexi, un unico contratto.

> Per evitare il verificarsi di una situazione di questo tipo, sarà
> quindi di fondamentale importanza impostare anche il parametro
> "**Gestione articoli in carrello/wishlist**" presente alla pagina
> "**Configurazione Catalogo**" del Wizard sull'opzione "**Modifica riga
> articolo**"

![](./assets/media/image137.png)

> In queste condizioni infatti nel momento in cui l'utente dovesse
> cercare di inserire in carrello due volte lo stesso servizio, non
> verrebbero create due righe distinte ma si tenterebbe di andare a
> modificare la quantità in ordine dello stesso articolo già presente in
> carrello, portandola da 1 a 2 cosa questa che verrebbe a sua volta
> bloccata dal fatto di aver precedentemente impostato, per l'articolo
> in esame, una quantità massima di vendita pari a 1.

In definitiva dunque operando come appena indicato potremo avere la
certezza che per ogni singolo servizio in abbonamento acquistato
all'interno del sito venga poi generato, in Passweb, un relativo ordine
e di conseguenza anche un singolo codice contratto Nexi

