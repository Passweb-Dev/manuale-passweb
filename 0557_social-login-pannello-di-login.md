# SOCIAL LOGIN (PANNELLO DI LOGIN)



Il Componente **"Social Login"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_social_login_res.bmp](./assets/media/image78.png){width="2.5388888888888888in"
height="2.5388888888888888in"}

permette di inserire all'interno del pannello di login una serie di
pulsanti mediante i quali poter consentire agli utenti del sito di
effettuare l'autenticazione utilizzando direttamente i propri profili
social o il proprio Apple ID.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\social_login.bmp](./assets/media/image79.png){width="4.967361111111111in"
height="3.5131944444444443in"}

**Nel momento in cui un utente non ancora registrato sul sito Passweb
dovesse effettuare l'autenticazione utilizzando uno dei propri account
social, i dati prelevati dal relativo profilo verranno utilizzati per
creare automaticamente la nuova anagrafica utente Passweb.**

In relazione a ciò occorre considerare che i dati restituiti dalle varie
piattaforme social e utilizzati da Passweb per effettuare la
registrazione automatica del nuovo utente potrebbero non essere
sufficienti per il completamento del primo ordine.

Nello specifico, infatti, nel processo di integrazione tra il sito
Passweb e la piattaforma social verranno sicuramente prelevati dal
relativo profilo dell'utente:

- il suo **Nome**

- il suo **Cognome**

- il suo Indirizzo **Email**

dati questi obbligatori e necessari a Passweb per poter creare la nuova
anagrafica utente che, ovviamente, **sarà sempre quella di un utente**
**Privato.**

**ATTENZIONE!** La username della nuova anagrafica creata
automaticamente da Passweb coinciderà con l'indirizzo mail prelevato
direttamente dal profilo social.

Tra i dati prelevati dal profilo social potrebbe non essere presente
l'indirizzo dell' utente o perché la specifica piattaforma non consente
di accedere a questo tipo di informazione o più semplicemente perché il
dato potrebbe non essere stato inserito in quanto non obbligatorio in
fase di registrazione al social network.

In queste condizioni dunque non ci sarebbero problemi relativamente alla
creazione in Passweb della nuova anagrafica (dove l'indirizzo non
rappresenta effettivamente un dato obbligatorio). Nel momento in cui
però l'utente dovesse effettuare il suo primo ordine l'assenza di questo
indirizzo si farà sentire in quanto di fatto verrebbero a mancare sia
l'indirizzo di fatturazione che quello di spedizione, dati questi
obbligatori per poter andare avanti nel normale processo di checkout.
Per poter completare l'ordine l'utente dovrà quindi accedere al suo
profilo Passweb ed inserire i dati relativi all' indirizzo di
fatturazione e ad eventuali indirizzi di spedizione secondari.

**ATTENZIONE! Sulla base di quanto detto, nel momento in cui un utente
già registrato al sito ed in possesso dunque di un proprio account
Passweb dovesse, successivamente, effettuare l'autenticazione
utilizzando i dati del proprio profilo social, e l'indirizzo mail
prelevato dal social network non dovesse coincidere con quello presente
nell'anagrafica Passweb, verrà creata una nuova anagrafica utente.**

Allo stesso modo nel caso in cui uno stesso utente effettui, in un primo
momento, l'autenticazione al sito utilizzando uno dei suoi profili
social e, successivamente, effettui una registrazione direttamente sul
sito Passweb utilizzando un diverso indirizzo mail verrà ovviamente
creata una nuova anagrafica.

Nel caso in cui invece l'indirizzo mail prelevato dal profilo social
dovesse coincidere con quello dell'anagrafica Passweb, verrà agganciata
ed eventualmente integrata l'anagrafica utente già esistente.

Infine, un'ultima cosa da prendere in considerazione, è quella che
riguarda l'utilizzo contemporaneo del social login e l'attivazione
utenti mediante verifica mail.

In queste condizioni infatti nel momento in cui la registrazione al sito
dovesse avvenire tramite social l'utente verrà sempre considerato
attendibile e, conseguentemente, verrà attivato in maniera immediata.
Verrà comunque inviata, all'utente, la mail di registrazione (nello
specifico all'indirizzo ottenuto dal relativo social network); tale
mail, non conterrà però alcun link di attivazione account.

Inserendo il Componente all'interno del pannello di login verrà aperta
**la maschera di gestione e di configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_login_configurazione_res.bmp](./assets/media/image80.png){width="5.143055555555556in"
height="3.0909722222222222in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile definire
il contenuto e settare i principali parametri di configurazione del
componente stesso.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di impostare il nome del Componente che si sta
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

**Label (etichetta):** consente di impostare il testo del pulsante che
verrà utilizzato per consentire agli utenti del sito di effettuare
l'autenticazione tramite il proprio profilo social.

> **ATTENZIONE!** Nel momento in cui si dovesse decidere di utilizzare
> per questo pulsante una specifica immagine il testo della label non
> verrà visualizzato

**Social:** consente di impostare lo specifico social network da
utilizzare. Attualmente è possibile effettuare l'autenticazione al sito
Passweb utilizzando il proprio il proprio account:

- **Facebook**

- **Instagram**

- **Twitter**

- **Google**

- **LinkedIn**

- **PayPal**

- **Amazon**

oppure il proprio **Apple ID.**

**ATTENZIONE!** Nel caso in cui si voglia concedere agli utenti del sito
la possibilità di autenticarsi con ciascuno dei social network sopra
indicati sarà necessario inserire all'interno del pannello di login un
componente "Social Login" per ognuno di essi.

Nel momento in cui non dovesse essere correttamente configurata
l'integrazione tra il sito Passweb ed uno dei social network inseriti
all'interno del pannello di login, il componente visualizzerà un
apposito messaggio di errore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\social_login_configurazione2_res.bmp](./assets/media/image81.png){width="4.967361111111111in"
height="3.5131944444444443in"}

Per maggiori informazioni relativamente all'integrazione tra Passweb e i
social network al fine di consentire agli utenti del sito di effettuare
l'autenticazione con il proprio profilo si veda anche la sezione "*Sito
-- Preferenze -- Social Media*" di questo manuale

**Immagine sul link:** consente di impostare l'immagine da utilizzare
per il pulsante di accesso al sito mediante account social.

**Immagine Hover sul link:** consente di impostare l'immagine da
utilizzare al passaggio del mouse pulsante di accesso al sito mediante
account social

Il pulsante "**Applica impostazione Immagine alle altre Lingue**",
presente in corrispondenza di ciascuno dei campi sopra indicati,
consente di utilizzare automaticamente l'immagine indicata per tutte le
lingue attualmente gestite all'interno del sito

**Testo alternativo Immagine sul link:** consente di impostare il testo
del tooltip visualizzato al passaggio del mouse sul pulsante di accesso
mediante account social

