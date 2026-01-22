# CATALOGO MEXAL / HO.RE.CA.



All'interno della pagina "**Catalogo Mexal / Ho.Re.Ca.**" accessibile
dalla voce di menu ***"Catalogo -- Configurazione Parametri
Catalogo",*** è possibile impostare alcuni comportamenti di fondamentale
importanza per quella che sarà poi la gestione del proprio catalogo web.

In particolare, come precedentemente evidenziato, all'interno di questa
sezione sarà possibile:

- Specificare se l'applicazione dovrà o meno riconoscere il cliente al
  login, applicandogli eventualmente le specifiche condizioni
  commerciali definite per esso all'interno del gestionale, oppure se
  dovranno essere applicati prezzi e sconti indipendentemente dal
  cliente attualmente loggato

- Specificare come dovrà essere gestita la valuta in uso sul sito nel
  momento in cui un utente dovesse effettuare l'autenticazione

- Definire il numero di decimali sui prezzi da visualizzare all'interno
  del sito

- Specificare se dovranno o meno essere considerati eventuali filtri
  articolo legati ai gruppi di appartenenza del cliente qualora l'ordine
  venga effettuato non direttamente dal cliente ma per suo conto da uno
  degli Agenti abilitati a gestirlo (Siti B2B -- **solo Ecommerce
  Mexal**)

- Definire come dovrà essere gestito il carrello in relazione ad esempio
  al login / logout degli utenti piuttosto che alla specifica modalità
  di inserimento articoli

- Specificare se eventuali articoli gestiti con un massimo/minimo
  fatturabile dovranno o meno essere aggiunti in carrello anche nel caso
  in cui la quantità indicata dall'utente in fase di acquisto non
  dovesse soddisfare le condizioni impostate.

- Specificare la modalità di acquisto degli articoli in catalogo in
  relazione alla loro disponibilità (**aggiornata all'ultima
  sincronizzazione**). Sarà quindi possibile abilitare l'acquisto degli
  articoli in catalogo indipendentemente da quella che è la loro attuale
  disponibilità all'interno di Passweb oppure solo nel caso in cui la
  quantità che si desidera acquistare, per uno specifico articolo, sia
  effettivamente disponibile

- Definire i campi articolo, Passweb o Mexal, da utilizzare per
  costruire un unico campo di ricerca Ecommerce

- Decidere se per determinate tipologie di filtri articolo la query di
  ricerca dovrà essere del tipo "Inizia per" piuttosto che "Contiene"

- Definire quale set di attributi dovrà essere associato alle nuove
  categorie merceologiche importate all'interno del sito

All'interno di questa pagina verrà quindi visualizzata la maschera
**"Configurazione Catalogo"**

![](./assets/media/image1.png)

dove poter specificare un valore per i seguenti parametri:

**Listino:** consente di decidere se utilizzare uno specifico listino
per i prezzi degli articoli presenti all\'interno del negozio web,
indipendentemente dal cliente attualmente loggato, oppure se consentire
all\'applicazione di riconoscere il cliente attualmente loggato sul sito
ed applicargli così, in relazione ai prezzi articolo, le sue specifiche
condizioni commerciali. In particolare dunque, selezionando il valore:

- **Cliente**: selezionando questa opzione prima dell\'autenticazione
  verranno visualizzati i prezzi degli articoli nel listino associato al
  paese di appartenenza dell'utente che sta visitando il sito, secondo
  quanto impostato alla pagina **"*Configurazione -- Parametri Paese,
  Lingua e Valuta -- Gestione Listini"*** del Wizard (per maggiori
  informazioni relative all'associazione di uno specifico listino Mexal
  ad uno specifico paese si veda l'apposita sezione di questo manuale).
  Una volta effettuata l\'autenticazione, l\'applicazione riconoscerà il
  cliente e gli applicherà, in relazione ai prezzi articolo, le sue
  specifiche condizioni commerciali (listini, particolarità prezzo ecc.
  ...).

- **Web:** [selezionando questa opzione l\'applicazione non sarà mai in
  grado di riconoscere il cliente attualmente loggato sul
  sito]{.underline}, per cui sia prima che dopo l\'autenticazione
  verranno visualizzati sempre i prezzi degli articoli nel listino
  associato al paese di appartenenza dell'utente che sta visitando il
  sito, secondo quanto impostato alla pagina **"*Configurazione --
  Parametri Paese, Lingua e Valuta -- Gestione Listini"*** del Wizard.

**Sconto:** consente di decidere se applicare agli articoli presenti
all\'interno del negozio web uno specifico sconto, indipendentemente dal
cliente attualmente loggato, o se consentire all\'applicazione di
riconoscere il cliente attualmente loggato sul sito ed applicargli così,
in relazione agli sconti articolo, le sue specifiche condizioni
commerciali. In particolare dunque, selezionando il valore:

- **Cliente**: selezionando questa opzione prima dell\'autenticazione
  verranno visualizzati, se presenti, eventuali sconti legati al listino
  associato al paese di appartenenza dell'utente che sta visitando il
  sito, secondo quanto impostato alla pagina **"*Configurazione --
  Parametri Paese, Lingua e Valuta -- Gestione Listini"*** del Wizard
  (per maggiori informazioni relative all'associazione di uno specifico
  listino ad uno specifico paese si veda l'apposita sezione di questo
  manuale). Una volta effettuata l\'autenticazione, l\'applicazione
  riconoscerà il cliente e gli applicherà, in relazione agli sconti
  articolo, le sue specifiche condizioni commerciali nel corretto ordine
  di priorità (particolarità sconto, sconto incondizionato, tabella
  sconti-quantità, tabella sconti, sconti su listino).

- **Web**: selezionando questa opzione [l\'applicazione non sarà mai in
  grado di riconoscere il cliente attualmente loggato sul
  sito]{.underline}. In queste condizioni dunque sia prima che dopo
  l\'autenticazione al sito, verrà visualizzato per ogni articolo, se
  presente, lo sconto indicato nel successivo campo "**Sconto Web**".

> **Per i siti Ecommerce collegati a Mexal,** nel caso in cui per il
> campo Sconto Web non sia indicato alcun valore, verranno visualizzati
> eventuali sconti sul listino. Nel caso in cui non siano presenti
> neppure sconti sul listino non verrà visualizzato alcun tipo di
> sconto.

- **Web se non cliente**: selezionando questa opzione prima
  dell\'autenticazione il valore del campo "Sconto Web" verrà preso in
  considerazione solo se presente e se non esistono specifici sconti sul
  listino. Nel caso in cui esistano sconti sul listino verranno invece
  considerati questi indipendentemente da quanto impostato nel campo
  "Sconto Web". Una volta effettuata l\'autenticazione l\'applicazione
  sarà in grado di riconoscere il cliente attualmente loggato e potrà
  quindi applicargli, nel corretto ordine di priorità, le sue specifiche
  condizioni commerciali (particolarità sconto, sconto incondizionato,
  tabella sconti-quantità, tabella sconti, sconti su listino)
  indipendentemente da quanto indicato nel campo "**Sconto Web"**.

> Nel caso in cui il cliente autenticato non abbia definite ne
> all'interno del gestionale, ne tanto meno sul suo gruppo Passweb di
> appartenenza, particolari condizioni commerciali relativamente agli
> sconti, l'applicazione si comporterà esattamente come prima
> dell'autenticazione

**Sconto Web:** attivo unicamente nel caso in cui il precedente
parametro **"Sconto"** sia stato impostato su **"Web"** oppure su **"Web
se non cliente**". Consente di indicare uno specifico sconto, da
applicare ai vari articoli presenti all\'interno del negozio web,
secondo quanto specificato nel precedente campo **\"Sconto\"**. I valori
ammessi sono gli stessi valori attraverso cui vengono definiti gli
sconti all\'interno di Mexal: sconto a valore (es. -10), sconto
percentuale (es. 5.10), sconto percentuale a cascata (es. 5+10+20).
**E\' inoltre accettato il carattere X per indicare \"Nessuno Sconto\".
Inserendo questo valore nel caso in cui il campo "Sconto" sia stato
impostato sul valore "Web" non verrà mai applicato nessuno sconto ne
prima ne dopo l'autenticazione di un eventuale cliente.**

**Prezzo:** consente di specificare la modalità di visualizzazione dei
prezzi (ed eventualmente delle etichette "Iva inclusa / Iva esclusa"
abilitate mediante il successivo parametro "Mostra indicazioni iva") in
relazione alla presenza dell\'Iva oltre che alla tipologia di cliente
attualmente loggato sul sito.

**ATTENZIONE!** L'impostazione settata per questo parametro determinerà
la visualizzazione degli importi e delle relative etichette anche per:

- eventuali tasse addizionali

- importi presenti all'interno del componente spedizione

- eventuali costi aggiuntivi sui pagamenti, sulle spese accessorie e
  sulle spese di spedizione visualizzati nei relativi step del checkout

In particolare poi, selezionando il valore:

- **Iva Cliente**: prima dell\'autenticazione verranno visualizzati, per
  i vari articoli presenti all\'interno del negozio web, prezzi
  comprensivi di Iva. Una volta effettuata l\'autenticazione i prezzi
  visualizzati continueranno ad essere comprensivi di iva nel caso in
  cui ad aver effettuato l\'autenticazione sia stato un cliente
  **\"Privato\"**; saranno invece visualizzati prezzi privi di Iva nel
  caso in cui ad aver effettuato l\'autenticazione sia stato un cliente
  di tipo **\"Azienda\".**

- **Con Iva**: verranno visualizzati, per i vari articoli presenti
  all\'interno del negozio web, **sempre** prezzi comprensivi di Iva sia
  prima dell\'autenticazione sia dopo aver effettuato il login
  indipendentemente, dunque, dalla tipologia di utente che effettua
  l\'accesso.

- **Senza Iva**: verranno visualizzati, per i vari articoli presenti
  all\'interno del negozio web, **sempre** prezzi privi di Iva sia prima
  dell\'autenticazione sia dopo aver effettuato il login
  indipendentemente, dunque, dalla tipologia di utente che effettua
  l\'accesso.

**NOTA BENE:** alle pagine \"Ordine\" e "Carrello" del sito verrà
comunque effettuato lo scorporo o il calcolo dell\'Iva a seconda della
tipologia di documento che si è scelto di generare per la specifica
tipologia di cliente (PR/PX, OC/OX), indipendentemente dunque dal valore
impostato nel campo "Prezzo" sopra indicato.

**NOTA BENE:** un utente non autenticato è considerato sempre come un
utente di tipo privato per cui, nel caso in cui non si fosse ancora
effettuata l'autenticazione al sito, in Carrello verrà comunque
effettuato lo scorporo o il calcolo dell\'Iva a seconda di quanto
impostato per il parametro "Documento Clienti Privati" presente alla
pagina "Configurazione Ordini" del Wizard.

Per maggiori informazioni relativamente alle tipologie di documenti
generati in relazione alle diverse tipologie di utenti (privati o
aziende) si veda anche la sezione *"Ordini -- Gestione Ordini --
Configurazione Ordini -- Impostazioni Generali"* di questo manuale.

**Visualizzazione decimali sui Prezzi:** consente di impostare la
modalità di visualizzazione relativamente al numero di decimali da
utilizzare all'interno del sito per quel che riguarda il prezzo degli
articoli.

Dipendentemente dal fatto di considerare siti Ecommerce collegati a
Mexal o ad uno dei gestionali Ho.Re.Ca. sarà possibile selezionare uno
dei seguenti valori:

**[ECOMMERCE MEXAL]{.underline}**

- **In base alla valuta Mexal:** selezionando questo valore i prezzi
  degli articoli gestiti all'interno del sito verranno visualizzati con
  il numero di decimali impostato in Mexal per la valuta in questione.

![](./assets/media/image2.png)

**NOTA BENE:** per maggiori informazioni relativamente a come gestire in
Mexal i decimali sulle valute si rimanda allo specifico manuale

- **In base al parametro di Magazzino del gestionale:** selezionando
  questo valore i prezzi degli articoli gestiti all'interno del sito
  verranno visualizzati con il numero di decimali impostato in Mexal,
  all'interno del campo "**Num. Decimali in prezzo (0-6)**" della
  tabella "**Parametri di Magazzino**" (*"Anagrafica Azienda -- Dati
  Aziendali -- Parametri di Magazzino"*)

![](./assets/media/image3.png)

**NOTA BENE:** per maggiori informazioni relativamente alla gestione del
parametro sopra evidenziato si rimanda allo specifico manuale Mexal

- **In base alla valuta:** selezionando questo valore i prezzi degli
  articoli gestiti all'interno del sito verranno visualizzati con il
  numero di decimali standard associato al codice ISO della valuta
  attualmente considerata.

> In ogni caso è comunque necessario considerare che:

a.  Il prezzo dei vari articoli pubblicati all'interno del sito verrà
    visualizzato con il numero di decimali definito dalla specifica
    impostazione Mexal sulla valuta o sul Magazzino in base a quanto
    stabilito dal parametro in oggetto

b.  I subtotali presenti in carrello verranno sempre visualizzati con il
    numero di decimali definito, lato gestionale, per la valuta in uso

c.  Per ragioni contabili, e in perfetto accordo con quanto avviene in
    Mexal, i subtotali e i totali documento visualizzati sul sito in
    fase di conferma ordine verranno sempre arrotondati a due soli
    decimali

**[ECOMMERCE HO.RE.CA.]{.underline}**

- **Decimali Ho.Re.Ca.:** selezionando questo valore i prezzi degli
  articoli gestiti all'interno del sito verranno visualizzati
  utilizzando 6 decimali (esattamente come avviene all'interno del
  gestionale)

- **In base alla valuta:** selezionando questo valore i prezzi degli
  articoli gestiti all'interno del sito verranno visualizzati con il
  numero di decimali standard associato al codice ISO della valuta
  attualmente considerata

**Mostra indicazione Iva:** se selezionato, consente di mostrare, in
relazione a determinati componenti, un testo utile per informare gli
utenti relativamente al fatto che l'importo attualmente visualizzato è
da considerarsi o meno comprensivo di Iva.

I componenti interessati sono:

- **Componente Prezzo**

> Selezionando il parametro in esame all'interno del componente
> "Prezzo", oltre all'importo, verrà visualizzata anche un'etichetta
> utile ad indicare se il prezzo in esame dovrà essere considerato o
> meno comprensivo di iva

![](./assets/media/image4.png)

> **ATTENZIONE!!** si ricorda che i prezzi visualizzati all'interno del
> componente Carrello e del componente Checkout saranno o meno ivati (e
> avranno quindi la relativa etichetta) in base allo specifico documento
> che dovrà poi essere generato (nel caso quindi di OC saranno sempre
> prezzi non ivati, nel caso di OX saranno invece sempre prezzi ivati).
>
> In tutti gli altri componenti il fatto di visualizzare prezzi ivati o
> non ivati (con la relativa etichetta) dipenderà invece dalle
> impostazioni settate per il precedente parametro "**Prezzo**", oltre
> che ovviamente dalla particolare tipologia di utenza (privato o
> azienda) che sta navigando il sito
>
> **ATTENZIONE!** nel momento in cui per un determinato articolo dovesse
> essere utilizzata un'esenzione iva, indipendentemente dal valore
> impostato per il parametro in esame, verrà visualizzato soltanto il
> prezzo di quello stesso articolo e non sarà quindi presente nessuna
> indicazione del tipo "Iva inclusa" o "Iva esclusa"

- **Componente Tasse**

> Selezionando il parametro in esame all'interno del componente "Tasse",
> oltre all'importo, verrà visualizzata anche un'etichetta utile ad
> indicare se l'importo della tassa in esame dovrà essere considerato o
> meno comprensivo di iva

![](./assets/media/image5.png)

> **ATTENZIONE!** Come per il prezzo anche l'importo di eventuali tasse
> visualizzate all'interno del componente Carrello e del componente
> Checkout sarà o meno ivato (e avrà quindi la relativa etichetta) in
> base allo specifico documento che dovrà poi essere generato (nel caso
> quindi di OC saranno sempre importi non ivati, nel caso di OX saranno
> invece sempre importi ivati).
>
> In tutti gli altri componenti il fatto di visualizzare importi ivati o
> non ivati (con la relativa etichetta) dipenderà invece dalle
> impostazioni settate per il precedente parametro "**Prezzo**", oltre
> che ovviamente dalla particolare tipologia di utenza (privato o
> azienda) che sta navigando il sito
>
> **ATTENZIONE!** nel momento in cui si dovesse decidere di utilizzare,
> in relazione ad una specifica Tassa, un articolo di tipo Spesa iva
> esente, indipendentemente dal valore impostato per il parametro in
> esame, sul front end del sito verrà poi visualizzato soltanto il costo
> di quella stessa tassa senza nessuna indicazione del tipo "Iva
> inclusa" o "Iva esclusa"

- **Componente Spedizione**

> Selezionando il parametro in esame all'interno del componente
> "Spedizione" verrà visualizzata, in corrispondenza di ogni singolo
> metodo di trasporto anche un'etichetta utile ad indicare se l'importo
> della relativa spesa (posto ovviamente che si sia scelto di
> visualizzare tale informazione) dovrà essere considerato o meno
> comprensivo di iva

![](./assets/media/image6.png)

> **ATTENZIONE!** il fatto di visualizzare all'interno del componente
> spedizione, importi ivati o non ivati dipenderà direttamente dalle
> impostazioni settate per il precedente parametro "**Prezzo** oltre che
> ovviamente dalla particolare tipologia di utenza (privato o azienda)
> che sta navigando il sito
>
> **ATTENZIONE!** nel momento in cui si dovesse decidere di utilizzare,
> in relazione ad uno specifico Metodo di Trasporto, un articolo di tipo
> Spesa iva esente, indipendentemente dal valore impostato per il
> parametro in esame, sul front end del sito verrà poi visualizzato
> soltanto il costo di quello specifico trasporto senza nessuna
> indicazione del tipo "Iva inclusa" o "Iva esclusa"

- **Componente Checkout**

> Selezionando il parametro in esame in fase di checkout, all'interno
> degli step relativi alla selezione del metodo di trasporto e del
> metodo di pagamento verrà visualizzata, in corrispondenza di ogni
> singola voce che dovesse mostrare un costo aggiuntivo (pagamenti,
> spedizioni, spese accessorie), un'etichetta utile ad indicare se
> l'importo di quello stesso costo dovrà essere considerato o meno
> comprensivo di iva

![](./assets/media/image7.png)

> **ATTENZIONE!** il fatto di visualizzare all'interno degli step
> relativi alla selezione del metodo di trasporto e / o del metodo di
> pagamento, costi aggiuntivi ivati o non ivati dipenderà direttamente
> dalle impostazioni settate per il precedente parametro "**Prezzo**
> oltre che ovviamente dalla particolare tipologia di utenza (privato o
> azienda) che sta navigando il sito
>
> **ATTENZIONE!** nel momento in cui si dovesse decidere di utilizzare,
> in relazione ad uno specifico Metodo di Trasporto, ad uno specifico
> Pagamento e/o ad una specifica Spesa Accessoria, un articolo di tipo
> Spesa iva esente, indipendentemente dal valore impostato per il
> parametro in esame, in fase di checkout verrà poi visualizzato
> soltanto l'importo del relativo costo aggiuntivo senza nessuna
> indicazione del tipo "Iva inclusa" o "Iva esclusa"

Il testo da mostrare può essere personalizzato, in tutte le lingue
attualmente gestite, all'interno della sezione "**Sito -- Testi /
Messaggi del Sito -- Testi Generici**" agendo in corrispondenza della
voce "**Iva**"

![](./assets/media/image8.png)

**Gestione Totale Merce:** consente di indicare come dovrà essere
considerato il Totale Merce **nel calcolo delle Spese di Trasporto**,
**delle Spese Accessorie, del Minimo d'ordine e nell'applicazione dei
diversi Metodi di Pagamento.**

E' possibile selezionare uno dei seguenti valori:

- **Non considerare Articoli Spesa in Carrello:** in queste condizioni
  qualora il calcolo delle Spese di Trasporto, delle Spese Accessorie,
  del Minimo d'ordine e/o l'applicazione dei diversi Metodi di Pagamento
  dovesse essere effettuato sulla base del Totale Merce, quello che
  verrà utilizzato per effettuare questi calcoli sarà il Totale Merce al
  netto di eventuali Articoli Spesa aggiunti in Carrello a seguito, ad
  esempio, dell'applicazione di Promozioni e/o Buoni Sconto.

- **Considera Articoli Spesa in Carrello:** in queste condizioni qualora
  il calcolo delle Spese di Trasporto, delle Spese Accessorie, del
  Minimo d'ordine e/o l'applicazione dei diversi Metodi di Pagamento
  dovesse essere effettuato sulla base del Totale Merce, quello che
  verrà utilizzato per effettuare questi calcoli sarà il Totale Merce
  comprensivo anche di eventuali Articoli Spesa aggiunti in Carrello a
  seguito, ad esempio, dell'applicazione di Promozioni e/o Buoni Sconto.

**ATTENZIONE!:** Il parametro "Gestione Totale Merce" ha effetto solo ed
esclusivamente in fase di determinazione delle Spese di Trasporto, delle
Spese Accessorie, del Minimo d'Ordine e della determinazione dei
Pagamenti.

Gli importi relativi alle voci "Totale Merce" e "Spese" presenti nel
piede del documento non verranno quindi influenzati in alcun modo dalle
impostazioni di questo parametro.

**ATTENZIONE!** Nel caso di siti Ecommerce collegati a Mexal, **in
presenza di un vettore abituale con valore in percentuale sul Totale
Merce,** per compatibilità con le logiche gestionali, l'importo delle
Spese di Trasporto **verrà sempre calcolato sul totale merce al netto di
eventuali articoli spesa presenti in carrello,** indipendentemente da
quanto impostato nel Wizard del sito per il parametro \"Gestione Totale
Merce\".

**Gestione Valuta al Login (solo Ecommerce Mexal):** consente di
specificare come dovrà essere gestita la valuta in uso sul sito nel
momento in cui un utente dovesse effettuare l'autenticazione. E'
possibile selezionare uno dei seguenti valori:

- **Corrente:** selezionando questa opzione una volta effettuata
  l'autenticazione verrà comunque mantenuta la valuta attualmente in uso
  sul sito, valuta questa che potrà essere determinata dalla lingua
  impostata sul browser dell'utente che visita il sito, dalla
  corrispondenza tra il suo indirizzo IP e la relativa località
  geografica oppure dalla particolare valuta impostata dall'utente
  stesso mediante l'apposito componente di "Cambio Valuta"

- **Cliente:** selezionando questa opzione una volta effettuata
  l'autenticazione verrà visualizzata, indipendentemente da qualsiasi
  altro parametro di configurazione, la valuta associata, lato
  gestionale, al relativo cliente.

> **ATTENZIONE!** In questo caso è necessario ovviamente che la valuta
> associata, lato gestionale, allo specifico utente sia una delle valute
> effettivamente abilitate e gestite anche all'interno del sito. In caso
> contrario anziché visualizzare la valuta del cliente continuerà ad
> essere visualizzata la valuta corrente

**Gestione Filtri Articoli Agente (solo Ecommerce Mexal):** consente di
decidere se dovranno essere applicati o meno eventuali filtri articolo
associati al gruppo di appartenenza del cliente che effettua l'ordine,
nel momento in cui ad effettuare quest'ordine non sia direttamente il
cliente stesso ma bensì uno degli Agenti abilitati a gestirlo. E'
possibile selezionare uno dei seguenti valori:

- **Considera i filtri articoli Agente e Cliente:** in queste condizioni
  nel caso in cui ad effettuare l'ordine non sia direttamente il cliente
  ma bensì uno degli Agenti abilitati a gestirlo, verranno considerati
  sia i filtri articolo applicati al gruppo di appartenenza dell'Agente
  che quelli eventualmente applicati al gruppo di appartenenza del
  Cliente.

> **L'Agente potrà quindi inserire in carrello solo ed esclusivamente
> gli articoli risultanti dall'intersezione tra i filtri applicati al
> suo gruppo di appartenenza e quelli applicati al gruppo di
> appartenenza del cliente per cui effettua l'ordine**

- **Considera solo i filtri articoli Agente:** in queste condizioni nel
  caso in cui ad effettuare l'ordine sia non direttamente il cliente ma
  bensì uno degli Agenti abilitati a gestirlo, verranno considerati solo
  ed esclusivamente eventuali filtri articolo applicati al gruppo di
  appartenenza dell'Agente.

> **L'Agente potrà quindi inserire in carrello solo ed esclusivamente
> gli articoli che soddisfano eventuali filtri applicati al suo gruppo
> di appartenenza (indipendentemente da eventuali altri filtri articolo
> che potranno o meno essere associati al gruppo di appartenenza del
> cliente per cui effettua l'ordine)**

**Gestione Gruppi Agente**: consente di decidere come dovranno essere
gestiti i Gruppi Utente nel momento in cui ad effettuare l'ordine sul
sito dovesse essere un Agente per conto di un determinato cliente.

E' possibile selezionare uno dei seguenti valori:

- **Considera solo i gruppi Agente:** selezionando questa opzione, nel
  momento in cui ad effettuare l'ordine sul sito dovesse essere un
  Agente per conto di un determinato cliente verranno considerati solo
  ed esclusivamente i Gruppi Utente cui appartiene l'Agente in esame.

> In queste condizioni dunque, nel caso in cui dovesse essere stata
> configurata, ad esempio, una promozione per il Gruppo Utenti cui
> appartiene il cliente per cui l'Agente sta effettuando l'ordine, tale
> promozione non verrà applicata

- **Considera i gruppi Agente e Cliente:** selezionando questa opzione,
  nel momento in cui nel momento in cui ad effettuare l'ordine sul sito
  dovesse essere un Agente per conto di un determinato cliente verranno
  considerati sia i Gruppi di appartenenza dell'Agente che quelli del
  Cliente.

> In queste condizioni dunque, nel caso in cui dovesse essere stata
> configurata, ad esempio, una promozione per il Gruppo Utenti cui
> appartiene il cliente per cui l'Agente sta effettuando l'ordine, tale
> promozione verrà correttamente applicata

**ATTENZIONE!** Il parametro "Gestione Gruppi Agente" non ha alcuna
influenza sugli articoli visualizzati dall'Agente dopo aver selezionato
un determinato cliente. I filtri articolo impostati sui Gruppi Utente
continueranno ad essere gestiti sempre e soltanto secondo quanto
specificato per il parametro "Gestione Filtri Articoli Agente".

