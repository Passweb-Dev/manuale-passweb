# COSA FARE IN PASSWEB



Per poter attivare il flusso di gestione delle conversioni offline,
all'interno di Passweb sarà necessario operare in maniera leggermente
diversa a seconda del fatto di gestire il tracciamento client della
conversione di acquisto direttamente dal sito oppure mediante Google Tag
Manager.

**[TRACCIAMENTO CLIENT DELLA CONVERSIONE DI ACQUISTO DAL SITO
PASSWEB]{.underline}**

In questo caso sarà necessario:

- Accertarsi di richiedere la mail come dato obbligatorio in fase di
  registrazione al sito

- Settare i parametri presenti all'interno della sezione "**Google
  Ads**" alla pagina "**Sito -- Preferenze**" del Wizard (tab
  "**Tracciamento Dati**") come descritto nel capitolo "*Sito --
  Preferenze -- Tracciamento Dati -- Google -- Google Ads*" di questo
  manuale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_1.bmp](./assets/media/image30.png){width="5.766666666666667in"
height="3.3in"}

**ATTENZIONE!** il consiglio, come indicato anche nella stessa
documentazione di Google Ads, è quello di attivare sempre anche il
parametro "**Inserisci GCLID export CSV**" in maniera tale da inserire
nel file che verrà poi importato su Ads anche questo valore (ovviamente
se presente).

**[TRACCIAMENTO CLIENT DELLA CONVERSIONE DI ACQUISTO MEDIANTE GOOGLE TAG
MANAGER]{.underline}**

In questo caso sarà necessario:

- Accertarsi di richiedere la mail come dato obbligatorio in fase di
  registrazione al sito.

- Accertarsi di aver correttamente attivato il parametro "Raccolta Dati
  Utente nel Data Layer" presente all'interno della sezione "**Google
  Tag Manager**" alla pagina "**Sito -- Preferenze**" del Wizard (tab
  "**Tracciamento Dati**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_2.bmp](./assets/media/image31.png){width="5.766666666666667in"
height="3.3in"}

L'attivazione del parametro evidenziato in figura farà si che nel
momento in cui l'utente abbandonerà il sito per essere ridiretto al
gateway di pagamento della banca, verrà inserito nel dataLayer l'evento
"***set_user_data_passweb***" contenente la mail hashata di questo
stesso utente.

In queste condizioni il dataLayer avrà quindi una struttura del tipo di
quella di seguito indicata

*{*

*event: 'set_user_data_passweb',*

*user_data: {*

*sha256_email_address: valore hashato della mail utente ,*

*sha256_phone_number: valore hashato del telefono utente,*

*address: {*

*sha256_first_name: valore hashato del nome utente,*

*sha256_last_name: valore hashato del cognome / ragione sociale utente,*

*street: indirizzo utente (via),*

*city: indirizzo utente (città),*

*postal_code: indirizzo utente (CAP),*

*country: indirizzo utente (Nazione)*

*}*

*}*

Detto questo all'interno di Google Tag Manager sarà poi necessario:

1.  Creare delle variabili di livello dati che leggano il valore dei
    dati utente presenti nel dataLayer.

> Per maggiori informazioni su questo tipo di operazione si veda anche
> quanto indicato all'interno del capitolo "*Google Tag Manager -- User
> Provided Data e Conversioni Avanzate -- Creazione delle variabili per
> la gestione dei dati*" di questo manuale

2.  Creare una variabile di tipo User Provided Data impostata con una
    configurazione di tipo Manuale e con i vari campi Email, Telefono
    ... impostato sulle variabili di livello dati definite al punto
    precedente

> Per maggiori informazioni su questo tipo di operazione si veda anche
> quanto indicato all'interno del capitolo "*Google Tag Manager -- User
> Provided Data e Conversioni Avanzate -- Creazione delle variabili per
> la gestione dei dati utente -- Variabile PWB User Provided Data*" di
> questo manuale

3.  Creare un Tag di tipo "**Google Ads User-provided Data Event**" con
    il parametro "User-provided Data" impostato sulla variabile definita
    al punto precedente e che si attiva sull' evento custom di nome
    ***set_user_data_passweb***

In questo modo dunque nel momento in cui l'utente abbandonerà il sito
per essere ricondotto al gateway di pagamento, esattamente come avveniva
anche nel tracciamento diretto da Sito, Tag Manager si preoccuperà di
prelevare dal dataLayer i dati dell'utente e di inviarli a Google Ads
(passaggio questo fondamentale perché, come ormai dovremmo aver capito,
la mail, assieme al gclid, è quella che consentirà poi ad Ads di
associare in maniera corretta la conversione quando andremo ad importare
offline il file contenente i dati dell'ordine)

