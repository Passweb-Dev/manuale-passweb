# COME FUNZIONA



Il sistema di tracciamento utilizzato da Brainlead si sviluppa sia lato
client che lato server.

Nello specifico, il tracciamento lato client viene effettuato via
Javascript, in modo molto simile a quello che avviene anche con Google
Analytics, utilizzando lo snippet di codice, presente all'interno del
backoffice di Brainlead (sezione "**Web Visits**" -- campo "**Codice
HTML**")

![](./assets/media/image2.png)

e già inserito nativamente anche in Passweb, posto ovviamente di aver
attivato il relativo modulo.

**ATTENZIONE! Il tracciamento lato client prende in considerazione solo
ed esclusivamente la visita alle pagine del sito (pageview)** e richiede
la corretta impostazione dei parametri window.\_bl_cid e
window.\_bl_msid presenti alla pagina "**Sito -- Preferenze**" del
Wizard (tab "**Tracciamento Dati**")

![](./assets/media/image3.png)

In queste condizioni dunque, l'utente che si collega e naviga sul sito
verrà inserito in una sessione collegata a dei cookie e il codice di
tracciamento si preoccuperà di inviare a Brainlead informazioni relative
alle pagine visitate dall'utente durante quella specifica sessione di
navigazione.

Va da sé, ovviamente, che, come avviene anche per altri strumenti di
tracciamento (es. Google Analytics), nel momento in cui un utente
dovesse decidere di rifiutare i cookie o di disabilitare javascript
risulterà poi impossibile tracciarlo in maniera corretta.

Per quel che riguarda invece il tracciamento lato server, posto di aver
configurato correttamente l'integrazione tra le due piattaforme, e di
aver quindi settato in maniera adeguata i parametri presenti alla pagina
"**Sito -- Preferenze**" del Wizard (tab "**Tracciamento Dati**" sezione
"**Brainlead -- Marketing automation software**"), Passweb si
preoccuperà di inviare a Brainlead, mediante apposite chiamate API,
informazioni relative agli articoli aggiunti in carrello, alla creazione
di nuovi ordini e alla registrazione di nuovi utenti, eventi questi che
verranno visualizzati nella Timeline di Brainlead assieme alle pageview
e che consentiranno poi a Brainlead stesso, se opportunamente
configurato, di attivare determinate operazioni di marketing automation
come ad esempio quella relativa ai carrelli abbandonati.

![](./assets/media/image4.png)

**ATTENZIONE! il tracciamento lato server prevede l'invio a Brainlead
degli eventi di:**

- **Aggiunta / Rimozione articoli in carrello**

- **Conferma ordine**

- **Registrazione Utente**

e richiede la corretta impostazione del parametro "**Brainlead API
Key**" presente alla pagina "**Sito -- Preferenze**" del Wizard (tab
"**Tracciamento Dati**")

![](./assets/media/image5.png)

Un'ulteriore considerazione di fondamentale importanza da fare è quella
che riguarda poi l'effettiva visualizzazione dei dati inviati a
Brainlead. In questo senso infatti occorre sottolineare che il sistema
di tracciamento messo in piedi da Brainlead è volto principalmente a
gestire specifiche azioni di marketing automation e, in conseguenza di
ciò, **ogni evento tracciato all'interno del sito** (pageview, aggiunta
/ rimozione articoli in carrello e relativa creazione / aggiornamento
del carrello abbandonato, conclusione di un ordine) **dovrà
necessariamente essere legato su Brainlead ad uno specifico utente
dotato di un indirizzo mail valido** (oltre che di un numero di
cellulare nel momento in cui si dovesse decidere di attivare e gestire
su Brainlead anche il canale degli SMS).

In sostanza dunque, una volta settati correttamente i parametri di
configurazione che consentono di abilitare sia il tracciamento lato
client che quello lato server, collegando tra loro i diversi eventi, lo
snippet di codice di Brainlead si occuperà di gestire il tracciamento
delle Pageview e Passweb, dall'altra parte, si occuperà di inviare gli
eventi lato server.

**Tutto questo verrà però effettivamente visualizzato sulla Timeline di
Brainlead solo nel momento in cui questi eventi potranno essere
effettivamente associati ad uno specifico utente, e soltanto nel momento
in cui si sia verificato almeno uno degli eventi server tracciati** (va
da sé, ovviamente, che in tutto questo processo l'indirizzo mail
dell'utente è un dato assolutamente necessario).

