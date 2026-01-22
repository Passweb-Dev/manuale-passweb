# TIPI DI DATO DA VISUALIZZARE



Come già evidenziato nel precedente capitolo di questo manuale il
componente "**Dati Articolo**" può essere mappato con diversi campi
dell'Anagrafica Articoli del gestionale oppure con Attributi Articolo
appositamente creati (siano essi attributi Passweb o Mexal)

Il tipo di dato da visualizzare mediante il componente in oggetto
dipende quindi dalle impostazioni settate per il parametro "**Tipo di
dato da visualizzare**" presente nella sua maschera di configurazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dati_articolo_da_visualizzare.bmp](./assets/media/image518.png){width="4.65in"
height="2.9631944444444445in"}

In particolare nel caso in cui il campo "Tipo di dato da Visualizzare"
sia impostato sul valore:

**Campo Articolo:** sarà possibile selezionare dal sottostante menu a
tendina ("**Campo da Visualizzare**"), e conseguentemente far
corrispondere al Componente "Dati Articolo" che si sta configurando, uno
dei seguenti valori:

- **Titolo Gestionale:** selezionando questo valore il Componente Dati
  Articolo verrà poi mappato con il campo "**Descrizione**"
  dell'Anagrafica Articoli presente all'interno del gestionale. In
  queste condizioni dunque il componente in oggetto verrà valorizzato,
  articolo per articolo, con la relativa descrizione gestionale.

> **ATTENZIONE!** Ovviamente tale opzione dovrebbe essere selezionata
> solo ed esclusivamente nel caso in cui il parametro "**Tipo di dato da
> utilizzare**", presente alla sezione "**Titolo / Permalink
> Articolo***"* della pagina *"Sito --Preferenze -- SEO*" del Wizard sia
> stato impostato su di un valore differente da "**Descrizione
> Gestionale**". In tali condizioni infatti per visualizzare sul sito la
> descrizione presente all'interno del gestionale potrebbe
> tranquillamente essere utilizzato il componente "**Titolo**".
>
> Per maggiori informazioni in merito si veda anche la sezione "*Sito --
> Preferenze -- SEO Titolo / Permalink Articolo*" di questo manuale

- **Alias:** selezionando questo valore il Componente Dati Articolo
  verrà poi mappato con il campo "**Codice Alias**" dell'Anagrafica
  Articoli presente all'interno del gestionale. In queste condizioni
  dunque il componente in oggetto verrà valorizzato, articolo per
  articolo, con l'elenco di tutti i Codici Alias (separati da virgole)
  definiti all'interno del gestionale per l'articolo in esame.

> **ATTENZIONE!** Nel caso di siti collegati ad uno dei gestioni
> Ho.Re.Ca. è possibile mappare il componente "Dati Articolo" anche
> soltanto su una determinata tipologia di codice Alias selezionandola
> tra quelle presenti all'interno del gestionale (es. Alias Code128,
> Alias Code39 ...)

- **Aliquota IVA:** selezionando questo valore il Componente Dati
  Articolo verrà poi mappato con il campo **"Aliquota IVA"**
  dell'Anagrafica Articoli presente all'interno del gestionale. In
  queste condizioni dunque il componente in oggetto verrà valorizzato,
  articolo per articolo, con l'aliquota IVA attualmente impostata per
  esso all'interno del gestionale.

<!-- -->

- **Categoria Merceologica:** selezionando questo valore il Componente
  Dati Articolo verrà poi mappato con la **"Categoria Merceologica"**
  impostata, articolo per articolo all'interno del gestionale.

- **Categoria Statistica Articolo:** selezionando questo valore il
  Componente Dati Articolo verrà poi mappato con il campo **"Categoria
  Statistica"** dell'Anagrafica Articoli presente all'interno del
  gestionale. In queste condizioni dunque il componente in oggetto verrà
  valorizzato, articolo per articolo, con la **descrizione** della
  Categoria Statistica di appartenenza dell'articolo stesso

- **Codice**: selezionando questo valore il Componente Dati Articolo
  verrà poi mappato con il campo **"Codice"** dell'Anagrafica Articoli
  presente all'interno del gestionale. In queste condizioni dunque il
  componente in oggetto verrà valorizzato, articolo per articolo, con il
  corrispondente codice Mexal/Ho.Re.Ca.

- **Codice Alternativo** **--** **valore disponibile solo per siti
  Ecommerce collegati a Mexal.**

> Selezionando questo valore il componente Dati Articolo verrà poi
> mappato con il campo **"Codice Alternativo"** dell'Anagrafica Articoli
> di Mexal. In queste condizioni dunque il componente in oggetto verrà
> valorizzato, articolo per articolo, con il corrispondente codice
> alternativo Mexal.

- **Codice Articolo Fornitore 1 --** **valore disponibile solo per siti
  Ecommerce collegati a Mexal.**

> Selezionando questo valore il Componente Dati Articolo verrà poi
> mappato con il campo "**Codice Fornitore**" del fornitore principale
> (Fornitore 1) presente nella relativa maschera "**Fornitori**"
> all'interno del gestionale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\codice_fornitore.bmp](./assets/media/image519.png){width="4.729861111111111in"
height="2.7055555555555557in"}

> In queste condizioni dunque il componente in oggetto verrà
> valorizzato, articolo per articolo, con il corrispondente codice
> assegnato all'articolo stesso dal fornitore principale.
>
> **ATTENZIONE! Affinchè i dati relativi al fornitore principale
> dell'articolo possano essere visualizzati all'interno del sito è
> necessario che il fornitore stesso sia stato correttamente esportato e
> che sia stato anche associato ad almeno un articolo mediante la
> maschera sopra evidenziata**
>
> Nel caso infatti in cui si decida di esportare e gestire all'interno
> del sito un utente di tipo "Fornitore" senza che questo sia stato
> associato ad almeno articolo, anch'esso gestito all'interno del sito,
> l'utente non verrà riconosciuto come Fornitore ma bensì come Agente.

- **Codice Fornitore 1 --** **valore disponibile solo per siti Ecommerce
  collegati a Mexal.**

> Selezionando questo valore il Componente Dati Articolo verrà poi
> mappato con il codice mastro del fornitore principale (Fornitore 1)
> dell'articolo in questione (es. 601.00001)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\codice_fornitore2.bmp](./assets/media/image520.png){width="4.729861111111111in"
height="2.7055555555555557in"}

- **Nominativo Fornitore 1:** selezionando questo valore il Componente
  Dati Articolo verrà poi mappato con la Ragione Sociale del fornitore
  principale (Fornitore 1) dell'articolo in questione (es. "MGM
  Forniture Elettriche")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\codice_fornitore3.bmp](./assets/media/image521.png){width="4.729861111111111in"
height="2.7055555555555557in"}

> **ATTENZIONE!** Nel caso di siti Ecommerce collegati ad uno dei
> gestionali Ho.Re.Ca. è necessario abilitare, in "**Replica Dati**" il
> canale relativo ai fornitori. In caso contrario non verranno esportate
> sul sito le informazioni dei fornitori e, ovviamene, il componente
> Dati Articolo mappato sul campo in oggetto non potrà essere
> valorizzato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\replica_dati_fornitori.bmp](./assets/media/image522.png){width="4.686805555555556in"
height="2.582638888888889in"}

- **Descrizione Dettagliata**: selezionando questo valore il Componente
  Dati Articolo verrà poi mappato con il campo "**Descrizione
  Dettagliata**" presente all' interno della maschera **"Dati
  Articolo"** qui di seguito riportata e accessibile, in Passweb, dalla
  voce di menu *"Catalogo -- Gestione Articoli"* dopo aver selezionato
  uno specifico articolo ed aver cliccato sul pulsante "Modifica
  Articolo" presente nella barra degli strumenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\descrizione_dettagliata.bmp](./assets/media/image523.png){width="5.809722222222222in"
height="3.3743055555555554in"}

> In queste condizioni dunque il componente "Dati Articolo" verrà
> sostituito, articolo per articolo, con il contenuto del campo sopra
> evidenziato
>
> **ATTENZIONE!** Per i siti Ecommerce collegati a Mexal il campo
> "Descrizione Dettagliata" evidenziato in figura potrà essere
> valorizzato in due modi diversi:

- Direttamente da Passweb attraverso la maschera di "Dati Articolo"
  sopra evidenziata (oppure mediante import massivo di appositi file
  csv)

- Direttamente all'interno del gestionale utilizzando per questo
  l'apposito campo "Descrizione Dettagliata"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\descrizione_dettagliata_mexal.bmp](./assets/media/image524.png){width="3.828472222222222in"
height="1.3680555555555556in"}

> Per maggiori informazioni in merito si veda anche la sezione
> "*Catalogo -- Gestione Articoli -- Articoli -- Anagrafica Articolo /
> Servizio -- Anagrafica Passweb -- Descrizioni*" di questo manuale

- **Descrizione HTML/2/3:** selezionando questo valore il Componente
  Dati Articolo verrà poi mappato con il campo **"Descrizione
  HTML/2/3"** presente all'interno della maschera **"Dati Articolo"**
  qui di seguito riportata e accessibile, in Passweb, dalla voce di menu
  *"Catalogo -- Gestione Articoli"* dopo aver selezionato uno specifico
  articolo ed aver cliccato sul pulsante "Modifica Articolo" presente
  nella barra degli strumenti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\maschera_modifica_articolo.bmp](./assets/media/image525.png){width="5.760416666666667in"
height="3.34375in"}

> In queste condizioni dunque il campo Dati Articolo, verrà sostituito,
> articolo per articolo, con il contenuto del campo "Descrizione
> HTML1/2/3" sopra evidenziato.

- **Disponibilità Indicativa**: selezionando questo valore il Componente
  Dati Articolo verrà mappato, nel caso di **siti Ecommerce collegati a
  Mexal**, con il campo delle videate aggiuntive Mexal appositamente
  riservate a Passweb ed utilizzato per gestire la disponibilità
  indicativa degli articoli presenti all'interno del sito (per maggiori
  informazioni si veda anche la sezione *"Configurazione Gestionale --
  Mexal Parametri Configurazione Gestionale -- Mexal Attivazione Passweb
  -- Gestione Disponibilità Indicativa"* di questo manuale).

> Nel caso invece di **siti Ecommerce collegati ad uno dei gestionali
> Ho.Re.Ca.**, il componente in esame verrà mappato con il
> corrispondente campo presente nell'Anagrafica Passweb del relativo
> articolo. (per maggiori informazioni in merito si veda anche la
> sezione *" Configurazione Gestionale -- Ho.Re.Ca. Parametri
> Configurazione Gestionale -- Funzionalità di gestione Articoli --
> Gestione Disponibilità Indicativa"* di questo manuale).

- **Massimo / Minimo Vendibile:** selezionando questa opzione il
  componente visualizzerà l'eventuale quantità massima / minima di
  vendita impostata per l'articolo in esame

> Per maggiori informazioni in merito alla possibilità di impostare, per
> un determinato articolo una quantità massima/minima di vendita, si
> vedano ad esempio le sezioni "*Configurazione -- Mexal Configurazione
> Gestionale -- Attivazione Passweb -- Funzionalità Mexal Articoli --
> Vendita Articoli per Quantità Massima / Minima*" di questo manuale

- **Natura -- valore disponibile solo per siti Ecommerce collegati a
  Mexal.**

> Selezionando questo valore il Componente Dati Articolo verrà poi
> mappato con il campo "Natura" dell'Anagrafica Articoli di Mexal. In
> queste condizioni dunque il componente in oggetto verrà valorizzato,
> articolo per articolo con la descrizione della Natura associata
> dell'articolo stesso

- **Taglie / Taglie Disponibili --** **valore disponibile solo per siti
  Ecommerce collegati a Mexal.**

> Selezionando uno di questi valori all'interno del Componente Dati
> Articolo verranno visualizzate le Taglie/Colori definite, all'interno
> della corrispondente tabella Mexal, per la serie di appartenenza del
> relativo prodotto.

![Videate\\dati_articolo_taglie_colori.bmp](./assets/media/image526.png){width="5.386805555555555in"
height="3.263888888888889in"}

> I valori mostrati sul front end del sito saranno esattamente quelli
> definiti, in relazione alla serie considerata, all'interno della
> maschera "**Modifica Elementi della serie**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_elementi_serie.bmp](./assets/media/image527.png){width="5.576388888888889in"
height="3.5277777777777777in"}

> considerando anche che il colore eventualmente associato agli elementi
> di una serie verrà effettivamente visualizzato sul front end del sito
> solo per Varianti Responsive
>
> Per maggiori informazioni in merito a come poter personalizzare questi
> elementi si veda anche quanto indicato all'interno del relativo
> capitolo di questo manuale ("*Catalogo -- Gestione Articoli --
> Articoli -- Taglie o Colori (Ecommerce Mexal) -- Personalizzazione
> degli elementi di una serie di taglie/colori*")
>
> Di base dunque nel momento in cui il Componente Dati Articolo dovesse
> essere mappato sul campo "**Taglie**" sul front end del sito verranno
> visualizzati, per ogni singolo prodotto, tutti gli elementi definiti
> all'interno del gestionale per la serie di Taglie/Colori cui
> appartiene l'articolo stesso, indipendentemente dal fatto che quella
> specifica Taglia/Colore sia effettivamente disponibile.
>
> Se invece il Componente Dati Articolo dovesse essere mappato sul campo
> "**Taglie Disponibili**", sul front end del sito verranno
> visualizzate, per ogni singolo prodotto, tra tutti gli elementi
> definiti all'interno del gestionale per la serie di Taglie/Colori cui
> appartiene l'articolo stesso, le sole Taglie/Colori effettivamente
> disponibili.
>
> In realtà occorre considerare anche che il fatto di visualizzare tutte
> le Taglie/Colori di un determinato prodotto o solo quelle
> effettivamente disponibili non dipende solamente dall'aver mappato il
> Componente Dati Articolo sul valore "Taglie" o "Taglie Disponibili" ma
> anche da come si è poi deciso di gestire l'acquisto di quel
> determinato prodotto in relazione a quella che è la sua reale
> disponibilità, o dalla particolare tipologia di prodotto considerata.
>
> In particolare dunque occorre considerare sempre le seguenti
> casistiche:

- Per i **padri di struttura** con articoli figlio gestiti a
  Taglie/Colori, indipendentemente dal fatto di aver mappato il
  componente Dati Articolo su "Taglie" o su "Taglie Disponibili",
  verranno visualizzati sempre tutti gli elementi della serie di
  Taglie/Colori cui appartiene l'articolo stesso (non verranno quindi
  valutate le reali disponibilità di tutti i possibili articoli figlio)

- Nel momento in cui per un determinato articolo dovesse essere gestita
  l'opzione "**Acquista Sempre**" tutte le Taglie/Colori di quel
  determinato prodotto risulteranno essere sempre acquistabili e,
  pertanto, sempre disponibili. E' chiaro quindi che in queste
  condizioni il fatto di mappare il Componente Dati Articolo su "Taglie"
  o su "Taglie Disponibili" non fa alcuna differenza e sul front end del
  sito verranno visualizzate sempre tutte le Taglie/Colori definite
  all'interno del gestionale per la serie di appartenenza del relativo
  prodotto.

- Nel momento in cui per un determinato articolo dovesse essere gestita
  l'opzione "**Acquista solo se disponibile**" e il Componente Dati
  Articolo dovesse essere mappato su "**Taglie Disponibili**" sul front
  end del sito verranno visualizzate le sole Taglie/Colori
  effettivamente disponibili per quel determinato prodotto (posto
  ovviamente che non si parli di un padre di struttura)

- Nel momento in cui per un determinato articolo dovesse essere gestita
  l'opzione "**Acquista solo se disponibile**" e il Componente Dati
  Articolo dovesse essere mappato su "**Taglie**", sul front end del
  sito verranno visualizzate comunque tutte le Taglie/Colori definite
  all'interno del gestionale per la relativa serie di appartenenza ma
  gli elementi relativi alle Taglie/Colori attualmente non disponibili
  verranno automaticamente opacizzati e il loro stile potrà comunque
  essere modificato operando direttamente dallo style editor di Passweb.

- Nel caso di articoli non gestiti a Taglie/Colori o per i quali la
  Taglia/Colore dovesse essere gestita come elemento di struttura e non
  attraverso la relativa tabella gestionale, mappando il Componente Dati
  Articolo su "Taglie" o "Taglie Disponibili" sul front end del sito non
  verrà mai visualizzato alcun valore

<!-- -->

- **Unità di Misura**: selezionando questo valore il Componente Dati
  Articolo verrà mappato con il campo **"Unità di Misura"**
  dell'Anagrafica Articoli presente all'interno del gestionale. In
  queste condizioni dunque il componente in oggetto verrà valorizzato,
  articolo per articolo, con la corrispondente unità di misura
  Mexal/Ho.Re.Ca. (primaria o secondaria dipendentemente dal fatto di
  aver attivato o meno per lo specifico articolo la corrispondente
  funzionalità di gestione dell'unità di misura secondaria)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\dati_articolo_um.bmp](./assets/media/image528.png){width="1.1902777777777778in"
height="2.2944444444444443in"}

> Per maggiori informazioni relativamente alla gestione dell'Unità di
> misura secondaria si rimanda agli specifici capitoli di questo manuale
> presenti all'interno della sezione ("Configurazione Gestionale --
> Mexal/Ho.Re.Ca. Parametri Configurazione Gestionale").
>
> **ATTENZIONE!** Nel caso in cui l'articolo in questione dovesse essere
> venduto a confezioni, oltre a visualizzare l'unità di misura verrà
> sempre visualizzata anche la quantità base della confezione

- **Unità di misura con quantità:** anche in questo caso il Componente
  Dati Articolo verrà mappato con il campo **"Unità di Misura"**
  dell'Anagrafica Articoli presente all'interno del gestionale. A
  differenza del caso precedente però, in queste condizioni, oltre a
  visualizzare l'unità di misura verrà sempre visualizzata, **anche per
  articoli non gestiti a confezione**, la quantità base.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\dati_articolo_um_2.bmp](./assets/media/image529.png){width="1.1902777777777778in"
height="2.2944444444444443in"}

- **Unità di misura della confezione:** anche in questo caso il
  Componente Dati Articolo verrà mappato con il campo **"Unità di
  Misura"** dell'Anagrafica Articoli presente all'interno del
  gestionale. A differenza dei casi precedenti però, il relativo valore
  verrà poi effettivamente visualizzato all'interno del sito solo ed
  esclusivamente in corrispondenza di articoli gestiti a confezione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\dati_articolo_um_3.bmp](./assets/media/image530.png){width="2.423611111111111in"
height="2.2270833333333333in"}

- **Unità di misura Primaria / Secondaria**: selezionando questo valore
  il Componente Dati Articolo verrà mappato con il campo **"Unità di
  Misura"** dell'Anagrafica Articoli presente all'interno del
  gestionale.

> In questo caso però il componente in oggetto verrà sempre valorizzato,
> articolo per articolo, con l' unità di misura Primaria / Secondaria
> definita all'interno del gestionale indipendentemente dal fatto di
> aver attivato o meno per lo specifico articolo la funzionalità di
> gestione dell'unità di misura secondaria.

- **Unità di misura Primaria / Secondaria con Quantità**: come nel caso
  precedente il componente Dati Articolo verrà mappato con il campo
  **"Unità di Misura"** dell'Anagrafica Articoli presente all'interno
  del gestionale e visualizzerà sempre l' unità di misura Primaria /
  Secondaria (indipendentemente dal fatto di aver attivato o meno per lo
  specifico articolo la funzionalità di gestione dell'unità di misura
  secondaria).

> In queste condizioni poi, oltre a visualizzare l'unità di misura verrà
> sempre visualizzata, **anche per articoli non gestiti a confezione**,
> la quantità base

- **Unità di misura Primaria / Secondaria della Confezione**: come nel
  caso precedente il componente Dati Articolo verrà mappato con il campo
  **"Unità di Misura"** dell'Anagrafica Articoli presente all'interno
  del gestionale e visualizzerà sempre l' unità di misura Primaria /
  Secondaria (indipendentemente dal fatto di aver attivato o meno per lo
  specifico articolo la funzionalità di gestione dell'unità di misura
  secondaria).

> In queste condizioni poi il relativo valore verrà effettivamente
> visualizzato all'interno del sito solo ed esclusivamente in
> corrispondenza di articoli gestiti a confezione.

- **Subtotale**: valore disponibile solo nel caso in cui il componente
  "Dati Articolo" sia stato inserito all'interno di un componente
  "Custom" (es. **Carrello Custom**, Ordine Custom, Prenotazione Custom
  ecc..). In queste condizioni il componente visualizzerà il totale di
  riga per ogni articolo presente, ad esempio, in carrello, valore
  questo ottenuto sulla base del prezzo dell'articolo e, ovviamente,
  delle quantità in ordine.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\dati_articolo_subtotale.bmp](./assets/media/image531.png){width="5.055555555555555in"
height="3.6013888888888888in"}

- **Provvigione --** **valore disponibile solo per siti Ecommerce
  collegati a Mexal**.

> Valore disponibile solo nel caso in cui il componente "Dati Articolo"
> sia stato inserito all'interno del componente "**Carrello Custom**".
> In queste condizioni il componente visualizzerà il valore della
> provvigione relativa allo specifico articolo presente in carrello e
> **ottenuta dall'Agente che sta effettuando l'ordine per un conto di un
> certo cliente**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\dati_articolo_provvigione.bmp](./assets/media/image532.png){width="5.055555555555555in"
height="3.6013888888888888in"}

- **Nota -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Beauty o Menu e componente Dati
    Articolo inserito all'interno di una "**Prenotazione Custom**" o di
    una "**Prenotazione Tavolo Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente eventuali note, **inserite lato gestionale**, all'interno
> della prenotazione.

- siti Ecommerce collegati a Mexal e componente Dati Articolo inserito
  all'interno di una **Lista Regalo**.

> In queste condizioni il componente consentirà di visualizzare
> all'interno della Lista Regalo l'eventuale nota inserita per il
> corrispondente articolo in fase di creazione della Lista Regalo.

- **Priorità** **-- valore disponibile nelle seguenti condizioni:**

  - componente Dati Articolo inserito all'interno di una **Lista
    Regalo**

> In queste condizioni il componente Dati Articolo visualizzerà la
> priorità inserita per il corrispondente articolo in fase di creazione
> della Lista Regalo. Nello specifico ad essere visualizzata sarà
> ovviamente la descrizione associata alla relativa priorità e non,
> ovviamente, il suo valore numerico (utilizzato invece per gestire
> l'ordinamento della lista)

- **Data** **-- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Beauty o Menu e componente Dati
    Articolo inserito all'interno di una "**Prenotazione Custom**" o di
    una "**Prenotazione Tavolo Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente la data della prenotazione

- **Durata -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Beauty e componente Dati Articolo
    inserito all'interno di una "**Prenotazione Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente la durata del servizio/trattamento prenotato

- **Risorse -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Beauty e componente Dati Articolo
    inserito all'interno di una "**Prenotazione Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente la risorsa associata al servizio/trattamento prenotato

- **Coperti -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Menu e componente Dati Articolo
    inserito all'interno di una "**Prenotazione Tavolo Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente il numero di coperti prenotati

- **Sala -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Menu e componente Dati Articolo
    inserito all'interno di una "**Prenotazione Tavolo Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente la sala prenotata

- **Tavoli -- valore disponibile nelle seguenti condizioni:**

  - siti collegati ai gestionali Menu e componente Dati Articolo
    inserito all'interno di una "**Prenotazione Tavolo Custom**"

> In queste condizioni il componente Dati Articolo visualizzerà
> esattamente i tavoli prenotati

Nel momento in cui l'esigenza dovesse invece essere quella di
visualizzare, mediante il componente "Dati Articolo" uno degli Attributi
Articolo gestiti all'interno del sito, sarà necessario impostare il
componente "**Tipo di dato da visualizzare**" sul valore "**Attributo
Articolo**"

**Attributo Articolo**: in questo caso sarà possibile selezionare dal
sottostante menu a tendina ("**Attributo da Visualizzare**") solo ed
esclusivamente uno degli Attributi Articolo (siano essi di tipo Mexal
siano essi di tipo Passweb) precedentemente codificati all'interno della
corrispondente sezione del Wizard.

Nello specifico, in relazione ad Attributi Articolo di tipo Mexal, sarà
possibile selezionare:

- attributi mappati con campi di "Videate Aggiuntive Articoli"

- attributi mappati con campi di tabelle di tipo "Anagrafica MyDB" che
  sono estensioni Standard o Riportabili delle tabelle Articoli

- i campi corrispondenti alle Funzionalità Mexal "Ulteriore Descrizione
  1/2/3" essendo essi a tutti gli effetti campi di una specifica Videata
  Aggiuntiva Articoli di Mexal.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> degli Attributi Articolo ed al processo di categorizzazione degli
> articoli gestiti all'interno del sito si rimanda alla relativa sezione
> di questo manuale (Catalogo -- Gestione Attributi Articoli).

**Separatore** -- visibile solo nel caso in cui il campo "Tipo di dato
da visualizzare" sia stato impostato sul valore "Attributo Articolo".

Consente di indicare il carattere che dovrà essere utilizzato come
separatore dei diversi valori presenti all'interno dell'Attributo
selezionato.

Tale campo è quindi utile solo nel caso in cui l'attributo in esame sia
a valori multipli. Sono accettati anche tag HTML per cui se l'esigenza
dovesse essere quella di mandare a capo i diversi valori presenti
all'interno dell'Attributo selezionato sarà sufficiente inserire
all'interno di questo campo il tag \<br\>

