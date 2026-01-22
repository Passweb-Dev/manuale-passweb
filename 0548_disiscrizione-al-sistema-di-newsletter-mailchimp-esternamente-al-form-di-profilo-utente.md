# DISISCRIZIONE AL SISTEMA DI NEWSLETTER MAILCHIMP ESTERNAMENTE AL FORM DI PROFILO UTENTE



Uno step indispensabile nell'implementazione di un corretto sistema di
gestione delle Newsletter è indubbiamente quello che permette agli
utenti iscritti di potersi disiscrivere in un qualsiasi momento.

Utilizzando MailChimp come sistema di gestione delle Newsletter questo
processo può essere implementato, così come avviene anche per
l'iscrizione, sia con componenti nativi di Passweb (esternamente o
internamente al form di profilo utente) sia utilizzando direttamente il
form di disiscrizione MailChimp (**Unscribe Form**) con uno dei metodi
di integrazione messi a disposizione dalla piattaforma terza (per
maggiori informazioni in merito ai metodi di integrazione messi a
disposizione da MailChimp si rimanda alla specifica documentazione di
prodotto).

Nello specifico poi, se l'esigenza dovesse essere quella di gestire la
disiscrizione alla Newsletter MailChimp utilizzando i componenti nativi
di Passweb e, in particolare, con un form specifico scollegato da tutto
il resto e quindi esternamente al "Profilo Utente" sarà necessario
utilizzare il componente di primo livello "Iscrizione Newsletter
(MailChimp o BrainLead)" impostando i parametri di configurazione
"**Tipo di Integrazione**" e "**Tipologia Form**" rispettivamente sui
valori "**MailChimp**" e "**Disiscrzione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_disiscrizione_newsletter_mailchimp.bmp](./assets/media/image51.png)

In queste condizioni, esattamente allo stesso modo di quanto avviene per
il form di iscrizione, al salvataggio del componente l'applicazione si
preoccuperà di contattare MailChimp, utilizzando l'API Key inserita in
fase di configurazione del sito (pagina "**Sito -- Preferenze**", tab
"**Integrazioni**", campo "**MailChimp API Key**"), prelevando questa
volta il form di disiscrizione (**Unscribe** **form)** associato alla
lista selezionata e andrà poi ad inserire automaticamente i relativi
campi all'interno della pagina del sito Passweb.

In genere, questo tipo di form ha il solo campo mail che l'utente dovrà
valorizzare, ovviamente, con lo stesso indirizzo utilizzato in fase di
iscrizione al servizio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_disiscrizone_newsletter.bmp](./assets/media/image52.png)

Una volta inserito l'indirizzo mail, cliccando sul pulsante
"**Disiscriviti**" l'utente verrà quindi disiscritto dal servizio.

Nello specifico poi a seguito di questa operazione la sua anagrafica
verrà posta, all'interno della corrispondente lista MailChimp, nello
stato di "**Archiviato**" lasciando comunque inalterati eventuali altri
dati relativi all'utente stesso.

![Videate\\mailchimp_utente_archiviato.bmp](./assets/media/image53.png)

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
eliminata completamente anche dal database di MailChimp.**

**ATTENZIONE!** Nel momento in cui si dovesse decidere di attivare
l'integrazione tra il proprio sito e MailChimp il consiglio è quello di
personalizzare il messaggio di "conferma eliminazione" del profilo
utente indicando esplicitamente che i dati verranno, eventualmente,
cancellati in maniera definitiva anche dal database della piattaforma di
newsletter.

![Videate\\messaggio_conferma_eliminazione_profilo.bmp](./assets/media/image28.png)

In queste condizioni va ricordato inoltre che:

- la cancellazione dell'anagrafica utente effettuata dal backend
  (Wizard) del sito Passweb NON comporta l'eliminazione della stessa
  anagrafica anche dal database della piattaforma utilizzata per gestire
  la Newsletter.

- **MailChimp non consente la reiscrizione di un utente precedentemente
  eliminato in maniera definitiva mediante un form di terze parti (es.
  integrazioni via API).** In conseguenza di ciò un utente eliminato in
  maniera definitiva dal database di MailChimp potrà, eventualmente,
  reiscriversi alla stessa Newsletter **solo attraverso uno dei form
  nativi messi a disposizione da MailChimp stesso.**

> Se un utente precedentemente eliminato dovesse quindi tentare di
> effettuare una nuova iscrizione da uno dei form Passweb (es.
> Registrazione / Profilo Utente ) questa non potrà andare a buon fine
> e, contestualmente, verrà inviata una mail all'amministratore del sito
> per notificargli il problema

