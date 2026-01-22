# CAMPO PRIVACY (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Privacy"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_privacy_registrazione_res.bmp](./assets/media/image124.png)

consente di inserire all'interno dei form di Registrazione e/o di
Profilo Utente un controllo mediante il quale l'utente potrà decidere di
accettare o meno determinate condizioni in merito alla privacy e al
trattamento dei dati personali.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campo_privacy_res.bmp](./assets/media/image125.png)

**ATTENZIONE! Dipendentemente dalle impostazioni di configurazione
settate per il componente, l'accettazione delle relative condizioni può
o meno essere obbligatoria, e dunque vincolante, ai fini della conferma
e del salvataggio del form.**

Rilasciando il componente all'interno del form si aprirà **la sua
maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_campo_privacy_res.bmp](./assets/media/image126.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

- **Nome:** permette di inserire un nome per il campo che si sta
  editando;

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Id/Name:** consente di personalizzare i selector HTML "id" e "name"
  per il componente in oggetto in modo tale da poterlo intercettare e
  personalizzare, a livello di CSS o di codice javascript, in maniera
  più semplice ed immediata.

> **Il valore inserito all'interno di questo campo verrà utilizzato per
> entrambi i selector indicati**

- **Tab Index:** consente di personalizzare l'ordine di tabulazione del
  form assegnando uno specifico numero d'ordine al campo in oggetto. Una
  volta assegnato un numero d'ordine ad ogni campo del form sarà poi
  possibile spostarsi da un elemento all'altro, utilizzando il tasto
  "TAB" e secondo l'ordine di tabulazione impostato.

> Nel caso in cui si decida di personalizzare l'ordine di tabulazione
> degli elementi del form sarà necessario assegnare uno specifico numero
> d'ordine ad ogni singolo campo. In caso contrario il passaggio da un
> campo all'altro attraverso il tasto TAB si interromperà in
> corrispondenza del campo con l'ultimo numero d'ordine impostato.
>
> Lato accessibilità il consiglio è quello di non definire una
> navigazione personalizzata impostando specifici valori per il
> parametro in oggetto e lasciare quindi che sia il browser stesso, in
> base alla struttura della pagina a definire gli spostamenti tra un
> campo e l'altro attraverso il tasto TAB.

- **Label (etichetta):** Il testo inserito in questo campo sarà
  visualizzato come etichetta propria del campo Privacy.

- **Condizione di Visibilità:** consente di impostare una condizione in
  base alla quale poter definire quando il componente in oggetto dovrà o
  meno essere visibile all'interno del relativo form.

> Nello specifico, tale condizione potrà essere definita sulla base:

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

> **ATTENZIONE!** **Affinché il controllo di visibilità possa funzionare
> in maniera corretta sarà quindi necessario verificare di aver inserito
> nel form di Registrazione / Profilo Utente appositi campi.**
>
> Per maggiori informazioni in merito a come poter impostare una
> specifica condizione di visibilità per un campo del form, si veda
> anche il successivo capitolo "*Condizioni di visibilità e
> obbligatorietà per i campi interni al form di Registrazione/Profilo
> Utente*" di questo manuale.

- **Campo Obbligatorio:** visibile solo nel caso in cui il successivo
  parametro "**Tipo di dato di destinazione**" sia stato impostato sul
  valore "**Condizioni Privacy Opzionali -- Attributo Cliente**".

> Consente di decidere se il campo in esame dovrà o meno essere
> obbligatorio per la corretta compilazione del form.
>
> Impostando il campo sul valore **SI,** l'utente dovrà necessariamente
> accettare le relative condizioni per poter procedere alla conferma del
> form
>
> Nel caso in cui invece il parametro in oggetto sia stato impostato sul
> valore **NO**, l'utente potrà procedere alla conferma del form anche
> nel caso in cui decidesse di non accettare le relative condizioni. In
> questo caso inoltre l'utente potrebbe procedere alla conferma del form
> anche se dovesse decidere di non selezionare nessuno dei due valori
> (Accetto/Rifiuto) proposti.

- **Condizioni di Obbligatorietà:** visualizzato solo nel caso in cui il
  precedente parametro "Campo Obbligatorio" sia stato impostato sul
  valore SI. Consente di impostare una condizione in base alla quale
  poter definire quando il componente in oggetto dovrà o meno essere
  considerato come obbligatorio per la corretta compilazione del form

> Nello specifico, tale condizione potrà essere definita sulla base:

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

> Per maggiori informazioni in merito a come poter impostare una
> specifica condizione di obbligatorietà per un campo del form, si veda
> anche il successivo capitolo "*Condizioni di visibilità e
> obbligatorietà per i campi interni al form di Registrazione/Profilo
> Utente*" di questo manuale.

- **Tipo di dato di destinazione:** consente di definire la tipologia
  del controllo "Privacy" da inserire all'interno del form.

> È possibile selezionare uno dei seguenti valori:

- **Condizioni Privacy Opzionali -- Attributo Cliente:** selezionando
  questa opzione le relative condizioni di privacy dovranno essere o
  meno accettate in maniera obbligatoria, ai fini della corretta
  compilazione del form, dipendentemente da quanto impostato per i
  precedenti parametri "**Campo Obbligatorio**" e "**Condizioni di
  obbligatorietà**".

> In queste condizioni sarà inoltre necessario indicare nel successivo
> campo "**Attributo di destinazione**", lo specifico Attributo Utente
> da utilizzare per memorizzare la scelta fatta dal cliente in merito
> alle condizioni in oggetto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_privacy_opzionali_res.bmp](./assets/media/image127.png)

> **ATTENZIONE!** L' Attributo di Destinazione, in cui memorizzare la
> scelta fatta dal cliente in merito alle condizioni in oggetto, dovrà
> essere un semplice attributo (Mexal o Passweb) testuale di un solo
> carattere. Per maggiori informazioni in merito alla creazione e alla
> gestione degli Attributi Utente, si veda anche l'apposita sezione di
> questo manuale ("*Utenti -- Siti Ecommerce -- Configurazione Utenti
> Sito -- Gestione Attributi*")
>
> Il campo "**Valore di Default**" consente infine, di inserire il
> dettaglio delle condizioni in oggetto, dettaglio questo che verrà poi
> visualizzato all'interno del form in una apposita area di testo.

- **Condizioni Privacy Sito:** selezionando questa opzione le relative
  condizioni di privacy verranno sempre considerate come obbligatorie e
  la loro accettazione sarà dunque vincolante ai fini della corretta
  compilazione del form.

> **ATTENZIONE!** Il testo delle condizioni in oggetto dovrà essere
> inserito nel campo "**Testo Privacy**" presente, per l'elemento
> "**Form Privacy**", all'interno della sezione "*Testi / Messaggi del
> Sito -- Testi dei Componenti*" del Wizard
>
> In queste condizioni il successivo parametro "**Campo di
> Destinazione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_privacy_obbligatorie_res.bmp](./assets/media/image128.png)

> dovrà essere impostato sul valore "**Privacy**" (l'unico possibile),
> la scelta effettuata dal cliente in merito a tali condizioni verrà
> memorizzata all'interno del database del proprio sito e potrà essere
> visualizzata, assieme all'eventuale data di accettazione, all'interno
> dei campi "**Consenso alla Privacy**" e "**Data Consenso alla
> Privacy**" presenti nella maschera "**Dati Utente -- Informazioni
> Generali**" accessibile dall'apposita sezione del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_privacy_obbligatorie2_res.bmp](./assets/media/image129.png)

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La Label

- Il Controllo (ossia il campo della Privacy)

- Il Messaggio di errore

> È possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame, permettendo dunque, già in fase di
> configurazione del componente stesso di decidere quale elemento dovrà
> essere visualizzato prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali" di questo
manuale.

