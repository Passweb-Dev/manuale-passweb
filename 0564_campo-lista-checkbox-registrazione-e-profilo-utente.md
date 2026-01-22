# CAMPO LISTA CHECKBOX (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Lista Checkbox"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_lista_check_registrazione_res.bmp](./assets/media/image107.png)

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente una serie di etichette seguite da altrettante caselline da
spuntare, in sostanza è simile al campo Radio (spiegato precedentemente)
ma, a differenza di quest'ultimo, che era limitato alla selezione di una
sola opzione tra quelle disponibili, il campo lista Checkbox consente
selezioni multiple.

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_lista_checkbox_configurazione_res.bmp](./assets/media/image108.png)

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

**Attributo di Destinazione:** consente di stabilire a quale attributo
cliente (Mexal o Passweb) dovrà corrispondere il Componente "Campo Lista
Checkbox" che si sta editando e conseguentemente dove verrà poi
memorizzata l'informazione inserita dall'utente in fase di
registrazione.

> **NOTA BENE**: per maggiori informazioni relativamente a come creare
> in Passweb Attributi Cliente si rimanda al relativo capitolo di questo
> manuale ("Utenti -- Gestione Parametri Utenti E-Commerce -- Gestione
> Attributi".)

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

La sezione "**Gestione valori"** consente di definire e gestire le
diverse possibili opzioni di scelta che verranno visualizzate
all'interno del controllo.

Per aggiungere una nuova opzione di scelta al controllo è sufficiente
cliccare sul relativo pulsante di aggiunta nuovo elemento (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png) ) e inserire poi i dati di
configurazione dell'elemento stesso nella parte destra della maschera.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\Form_radio_nuovo_valore_res.bmp](./assets/media/image104.png)

Per ciascuna delle possibili opzioni di scelta sarà necessario indicare:

- **Valore:** consente di specificare il valore che dovrà essere salvato
  nel momento in cui l'utente dovesse selezionare questa opzione.

> **ATTENZIONE!** in relazione ad attributi cliente di tipo Mexal, sarà
> necessario prestare particolare attenzione al fatto che il dato che
> l'utente potrà poi andare ad inserire sul front end del sito, sia
> compatibile con il tipo di dato effettivamente accettato dal campo
> Mexal su cui è stato mappato l'attributo in esame.

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
selezionabili, è necessario premere **"Aggiungi Elemento"** e
successivamente il tasto "**salva**".

Per **modificare** uno dei valori presenti in elenco è sufficiente
selezionarlo ed agire poi sulle relative proprietà.

Gli altri pulsanti presenti nella parte sinistra della maschera
consentono rispettivamente di:

- **Elimina elemento** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image48.png) ): consente di eliminare l'elemento
  attualmente selezionata in elenco

- **Sposta su / giù**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icone_su_giu.bmp](./assets/media/image49.png) ): consente di riordinare tra loro le
  varie opzioni di scelta spostando verso l'alto o il basso l'elemento
  attualmente selezionato in elenco.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

