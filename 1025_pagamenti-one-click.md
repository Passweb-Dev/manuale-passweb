# PAGAMENTI ONE CLICK



Oltre alla modalità "tradizionale" esaminata nel precedente capitolo di
questo manuale, l'integrazione Passweb -- Nexi consente anche di
configurare il pagamento in maniera tale che l'utente abbia la
possibilità di memorizzare le proprie carte di credito così da poter
concludere più rapidamente l'ordine senza dover ogni volta digitare
tutti i dati della propria carta

Per far questo sarà necessario:

- Impostare il parametro "**Soluzione**" sull'opzione "**Pagamento
  Semplice / One Click**"

- Impostare, secondo quanto indicato nel precedente capitoli di questo
  manuale, i parametri presenti all'interno della sezione "**Pagamento
  Semplice**"

- Impostare in maniera corretta anche i parametri di configurazione
  presenti all'interno della sezione "**Pagamento One Click**"

**ATTENZIONE!** per attivare questa modalità di pagamento non è
sufficiente impostare i parametri della sezione "Pagamenti One Click" ma
vanno impostati in maniera corretta anche quelli della sezione
"Pagamento Semplice"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nexi_pagamento_one_click.bmp](./assets/media/image126.png){width="5.565277777777778in"
height="3.825in"}

Nello specifico per quel che riguarda la sezione "Pagamento One Click" i
parametri "**Alias**" , "**Chiave** **Segreta**" e "**Gruppo**"
consentiranno di impostare i relativi codici di attivazione forniti
(come per il pagamento semplice) direttamente dalla banca all'esercente
all'atto dell'adesione allo specifico servizio.

**ATTENZIONE!** A differenza dei parametri presenti all'interno della
sezione "Pagamento Semplice" (obbligatori per poter attivare
correttamente il pagamento online), **quelli presenti nella sezione
"Pagamento One Click"** **non sono dati obbligatori** e possono essere
inseriti solo ed esclusivamente nel caso in cui l'amministratore del
sito decida di abilitare in maniera specifica la relativa opzione.

Una volta valorizzati correttamente i campi sopra evidenziati, nel
momento in cui l'utente in fase di checkout andrà a selezionare, la
prima volta, la modalità di pagamento in oggetto gli verrà proposta
anche l'opzione memorizzare i dati della carta che andrà poi ad
utilizzare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nexi_pagamento_ricorrente_2.bmp](./assets/media/image127.png){width="4.980555555555555in"
height="3.0131944444444443in"}

**ATTENZIONE! La memorizzazione dei dati sensibili avviene solo ed
esclusivamente sul sito della banca e NON sul sito Passweb.**

Al completamento della transazione il gateway della banca memorizzerà
quindi i dati della carta di credito utilizzata.

In queste condizioni quando lo stesso utente effettuerà un nuovo ordine
all'interno del sito Ecommerce selezionando, in fase di checkout, il
pagamento Nexi potrà scegliere se pagare con una delle carte di credito
precedentemente memorizzate oppure se utilizzare una nuova carta non
ancora presente tra quelle in elenco.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carta_si_pagamento_ricorrente_3.bmp](./assets/media/image128.png){width="4.980555555555555in"
height="2.954861111111111in"}

Nel caso in cui decida di utilizzare una nuova carta la procedura per il
completamente dell'ordine sarà in tutto e per tutto analoga a quella
precedentemente descritta.

Nel caso in cui l'utente decida invece di utilizzare una delle carte
precedentemente memorizzate, una volta reindirizzato sul sito della
banca l'unico dato da inserire per completare il pagamento sarà quello
relativo al codice CVV della carta stessa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carta_si_pagamento_ricorrente_4.bmp](./assets/media/image129.png){width="4.980555555555555in"
height="2.954861111111111in"}

**NOTA BENE**: Nexi XPay gestisce solamente importi in euro; per
eventuali ordini in valuta il totale del documento verrà quindi
opportunamente convertito in euro e passato alla banca.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office di Nexy potrebbe non
essere allineato con la corrente versione di tale software. Si consiglia
quindi di utilizzare la specifica manualistica reperibile dal sito della
banca.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà CartaSì occorre rivolgersi alla relativa assistenza.

