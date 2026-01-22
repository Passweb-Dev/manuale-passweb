# COMPONENTE REGISTRAZIONE UTENTE



Il Componente **"Registrazione Utente"** consente di definire il form di
registrazione che dovrà essere obbligatoriamente compilato dai
visitatori del sito prima di potersi autenticare e, conseguentemente,
prima di poter effettuare ordini.

Può essere inserito:

- all'interno dell'omonima pagina "**Registrazione Utente**" --
  **obbligatorio per poter consentire il corretto funzionamento del
  sito**

- all'interno di pagine generiche (bianche) -- opzionale

- all'interno del Componente "**Checkout Custom**" per realizzare il
  modulo di "**One Step Checkout**" -- opzionale

> Per maggiori informazioni in merito al modulo di "One Step Checkout" e
> a come poter configurare in tal senso il Componente "Checkout Custom"
> si veda anche il relativo capitolo di questo manuale (*"Varianti Sito
> Responsive -- Lista Componenti Ecommerce -- Componente Ordine
> Custom"*)

![](./assets/media/image19.png)

In genere, la registrazione di un nuovo utente mediante questo form non
determina la creazione immediata della relativa anagrafica cliente
all'interno del gestionale.

Tale anagrafica verrà infatti creata solo nel momento in cui il primo
ordine del nuovo cliente verrà inserito all'interno del gestionale (i
dati della nuova anagrafica saranno ovviamente quelli inseriti
dall'utente stesso all'interno del form di registrazione).

**ATTENZIONE!** Considerata la possibilità, per i siti Ecommerce Mexal,
di collegare più siti differenti (**fino ad un massimo di 9**) alla
stessa azienda, va anche considerato che possano poi essere create,
all'interno del gestionale, più anagrafiche distinte per lo stesso
cliente, nel momento in cui questo cliente dovesse registrarsi ed
effettuare ordini su due o più siti collegati alla stessa azienda Mexal.

Per maggiori informazioni in merito si veda anche la sezione
"*Configurazione gestionale -- Registrazione Utenti da web su più siti
collegati alla stessa azienda Mexal*" di questo manuale.

Una volta effettuata la registrazione, il form scomparirà, verrà inviata
una mail all'indirizzo indicato dall'utente con il riepilogo dei dati da
lui stesso inseriti, verrà effettuata l'autenticazione e l'utente stesso
potrebbe anche, dipendentemente dalla configurazione del form e/o dai
dati da lui inseriti, essere automaticamente ridiretto alla pagina
**"Profilo Utente"**, dove potrà , eventualmente, integrare i propri
dati oltre che indicare diversi possibili indirizzi di spedizione merce.

In particolare poi, relativamente alla possibilità, da parte dell'utente
di dichiarare direttamente in fase di registrazione più indirizzi
diversi (tipicamente un indirizzo di fatturazione e un diverso indirizzo
di spedizione) **va detto che Passweb consente di gestire all'interno
del form di registrazione fino a 4 diversi indirizzi**, il primo dei
quali verrà memorizzato nei corrispondenti campi dell'Anagrafica del
cliente sul gestionale e gli altri tre nei corrispondenti campi di tre
distinti indirizzi di spedizione memorizzati nella tabella Anagrafica
Indirizzi di Spedizione di Mexal.

**ATTENZIONE!** Nel caso in cui l'utente dovesse gestire 4 o più
indirizzi di spedizione differenti è necessario ricorre all'utilizzo del
componente "Rubrica Indirizzi".

Sulla base di quanto precedentemente detto potrebbe sembrare che il
Componente Registrazione Utente sia visibile solo ed esclusivamente
prima di aver effettuato il login.

In generale infatti una volta effettuata l'autenticazione al sito il
form di registrazione non sarà più visibile.

**Nel caso però in cui ad autenticarsi non sia un normale cliente ma
bensì un Agente (Ecommerce Mexal), il form di registrazione rimarrà
visibile anche dopo il login in modo tale da consentire all'Agente di
registrare nuovi clienti.**

Tali clienti all'atto della registrazione verranno automaticamente
associati all'Agente stesso, il quale potrà quindi, immediatamente,
effettuare per essi dei nuovi ordini (il nuovo nominativo comparirà
anche nella sezione "Business -- Clienti" dell'Area Riservata
dell'Agente).

Alla conferma del nuovo ordine e/o alla successiva sincronizzazione
questo verrà inserito nel gestionale assieme all'anagrafica del nuovo
utente, il quale avrà il relativo campo delle condizioni commerciali
automaticamente valorizzato con il codice conto dell' Agente che ha
effettuato per lui la registrazione al sito.

**ATTENZIONE!** per poter garantire un corretto e normale funzionamento
del sito è necessario verificare di aver inserito il componente in esame
all'interno dell'omonima pagina "**Registrazione Utente**". In caso
contrario infatti determinati automatismi potrebbero non funzionare in
maniera corretta pregiudicando agli utenti la possibilità di registrarsi
al sito.

Inoltre, ovviamente, nel caso in cui il Componente **"Registrazione
Utente"** non dovesse essere inserito all'interno del sito e /o non
dovesse essere gestito in maniera corretta gli unici utenti che
potrebbero effettuare ordini sarebbero i clienti già presenti sul
gestionale e correttamente esportati anche all'interno del sito.

