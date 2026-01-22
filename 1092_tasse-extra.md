# TASSE EXTRA



Come già evidenziato all'interno del precedente capitolo, le Tasse Extra
sono tasse addizionali, diverse dall'IVA (es. CONAI, RAEE ecc...), che
dovranno essere applicate agli ordini effettuati all'interno del sito e
il cui importo potrà essere fisso o variare in relazione allo specifico
prodotto.

Per codificare una tassa di questo tipo sarà necessario cliccare sul
pulsante **Aggiungi Tassa**
(![Videate\\pulsante_aggiungi_tassa.bmp](./assets/media/image444.png) ) presente nella barra degli strumenti della maschera
"**Tasse**" precedentemente analizzata e, successivamente, impostare il
parametro "**Tipologia Tassa**" sull'opzione "**Tassa Extra**"

![](./assets/media/image445.png)

I restanti parametri presenti all'interno di questa maschera consentono
rispettivamente di:

- **Valuta di riferimento:** consente di indicare, selezionandola dal
  relativo menu a tendina, la valuta in cui dovranno essere considerati
  gli importi definiti per la tassa in esame.

> **ATTENZIONE!** le valute selezionabili in corrispondenza di questo
> parametro sono quelle attivate all'interno della corrispondente
> sezione del Wizard (menu "*Configurazione -- Paese Linga e Valuta --
> Gestione Valute*")

- **Gestione Tassa**: consente di specificare se, per l'applicazione
  della tassa in esame, dovrà essere considerato un importo fisso oppure
  un importo variabile e diverso per ogni singolo articolo gestito
  all'interno del sito

> E' possibile selezionare una delle seguenti opzioni:

- **Articolo**: selezionando questa opzione l'importo da applicare per
  la tassa in esame potrà variare a seconda dello specifico prodotto in
  ordine e dovrà essere inserito all'interno dell'Attributo Articolo
  indicato in corrispondenza del successivo parametro "**Attributo**"

- **Fissa**: selezionando questa opzione l'importo da applicare per la
  tassa in esame, sarà un importo fisso (indipendente dai prodotti in
  ordine) e dovrà essere indicato all'interno del successivo parametro
  "**Importo Tassa**"

<!-- -->

- **Attributo -- solo per "Gestione Tassa = Articolo"**

> Consente di specificare, selezionandolo tra quelli presenti in elenco,
> l' Attributo Articolo (Passweb o Mexal) che dovrà essere utilizzato
> per indicare, in relazione alla tassa che si sta codificando, l'
> esatto importo cui dovrà essere soggetto un determinato articolo.
>
> **ATTENZIONE! La logica di calcolo che, per una determinata tassa,
> consente di ricavare l'importo cui dovrà essere soggetto un certo
> articolo deve essere gestita esternamente Passweb.**
>
> Indipendentemente dalla logica di calcolo utilizzata, l'importo
> ottenuto andrà poi inserito prodotto per prodotto all'interno
> dell'attributo dichiarato in corrispondenza di questo parametro. Tale
> importo verrà poi utilizzato da Passweb per determinare il prezzo
> complessivo del relativo articolo.
>
> **L'attributo (Passweb o Mexal) utilizzato per gestire gli importi di
> una tassa addizionale dovrà quindi essere un** **attributo di tipo
> numerico.**
>
> In conseguenza di ciò se, in queste condizioni, dovesse essere
> selezionato dal relativo menu a tendina un attributo non numerico, in
> fase di salvataggio verrà visualizzato un apposito messaggio di
> errore.

- **Lingua Attributo**: consente di indicare la lingua di riferimento
  per l'Attributo Articolo dichiarato in corrispondenza del precedente
  parametro.

> **ATTENZIONE**! Questo campo si rivela quindi particolarmente utile
> nel momento in cui si dovesse decidere di utilizzare (per siti
> multilingua) un Attributo Articolo di tipo Passweb
>
> In queste condizioni infatti l'utente non dovrà indicare l'importo
> della Tassa o l'aliquota Iva per tutte le lingue gestite ma solo per
> la lingua indicata in corrispondenza di questo parametro

- **Importo Tassa -- solo per "Gestione Tassa = Fissa"**

> Consente di indicare l'esatto importo da applicare per la tassa in
> esame

- **Tipo di costo:** consente di specificare se l'importo indicato per
  la tassa che si sta codificando dovrà essere considerato o meno
  comprensivo di iva. Sarà quindi possibile selezionare uno dei seguenti
  valori:

  - **Non Ivato:** in questo caso l'importo specificato in
    corrispondenza dell'Attributo Articolo utilizzato per gestire la
    tassa in esame sarà considerato iva esclusa.

> In conseguenza di ciò se ad effettuare l'ordine sul sito dovesse
> essere un privato (generando quindi un OX) su tali importi verrà
> calcolata l'iva. In queste condizioni l'importo della tassa sarà
> dunque quello indicato all'interno dell'Attributo Articolo, o del
> campo "Importo Tassa", maggiorato dell'iva.
>
> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo della tassa
> coinciderà esattamente con quello indicato all'interno dell'Attributo
> Articolo o del campo "Importo Tassa". L'iva verrà comunque calcolata e
> andrà ad influire sul totale della relativa voce presente nel piede
> del documento.

- **Ivato:** in questo caso l'importo specificato in corrispondenza
  dell'Attributo Articolo utilizzato per gestire la tassa in esame o del
  campo "Importo Tassa", sarà considerato iva compresa.

> In conseguenza di ciò se ad effettuare l'ordine sul sito dovesse
> essere un privato (generando quindi un OX) l'importo della tassa
> coinciderà esattamente con quello con quello indicato.
>
> Nel caso in cui ad effettuare l'ordine dovesse invece essere un utente
> di tipo azienda (generando quindi un OC) l'importo della tassa sarà
> quello indicato all'interno dell'Attributo Articolo o del campo
> "Importo Tassa", scorporato dell'iva. L'iva così calcolata andrà
> quindi ad influire sul totale della relativa voce presente nel piede
> del documento.
>
> **ATTENZIONE!** In entrambi i casi il calcolo dell'Iva verrà
> effettuato tendo conto nell'ordine di:

- Eventuali Particolarità IVA attive

- Eventuale assoggettamento Iva specifico per il cliente che effettua
  l'ordine

- Iva OSS (e conseguenti aliquote determinate dal paese di spedizione
  della merce)

- Aliquota iva presente in anagrafica articolo.

> In questo caso inoltre, verrà considerata l'aliquota presente
> nell'anagrafica del singolo prodotto oppure quella presente
> nell'anagrafica dell'articolo spesa utilizzato per gestire la Tassa in
> esame, a seconda del fatto che il successivo parametro "Aliquota Iva"
> sia impostato sull'opzione "Prodotto" o "Articolo Spesa"

- **Articolo:** consente di selezionare l'articolo di tipo Spesa che
  dovrà essere utilizzato, lato gestionale, per gestire la relativa
  Tassa.

> Al fine di poter codificare all'interno del proprio sito E-commerce
> delle tasse addizionali è quindi necessario utilizzare un articolo di
> tipo Spesa opportunamente codificato ed esportato anche all'interno
> del sito (Ecommerce Mexal) oppure marcato come tale all'interno del
> Wizard di Passweb (Ecommerce Ho.Re.Ca.)
>
> Per maggiori informazioni relativamente alla gestione, sui siti
> Ho.Re.Ca., degli articoli di tipo spesa si veda anche la sezione
> "*Configurazione gestionale -- Ho.Re.Ca. Parametri Configurazione
> Gestionale -- Funzionalità di gestione articoli -- Articoli di tipo
> Spesa*" di questo manuale.

- **Aliquota Iva:** consente di indicare se l'aliquota iva da utilizzare
  per il calcolo dell'importo effettivo della tassa dovrà essere, al
  netto di eventuali particolarità e/o di specifici assoggettamenti iva,
  quella del prodotto oppure quella dell'Articolo Spesa utilizzato per
  gestire la tassa in questione.

> E' quindi possibile selezionare uno dei seguenti valori:

- **Prodotto --** opzione di default: selezionando questa opzione **per
  il calcolo dell'importo effettivo della tassa in esame verrà
  utilizzata l'aliquota iva del prodotto cui la tassa stessa fa
  riferimento**

> In conseguenza di ciò, nel momento in cui dovessimo andare ad
> acquistare articoli con aliquote iva differenti, tutti soggetti alla
> medesima tassa, in ordine verrà poi aggiunta una riga relativa
> all'articolo spesa indicato in corrispondenza del precedente parametro
> "Articolo", per ogni diversa aliquota presente sul documento.
>
> Supponendo dunque di acquistare 3 articoli nelle condizioni indicate
> in tabella

  -------------------------------------------------------
  **CODICE**   **QUANTITA'**   **IMPORTO    **ALIQUOTA
                               TASSA**      IVA**
  ------------ --------------- ------------ -------------
  AR1          2               2€           22%

  AR2          1               1€           4%

  AR3          1               0.5€         22%
  -------------------------------------------------------

> a seguito dell'applicazione della tassa in esame verranno aggiunte in
> ordine due ulteriori righe, entrambe relative all'articolo spesa
> indicato in fase di configurazione della tassa, una con importo di
> 4.5€ ed iva al 22% e una con importo pari a 1€ e iva al 4%

- **Articolo Spesa**: selezionando questa opzione **per il calcolo
  dell'importo effettivo della tassa in esame verrà utilizzata
  l'aliquota iva** **impostata sull' articolo spesa** utilizzato per
  gestire la tassa (ed indicato in corrispondenza del precedente
  parametro "Articolo") indipendentemente dal prodotto cui la tassa
  stessa fa riferimento

> In conseguenza di ciò, nel momento in cui dovessimo andare ad
> acquistare articoli con aliquote iva differenti, tutti soggetti alla
> medesima tassa, in ordine verrà poi aggiunta un' unica riga relativa
> all'articolo spesa in esame cui verrà applicata l'aliquota per esso
> definita all'interno del gestionale.

Una volta impostati questi parametri generali, sarà poi possibile
definire anche:

- i Gruppi Utente in relazione ai quali dover eventualmente applicare la
  tassa in esame

- le Zone geografiche (identificate con l'indirizzo di spedizione merce)
  in relazione alle quali dover effettivamente applicare la tassa in
  esame

Per maggiori informazioni in merito a queste due ulteriori operazioni si
vedano anche i successivi capitoli di questo manuale.

