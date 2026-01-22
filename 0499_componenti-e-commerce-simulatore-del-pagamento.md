# COMPONENTI E-COMMERCE -- SIMULATORE DEL PAGAMENTO



Il Componente **"Simulatore del Pagamento"**

![](./assets/media/image592.png)

**può essere inserito unicamente all'interno del componente Ecommerce di
primo livello "Scheda Prodotto"** dove consente di mostrare all'utente
una possibile simulazione di rateizzazione collegata, ovviamente, al
prezzo dello specifico articolo e ad uno dei pagamenti rateali gestiti
da Passweb.

![](./assets/media/image593.png)

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata la sua maschera di gestione e
configurazione

![](./assets/media/image594.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Metodo di Pagamento:** consente di indicare la specifica modalità di
  pagamento rateale in relazione alla quale mostrare all'interno della
  scheda prodotto il relativo widget di simulazione.

> E' possibile selezionare uno dei seguenti valori:

- **Findomestic**: in questo caso verrà mostrato il widget di
  simulazione per la rateizzazione Findomestic.

> Nel caso specifico, all'interno della scheda prodotto, verrà inserita
> l'etichetta o l' immagine impostata mediante i successivi parametri.
> Cliccando su questi elementi verrà aperta la pagina di Findomestic
> dove poter effettuare le diverse possibili simulazioni di
> rateizzazione proposte in relazione al prezzo di acquisto dello
> specifico articolo.
>
> **ATTENZIONE!** Findomestic potrebbe applicare il finanziamento solo
> nel caso in cui il prezzo di acquisto del prodotto rientri un certo
> range. Nel momento in cui il prezzo dovesse essere minore o maggiore
> ai limiti di applicabilità imposti da Findomestic il widget in esame
> non verrà visualizzato

- **Clearpay**: in questo caso verrà mostrato il widget di simulazione
  per la rateizzazione proposta dalla piattaforma Clearpay.

> Nel caso specifico, all'interno della scheda prodotto, verrà inserita
> direttamente un etichetta con l'indicazione delle 4 rate proposte da
> Clearpay più un pop up informativo sulla procedura di acquisto
>
> **ATTENZIONE!** Clearpay potrebbe applicare il finanziamento solo nel
> caso in cui il prezzo di acquisto del prodotto rientri un certo range.
> Nel momento in cui il prezzo dovesse essere minore o maggiore ai
> limiti di applicabilità imposti da Findomestic il widget mostrerà un
> indicazione di quelli che sono i limiti di applicabilità del
> finanziamento

- **Soisy**: in questo caso verrà mostrato il widget di simulazione per
  la rateizzazione proposta dalla piattaforma Soisy.

> Nel caso specifico, all'interno della scheda prodotto, verrà inserita
> direttamente un' etichetta con l'indicazione delle rate proposte da
> Soisy più un pop up informativo sulla procedura di acquisto
>
> **ATTENZIONE!** Soisy potrebbe applicare il finanziamento solo nel
> caso in cui il prezzo di acquisto del prodotto rientri un certo range.
> Nel momento in cui il prezzo dovesse essere minore o maggiore ai
> limiti di applicabilità imposti da Soisy il widget in esame non verrà
> visualizzato

- **Scalapay**: in questo caso verrà mostrato il widget di simulazione
  per la rateizzazione proposta dalla piattaforma Scalapay.

> Nel caso specifico, all'interno della scheda prodotto, verrà inserita
> direttamente un' etichetta con l'indicazione delle rate proposte da
> Scalapay più un pop up informativo sulla procedura di acquisto
>
> **ATTENZIONE!** Scalapay potrebbe applicare il finanziamento solo nel
> caso in cui il prezzo di acquisto del prodotto rientri un certo range.
> Nel momento in cui il prezzo dovesse essere minore o maggiore ai
> limiti di applicabilità imposti da Scalapay il widget in esame non
> verrà visualizzato

- **PayPal Checkout**: in questo caso verrà mostrato il widget di
  simulazione per la rateizzazione proposta da PayPal

> **ATTENZIONE!** la rateizzazione in esame è relativa unicamente alla
> tipologia di pagamento PayPal Checkout
>
> Per maggiori informazioni in merito si rimanda a quanto indicato nella
> relativa sezione di questo manuale (*Ordini -- Metodi di Pagamento --
> PayPal Checkout*)
>
> **ATTENZIONE!** PayPal potrebbe applicare la rateizzazione solo nel
> caso in cui il prezzo di acquisto del prodotto rientri un certo range.
> Per maggiori informazioni relativamente alla possibilità di attivare
> il servizio di rateizzazione sul pagamento PayPal Checkout e alle
> relative condizioni di servizio è necessario fare riferimento a quanto
> indicato direttamente sul sito di PayPal

- **Pago Light**: in questo caso verrà mostrato il widget di simulazione
  per la rateizzazione proposta dalla piattaforma Pago Light.

> Nel caso specifico potrà essere visualizzato il simulatore standard di
> Pago Light o quello Pro, dipendentemente dai parametri di
> configurazione impostati per il relativo pagamento.
>
> Per maggiori informazioni in merito all'utilizzo del simulatore
> standard o pro si rimanda a quanto indicato all'interno del relativo
> capitolo di questo manuale ("*Ordini -- Metodi di Pagamento -- Pago
> Light -- Simulatore del pagamento*")
>
> **ATTENZIONE!** Pago Light offre la rateizzazione dell'importo solo
> nel caso in cui il prezzo di acquisto del prodotto rientri un certo
> range. Nel momento in cui il prezzo dovesse essere minore o maggiore
> ai limiti di applicabilità imposti dalla piattaforma terza il widget
> in esame non verrà visualizzato

- **Etichetta -- solo per pagamenti Findomestic:** consente di impostare
  l'etichetta sulla quale l'utente dovrà cliccare per aprire il widget
  di simulazione di Findomestic

- **Immagine / Immagine (rollover) -- solo per pagamenti Findomestic:**
  consente di impostare l'immagine (e quella che dovrà essere
  visualizzata al passaggio del mouse) su cui l'utente dovrà cliccare
  per aprire il widget di simulazione di Findomestic. Nel momento in cui
  dovesse essere impostata questa immagine essa avrà priorità rispetto
  all'etichetta che quini non verrà più visualizzata.

**ATTENZIONE!** Ovviamente affinché il simulatore possa funzionare in
maniera corretta è indispensabile aver configurato la relativa modalità
di pagamento. Inoltre, a seconda della modalità di pagamento
considerata, è indispensabile anche che il prezzo di acquisto dello
specifico articolo rientri effettivamente nel range di applicazione del
finanziamento stesso.

Per maggiori informazioni relativamente alla gestione dei pagamenti
rateali si rimanda a quanto indicato nei relativi capitoli di questo
manuale ("*Ordini -- Metodi di pagamento -- Findomestic / Clearpay /
Soisy ...*")

