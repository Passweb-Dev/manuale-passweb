# CAMPO DI TESTO (REGISTRAZIONE E PROFILO UTENTE)



Il Componente "**Campo di Testo**"

![](./assets/media/image82.png)

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente un classico campo di input all'interno del quale l'utente dovrà
digitare l'informazione richiesta (es. Nome, Cognome, Ragione Sociale
ecc ...). Il campo, oltre a non accettare valori di formattazione del
testo (maiuscole o minuscole), non conformi con quanto stabilito, può
contenere anche valori numerici, un indirizzo mail e un numero di
telefono

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico la sua maschera di gestione e configurazione

![](./assets/media/image83.png)

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

**Segnaposto:** permette di definire un testo da utilizzare **come
segnaposto** da poter visualizzare all'interno del campo di input.

**ATTENZIONE!** Al click dell'utente sul campo in esame il testo
indicato scomparirà consentendo quindi all'utente di inserire il valore
desiderato. Quanto indicato all'interno di questo campo non verrà quindi
considerato alla conferma del form.

**Valore di default:** consente di indicare un testo che verrà
utilizzato (e visualizzato) **come valore di default** per il campo in
esame.

**ATTENZIONE!** A differenza di quanto indicato per il precedente
parametro "Segnaposto", il testo inserito all'interno del campo "Valore
di default" **non scomparirà** in automatico al click dell'utente sul
campo di input ma, al contrario, verrà considerato come se fosse un vero
e proprio valore indicato dall\'utente stesso in fase di compilazione
del form.

**Sola Lettura:** consente di stabilire se il campo in oggetto dovrà o
meno essere in sola lettura. Selezionando quindi questo parametro, il
corrispondente campo verrà considerato in sola lettura e l'utente non
avrà alcuna possibilità di inserire o modificare i valori in esso
contenuti.

**Tipo Valore:** consente di specificare il tipo di dati che potranno
essere inseriti all'interno del campo.

È possibile selezionare uno tra i seguenti valori:

- **Testo:** all'interno del campo potrà essere inserito un qualsiasi
  carattere alfanumerico maiuscolo o minuscolo (compresi eventuali
  caratteri speciali)

- **Maiuscolo:** all'interno del campo potranno essere inseriti soltanto
  caratteri testuali maiuscoli.

- **Mail:** all'interno del campo dovrà essere inserito un indirizzo di
  posta elettronica. Un apposito controllo verificherà la corretta
  sintassi dell'indirizzo mail inserito che dovrà quindi rispettare il
  formato "*nomecasella@indirizzo.it*".

- **Numerico:** all'interno del campo potranno essere inseriti soltanto
  numeri interi

- **Decimale:** all'interno del campo potranno essere inseriti soltanto
  numeri con un massimo di 6 decimali

- **Telefono:** all'interno del campo potranno essere inseriti soltanto
  numeri di telefono nel formato E.164 (lo standard internazionale per
  la telefonia). Un apposito controllo verificherà la correttezza del
  numero inserito che dovrà quindi rispettare le seguenti regole:

  - il primo carattere deve essere un + seguito dal country code (es.
    +39 per l'Italia) e dal numero di telefono

  - il primo numero dopo il + non può essere uno 0

  - il numero di telefono, comprensivo di country code, non può avere
    meno di 5 cifre né più di 15

  - non sono consentiti caratteri speciali (trattini spazi o punti)

> **ATTENZIONE!** nel caso in cui il browser in uso non dovesse
> supportare l'attributo type="tel" (che attiva i controlli sopra
> indicati) il campo verrà gestito come un semplice campo di testo

**ATTENZIONE!** I messaggi di errore visualizzati nel momento in cui si
dovessero inserire caratteri diversi da quelli richiesti dalla specifica
tipologia di campo possono essere personalizzati alla pagina "**Testi
dei Componenti**" del Wizard (menu "***Sito -- Testi / Messaggi del
sito***") selezionando il componente "**Form**"

**Valore minimo / massimo:** visibili solo nel caso in cui il campo
"**Tipo Valore**" sia impostato su "**Numerico**" o "**Decimale**"

Consentono di impostare un range di validazione per il numero inserito a
front end all'interno del corrispondente campo di input

Nel momento in cui si dovesse dunque decidere di valorizzare questi
campi, la validazione del form potrà poi avvenire con successo solo nel
caso in cui il valore inserito a front end rientri effettivamente nel
range definito da questi due campi

In queste condizioni inoltre, in corrispondenza del campo di input,
verrà visualizzato anche un apposito messaggio per informare l'utente
relativamente al range di valori accettati dal campo in esame

**Step:** visibile solo nel caso in cui il campo "**Tipo Valore**" sia
impostato su "**Numerico**" o "**Decimale**"

Consente di impostare lo step di validazione per i valori che verranno
poi inseriti all'interno del corrispondente campo di input.

Nel momento in cui si dovesse dunque decidere di impostare per questo
parametro un valore diverso da zero, la validazione del form potrà poi
avvenire con successo solo nel caso in cui il valore inserito a front
end sia effettivamente un multiplo dello step indicato.

In queste condizioni inoltre, in corrispondenza del campo di input,
verrà visualizzato anche un apposito messaggio per informare l'utente
del fatto che il valore da inserire all'interno del campo dovrà essere
necessariamente un multiplo dello step indicato. Il testo in questione
potrà essere personalizzato alla pagina "**Gestione Testi / Messaggi del
Sito**" (componente "Form" campo "Step")

Nel caso in cui l'utente non dovesse rispettare questa indicazione,
andando quindi ad inserire un valore diverso da un multiplo dello step
indicato, alla conferma del form verrà visualizzato un apposito
messaggio di errore.

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

**Minimo Caratteri:** consente di indicare il numero minimo di caratteri
che l'utente dovrà inserire per poter validare il campo.

Nel caso in cui dovesse essere inserito un numero di caratteri inferiore
a quello indicato, alla conferma del form verrà visualizzato un apposito
messaggio di errore.

**Massimo Caratteri:** consente di indicare il numero massimo di
caratteri che l'utente potrà digitare durante l'inserimento dei dati
(tale valore sarà determinato dalle dimensioni massime del
corrispondente campo del gestionale).

**Tipo di dato di Destinazione:** consente di stabilire a quale campo
del gestionale (opzione **Campo Cliente**) o a quale attributo Passweb
(opzione **Attributo Cliente**) dovrà corrispondere il Componente "Campo
di Testo" che si sta editando e conseguentemente in quale campo del
gestionale o di Passweb verrà poi memorizzata l'informazione inserita
dall'utente all'interno del campo.

Per maggiori informazioni relativamente ai diversi possibili tipi di
dato di destinazione si veda anche quanto indicato nel successivo
capitolo di questo manuale ("*Destinazione dei Dati*")

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

Il pulsante "Salva" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**ATTENZIONE! Per un corretto funzionamento del sito è necessario
inserire nel form di registrazione almeno un indirizzo completo e
costituito dunque dai campi Indirizzo, Località, CAP, Nazione e
Provincia, campi questi che andrebbero inseriti nel form di
registrazione anche come obbligatori.**

Per maggiori informazioni in merito a come gestire i campi Nazione e
Provincia si veda anche la sezione "*Live Editing per Varianti
Responsive -- Lista Componenti Interazione Utente -- Componenti interni
ai componenti interazione utente -- Campo Lista Valori"* di questo
manuale

**Nel caso in cui non dovessero essere inseriti nel form di
registrazione i campi necessari per comporre un indirizzo completo si
potrebbe verificare una situazione in cui un nuovo utente avrebbe la
possibilità di completare la registrazione al sito senza indicare però
nessun indirizzo di spedizione merce.**

In queste condizioni al termine della registrazione l'utente sarebbe
immediatamente ridiretto alla pagina Profilo Utente dove avrebbe la
possibilità, attraverso il componente "Rubrica Indirizzi", di codificare
tutti gli indirizzi di spedizione desiderati. Considerando però che in
questo senso non sono previsti vincoli di alcun tipo l'utente potrebbe
anche procedere nella conferma dell'ordine senza specificare nessun
indirizzo di spedizione.

Se così fosse l'applicazione si preoccuperà di bloccare la procedura di
conferma dell'ordine in corrispondenza della fase di selezione
dell'indirizzo di spedizione, fase questa obbligatoria e di fondamentale
importanza per determinare anche la corretta applicazione delle spese di
trasporto.

**In definitiva dunque, un utente privo di indirizzi di spedizione non
potrebbe in alcun modo portare a termine la conferma di un ordine.**

Il fatto quindi di richiedere all'interno del form di registrazione in
maniera obbligatoria informazioni quali indirizzo, CAP, località,
provincia e/o nazione permette di evitare agli utenti del sito blocchi
imprevisti in fase di conferma dell'ordine.

Se poi, l'esigenza dovesse essere quella di permettere all'utente di
inserire direttamente in fase di registrazione più indirizzi diversi, ad
esempio un indirizzo di fatturazione e uno di spedizione, sarebbe allora
necessario inserire all'interno del form stesso tutti i campi necessari
per comporre in maniera completa questi due indirizzi, ossia: Indirizzo,
Località, CAP, Nazione, Provincia e Indirizzo n.2, Località n.2, CAP
n.2, Nazione n.2 e Provincia n.2

In queste condizioni inoltre **i campi di uno stesso indirizzo sono
strettamente legati tra loro** per cui nel caso in cui si fosse commesso
un errore in fase di configurazione del form, inserendo, ad esempio per
il secondo indirizzo il campo Località n.3 anziché quello Località n.2,
l'applicazione rileverebbe la presenza, nel form, di due indirizzi non
completi e visualizzerebbe un apposito messaggio di avviso.

**ATTENZIONE! Il messaggio in esame non è in alcun modo bloccante.**

Ciò significa quindi che, in queste condizioni, nel momento in cui
l'utente dovesse compilare e confermare il form di registrazione, lato
gestionale verrà inserito un indirizzo completo (relativo ai campi
Indirizzo, Località, CAP, Nazione e Provincia ) nell'anagrafica
dell'utente e due indirizzi incompleti (relativi rispettivamente ai
campi Indirizzo n.2, CAP n.2, Nazione n.2, Provincia n.2 e al campo
Località n.3) nella tabella Anagrafica Indirizzi di Spedizione
(Ecommerce Mexal).

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

