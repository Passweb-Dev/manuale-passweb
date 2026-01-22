# CAMPO DATA (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Data"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_data_registrazione_res.bmp](./assets/media/image113.png){width="2.5194444444444444in"
height="2.545138888888889in"}

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente un campo di tipo Data tramite il quale poter scegliere,
attraverso un apposito controllo di tipo calendario una specifica data.

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_campo_data_configurazione_res.bmp](./assets/media/image114.png){width="4.584722222222222in"
height="2.915277777777778in"}

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
visualizzata all'interno del form di registrazione in corrispondenza del
Componente in esame.

**Segnaposto:** permette di definire un testo da utilizzare **come
segnaposto** da poter visualizzare all'interno del campo di input.

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

**Tipo di dato di Destinazione:** consente di stabilire a quale campo
del gestionale o a quale attributo Passweb dovrà corrispondere il
Componente "Campo data" che si sta editando e conseguentemente in quale
campo del gestionale o di Passweb verrà poi memorizzata l'informazione
inserita dall'utente all'interno del campo.

In particolare nel caso in cui il campo "Tipo di Dato di Destinazione"
sia impostato sul valore:

1.  **Campo Cliente:** sarà possibile selezionare dal sottostante menu a
    tendina ("Campo di Destinazione") alcuni campi dell'Anagrafica
    Clienti/Fornitori del gestionale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_data_nascita_res.bmp](./assets/media/image115.png){width="4.584722222222222in"
height="2.915277777777778in"}

- **Data di nascita:** selezionando questo valore il Componente "Campo
  Data" corrisponderà al campo "**Data Nascita**" dell'Anagrafica
  Clienti/Fornitori del gestionale

> **Inserendo questo campo all'interno del form l'utente avrà quindi la
> possibilità di impostare, in fase di registrazione, la propria data di
> nascita**. Il valore inserito dall'utente verrà poi memorizzato sul
> gestionale all'interno del relativo campo.
>
> Questo tipo di campo verrà visualizzato all'interno del form
> unicamente nel caso in cui ad effettuare la registrazione sia un
> utente di tipo Privato.

2.  **Attributo Cliente:** sarà possibile selezionare dal sottostante
    menu a tendina ("Campo di Destinazione") uno degli attributi cliente
    (siano essi attributi di tipo Mexal o di tipo Passweb)
    precedentemente codificati all'interno della corrispondente sezione
    del Wizard

> **ATTENZIONE!** in relazione ad attributi cliente di tipo Mexal, sarà
> inoltre necessario prestare particolare attenzione al fatto che il
> dato che l'utente potrà poi andare ad inserire sul front end del sito,
> sia compatibile con il tipo di dato effettivamente accettato dal campo
> Mexal su cui è stato mappato l'attributo in esame.
>
> Nello specifico, ad esempio, se si tentasse di selezionare un
> Attributo mappato su di un campo MyDB di tipo Data, in fase di
> sincronizzazione verrebbe ritornato un apposito messaggio di errore,
> dovuto al fatto che il valore salvato sul sito per un campo data non è
> compatibile con il tipo di dato che si aspetta Mexal per un campo MyDB
> di questo stesso tipo
>
> **NOTA BENE**: per maggiori informazioni relativamente a come creare
> in Passweb Attributi Cliente si rimanda al relativo capitolo di questo
> manuale ("Utenti -- Gestione Parametri Utenti E-Commerce -- Gestione
> Attributi".)

**Tipologia di selezione (solo per varianti Desktop):** consente di
indicare la specifica tipologia di controllo che verrà poi utilizzato
per la selezione della data. E' possibile indicare uno dei seguenti
valori:

- **Default:** selezionando questa opzione il controllo per la selezione
  della data sarà costituito da un semplice calendario in cui l'utente
  dovrà utilizzare apposite frecce per passare da un mese all'altro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_default.bmp](./assets/media/image116.png){width="1.136111111111111in"
height="1.038888888888889in"}

- **Mostra menu Mesi:** selezionando questa opzione il controllo per la
  selezione della data sarà costituito da un calendario in cui la
  selezione del mese potrà avvenire anche mediante un apposito menu a
  tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_mesi.bmp](./assets/media/image117.png){width="1.1298611111111112in"
height="1.363888888888889in"}

- **Mostra menu Anni:** selezionando questa opzione il controllo per la
  selezione della data sarà costituito da un calendario in cui la
  selezione dello specifico anno potrà avvenire mediante un apposito
  menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_anni.bmp](./assets/media/image118.png){width="1.1298611111111112in"
height="1.4090277777777778in"}

- **Mostra menu Mesi e menu Anni:** selezionando questa opzione il
  controllo per la selezione della data sarà costituito da un calendario
  in cui la selezione dello specifico mese così come quella dello
  specifico anno potrà avvenire mediante un apposito menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_mesi_anni.bmp](./assets/media/image119.png){width="1.136111111111111in"
height="1.4090277777777778in"}

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

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

