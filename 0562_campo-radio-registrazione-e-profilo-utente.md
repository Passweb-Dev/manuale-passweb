# CAMPO RADIO (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Radio"**

![](./assets/media/image95.png)

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente un modulo a scelta multipla di tipo "Radio Button", modulo che
per sua natura ammette la selezione di una sola scelta tra quelle
disponibili (una volta cliccato su un'opzione, facendo click su un'altra
la prima selezione verrà automaticamente deselezionata)

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image96.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di impostare un nome per il Componente che si sta
editando.

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Tab Index:** consente di personalizzare l'ordine di tabulazione del
form assegnando uno specifico numero d'ordine al campo in oggetto. Una
volta assegnato un numero d'ordine ad ogni campo del form sarà poi
possibile spostarsi da un elemento all'altro, utilizzando il tasto "TAB"
e secondo l'ordine di tabulazione impostato.

Nel caso in cui si decida di personalizzare l'ordine di tabulazione
degli elementi del form sarà necessario assegnare uno specifico numero
d'ordine ad ogni singolo campo. In caso contrario il passaggio da un
campo all'altro attraverso il tasto TAB si interromperà in
corrispondenza del campo con l'ultimo numero d'ordine impostato.

Lato accessibilità il consiglio è quello di non definire una navigazione
personalizzata impostando specifici valori per il parametro in oggetto e
lasciare quindi che sia il browser stesso, in base alla struttura della
pagina a definire gli spostamenti tra un campo e l'altro attraverso il
tasto TAB.

**Label (etichetta):** consente di impostare l'etichetta che verrà
visualizzata in corrispondenza del campo che l'utente dovrà compilare.

**Sola Lettura:** consente di stabilire se il campo in oggetto dovrà o
meno essere in sola lettura. Selezionando quindi questo parametro, il
corrispondente campo verrà considerato in sola lettura e l'utente non
avrà alcuna possibilità di inserire o modificare i valori in esso
contenuti.

**Condizione di Visibilità:** consente di impostare una condizione in
base alla quale poter definire quando il componente in oggetto dovrà o
meno essere visibile all'interno del relativo form.

Nello specifico, tale condizione potrà essere definita sulla base:

- della nazione di appartenenza dell'utente

- del fatto che l'utente abbia dichiarato di essere un Privato oppure
  un'Azienda

- del fatto che l'utente abbia dichiarato di essere o meno un Ente
  Pubblico

- del fatto che l'utente abbia dichiarato o meno di voler ricevere la
  fattura elettronica

- del valore assunto da uno qualsiasi degli "Attributi Utente" (ad
  eccezione di quelli di tipo File) eventualmente inseriti all'interno
  del relativo form

**ATTENZIONE!** **Affinchè il controllo di visibilità possa funzionare
in maniera corretta sarà quindi necessario verificare di aver inserito
nel form di Registrazione / Profilo Utente appositi campi.**

Per maggiori informazioni in merito a come poter impostare una specifica
condizione di visibilità per un campo del form, si veda anche il
successivo capitolo "*Condizioni di visibilità e obbligatorietà per i
campi interni al form di Registrazione/Profilo Utente*" di questo
manuale.

**Campo Obbligatorio:** consente di stabilire se il campo che si sta
editando debba o meno essere obbligatoriamente compilato per poter
procedere poi alla conferma del form.

**Condizioni di Obbligatorietà:** visualizzato solo nel caso in cui il
precedente parametro "Campo Obbligatorio" sia stato impostato sul valore
SI. Consente di impostare una condizione in base alla quale poter
definire quando il componente in oggetto dovrà o meno essere considerato
come obbligatorio per la corretta compilazione del form.

Nello specifico, tale condizione potrà essere definita sulla base:

- della nazione di appartenenza dell'utente

- del fatto che l'utente abbia dichiarato di essere un Privato oppure
  un'Azienda

- del fatto che l'utente abbia dichiarato di essere o meno un Ente
  Pubblico

- del fatto che l'utente abbia dichiarato o meno di voler ricevere la
  fattura elettronica

- del valore assunto da uno qualsiasi degli "Attributi Utente" (ad
  eccezione di quelli di tipo File) eventualmente inseriti all'interno
  del relativo form

Per maggiori informazioni in merito a come poter impostare una specifica
condizione di obbligatorietà per un campo del form, si veda anche il
successivo capitolo "*Condizioni di visibilità e obbligatorietà per i
campi interni al form di Registrazione/Profilo Utente*" di questo
manuale.

**Tipo Valore:** consente di definire la tipologia degli elementi che
andranno poi a definire le varie opzioni del radio button. E' possibile
selezionare uno dei seguenti valori:

- **Testo:** in questo caso sarà poi necessario definire manualmente,
  all'interno dell'apposita sezione "**Gestione Valori**", le diverse
  possibili opzioni di scelta che verranno visualizzate all'interno del
  controllo

- **Scelta:** in questo caso il controllo visualizzerà tre diverse
  possibili opzioni di scelta (es. Si / No) e non sarà possibile
  aggiungerne altre né tanto meno sarà possibile eliminare una delle due
  opzioni presenti. In queste condizioni non sarà infatti presente la
  sezione "Gestione Valori".

> Le etichette delle due diverse possibili opzioni di scelta potranno
> comunque essere personalizzate all'interno della sezione "Testi /
> Messaggi del sito" del Wizard, selezionando il componente
> "Registrazione Utente" e andando ad agire su determinati campi che
> varieranno in relazione alla scelta effettuata nel successivo
> parametro "Campo di destinazione":
>
> L'opzione "**Scelta**" diventa di fondamentale importanza nel momento
> in cui l'esigenza dovesse essere:

- quella di inserire all'interno del form di Registrazione / Profilo
  Utente un Radio Button che consenta all'utente di dichiarare se è
  soggetto o meno all'obbligo di fattura elettronica

- quella di inserire all'interno del form di Registrazione / Profilo
  Utente un Radio Button che consenta all'utente di dichiarare se è o
  meno un Ente Pubblico

- quella di inserire all'interno del form di Registrazione / Profilo
  Utente un Radio Button che consenta all'utente di dichiarare se è o
  meno una Persona fisica

**Tipo di dati di Destinazione:** consente di stabilire a che cosa dovrà
corrispondere il "Campo Radio" che si sta realizzando e dove dovrà
quindi essere memorizzata l'informazione inserita dall'utente in fase di
compilazione del form.

È possibile selezionare una delle seguenti opzioni:

- **Attributo Cliente --** visibile solo nel caso in cui il precedente
  parametro "**Tipo Valore**" sia sitato impostato su "**Testo**"

> In questo caso l'informazione inserita dall'utente in fase di
> compilazione del form verrà salvata nell' Attributo Cliente indicato
> nel successivo campo **"Attributo di Destinazione"** campo questo da
> cui sarà possibile selezionare uno qualsiasi degli Attributi Cliente
> (Passweb o Mexal) precedentemente codificati all'interno della
> corrispondente sezione del Wizard
>
> **ATTENZIONE!** in relazione ad attributi cliente di tipo Mexal, sarà
> inoltre necessario prestare particolare attenzione al fatto che il
> dato che l'utente potrà poi andare ad inserire sul front end del sito,
> sia compatibile con il tipo di dato effettivamente accettato dal campo
> Mexal su cui è stato mappato l'attributo in esame.
>
> Per maggiori informazioni relativamente a come creare in Passweb
> Attributi Cliente si rimanda al relativo capitolo di questo manuale
> ("Utenti -- Gestione Parametri Utenti E-Commerce -- Gestione
> Attributi".)

- **Campo Cliente --** visibile solo nel caso in cui il precedente
  parametro "**Tipo Valore**" sia sitato impostato su "**Scelta**"

> In queste condizioni sarà poi possibile selezionare, in corrispondenza
> del successivo parametro "**Campo di destinazione**", una delle
> seguenti opzioni:

- **Fattura Elettronica:** selezionando questa opzione il componente in
  esame consentirà di inserire all'interno del form di Registrazione /
  Profilo **un controllo mediante il quale l'utente avrà la possibilità
  di dichiarare se è soggetto o meno all'obbligo di fattura
  elettronica**

![Videate\\campo_radio_fa_2_res.bmp](./assets/media/image97.png)

> Le etichette delle due diverse possibili opzioni di scelta possono
> essere personalizzate all'interno della sezione "Testi / Messaggi del
> sito" del Wizard, selezionando il componente "Registrazione Utente" e
> agendo sui campi "**Testo etichetta Fattura Elettronica Sì**" e
> "**Testo etichetta Fattura Elettronica No**".
>
> Nel momento in cui l'utente dovesse selezionare l'opzione **SI**, in
> fase di sincronizzazione il campo "**Tipo Fattura Elettronica**"
> presente nella relativa anagrafica gestionale verrà impostato sul
> valore "**Fattura B2B**" abilitando, di fatto, per il cliente in esame
> l'emissione della fattura elettronica.

![](./assets/media/image98.png)

> Al contrario nel momento in cui l'utente dovesse selezionare l'opzione
> **NO,** in fase di sincronizzazione il campo **Tipo Fattura
> Elettronica**" presente nella relativa anagrafica gestionale verrà
> impostato sul valore "**Non gestita**" con tutto ciò che ne consegue
> in termini di emissione da parte del gestionale della fattura
> elettronica.
>
> **ATTENZIONE!** Il fatto lasciare agli utenti del sito la possibilità
> di decidere se per essi debba o meno essere emessa fattura elettronica
> potrebbe essere fiscalmente non corretto. **Si consiglia dunque di
> fare particolare attenzione nel momento in cui si dovesse decidere di
> adottare questa opzione.**

- **Ente Pubblico -- solo per siti Ecommerce collegati a Mexal:**
  selezionando questa opzione il componente in esame consentirà di
  inserire all'interno del form di Registrazione / Profilo **un
  controllo mediante il quale l'utente avrà la possibilità di dichiarare
  se è o meno un Ente Pubblico**

![](./assets/media/image99.png)

> Le etichette delle due diverse possibili opzioni di scelta possono
> essere personalizzate all'interno della sezione "Testi / Messaggi del
> sito" del Wizard, selezionando il componente "Registrazione Utente" e
> agendo sui campi "**Testo etichetta Ente Pubblico Sì**" e "**Testo
> etichetta Ente Pubblico No**".
>
> Nel momento in cui l'utente dovesse selezionare l'opzione **SI**, in
> fase di sincronizzazione verrà selezionato il check "**Ente
> Pubblico**" presente nella relativa anagrafica gestionale e,
> contemporaneamente il parametro "**Fattura PA**" verrà impostato sul
> corrispondente valore "**Fattura PA**" abilitando, di fatto, per il
> cliente in esame l'emissione della fattura elettronica come ente
> pubblico.

![](./assets/media/image100.png)

> Al contrario nel momento in cui l'utente dovesse selezionare l'opzione
> **NO,** in fase di sincronizzazione il check "**Ente Pubblico**" non
> verrà selezionato e il campo "**Tipo Fattura Elettronica**" verrà
> impostato sul valore "**Fattura B2B**" o "**Non gestita**"
> dipendentemente da quanto impostato per il precedente controllo
> relativo all'assoggettamento alla fatturazione elettronica .
>
> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> consentire la registrazione al sito anche a enti pubblici, oltre ad
> inserire nel form di Registrazione un componente "Campo Radio"
> configurato secondo le specifiche sopra indicate ("Tipo Valore =
> Scelta" e "Campo di Destinazione = Ente Pubblico") è necessario
> verificare di aver inserito, nello stesso form di registrazione,
> **anche un componente "Campo Testo" mappato sul campo cliente**
> "**Codice Ufficio PA**"

- **Persona Fisica:** selezionando questa opzione il componente in esame
  consentirà di inserire all'interno del form di Registrazione / Profilo
  **un controllo mediante il quale un utente di tipo Azienda avrà la
  possibilità di dichiarare se dovrà essere considerato o meno come una
  ditta individuale**

![](./assets/media/image101.png)

> **ATTENZIONE!** Il campo in esame verrà visualizzato, ovviamente, solo
> per utenti di tipo Azienda
>
> Le etichette delle due diverse possibili opzioni di scelta possono
> essere personalizzate all'interno della sezione "Testi / Messaggi del
> sito" del Wizard, selezionando il componente "Registrazione Utente" e
> agendo sui campi "**Testo etichetta Persona Fisica Si**" e "**Testo
> etichetta Persona Fisica No**".
>
> Nel momento in cui l'utente dovesse selezionare l'opzione "**No**"
> (valore di default) indicando quindi di non essere una detta
> individuale, verrà considerato come una persona giuridica e:

- nel form di Registrazione / Profilo Utente verranno nascosti i campi
  "Cognome", "Nome" e "Denominazione" e verrà invece mostrato il campo
  "Ragione Sociale"

- in Mexal verrà creata un'anagrafica utente con il campo "Persona
  Fisica" deselezionato

![](./assets/media/image102.png)

> Nel momento in cui l'utente dovesse invece selezionare l'opzione
> "**Si**", indicando quindi di essere una ditta individuale:

- nel form di Registrazione / Profilo Utente verranno mostrati i campi
  "Cognome", "Nome" e "Denominazione" e verrà invece nascosto il campo
  "Ragione Sociale"

- in Mexal verrà creata un'anagrafica utente con il campo "Persona
  Fisica" selezionato

![](./assets/media/image103.png)

> **ATTENZIONE!** si ricorda che per utenti di tipo "Azienda" la
> corrispondente anagrafica Mexal avrà sempre il campo "Soggetto
> privato" deselezionato. Allo stesso modo per utenti di tipo "Privato"
> la corrispondente anagrafica Mexal avrà sempre il campo "Persona
> Fisica" correttamente selezionato

- **Valore di default --** visibile solo nel caso in cui il componente
  sia stato inserito all'interno del Form di Registrazione Utente e solo
  se il precedente parametro "**Tipo Valore**" sia sitato impostato su
  "**Scelta**".

> Consente di impostare il valore (SI o NO) da assegnare di default al
> campo Radio utilizzato per mappare le opzioni "Persona Fisica", "Ente
> Pubblico" e "Fattura Elettronica"

Per maggiori informazioni in merito ad ulteriori eventuali opzioni di
configurazione per il componente "Radio Button" si veda anche la sezione
"*Componenti Ecommerce -- Componente Ordine Custom -- One Step Checkout
-- Campo Radio*" di questo manuale

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia il Campo di input)

- Il Messaggio di errore

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE**! Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

La sezione "**Gestione valori",** visibile solo nel caso in cui il
precedente parametro **"Tipo Valore" sia stato impostato su "Testo"**,
consente, come detto, di definire e gestire le diverse possibili opzioni
di scelta che verranno visualizzate all'interno del controllo.

Per aggiungere una nuova opzione di scelta al controllo è sufficiente
cliccare sul relativo pulsante di aggiunta nuovo elemento (
![](./assets/media/image47.png) ) e inserire poi i dati di
configurazione dell'elemento stesso nella parte destra della maschera.

![](./assets/media/image104.png)

Per ciascuna delle possibili opzioni di scelta sarà necessario indicare:

- **Valore:** consente di specificare il valore che dovrà essere salvato
  nel momento in cui l'utente dovesse selezionare questa opzione.

- **Testo:** consente di indicare la label che dovrà essere
  visualizzata, all'interno del controllo, in corrispondenza
  dell'opzione di scelta che si sta configurando.

> **ATTENZIONE!** Nel caso in cui il campo "Testo" venga lasciato vuoto,
> label e valore dell'opzione di scelta coincideranno entrambi con
> quanto inserito all'interno del campo Valore.
>
> **NOTA BENE:** in ogni caso, alla conferma del form verrà sempre
> salvato solo **il Valore (e NON il Testo)** delle varie opzioni di
> scelta selezionate dall'utente

- **Selezionato:** flaggando questa casella l'opzione di scelta che si
  sta configurando apparirà sul sito già selezionato a default**.**

Una volta inserito un valore, per aggiungerlo all'elenco di valori
selezionabili tramite Radio Button, è necessario premere **"Aggiungi
Elemento"** presente nella parte alta della maschera.

Per **modificare** uno dei valori presenti in elenco è sufficiente
selezionarlo ed agire poi sulle relative proprietà.

Gli altri pulsanti presenti nella parte sinistra della maschera
consentono rispettivamente di:

- **Elimina elemento** (
  ![](./assets/media/image48.png) ): consente di eliminare l'elemento
  attualmente selezionata in elenco

- **Sposta su / giù**
  (![](./assets/media/image49.png) ): consente di riordinare tra loro le
  varie opzioni di scelta spostando verso l'alto o il basso l'elemento
  attualmente selezionato in elenco.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

