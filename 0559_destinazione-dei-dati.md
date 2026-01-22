# DESTINAZIONE DEI DATI



Come già evidenziato nel precedente capitolo di questo manuale il
componente "Campo di Testo" può essere mappato con diversi campi dell'
anagrafica cliente gestionale oppure con attributi utente Passweb
appositamente creati.

In questo senso per definire il campo in cui verranno poi memorizzati i
dati inseriti dall'utente in fase di registrazione e/o di variazione del
proprio profilo, sarà necessario agire mediante il parametro "**Tipo di
dato di Destinazione**" presente, come visto, tra i parametri di
configurazione del componente "Campo di Testo" decidendo, per prima
cosa, se il dato dovrà essere memorizzato in un campo dell'anagrafica
gestionale (opzione **Campo Cliente**) oppure in un attributo Passweb
(opzione **Attributo Cliente**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_testo_destinazione_dati.bmp](./assets/media/image84.png){width="4.649305555555555in"
height="2.9611111111111112in"}

Nel momento in cui l'esigenza dovesse essere quella di memorizzare il
dato in un campo dell'anagrafica gestionale sarà quindi necessario
impostare il parametro in questione sul valore "**Campo Cliente**" e
selezionare poi come destinazione uno dei seguenti campi:

**[USERNAME]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo utilizzato all'interno del gestionale per memorizzare la login
di accesso al sito

**Inserendo questo campo all'interno del form, l'utente avrà quindi la
possibilità, in fase di registrazione, di impostare la propria login di
accesso.**

Considerando quanto appena detto è abbastanza semplice comprendere come
**sia obbligatorio** inserire all'interno del form di registrazione un
Componente "Campo di Testo" che corrisponda al campo "Username".

Chiaramente oltre ad un Componente di questo tipo sarà poi necessario
inserire all'interno del form di registrazione anche un Componente di
tipo "Campo Password" in modo tale da consentire all'utente di poter
impostare anche la propria password di accesso al sito

**ATTENZIONE!** al fine di garantire il corretto funzionamento del sito,
permettendo la registrazione di nuovi clienti (siti B2C), è obbligatorio
inserire all'interno del form di registrazione un componente" Campo di
Testo" corrispondente al campo "Login: Utente" e un Componente "Campo
Password". Nel caso di siti B2B con accesso al sito solo da parte degli
Agenti è invece possibile realizzare anche form di registrazione privi
di questi campi.

**[INDIRIZZO E-MAIL]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "E-mail" dell'Anagrafica Clienti/Fornitori del gestionale.

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio indirizzo
mail**.

**ATTENZIONE!** non è possibile effettuare due registrazioni diverse
utilizzando lo stesso indirizzo mail.

In queste condizioni inoltre è consigliato impostare il campo **"Tipo
Valore"** precedentemente esaminato su **"Mail"** in modo tale da poter
attivare un apposito controllo per verificare la corretta sintassi
dell'indirizzo mail inserito dall'utente stesso in fase di
registrazione.

Passweb gestisce, infine, tutta una serie di E-Mail connesse ai vari
stati dell'ordine e che verranno inviate in automatico, dal sistema
all'indirizzo indicato dal cliente stesso in fase di registrazione. In
questo modo il cliente potrà essere avvisato via mail relativamente a
quello che è lo stato dei suoi ordini**. E' abbastanza semplice
comprendere quindi che non inserendo questo campo all'interno del form
di registrazione, non ci sarà poi la possibilità da parte di Passweb di
notificare al cliente via mail quello che è lo stato dei sui ordini.**

**ATTENZIONE:** è fortemente consigliato inserire questo tipo di campo
all'interno del form di registrazione impostandolo inoltre come un campo
obbligatorio.

**[MAIL INDIRIZZO 2 /3/4]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Email**" di un ben preciso indirizzo di spedizione merce
dell'utente.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 3 indirizzi Email aggiuntivi (oltre a quello
dell'anagrafica utente) che verranno poi memorizzati nei relativi
indirizzi di spedizione.

**[CONFERMA INDIRIZZO E-MAIL]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" verrà
utilizzato come campo per la conferma dell'indirizzo mail, validando
quindi quanto inserito all'interno di un altro Campo di Testo (che dovrà
ovviamente essere presente all'interno dello stesso form) mappato per
gestire l'Email utente.

**Nel momento in cui si dovesse decidere di inserire questo campo
all'interno del form, la registrazione potrà poi avvenire solo ed
esclusivamente nel caso in cui l'indirizzo inserito nel campo Email
coincida esattamene con quello inserito nel campo di Conferma Email**

**[PEC]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Indirizzo PEC**" dell'Anagrafica Clienti/Fornitori del
gestionale.

Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio indirizzo
di posta certificata.

In queste condizioni inoltre è consigliato impostare il campo "Tipo
Valore" precedentemente esaminato su "Mail" in modo tale da poter
attivare un apposito controllo per verificare la corretta sintassi
dell'indirizzo mail inserito dall'utente stesso in fase di
registrazione.

**[NOME]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Nome**" dell'Anagrafica Clienti/Fornitori del gestionale

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio Nome**.

Questo tipo di campo verrà visualizzato all'interno del form unicamente
nel caso in cui ad effettuare la registrazione sia un utente di tipo
Privato (Persona Fisica).

**[COGNOME]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Cognome**" dell'Anagrafica Clienti/Fornitori del gestionale

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio
Cognome**.

Questo tipo di campo verrà visualizzato all'interno del form unicamente
nel caso in cui ad effettuare la registrazione sia un utente di tipo
Privato (Persona Fisica).

**[CODICE FISCALE]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Cod.Fiscale**" dell'Anagrafica Clienti/Fornitori del
gestionale

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio Codice
Fiscale**.

In relazione al campo in esame ci sono poi alcune cose di fondamentale
importanza di cui è sempre bene tener conto. Nello specifico occorre
ricordare che:

- Lato front end il campo in esame verrà visualizzato solo nel caso in
  cui ad effettuare la registrazione sia un utente di tipo Privato
  (Persona Fisica).

- Il valore inserito all'interno di questo campo potrebbe essere
  utilizzato come chiave di ricerca della relativa anagrafica
  all'interno del database di CRIBS e, conseguentemente, per compilare
  in maniera automatica determinati campi del form di registrazione
  utente sfruttando l'integrazione tra Passweb stesso e CRIBIS.

> Per utilizzare tale funzionalità sarà necessario:

- Aver attivato il relativo modulo (Arricchimento Anagrafiche)
  nell'installazione Mexal collegata al sito

- Selezionare il parametro "**Abilita autocompletamento campi CRIBIS**"
  presente nella maschera di configurazione del componente "Campo di
  Testo" nel momento in cui dovesse appunto essere mappato sul Codice
  Fiscale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_cribis_2.bmp](./assets/media/image85.png){width="4.785416666666666in"
height="3.0652777777777778in"}

> **ATTENZIONE!** La funzione di autocompletamento dei campi del form di
> registrazione è disponibile solo per utenti di tipo Agente
>
> Per maggiori informazioni in merito all'integrazione Passweb -- CRIBS
> si veda anche quanto indicato nel successivo capitolo "*Integrazione
> CRIBIS*" di questo manuale

- **Relativamente ai siti** **collegati ad uno dei gestionali
  Ho.Re.Ca.** il campo "Codice Fiscale" è, di base, uno dei tre dati
  obbligatori da utilizzare in fase di registrazione affinché l'utente
  possa essere correttamente inserito all'interno del relativo
  gestionale (gli altri due campi obbligatori sono Nome / Cognome /
  Ragione Sociale e Partita IVA)

> **Nel caso in cui l'esigenza dovesse essere quella di semplificare il
> form di registrazione utente, è possibile decidere di non inserire
> all'interno del form web il campo relativo al codice fiscale.**
>
> In queste condizioni per poter garantire l'univocità delle anagrafiche
> utente e il loro corretto inserimento all'interno del gestionale, il
> campo codice fiscale (**che rimane comunque, per il gestionale, un
> campo obbligatorio**) verrà valorizzato con un valore fittizio
> (stringa alfanumerica univoca iniziante per PWB) in maniera tale da
> evitare eventuali sovrascritture in caso di utenti privati che
> dovessero avere lo stesso nome e lo stesso cognome
>
> Lato Wizard, inoltre, verrà anche visualizzato un apposito messaggio
> informativo per ricordare all'amministratore quanto appena
> evidenziato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_codice_fiscale.bmp](./assets/media/image86.png){width="5.065277777777778in"
height="2.9090277777777778in"}

> **ATTENZIONE!** Nel caso in cui all'interno del gestionale siano
> presenti anagrafiche utente con stesso nome e stesso cognome è
> necessario verificare che per tali anagrafiche il campo relativo al
> codice fiscale sia stato correttamente valorizzato con un dato
> univoco.
>
> In caso contrario, nel momento in cui tali utenti dovessero essere
> esportati e gestiti all'interno del sito, venendo meno l'univocità dei
> dati necessari per individuare un' anagrafica utente, si potrebbe
> correre il rischio che eventuali variazioni al profilo web dell'utente
> vengano poi inserite, lato gestionale, nell'anagrafica sbagliata.

**[DENOMINAZIONE (SOLO ECOMMERCE MEXAL)]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Denominazione**" dell'Anagrafica Clienti/Fornitori del
gestionale.

**Tipicamente questo campo viene utilizzato per gestire la Ragione
Sociale del cliente che opera in forma di ditta individuale**.

In conseguenza di ciò il campo in esame verrà visualizzato all'interno
del form di Registrazione / Profilo solo per utenti di tipo Privato
(Persona Fisica) esattamente come i campi Nome e Cognome.

**ATTENZIONE!** Nel momento in cui si dovesse decidere di gestire il
campo "Denominazione" occorre prestare particolare attenzione al fatto
di inserirlo in tutti i form del sito relativi ai dati dell'utente
quindi nel form di Registrazione, nel form del Profilo Utente e, nel
caso in cui si dovesse decidere di gestire il One Step Checkout anche
nel form di Registrazione presente all'interno di questo stesso
componente.

Nel caso in cui si dovesse infatti inserire il campo Denominazione
all'interno del form di Registrazione al sito ma, ad esempio, non in
quello del One Step Checkout (o viceversa) in fase di conferma ordine la
tipologia dell'utente potrebbe cambiare.

**[CODICE LOTTERIA]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Codice lotteria**" dell'Anagrafica Clienti/Fornitori del
gestionale.

**Questo campo viene utilizzato per gestire il codice utente relativo
alla lotteria degli scontrini elettronici che entrerà in vigore a
partire dall\'1/1/2021**.

**ATTENZIONE!** Prima di attivare il campo verificare con il proprio
commercialista che gli acquisti effettuati mediante ecommerce rientrino
effettivamente nell'ambito della lotteria degli scontrini elettronici.

Considerata la finalità del campo in esame questo verrà effettivamente
visualizzato all'interno del form di Registrazione / Profilo solo per
utenti di tipo Privato (Persona Fisica) esattamente come i campi Nome e
Cognome.

**ATTENZIONE!** Nel momento in cui si dovesse gestire anche la
registrazione al sito da parte di utenti stranieri è importante
impostare il campo in esame come visibile ai soli utenti Italiani (gli
unici che possono effettivamente partecipare alla lotteria degli
scontrini)

**Inoltre occorre anche considerare che il codice lotteria deve essere
un codice alfanumerico di 8 caratteri**.

Nel momento in cui si dovesse decidere di gestirlo sarà necessario,
quindi, impostare correttamente anche tutti i controlli di validità
sulla lunghezza minima (8 caratteri) e massima (8 caratteri) del campo
in esame in modo tale da non avere poi errori in fase di
sincronizzazione con il gestionale

Per maggiori informazioni relativamente a come poter impostare
condizione di visibilità, e controlli sulla tipologia e sulla lunghezza
del campo, si veda anche quanto indicato nel precedente capitolo di
questo manuale

**[RAGIONE SOCIALE]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Rag. Sociale**" dell'Anagrafica Clienti/Fornitori del
gestionale

Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, la Ragione Sociale
della propria azienda.

**Questo tipo di campo verrà visualizzato all'interno del form
unicamente nel caso in cui ad effettuare la registrazione sia un utente
di tipo Azienda**.

**[PARTITA IVA]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Partita Iva**" dell'Anagrafica Clienti/Fornitori del
gestionale.

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, la partita iva della
propria azienda**.

In relazione al campo in esame ci sono poi alcune cose di fondamentale
importanza di cui è sempre bene tener conto. Nello specifico occorre
ricordare che:

- Lato front end il campo in esame verrà visualizzato solo nel caso in
  cui ad effettuare la registrazione sia un utente di tipo Azienda.

- Il valore inserito all'interno di questo campo potrebbe essere
  utilizzato come chiave di ricerca della relativa anagrafica
  all'interno del database di CRIBS e, conseguentemente, per compilare
  in maniera automatica determinati campi del form di registrazione
  utente sfruttando l'integrazione tra Passweb stesso e CRIBIS.

> Per utilizzare tale funzionalità sarà necessario:

- Aver attivato il relativo modulo (Arricchimento Anagrafiche)
  nell'installazione Mexal collegata al sito

- Selezionare il parametro "**Abilita autocompletamento campi CRIBIS**"
  presente nella maschera di configurazione del componente "Campo di
  Testo" nel momento in cui dovesse appunto essere mappato sulla Partita
  IVA

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_cribis_1.bmp](./assets/media/image87.png){width="4.792361111111111in"
height="3.0520833333333335in"}

> **ATTENZIONE!** La funzione di autocompletamento dei campi del form di
> registrazione è disponibile solo per utenti di tipo Agente
>
> Per maggiori informazioni in merito all'integrazione Passweb -- CRIBS
> si veda anche quanto indicato nel successivo capitolo "*Integrazione
> CRIBIS*" di questo manuale

**[CODICE DESTINATARIO SDI]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Codice Destinatario SDI**" dell'Anagrafica Clienti/Fornitori
del gestionale

Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il codice SDI della
propria azienda, utile ai fini della corretta emissione della fattura
elettronica.

**ATTENZIONE!** Allo stato attuale il codice SDI è richiesto ai fini
dell'emissione della fattura elettronica **alle sole aziende italiane**.

In considerazione di ciò sarà quindi necessario prestare particolare
attenzione al fatto di aver impostato per questo stesso campo anche una
Condizione di visibilità tale per cui il dato venga effettivamente
richiesto solo per utenti di tipo "Azienda" e sole se l'utente dovesse
selezionare come sua nazione d'appartenenza l'Italia.

**ATTENZIONE!** Prima di inserire il campo SDI nel form di "Profilo
Utente" è opportuno effettuare una sincronizzazione totale in modo da
poter aggiornare correttamente il database di Passweb con il valore
effettivamente presente sul gestionale, nelle anagrafiche dei vari
utenti, per questo campo.

In ogni caso la sovrascrittura dello SDI sul gestionale avverrà solo nel
momento in cui il corrispondente campo venga effettivamente valorizzato
sul sito. Pertanto se il campo SDI, nel form di Profilo Utente, dovesse
essere lasciato vuoto e l'utente dovesse comunque aver variato e salvato
il suo Profilo, il valore di questo campo non verrà passato al
gestionale dove continuerà quindi ad avere il valore corretto.

**[CODICE UFFICIO PA]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Codice Univoco Ufficio PA**" dell'Anagrafica
Clienti/Fornitori del gestionale, dato questo obbligatorio per utenti
che dichiarino di essere una pubblica amministrazione.

Nel momento in cui l'esigenza dovesse quindi essere quella di consentire
la registrazione al sito anche a enti pubblici sarà necessario
accertarsi di aver correttamente inserito nel form di registrazione:

- Un componente "**Campo Radio**" configurato con i parametri "**Tipo
  Valore = Scelta**" e "**Campo di destinazione = Ente Pubblico**" .

- Un componente "**Campo di Testo**" mappato sul campo cliente **"Codice
  Ufficio PA**"

**ATTENZIONE!** Come per il "Codice destinatario SDI" anche il "Codice
Ufficio PA" è richiesto, ai fini della fatturazione elettronica, solo ad
aziende italiane che dichiarino di essere delle pubbliche
amministrazioni.

In considerazione di ciò sarà quindi necessario prestare particolare
attenzione al fatto di aver impostato per questo stesso campo anche una
Condizione di visibilità tale per cui il dato venga effettivamente
richiesto solo per utenti di tipo "Azienda", che hanno dichiarato di
essere delle pubbliche amministrazione e che hanno selezionato come loro
nazione d'appartenenza l'Italia.

**[TELEFONO/TELEFONO INDIRIZZO N.2/TELEFONO INDIRIZZO N.3/TELEFONO
INDIRIZZO N.4]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Telefono**" dell'Anagrafica Clienti/Fornitori del gestionale
oppure, all' analogo campo di un ben preciso indirizzo di spedizione
merce.

Nello specifico, **il Telefono con il numero d'ordine più basso presente
nel form di registrazione corrisponderà con il campo Telefono
dell'Anagrafica Clienti/Fornitori del gestionale, tutti gli atri
corrisponderanno invece con l'analogo campo di un diverso indirizzo di
spedizione merce**.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 4 Numeri di Telefono differenti, uno dei quali finirà
nell'anagrafica dell' utente e gli altri tre in tre distinti indirizzi
di spedizione.

**[FAX/FAX INDIRIZZO N.2/ FAX INDIRIZZO N.3/ FAX INDIRIZZO
N.4]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà
al campo "**Fax**" dell'Anagrafica Clienti/Fornitori del gestionale
oppure, all' analogo campo di un ben preciso indirizzo di spedizione
merce.

Nello specifico, **il Fax con il numero d'ordine più basso presente nel
form di registrazione corrisponderà con il campo Fax dell'Anagrafica
Clienti/Fornitori del gestionale, tutti gli atri corrisponderanno invece
con l'analogo campo di un diverso indirizzo di spedizione merce**.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 4 Numeri di Fax differenti, uno dei quali finirà
nell'anagrafica dell' utente e gli altri tre in tre distinti indirizzi
di spedizione.

**[LUOGO DI NASCITA]{.underline}**

Selezionando questo valore il Componente "Campo di Testo" corrisponderà,
nel caso di siti Ecommerce collegati a Mexal al campo "**Comune/Stato
estero nas**" dell'Anagrafica Clienti/Fornitori, nel caso invece di siti
collegati ad uno dei gestionali Ho.Re.Ca. al campo "**Luogo"** presente,
anch'esso nella corrispondente Anagrafica Clienti/Fornitori.

**Inserendo questo campo all'interno del form l'utente avrà quindi la
possibilità di impostare, in fase di registrazione, il proprio comune di
nascita**.

Questo tipo di campo verrà visualizzato all'interno del form unicamente
nel caso in cui ad effettuare la registrazione sia un utente di tipo
Privato.

**[INDIRIZZO/INDIRIZZO N.2/INDIRIZZO N.3/INDIRIZZO N.4]{.underline}**

Selezionando uno di questi valori il componente "Campo di Testo"
corrisponderà al campo "**Indirizzo**" dell'Anagrafica Clienti/Fornitori
del gestionale oppure, all' analogo campo di un ben preciso indirizzo di
spedizione merce.

Nello specifico, **l'indirizzo con il numero d'ordine più basso presente
nel form di registrazione corrisponderà con il campo Indirizzo
dell'Anagrafica Clienti/Fornitori del gestionale, tutti gli atri
corrisponderanno invece con l'analogo campo di un diverso indirizzo di
spedizione merce**.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 4 campi Indirizzo differenti, uno dei quali finirà
nell'anagrafica del utente e gli altri tre in tre distinti indirizzi di
spedizione.

**[CAP/CAP n.2/CAP n.3/CAP n.4]{.underline}**

Selezionando uno di questi valori il Componente "Campo di Testo"
corrisponderà al campo "**CAP**" dell'Anagrafica Clienti/Fornitori del
gestionale o all' analogo campo di un ben preciso indirizzo di
spedizione.

Nello specifico, **il CAP con il numero d'ordine più basso presente nel
form di registrazione corrisponderà con il campo CAP dell'Anagrafica
Clienti/Fornitori del gestionale, tutti gli atri corrisponderanno invece
con l'analogo campo di un diverso indirizzo di spedizione merce**.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 4 campi CAP differenti, uno dei quali finirà
nell'anagrafica del utente e gli altri tre in tre distinti indirizzi di
spedizione.

**[ATTENZIONE!]{.underline}**

Sono gestiti dall'applicazione appositi controlli atti a validare il
corretto formato del CAP inserito dall'utente in relazione al paese da
lui stesso selezionato all'interno form di registrazione.

Nello specifico un primo controllo di validazione sul formato del CAP è
gestito, lato client, sulla base sull'attributo "pattern" di HTML5. In
relazione a tale controllo la visualizzazione del messaggio di errore
può variare a seconda del browser utilizzato.

Considerando inoltre che questo tipo di validazione potrebbe non
funzionare correttamente nei browser più datati, lo stesso controllo di
validazione viene applicato anche lato server.

**[LOCALITÀ/LOCALITÀ N.2/LOCALITÀ N.3/LOCALITÀ N.4]{.underline}**

Selezionando uno di questi valori il Componente "Campo di Testo"
corrisponderà al campo "**Località**" dell'Anagrafica Clienti/Fornitori
del gestionale o all' analogo campo di un ben preciso indirizzo di
spedizione.

Nello specifico, il campo **Località con il numero d'ordine più basso
presente nel form di registrazione corrisponderà al campo Località
dell'Anagrafica Clienti/Fornitori del gestionale, tutti gli atri
corrisponderanno invece all'analogo campo di un diverso indirizzo di
spedizione merce**.

In definitiva dunque, è possibile gestire nel form di registrazione
utente fino a 4 campi Località differenti, uno dei quali finirà
nell'anagrafica del utente e gli altri tre in tre distinti indirizzi di
spedizione.

In queste condizioni, inoltre, nella maschera di configurazione del
componente verrà visualizzato anche il parametro "**Abilita Validazione
Google**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\validazione_citta_2.bmp](./assets/media/image88.png){width="4.785416666666666in"
height="3.045138888888889in"}

**Abilita Validazione Google**: consente, se selezionato, di attivare la
validazione di quanto inserito all'interno del campo in esame mediante i
servizi offerti da Google Maps.

**ATTENZIONE! per ovvie ragioni, questo tipo di validazione potrà
avvenire in maniera corretta solo nel caso in cui il sito possa
utilizzare effettivamente i servizi della Google Maps**.

Nello specifico, considerando che la funzione di validazione offerta da
Google Maps accetta API Key con restrizione a livello di indirizzo IP
(ma non a livello di Referrer), affinché la validazione del dato
inserito all'interno del campo in esame possa avvenire in maniera
corretta è necessario verificare di aver inserito all'interno del campo
"**Chiave Google Maps Distance API**" (pagina "**Preferenze Sito**", tab
"**Integrazioni**" del Wizard) una API key valida e funzionante.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\validazione_citta.bmp](./assets/media/image33.png){width="5.759722222222222in"
height="3.3444444444444446in"}

Per maggiori informazioni in merito all'utilizzo della Google Maps e dei
relativi servizi si consiglia di fare riferimento anche a quanto
indicato all'interno del capitolo "*Sito -- Preferenze -- Integrazioni
-- Google Maps API*" di questo manuale

Supponendo dunque di aver configurato ed impostato tutto in maniera
corretta, andando poi a compilare sul front end del sito il campo in
questione con l'indicazione di una specifica Località, alla conferma dei
dati verrà effettuata una chiamata ad un'apposita API di Google cui
verrà passato l'indirizzo (completo eventualmente di Via, Città,
Provincia, CAP e Nazione) inserito dall'utente. L'API oltre a restituire
le coordinate geografiche relative a latitudine e longitudine,
restituirà anche i valori esatti dell'indirizzo corrispondente.

Nel momento in cui il valore ritornato da Google **relativamente al
campo "Località"** dovesse coincidere esattamente con quello inserito
dall'utente in fase di compilazione del form, la validazione avverrà con
successo, e l'indirizzo verrà effettivamente salvato.

In caso contrario invece, i dati inseriti dall'utente non verranno
salvati, verrà mostrato, in corrispondenza del campo in questione, un
apposito messaggio di errore (modificabile alla sezione "Testi/Messaggi
del Sito" agendo per il componente "Registrazione Utente" sul campo
"**Errore Validazione Google**") e all'interno di questo stesso campo
verrà inserito automaticamente il valore della Città ritornato da
Google.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\validazione_citta_3.bmp](./assets/media/image89.png){width="5.363888888888889in"
height="3.3444444444444446in"}

**ATTENZIONE!** L'unico campo ad essere validato ed eventualmente
valorizzato con quanto ritornato da Google è il campo "Città". **Non
verranno quindi corretti in automatico dati quali la Via, il CAP, la
Nazione o la Provincia**

**[NOMINATIVO INDIRIZZO N.2/ NOMINATIVO INDIRIZZO N.3/ NOMINATIVO
INDIRIZZO N.4]{.underline}**

Selezionando uno di questi valori il Componente "Campo di Testo"
corrisponderà al campo "**Riferimento**" del relativo indirizzo di
spedizione (utile nel momento in cui si voglia utilizzare un indirizzo
di spedizione diverso da quello di fatturazione dovendo anche indicare,
oltre all'indirizzo, un riferimento della persona a cui consegnare la
merce).

**[ATTRIBUTI UTENTE]{.underline}**

Nel caso in cui l'esigenza dovesse invece essere quella di memorizzare
il dato in un Attributo Utente sarà necessario impostare il parametro in
questione sul valore "**Attributo Cliente**" e selezionare poi dal
sottostante menu a tendina ("**Campo di Destinazione**") uno degli
attributi cliente (siano essi attributi di tipo Mexal o di tipo Passweb)
precedentemente codificati all'interno della corrispondente sezione del
Wizard.

**ATTENZIONE!** in relazione ad attributi cliente di tipo Mexal, sarà
inoltre necessario prestare particolare attenzione al fatto che il dato
che l'utente potrà poi andare ad inserire sul front end del sito, sia
compatibile con il tipo di dato effettivamente accettato dal campo Mexal
su cui è stato mappato l'attributo in esame.

Se ad esempio l'attributo selezionato dovesse essere stato mappato su di
un campo Mexal (di una Videata Aggiuntiva Clienti / Fornitori o di
un'Anagrafica MyDB) numerico di 4 caratteri, il componente "Campo di
Testo" dovrebbe essere configurato in maniera tale che possa accettare
solo numeri con un valore massimo pari a 9999

**NOTA BENE**: per maggiori informazioni relativamente a come creare in
Passweb Attributi Cliente si rimanda al relativo capitolo di questo
manuale ("Utenti -- Gestione Parametri Utenti E-Commerce -- Gestione
Attributi".)

