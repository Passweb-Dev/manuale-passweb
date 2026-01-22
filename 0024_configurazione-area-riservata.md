# CONFIGURAZIONE -- AREA RISERVATA



Come già indicato nel precedente capitolo di questo manuale la sezione
"**Area Riservata\"** consente di impostare i principali parametri di
configurazione relativi all'Area Riservata del proprio sito Passweb.

![](./assets/media/image9.png)

Nello specifico il parametro:

**App Area Riservata:** consente di decidere quale App e quindi quali
sezioni dell'Area Riservata abilitare o non abilitare.

In questo senso dunque il parametro:

- **Messaggi**: consente, se selezionato, di abilitare l'App attraverso
  cui poter gestire l'invio e la ricezione di messaggi con utenti
  abilitati ad accedere in area riservata

![Videate\\ar_messaggi.bmp](./assets/media/image10.png)

- **Agenda:** consente, se selezionato, di abilitare l'App attraverso
  cui poter gestire la consultazione e l'inserimento di attività,
  scadenze o appuntamenti in Agenda

![Videate\\ar_agenda.bmp](./assets/media/image11.png)

- **Documenti:** consente, se selezionato, di abilitare l'App attraverso
  cui poter gestire lo scambio di generici documenti con utenti
  abilitati ad accedere in Area Riservata

![Videate\\ar_documenti.bmp](./assets/media/image12.png)

- **Business:** consente, se selezionato, di abilitare due distinte App,
  **Clienti** e **Ordini**, mediante le quali ogni Agente avrà la
  possibilità di gestire i propri clienti e i relativi ordini.

![Videate\\ar_ordini.bmp](./assets/media/image13.png)

![Videate\\ar_clienti.bmp](./assets/media/image14.png)

> Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.
> verrà abilitata, per ovvie ragioni, la sola App Ordini
>
> **ATTENZIONE!** il parametro in questione determina anche la
> visualizzazione o meno della sezione "**Riepilogo Ecommerce**"
> presente in bacheca

![Videate\\ar_riepilogoecommerce.bmp](./assets/media/image15.png)

> Tale sezione verrà quindi visualizzata solo nel momento in cui il
> check "Business" dovesse essere correttamente abilitato.

- **Docuvision (Ecommerce Mexal):** consente, se selezionato, di
  abilitare l'App attraverso cui poter prelevare in tempo reale i
  documenti associati all'interno del gestionale (in Docuvision) alla
  propria anagrafica utente

![Videate\\ar_docuvision.bmp](./assets/media/image16.png)

- **Sprix (Ecommerce Mexal):** consente, se selezionato, di abilitare
  per gli Agenti di un sito Business To Business, l'App attraverso cui
  poter visualizzare ed eseguire direttamente da web gli sprix
  correttamente mappati all'interno della corrispondente sezione del
  Wizard

![Videate\\ar_sprix.bmp](./assets/media/image17.png)

**NOTA BENE**: per maggiori informazioni relativamente alla funzionalità
e all'utilizzo dell'area riservata di un sito Ecommerce si veda anche il
capitolo "Business To Business -- Area Riservata" di questo manuale.

Il campo "**Code Snippet Area Riservata**"

![](./assets/media/image18.png)

consente invece di inserire codice CSS e/o Javascript (iniettato poi in
apposti tag \< style \> e \< script \>) che verrà riportato in tutte le
pagine dell'Area Riservata e che potrebbe quindi rivelarsi
particolarmente utile nel momento in cui fossero necessarie alcune
personalizzazioni al layout di queste stesse pagine.

**ATTENZIONE!** l'utilizzo di questa sezione richiede specifiche
conoscenze lato CSS e Javascript per cui un suo utilizzo non consapevole
potrebbe anche pregiudicare la visualizzazione ed il funzionamento di
tutta l'area riservata.

La sezione "**Dashboard Cliente**", visibile solo per Siti Ecommerce
(Mexal e Ho.Re.Ca.), consente invece di decidere quali dati statistici
dovranno essere visualizzati, nella Dashboard dell'Area Riservata, nel
momento in cui ad effettuare il login dovesse essere un cliente
appositamente abilitato ad accedere a questa specifica sezione del sito.

![](./assets/media/image19.png)

In questo senso il parametro:

**Ordini:** consente, se attivato, di visualizzare nella Dashboard
dell'Area Riservata i dati relativi a:

- Totale Vendite

- Numero Ordini

- Valore medio Ordini

- Ultimi 10 Ordini

- Articoli più visiti

- Articoli più Venduti

**Pagamenti**: consente, se attivato, di visualizzare nella Dashboard
dell'Area Riservata i dati relativi a:

- Pagamento più utilizzato

**Trasporti**: consente, se attivato, di visualizzare nella Dashboard
dell'Area Riservata i dati relativi a:

- Trasporto più utilizzato

**Resi**: consente, se attivato, di visualizzare nella Dashboard del
Wizard i dati relativi a:

- Numero Resi

**Importi**: consente di definire la tipologia degli importi
visualizzati in Area Riservata relativamente a "Ordini" e "Carrelli
Abbandonati". E' possibile selezionare una delle seguenti opzioni:

- **Totale**: selezionando questa opzione le statistiche relative ad
  Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Ordine**" e il "**Totale Carrello**"

- **Totale Merce**: selezionando questa opzione le statistiche relative
  ad Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Merce Ordine**" e il "**Totale Merce Carrello**"

**Gestione Iva**: consente di indicare come dovrà essere gestita l'IVA
in relazione agli importi visualizzati in Area Riservata. E' possibile
selezionare una delle seguenti opzioni:

- **Ivato**: selezionando questa opzione nella Dashboard dell'Area
  Riservata dei Clienti verranno visualizzati sempre e comunque importi
  Ivati

- **Non Ivato**: selezionando questa opzione nella Dashboard dell'Area
  Riservata dei Clienti verranno visualizzati sempre e comunque importi
  non Ivati

- **Iva Cliente**: selezionando questa opzione nella Dashboard dell'Area
  Riservata dei Clienti verranno visualizzati:

  - importi Ivati nel momento in cui l'utente connesso dovesse essere un
    Privato

  - importi non Ivati nel momento in cui l'utente connesso dovesse
    essere un'Azienda

**ATTENZIONE!** nel momento in cui dovessero essere variate delle
impostazioni relative ai parametri presenti all'interno della sezione
"Dashboard Cliente", eventuali clienti connessi in Area Riservata
potranno visualizzare le modifiche apportate solo dopo aver effettuato
un logout e un successivo login

La sezione "**Dashboard Agente**", visibile solo per Siti Ecommerce
collegati a Mexal consente, infine, di decidere quali dati statistici
dovranno essere visualizzati, nella Dashboard dell'Area Riservata, nel
momento in cui ad effettuare il login dovesse essere un Agente
appositamente abilitato ad accedere a questa specifica sezione del sito.

![](./assets/media/image20.png)

In questo senso il parametro:

**Ordini:** consente, se attivato, di visualizzare nella Dashboard
dell'Area Riservata i dati relativi a:

- Totale Vendite

- Numero Ordini

- Valore medio Ordini

- Ultimi 10 Ordini

- Articoli più visiti

- Articoli più Venduti

- Clienti

**Resi**: consente, se attivato, di visualizzare nella Dashboard
dell'Area Riservata i dati relativi a:

- Numero Resi

**Carrelli abbandonati**: consente, se attivato, di visualizzare nella
Dashboard dell'Area Riservata i dati relativi a:

- Numero Carrelli Abbandonati

- Valore Carrelli Abbandonati

**Importi**: consente di definire la tipologia degli importi
visualizzati in Area Riservata relativamente a "Ordini" e "Carrelli
Abbandonati". E' possibile selezionare una delle seguenti opzioni:

- **Totale**: selezionando questa opzione le statistiche relative ad
  Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Ordine**" e il "**Totale Carrello**"

- **Totale Merce**: selezionando questa opzione le statistiche relative
  ad Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Merce Ordine**" e il "**Totale Merce Carrello**"

**Gestione Iva**: consente di indicare come dovrà essere gestita l'IVA
in relazione agli importi visualizzati in Area Riservata. E' possibile
selezionare una delle seguenti opzioni:

- **Ivato**: selezionando questa opzione nella Dashboard dell'Area
  Riservata degli Agenti verranno visualizzati sempre e comunque importi
  Ivati

- **Non Ivato**: selezionando questa opzione nella Dashboard dell'Area
  Riservata degli Agenti verranno visualizzati sempre e comunque importi
  non Ivati

**ATTENZIONE!** nel momento in cui dovessero essere variate delle
impostazioni relative ai parametri presenti all'interno della sezione
"Dashboard Agente", eventuali Agenti connessi in Area Riservata potranno
visualizzare le modifiche apportate solo dopo aver effettuato un logout
e un successivo login

Per comprendere meglio i valori che potrebbero essere visualizzati in
Area Riservata considerando le diverse possibili combinazioni dei due
parametri "**Importi**" e "**Gestione Iva**", consideriamo un semplice
esempio.

Supponiamo di dover prendere in considerazione **un solo ordine
effettuato da un utente di tipo Azienda** i cui totali sono esattamente
quelli rappresentati in figura

![](./assets/media/image21.png)

- Totale Merce: 203.52€

- Spese: 73.33€

- Iva: 55.37€

- Totale Documento: 332.22€

Nello specifico poi la voce "Iva" che raccoglie, ovviamente, l'iva sui
prodotti in ordine più, eventualmente, l'iva su spese aggiuntive (es.
Spese di trasporto, Spese accessorie, Spese sui pagamenti ...) gestite
mediante l'inserimento di appositi articoli di tipo Spesa è così
composta:

- 40.7€ 🡪 Iva sui prodotti

- 11€ 🡪 Iva sulle spese di trasporto (art. SPTRASPORTO)

- 1.67€ 🡪 Iva sulle spese accessorie (art. SPESE-ACCESSIORIE)

- 2€ 🡪 Iva sulle spese di pagamento (art. SPESE-ACCESSIORIE)

In queste condizioni, dipendentemente dalle impostazioni settate per i
parametri "**Importi**" e "**Gestione Iva**" l'indicatore "**Totale
Vendite**", presente nelle statistiche della Dashboard di Area
Riservata, potrà visualizzare i seguenti importi:

- "Importi = Totale" e "Gestione Iva = Iva Cliente"

> **Totale Vendite = 276.85€** -- ottenuto come "Totale Documento --
> Totale Iva"
>
> (considerando che l'utente in esame è un utente di tipo Azienda
> l'importazione "Gestione Iva = Iva Cliente" coincide con "Gestione Iva
> = Non Ivato")

- "Importi = Totale" e "Gestione Iva = Non Ivato"

> **Totale Vendite = 276.85€** -- ottenuto come "Totale Documento --
> Totale Iva"

- "Importi = Totale" e "Gestione Iva = Ivato"

> **Totale Vendite = 332.22€** -- coincidente con il "Totale Documento"

- "Importi = Totale Merce" e "Gestione Iva = Iva Cliente"

> **Totale Vendite = 203.52€** -- coincidente con il "Totale Merce"
>
> (considerando che l'utente in esame è un utente di tipo Azienda
> l'importazione "Gestione Iva = Iva Cliente" coincide con "Gestione Iva
> = Non Ivato")

- "Importi = Totale Merce" e "Gestione Iva = Non Ivato"

> **Totale Vendite = 203.52€** -- coincidente con il "Totale Merce"

- "Importi = Totale Merce" e "Gestione Iva = Ivato"

> **Totale Vendite = 244.22€** -- ottenuto come "Totale Merce + Iva
> Prodotti"

Nel momento in cui l'esigenza dovesse essere, ad esempio, quella di far
visualizzare agli Agenti nelle statistiche della Dashboard di Area
Riservata importi calcolati esclusivamente sul Totale Merce escludendo
anche eventuali articoli di tipo spesa presenti nel corpo del documento,
sarà necessario impostare il parametro "Importi" sul valore "Totale
Merce" e "Gestione Iva" sul valore "Non Ivato"

