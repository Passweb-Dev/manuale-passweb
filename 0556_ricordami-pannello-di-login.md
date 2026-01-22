# RICORDAMI (PANNELLO DI LOGIN)



Il Componente **"Ricordami"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_ricordami_login_res.bmp](./assets/media/image76.png){width="2.5388888888888888in"
height="2.5388888888888888in"}

consente di inserire all'interno del pannello di login un check box che,
se selezionato, permetterà di generare un cookie che verrà poi
utilizzato per consentire all'utente di effettuare automaticamente il
login senza dover reinserire le proprie credenziali in maniera manuale.

> **NOTA BENE:** affinchè il componente Ricordami possa funzionare in
> maniera corretta è necessario che il browser utilizzato dall'utente
> che visita il sito abbia la gestione dei cookie attiva.

In questo modo dunque, nel momento in cui l'utente dovesse tornare a
visitare la pagina di login del sito, **utilizzando ovviamente lo stesso
browser web**, verrà automaticamente autenticato senza dover reinserire
le proprie credenziali di accesso.

> **NOTA BENE:** per poter effettuare il login automatico sarà
> sufficiente visitare una pagina del sito contenente il "Pannello di
> Login" con il relativo check "Ricordami".

Inserendo questo Componente all'interno del pannello di login verrà
aperta **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricordami_configurazione_res.bmp](./assets/media/image77.png){width="4.590972222222222in"
height="2.415277777777778in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

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

**Label (etichetta):** consente di impostare l'etichetta visualizzata in
corrispondenza del check box che l'utente dovrà selezionare per attivare
la generazione del cookie, e la conseguente memorizzazione a livello
client delle credenziali di accesso al sito.

**Giorni di Scadenza:** consente di definire i giorni di scadenza del
cookie generato dal componente in esame. Una volta trascorso il periodo
indicato il cookie verrà automaticamente eliminato dal browser e
l'utente dovrà quindi digitare nuovamente le proprie credenziale per
accedere al sito.

Nel caso in cui un utente decida di effettuare l'accesso al sito
selezionando il campo "Ricordami", e generando conseguentemente il
relativo cookie, nel momento in cui questo stesso utente dovesse poi
tentare di disconnettersi dal sito, cliccando per questo sul pulsante di
Logout, verrà visualizzato un apposito messaggio per avvisarlo che,
effettuando questa operazione, il cookie precedentemente salvato verrà
eliminato e al successivo accesso sarà quindi necessario inserire
nuovamente le relative credenziali.

Cliccando sul pulsante "**Conferma**" il cookie precedentemente salvato
verrà cancellato e l'utente, nelle successive visite, non verrà più
autenticato in maniera automatica.

Cliccando invece sul pulsante "**Annulla**" e chiudendo semplicemente il
browser il cookie verrà mantenuto e utilizzato durante le prossime
visite dell'utente per effettuare il login automatico.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

