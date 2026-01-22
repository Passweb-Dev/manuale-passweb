# DISISCRIZIONE AL SISTEMA DI NEWSLETTER ACTIVECAMPAIGN ESTERNAMENTE AL FORM DI PROFILO UTENTE



Uno step indispensabile nell'implementazione di un corretto sistema di
gestione delle Newsletter è indubbiamente quello che permette agli
utenti iscritti di potersi disiscrivere in un qualsiasi momento.

Utilizzando ActiveCampaign come sistema di gestione delle Newsletter
questo processo può essere implementato sia con componenti nativi di
Passweb (esternamente o internamente al form di profilo utente) sia
utilizzando il form di disiscrizione messo a disposizione (**su di una
pagina diversa del sito Passweb**) da ActiveCampaign stesso, form questo
che, tipicamente, potrà essere raggiunto cliccando su di un apposito
link di "**Unscribe**" da inserire all'interno di ogni mail inviata dal
sistema di Newsletter (per maggiori informazioni in merito si rimanda
alla relativa documentazione di ActiveCampaign).

Nel momento in cui l'esigenza dovesse essere invece quella di gestire la
disiscrizione alla Newsletter di ActiveCampaign utilizzando i componenti
nativi di Passweb e, in particolare, un form specifico scollegato da
tutto il resto e quindi esternamente al "Profilo Utente", sarà
necessario utilizzare il componente di primo livello "**Iscrizione
Newsletter**" impostando i parametri di configurazione "**Tipo di
Integrazione**" e "**Tipologia Form**" rispettivamente sui valori
"**ActiveCampaign**" e "**Disiscrzione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_disiscrizione_newsletter_activecampaign.bmp](./assets/media/image64.png){width="4.370138888888889in"
height="3.9479166666666665in"}

Il campo "**Lista Associata**" consentirà inoltre di indicare,
selezionandola tra quelle definite all'interno del proprio account
ActiveCampaign, la specifica Lista da cui l'utente dovrà essere
disiscritto.

**ATTENZIONE!** impostando il campo "**Lista Associata**" sull'opzione
"**Tutte**" l'utente verrà disiscritto da tutte le Liste presenti
all'interno di ActiveCampaign

**Come per MailChimp e BrainLead, anche in questo caso l'unico campo
presente all'interno del form, inserito automaticamente al salvataggio
del componente, sarà il campo Email**

![Videate\\form_disiscrizone_newsletter.bmp](./assets/media/image57.png){width="5.6625in"
height="3.298611111111111in"}

Una volta inserito lo stesso indirizzo mail utilizzato anche in fase di
iscrizione al servizio, cliccando sul pulsante "**Disiscriviti**",
l'utente verrà disiscritto dalla Lista indicata in fase di
configurazione del componente, mantenendo comunque inalterati tutti i
suoi dati (compresi eventuali dati ecommerce e/o consensi GDPR
precedentemente forniti)

Lo stato del contatto potrà essere verificato, ovviamente, anche
all'interno di ActiveCampaign esaminando il campo "**Liste -- Email**"
presente all'interno della sua anagrafica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\annullamento_iscrizione_activecampaign.bmp](./assets/media/image65.png){width="5.538888888888889in"
height="3.4743055555555555in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\annullamento_iscrizione_activecampaign_2.bmp](./assets/media/image66.png){width="5.538888888888889in"
height="3.4743055555555555in"}

**ATTENZIONE! la disiscrizione dal servizio di Newsletter di
ActiveCampaign NON comporta l'eliminazione della relativa anagrafica
sulla piattaforma terza ma, semplicemente, annulla l'iscrizione
dell'utente alla Lista indicata in fase di configurazione del componente
Passweb.**

Nel momento in cui l'esigenza dovesse invece essere quella di eliminare
completamente l'anagrafica dell'utente sul database della piattaforma
terza, questo potrà essere fatto direttamente dall'interessato operando
dalla pagina "Profilo Utente" attraverso il pulsante **"Elimina
Profilo"**

![Videate\\elimina_profilo.bmp](./assets/media/image27.png){width="5.552083333333333in"
height="3.298611111111111in"}

**Cliccando su questo pulsante infatti oltre a cancellare la
corrispondente anagrafica dal database di Passweb, questa verrà
eliminata completamente anche dal database di ActiveCampaign.**

**ATTENZIONE!** Nel momento in cui si dovesse decidere di attivare
l'integrazione tra il proprio sito e ActiveCampaign il consiglio è
quello di personalizzare il messaggio di "conferma eliminazione" del
profilo utente indicando esplicitamente che i dati verranno,
eventualmente, cancellati in maniera definitiva anche dal database della
piattaforma di newsletter.

![Videate\\messaggio_conferma_eliminazione_profilo.bmp](./assets/media/image28.png){width="5.552083333333333in"
height="3.298611111111111in"}

