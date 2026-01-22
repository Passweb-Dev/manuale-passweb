# ONE STOP SHOP (OSS)



A partire dal 1° Luglio 2021 sono entrate in vigore alcune modifiche
applicate alla disciplina di gestione dell'IVA comunitaria. Nello
specifico è stata introdotta la figura della "vendita a distanza
intracomunitaria di beni" con la previsione per queste vendite della
tassazione nel luogo di destinazione del bene presso l'acquirente, salvo
che il valore delle cessioni non superi la soglia annua di 10.000 euro.

Inoltre per evitare che i fornitori di beni destinati a consumatori
privati debbano registrarsi ai fini IVA in ogni stato membro in cui
prestano servizi, il "mini" sportello unico per l'IVA (denominato **MOSS
-- Mini One Stop Shop**) è diventato **sportello unico OSS (One Stop
Shop)** aprendosi quindi anche a tutti i servizi resi ai consumatori
privati e alle vendite a distanza intracomunitarie di beni.

In poche parole quindi nel momento in cui si dovesse aderire a questo
nuovo servizio non ci sarà più l'obbligo, relativamente alle vendite
effettuate tramite il proprio sito Ecommerce, **a privati e/o ad aziende
non iscritte al VIES e dirette verso paesi comunitari diversi
dall'Italia**, di registrarsi ai fini IVA nello specifico paese di
destinazione della merce.

Sarà però necessario applicare per gli articoli venduti le aliquote IVA
in vigore nello specifico paese in cui si dovrà poi essere
effettivamente spedita la merce.

**ATTENZIONE!** Per maggiori informazioni in merito si consiglia di fare
sempre riferimento alle specifiche normative ministeriali

Ora, considerando che all'interno del gestionale l'aliquota IVA è
definita direttamente sull'anagrafica dell'articolo ed è ovviamente
indipendente dal paese dichiarato nell'indirizzo di spedizione merce,
nel momento in cui l'amministratore del sito dovesse decidere di aderire
al nuovo sistema di sportello unico OSS, per poter definire e gestire
aliquote Iva diverse, per i singoli articoli, in relazione al paese in
cui verrà poi effettivamente spedita la merce, dovrà necessariamente
codificare all'interno di Passweb delle Tasse di tipo IVA.

Nello specifico sarà necessario:

- Codificare una Tassa di tipo IVA per ogni paese in cui potrà essere
  spedita la merce e in cui le aliquote IVA dei vari articoli sono
  effettivamente diverse da quelle Italiane

- Inserire, per ogni articolo, le relative aliquote o esenzioni IVA
  nell'Attributo dichiarato in fase di configurazione della specifica
  Tassa (in questo senso si consiglia di utilizzare l'App Mexal
  "**Passweb dati articolo IVA OSS**")

Supponendo quindi di effettuare vendite a privati e/o ad aziende non
iscritte al VIES anche in Germania e in Francia, e nell'ipotesi in cui
le aliquote IVA applicate da questi due paesi siano effettivamente
diverse da quelle italiane sarà necessario:

- Codificare due nuovi Attributi Articolo da utilizzare per gestire le
  aliquote e/o le esenzioni IVA nello specifico paese.

> Si consiglia, in questo senso, di attivare l'App Mexal "**Passweb dati
> articolo IVA OSS**" e di mappare gli Attributi Articolo sui relativi
> campi della tabella MyDB messa a disposizione da questa stessa App.

- Valorizzare, per ogni articolo gestito sul sito, gli Attributi di cui
  al punto precedente con le corrette aliquote o esenzioni IVA applicate
  per il prodotto stesso in Germania e in Francia.

> In questo senso se è stata attivata l'App Mexal "**Passweb dati
> articolo IVA OSS**" sarà possibile utilizzare l'apposita funzione
> accessibile dal menu **"Magazzino -- APP -- Passweb dati articolo IVA
> OSS -- Popola aliquota IVA su articoli"**

- Creare e abilitare lato Passweb due nuove Tasse di tipo IVA valide
  rispettivamente ed esclusivamente nelle nazioni Germania e Francia e
  configurate come nella figura di seguito riportata

![](./assets/media/image454.png)

> **Tipologia Tassa** = IVA
>
> **Soggetto** = Privato / Azienda non iscritta al VIES
>
> **Gestione Tassa** = Articolo
>
> **Attributo** = attributo articolo utilizzato per impostare l'aliquota
> iva da applicare per l'articolo
>
> **Zona Tasse** = Francia / Germania

In queste condizioni nel momento in cui un utente della tipologia
indicata in corrispondenza del campo "Soggetto"**,** dovesse effettuare
l'autenticazione al sito, verrà controllata la Nazione associata al suo
indirizzo principale (generalmente quella indicata nell'indirizzo di
fatturazione e dichiarata quindi nel relativo campo dell'anagrafica
gestionale) e se dovesse essere rilevata una Tassa di tipo IVA valida
per questa Nazione verranno automaticamente applicate le aliquote
definite in corrispondenza dell' Attributo Articolo dichiarato in fase
di definizione della Tassa stessa.

Inoltre, nel momento in cui l' utente dovesse poi selezionare, in
carrello (quindi in fase di preventivo) o direttamente in checkout, uno
specifico indirizzo di spedizione francese o tedesco verranno applicate
le relative tasse e quindi, nello specifico, **verranno automaticamente
aggiornati i totali del documento prendendo in considerazione ancora una
volta, per gli articoli in ordine, le aliquote o le esenzioni IVA per
essi indicate negli Attributi dichiarati in fase di configurazione della
relativa Tassa**.

**ATTENZIONE!** Nel momento in cui si dovesse decidere di attivare
questo tipo di gestione potrebbe rivelarsi particolarmente utile:

- Inserire in carrello e in checkout un testo informativo per avvisare
  l'utente che a seconda dell'indirizzo di spedizione selezionato
  potrebbero essere applicate aliquote iva diverse (in uso nello
  specifico paese di destinazione della merce) e che quindi potrebbero
  cambiare i totali del documento.

- Utilizzare il segnaposto "**Zona Spedizione**" presente all'interno
  dei componenti "**Paragrafo**" e "**HTML**"

![](./assets/media/image455.png)

> segnaposto questo che verrà poi sostituito in fase di generazione
> della pagina web con i dati relativi alla zona di spedizione
> attualmente considerata e in relazione alla quale, dunque, sono
> attualmente calcolati gli importi delle Tasse Addizionali.

- Utilizzare il componente "**Selezione Indirizzo**" per consentire
  all'utente di indicare, in un qualunque momento, una zona di
  spedizione merce diversa da quella attualmente considerata e in
  relazione alla quale valutare gli importi delle tasse addizionali

Altra cosa fondamentale da tenere in considerazione è che **una volta
selezionato uno specifico indirizzo di spedizione merce, l'informazione
sul paese di destinazione verrà mantenuta in sessione** **per cui
tornando, ad esempio, in Catalogo piuttosto che in una specifica scheda
prodotto (o direttamente anche in carrello e/o in checkout posto di aver
inserito anche in queste pagine l'informazione relativa alle aliquote
iva degli articoli) verrà visualizzata l'aliquota IVA effettivamente in
uso, per l'articolo in esame, nel paese di destinazione della merce
indicato nell'ultimo indirizzo di spedizione selezionato**.

Infine occorre evidenziare altre tre cose di fondamentale importanza:

- L'applicazione delle Tasse IVA ai fini OSS avverrà solo ed
  esclusivamente per le tipologie di utenti indicati in corrispondenza
  del parametro "Soggetto". **Nel caso dunque di ordini effettuati da
  utenti non della tipologia indicata verranno applicate sempre e
  soltanto aliquote ed esenzioni iva Italiane definite quindi
  nell'anagrafica gestionale del relativo articolo**

- Oltre alle Tasse di tipo Iva, Passweb prenderà sempre in
  considerazione anche quelle che possono essere eventuali particolarità
  di tipo IVA e/o assoggettamenti IVA specifici per un determinato
  cliente definiti direttamente all'interno del gestionale.

> In conseguenza di ciò la determinazione della corretta aliquota IVA da
> applicare per ogni articolo, avverrà secondo le priorità di seguito
> indicate:

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
    della merce, verrà utilizzata l'aliquota iva indicata nell'
    attributo definito in fase di configurazione della tassa stessa.

> Se l' attributo in questione dovesse essere vuoto o dovese contenere
> un'aliquota o un esenzione non valida, tale valore non verrà
> considerato e verrà invece utilizzata l'iva italiana definita nell'
> anagrafica articolo del gestionale.

4.  Nel momento in cui non dovesse presentarsi nessuna delle condizioni
    indicate ai punti precedenti, verrà sempre considerata l'iva
    italiana definita nell' anagrafica articolo del gestionale

> In sostanza **nel momento in cui si dovesse decidere di utilizzare le
> tasse di tipo IVA per la gestione dell'IVA OSS sarà di fondamentale
> importanza accertarsi che, per gli utenti interessati, non sia stata
> impostato, lato gestionale, nessun assoggettamento Iva nella loro
> anagrafica e che non sia stata definita per essi nessuna Particolarità
> di tipo IVA**.

- Per quel che riguarda l'IVA associata alle spese di trasporto
  l'aliquota utilizzata potrà variare in relazione al fatto di gestire
  tali spese mediante un apposito articolo di tipo Spesa oppure nel
  piede del documento. In particolare:

  - Nel caso in cui le **spese di trasporto** dovessero essere gestite
    con un **articolo di tipo Spesa**, questo verrà trattato esattamente
    come tutti gli altri articoli in ordine e quindi anche per esso
    verrà utilizzata esattamente l'aliquota indicata nell' attributo
    definito in fase di configurazione della tassa utilizzata per
    gestire l'IVA OSS

  - Nel caso in cui le **spese di trasporto** dovessero invece essere
    gestite nel **piede del documento** l'applicazione dell'aliquota IVA
    seguirà, di base, le stesse logiche del gestionale. In questo senso
    l'unica eccezione da tenere in considerazione è quella che si avrà
    quando all'interno del gestionale è stato selezionato il parametro
    "**Gestione IVA OSS**" presente all'interno della maschera
    "**Parametri attività IVA**" (menu "*Anagrafica Azienda -- Dati
    Aziendali*")

![](./assets/media/image456.png)

> In queste condizioni infatti se il cliente che acquista sul sito è un
> privato e la merce viene spedita fuori Italia ma comunque in un paese
> appartenente all'Unione Europea allora l'iva sulle spese di trasporto
> verrà sempre ripartita indipendentemente dal fatto che per lo
> specifico cliente sia stata abilitata o meno la gestione della
> fatturazione elettronica

