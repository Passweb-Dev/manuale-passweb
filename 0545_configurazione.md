# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_step_40.bmp](./assets/media/image35.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di definire un nome per il Componente "Iscrizione
Newsletter " che si sta editando

**Pubblico**: consente di impostare la visibilità del componente in
esame. Lasciando il flag deselezionato, il relativo componente verrà
comunque inserito all'interno della pagina, sarà quindi visibile e
personalizzabile graficamente lato Wizard, ma NON risulterà visibile
lato Front End.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Tipo di integrazione:** consente di specificare la piattaforma
utilizzata per gestire il sistema di Newsletter. E' possibile
selezionare una delle seguenti opzioni:

- MailChimp

- ActiveCampaign

- Brainlead

**ATTENZIONE!** per poter gestire il sistema di newsletter con Brainlead
/ ActiveCampaign è richiesta l'attivazione del relativo modulo su
Passstore

**Tipologia Form:** consente di specificare il tipo di Form che si
desidera inserire e integrare all'interno del proprio sito Passweb.

Dipendentemente da quanto impostato all'interno del precedente parametro
sarà possibile selezionare una delle seguenti opzioni:

- **Iscrizione -- disponibile solo per MailChimp:** consente di gestire
  il form di iscrizione al servizio di Newsletter (corrispondente al
  "S**ignup** **form**") realizzato in MailChimp

<!-- -->

- **Disiscrizione -- disponibile per MailChimp / Brainlead /
  ActiveCampaign:** consente di gestire il form di cancellazione dal
  servizio di Newsletter gestito con la relativa piattaforma.

**Tipo di conferma:** permette di decidere come si dovrà comportare il
componente nel momento in cui l'utente cliccherà sul pulsante di
iscrizione / disiscrizione effettuando così il submit del form. E'
possibile selezionare uno dei seguenti valori:

- **Con caricamento della pagina:** in queste condizioni al click sul
  pulsante di iscrizione verrà ricaricata l'intera pagina web.

- **Senza caricamento della pagina:** in queste condizioni al click sul
  pulsante di conferma verrà ricaricato solo il componente in esame
  senza effettuare il reload dell'intera pagina web

**ATTENZIONE!** Nel caso in cui si desideri inserire il componente di
iscrizione alla newsletter all'interno di un pop up, di un componente
"Contenuti su tab" o "Contenuti su Accordion" sarà necessario impostare
il parametro "Tipo di Conferma" sul valore "Senza il caricamento della
pagina"

In caso contrario verrebbe infatti ricaricata l'intera pagina web e,
soprattutto nel caso in cui il form di iscrizione fosse stato inserito
all'interno di un pop up, non sarebbe possibile visualizzare eventuali
errori riscontrati in fase di validazione a meno di non riaprire
manualmente la finestra di pop up e/o a meno di non gestire codice
javascript personalizzato che, in caso di errore, riapra questa stessa
finestra in maniera automatica.

**Lista Associata -- disponibile per MailChimp e ActiveCampaign**:

In particolare nel caso di:

- **MailChimp**: consente di indicare, selezionandola tra quelle
  realizzate e disponibili nel proprio account MailChimp, la specifica
  Lista cui associare il form di iscrizione alla Newsletter (per
  maggiori informazioni in merito alla realizzazione in MailChimp delle
  varie liste si vedano i precedenti capitoli di questo manuale)

- **ActiveCampaign**: consente di indicare, selezionandola tra quelle
  gestite all'interno del proprio account ActiveCampaign, la specifica
  Lista da cui l'utente dovrà essere disiscritto.

> **ATTENZIONE!** Selezionando l'opzione "**Tutte**" l'utente verrà
> disiscritto da tutte le liste presenti su ActiveCampaign
>
> Per maggiori informazioni relativamente alla creazione e alla gestione
> delle Liste di ActiveCampaign si rimanda alla relativa documentazione
> di prodotto

**ATTENZIONE!** Il campo in esame è multilingua per cui è perfettamente
possibile associare una diversa lista ad ogni singola lingua gestita
all'interno del proprio sito

Supponendo dunque di gestire il nostro sito in Italiano, Inglese e
Francese, sarà possibile creare in MailChimp tre distinte liste di
iscrizione che raccolgano rispettivamente gli utenti italiani, quelli
inglesi e quelli francesi in maniera tale da poter poi inviare ad ogni
utente le Newsletter nella lingua corretta.

**Il fatto di iscriversi alla Lista in Italiano, a quella in Inglese
oppure a quella in Francese dipenderà poi dalla lingua attualmente
caricata sul sito al momento dell' iscrizione.**

Effettuando dunque l'iscrizione alla Newsletter dalla pagina in italiano
l'utente verrà iscritto alla Newsletter Italiana, registrandosi invece
dalla pagina in Inglese verrà iscritto alla Newsletter in Inglese così
come registrandosi dalla pagina in Francese verrà iscritto alla
Newsletter in Francese.

Lo stesso discorso vale, ovviamente, per la disiscrizione alle Liste di
ActiveCampaign

**ATTENZIONE**! nel caso di MailChimp per poter utilizzare una lista è
necessario che questa abbia associato almeno un gruppo di interesse

**Azione alla conferma:** consente di specificare l'azione che verrà
effettuata alla conferma del form. E' possibile selezionare uno dei
seguenti valori

- **Messaggio:** selezionando questo valore alla conferma da parte
  dell'utente dei dati immessi nel form, il form stesso scomparirà e al
  suo posto verrà visualizzato il messaggio inserito nel successivo
  campo **"Messaggio"**.

- **Pagina di Ringraziamento:** selezionando questo valore, alla
  conferma del form l'utente verrà ridiretto alla pagina selezionata nel
  sottostante albero delle pagine (**Pagina di ringraziamento**).

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- Il form di iscrizione

- Il pulsante di iscrizione

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

