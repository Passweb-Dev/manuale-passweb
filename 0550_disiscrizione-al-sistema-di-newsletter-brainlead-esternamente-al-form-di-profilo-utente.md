# DISISCRIZIONE AL SISTEMA DI NEWSLETTER BRAINLEAD ESTERNAMENTE AL FORM DI PROFILO UTENTE



Uno step indispensabile nell'implementazione di un corretto sistema di
gestione delle Newsletter è indubbiamente quello che permette agli
utenti iscritti di potersi disiscrivere in un qualsiasi momento.

Utilizzando BrainLead come sistema di gestione delle Newsletter questo
processo può essere implementato sia con componenti nativi di Passweb
(esternamente o internamente al form di profilo utente) sia utilizzando
il form di disiscrizione messo a disposizione (su di una pagina diversa
dal sito Passweb) da BrainLead stesso, form questo che, tipicamente,
potrà essere raggiunto cliccando su di un apposito link di "Unscribe" da
inserire all'interno di ogni mail inviata dal sistema di Newsletter (per
maggiori informazioni in merito si rimanda alla relativa documentazione
BrainLead).

Nel momento in cui l'esigenza dovesse essere invece quella di gestire la
disiscrizione alla Newsletter BrainLead utilizzando i componenti nativi
di Passweb e, in particolare, con un form specifico scollegato da tutto
il resto e quindi esternamente al "Profilo Utente" sarà necessario
utilizzare il componente di primo livello "Iscrizione Newsletter
(MailChimp o BrainLead)" impostando i parametri di configurazione
"**Tipo di Integrazione**" e "**Tipologia Form**" rispettivamente sui
valori "**BrainLead**" e "**Disiscrzione**"

![](./assets/media/image56.png)

**ATTENZIONE! in queste condizioni l'unico campo presente all'interno
del form, inserito automaticamente al salvataggio del componente, sarà
il campo Email**

![Videate\\form_disiscrizone_newsletter.bmp](./assets/media/image57.png)

Una volta inserito lo stesso indirizzo mail utilizzato anche in fase di
iscrizione al servizio, cliccando sul pulsante "**Disiscriviti**",
l'utente verrà quindi disiscritto dal servizio, mantenendo comunque
inalterati tutti i suoi dati (compresi eventuali altri consensi
precedentemente forniti e memorizzati all'interno di appositi campi
custom di tipo GDPR)

Il fatto poi che l'utente in esame ha effettuato una disiscrizione dal
servizio lo si potrà verificare anche su BrainLead grazie al piccolo
badge rosso posto, nel dettaglio della persona, in corrispondenza del
suo indirizzo mail

![](./assets/media/image58.png)

**ATTENZIONE! la disiscrizione dal servizio di Newsletter NON comporta
l'eliminazione della relativa anagrafica sulla piattaforma terza ma,
semplicemente, mette l'utente nelle condizioni di non ricevere più mail
di carattere commerciale.**

Nel momento in cui l'esigenza dovesse invece essere quella di eliminare
completamente l'anagrafica dell'utente sul database della piattaforma
terza, questo potrà essere fatto direttamente dall'interessato operando
dalla pagina "Profilo Utente" attraverso il pulsante **"Elimina
Profilo"**

![Videate\\elimina_profilo.bmp](./assets/media/image27.png)

**Cliccando su questo pulsante infatti oltre a cancellare la
corrispondente anagrafica dal database di Passweb, questa verrà
eliminata completamente anche dal database di Brainlead.**

**ATTENZIONE!** Nel momento in cui si dovesse decidere di attivare
l'integrazione tra il proprio sito e Brainlead il consiglio è quello di
personalizzare il messaggio di "conferma eliminazione" del profilo
utente indicando esplicitamente che i dati verranno, eventualmente,
cancellati in maniera definitiva anche dal database della piattaforma di
newsletter.

![Videate\\messaggio_conferma_eliminazione_profilo.bmp](./assets/media/image28.png)

