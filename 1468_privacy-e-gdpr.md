# PRIVACY E GDPR



Come indicato nei precedenti capitoli di questo manuale, dal punto di
vista del GDPR Telegram non è una vera e propria piattaforma di
Marketing e i messaggi gestiti in automatico da Passweb, vista la loro
tipologia, potranno essere inviati senza dover raccogliere nessun tipo
di consenso preventivo.

In ogni caso, trattandosi comunque di un servizio esterno con cui
potranno essere condivisi determinati dati è sempre bene verificare di
aver inserito all'interno del sito un'informativa adeguata circa
l'utilizzo del servizio in esame e dei dati che verranno effettivamente
condivisi con esso.

Inoltre se da una parte è vero che i messaggi di notifica stato ordine,
di carrelli abbandonati, di notifica messaggi in area riservata ...
possono effettivamente essere inviati senza richiedere esplicito
consenso è anche vero, dall'altra parte, che prima di poter
effettivamente ricevere questi messaggi l'utente deve esplicitamente
autorizzarne la ricezione (per maggiori informazioni in merito si veda
anche quanto indicato nel precedente capitolo di questo manuale)

Oltre a questo poi, sarà anche possibile gestire un'opzione di Opt Out
(esattamente come avviene per le integrazioni con piattaforme per la
gestione della messaggistica Whatsapp) che, se esercitata, metterà
l'utente nelle condizioni di non ricevere più nessun tipo di messaggio
automatico da parte del Bot del sito Ecommerce (posto ovviamente che
l'utente stesso potrebbe già fare in autonomia questa operazione
semplicemente scollegando il Bot Telegram dal suo account).

Per poter implementare questa opzione sarà sufficiente inserire nei form
di Registrazione e Profilo Utente un componente "**Campo Checkbox**"
mappato sul Campo Cliente "**Opt Out Telegram**" come in figura

![](./assets/media/image33.png)

![](./assets/media/image34.png)

In questo modo gli utenti che non avranno esercitato questa specifica
opzione, e che avranno ovviamente completato il processo di connessione
del loro account Telegram al Bot del sito, continueranno a ricevere i
messaggi impostati all'interno della corrispondente sezione del Wizard.

Una volta esercitata l'opzione invece, l'utente non riceverà più nessun
tipo di comunicazione dal Bot Telegram del sito indipendentemente da
quelli che potranno essere i messaggi effettivamente impostati lato
Wizard.

**ATTENZIONE! in ogni caso Passepartout non è in alcun modo responsabile
in merito all'utilizzo, in maniera conforme a quanto previsto dal GDPR,
di strumenti di terze parti, per cui il consiglio è sempre quello di
verificare direttamente con il relativo supporto piuttosto che con il
proprio DPO se la soluzione che si è scelto di adottare è o meno
conforme a quanto richiesto dalla normativa**
