# CESSIONI INTRACOMUNITARIE E ESPORTAZIONI VERSO PAESI EXTRA UE



Le normative che regolano l'applicazione dell'IVA per le cessioni
intracomunitarie e le esportazioni extra UE sono definite principalmente
dal D.P.R. 633/1972 per il regime IVA in Italia, integrato dalle
disposizioni del D.L. 331/1993 per le cessioni intracomunitarie, e dai
regolamenti UE come il Regolamento 282/2011 per la prova delle
operazioni intracomunitarie.

Nello specifico per quel che riguarda le **Cessioni intracomunitarie**
la normativa chiave è l'articolo 41, c.1, lett. a del D.L. 331/1993,
secondo cui queste operazioni possono essere non imponibili IVA a
condizione che:

- La transazione avvenga tra soggetti passivi IVA (aziende o
  professionisti) stabiliti in due diversi Stati membri dell\'Unione
  Europea.

- I beni siano spediti o trasportati dal venditore o dal cliente (o da
  terzi per loro conto) da un paese dell\'UE a un altro.

- Entrambi i soggetti siano registrati al VIES

Per quel che riguarda invece le **Esportazioni verso Paesi extra UE**
queste possono sempre essere considerate non imponibili IVA, ai sensi
dell'articolo 8, c.1 del D.P.R. 633/1972, se soddisfano i seguenti
requisiti:

- I beni vengono materialmente spediti o trasportati fuori dall'Unione
  Europea.

- Il cedente (venditore italiano) è in grado di fornire prova della
  spedizione o del trasporto dei beni.

- Non è rilevante se l'acquirente sia un'azienda o un privato.

**ATTENZIONE!** Per maggiori informazioni in merito alla non
imponibilità IVA delle cessioni intracomunitarie e/o delle esportazione
extra UE si consiglia di fare sempre riferimento alle specifiche
normative fiscali e al proprio commercialista

Ora, considerando che Passweb, come indicato nel precedente capitolo di
questo manuale, gestisce in maniera completamente automatica un sistema
di verifica dell'iscrizione al VIES da parte di aziende abilitate ad
effettuare acquisti all'interno del sito, per fare in modo che nelle
diverse casistiche venga applicata la corretta esenzione / aliquota IVA
sarà necessario impostare due distinte Tasse di tipo IVA con le
caratteristiche di seguito indicate:

**[ESENZIONE IVA PER VENDITE INTRACOMUNITARIE]{.underline}**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tassa_cessioni_intra_ue.bmp](./assets/media/image458.png){width="5.83125in"
height="3.8375in"}

- **Soggetto**: Azienda iscritta al VIES

- **Gestione** **Tassa**: Fissa

- **Aliquota IVA**: codice di esenzione per le vendite intracomunitarie
  (es. N32)

> **ATTENZIONE!** il codice esenzione indicato all'interno di questo
> campo deve essere uno dei codici esenzione effettivamente gestiti
> all'interno del gestionale

- **Nazioni** : tutte le nazioni europee

**[ESENZIONE IVA PER VENDITE EXTRA UE]{.underline}**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tassa_cessioni_extra_ue.bmp](./assets/media/image459.png){width="5.83125in"
height="3.8375in"}

- **Soggetto**: Azienda iscritta al VIES, Azienda non iscritta al VIES,
  Privato

- **Gestione** **Tassa**: Fissa

- **Aliquota IVA**: codice di esenzione per le vendite Extra UE (es.
  N31)

> **ATTENZIONE!** il codice esenzione indicato all'interno di questo
> campo deve essere uno dei codici esenzione effettivamente gestiti
> all'interno del gestionale

- **Nazioni** : tutte le nazioni extra europee

In queste condizioni nel momento in cui ad effettuare l'ordine
all'interno del sito dovesse essere:

- **Un'azienda iscritta al VIES** e **l'indirizzo di spedizione** merce
  dovesse essere quello di una **nazione europea** verrà applicata la
  Tassa "Esenzione IVA per vendite intracomunitarie" e, di conseguenza,
  tutti gli articoli in ordine saranno esenti iva con il codice
  esenzione indicato in fase di configurazione della relativa tassa

- **Un' azienda non iscritta al VIES** e **l'indirizzo di spedizione**
  merce dovesse essere quello di una **nazione europea** non verrà
  applicata nessuna delle due Tasse sopra indicate (nessuna delle due
  prevede infatti la configurazione "Azienda non iscritta al VIES + area
  di spedizione europea")

> In queste condizioni dunque potrebbe:

- **Essere applicata l'IVA OSS** posto che tale regime sia
  effettivamente applicabile e che siano state create apposite Tasse di
  tipo IVA secondo quanto indicato nel precedente capitolo (*One Stop
  Shop OSS*) di questo manuale. Ogni articolo in ordine avrebbe quindi
  l'aliquota in uso per quello stesso articolo nel paese di spedizione
  della merce

- **Essere applicata l'IVA Italiana**. Nel caso in cui non fosse
  possibile applicare l'IVA OSS ogni articolo in ordine avrebbe
  esattamente l'aliquota per esso impostata nella sua anagrafica
  gestionale

<!-- -->

- **Un'azienda iscritta o non iscritta al VIES** o un **Privato** e
  **l'indirizzo di spedizione** merce dovesse essere quello di una
  **nazione extra europea** verrà applicata la Tassa "Esenzione IVA per
  vendite extra UE" e, di conseguenza tutti gli articoli in ordine
  saranno esenti iva con il codice esenzione indicato in fase di
  configurazione della relativa tassa

- **Un Privato** e **l'indirizzo di spedizione** merce dovesse essere
  quello di una **nazione europea** non verrà applicata nessuna delle
  due Tasse sopra indicate (nessuna delle due prevede infatti la
  configurazione "Privato + area di spedizione europea")

> In queste condizioni dunque potrebbe:

- **Essere applicata l'IVA OSS** posto che tale regime sia
  effettivamente applicabile e che siano state create apposite Tasse di
  tipo IVA secondo quanto indicato nel precedente capitolo (*One Stop
  Shop OSS*) di questo manuale. Ogni articolo in ordine avrebbe quindi
  l'aliquota in uso per quello stesso articolo nel paese di spedizione
  della merce

- **Essere applicata l'IVA Italiana**. Nel caso in cui non fosse
  possibile applicare l'IVA OSS ogni articolo in ordine avrebbe
  esattamente l'aliquota per esso impostata nella sua anagrafica
  gestionale

Infine trattandosi comunque, anche in questo caso, di Tasse di tipo IVA,
restano valide le stesse considerazione che sono state fatte parlando di
IVA OSS. Nello specifico:

- Considerando che cambiando l'indirizzo di spedizione merce (in
  Carrello, in Checkout o mediante il componente "Spedizione")
  cambieranno anche le aliquote / esenzioni iva associate agli articoli
  gestiti all'interno del sito, come per l'IVA OSS anche in questo caso
  potrebbe rivelarsi particolarmente utile inserire in carrello e in
  checkout un testo informativo per avvisare l'utente che a seconda
  dell'indirizzo di spedizione selezionato potrebbero essere applicate
  aliquote iva diverse (in uso nello specifico paese di destinazione
  della merce) e che quindi potrebbero cambiare i totali del documento.

- **Una** **volta selezionato uno specifico indirizzo di spedizione
  merce, l'informazione sul paese di destinazione verrà mantenuta in
  sessione** per cui tornando, ad esempio, in Catalogo piuttosto che in
  una specifica scheda prodotto (o direttamente anche in carrello e/o in
  checkout posto di aver inserito anche in queste pagine l'informazione
  relativa alle aliquote iva degli articoli) verrà visualizzata
  l'aliquota / esenzione IVA effettivamente in uso, per l'articolo in
  esame, nel paese di destinazione della merce indicato nell'ultimo
  indirizzo di spedizione selezionato.

<!-- -->

- Oltre alle Tasse di tipo Iva, Passweb prenderà sempre in
  considerazione anche quelle che possono essere eventuali particolarità
  di tipo IVA e/o assoggettamenti IVA specifici per un determinato
  cliente definiti direttamente all'interno del gestionale.

> In conseguenza di ciò la determinazione della corretta aliquota /
> esenzione IVA da applicare per ogni articolo, avverrà secondo le
> priorità di seguito indicate:

1.  **Particolarità Iva**: nel momento in cui dovesse essere attiva una
    specifica particolarità iva verrà gestita l'aliquota definita nella
    particolarità stessa

2.  **Iva utente**: nel momento in cui l'utente che sta effettuando
    l'ordine dovesse avere una specifica aliquota, associata
    direttamente sulla sua anagrafica gestionale, verrà utilizzata
    questa stessa aliquota

3.  **Tassa IVA legata alla Nazione**: se non sono presenti
    particolarità o assoggettamenti iva specifici per l'utente ed è
    attiva una Tassa di tipo IVA definita sulla nazione di spedizione
    della merce, verrà utilizzata l'aliquota / esenzione iva indicata in
    fase di configurazione della tassa stessa.

4.  Nel momento in cui non dovesse presentarsi nessuna delle condizioni
    indicate ai punti precedenti, verrà sempre considerata l'iva
    italiana definita nell' anagrafica articolo del gestionale

> In sostanza **nel momento in cui si dovesse decidere di utilizzare le
> tasse di tipo IVA per la gestione delle cessioni intracomunitarie e/o
> delle esportazioni extra UE, sarà di fondamentale importanza
> accertarsi che, per gli utenti interessati, non sia stata impostato,
> lato gestionale, nessun assoggettamento Iva nella loro anagrafica e
> che non sia stata definita per essi nessuna Particolarità di tipo
> IVA**.

- Per quel che riguarda l'IVA associata alle spese di trasporto
  l'aliquota utilizzata potrà variare, anche in questo caso, in
  relazione al fatto di gestire tali spese mediante un apposito articolo
  di tipo Spesa oppure nel piede del documento. In particolare:

  - Nel caso in cui le **spese di trasporto** dovessero essere gestite
    con un **articolo di tipo Spesa**, questo verrà trattato esattamente
    come tutti gli altri articoli in ordine e quindi anche per esso
    verrà utilizzata esattamente l'aliquota / esenzione indicata in fase
    di configurazione della tassa

  - Nel caso in cui le **spese di trasporto** dovessero invece essere
    gestite nel **piede del documento** l'applicazione dell'aliquota IVA
    seguirà, di base, le stesse logiche del gestionale. In questo senso
    l'unica eccezione da tenere in considerazione è quella che si avrà
    quando all'interno del gestionale è stato selezionato il parametro
    "**Gestione IVA OSS**" presente all'interno della maschera
    "**Parametri attività IVA**" (menu "*Anagrafica Azienda -- Dati
    Aziendali*")

![Videate\\parametri_attivita_iva.bmp](./assets/media/image456.png){width="5.5256944444444445in"
height="2.707638888888889in"}

> In queste condizioni infatti se il cliente che acquista sul sito è un
> privato e la merce viene spedita fuori Italia ma comunque in un paese
> appartenente all'Unione Europea allora l'iva sulle spese di trasporto
> verrà sempre ripartita indipendentemente dal fatto che per lo
> specifico cliente sia stata abilitata o meno la gestione della
> fatturazione elettronica.

