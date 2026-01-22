# COMPONENTE RUBRICA



Il Componente **"Rubrica"** consente di inserire all'interno del sito un
pannellino che l'utente potrà utilizzare, una volta effettuata
l'autenticazione, per gestire i propri indirizzi di spedizione.

Tale componente può essere inserito:

- all'interno della pagina "**Profilo Utente**" -- **obbligatorio per
  poter consentire il corretto funzionamento del sito**

- all'interno di pagine generiche (bianche) -- opzionale

![](./assets/media/image29.png)

**ATTENZIONE! Il componente "Rubrica" è accessibile soltanto dopo aver
effettuato l'autenticazione**

All'interno di questo pannello saranno quindi presenti due distinte
sezioni:

- **Pannello Rubrica:** consente di visualizzare gli indirizzi di
  spedizione già registrati

- **Form Inserimento \\ Modifica Indirizzo:** consente di modificare uno
  degli indirizzi registrati e/o di aggiungere un nuovo indirizzo di
  spedizione.

![](./assets/media/image30.png)

La gestione degli indirizzi di spedizione merce è leggermente diversa
dipendentemente dal fatto di considerare un sito collegato a Mexal
oppure ad uno dei gestionali Ho.Re.Ca.

**[ECOMMERCE MEXAL]{.underline}**

Per quel che riguarda i siti Ecommerce collegati a Mexal, **la gestione
degli indirizzi di spedizione merce è strettamente collegata con la
relativa tabella "Anagrafica Indirizzi di spedizione" presente
all'interno del gestionale.**

![](./assets/media/image31.png)

Nel caso in cui sia stato realizzato un form di registrazione utente in
cui vengono richieste informazioni quali indirizzo, CAP, località,
provincia e nazione, queste stesse informazioni oltre ad essere
memorizzate nei corrispondenti campi dell'Anagrafica Clienti/Fornitori
del gestionale verranno considerate anche come indirizzo di spedizione
primario dell'utente e verranno quindi inserite all'interno del
componente "Rubrica Indirizzi" non appena l'utente stesso avrà terminato
il processo di registrazione

In caso contrario il primo degli indirizzi inseriti in elenco verrà
considerato come indirizzo primario e le relative informazioni verranno
memorizzate nei corrispondenti campi dell'Anagrafica Clienti/Fornitori
del gestionale. I successivi indirizzi verranno invece inseriti
all'interno della tabella **Anagrafica Indirizzi di Spedizione** del
gestionale.

In merito agli indirizzi di spedizione memorizzati in Mexal sono gestiti
i seguenti campi:

- **Nominativo** -- campo opzionale

- **Indirizzo** -- campo obbligatorio

- **Città** -- campo obbligatorio

- **Cap** -- campo obbligatorio

- **Provincia** -- campo obbligatorio

- **Nazione** -- campo obbligatorio

- **Mail** -- campo opzionale

- **Telefono** -- campo opzionale

- **Fax** -- campo opzionale

- **Nota** -- campo opzionale

**ATTENZIONE!** Le corrispondenze tra i campi del componente "Rubrica
Indirizzi" e quelli della Tabella "Anagrafica Indirizzi di spedizione"
di Mexal **sono gestite in maniera completamente automatica da Passweb**

> **NOTA BENE:** le mail di notifica sui vari stati dell'ordine verranno
> inviate all'indirizzo mail indicato dall' utente in fase di
> registrazione al sito e, inoltre, anche all'indirizzo mail associato
> all'indirizzo di spedizione merce selezionato in fase di conferma
> ordine.

**[ECOMMERCE HO.RE.CA.]{.underline}**

A differenza di quanto appena visto per i siti Ecommerce collegati a
Mexal, nel caso di siti collegati ad uno dei gestionali Ho.Re.Ca. **gli
indirizzi di spedizione saranno gestiti, principalmente, all'interno di
Passweb** (non è infatti presente sul gestionale una tabella in cui
poter memorizzare questo tipo di informazioni)

In queste condizioni dunque, **nel caso in cui sia stato realizzato un
form di registrazione utente in cui vengono richieste informazioni quali
indirizzo, CAP, località, provincia e nazione**, queste stesse
informazioni verranno inserite nei relativi campi dell'anagrafica
clienti del gestionale e andranno a costituire quello che verrà
considerato come **indirizzo di spedizione principale**.

**Nel caso in cui invece i campi relativi all' indirizzo dell'utente non
siano stati inseriti nel form di registrazione** allora il **primo**
degli indirizzi inseriti all'interno del componente "Rubrica Indirizzi"
verrà considerato come **indirizzo di spedizione principale** e le
relative informazioni verranno memorizzate nei corrispondenti campi
dell'Anagrafica Clienti del gestionale. **I successivi indirizzi**
verranno invece considerati solo ed esclusivamente come possibili
**indirizzi di spedizione secondari** e saranno per questo memorizzati
sul database di Passweb.

**Lato gestionale, gli indirizzi di spedizione secondari, verranno
riportati solo ed esclusivamente nel piede dello specifico documento per
cui sono stati selezionati.**

**ATTENZIONE!** Dipendentemente dal fatto di aver selezionato in fase di
conferma ordine il proprio indirizzo di spedizione principale o uno
degli indirizzi di spedizione secondari, i riferimenti di questo
indirizzo potranno comparire o meno, all'interno del gestionale
Ho.Re.Ca., nel piede del corrispondente documento.

In particolare nel caso in cui i campi "**Destinatario**",
"**Indirizzo**", "**Città**", "**Cap**", "**Provincia**", presenti nel
piede del documento (sezione "Riferimenti trasporto")

non risultino essere valorizzati allora dovrà essere considerato come
indirizzo di spedizione merce l'indirizzo principale memorizzato
nell'anagrafica del cliente intestatario del documento stesso.

> **NOTA BENE:** se, in riferimento ad ordini provenienti da web, i
> campi evidenziati all'interno della figura sopra riportata sono vuoti,
> dovrà essere considerato come indirizzo di spedizione merce
> l'indirizzo presente all'interno dell'anagrafica del cliente
> intestatario del documento stesso.

Nel caso in cui invece in fase di conferma ordine si sia scelto un
indirizzo di spedizione secondario, come precedentemente evidenziato, i
riferimenti di questo indirizzo verranno inseriti negli appositi campi
presenti nel piede del documento Ho.Re.Ca. (quelli indicati all'interno
della figura sopra riportata).

Indipendentemente dalla tipologia di sito considerata, per modificare
uno degli indirizzi presenti in elenco è sufficiente cliccare sul
pulsante "**Modifica**" presente in corrispondenza dell'indirizzo
stesso.

Per aggiungere invece un nuovo indirizzo occorrerà cliccare sul pulsante
"**Aggiungi Nuovo Indirizzo**".

> **NOTA BENE:** un utente privo di indirizzi di spedizione non potrebbe
> in alcun modo portare a termine la conferma di un ordine. Il fatto
> quindi di richiedere all'interno del form di registrazione in maniera
> obbligatoria informazioni quali indirizzo, CAP, località, provincia
> e/o nazione permette di evitare agli utenti del sito blocchi
> imprevisti in fase di conferma dell'ordine.

**ATTENZIONE!** per poter garantire un corretto e normale funzionamento
del sito è necessario verificare di aver inserito il componente in esame
all'interno dell'omonima pagina "**Profilo Utente**". In caso contrario
infatti determinati automatismi potrebbero non funzionare in maniera
corretta pregiudicando agli utenti la possibilità di gestire i propri
indirizzi di spedizione.

