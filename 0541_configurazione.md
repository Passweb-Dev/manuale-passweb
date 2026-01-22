# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_profilo_utente_configurazione_res.bmp](./assets/media/image26.png){width="4.636111111111111in"
height="2.077777777777778in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** permette di inserire un nome per il campo che si sta editando;

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

**Tipo di conferma:** permette di decidere come si dovrà comportare il
componente nel momento in cui l'utente cliccherà sul pulsante di
conferma effettuando così il submit del form. E' possibile selezionare
uno dei seguenti valori:

- **Con caricamento della pagina:** in queste condizioni al click sul
  pulsante di login verrà ricaricata l'intera pagina web.

- **Senza caricamento della pagina:** in queste condizioni al click sul
  pulsante di conferma verrà ricaricato solo il componente in esame
  senza effettuare il reload dell'intera pagina web

**ATTENZIONE!** Nel caso in cui si desideri inserire il form
all'interno, ad esempio, di un componente "Contenuti su tab" o
"Contenuti su Accordion", è consigliabile impostare il parametro "Tipo
di Conferma" sul valore "Senza il caricamento della pagina"

In caso contrario verrebbe infatti ricaricata l'intera pagina web e, in
conseguenza di ciò, verrebbe sempre visualizzato il primo tab e/o il
primo pannello dell'accordion. Posto quindi di aver inserito il
componente in un tab e/o in un pannello dell'accordion successivo al
primo, per verificare la presenza di eventuali errori in compilazione
del form sarebbe poi necessario selezionare manualmente il tab e/o il
pannello dell'accordion in cui si era deciso di inserire il form del
profilo utente

**Pulsante di Elimina Utente:** se selezionato consente di attivare
all'interno del form un pulsante mediante il quale l'utente avrà la
possibilità di cancellare il proprio profilo e, conseguentemente, la
propria iscrizione al sito.

![Videate\\elimina_profilo.bmp](./assets/media/image27.png){width="5.552083333333333in"
height="3.298611111111111in"}

**Cliccando su questo pulsante oltre a cancellare la sua anagrafica dal
database di Passweb, questa verrà completamente eliminata, se presente,
anche da un eventuale piattaforma terza utilizzata per la gestione delle
Newsletter.**

Nel momento in cui si dovesse implementare l'integrazione con una delle
piattaforme di newsletter gestite da Passweb si consiglia quindi di
personalizzare il messaggio di "conferma eliminazione del profilo"
indicando che i dati dell'utente verranno, eventualmente, cancellati
anche dalla piattaforma di newsletter utilizzata.

![Videate\\messaggio_conferma_eliminazione_profilo.bmp](./assets/media/image28.png){width="5.552083333333333in"
height="3.298611111111111in"}

**ATTENZIONE!** In queste condizioni va ricordato inoltre che:

- se la piattaforma utilizzata per la Newsletter dovesse essere
  MailChimp, un utente eliminato in maniera definitiva potrà
  eventualmente reiscriversi alla stessa Newsletter **solo attraverso
  uno dei form nativi di MailChimp stesso** (l'iscrizione attraverso
  form Passweb, quindi, non potrà più essere utilizzata)

- La cancellazione dell'anagrafica utente effettuata dal backend
  (Wizard) del sito Passweb NON comporta l'eliminazione della stessa
  anagrafica anche dal database della piattaforma utilizzata per gestire
  la Newsletter.

I testi del pulsante di cancellazione e quello relativo al messaggio
visualizzato una volta completata la procedura di eliminazione, possono
essere personalizzati all'interno della sezione "*Testi/Messaggi del
Sito -- Testi dei Componenti*" del Wizard agendo ovviamente sul
componente "Profilo Utente"

Una volta terminata correttamente la procedura di eliminazione, il
sistema potrà provvedere ad inviare automaticamente due mail di avvenuta
cancellazione, una al cliente che ha appena effettuato l'operazione e
una all'amministratore del sito. Per maggiori informazioni su come
attivare l'invio di tali mail si veda anche la sezione "*Utenti -- Siti
Ecommerce -- Configurazione Utenti Sito -- Configurazione Utenti -- Dati
Email*" di questo manuale.

In merito alla procedura di cancellazione dell'utente è bene
sottolineare poi alcune cose di fondamentale importanza.

Nello specifico:

- Nel caso in cui l'utente che decide di eliminare il proprio profilo
  sia un **Utente di tipo Contatto** (e quindi non ancora presente nelle
  anagrafiche gestionali) la cancellazione del suo profilo dal database
  del sito sarà immediata.

- Nel caso in cui invece il cliente che decide di eliminare il proprio
  profilo sia un **Utente di tipo Cliente** (e quindi già presente nelle
  anagrafiche gestionali) l'eliminazione del profilo dal database del
  sito non sarà immediata. Nello specifico, l'utente verrà posto
  inizialmente in uno stato di "**Cancellato**" a seguito del quale non
  sarà più gestibile ne sul back end ne tanto meno sul front end del
  sito. Successivamente a seguito della prima sincronizzazione parziale
  utile l'utente verrà eliminato definitivamente dal database del sito e
  il campo "**Trasferisci sul sito**" (per Ecommerce Mexal) o "**Sempre
  Attivo**" (per Ecommerce Ho.Re.Ca.) della sua anagrafica gestionale
  verrà automaticamente impostato in maniera tale da non esportarlo
  nuovamente durante le successive sincronizzazioni.

<!-- -->

- **tanto per i siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca
  quanto per quelli collegati a Mexal**, per gli utenti di tipo Cliente,
  l'anagrafica verrà eliminata, per ovvie ragioni, dal database del sito
  ma non dal gestionale dove i dati del cliente in esame verranno quindi
  mantenuti.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione dei suoi contenuti, le
modalità di inserimento all'interno del Componente dei vari campi e le
tipologie dei campi stessi, il Componente "**Profilo Utente**" è in
tutto e per tutto simile al Componente "Registrazione Utente"
precedentemente esaminato.

Per maggiori informazioni relativamente alla costruzione e
personalizzazione del form di Profilo Utente si rimanda dunque a quanto
detto per il Componente "**Registrazione Utente**".

> **NOTA BENE:** non è obbligatorio inserire all'interno del form di
> Profilo Utente gli stessi esatti campi presenti anche all'interno del
> form di registrazione

Volendo si potrebbero inserire dunque all'interno del form di Profilo
Utente anche campi completamente diversi da quelli richiesti all'utente
in fase di registrazione. In questo senso occorre comunque ricordare
sempre che l'utente potrà variare e/o aggiornare all'interno del proprio
profilo solamente i dati relativi ai campi inseriti all'interno del
Componente stesso (se vi vuol dare all'utente, ad esempio, la
possibilità di variare le proprie credenziali di accesso al sito,
ovviamente occorrerà inserire all'interno del form i campi relativi a
login e password).

