# SCONTO ARTICOLO QUANTITA'



Utilizzando questo tipo di promozione è possibile configurare, per gli
articoli coinvolti, degli sconti (in percentuale o a valore) definiti in
base a quella che è la quantità in ordine di questi stessi articoli (10%
in caso di acquisto di un solo pezzo, 15% in caso di acquisto di due
pezzi ecc\...) .

E' possibile mettere in promozione singoli articoli (Tabella "**Articoli
in Promozione**") oppure intere categorie (Tabella **"Articoli
appartenenti alle categorie"**) definendo poi, all'interno della
relativa Tabella "**Sconto a Quantità**", i vari scaglioni con i
relativi sconti da applicare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_14.bmp](./assets/media/image543.png){width="5.363888888888889in"
height="3.1819444444444445in"}

Il campo "**Tipo Sconto**" presente all'interno della scheda "**Opzioni
Sconto articolo**" permette di definire se dovranno essere utilizzati
(**all'interno del gestionale e anche sul sito**) sconti a valore o in
percentuale.

E' quindi possibile selezionare uno dei seguenti valori:

- **Percentuale:** selezionando questa opzione verranno utilizzati
  sconti in percentuale.

> All'interno della Tabella **Sconto a quantità** andranno quindi
> indicate, in corrispondenza di ogni scaglione, le relative percentuali
> di sconto che dovranno poi essere applicate nel momento in cui uno
> degli articoli coinvolti nella promozione venga inserito in ordine con
> una quantità che rientra nel relativo scaglione

- **Valore:** selezionando questa opzione verranno utilizzati sconti a
  valore.

> All'interno della Tabella **Sconto a quantità** andranno quindi
> indicati, in corrispondenza di ogni scaglione, i relativi valori dello
> sconto da applicare nel momento in cui uno degli articoli coinvolti
> nella promozione venga inserito in ordine con una quantità che rientra
> nel relativo scaglione

Per maggiori informazioni relativamente alla configurazione, lato
gestionale, di questa particolare tipologia di promozione si rimanda
all'apposito manuale di prodotto.

Una volta codificata ed esportata, questo tipo di Promozione potrà poi
essere utilizzata all'interno del sito in due modi differenti,
dipendentemente dal fatto di aver valorizzato o meno il campo "**Applica
solo ai primi articoli**" (scheda "**Opzioni Sconto articolo**").

**[CASO A -- APPLICA SOLO AI PRIMI ARTICOLI 🡪 NON
VALORIZZATO]{.underline}**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_16.bmp](./assets/media/image544.png){width="5.1625in"
height="3.058333333333333in"}

In queste condizioni sarà possibile decidere, in fase di attivazione e
configurazione della Promozione all'interno del sito, come questa dovrà
effettivamente comportarsi.

Selezionando, all'interno della maschera "Lista delle Promozioni"
precedentemente esaminata, la Promozione in esame, e cliccando sul
pulsante **Modifica Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_promozione.bmp](./assets/media/image479.png){width="0.83125in"
height="0.2013888888888889in"} ) si avrà accesso alla maschera di
configurazione della Promozione stessa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_17.bmp](./assets/media/image545.png){width="5.746527777777778in"
height="3.50625in"}

all'interno della quale il campo:

**Attivo:** consente di attivare la Promozione e di poterla quindi
utilizzare all'interno del sito

**Gestione:** permette di stabilire come la Promozione in esame dovrà
essere applicata all'interno del sito. E' possibile selezionare una
delle seguenti opzioni:

- **Ho.Re.Ca.:** in queste condizioni la Promozione verrà applicata
  utilizzando esattamente le stesse logiche definite all'interno del
  gestionale.

> In particolare, **qualunque sia l'unità di misura dell'articolo**,
> eventuali sconti (in percentuale o a valore) dovuti alla Promozione
> verranno applicati **sempre e comunque a livello di Carrello mediante
> l'inserimento di un relativo Abbuono.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_30.bmp](./assets/media/image538.png){width="5.155555555555556in"
height="3.765972222222222in"}

> In queste condizioni non sarà quindi possibile visualizzare gli sconti
> dovuti alla promozione ne in Catalogo ne tanto meno all'interno della
> relativa scheda prodotto.
>
> L'Abbuono dovuto all'applicazione della Promozione verrà infatti
> visualizzato soltanto in Carrello oltre che, ovviamente, in fase di
> Checkout ordine.
>
> **ATTENZIONE!** in queste condizioni il parametro "**Applica Sconto
> come prezzo", non ha alcun effetto all'interno del sito.** In
> conseguenza di ciò, anche nel caso in cui si dovesse selezionare tale
> parametro **eventuali sconti dovuti alla Promozione saranno comunque
> applicati (sul sito) a livello di Carrello mediate l'inserimento di un
> Abbuono**

- **Listino:** selezionando questa opzione, la Promozione verrà
  applicata utilizzando una logica propria del sito web, non sempre
  replicabile all'interno del gestionale.

> In particolare gli Sconti (in percentuale o a valore) dovuti
> all'applicazione di questa promozione verranno applicati **sempre e
> comunque a livello di listino, indipendentemente dal fatto di
> considerare articoli con unità di misura uguale o diversa da pz.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_9.bmp](./assets/media/image537.png){width="5.155555555555556in"
height="3.5972222222222223in"}

> Sarà quindi possibile visualizzare gli sconti dovuti alla promozione
> tanto in Catalogo quanto nella relativa scheda prodotto.
>
> Inoltre, in queste condizioni, nel caso in cui sia stato selezionato,
> sul gestionale, anche il parametro "**Applica Sconto come prezzo"**
> sarà poi necessario considerare che:

- All'interno del sito non verranno visualizzati gli sconti dovuti alla
  promozione ma verranno applicati direttamente i prezzi al netto di
  tali sconti

- Nel calcolo dei prezzi al netto degli sconti, sul sito il risultato
  verrà arrotondato sempre a 2 decimali.

- Gli sconti dovuti alla promozione andranno ad incidere direttamente
  sui prezzi dell'articolo e non sui totali di riga. In queste
  condizioni dunque, aumentando le quantità in ordine, aumenteranno
  (tipicamente) anche gli sconti soprattutto nel caso in cui questi
  siano gestiti a valore.

**[CASO B -- APPLICA SOLO AI PRIMI ARTICOLI 🡪 VALORIZZATO]{.underline}**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_18.bmp](./assets/media/image546.png){width="5.1625in"
height="3.058333333333333in"}

In queste condizioni eventuali sconti dovuti alla Promozione verranno
applicati **sempre e comunque a livello di Carrello mediante
l'inserimento di un relativo Abbuono.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_30.bmp](./assets/media/image538.png){width="5.155555555555556in"
height="3.765972222222222in"}

Selezionando, all'interno della maschera "Lista delle Promozioni"
precedentemente esaminata, la Promozione in esame, e cliccando sul
pulsante **Modifica Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_promozione.bmp](./assets/media/image479.png){width="0.83125in"
height="0.2013888888888889in"} ) si avrà sempre accesso alla maschera di
configurazione della Promozione stessa dove, questa volta però, non sarà
più possibile decidere come questa dovrà comportarsi all'interno del
sito ma solamente se attivarla o meno (parametro "**Attivo**").

In relazione a questa particolare configurazione della Promozione va
sottolineato inoltre che questa verrà effettivamente applicata solo ai
primi N articoli presenti in ordine e che rientrano, ovviamente, nella
promozione.

A differenza delle Promozioni di tipo "Sconto Articolo o Prezzo Fisso",
per le Promozioni "Sconto Articolo a Quantità" il numero N indicato
all'interno del campo "**Applica solo ai primi Articoli**", viene
valutato sempre allo stesso modo sia per articoli con unità di misura
uguale a pz che per articoli con unità di misura diversa da pz.

Nello specifico, **ogni articolo in ordine avrà sempre un incidenza pari
a 1** indipendentemente da quella che è la quantità per esso acquistata.
In queste condizioni, infatti, la quantità acquistata determinerà lo
scaglione in cui far ricadere lo specifico articolo e, conseguentemente
quello che sarà lo sconto da applicare

Lato gestionale, infine, nel momento in cui si andrà a caricare, in
cassa, l'ordine nato all'interno del sito web si avrà che:

- eventuali **sconti sui singoli articoli** dovuti all'applicazione
  della promozione verranno riportati **all'interno delle relative righe
  articolo**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_11.bmp](./assets/media/image541.png){width="5.279166666666667in"
height="3.5256944444444445in"}

- eventuali sconti, dovuti alla promozione e **applicati sul sito a
  livello di Carrello** mediante **Abbuoni,** verranno riportati
  all'interno del campo **Sconto**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_promozioni_12.bmp](./assets/media/image542.png){width="5.279166666666667in"
height="3.5256944444444445in"}

**ATTENZIONE!** Le Promozioni di tipo **Sconto Articolo Quantità** non
sono considerate tra l'elenco delle Promozioni da poter escludere nel
caso di applicazione di eventuali Buoni Sconto.

Ciò significa dunque che nel momento in cui un dato utente dovesse
trovarsi applicata questo tipo di promozione, e fosse anche in possesso
di un Codice Sconto ancora valido, potrebbe tranquillamente utilizzarlo
usufruendo quindi di un ulteriore sconto oltre a quello previsto dalla
Promozione.

Per maggiori informazioni sull'utilizzo dei Buoni Sconto e sulla
possibilità di escludere determinate promozioni all'applicazione dei
Buoni Sconto si veda anche il capitolo "*Ordini -- Configurazione
Promozioni -- Buoni Sconto*" di questo manuale.

