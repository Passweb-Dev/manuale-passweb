# CAMPO LISTA VALORI (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Lista Valori"**

![](./assets/media/image109.png)

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente un'etichetta (label) seguita da un menù a tendina (drop down
list) contenente una serie di valori tra cui selezionare quello più
idoneo.

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image110.png)

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

**Testo del controllo senza valori selezionati:** consente di impostare
un testo che verrà inizialmente visualizzato all'interno del
corrispondente controllo (es. ------ selezionare un valore ------ ).

Nel caso in cui il campo in oggetto non venga valorizzato, e non venga
neppure impostato uno dei possibili valori da selezionare come valore di
default per il controllo, il menu a tendina sarà impostato,
inizialmente, su di un valore nullo.

**Sola Lettura:** consente di stabilire se il campo in oggetto dovrà o
meno essere in sola lettura. Selezionando quindi questo parametro, il
corrispondente campo verrà considerato in sola lettura e l'utente non
avrà alcuna possibilità di inserire o modificare i valori in esso
contenuti.

**Tipo Valore:** consente di definire il tipo di valore con il quale
popolare il menù a tendina (drop down list).

- **Testo:** permette di popolare il menu a tendina con valori
  personalizzati.

> Selezionando questa opzione si attiverà infatti la sezione "**Gestione
> Valori**" della finestra "Nuovo Campo Select", permettendo di poter
> inserire, modificare e cancellare i valori desiderati**.**

- **Provincia:** selezionando questa opzione il menu a tendina si
  popolerà automaticamente con l'elenco di tutte le Provincie della
  Nazione cui appartiene l'utente che sta visitando il sito.

> Per maggiori informazioni relativamente alle modalità di
> determinazione del paese di provenienza dell'utente che naviga il sito
> si veda anche quanto indicato all'interno dei capitoli e "*Sito -
> Gestione Lingue del sito*" e "*Configurazione Gestionale -- Parametri
> Paese Lingua e Valuta -- Gestione Listini*" di questo manuale.
>
> **Nel caso in cui la nazione di appartenenza dell'utente non sia tra
> quelle gestite all'interno del sito, il campo visualizzerà le
> provincie della nazione di default** (per maggiori informazioni
> relativamente alla gestione dei paesi si veda la corrispondente
> sezione "*Configurazione Gestionale -- Parametri Paese Lingua e Valuta
> -- Gestione Paese"* di questo manuale)
>
> Inoltre nel caso in cui all'interno del form sia presente anche il
> campo "Nazione" l'elenco delle province varierà in maniera contestuale
> alla specifica nazione selezionata dall'utente.
>
> [**ATTENZIONE!!**]{.underline}
>
> **In relazione alla gestione delle province estere Passweb adottata lo
> standard ISO 3166-2 che definisce appunto le diverse suddivisioni
> territoriali delle varie nazioni**. In base a tale standard ogni
> suddivisione territoriale è contraddistinta da un codice costituito da
> due parti separate da un -. La prima parte di questo codice è composta
> da due caratteri alfabetici che identificano la nazione di
> appartenenza, la seconda parte (dopo il -) può invece essere
> alfabetica o numerica ed è composta da uno, due o tre caratteri in
> base a specifici standard nazionali.
>
> **Esempio**
>
> IT-TO: è il codice ISO 3166-2 che definisce la provincia di Torino in
> Italia
>
> BR-TO: è il codice ISO 3166-2 che definisce la provincia di Tocantis
> in Brasile
>
> Considerando che, in queste condizioni, il campo in esame dovrà essere
> mappato con il campo "Provincia" dell' Anagrafica Clienti/Fornitori di
> Mexal, che tale campo all'interno del gestionale ha una lunghezza
> massima di 4 caratteri e che in ogni caso la nazione di appartenenza è
> facilmente individuale dal campo "Paese" presente all'interno di
> questa stessa anagrafica, Passweb inserirà in Mexal nel relativo
> campo, solo la seconda parte (quella identificativa della provincia)
> del codice ISO 3166-2 corrispondente alla Provincia selezionata
> dall'utente.

- **Nazione:** selezionando questa opzione il menu a tendina si popolerà
  automaticamente con l'elenco di tutte le Nazioni gestite all'interno
  del sito (per maggiori informazioni relativamente alla gestione dei
  paesi si veda la corrispondente sezione "*Configurazione Gestionale --
  Parametri Paese Lingua e Valuta -- Gestione Paese*" di questo manuale)

> **ATTENZIONE!** In queste condizioni il campo in esame dovrà quindi
> essere mappato con il campo "Paese" dell' Anagrafica Clienti/Fornitori
> di Mexal.
>
> Nel caso in cui all'interno del form sia presente anche il campo
> "Provincia", la selezione di una specifica Nazione determinerà
> l'elenco delle provincie visualizzate all'interno del suddetto campo.

- **Categoria Statistica:** selezionando questa opzione il menu a
  tendina si popolerà automaticamente con l'elenco delle Categorie
  Statistiche utente attualmente gestite all'interno del sito.

> **ATTENZIONE!** all'interno del menu a tendina verranno visualizzate
> solo ed esclusivamente le Categorie Statistiche per le quali è stata
> definita una specifica descrizione
>
> Per maggiori informazioni relativamente a come poter assegnare e/o
> personalizzare le descrizioni delle Categorie Statistiche utente si
> veda anche quanto indicato all'interno del capitolo "*Utenti -- Siti
> Ecommerce -- Configurazione Utenti Sito -- Categorie Statistiche*" di
> questo manuale

**ATTENZIONE!** nel momento in cui si dovesse selezionare come "Tipo
Valore" l'opzione Provincia, Nazione o Categoria Statistica i valori
della select box saranno gestiti in automatico dall'applicazione. In
conseguenza di ciò la sezione "**Gestione Valori**" della finestra "
Nuovo Campo Select" non verrà abilitata.

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
Componente "Campo Lista Valori" che si sta editando e, conseguentemente,
in quale campo del gestionale o di Passweb verrà poi memorizzata
l'informazione selezionata dall'utente in fase di registrazione.

In particolare nel caso in cui il campo "Tipo di Dato di Destinazione"
sia impostato sul valore:

1.  **Campo Cliente:** sarà possibile selezionare dal sottostante menu a
    tendina ("Campo di Destinazione") uno dei seguenti valori:

- **Nazione Anagrafica Utente/Nazione n.2/Nazione n.3/Nazione n.4:**
  solo per "**Tipo Valore = Nazione**".

> In queste condizioni il componente "Campo Lista Valori" corrisponderà
> al campo "**Paese**" dell'Anagrafica Clienti/Fornitori del gestionale
> (Nazione Anagrafica Utente) o all'analogo campo di un ben preciso
> indirizzo di spedizione merce (Nazione n.2/n.3/n.4)
>
> In definitiva dunque, è possibile gestire nel form di registrazione
> utente fino a 4 campi Nazione differenti, uno dei quali finirà
> nell'anagrafica del utente e gli altri tre in tre distinti indirizzi
> di spedizione.

- **Provincia Anagrafica Utente/Provincia n.2/Provincia n.3/Provincia
  n.4:** solo per "**Tipo Valore = Provincia**".

> In queste condizioni il Componente "Campo Lista Valori" corrisponderà
> al campo "**Provincia**" dell'Anagrafica Clienti/Fornitori del
> gestionale (Provincia Anagrafica) oppure all'analogo campo di un ben
> preciso indirizzo di spedizione merce (Provincia n.2/n.3/n.4).
>
> In definitiva dunque, è possibile gestire nel form di registrazione
> utente fino a 4 campi Provincia differenti, uno dei quali finirà
> nell'anagrafica del utente e gli altri tre in tre distinti indirizzi
> di spedizione.
>
> **NOTA BENE:** analogamente a quanto già detto in relazione al
> componente "Campo Testo" e alla necessita di richiedere all'interno
> del form di registrazione tutti i dati necessari a comporre un
> indirizzo completo, si consiglia, per la stessa ragione, **di inserire
> sempre all'interno del form anche due componenti "Lista Valori"
> mappati con i campi Mexal Nazione e Provincia impostandoli anche come
> obbligatori**

- **Categoria Statistica:** solo per "**Tipo Valore = Categoria
  Statistica**" e solo per siti Ecommerce collegati a Mexal

> In queste condizioni il componente "Campo Lista Valori" corrisponderà
> al campo "Categoria Statistica" presente sul gestionale all'interno
> della maschera "Condizioni generali del soggetto"

![](./assets/media/image111.png)

> Selezionando una delle opzioni presenti all'interno del menu a tendina
> l'utente verrà quindi associato alla relativa Categoria Statistica.
>
> **ATTENZIONE!** Nel momento in cui un utente dovesse avere già
> associata una determinata Categoria Statistica, il campo in esame, se
> inserito all'interno del componente "Profilo Utente", permetterà,
> eventualmente, soltanto la modifica di questa informazione. Non sarà
> quindi possibile in alcun modo rimuovere, da Passweb, la Categoria
> Statistica assegnata ad un determinato utente.

2.  **Attributo Cliente:** sarà possibile selezionare dal sottostante
    menu a tendina ("Campo di Destinazione") uno degli attributi cliente
    (siano essi attributi di tipo Mexal o di tipo Passweb)
    precedentemente codificati all'interno della corrispondente sezione
    del Wizard.

> **ATTENZIONE!** in relazione ad attributi cliente di tipo Mexal, sarà
> inoltre necessario prestare particolare attenzione al fatto che il
> dato che l'utente potrà poi andare ad inserire sul front end del sito,
> sia compatibile con il tipo di dato effettivamente accettato dal campo
> Mexal su cui è stato mappato l'attributo in esame.
>
> **NOTA BENE**: per maggiori informazioni relativamente a come creare
> in Passweb Attributi Cliente si rimanda al relativo capitolo di questo
> manuale ("Utenti -- Gestione Parametri Utenti E-Commerce -- Gestione
> Attributi".

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
![](./assets/media/image47.png) ) e inserire poi i dati di
configurazione dell'elemento stesso nella parte destra della maschera.

![](./assets/media/image112.png)

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
selezionabili, è necessario premere **"Aggiungi Elemento"** e
successivamente il tasto "**salva**".

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

