# PARAMETRI DEL TRASPORTO



La sezione **"Parametri del Trasporto"** consente di definire e
configurare il tipo di trasporto che dovrà essere utilizzato per il
metodo di spedizione che si sta configurando.

E' all'interno di questa sezione dunque che sarà possibile decidere se
il trasporto della merce acquistata dai clienti che selezioneranno poi
questo particole metodo di spedizione, dovrà essere a carico del
mittente, del destinatario (con ritiro in uno dei punti vendita o dei
fermopoint abilitati) o di un ben preciso Vettore.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_mezzo_vettore.bmp](./assets/media/image278.png)

Nello specifico dunque il parametro

**Trasporto a Mezzo:** consente di definire il tipo di trasporto che
dovrà essere utilizzato per il metodo di spedizione in esame potendo
scegliere tra una delle seguenti opzioni:

- Destinatario

- Mittente

- Vettore

**ATTENZIONE!** Il valore impostato per questo parametro verrà poi
memorizzato nel corrispondente campo del piede del documento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_a_mezzo_mexal.bmp](./assets/media/image279.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_a_mezzo_gestionale.bmp](./assets/media/image280.png)

Dipendentemente dal fatto di considerare trasporti a mezzo mittente,
destinatario o vettore, andranno poi impostati altri specifici parametri
di configurazione. Per maggiori informazioni in merito si vedano anche i
successivi capitoli di questo manuale

##### TRASPORTO A MEZZO DESTINATARIO -- RITIRO IN NEGOZIO

Nel momento in cui in fase di configurazione di un determinato metodo di
spedizione dovessimo decidere di impostare il parametro "**Trasporto a
mezzo**" sull'opzione "**Destinatario**", ciò starà a significare che il
trasporto dovrà essere a carico del destinatario ossia del cliente che
ha acquistato la merce.

Tipicamente questo tipo di trasporto viene quindi utilizzato per
configurare dei ritiri in sede o presso specifici Punti Vendita
opportunamente abilitati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_mezzo_destinatario.bmp](./assets/media/image281.png)

In queste condizioni infatti sarà necessario specificare un valore anche
per i seguenti parametri:

- **Punti Vendita:** consente di indicare i **Punti Vendita** da
  associare alla spedizione. Tali punti vendita saranno poi
  selezionabili dall'utente, in fase di acquisto all'interno del sito,
  nel momento in cui dovesse selezionare effettivamente il metodo di
  spedizione in esame

> Per associare uno o più Punti Vendita al metodo di trasporto in esame
> è sufficiente selezionarli dall'elenco di sinistra ed inserirli nel
> box di destra cliccando sulla piccola freccia rivolta verso destra.
>
> Allo stesso modo per eliminare l'associazione tra il metodo di
> trasporto in oggetto ed un ben preciso punto vendita, è sufficiente
> selezionarlo dal box di destra e cliccare sulla piccola freccia
> rivolta verso sinistra
>
> **ATTENZIONE!** All'interno del campo Punti Vendita verranno
> visualizzati solo ed esclusivamente i Punti Vendita correttamente
> configurati ed abilitati all'interno dell'apposita sezione del Wizard.
>
> Per maggiori informazioni in merito alla configurazione e
> all'attivazione di un Punto Vendita si veda anche la sezione "*Ordini
> -- Configurazione Punti Vendita*" di questo manuale

- **Tipo Porto:** consente di specificare il tipo di porto (Addebito,
  Franco, Assegnato) che dovrà essere impostato sulla spesa di
  spedizione e che verrà poi memorizzato nel corrispondente campo del
  piede del documento (campo **"Porto"**).

> **ATTENZIONE!** **Nel caso in cui le spese di trasporto risultino
> essere maggiori di zero, indipendentemente da quanto impostato
> all'interno di questo campo, la relativa spesa nascerà sul gestionale
> con porto di tipo ADDEBITO e Tipo Spese definito sulla base delle
> impostazioni settate per il successivo parametro "Tipologia di
> Spesa"**
>
> Il valore impostato per questo parametro ha quindi effetto solo ed
> esclusivamente per spese di trasporto pari a 0 (gratuite). Per spese
> maggiori di 0 il porto sarà sempre di tipo Addebito.
>
> Nel caso in cui non venga specificato alcun valore per questo
> parametro, il tipo di porto sarà impostato, a default, sul valore
> ADDEBITO per spese maggiori di 0, sul valore FRANCO per spese invece
> pari a 0.

- **Tipologia di spesa -- solo Ecommerce Mexal:** corrisponde con il
  campo "Tipo Spese" presente nel piede del documento Mexal e consente
  quindi di specificare il criterio di addebito del trasporto che verrà
  poi applicato all'interno del gestionale. E' possibile selezionare uno
  dei seguenti valori:

  - **A Valore Fisso (opzione di default):** selezionando questa opzione
    il campo "Tipo Spese" presente nel piede del documento Mexal verrà
    impostato sul valore "**V**". In queste condizioni nel momento in
    cui si dovessero poi unire, lato gestionale, più ordini in una sola
    bolla le spese di trasporto presenti nei singoli ordini verranno
    sommate tra loro

  - **A Valore Fisso calcolato sulle bolle:** selezionando questa
    opzione il campo "Tipo Spese" presente nel piede del documento Mexal
    verrà impostato sul valore "**B**". A differenza del caso precedente
    in queste condizioni nel momento in cui si dovessero poi unire, lato
    gestionale, più ordini in una sola bolla le spese di trasporto
    presenti nei singoli ordini verranno NON saranno sommate tra loro e
    verrà invece presa una sola volta la spesa di addebito definita
    nelle condizioni del cliente

> **ATTENZIONE!** per maggiori informazioni relativamente alla gestione
> del parametro "Tipo Spese" di Mexal e al suo comportamento in caso di
> unione di più ordini in un\'unica bolla si consiglia di fare
> riferimento alla specifica documentazione di prodotto
>
> In ogni caso è bene sottolineare che nel momento in cui si dovesse
> decidere di impostare il parametro in esame sull'opzione "A Valore
> Fisso calcolato sulle bolle" e si dovesse poi andare, lato gestionale,
> ad unire più ordini in un'unica bolla, il totale documento della bolla
> potrebbe chiaramente non coincidere con la somma dei totali dei
> singoli documenti, documenti questi che il cliente potrebbe anche aver
> già pagata.
>
> Si consiglia quindi di utilizzare questa opzione in maniera
> consapevole e soprattutto non in combinazione con pagamenti online.

##### TRASPORTO A MEZZO MITTENTE

Nel momento in cui in fase di configurazione di un determinato metodo di
spedizione dovessimo decidere di impostare il parametro "**Trasporto a
mezzo**" sull'opzione "**Mittente**", ciò starà a significare che il
trasporto dovrà essere a carico del mittente ossia di chi ha venduto la
merce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_mezzo_mittente.bmp](./assets/media/image282.png)

In queste condizioni sarà necessario specificare un valore anche per i
seguenti parametri:

**Abilita stima costi/consegna -- richiede l'attivazione del modulo
"Stima Trasporto"**

Consente di decidere se il metodo di trasporto in esame dovrà essere
considerato o meno nel calcolo della stima dei costi e dei tempi di
spedizione, informazioni queste che potranno poi essere visualizzata
all'interno del componente Ecommerce "**Spedizione**"

**ATTENZIONE! Per poter visualizzare il parametro in esame e abilitare
di fatto la gestione della stima dei costi e dei tempi di consegna è
necessario attivare, su Passstore, il modulo "Stima Trasporto"**

Per maggiori informazioni relativamente al componente "**Spedizione**" e
a come poter visualizzare una stima dei tempi e dei costi di spedizione
all'interno di componenti quali Scheda Prodotto, Catalogo Ecommerce ...
si veda quanto indicato all'interno dei relativi capitoli di questo
manuale ("*Varianti Responsive -- Lista Componenti Ecommerce --
Componenti interni ai componenti Ecommerce -- Componente Spedizione --
Visualizzazione dei costi di spedizione / tempi di consegna"* )

**Tipo Porto:** consente di specificare il tipo di porto (Addebito,
Franco, Assegnato) che dovrà essere impostato sulla spesa di spedizione
e che verrà poi memorizzato nel corrispondente campo del piede del
documento (campo **"Porto"**).

**ATTENZIONE!** **Nel caso in cui le spese di trasporto risultino essere
maggiori di zero, indipendentemente da quanto impostato all'interno di
questo campo, la relativa spesa nascerà sul gestionale con porto di tipo
ADDEBITO e Tipo Spese definito sulla base delle impostazioni settate per
il successivo parametro "Tipologia di Spesa"**

Il valore impostato per questo parametro ha quindi effetto solo ed
esclusivamente per spese di trasporto pari a 0 (gratuite). Per spese
maggiori di 0 il porto sarà sempre di tipo Addebito.

Nel caso in cui non venga specificato alcun valore per questo parametro,
il tipo di porto sarà impostato, a default, sul valore ADDEBITO per
spese maggiori di 0, sul valore FRANCO per spese invece pari a 0.

**Tipologia di spesa -- solo Ecommerce Mexal:** corrisponde con il campo
"Tipo Spese" presente nel piede del documento Mexal e consente quindi di
specificare il criterio di addebito del trasporto che verrà poi
applicato all'interno del gestionale. E' possibile selezionare uno dei
seguenti valori:

- **A Valore Fisso (opzione di default):** selezionando questa opzione
  il campo "Tipo Spese" presente nel piede del documento Mexal verrà
  impostato sul valore "**V**". In queste condizioni nel momento in cui
  si dovessero poi unire, lato gestionale, più ordini in una sola bolla
  le spese di trasporto presenti nei singoli ordini verranno sommate tra
  loro

- **A Valore Fisso calcolato sulle bolle:** selezionando questa opzione
  il campo "Tipo Spese" presente nel piede del documento Mexal verrà
  impostato sul valore "**B**". A differenza del caso precedente in
  queste condizioni nel momento in cui si dovessero poi unire, lato
  gestionale, più ordini in una sola bolla le spese di trasporto
  presenti nei singoli ordini verranno NON saranno sommate tra loro e
  verrà invece presa una sola volta la spesa di addebito definita nelle
  condizioni del cliente

**ATTENZIONE!** per maggiori informazioni relativamente alla gestione
del parametro "Tipo Spese" di Mexal e al suo comportamento in caso di
unione di più ordini in un\'unica bolla si consiglia di fare riferimento
alla specifica documentazione di prodotto

In ogni caso è bene sottolineare che nel momento in cui si dovesse
decidere di impostare il parametro in esame sull'opzione "A Valore Fisso
calcolato sulle bolle" e si dovesse poi andare, lato gestionale, ad
unire più ordini in un'unica bolla, il totale documento della bolla
potrebbe chiaramente non coincidere con la somma dei totali dei singoli
documenti, documenti questi che il cliente potrebbe anche aver già
pagata.

Si consiglia quindi di utilizzare questa opzione in maniera consapevole
e soprattutto non in combinazione con pagamenti online.

**Gestione Punti Vendita:** consente di decidere se associare o meno al
metodo di spedizione in esame uno o più Punti Vendita. Nel momento in
cui il parametro dovesse essere impostato sul valore SI verrà infatti
visualizzato l'elenco dei Punti Vendita attualmente gestiti all'interno
del sito.

Per associare un Punto Vendita al metodo di spedizione che si sta
codificando è sufficiente selezionarlo dall'elenco di sinistra ed
inserirlo nel box di destra cliccando sulla piccola freccia rivolta
verso destra.

Allo stesso modo per eliminare l'associazione tra il metodo di trasporto
in oggetto ed un ben preciso punto vendita, è sufficiente selezionarlo
dal box di destra e cliccare sulla piccola freccia rivolta verso
sinistra.

**ATTENZIONE!** E' possibile associare al metodo di trasporto solamente
i Punti Vendita per i quali sono state impostate specifiche coordinate
geografiche. In tal senso è possibile effettuare la conversione
automatica "Indirizzo -- Coordinate" mediante l'apposito pulsante
presente nella barra degli strumenti della maschera "Lista dei Punti
Vendita"

**L'associazione delle coordinate geografiche al Punto Vendita è di
fondamentale importanza.**

Solo in presenza di queste coordinate sarà infatti possibile calcolare,
in fase di checkout, l'effettiva distanza tra l'indirizzo di spedizione
indicato dal cliente e i Punti Vendita assegnati al metodo di trasporto
in esame. Tale distanza potrà poi rivelarsi fondamentale nel determinare
se il metodo di trasporto potrà o meno essere selezionabile dall'utente
in fase di checkout.

**La gestione dei Punti Vendita sui Metodi di Trasporto attiva infatti,
in fase di checkout, tutta una serie di controlli per determinare
esattamente quali possano essere le modalità di trasporto effettivamente
selezionabili sulla base dell'indirizzo di spedizione indicato dal
cliente.**

Nello specifico, una volta attivata questa gestione, in fase di checkout
verranno considerate tutte le Modalità di Trasporto per cui è prevista
la gestione dei punti vendita e per ciascuna di esse verrà calcolata
esattamente anche la distanza in km tra questi punti vendita e
l'indirizzo di spedizione indicato dal cliente

Nel momento in cui dovessero essere individuate delle modalità di
trasporto con associate delle aree geografiche compatibili, a livello di
Nazione, Regione, Provincia, Località, Cap con l'indirizzo indicato dal
cliente verrà valutata la distanza (in Km) tra questo stesso indirizzo e
i Punti Vendita associati alla modalità di trasporto in esame.

A questo punto se dovessero essere trovati dei punti vendita la cui
distanza dall'indirizzo di spedizione dovesse essere minore o uguale al
numero massimo di Km impostati per l'area geografica (campo "**Km**"
presente nella maschera di configurazione dell'area) verrà valutato (a
partire da quello più vicino) se a questi punti vendita sono stati
associati o meno anche specifici magazzini.

In caso negativo (nessuna associazione magazzino -- punto vendita) la
modalità di spedizione individuata sarà effettivamente selezionabile
dall'utente. Nel caso in cui al punto vendita dovesse invece essere
stato associato uno specifico magazzino e nel caso in cui tale magazzino
dovesse essere anche uno di quelli impostati per il calcolo della
disponibilità, verrà effettuato un ulteriore controllo relativamente
alla disponibilità, su questo stesso magazzino, degli articoli presenti
in ordine.

**ATTENZIONE!** Affinchè quest'ultimo controllo possa essere effettuato
in maniera corretta è necessario che il parametro "Gestione Acquisto"
(sezione "Disponibilità" della pagina "Configurazione Catalogo" del
Wizard) sia stato impostato su "Acquista solo se disponibile"

Se quest'ultimo controllo dovesse dare esito negativo per tutti i Punti
Vendita che soddisfano le precedenti condizioni la modalità di
spedizione individuata non sarà selezionabile dall'utente.

Se invece per almeno uno di questi Punti Vendita il controllo sulla
disponibilità dovesse dare esito positivo la modalità di spedizione
individuata sarà effettivamente selezionabile e, nel momento in cui
l'utente dovesse effettivamente selezionarla per concludere l'odine, in
testata al documento gestionale verrà messo esattamente il magazzino
associato al Punto vendita più vicino all'indirizzo di spedizione
indicato e per il quale c'è effettivamente disponibilità dei prodotti
presenti in ordine

**ATTENZIONE!** Il calcolo della distanza tra il punto vendita e
l'indirizzo di spedizione indicato dal cliente verrà effettuato
utilizzando apposite chiamate alle API di Google Map. Tale servizio
richiede quindi la corretta impostazione della chiave "**Google Maps
API**" all'interno della relativa sezione alla pagina "Sito --
Preferenze" del Wizard

In ogni chiamata possono essere processati un massimo di 25 Punti
Vendita per cui se i Punti Vendita complessivamente associati alle
diverse modalità di trasporto dovessero essere più di 25, il calcolo
della loro distanza dall'indirizzo di spedizione merce dovrà essere
fatto con due o più chiamate successive rallentando di conseguenza il
caricamento della pagina.

Le API di Google inoltre impongono anche tutta una serie di condizioni
da dover rispettare come ad esempio un numero massimo di chiamate
contemporanee, un numero massimo di chiamate giornaliere ecc... per cui
dipendentemente dai punti vendita complessivamente associati ai vari
metodi di spedizione gestiti si potrebbe incorrere anche in uno degli
errori di seguito indicati:

- **OVER_QUERY_LIMIT**: in presenza di questo errore verranno effettuati
  altri 2 tentativi per calcolare la distanza tra il punto vendita e
  l'indirizzo di spedizione indicato dal cliente. Nel caso in cui
  dovesse permanere l'errore i punti vendita utilizzati nella chiamata
  non verranno valutati

- **INVALID_REQUEST**: in presenza di questo errore i punti vendita
  utilizzati nella chiamata non verranno valutati

- **OVER_DAILY_LIMIT**: in presenza di questo errore i punti vendita
  utilizzati nella chiamata non verranno valutati

- **REQUEST_DENIED**: in presenza di questo errore i punti vendita
  utilizzati nella chiamata non verranno valutati

- **UNKNOWN_ERROR**: in presenza di questo errore i punti vendita
  utilizzati nella chiamata non verranno valutati

- **NOT_FOUND**: in presenza di questo errore il punto vendita non viene
  valutato

- **ZERO_RESULTS**: in presenza di questo errore il punto vendita non
  viene valutato

- **MAX_ROUTE_LENGTH_EXCEEDED**: in presenza di questo errore il punto
  vendita non viene valutato

**ATTENZIONE! Attivando la gestione dei Punti Vendita ogni accesso alla
pagina di checkout effettuato da utenti diversi e/o in diverse sessioni
di navigazione comporterà specifiche chiamate alla API di Google per cui
potrebbe essere più probabile terminare il numero di chiamate gratuite
messe a disposizione da Google passando così ad una fascia a pagamento
del relativo servizio.**

##### TRASPORTO A MEZZO VETTORE

Nel momento in cui in fase di configurazione di un determinato metodo di
spedizione dovessimo decidere di impostare il parametro "**Trasporto a
mezzo**" sull'opzione **Vettore**, ciò starà ad indicare che il
trasporto verrà effettuato da uno specifico Vettore che potrà poi
consegnare la merce direttamente a casa dell'acquirente (o quanto meno
all'indirizzo di spedizione indicato in fase di acquisto) oppure in uno
dei Fermopoint (Punti di ritiro) abilitati.

**ATTENZIONE! Per poter attivare l'opzione del ritiro merce in uno dei
Fermopoint gestiti è necessario aver abilitato, innanzitutto, il
corrispondente modulo su Passstore**

In questo senso è bene sottolineare che, al momento, l'integrazione con
il servizio di consegna e ritiro in Fermopoint è disponibile unicamente
per il vettore **BRT -- Bartolini**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\trasporto_mezzo_vettore.bmp](./assets/media/image283.png)

In queste condizioni dunque, oltre ai parametri "**Tipo di Porto**",
"**Tipologia di Spesa**" e "**Gestione Punti Vendita**" già esaminati
nel precedente capitolo di questo manuale, sarà necessario impostare un
valore anche per i seguenti campi:

**Abilita stima costi/consegna -- richiede l'attivazione del modulo
"Stima Trasporto"**

Consente di decidere se il metodo di trasporto in esame dovrà essere
considerato o meno nel calcolo della stima dei costi e dei tempi di
spedizione, informazioni queste che potranno poi essere visualizzata
all'interno del componente Ecommerce "**Spedizione**"

**ATTENZIONE! Per poter visualizzare il parametro in esame e abilitare
così la gestione della stima dei costi e dei tempi di consegna è
necessario attivare, su Passstore, il modulo "Stima Trasporto"**

Per maggiori informazioni relativamente al componente "**Spedizione**" e
a come poter visualizzare una stima dei tempi e dei costi di spedizione
all'interno di componenti quali Scheda Prodotto, Catalogo Ecommerce ...
si veda quanto indicato all'interno dei relativi capitoli di questo
manuale ("*Varianti Responsive -- Lista Componenti Ecommerce --
Componenti interni ai componenti Ecommerce -- Componente Spedizione --
Visualizzazione dei costi di spedizione / tempi di consegna"* )

**Vettore:** consente di indicare lo specifico vettore da associare al
trasporto attualmente considerato. E' possibile selezionare uno dei
vettori proposti in elenco (Bartolini, DHL, UPS, SDA, TNT Traco, GLS,
Passdelivery), oppure definirne uno "**Personalizzato**" e diverso
quindi da quelli proposti**.**

**ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
creare un metodo di spedizione che possa gestire le consegne mediante
l'applicazione Passepartout Passdelivery, sarà necessario impostare il
campo vettore sulla corrispondente opzione Passdelivery (per maggiori
informazioni in merito si veda anche quanto indicato nel successivo
capitolo "*Spedizioni con Passdelivery*" di questo manuale)

**Url di Ricerca del Number Tracking del Vettore:** indirizzo della
pagina internet messa a disposizione dal vettore per consentire ai
propri clienti di sapere in ogni momento dove si trova la merce spedita.
Per i vettori già cablati all'interno dell'applicazione questo campo
verrà valorizzato automaticamente in base al vettore selezionato. Per i
vettori personalizzati dovrà invece essere indicato manualmente
l'indirizzo della pagina internet cui far riferimento.

**ATTENZIONE!:** **si consiglia di non modificare l'indirizzo associato
a default ai vettori cablati all'interno dell'applicazione**

**In ogni caso è importante verificare che l'indirizzo della pagina
internet inserito nel campo in oggetto abbia al suo interno, in una
posizione che può variare a seconda di quanto richiesto dallo specifico
vettore, il carattere @**.

Tale carattere verrà poi sostituito di volta in volta con il codice di
spedizione associato al relativo documento e passato quindi
all'indirizzo specificato per consentire al cliente di visualizzare il
tracciamento della consegna.

**ATTENZIONE!** Il vettore ed il Number Tracking impostati nei due campi
sopra esaminati verranno utilizzati solo ed esclusivamente per ordini
acquisiti all'interno del proprio sito Ecommerce. Nel caso in cui gli
ordini dovessero essere acquisiti da eventuali Marketplace, il vettore
utilizzato per le spedizioni sarà quello indicato nei successivi campi
"Vettore eBay" e "Vettore Amazon"

Nel caso in cui il campo utilizzato per la gestione del Number Tracking
sia stato correttamente valorizzato, nel momento in cui un utente
dovesse visualizzare, all'interno del sito, il dettaglio del relativo
documento avrebbe la possibilità di visualizzare questo stesso codice
nella parte alta dell'ordine.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\number_tracking1.bmp](./assets/media/image284.png)

Per maggiori informazioni relativamente al campo da utilizzare per la
gestione del Number Tracking, si veda anche quanto indicato all'interno
della sezione *"Ordini -- Configurazione Ordini -- Impostazioni
Generali"* di questo manuale

Inoltre, posto di aver settato correttamente i due campi "**Vettore**" e
"**Url di Ricerca del Number Tracking**", immediatamente al di sotto del
codice di spedizione verrà visualizzato, come indicato nella figura
sopra riportata, un link di collegamento (pulsante "**Segui la
spedizione"**) alla pagina internet messa a disposizione dal vettore
stesso per consentire al cliente di sapere dove si trova esattamente la
merce spedita.

Di base le informazioni relative al tracciamento della spedizione
verranno visualizzate direttamente sul sito del vettore. Passweb in
questo senso si limita a fornire un link di collegamento al sito del
corriere passando alla pagina indicata in fase di configurazione il
codice di spedizione (tracking number) associato al documento in
questione.

**Nel caso in cui il vettore in esame sia quello utilizzato da
Passdelivery**, cliccando sul pulsante "**Segui la Spedizione**"
l'utente verrà invece ridiretto su di una pagina specifica del sito
Ecommerce dove potrà visionare i dati relativi alla consegna effettuata
mediante Passdelivery, dati questi che verranno prelevati in tempo reale
dal corrispondente portale.

**Vettore eBay:** consente di indicare, selezionandolo dall'apposito
menu a tendina, il Vettore che verrà utilizzato nel momento in cui il
metodo di trasporto che si sta codificando dovesse essere utilizzato per
spedire la merce in relazione ad ordini acquisiti da uno dei Marketplace
eBay gestiti

**L'elenco dei vettori presenti all'interno di questo campo è fornito
direttamente da eBay e non può quindi essere modificato in alcun modo**

**ATTENZIONE!** il parametro "Vettore eBay" non è obbligatorio e
andrebbe quindi impostato solo nel caso in cui il metodo di trasporto
che si sta codificando dovesse essere uno dei possibili metodi
utilizzati per spedire la merce in relazione ad acquisti effettuati sul
Marketplace eBay.

**In queste condizioni è inoltre necessario accertarsi che il metodo di
Trasporto che si sta codificando sia correttamente legato ad uno dei
Vettori presenti all'interno del gestionale.**

In caso contrario infatti il processo di spedizione di ordini eBay
potrebbe non andare a buon fine

Per maggiori informazioni in merito si veda anche la sezione "*Catalogo
-- eBay -- Ordini*" di questo manuale

**Vettore Amazon:** consente di indicare, selezionandolo dall'apposito
menu a tendina, il Vettore che verrà utilizzato nel momento in cui il
metodo di trasporto che si sta codificando dovesse essere utilizzato per
spedire la merce in relazione ad ordini acquisiti da uno dei Marketplace
Amazon gestiti

**L'elenco dei vettori presenti all'interno di questo campo è fornito
direttamente da Amazon e non può quindi essere modificato in alcun
modo**

**ATTENZIONE!** il parametro "Vettore Amazon" non è obbligatorio e
andrebbe quindi impostato solo nel caso in cui il metodo di trasporto
che si sta codificando dovesse essere uno dei possibili metodi
utilizzati per spedire la merce in relazione ad acquisti effettuati sui
Marketplace Amazon.

**In queste condizioni è inoltre necessario accertarsi che il metodo di
Trasporto che si sta codificando sia correttamente legato ad uno dei
Vettori presenti all'interno del gestionale.**

In caso contrario infatti il processo di spedizione di ordini Amazon
potrebbe non andare a buon fine

Per maggiori informazioni in merito si veda anche la sezione "*Catalogo
-- Amazon -- Ordini*" di questo manuale

**Codice Gestionale del Vettore (solo Ecommerce Mexal - non
obbligatorio):** consente di indicare il codice mastro di un vettore,
opportunamente codificato all'interno del gestionale (attraverso
un'apposita anagrafica fornitore), che dovrà essere inserito nel piede
del documento nel momento in cui l'utente dovesse selezionare, in fase
di ordine sul sito, il metodo di trasporto in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\codice_gestionale_mexal.bmp](./assets/media/image285.png)

**ATTENZIONE!**: Nel caso in cui venga indicato il codice mastro di un
Vettore non ancora codificato in Mexal, in fase di inserimento ordine
all'interno del gestionale verrà ritornato un errore (Errore
nell\'aggiornamento del documento \-\-- : Errore 1: Conto vettore non
trovato nel piano dei conti) e il documento in esame resterà memorizzato
sul sito.

**Per risolvere il problema sarà quindi necessario impostare all'interno
di questo campo il codice mastro di un vettore effettivamente codificato
in Mexal o, al limite, lasciare il campo vuoto**

**Nome del Vettore (solo Ecommerce Ho.Re.Ca. - non obbligatorio):**
consente di indicare la Ragione Sociale di un vettore, opportunamente
codificato all'interno del gestionale (attraverso un'apposita anagrafica
fornitore), e che dovrà poi essere inserito nel piede del relativo
documento nel momento in cui l'utente dovesse selezionare, in fase di
ordine sul sito, il metodo di trasporto in esame.

**ATTENZIONE!** Il nome inserito all'interno di questo campo serve anche
per agganciare il relativo metodo di trasporto nel processo di
spedizione di ordini eBay. Nel momento in cui il metodo di trasporto che
si sta configurando dovesse quindi essere utilizzato anche come Vettore
eBay per far partire il processo di spedizione con la comunicazione dei
vari cambi di stato anche al Marketplace, è necessario che la Ragione
Sociale del vettore indicato nel piede del documento Ho.Re.Ca. coincida
esattamente con quella inserita all'interno del campo "Nome del Vettore"

**Gestione Punti di ritiro**: consente di attivare, per il metodo di
trasporto in esame, l'opzione di ritiro merce in uno dei Fermopoint
abilitati.

**ATTENZIONE!** Il parametro in oggetto sarà disponibile solo dopo aver
attivato il corrispondente modulo su Passstore

Ovviamente il valore impostato in corrispondenza di questo campo
(selezionabile attraverso un apposito menu a tendina) dovrà essere
coerente con quello che è il vettore effettivamente in uso per il
trasporto in esame (e quindi con quanto impostato ad esempio in
corrispondenza del precedente parametro "Vettore").

In sostanza dunque, se il metodo di trasporto in questione dovesse
essere codificato in relazione, ad esempio, al vettore GLS, non avrebbe
poi alcun senso impostare per il parametro "Gestione Punti di ritiro"
l'opzione "Pudo BRT" corrispondente invece al vettore Bartolini.

I punti di ritiro abilitati verranno prelevati direttamente dal sito del
corrispondente vettore e verranno mostrati all'utente in fase di
checkout sia sotto forma di elenco sia all'interno di un' apposita
Google Map

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_3.bmp](./assets/media/image286.png)

Per maggiori informazioni relativamente a come poter effettivamente
abilitare e utilizzare questa specifica modalità di trasporto in
relazione allo specifico vettore, si veda quanto indicato nei successivi
capitoli di questo manuale

###### PUDO BRT -- BARTOLINI

Di seguito viene illustrata la procedura da seguire per attivare e
configurare correttamente, **in relazione al Vettore Bartolini**, un
metodo di spedizione che preveda l'opzione di consegna merce (a carico
del vettore) e ritiro (a carico dell'utente) in uno dei Fermopoint
abilitati

In questo senso la prima cosa da prendere in considerazione è che tale
opzione non è disponibile a default all'interno del proprio sito Passweb
ma richiede l'attivazione su Passstore del corrispondente modulo.

Una volta attivato tale modulo, e sottoscritto ovviamente il relativo
servizio con il Vettore in questione, sarà poi necessario:

- Inserire la chiave di configurazione, fornita direttamente all'atto
  della sottoscrizione del servizio, all'interno del campo "**BRT -- Api
  key**" presente alla pagina "**Sito -- Preferenze**" del Wizard (tab
  "**Integrazione**" sezione "**Logistica -- BRT**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_1.bmp](./assets/media/image287.png)

> **ATTENZIONE!** Il parametro evidenziato in figura sarà disponibile
> solo dopo aver attivato il corrispondente modulo su Passstore

- Creare un nuovo metodo di spedizione di tipo Passweb secondo quanto
  descritto nei precedenti capitoli di questo manuale e, nello
  specifico, prestare particolare attenzione al fatto di impostare i
  campi "**Trasporto a mezzo**", "**Vettore**" e "**Gestione punti di
  ritiro**", presenti all'interno della sezione "Parametri del
  trasporto" come di seguito indicato:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_2.bmp](./assets/media/image288.png)

> **Trasporto a Mezzo**: **Vettore**
>
> **Vettore: Bartolini**
>
> **Gestione Punti di Ritiro: Pudo BRT**

In queste condizioni nel momento in cui l'utente dovesse selezionare, in
fase di checkout, il metodo di trasporto in esame avrà poi la
possibilità di indicare esattamente il punto di ritiro in cui il
corriere dovrà consegnare la merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_3.bmp](./assets/media/image286.png)

I punti di ritiro verranno prelevati direttamente dal sito del relativo
Vettore e, come evidenziato nella figura sopra riportata, potranno
essere visualizzati sia all'interno di una Google Map sia sotto forma di
elenco con l'indicazione estesa del corrispondente indirizzo.

Inizialmente verranno visualizzati i punti di ritiro ottenuti sulla base
della Città e del C.A.P. indicati nell'indirizzo di spedizione
attualmente in uso per l'utente che sta effettuando l'ordine (in un
range di 40 km). Modificando l'indirizzo di spedizione verranno
aggiornati anche i punti di ritiro.

Inoltre sarà sempre possibile utilizzare anche i campi del form presente
immediatamente al di sopra delle Google Map, per indicare un diverso
indirizzo ed eventualmente anche uno specifico range di km in relazione
al quale ricercare e visualizzare i punti di ritiro effettivamente
disponibili.

In quest' ultimo caso poi è bene sottolineare che:

- **Per ottenere dei punti di ritiro validi** **è necessario indicare
  sia la Città che il C.A.P.** **(entrambi i campi sono dunque
  obbligatori)**

- **I campi relativi all'Indirizzo e al range di km sono invece
  opzionali**

- **Nel momento in cui non dovessero essere specificati Indirizzo e
  Range verranno visualizzati sempre i primi 25 punti di ritiro
  disponibili in un range di 40 km rispetto alla città e al cap
  indicati**

**ATTENZIONE!** I testi dei campi presenti all'interno del form di
ricerca dei punti di ritiro (Città, C.A.P., Indirizzo, Range, pulsante
di ricerca ...) possono essere personalizzati agendo dalla sezione
"Gestione Testi / Messaggi del sito" (componente "Checkout Custom
Ordine")

Una volta concluso l'ordine l'indirizzo del punto di ritiro selezionato
verrà inserito, assieme al documento stesso, all'interno del gestionale.

Nello specifico, nel caso in cui il sito in esame sia **collegato a
Mexal** verrà creato e inserito nella relativa anagrafica degli
indirizzi di spedizione, posto ovviamente che non esista già, un
indirizzo di tipo "Punto di ritiro" che, come tale, non sarà quindi
associato a nessun utente in particolare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_5.bmp](./assets/media/image289.png)

**ATTENZIONE!** Nel campo "**Riferimento**" dell'indirizzo di spedizione
verrà inserito l'identificativo del Punto di ritiro selezionato
dall'utente in fase di acquisto.

Tale indirizzo verrà poi inserito, come indirizzo di spedizione, anche
nel piede del corrispondente documento gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_4.bmp](./assets/media/image290.png)

Nel momento in cui il sito in esame dovesse essere **collegato invece
con uno dei gestionali Ho.Re.Ca.**, non essendo presente una specifica
anagrafica degli indirizzi di spedizione l'indirizzo del punto di ritiro
selezionato dall'utente in fase di acquisto verrà semplicemente inserito
(con anche il relativo codice identificativo) nel piede del
corrispondente documento gestionale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pudo_brt_6.bmp](./assets/media/image291.png)

