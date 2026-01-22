# PRENOTAZIONE DI UN TAVOLO VIA WEB



La procedura attraverso cui dovrà passare l'utente per confermare la
prenotazione di un tavolo all'interno del sito è composta da un unico
step all'interno del quale dovranno essere fornite diverse informazioni
a seconda delle impostazioni attivate in fase di configurazione del
relativo componente e/o direttamente all'interno del gestionale.

In generale, comunque, i dati che un utente potrebbe dover indicare per
completare la sua prenotazione saranno i seguenti

- **Data della prenotazione**

- **Orario della prenotazione**

- **Numero di coperti**

- **Sala**. L'eventuale selezione della sala dipende dalle impostazioni
  di configurazione del componente "Prenotazione"

- **Tavolo**. L'eventuale selezione dello specifico tavolo, per la sala
  indicata al punto precedente, dipende da come è stata configurata la
  sala stessa all'interno del gestionale.

Non appena l'utente effettuerà l'accesso alla pagina di prenotazione,
l'applicazione si connetterà automaticamente con il gestionale per
richiedere, in relazione al giorno corrente, i turni e gli orari in cui
poter effettuare la prenotazione.

![](./assets/media/image349.png)

Sarà comunque possibile, ovviamente, indicare una qualsiasi altra data
di prenotazione (successiva a quella odierna) selezionandola
dall'apposito calendario che verrà visualizzato cliccando all'interno
del campo Data.

Una volta selezionata la data verranno prelevate dal gestionale, in
tempo reale, le nuove informazioni relativamente agli orari e ai turni
in cui è possibile, per quella specifica data, effettuare una
prenotazione.

> **NOTA BENE:** nel caso in cui la data selezionata per la prenotazione
> corrisponda alla data di chiusura del ristorante verrà visualizzato un
> apposito messaggio di avviso personalizzabile all'interno della
> sezione "Test/Messaggi Sito" del Wizard.

![](./assets/media/image350.png)

Le date selezionabili per effettuare una prenotazione corrispondono a
quanto impostato all'interno del gestionale nella scheda "**Orari di
Apertura**" del menu "**Opzioni di installazione**".

![](./assets/media/image351.png)

Gli orari dei vari turni dipendono invece dalla configurazione a livello
gestionale del singolo turno.

![](./assets/media/image352.png)

Il campo "**Note**" visualizzato nel form di prenotazione,
immediatamente al di sotto del campo relativo al numero di Coperti,
potrà essere o meno visualizzato dipendentemente dalle impostazioni di
configurazione settate sul componente "Prenotazione" (parametro
"**Nascondi Nota**").

![](./assets/media/image353.png)

Eventuali note impostate all'interno di questo campo verranno poi
riportate all'interno del gestionale nell'omonimo campo del documento di
prenotazione.

Analogamente al campo "Note" anche la visualizzazione o meno del campo
relativo alla selezione della specifica sala dipenderà, innanzitutto,
dalle impostazioni di configurazione del componente "Prenotazione"
(parametro "**Nascondi Scelta Sala**").

Nel momento in cui si dovesse quindi decidere di dare all'utente la
possibilità di selezionare, in fase di prenotazione web, anche una
specifica sala, nel corrispondente menu a tendina verranno visualizzate
tutte quelle sale impostate all'interno del gestionale per essere
esportate e gestite anche sul sito.

![](./assets/media/image354.png)

Nello specifico per poter configurare, lato gestionale, una specifica
sala affinchè questa possa essere esportata e gestita anche all'interno
del sito sarà necessario per prima cosa configurare un apposito
"**Portale Passweb**".

Per far questo sarà necessario agire all'interno dell'apposita sezione
del gestionale ***"Utilità di sistema -- Portale Ristorante"***

![](./assets/media/image355.png)

dove andranno impostati i parametri di configurazione dello specifico
portale, le sale che dovranno poi essere esportate e gestite all'interno
del sito e, ovviamente, anche la specifica modalità con cui tali sale
dovranno essere gestite.

In particolare sarà quindi necessario impostare un valore per i seguenti
parametri:

**Portale:** consente di assegnare un nome allo specifico portale che si
sta configurando

**Attivo:** consente di attivare/disattivare lo specifico portale che si
sta configurando

**Sala:** all'interno di questa sezione andranno inserite,
selezionandole dall'apposito menu a tendina, tutte le sale che dovranno
poi essere gestite, nell'ambito di questo portale, all'interno del
corrispondente sito Passweb.

![](./assets/media/image356.png)

**Modalità:** consente di impostare la specifica modalità con cui le
sale inserite all'interno del portale dovranno poi essere gestite
all'interno del sito web.

![](./assets/media/image357.png)

E' possibile selezionare uno dei seguenti valori:

- **Richiesta di prenotazione da confermare**

- **Prenotazione confermata con scelta tavolo**

- **Scelta Tavolo + richiesta se non disponibile**

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> e/o alla configurazione di un portale all'interno del gestionale si
> rimanda allo specifico manuale.

Di seguito verranno analizzati i dettagli di ciascuna delle tre
possibili modalità di gestione delle sale all'interno del sito web

