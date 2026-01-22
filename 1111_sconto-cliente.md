# SCONTO CLIENTE



Utilizzando questo tipo di promozione è possibile definire, per i
clienti coinvolti, determinati sconti indipendentemente da quelli che
sono gli articoli che si andranno poi ad acquistare.

A differenza delle due promozioni precedentemente esaminate, in cui era
necessario definire non solo i clienti per i quali applicarle ma anche
gli specifici articoli coinvolti, **questo tipo di promozione è legata
solo ed esclusivamente ai clienti e verrà quindi applicata
indipendentemente da quelli che saranno poi gli articoli da essi
inseriti in carrello.**

La scheda "**Clienti Associati**" permette dunque di definire i singoli
clienti (Tabella "**Clienti attualmente associati**") o le singole
categorie clienti (Tabella "**Categoria Cliente**") coinvolte nella
Promozione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_19.bmp](./assets/media/image547.png)

Per poter definire il tipo di sconto che dovrà essere associato ai
clienti coinvolti è invece necessario utilizzare il parametro "**Tipo**"
presente all'interno della scheda "**Opzioni**" (sezione "**Opzioni
sconto cliente**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_20.bmp](./assets/media/image548.png)

E' possibile selezionare uno dei seguenti valori:

- **Formula:** permette di impostare uno sconto a valore per ogni tot
  euro di spesa. Ad esempio ogni 100 € di spesa verrà applicato uno
  sconto di 5,00€.

> In queste condizioni se, in fase di ordine all'interno del sito, il
> cliente dovesse raggiungere 150 € avrà diritto ad uno sconto di 5 €,
> se invece dovesse raggiungere 220 € di spesa allora avrà diritto ad
> uno sconto di 10 €
>
> La maschera "**Opzioni Sconto Cliente**" visualizzata automaticamente
> dopo aver impostato il campo "Tipo" sul valore in esame, oppure
> richiamabile mediante il pulsante "**Opzioni**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_21.bmp](./assets/media/image549.png)

> consente di definire nei dettagli la formula di applicazione dello
> sconto.

- **Incondizionato:** permette di impostare uno sconto in percentuale
  che verrà applicato al cliente in fase di ordine indipendentemente
  dalla spesa effettuata.

> La maschera "**Opzioni Sconto Cliente**" visualizzata automaticamente
> dopo aver impostato il campo "Tipo" sul valore in esame, oppure
> richiamabile mediante il pulsante "**Opzioni**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_22.bmp](./assets/media/image550.png)

> consente di definire (campo "**Sconto Incondizionato**" ) la
> percentuale di sconto che dovrà effettivamente essere applicata.
>
> **ATTENZIONE!** E' possibile inserire anche sconti a cascata (es.
> 10%+20%+30%)

- **Tabella:** permette di definire vari scaglioni di spesa e di
  associare a ciascuno di essi l'esatto sconto che dovrà essere
  applicato.

> La maschera "**Opzioni Sconto Cliente**" visualizzata automaticamente
> dopo aver impostato il campo "Tipo" sul valore in esame, oppure
> richiamabile mediante il pulsante "**Opzioni**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_23.bmp](./assets/media/image551.png)

> consente di definire (**Tabella Sconto**) gli scaglioni di spesa
> (campo "**Spesa da..**") ed il relativo sconto da applicare (campo
> "**Sconto**").
>
> Il campo "**Tipo Sconto**" presente all'interno di questa stessa
> maschera, consente invece di definire se, in tabella, andranno
> indicate le percentuali (opzione "**Percentuale**") oppure i valori
> dello sconto (opzione "**Valore**").

I tre parametri presenti nella parte bassa della maschera "**Opzioni
sconto cliente**" consentono rispettivamente di:

- **Escludi promo sconto articolo:** se selezionato, nel momento in cui
  verrà applicata la Promozione di tipo "Sconto Cliente" verranno
  automaticamente disattivate eventuali altre Promozioni (es. Sconto
  Articolo o Prezzo Fisso, Sconto Articolo a quantità, Offerte M x N
  ecc...) che potrebbero essere attive sugli articoli presenti in
  carrello.

- **Escludi promo accumulo punti:** opzione non attualmente gestita
  all'interno del sito

- **Disattiva se presente promo sconto articolo:** se selezionato
  consente di disattivare automaticamente la Promozione di tipo "Sconto
  Cliente" nel momento in cui dovessero essere attive eventuali altre
  Promozioni di tipo Articolo (es. Sconto Articolo o Prezzo Fisso,
  Sconto Articolo a quantità, Offerte M x N ecc...) sui prodotti
  attualmente presenti in carrello.

Dopo aver codificato questa Promozione ed averla esportata all'interno
del sito, prima di poterla effettivamente utilizzare sarà necessario,
ovviamente, attivarla e questo potrà essere fatto direttamente dalla
maschera "Lista delle Promozioni", selezionandola in elenco e cliccando
sul pulsante "**Attiva Promozione**" oppure agendo dal parametro
"**Attivo**" presente nella maschera di configurazione della Promozione
stessa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_33.bmp](./assets/media/image552.png)

**ATTENZIONE! Gli sconti dovuti all'applicazione di questo tipo di
Promozioni verranno applicati, all'interno del sito, sempre e comunque a
livello di Carrello mediante l'inserimento di un relativo Abbuono**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_30.bmp](./assets/media/image538.png)

In queste condizioni non sarà ovviamente possibile visualizzare gli
sconti dovuti alla promozione ne in Catalogo ne tanto meno all'interno
delle varie schede prodotto.

L'Abbuono dovuto all'applicazione della Promozione verrà infatti
visualizzato soltanto in Carrello oltre che, ovviamente, in fase di
Checkout ordine.

Lato gestionale, infine, nel momento in cui si andrà a caricare, in
cassa, l'ordine nato all'interno del sito web si avrà che lo sconto,
dovuto alla promozione e **applicato sul sito a livello di Carrello**
mediante un relativo **Abbuono,** verrà riportato all'interno del campo
**Sconto**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_12.bmp](./assets/media/image542.png)

**ATTENZIONE!** Le Promozioni di tipo **Sconto Cliente** sono
considerate tra l'elenco delle Promozioni da poter escludere nel caso di
applicazione di eventuali Buoni Sconto.

Ciò significa dunque che nel momento in cui un dato utente dovesse
trovarsi applicata questo tipo di promozione, e fosse anche in possesso
di un Codice Sconto ancora valido, potrebbe essere possibile fare in
modo che l'applicazione del Buono Sconto annulli automaticamente
l'applicazione della Promozione.

Per maggiori informazioni sull'utilizzo dei Buoni Sconto e sulla
possibilità di escludere o meno determinate promozioni all'applicazione
dei Buoni Sconto si veda anche il capitolo "*Ordini -- Configurazione
Promozioni -- Buoni Sconto*" di questo manuale.

