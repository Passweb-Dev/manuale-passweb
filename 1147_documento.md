# DOCUMENTO



All'interno della sezione **Documento** è possibile:

- Gestire e personalizzare il Template utilizzato per la costruzione e
  la visualizzazione del dettaglio dei documenti di Reso Merce in Area
  Riservata, nelle Stampe e nelle varie Email inviate in automatico
  dall'applicazione in corrispondenza dei diversi possibili stati
  assunti da questa particolare tipologia di documenti

- Impostare snippet di codice, utili ad esempio per il tracciamento
  delle conversioni, da poter inserire nella pagina di conferma del
  documento di Reso Merce

Nello specifico il campo:

- **Dettaglio:** consente di impostare e personalizzare il Template
  utilizzato per la costruzione del dettaglio dei documenti di Reso
  Merce che verrà poi visualizzato in **Area Riservata** nel momento in
  cui si dovesse visualizzare uno di questi documenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\reso_dettaglio_ar.bmp](./assets/media/image737.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\reso_dettaglio_ar_esempio.bmp](./assets/media/image738.png)

> **ATTENZIONE! in area riservata è disponibile Bootstrap 5** per cui,
> in fase di realizzazione di questo Template, è possibile utilizzare il
> markup e le classi CSS del relativo framework in maniera tale da
> rendere la pagina di dettaglio perfettamente responsiva

- **Dettaglio Mail:** consente di impostare e personalizzare il Template
  utilizzato per la costruzione del dettaglio dei documenti di Reso
  Merce che verrà poi inserito nelle varie Email inviate in automatico
  dall'applicazione in corrispondenza dei diversi possibili stati
  assunti da questa particolare tipologia di documenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_dettaglio_mail.bmp](./assets/media/image626.png)

![Videate\\ordine_dettaglio_mail_esempio.bmp](./assets/media/image739.png)

> **ATTENZIONE!** si ricorda che i diversi client email interpretano
> ciascuno in maniera diversa il markup HTML utilizzato per costruire la
> mail e supportano solo determinate proprietà CSS (maggiori
> informazioni in merito possono essere trovate anche a questo indirizzo
> <https://www.caniemail.com/> ).
>
> In conseguenza di ciò, in fase di costruzione di questo Template, è
> sempre consigliabile utilizzare un markup e delle proprietà CSS
> correttamente interpretabili dalla maggioranza dei client email
> (tipicamente sarà necessario lavorare sempre con delle tabelle)

- **Dettaglio Stampa:** consente di impostare e personalizzare il
  Template utilizzato per la costruzione del dettaglio dei documenti di
  Reso Merce che verrà poi utilizzato nel momento in cui si dovesse
  decidere di stampare, da Area Riservata o da Front end, uno di questi
  documenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_dettaglio_stampa.bmp](./assets/media/image628.png)

![Videate\\ordine_dettaglio_stampa_esempio.bmp](./assets/media/image629.png)

> **ATTENZIONE!** come per le mail anche in fase di Stampa, non tutto il
> markup HTML e non tutte le proprietà CSS potrebbero essere
> interpretate come avviene effettivamente all'interno di una pagina web
>
> Anche in questo caso quindi, in fase di costruzione di questo
> Template, è sempre consigliabile utilizzare un markup e delle
> proprietà CSS il più standard possibile (tipicamente, come per le
> mail, il consiglio è quello di lavorare sempre con delle tabelle)

- **Codice completamento:** consente di impostare snippet di codice,
  utili ad esempio per il tracciamento delle conversioni, da poter
  inserire nella pagina di conferma del documento di Reso Merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_codice_completamento.bmp](./assets/media/image630.png)

**ATTENZIONE!** Per maggiori informazioni relativamente a come dover
operare per costruire e/o personalizzare il Template che verrà poi
utilizzato in Area Riservata, nelle Mail e in fase di Stampa si veda
anche quanto indicato nel successivo capitolo di questo manuale

##### PERSONALIZZAZIONE DEL TEMPLATE DEI DOCUMENTI DI RESO MERCE

Come indicato nel precedente capitolo di questo manuale i tre campi
"**Dettaglio**", "**Dettaglio** **Mail**" e "**Dettaglio** **Stampa**"
presenti alla pagina "**Configurazione Parametri del Reso**" del Wizard
(tab "**Documento**") consentono di definire e personalizzare il
template che verrà poi utilizzato per i documenti di Reso Merce
rispettivamente, in Area Riservata, nelle mail e in fase di Stampa.

Il modo di operare all'interno di ciascuno dei campi in questione è
sostanzialmente lo stesso.

In questo senso le uniche differenze da prendere in considerazione sono
il fatto che in Area Riservata è disponibile Bootstrap 5 (per cui
possono essere utilizzato un certo tipo di markup e determinate classi
CSS per rendere facilmente tutta la pagina perfettamente responsiva)
mentre in fase di stampa e/o all'interno delle mail dovrà essere
utilizzato un markup diverso e il più standard possibile (tipicamente
sarà necessario lavorare con delle tabelle)

In ogni caso, come detto, il modo di operare all'interno dei 3 editor di
codice è sempre lo stesso. Volendo è possibile aprire l'editor in
modalità full screen utilizzando il tasto funzione **F11**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_mirror_full_screen.bmp](./assets/media/image631.png)

Una volta entrati in modalità full screen è poi possibile ritornare alla
visualizzazione standard utilizzando il tasto **ESC**.

Il pulsante "**Preview**" presente nella parte alta della maschera
consente invece di visualizzare un'anteprima del Template che si sta
realizzando, dove, ovviamente, al posto dei dati reali relativi ad
articoli e clienti, verranno visualizzati appositi segnaposto.

![Videate\\code_mirror_preview_dettaglio_ordine_ar.bmp](./assets/media/image740.png)

In modalità Preview è possibile selezionare uno qualsiasi degli elementi
presenti all'interno del Template.

Cliccandoci sopra si passerà automaticamente alla versione
"**Sorgente**" del template con evidenziata la riga di codice relativa
all'elemento selezionato

All'interno del Wizard nelle pagine in cui è richiesta la
visualizzazione del dettaglio di un documento di Reso Merce (es.
"Gestione Resi") verrà utilizzato un Template predefinito in modo da
evitare il caricamento delle immagini articolo e soprattutto in modo
tale da mantenere la possibilità di variare le note del Reso e/o di
modificare lo stato, la quantità e l'aspetto esteriore dei beni nel
momento in cui il Reso dovesse ancora essere in stato "DA VERIFICARE"
(per maggiori informazioni relativamente alla gestione dei documenti di
Reso Merce si vedano i successivi capitoli di questo manuale).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi5.bmp](./assets/media/image741.png)

La possibilità di intervenire direttamente sul codice HTML dei vari
template offre, indubbiamente, ampie possibilità di personalizzazione,
sia grafiche che a livello di veri e propri contenuti.

Ad esempio la stampa di un reso e/o il dettaglio di questo stesso
documento presente nelle varie mail o visualizzato dagli Agenti in Area
Riservata, potrebbe tranquillamente contenere anche informazioni diverse
rispetto a quelle presenti nella visualizzazione sul front end del sito
del dettaglio di questo stesso documento.

**D'altra parte dovendo intervenire direttamente sul codice HTML questo
tipo di personalizzazione richiede chiaramente specifiche conoscenze
tecniche.**

In questo senso Passweb viene comunque in aiuto dell'utente in due modi
diversi.

Innanzitutto non è necessario creare da zero l'intero template; volendo,
infatti, è anche possibile partire da uno dei modelli preconfigurati
messi a disposizione direttamente da Passweb.

In questo senso cliccando sul pulsante "**Template**" presente in
corrispondenza di ciascuna delle sezioni precedentemente esaminate

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\template_ordini_galleria.bmp](./assets/media/image633.png)

verrà aperta la relativa galleria dei modelli preconfigurati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\template_ordini_galleria_1.bmp](./assets/media/image634.png)

Il pulsante "**Visualizza**" presente in corrispondenza di ciascuno dei
modelli presenti in elenco consente di visualizzare, in un nuovo tab del
browser, un' immagine rappresentativa di quello che dovrebbe poi essere
il risultato finale.

Il pulsante "**Utilizza**" consente invece di caricare, nel campo
corrispondente, il codice HTML e CSS relativo al modello selezionato.

**ATTENZIONE!** Per ovvie ragioni i template messi a disposizione da
Passweb, non conterranno, ad esempio, né attributi articolo né tanto
meno attributi cliente. Potremo trovare in essi la maggior parte dei
campi standard relativi agli articoli in ordine (codice, titolo ...)
agli indirizzi di fatturazione, agli indirizzi di spedizione ... campi
questi che, comunque, potrebbero anche non dover essere utilizzati nel
relativo elemento.

**In sostanza dunque è sempre bene ricordare che i template messi a
disposizione da Passweb sono soltanto un punto di partenza e, nella
maggior parte dei casi, dovranno quindi essere customizzati, sia dal
punto di vista grafico che in termini di contenuti, secondo le
specifiche esigenze del caso**

Nel momento in cui il template messo a disposizione da Passweb non
dovesse quindi soddisfare le specifiche esigenze del caso, e ci fosse la
necessità di modificarlo e/o integrarlo a livello di contenuti ad
esempio con altre informazioni sugli articoli presenti nel documento e/o
sul cliente intestatario, sarà possibile sfruttare uno degli appositi
segnaposto messi a disposizione da Passweb.

In questo senso una volta posizionato il cursore nel punto del template
in cui dovrà essere inserita la nuova informazione, sarà necessario
cliccare sul pulsante "**Seleziona un segnaposto ...**" in maniera tale
da visualizzare l'elenco di tutti i segnaposto disponibili

Selezionando quindi il segnaposto desiderato tra quelli presenti in
elenco, Passweb provvederà poi ad inserire automaticamente nel template
tutto il codice necessario per gestire quello specifico tipo di
informazione.

In questo senso è possibile selezionare differenti tipologie di
segnaposto:

- **Campi Testata Documento:** all'interno di questa sezione è possibile
  trovare i segnaposto relativi ad informazioni da inserire nella
  Testata del documento e che fanno quindi riferimento all' Utente di
  Fatturazione (es. Codice fiscale, Email, Telefono, Partita Iva,
  Indirizzo di fatturazione ecc...), alla Spedizione (es. Indirizzo di
  Spedizione, Metodo di Spedizione ecc...) o al Pagamento (es. Metodo di
  Pagamento).

- **Campi Attributi Documento:** all'interno di questa sezione è
  possibile trovare i segnaposto relativi agli Attributi Passweb gestiti
  per i documenti di Reso Merce e visualizzati nella testata di questi
  stessi documenti.

> E' possibile decidere se inserire o meno queste informazioni
> all'interno del template ma non in maniera individuale, per cui una
> volta deciso di utilizzare anche gli Attributi Ordine questi verranno
> poi inseriti tutti nel template.
>
> In questo senso il segnaposto "**CICLO -- Articoli Documento**",
> presente all'interno di questa sezione, consente di inserire
> l'istruzione necessaria per creare un ciclo di iterazione su questi
> attributi. Selezionando questo elemento nel Template verranno infatti
> inserite le seguenti istruzioni
>
> **\$headerAttributes_entries:{**
>
> **}\$**
>
> Fatto questo andranno poi inseriti tra le due parentesi graffe i
> segnaposto relativi all'etichetta e/o al valore dell'attributo.
>
> **ATTENZIONE!** nel caso in cui i segnaposto relativi all'etichetta
> e/o al valore dell'Attributo Documento non siano stati inseriti
> all'interno di questo ciclo, in fase di generazione del documento non
> saranno sostituiti con i relativi dati.

- **Campi Piede Documento:** all'interno di questa sezione è possibile
  trovare i segnaposto relativi ad informazioni da inserire nel Piede
  del documento e che fanno quindi riferimento, più che altro, ai vari
  Totali (es. Totale Merce, Totale Spese, Abbuoni ecc...)

- **Campi Riga Documento:** all'interno di questa sezione è possibile
  trovare i segnaposto relativi ad informazioni da inserire nelle righe
  del documento e che fano quindi riferimento ai vari articoli. Possiamo
  trovare segnaposto relativi a campi gestionali quali Codice Articolo,
  Categoria Merceologica, Natura, Aliquota IVA ecc..., piuttosto che
  relativi ad un qualsiasi attributo Passweb gestito all'interno del
  sito.

> **Ovviamente questo tipo di informazioni andranno ripetute e
> contestualizzate per ogni singola riga articolo presente nel documento
> per cui i relativi segnaposto, ed il codice HTML "di contorno", andrà
> necessariamente inserito in un apposito ciclo che permetta di ripetere
> l'informazione per ogni singola riga articolo.**
>
> In questo senso il segnaposto "**CICLO -- Articoli Documento**",
> presente all'interno di questa sezione, consente di inserire
> l'istruzione necessaria per gestire questo tipo di ciclo. Selezionando
> questo elemento nel Template verranno infatti inserite le seguenti
> istruzioni
>
> **\$documentItems:{**
>
> **}\$**
>
> In questo modo il codice HTML e i segnaposto inseriti tra le due
> parentesi graffe dell'istruzione sopra evidenziata verranno quindi
> ripetuti e contestualizzati per ogni singola riga articolo presente
> nel documento.
>
> **ATTENZIONE!** nel caso in cui i segnaposto relativi alle
> informazioni sugli articoli non siano stati inseriti all'interno di
> questo ciclo, in fase di generazione del documento non potranno poi
> essere sostituiti con i relativi dati.

- **Condizioni Gruppi:** i segnaposto presenti all'interno di questa
  sezione permettono di inserire nel template del documento delle
  istruzioni mediante le quali poter condizionare la visualizzazione di
  determinate informazioni all'appartenenza dell'utente ad uno dei
  Gruppi Utente gestiti all'interno del sito.

> Supponendo dunque di selezionare il segnaposto "**Se l'utente
> appartiene al Gruppo Clienti Agente Rossi**" (dove "Clienti Agente
> Rossi" è un gruppo creato all'interno dell'apposita sezione del
> Wizard) nel template verranno inserite le seguenti istruzioni
>
> **\$if(id_gruppo)\$**
>
> **\$endif\$**
>
> In questo modo il codice HMTL e i vari segnaposto inseriti tra le due
> istruzioni sopra evidenziate verranno visualizzati, per quel che
> riguarda la Stampa o la visualizzazione del reso in Area Riservata,
> solo ed esclusivamente nel caso in cui l'utente attualmente loggato
> appartenga al gruppo indicato nella condizione.
>
> Per quel che riguarda invece il dettaglio del documento di reso merce
> presente nelle varie mail inviate in automatico dall'applicazione, le
> informazioni inserite all'interno delle due istruzioni sopra
> evidenziate verranno effettivamente inserite solo nel momento in cui
> l'utente che ha generato il documento di reso appartenga al gruppo
> indicato nella condizione.

- **Condizioni Documento:** i segnaposto presenti all'interno di questa
  sezione permettono di inserire nel template del documento delle
  istruzioni mediante le quali poter condizionare la visualizzazione di
  determinate informazioni ad uno specifico stato del documento, ad uno
  specifico metodo di pagamento e / o ad uno specifico metodo di
  spedizione

Di seguito vengono infine riportati alcuni consigli utili relativamente
alla sintassi da utilizzare nel momento in cui si dovesse decidere di
intervenire manualmente sulla personalizzazione del Template.

- Ogni segnaposto o istruzione utilizzata all'interno del template deve
  necessariamente essere inserita tra i caratteri **\$**

> **Esempio di segnaposto**
>
> \$billing_vat\$
>
> **Esempio di ciclo**
>
> \$documentItems:{
>
> }\$
>
> **Esempio di istruzione condizionale**
>
> \$if(isdocumentstatusdone)\$
>
> \$endif\$

- Per fare riferimento ad una specifica informazione di un elemento
  presente all'interno di un ciclo è necessario utilizzare la notazione
  **\$it.codicecampo\$**

> **Esempio**
>
> \$it.entryCode\$ 🡪 Segnaposto del codice articolo inserito all'interno
> del ciclo per la gestione delle righe del documento

- Per utilizzare l'istruzione condizionale if -- else è necessario
  ricorrere alla seguente notazione

> **\$if(condizione)\$**
>
> **.....................**
>
> **\$else\$**
>
> **......................**
>
> **\$endif\$**

- All'interno delle istruzioni condizionali non è possibile utilizzare
  gli operatori AND o OR

- Il carattere \$ è un carattere speciale che, come evidenziato, serve a
  racchiudere ed identificare le diverse istruzioni e i diversi
  segnaposto presenti nel template. **Nel momento in cui dovesse quindi
  essere necessario inserire nel template del documento il \$ come
  semplice carattere, sarà necessario farlo precedere dal carattere \\
  (es .\\\$)**

##### IMPOSTAZIONE DI UN CODICE DI TRACCIAMENTO NELLA PAGINA DI CONFERMA RESO MERCE

Nel momento in cui l'esigenza dovesse essere quella di inserire nella
pagina di Conferma del documento di Reso Merce uno snippet di codice,
utile ad esempio per il tracciamento delle conversioni (es. pixel di
tracciamento per facebook, per Google AdWords ... ), tale snippet dovrà
essere inserito all'interno del campo **"Codice Completamento"**
(*"Ordini -- Gestione Resi -- Configurazione Resi -- Documento"*).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_codice_completamento.bmp](./assets/media/image630.png)

**ATTENZIONE!** Il contenuto del campo "Codice completamento" verrà poi
riportato all'interno della sezione **\< head \>** della thankyou page
cui viene ricondotto l'utente una volta confermato il documento di Reso
Merce.

Volendo è possibile aprire l'editor in modalità full screen utilizzando
il tasto funzione **F11**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_mirror_full_screen2.bmp](./assets/media/image636.png)

Una volta entrati in modalità full screen è poi possibile ritornare alla
visualizzazione standard utilizzando il tasto **ESC**.

Nella creazione dello snippet di codice è possibile utilizzare
determinati segnaposto che verranno poi valorizzati in maniera opportuna
a runtime con specifici valori relativi all' ordine appena confermato ed
utili, quindi, nel momento in cui si volessero tracciare delle
conversioni legate appunto alla conferma dell'ordine.

In questo senso una volta posizionato il cursore nel punto in cui dovrà
essere inserito lo specifico segnaposto sarà poi necessario cliccare sul
pulsante "Seleziona un segnaposto ..." in maniera tale da visualizzare
l'elenco di tutti i segnaposto disponibili.

Selezionando quindi il segnaposto desiderato tra quelli presenti in
elenco, Passweb provvederà poi ad inserire automaticamente nel template
tutto il codice necessario per gestire quello specifico tipo di
informazione.

