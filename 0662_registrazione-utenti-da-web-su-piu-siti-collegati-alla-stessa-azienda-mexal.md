# REGISTRAZIONE UTENTI DA WEB SU PIU' SITI COLLEGATI ALLA STESSA AZIENDA MEXAL



Considerata la possibilità, come visto, di collegare ad una stessa
azienda più siti differenti (**fino ad un massimo di 9**) diventa di
fondamentale importanza comprendere bene come viene gestita, a livello
di anagrafiche Mexal, la registrazione di uno stesso utente su due o più
siti collegati tutti alla stessa azienda.

In questo senso vanno quindi considerate le seguenti condizioni:

- Nel caso in cui uno **stesso utente privato** **si registri con gli
  stessi dati**, effettuando anche degli ordini, su due o più siti
  collegati alla stessa azienda Mexal, **lato gestionale verranno create
  sempre e comunque anagrafiche utente distinte.**

> Supponendo dunque che l'utente Mario Rossi si registri al sito
> *www.sito1.passweb.it* collegato all'azienda Mexal ECP ed effettui
> anche un ordine, contestualmente all'inserimento di tale ordine verrà
> inserita in Mexal anche una prima anagrafica, per l'utente Mario
> Rossi, con i dati da lui stesso inseriti all'interno del form di
> registrazione sul sito 1.
>
> Supponendo poi che lo stesso utente Mario Rossi si registri, con gli
> stessi dati, anche sul sito *www.sito2.passweb.it* collegato sempre
> alla stessa azienda Mexal ECP ed effettui anche qui un ordine,
> contestualmente all'inserimento di quest'ordine verrà creata in Mexal
> anche una seconda anagrafica, per lo stesso utente Mario Rossi.
>
> I dati aggiuntivi (es. Login e Password) relativi all'utente Mario
> Rossi che si è registrato sul sito 1 saranno memorizzati e gestiti in
> Mexal, nella prima anagrafica sui relativi campi della videata
> aggiuntiva clienti/fornitori appositamente riservata per il sito 1
>
> Allo stesso modo i dati aggiunti relativi allo stesso utente che si è
> registrato sul sito 2 saranno memorizzati e gestiti in Mexal, nella
> seconda anagrafica sui relativi campi della videata aggiuntiva
> clienti/fornitori appositamente riservata per il sito 2.

- Nel caso in cui **uno stesso utente di tipo Azienda si registri con la
  stessa Partita IVA,** effettuando anche degli ordini su due o più siti
  collegati alla stessa azienda Mexal **potranno o meno essere create,
  lato gestionale, anagrafiche distinte** dipendentemente dal fatto di
  aver selezionato o meno, in fase di configurazione dei siti, il
  parametro "**Gestione Iva Secondaria**" presente alla pagina
  **"*Utenti -- Gestione Parametri Utenti Ecommerce -- Configurazione
  Utenti*"** del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\multi_sito_ec17.bmp](./assets/media/image103.png)

> Per maggiori informazioni relativamente al parametro "Gestione Iva
> Secondaria" si veda anche il capitolo "*Utenti -- Gestione Parametri
> Utenti Ecommerce -- Configurazione Utenti"* di questo manuale.
>
> In particolare dunque:

- Nel caso in cui **sia stato selezionato il parametro** **"Gestione Iva
  Secondaria"** sopra evidenziato, se uno stesso utente si dovesse
  registrare, effettuando poi degli ordini, su due siti diversi
  collegati alla stessa azienda **indicando nei form di registrazione
  dei due siti la stessa Partita IVA**, verranno comunque create, lato
  gestionale, due anagrafiche utente distinte (esattamente come avveniva
  per gli utenti privati)

> **ATTENZIONE! Il parametro Gestione Iva Secondaria va, ovviamente,
> selezionato su tutti i siti collegati alla stessa azienda Mexal**

- Nel caso in cui si sia deciso invece di **non selezionare il
  parametro** **"Gestione Iva Secondaria",** se uno stesso utente si
  dovesse registrare, effettuando poi degli ordini, su due siti diversi
  collegati alla stessa azienda **indicando nei form di registrazione
  dei due siti la stessa Partita IVA**, lato gestionale verrà poi creata
  e gestita per questo stesso utente **una sola anagrafica**.

> In queste condizioni dunque i dati inseriti dall'utente su sito 2
> andranno a sovrascrivere quelli precedentemente inseriti dallo stesso
> utente sul sito 1 (e viceversa).
>
> **ATTENZIONE!** In realtà la sovrascrittura che potrebbe verificarsi
> nelle suddette condizioni, riguarderebbe i soli campi standard
> dell'anagrafica utente. I campi aggiuntivi (es. Login e Password)
> continueranno invece ad essere gestiti individualmente mediante le
> apposite videate aggiuntive clienti/fornitori riservate in Mexal per
> lo specifico sito.

- Nel caso in cui sia stata attivata in Passweb la gestione dei
  contatti, se uno stesso utente, **sia esso privato o azienda**, si
  dovesse registrare su più siti collegati alla stessa azienda Mexal
  indicando gli stessi dati, verranno create in Mexal, nella
  corrispondente tabella "**Anagrafica Contatti", sempre e comunque
  delle anagrafiche distinte**.

