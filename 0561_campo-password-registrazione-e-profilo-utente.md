# CAMPO PASSWORD (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Password"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_password_registrazione_res.bmp](./assets/media/image92.png){width="2.5194444444444444in"
height="2.545138888888889in"}

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente un campo di input che dovrà poi essere utilizzato dall'utente per
impostare la propria password di accesso al sito.

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_campo_password_configurazione_res.bmp](./assets/media/image93.png){width="4.792361111111111in"
height="3.045138888888889in"}

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

> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

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

**Sola Lettura:** consente di stabilire se il campo in oggetto dovrà o
meno essere in sola lettura. Selezionando quindi questo parametro, il
corrispondente campo verrà considerato in sola lettura e l'utente non
avrà alcuna possibilità di inserire o modificare i valori in esso
contenuti.

**Tipo Valore:** consente di specificare il tipo di dati che potranno
essere inseriti all'interno del campo. E' possibile selezionare uno tra
i seguenti valori:

- **Testo:** all'interno del campo potrà essere inserito soltanto del
  testo

- **Maiuscolo:** all''interno del campo potranno essere inseriti
  soltanto caratteri testuali maiuscoli

- **Numerico:** all''interno del campo potranno essere inseriti soltanto
  numeri (nel caso, ad esempio, si richieda un numero di telefono)

- **Mail:** all'interno del campo dovrà essere inserito un indirizzo di
  posta elettronica; un apposito controllo verificherà la corretta
  sintassi dell'indirizzo mail inserito.

**Campo Obbligatorio:** consente di stabilire se il campo che si sta
editando debba o meno essere obbligatoriamente compilato per poter
procedere all'accettazione dei dati che verranno inseriti dall'utente.
**E' consigliato selezionare questo parametro.**

**Condizioni di Obbligatorietà:** visualizzato solo nel caso in cui il
precedente parametro "Campo Obbligatorio" sia stato impostato sul valore
Si. Consente di impostare una condizione in base alla quale poter
definire quando il componente in oggetto dovrà o meno essere considerato
come obbligatorio per la corretta compilazione del form.

**Massimo Caratteri:** permette di indicare il numero massimo di
caratteri che l'utente potrà digitare durante l'inserimento dei dati
(tale valore sarà determinato dalle dimensioni massime del
corrispondente campo del gestionale).

**Visualizza "Mostra / Nascondi Password"**: consente, se selezionato,
di abilitare un pulsante che l'utente potrà utilizzare, in fase di
inserimento Password, per mostrare o meno, in chiaro, i caratteri
digitati.

**Visualizza suggerimenti password:** consente, se selezionato, di
visualizzare sul front end del sito, in fase di compilazione della
password, una serie di suggerimenti utili per informare l'utente
relativamente ai criteri da soddisfare affinché la password da lui
inserita possa essere ritenuta corretta

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\suggerimenti_password.bmp](./assets/media/image94.png){width="5.9743055555555555in"
height="3.441666666666667in"}

**ATTENZIONE!** I criteri da soddisfare per validare la password e,
conseguentemente, i relativi suggerimenti dipendono direttamente da
quanto impostato in corrispondenza del parametro "**Formato della
Password**" presente alla pagina "**Configurazione Parametri Utenti**"
del Wizard. Per maggiori informazioni in merito si veda anche quanto
indicato nel relativo capitolo di questo manuale ("*Utenti -- Siti
Ecommerce -- Configurazione utenti sito -- Configurazione Utenti --
Impostazioni generali Gestione delle credenziali*")

I testi dei suggerimenti possono essere modificati dalla sezione
"**Testi/Messaggi del Sito -- Testi dei Componenti**" del Wizard agendo
sul componente "**Form Password**"

**Campo di Destinazione:** consente di definire come dovrà essere
effettivamente utilizzato il campo in esame e che tipo di dato dovrà
contenere o validare.

E' possibile selezionare uno dei seguenti valori:

- **Password Attuale:** selezionando questa opzione il campo in esame
  dovrà essere utilizzato per consentire all'utente di inserire la
  password attualmente in uso.

> In queste condizioni dunque, verrà attivato un particolare controllo a
> seguito del quale il relativo form potrà essere validato solo nel
> momento in cui la password inserita dall'utente coincida esattamente
> con quella attualmente utilizzata.
>
> **ATTENZIONE!** Per ovvie ragioni questo tipo di campo dovrà essere
> inserito solo nel form di Profilo Utente e consentirà di gestire un
> maggior livello di sicurezza sulla funzione di Cambio Password

- **Password:** selezionando questa opzione il campo in esame dovrà
  essere utilizzato per consentire all'utente di inserire la sua nuova
  password di accesso al sito.

> Il valore inserito dall'utente verrà poi memorizzato sul gestionale
> all'interno del relativo campo.

- **Conferma Password:** selezionando questa opzione il campo in esame
  dovrà essere utilizzato per validare la password scelta dall'utente.

> In queste condizioni dunque, verrà abilitato un particolare controllo
> a seguito del quale il relativo form potrà essere validato solo nel
> momento in cui il dato inserito all'interno del campo "Password"
> coincida esattamente con quello inserito all'interno del campo
> "Conferma Password"

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

Considerata la natura di questo campo è abbastanza semplice comprendere
come **sia obbligatorio** inserirlo all'interno del form di
registrazione. E' anzi consigliato inserire all'interno del form sia il
campo Password che il campo Conferma Password.

Chiaramente oltre ad un Componente di questo tipo sarà poi necessario
inserire all'interno del form di registrazione anche un Componente di
tipo "Campo Testo" corrispondente al campo "Username" in modo tale da
consentire all'utente di poter impostare anche la propria login di
accesso al sito.

> **NOTA BENE:** al fine di garantire il corretto funzionamento del
> sito, permettendo la registrazione di nuovi clienti (siti B2C), è
> obbligatorio inserire all'interno del form di registrazione un
> componente" Campo di Testo" corrispondente al campo Mexal "Login:
> Utente" e un Componente "Campo Password". Nel caso di siti B2B con
> accesso al sito solo da parte degli Agenti è invece possibile
> realizzare anche form di registrazione privi di questi campi.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

