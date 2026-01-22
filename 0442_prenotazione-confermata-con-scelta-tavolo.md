# PRENOTAZIONE CONFERMATA CON SCELTA TAVOLO



In queste condizioni la Sala in esame sarà correttamente esportata
all'interno del sito. L'utente **avrà quindi la possibilità di
selezionarla in fase di prenotazione web e, una volta selezionata, avrà
anche la possibilità di indicare lo specifico tavolo che intende
riservare.**

Dopo aver selezionato la Sala in esame, verrà infatti visualizzata
all'interno del sito, la piantina associata, nel gestionale, alla sala
stessa.

![](./assets/media/image360.png)

I Tavoli presenti all'interno della piantina rifletteranno esattamente
la stessa configurazione, a livello di dimensioni, forme e disposizione,
impostata all'interno del gestionale.

Per ogni singolo tavolo verrà visualizzato

- Il numero del tavolo

- Il numero di coperti minimi (necessari per poter abilitare il tavolo
  alla prenotazione via web)

- Il numero di coperti massimi

![](./assets/media/image361.png)

**Tali informazioni (numero del tavolo, coperti minimi e coperti
massimi) verranno prelevate, e dovranno quindi essere impostate,
necessariamente all'interno del gestionale.**

Nello specifico, per quel che riguarda il numero del tavolo ed i coperti
massimi, tali dati potranno essere inseriti direttamente in fase di
creazione del tavolo

![](./assets/media/image362.png)

Per quel che riguarda invece il numero di **coperti minimi** questo dato
dovrà essere impostato utilizzando il corrispondente parametro,
appositamente riservato a Passweb, presente nel "Dettaglio" della
configurazione dello specifico tavolo.

![](./assets/media/image363.png)

**Coperti minimi Passweb:** consente di definire per il tavolo in esame
un ben preciso numero di coperti minimi.

**Lato sito questo stesso tavolo potrà quindi essere selezionato in fase
di prenotazione solo ed esclusivamente nel momento in cui il numero di
coperti indicato dall'utente dovesse essere maggiore o uguale al numero
dei suoi coperti minimi.**

In relazione dunque a quelle che sono, nel momento in cui viene
effettuata la prenotazione, le effettive disponibilità all'interno del
gestionale, il numero di coperti indicati dall'utente e il numero di
coperti minimi impostati per ogni singolo tavolo, questi stessi tavoli
potranno essere o memo degli oggetti cliccabili che l'utente dovrà
quindi selezionare per poter completare la sua prenotazione.

In particolare occorre quindi sottolineare che all'interno della
piantina sopra indicata:

- I tavoli **disponibili**, e quindi selezionabili dall'utente in fase
  di prenotazione, verranno evidenziati in **verde**

- I tavoli **già prenotati,** e quindi non ulteriormente selezionabili,
  per la data e l'ora indicata verranno visualizzati in **rosso**

- I tavoli per i quali è stato impostato, lato gestionale, **un numero
  di coperti minimo superiore al numero di coperti indicato dall'utente
  in fase di prenotazione web,** verranno visualizzati in **grigio.**

> **NOTA BENE:** i colori sopra indicati ed utilizzati per distinguere,
> nelle diverse situazioni, i tavoli prenotabili da quelli non
> prenotabili, sono colori di default che possono essere modificati
> secondo le specifiche esigenze dell'utente , operando per questo
> attraverso gli appositi elementi dello style editor.

Analogamente ai tavoli evidenziati in rosso anche quelli evidenziati in
grigio non potranno essere selezionati.

> **NOTA BENE:** nel caso in cui l'utente modifichi, prima della
> conferma, la data, l'ora o il numero di coperti per la sua
> prenotazione, la piantina della sala verrà ricaricata e ridisegnata in
> base alle nuove impostazioni.

**In queste condizioni, infine, l'utente potrà confermare la propria
prenotazione solo ed esclusivamente nel caso in cui la somma del numero
di coperti dei tavoli selezionati risulti essere maggiore o uguale al
numero di coperti indicato dall'utente nella sua prenotazione.**

L'utente ha infatti la possibilità di selezionare, tra quelli
disponibili, uno o più tavoli contemporaneamente. Mano a mano che dei
tavoli vengono selezionati, quelli restanti verranno eventualmente
ricolorati in grigio, in relazione ovviamente ai coperti restanti da
prenotare e a quello che è il loro numero di coperti minimi.

Supponendo dunque di voler effettuare una prenotazione per 7 coperti,
nel momento in cui venisse selezionato un tavolo da 4, restando ancora 3
posti da coprire, automaticamente tutti i tavoli liberi con coperti
minimi maggiori o uguali a 4 verrebbero colorati in grigio e non
sarebbero più selezionabili.

Nel momento in cui le condizioni per confermare la prenotazione non
dovessero essere soddisfatte, perché il numero di coperti dei tavoli
selezionati non è maggiore o uguale al numero di coperti indicato per la
prenotazione, o perché per la data e l'orario selezionato non risultano
esserci dei tavoli disponibili, tentando comunque di effettuare la
prenotazione, l'utente verrebbe bloccato e gli verrebbe visualizzato un
apposito messaggio per informarlo del perché la sua prenotazione non può
andare a buon fine:

![](./assets/media/image364.png)

Se le condizioni per poter effettuare la prenotazione dovessero invece
essere pienamente soddisfatte, dopo aver selezionato anche il tavolo o i
tavoli desiderati cliccando sul pulsante "**Procedi**" l'utente verrà
immediatamente ricondotto alla pagina di riepilogo per la conferma della
sua prenotazione

![](./assets/media/image358.png)

I dati della prenotazione saranno inserito all'interno di una griglia
responsiva le cui colonne possono essere definite direttamente
all'interno della sezione "**Gestione Contenuti**" presente nella
maschera di gestione e configurazione del Componente Prenotazione Tavolo
Custom.

Cliccando sul pulsante **"Conferma"** la prenotazione verrà inserita
immediatamente all'interno del gestionale, dove verrà memorizzata nello
stato di "**CONFERMATA**"

> **NOTA BENE:** sono gestiti eventuali casi di **over booking** per cui
> se, tra il momento in cui l'utente seleziona il tavolo desiderato e
> quello in cui clicca sul pulsante "Procedi" per confermare la sua
> prenotazione, contemporaneamente lo stesso tavolo venisse occupato da
> altre prenotazioni (effettuate via web o direttamente all'interno del
> gestionale), l'utente verrebbe avvisato con un apposito messaggio e la
> sua prenotazione verrebbe bloccata.

![](./assets/media/image365.png)

