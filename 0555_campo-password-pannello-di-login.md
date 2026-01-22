# CAMPO PASSWORD (PANNELLO DI LOGIN)



Il Componente **"Campo Password"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_password_login_res.bmp](./assets/media/image71.png){width="2.5388888888888888in"
height="2.5388888888888888in"}

consente di inserire all'interno del pannello di login il campo che
dovrà poi essere utilizzato dall'utente, in fase di autenticazione al
sito, per inserire la propria password

**Tale campo corrisponderà quindi con quello utilizzato all'interno del
gestionale per memorizzare la password di accesso al sito.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campo_password_mexal.bmp](./assets/media/image72.png){width="4.415277777777778in"
height="2.3833333333333333in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_campo_testo_password.bmp](./assets/media/image73.png){width="5.052083333333333in"
height="3.4805555555555556in"}

Inserendo questo Componente all'interno del pannello di login verrà
aperta **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_password_configurazione_res.bmp](./assets/media/image74.png){width="5.143055555555556in"
height="3.0909722222222222in"}

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
password. Quanto indicato all'interno di questo campo non verrà quindi
considerato alla conferma del form.

**Massimo Caratteri:** permette di indicare il numero massimo di
caratteri che l'utente potrà digitare durante l'inserimento dei dati
(tale valore sarà determinato dalle dimensioni massime del
corrispondente campo del gestionale).

**Visualizza "Mostra / Nascondi Password"**: consente, se selezionato,
di abilitare un pulsante che l'utente potrà utilizzare, in fase di
inserimento Password, per mostrare in chiaro o meno i caratteri digitati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_mostra_nascondi_password.bmp](./assets/media/image75.png){width="3.234027777777778in"
height="3.279166666666667in"}

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

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
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

