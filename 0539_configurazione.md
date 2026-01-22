# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image20.png)

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

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Tipologia Utente:** consente di specificare la tipologia di utente che
potrà effettuare la registrazione al sito. E' possibile selezionare uno
dei seguenti valori:

- **Privato:** in queste condizioni potranno effettuare la registrazione
  al sito i soli utenti di tipo "Privato". In conseguenza di ciò tutti i
  campi del form relativi ad utenti di tipo "Azienda" (es. Partita iva,
  Ragione Sociale ecc\...), sul front end del sito verranno
  automaticamente nascosti.

> Utenti di tipo "Privato" creeranno poi, all'interno di Mexal,
> anagrafiche utente con entrambi i campi "**Soggetto Privato**" e
> "**Persona Fisica**" selezionati

![](./assets/media/image21.png)

- **Azienda:** in queste condizioni potranno effettuare la registrazione
  al sito i soli utenti di tipo "Azienda". In conseguenza di ciò tutti i
  campi del form relativi ad utenti di tipo "Privato" (es. Nome, Cognome
  ecc\...), sul front end del sito verranno automaticamente nascosti

> Utenti di tipo "Azienda" creeranno poi, all'interno di Mexal,
> anagrafiche utente con il campo "**Soggetto Privato**" deselezionato

![](./assets/media/image22.png)

> In queste condizioni inoltre sarà possibile inserire nel form di
> registrazione di siti Ecommerce collegati a Mexal, un'ulteriore campo
> mediante il quale l'utente di tipo Azienda avrà la possibilità di
> indicare se si stratta o meno di una ditta individuale e se dovrà
> quindi essere registrato come persona fisica o come persona giuridica.
>
> Nel primo caso (persona fisica) verrà creata in Mexal un'anagrafica
> utente con il campo "Persona Fisica" selezionato; nel secondo caso
> invece (persona giuridica) verrà creata in Mexal un'anagrafica utente
> con il campo "Persona Fisica" deselezionato
>
> Per maggiori informazioni in merito si consiglia di fare riferimento a
> quanto indicato all'interno del capitolo "*Varianti Sito Responsive --
> Lista componenti Interazione Utente -- Componenti interni ai
> componenti Interazione Utente -- Campo Radio (Registrazione e Profilo
> Utente)*" di questo manuale

- **A scelta:** in queste condizioni verrà visualizzato all'interno del
  form un radio button attraverso il quale l'utente che effettua la
  registrazione potrà indicare la propria tipologia (Privato o Azienda)
  e conseguentemente visualizzare all'interno tutti i campi necessari
  per completare la registrazione in maniera corretta.

**Tipo di conferma:** permette di decidere come si dovrà comportare il
componente nel momento in cui l'utente cliccherà sul pulsante di
conferma effettuando così il submit del form. E' possibile selezionare
uno dei seguenti valori:

- **Con caricamento della pagina:** in queste condizioni al click sul
  pulsante di login verrà ricaricata l'intera pagina web.

- **Senza caricamento della pagina:** in queste condizioni al click sul
  pulsante di conferma verrà ricaricato solo il componente in esame
  senza effettuare il reload dell'intera pagina web

**ATTENZIONE!** Nel caso in cui si desideri inserire il componente di
Registrazione Utente all'interno, ad esempio, di un componente
"Contenuti su tab" o "Contenuti su Accordion", è consigliabile impostare
il parametro "Tipo di Conferma" sul valore "Senza il caricamento della
pagina"

In caso contrario verrebbe infatti ricaricata l'intera pagina web e, in
conseguenza di ciò, verrebbe sempre visualizzato il primo tab e/o il
primo pannello dell'accordion. Posto quindi di aver inserito il
componente di registrazione in un tab e/o in un pannello dell'accordion
successivo al primo, per verificare la presenza di eventuali errori in
compilazione del form sarebbe poi necessario selezionare manualmente il
tab e/o il pannello dell'accordion in cui si era deciso di inserire il
form di registrazione

**Pagina di destinazione alla registrazione:** consente di specificare
la pagina del sito cui l'utente verrà automaticamente ridiretto dopo
essersi registrato **nel caso in cui non siano presenti articoli in
carrello e l'utente in questione sia gestito con una modalità di
attivazione "Immediata".**

Il pulsante "**Deseleziona**"
(![](./assets/media/image4.png) ) presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

**Pagina di destinazione all'autenticazione in fase di acquisto:**
consente di specificare la pagina del sito cui l'utente verrà
automaticamente ridiretto dopo essersi registrato **nel caso in cui
siano già stati inseriti articoli in carrello e l'utente in questione
sia gestito con una modalità di attivazione "Immediata"**.

Il pulsante "**Deseleziona**"
(![](./assets/media/image4.png) ), presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

**Pagina di destinazione alla registrazione con Attivazione Differita:**
consente di specificare la pagina del sito cui l'utente verrà
automaticamente ridiretto dopo essersi registrato **nel caso in cui
l'utente in questione sia gestito con una modalità di attivazione
"Differita".**

Il pulsante "**Deseleziona**"
(![](./assets/media/image4.png) ), presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

> **NOTA BENE:** la pagina cui verrà effettivamente ricondotto un utente
> gestito con attivazione immediata dopo essersi registrato, dipende non
> solo dai parametri sopra evidenziati ma anche dal fatto di aver già
> inserito o meno articoli in carrello o dal fato di aver già
> selezionato o meno uno specifico servizio/trattamento da prenotare.

In particolare, dunque, in relazione alla pagina cui verrà
effettivamente ricondotto un utente gestito con attivazione "Immediata"
dopo aver effettuato l'accesso al sito occorrerà considerare il seguente
schema:

![](./assets/media/image23.png)

La sezione **"Attivazione tramite Verifica Mail"** consente, infine, di
definire quello che dovrà essere il comportamento dell'applicazione
all'atto della verifica del proprio indirizzo mail nel caso in cui
l'attivazione dei nuovi utenti venga gestita tramite **"Verifica
dell'indirizzo Email"**

> **NOTA BENE:** per maggiori informazioni relativamente alle modalità
> di attivazione di un nuovo utente si veda anche la sezione "Utenti --
> Gestione Parametri Utenti Ecommerce" di questo manuale

In questo senso dunque il parametro:

**Effettua il login alla verifica della mail:** consente di specificare
se, a seguito della verifica dell'indirizzo mail da parte dell'utente
che effettua la registrazione al sito, questo dovrà essere o meno
autenticato in maniera automatica

**Pagina di destinazione alla verifica della mail:** consente di
impostare la pagina cui dovrà essere automaticamente ridiretto l'utente
a seguito della verifica del suo indirizzo mail.

Il pulsante "**Deseleziona**"
(![](./assets/media/image4.png) ) presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

Nel caso in cui non venga indicata una specifica pagina una volta
effettuata la verifica del proprio indirizzo mail in maniera corretta
l'utente verrà ricondotto alla pagina "Profilo Utente"

In sostanza dunque, nel caso in cui si sia deciso di gestire
l'attivazione dei nuovi utenti mediante "Verifica Mail", nel momento in
cui l'utente completerà la propria registrazione, verrà posto,
all'interno di Passweb, nello stato di "**Contatto Non Verificato**" e
l'applicazione invierà all'indirizzo indicato una mail (quella di "Nuovo
Utente Ecommerce") contenente, tra le altre cose, anche il link sul
quale cliccare per effettuare la verifica del proprio indirizzo. Tale
link farà riferimento alla pagina "Registrazione" del sito.

Nel caso in cui la verifica in questione dia esito negativo, ad esempio
perché l'utente anziché cliccare sul link presente nella mail lo copia e
lo incolla in maniera non corretta nella barra degli indirizzi del
browser, o più semplicemente perché sono trascorse le 24 ore entro cui
dover necessariamente effettuare la verifica richiesta, verrà
visualizzato nella parte alta del componente "Registrazione Utente" un
messaggio di errore ad indicare appunto la mancata verifica e la
conseguente non attivazione del relativo account.

> **NOTA BENE:** in fase di sincronizzazione verranno automaticamente
> eliminati dal database di Passweb tutti i contatti non verificati e
> registrati da più di un giorno

Il contenuto di questo messaggio di errore potrà essere personalizzato
all'interno della sezione "**Gestione Testi/Messaggi**" del sito agendo
sui testi del componente "**Registrazione Utente**" e nello specifico
sulle due voci "**Link Errato**" e "**Mail già Verificata**":

![](./assets/media/image24.png)

- **Link Errato:** consente di personalizzare il messaggio di errore che
  verrà visualizzato nel caso in cui il link di verifica non sia
  corretto o nel caso in cui siano già trascorse le 24 ore entro cui
  dover necessariamente effettuare la verifica richiesta

- **Mail già verificata:** consente di personalizzare il messaggio di
  errore che verrà visualizzato nel caso in cui il link di verifica sia
  già stato visitato e il relativo utente già attivato

A livello grafico i messaggi di errore sopra indicati potranno essere
personalizzati agendo sul corrispondente elemento (Messaggio Errore
Verifica Mail) presente nello style editor del componente registrazione.

Nel caso in cui, invece, la verifica del proprio indirizzo mail dia
esito positivo l'utente verrà immediatamente attivato e automaticamente
passato dallo stato di "Contatto Non Verificato" allo stato di
"**Contatto**". A verifica effettata inoltre, l'utente verrà anche
ridiretto alla pagina selezionata all'interno del campo **"Pagina di
destinazione alla verifica della mail"** precedentemente esaminato e,
dipendentemente dal fatto di aver selezionato o meno il flag **"Effettua
il login alla verifica della mail"** per questo stesso utente potrà
anche essere effettuata in maniera del tutto automatica l'autenticazione
al sito.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Registrazione Utente" può essere considerato a tutti
gli effetti come un "Componente di tipo Contenitore".** Sarà infatti
possibile inserire al suo interno dei campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Una volta inserito il Componente all'interno della pagina, per poterne
poi personalizzare i contenuti sarà necessario attivare la modalità di
gestione dei componenti, portarsi sul Componente in esame e, alla
comparsa del R.O.C. cliccare sull'icona "**Accedi ai componenti
interni".**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Registrazione
Utente" sarà possibile inserire tre differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale

- **Componenti per il Form:** contiene tutta una serie di controlli che
  potranno essere fatti corrispondere a specifici campi del gestionale
  e/o a specifici Attributi Utente.

- **Interazione Utente:** contiene il componente di Iscrizione alla
  Newsletter da utilizzare nel momento in cui si desideri permettere
  agli utenti di iscriversi alla Newsletter direttamente in fase di
  registrazione al sito. Per maggiori informazioni in questo senso, si
  veda anche la sezione "*Live Editing per Varianti Responsive -- Lista
  componenti Interazione Utente -- Componente Iscrizione Newsletter --
  Iscrizione alla Newsletter in fase di registrazione / Modifica
  Profilo*" di questo manuale.

Ovviamente per poter garantire il corretto funzionamento del Componente
"Registrazione Utente" alcuni dei campi sopra evidenziati dovranno
obbligatoriamente essere inseriti all'interno del form di registrazione.
E' il caso ad esempio dei campi relativi allo Username e alla Password,
campi necessari per poter consentire all'utente di impostare in fase di
registrazione quelle che poi diventeranno le proprie credenziali di
accesso al sito.

> **NOTA BENE:** per poter garantire il corretto funzionamento del form
> di registrazione è obbligatorio inserire al suo interno il Componente
> "Campo Password" e un Componente "Campo di Testo" mappato con il campo
> utilizzato per gestire la Username di accesso al sito

**Oltre alla Username e alla Password è fortemente consigliato, inoltre,
di inserire all'interno del form di registrazione anche tutti i campi
necessari a comporre almeno un indirizzo completo in maniera tale da
consentire all'utente che si registra di poter effettuare correttamente
il suo primo ordine.**

Per il resto sarà possibile far corrispondere i vari controlli (Campo di
Testo, Campo Radio, Campo Lista Valori ecc. ...) indifferentemente ad
alcuni campi dell'Anagrafica Clienti/Fornitori di Mexal o di Videate
Aggiuntive Clienti/Fornitori appositamente realizzate.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Interazione Utente interni alla "Registrazione Utente" si
> veda la corrispondente sezione di questo manuale (Live Editing per
> Varianti Responsive -- Lista Componenti Interazione Utente --
> Componenti Interni ai Componenti Interazione Utente).

All'interno del form di registrazione verrà poi collocato a default un
controllo di tipo "Radio Button" necessario per determinare se l'utente
che sta effettuando la registrazione dovrà essere considerato da Passweb
come una persona fisica oppure come un'azienda. Dipendentemente dalla
scelta effettuata dall'utente in tal senso, potranno poi essere
visualizzati o nascosti alcuni campi all'interno del form.

L'inserimento dei vari componenti all'interno del Componente
"Registrazione Utente" avviene utilizzando le solite tecniche di
interazione con l'editor (Drag and Drop o Point and Click) già esaminate
all'interno di questo manuale (per maggiori informazioni si rimanda allo
specifico capitolo di questo manuale).

Come si può notare, infine, i controlli presenti all'interno del
raggruppamento "Componenti per il Form" sono esattamente gli stessi di
quelli presenti per il Componente "Form" generico precedentemente
esaminato.

In definitiva la procedura per la creazione del form di registrazione
non si discosta di molto da quella per la creazione di un form generico.
La principale differenza tra un Form generico ed il Form di
Registrazione Utente consiste dunque nella necessità di far
corrispondere, in quest'ultimo caso, alcuni controlli inseriti
all'interno del form a specifici campi Mexal, in maniera tale che la
varie informazioni possano poi essere riportate all'interno del
gestionale.

