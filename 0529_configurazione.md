# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image3.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**Statico**: consente di decidere se il componente in esame deve o meno
essere reso statico

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Tipo di conferma:** permette di decidere come si dovrà comportare il
componente nel momento in cui l'utente cliccherà sul pulsante di login
effettuando così il submit del form. E' possibile selezionare uno dei
seguenti valori:

- **Con caricamento della pagina:** in queste condizioni al click sul
  pulsante di login verrà ricaricata l'intera pagina web.

- **Senza caricamento della pagina:** in queste condizioni al click sul
  pulsante di login verrà ricaricato solo il componente in esame senza
  effettuare il reload dell'intera pagina web

**ATTENZIONE!** Nel caso in cui si desideri inserire il componente di
login all'interno di un pop up, di un componente "Contenuti su tab" o
"Contenuti su Accordion" sarà necessario impostare il parametro "Tipo di
Conferma" sul valore "Senza il caricamento della pagina"

In caso contrario verrebbe infatti ricaricata l'intera pagina web e,
soprattutto nel caso in cui il pannello di login fosse stato inserito
all'interno di un pop up, non sarebbe possibile visualizzare eventuali
errori riscontrati in fase di autenticazione a meno di non riaprire
manualmente la finestra di login e/o a meno di non gestire codice
javascript personalizzato che, in caso di errore, riapra questa stessa
finestra di login in maniera automatica.

**Pagina di destinazione all'autenticazione:** consente di specificare
la pagina del sito cui l'utente verrà automaticamente ridiretto dopo
aver effettuato il login **nel caso in cui non siano presenti articoli
in carrello.**

Il pulsante "**Deseleziona**"
(![](./assets/media/image4.png) ), presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

**Pagina di destinazione all'autenticazione in fase di acquisto:**
consente di specificare la pagina del sito cui l'utente verrà
automaticamente ridiretto dopo aver effettuato il login **nel caso in
cui siano già stati inseriti articoli in carrello e/o si sia già scelto
di prenotare uno specifico trattamento/servizio**. Il pulsante
"**Deseleziona**" (
![](./assets/media/image4.png) ), presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

> **NOTA BENE:** la pagina cui verrà effettivamente ricondotto l'utente
> dopo aver effettuato il login al sito dipende non solo dai due
> parametri sopra evidenziati ma anche dal fatto di aver già inserito o
> meno articoli in carrello o dal fato di aver già selezionato o meno
> uno specifico servizio/trattamento da prenotare

In particolare, dunque, in relazione alla pagina cui verrà
effettivamente ricondotto l'utente dopo aver effettuato l'accesso al
sito occorrerà considerare il seguente schema:

![](./assets/media/image5.png)

**Pagina di destinazione uguale anche per gli Agenti:** consente di
impostare la specifica pagina del sito cui dovranno essere ridiretti gli
Agenti nel momento in cui dovessero effettuare l'autenticazione
utilizzando il pannello di login in esame. Nello specifico dunque nel
caso in cui il parametro in oggetto sia:

- **Deselezionato**: gli Agenti che effettueranno l'autenticazione,
  utilizzando il pannello di login in esame, **verranno ridiretti sempre
  e comunque in Area Riservata** (in particolare nella Bacheca),
  indipendentemente dalle impostazioni settate per gli altri parametri
  di configurazione.

- **Selezionato**: gli Agenti che effettueranno l'autenticazione,
  utilizzando il pannello di login in esame, verranno ricondotti
  esattamente alla stessa pagina cui sono ricondotti anche gli utenti di
  tipo "Cliente".

> In queste condizioni sarà quindi necessario inserire all'interno del
> sito appositi link di collegamento all'Area Riservata in maniera tale
> da dare comunque la possibilità all'Agente di accedere a questa
> specifica sezione del sito.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Login Utente" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore".** Sarà infatti
possibile inserire al suo interno dei campi che, per poter esser gestiti
liberamente, dovranno inevitabilmente esser trattati a loro volta come
Componenti autonomi editabili singolarmente.

Una volta inserito il Componente all'interno della pagina, per poterne
poi personalizzare i contenuti sarà necessario attivare la modalità di
gestione dei componenti, portarsi sul Componente in esame e, alla
comparsa del R.O.C. cliccare sull'icona "**Accedi ai componenti
interni"**

**Per maggiori informazioni relativamente alla gestione dei Componenti
di tipo Contenitore si veda anche il corrispondente capitolo di questo
manuale ("Live Editing per Varianti Responsive -- Componenti --
Componenti di tipo Contenitore")**

In particolare all'interno di un componente di tipo "Login Utente" sarà
possibile inserire due differenti tipologie di componenti.

- **Componenti Comuni:** contiene componenti generici che potranno
  essere utilizzati per completare graficamente il componente in esame.
  Per maggiori informazioni relativamente all'utilizzo di questi
  componenti si vedano le corrispondenti sezioni di questo manuale.

- **Componenti per il Form:** contiene i campi di Login e Password
  (corrispondenti alle relative funzionalità utente, da inserire
  obbligatoriamente all'interno del Componente per poterne garantire il
  corretto funzionamento), il componente Ricordami e il componente
  Social Login utile nel momento in cui si volesse concedere agli utenti
  del sito la possibilità di autenticarsi utilizzando i propri profili
  social.

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> i Componenti Interazione Utente interni al "Pannello di Login" si veda
> la corrispondente sezione di questo manuale (Live Editing per Varianti
> Responsive -- Lista Componenti Interazione Utente -- Componenti
> Interni ai Componenti Interazione Utente).

