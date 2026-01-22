# CAMPO DI TESTO (PANNELLO DI LOGIN)



Il Componente **"Campo di Testo"**

![](./assets/media/image67.png)

consente di inserire all'interno del pannello di login il campo che
dovrà poi essere utilizzato dall'utente, in fase di autenticazione al
sito, per inserire la propria username.

**Tale campo corrisponderà quindi con quello utilizzato all'interno del
gestionale per memorizzare la login utente.**

![](./assets/media/image68.png)

![](./assets/media/image69.png)

Inserendo questo Componente all'interno del pannello di login verrà
aperta **la sua maschera di gestione e configurazione**

![](./assets/media/image70.png)

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
indicato scomparirà consentendo quindi all'utente di inserire la propria
username. Quanto indicato all'interno di questo campo non verrà quindi
considerato alla conferma del form.

**Valore di default:** consente di indicare un testo che verrà
utilizzato (e visualizzato) **come valore di default** per il campo in
esame.

**ATTENZIONE!** A differenza di quanto indicato per il precedente
parametro "Segnaposto", il testo inserito all'interno del campo "Valore
di default" **non scomparirà** in automatico al click dell'utente sul
campo di input ma, al contrario, verrà considerato come se fosse un vero
e proprio valore indicato dall\'utente stesso in fase di compilazione.

**Tipo Valore:** consente di specificare il tipo di dati che potranno
essere inseriti all'interno del campo. E' possibile selezionare uno tra
i seguenti valori:

- **Testo:** all'interno del campo potrà essere inserito soltanto del
  testo

- **Mail:** all'interno del campo dovrà essere inserito un indirizzo di
  posta elettronica; un apposito controllo verificherà la corretta
  sintassi dell'indirizzo mail inserito.

**Massimo Caratteri:** Permette di indicare il numero massimo di
caratteri che l'utente potrà digitare durante l'inserimento dei dati
(tale valore sarà determinato dalle dimensioni massime del
corrispondente campo del gestionale).

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

