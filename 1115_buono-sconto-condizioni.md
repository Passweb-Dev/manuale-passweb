# BUONO SCONTO -- CONDIZIONI



All'interno della sezione "**Condizioni**" è possibile definire una o
più condizioni che dovranno essere obbligatoriamente soddisfatte
affinchè i codici sconto che andremo poi ad aggiungere possano
effettivamente essere ritenuti validi dando quindi accesso alla relativa
scontistica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\generatore_condizioni.bmp](./assets/media/image574.png)

**ATTENZIONE!** Prima di poter definire delle nuove condizioni è
necessario effettuare almeno un salvataggio del Buono Sconto

Una vota salvato il Buono Sconto si attiverà infatti un nuovo pulsante
mediante il quale poter gestire, attraverso l'apposita maschera,
l'inserimento di una nuova condizione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_promozione1.bmp](./assets/media/image575.png)

Per ogni condizione è possibile impostare un valore per i seguenti
parametri:

**Nome:** nome identificativo della condizione che si sta codificando

**Filtro Articoli:** consente di impostare un determinato filtro
articoli. Per maggiori informazioni in merito alla creazione di un
filtro articoli si veda anche la sezione "*Utenti -- Gruppi Utenti Sito
-- Filtri Utente e Filtri Articolo -- Filtri Articolo*" di questo
manuale.

Impostando, sulla condizione in esame, un filtro articoli, i codici
associati al Buono Sconto verranno considerati validi solo ed
esclusivamente nel momento in cui gli articoli in carrello dovessero
effettivamente soddisfare tale filtro.

In questo senso poi occorre sottolineare che, **relativamente agli
articoli di tipo Campionario**, la validazione del filtro impostato
verrà fatta prendendo in considerazione l'articolo Campionario in sé
piuttosto che i singoli Componenti dipendentemente da come è stato
impostato il parametro "**Gestione Articoli Box**" alla pagina
"**Configurazione Catalogo**" del Wizard.

In particolare nel caso in cui il parametro in questione dovesse essere
impostato sul valore:

- **Considera il Box** -- **opzione di default**: verrà preso in
  considerazione soltanto l'articolo Campionario.

> In questo caso dunque, la condizione di applicabilità del Buono Sconto
> verrà validata, se l'articolo Campionario in sé dovesse effettivamente
> soddisfare il filtro impostato, indipendentemente dal fatto che i suoi
> componenti possano poi soddisfare o meno lo stesso filtro

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, la condizione di applicabilità del Buono Sconto
> verrà eventualmente validata prendendo in considerazione i componenti
> del Campionario ma non l'articolo Campionario in sé che, quindi,
> potrebbe anche non soddisfare il filtro impostato.

**Filtro Carrello:** consente di impostare un filtro sulla quantità /
numero di articoli presenti in carrello, a livello globale o di singola
riga, , e/o sulla base del fatto che gli articoli in carrello abbiano o
meno uno sconto già applicato. Di base quindi lavorando sul "Filtro
Carrello" sarà possibile:

- decidere anche se i codici associati al Buono Sconto dovranno essere
  applicati solo nel momento in cui tutte le righe articolo presenti in
  carrello dovessero soddisfare un eventuale "Filtro Articoli" o anche
  se solo una certa percentuale di esse dovesse essere effettivamente
  sufficiente per fare scattare la promozione.

- decidere se la condizione di applicabilità del Buono Sconto dovrà
  essere validata considerando tutti gli articoli presenti in carrello
  che soddisfano un eventuale "Filtro Articoli", oppure solo quelli che,
  oltre a soddisfare un eventuale "Filtro Articoli", risultino anche
  privi di eventuali altri sconti già applicati

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

- **Quantità in carrello:** permette di definire una condizione sulla
  quantità complessiva di articoli presenti in carrello. Supponendo
  quindi di impostare un filtro del tipo "Quantità in carrello maggiore
  di 5" i codici associati al Buono Sconto in esame verranno considerati
  validi solo ed esclusivamente nel caso in cui la quantità complessiva
  di articoli in carrello dovesse essere maggiore di 5. Tale condizione
  potrebbe quindi essere soddisfatta inserendo in carrello un solo
  articolo in quantità 6 o, ad esempio, due distinti articoli ciascuno
  in quantità 3.

- **Elementi in carrello:** permette di definire una condizione sul
  **numero complessivo di articoli presenti in carrello**. Supponendo
  quindi di impostare un filtro del tipo "Elementi in Carrello maggiore
  di 2" i codici associati al Buono Sconto in esame verranno considerati
  validi solo ed esclusivamente nel caso in cui dovessero essere
  presenti in carrello almeno 3 distinte righe articolo
  indipendentemente dalla quantità acquistata per ognuno di essi e
  indipendentemente dal fatto che tali righe siano riferite o meno allo
  stesso prodotto.

> **ATTENZIONE!** **Nel caso in cui, sulla condizione in esame, sia
> stato impostato anche un Filtro Articoli, nella valutazione del filtro
> sulle quantità e/o sul numero di articoli presenti in carrello
> verranno considerati solo ed esclusivamente gli articoli che
> soddisfano il filtro impostato.**
>
> Di base dunque se dovessimo trovarci in una situazione mista in cui
> sono presenti in carrello sia prodotti che soddisfano un eventuale
> Filtro Articoli sia prodotti che non lo soddisfano, nel momento in cui
> quelli che lo soddisfano dovessero soddisfare anche eventuali
> condizioni impostate sulla quantità o sul numero di elementi, allora i
> codici associati al Buono Sconto verrebbero considerati validi.
>
> Diversamente se l'esigenza dovesse essere quella di non validare i
> codici sconto in una situazione mista, in cui ci ritroviamo in
> carrello prodotti che soddisfano il Filtro Articoli ma anche prodotti
> che non lo soddisfano, sarà necessario utilizzare allora per il Filtro
> Quantità l'opzione "Percentuale Elementi in Carrello"

- **Elementi distinti in Carrello**: stesso funzionamento della
  condizione "Elementi in carrello" con la particolarità però di
  considerare eventuali righe che fanno riferimento allo stesso articolo
  come un unico elemento in carrello.

> Supponendo dunque di impostare un filtro del tipo "Elementi distinti
> in carrello maggiore di 2" il Buono Sconto in esame verrà considerato
> valido solo nel caso in cui dovessero essere presenti in carrello
> almeno 3 righe di articoli questa volta **tutti diversi tra loro.**

- **Percentuale Elementi in Carrello**: permette di indicare la
  percentuale di articoli presenti in carrello che dovranno soddisfare
  un eventuale condizione di Filtro Articoli affinché i codici associati
  al Buono Sconto in esame possano effettivamente essere ritenuti
  validi.

> Nel momento in cui l'esigenza dovesse essere dunque quella di non
> validare i codici sconto in una situazione mista e applicarli solo ed
> esclusivamente nel caso in cui tutti gli articoli presenti in carrello
> dovessero soddisfare un'eventuale condizioni di Filtro Articoli, sarà
> allora necessario impostare un Filtro Quantità del tipo "**Percentuale
> elementi in carrello = 100**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promo_percentuale_articoli.bmp](./assets/media/image576.png)

> In queste condizioni se dovessimo avere in carrello anche un solo
> articolo che non soddisfa la condizione impostata all'interno del
> campo "Filtro Articoli" i codici sconto, indipendentemente da tutto il
> resto, non verranno considerati validi.
>
> Allo stesso modo se l'esigenza dovesse essere quella di validare i
> codici sconto quando almeno il 50% delle righe articolo presenti in
> carrello dovessero soddisfare la condizione di Filtro Articoli, sarà
> allora necessario impostare un Filtro Quantità del tipo "**Percentuale
> elementi in carrello maggiore o uguale 50**"
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere impostato nessun
> Filtro Articoli la "Percentuale elementi in carrello" sarà ovviamente
> sempre uguale a 100

- **Percentuale Quantità in Carrello**: permette di indicare quanti
  articoli in percentuale, rispetto alla quantità totale di prodotti
  presenti in carrello, dovranno soddisfare un eventuale condizione di
  Filtro Articoli, affinché i codici associati al Buono Sconto in esame
  possano effettivamente essere ritenuti validi.

> Supponendo dunque che l'esigenza sia quella di dover applicare il
> buono sconto solo nel momento in cui almeno il 30% della quantità
> complessiva di articoli presenti in carrello appartenga alla categoria
> 24 ("Outlet Uomo"), dovremmo configurare una condizione di
> applicabilità del tipo di quella rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promo_percentuale_quantita.bmp](./assets/media/image491.png)

> In questo modo infatti se dovessimo trovarci ad avere in carrello una
> quantità complessiva di 5 prodotti di cui 4 (quindi 80% del totale)
> appartenenti ad una categoria diversa dalla 24 ed uno solo (quindi il
> 20% del totale) appartenente alla categoria 24, la condizione
> impostata non risulterebbe soddisfatta e, di conseguenza, i relativi
> codici sconto non verrebbero validati.
>
> Se invece, in queste stesse condizioni, dovessimo trovarci ad avere in
> carrello una quantità complessiva di 6 prodotti di cui sempre 4 (ossia
> il 67% del totale) appartenenti ad una categoria diversa dalla 24 e i
> restanti 2 (quindi il 33% del totale) appartenenti invece alla
> categoria 24, la condizione impostata sarebbe verificata e, di
> conseguenza, i relativi codici sconto verrebbe correttamente validati.

- **Quantità in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verrà valutata la quantità di riga per ogni
  singolo prodotto che soddisfa l'eventuale filtro impostato. Supponendo
  dunque di considerare una configurazione del tipo di quella
  rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_riga.bmp](./assets/media/image492.png)

> il Buono Sconto verrà effettivamente applicato solo nel momento in cui
> in carrello dovessimo avere almeno un articolo il cui codice inizia
> con AGLIANIC e la sua quantità di riga dovesse essere maggiore o
> uguale a 2
>
> Nelle condizioni indicate con i seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   1

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> il Buono Sconto non verrebbe quindi applicato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due e nessuno di
> essi ha in riga una quantità maggiore o uguale a 2
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   2
  --------------------------------------------------------------------

> il Buono Sconto verrebbe correttamente applicato perché uno dei due
> prodotti che soddisfano il filtro articoli impostato
> (AGLIANICVULDON99) ha effettivamente una quantità di riga uguale a 2

- **Quantità Massima in Riga:** permette di definire una condizione
  sulla quantità di articoli presenti nelle singole righe del carrello.
  Nello specifico, in questo caso, verranno valutati tutti i prodotti
  che soddisfano l'eventuale filtro impostato e tra questi verrà preso
  in considerazione solo quello con la quantità in riga più alta. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata il Buono Sconto verrebbe applicato altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_riga_2.bmp](./assets/media/image493.png)

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il Buono Sconto non verrebbe applicato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il primo ma tale quantità
> (2) non soddisfa comunque la condizione impostata (maggiore o uguale a
> 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   2

  AGLIANICVULROI01                   4

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il Buono Sconto verrebbe correttamente applicato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più alta è il secondo
> (AGLIANICVULROI01) e tale quantità (4) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Quantità Minima in Riga:** permette di definire una condizione sulla
  quantità di articoli presenti nelle singole righe del carrello. Nello
  specifico, in questo caso, verranno valutati tutti i prodotti che
  soddisfano l'eventuale filtro impostato e tra questi verrà preso in
  considerazione solo quello con la quantità in riga più bassa. Se la
  quantità di riga di questo articolo dovesse soddisfare la condizione
  impostata il Buono Sconto verrebbe applicato altrimenti no.

> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_riga_3.bmp](./assets/media/image494.png)

> e supponendo di avere in carrello i seguenti articoli

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   1

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il Buono Sconto non verrebbe applicato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il primo (AGLIANICVULDON99)
> ma tale quantità (1) non soddisfa comunque la condizione impostata
> (maggiore o uguale a 3)
>
> Nel momento in cui, nelle stesse condizioni, dovessimo invece avere i
> seguenti articoli in carrello

  --------------------------------------------------------------------
  PRODOTTO                           QUANTITA' IN CARRELLO
  ---------------------------------- ---------------------------------
  AGLIANICVULDON99                   4

  AGLIANICVULROI01                   3

  BARBARESASILI_00                   3
  --------------------------------------------------------------------

> il Buono Sconto verrebbe correttamente applicato perché i prodotti che
> soddisfano il filtro articoli impostato sono i primi due; tra questi
> quello con la quantità in riga più bassa è il secondo
> (AGLIANICVULROI01) e tale quantità (3) soddisfa correttamente la
> condizione impostata (maggiore o uguale a 3)

- **Sconto in Riga**: permette di definire una condizione di
  applicabilità del Buono Sconto che tenga conto di tutti gli articoli
  presenti in carrello che soddisfano un eventuale "Filtro Articoli", o
  solo di quelli che, oltre a soddisfare un eventuale "Filtro Articoli",
  risultino anche privi di eventuali altri sconti già applicati.

> **ATTENZIONE! l'opzione "Sconto in Riga" è di tipo Stringa**
>
> In conseguenza di ciò per creare una condizione che verrà validata
> solo nel caso in cui i prodotti in carrello che soddisfano un
> eventuale "Filtro Articoli" risultino essere anche privi di altri
> sconti già applicati, **il campo "Valore" della condizione "Sconto in
> Riga" dovrà essere lasciato vuoto (**Valore = Stringa vuota).
>
> Considerando dunque una configurazione del tipo di quella
> rappresentata in figura

![Videate\\promozioni_sconto_in_riga.bmp](./assets/media/image495.png)

> la condizione in esame verrà validata e i relativi codici sconto
> potranno essere correttamente applicati solo nel caso in cui tutti gli
> articoli presenti in carrello (**Percentuale Elementi in Carrello =
> 100**) appartengano alla categoria 24 e siano tutti privi di sconto
> (**Sconto in Riga = stringa vuota**)
>
> Al contrario, se anche tutti gli articoli presenti in carrello
> appartenessero effettivamente alla categoria 24 ma anche uno solo di
> essi avesse già uno sconto applicato (perché ad esempio importato dal
> gestionale) la condizione non verrebbe validata e, di conseguenza, i
> relativi codici sconto non potrebbero essere applicati
>
> **ATTENZIONE!** **si ricorda che nel caso di articoli box (campionari
> standard e configurabili) il prezzo del box stesso viene determinato
> sommando il prezzo dei singoli componenti al netto di eventuali sconti
> ad essi applicati**
>
> In sostanza dunque ad articoli Campionario non verrà mai applicato
> direttamente un determinato sconto.
>
> Nel momento in cui l'esigenza dovesse essere quindi quella di
> considerare non lo sconto dell'articolo campionario in sé ma quello
> eventualmente applicato ai suoi componenti sarà necessario verificare
> di aver correttamente impostato il parametro "**Gestione Articoli
> Box**" presente alla pagina "**Configurazione Catalogo**" del Wizard
> sul valore "**Considera i componenti del Box**".
>
> Per maggiori informazioni in merito a questo parametro si veda anche
> quanto indicato nel relativo capitolo di questo manuale ("*Catalogo --
> Configurazione Parametri Catalogo - Catalogo Mexal / Ho.Re.Ca. --
> Gestione Carrello*")

**Filtro Totale:** consente di impostare un Filtro mediante il quale
poter decidere se la i codici associati al Buono Sconto in esame
dovranno essere considerati validi o meno in relazione a determinati
Totali del documento.

**ATTENZIONE!** l'importo indicato nelle condizioni di filtro dovrà
essere espresso nella valuta definita all'intero del campo **"Valuta di
Riferimento"** presente tra i parametri di configurazione del Buono
Sconto in esame

Cliccando sul pulsante "**Aggiungi Filtro**" verranno quindi
visualizzate le seguenti opzioni:

- **Totale merce ivato / non ivato:** consente di impostare una
  condizione di applicabilità dei codici sconto basata sul Totale merce
  ivato / non ivato del carrello.

> Supponendo quindi di impostare un filtro del tipo "**Totale merce
> ivato maggiore o uguale 50**" i codici sconto verranno considerati
> validi solo nel caso in cui il totale merce ivato / non ivato in
> carrello sia effettivamente maggiore o uguale a 50€

- **Subtotale merce ivato / non ivato:** consente di impostare una
  condizione di applicabilità basata sulla somma dei Totali di Riga
  ivati / non ivati dei soli prodotti in carrello che soddisfano un'
  eventuale condizione di Filtro Articoli impostata per il Buono Sconto
  in questione

> **ATTENZIONE!** Nel momento in cui non dovesse essere presente nessun
> Filtro Articoli anche in questo caso verrà preso in considerazione,
> ovviamente, il Totale merce ivato / non ivato dell'interno carrello

- **Percentuale subtotale merce ivato / non ivato:** consente di
  impostare una condizione di applicabilità basata sulla percentuale del
  subtotale merce (ivato /non ivato) dei soli prodotti in carrello che
  soddisfano un' eventuale condizione di Filtro Articoli in relazione a
  quello che è il totale merce (ivato / non ivato) complessivo
  dell'interno carello.

> Supponendo quindi di configurare una condizione del tipo di quella
> rappresentata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esempio_condizione_percentuale_subtotale.bmp](./assets/media/image496.png)

> i codici sconto verranno considerati validi solo nel caso in cui
> dovessero essere presenti in carrello articoli della categoria 113 il
> cui totale merce, non ivato, risulti maggiore o uguale al 30% del
> totale merce, non ivato, dell'interno carrello

Nella definizione dei Filtri Articolo / Quantità / Totale è anche
possibile, volendo, concatenare tra loro due o più condizioni. Al
termine di ogni condizione, dopo aver impostato operatore relazionale e
relativo valore della condizione, verrà infatti visualizzata una "e",
corrispondente all'operatore logico "AND", e utilizzata, a default, per
concatenare tra loro eventuali ulteriori filtri che dovranno essere
considerati nella definizione della condizione da soddisfare per
l'effettiva applicazione della Promozione.

Cliccando su questo elemento verrà aperta una piccola finestra
all'interno della quale poter selezionare eventuali ulteriori operatori
logici. Le eventuali parentesi, poste prima o dopo questi operatori,
vanno utilizzate esattamente come avviene in algebra, per specificare
quali condizioni dovranno essere valutate prima e quali dopo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_condizione4.bmp](./assets/media/image497.png)

Il parametro "**Gestione Condizioni**" permette di decidere, infine, se
i codici associati al Buono Sconto in esame dovranno essere ritenuti
validi al verificarsi di tutte le condizioni indicate oppure solamente
di un determinato numero di esse.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_condizioni.bmp](./assets/media/image498.png)

In particolare dunque impostando questo parametro sul valore:

- **Tutte le condizioni devono essere soddisfatte**: i codici associati
  al Buono Sconto verranno considerati validi solo ed esclusivamente nel
  momento in cui tutte le condizioni inserite siano state soddisfatte

- **Almeno X condizioni devono essere soddisfatte**: per poter
  considerare validi i codici associati al Buono Sconto in esame è
  sufficiente che siano soddisfatte almeno X condizioni di quelle
  indicate, dove X sarà esattamente il numero specificato in
  corrispondenza del successivo campo "**Numero condizioni (X)**"

