# FORM DI ISCRIZIONE



Relativamente ai form di iscrizione alla Newsletter va detto subito che
ActiveCampaign mette a disposizione dell'utente la possibilità di
embeddare all'interno del sito form di iscrizione creati direttamente
sulla piattaforma operando in questo senso all'interno della sezione
"**Sito -- Moduli**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\activecampaign_form_iscrizione_1.bmp](./assets/media/image9.png)

**ATTENZIONE!** per maggiori informazioni relativamente a come poter
creare e gestire all'interno di ActiveCampaign i vari form di iscrizione
alla Newsletter si rimanda alla relativa documentazione di prodotto

Nel momento in cui l'esigenza dovesse essere quella di creare un form di
iscrizione alla Newsletter a se stante, da inserire magari in tutte le
pagine del sito, questa potrebbe essere sicuramente la soluzione più
rapida. In queste caso infatti non ci sono ragioni specifiche per
ricreare questo form direttamente in Passweb, anzi il fatto di embeddare
il form creato direttamente su ActiveCampaign offre anche la possibilità
di gestire l'iscrizione alla Newsletter con il double opt-in.

In ogni caso se la scelta dovesse essere comunque quella di creare il
form di iscrizione utilizzando i componenti nativi di Passweb, sarà
perfettamente possibile farlo utilizzando il componente Form generico
all'interno del quale dovrà essere inserito il componente
"**Newsletter**" configurato ovviamente per poter interagire con
ActiveCampaign.

Va detto anche che, in questo caso, non sarà però possibile gestire
l'iscrizione con il double opt-in per cui, per essere compliance con il
GDPR, dovranno essere inseriti nel form di iscrizione appositi campi
contatto custom di ActiveCampaign per raccogliere tutti i consensi del
caso

Per maggiori informazioni relativamente a come poter utilizzare il
componente "Form" di Passweb per creare un modulo di iscrizione alla
Newsletter di ActiveCampaign si rimanda a quanto indicato all'interno
del capitolo "*Componenti Interazione Utente -- Componenti interni ai
Componenti Interazione Utente -- Componente Newsletter -- Iscrizione
alla Newsletter mediante Form generico*" di questo manuale.

Nel momento in cui l'esigenza dovesse essere invece quella di consentire
agli utenti di iscriversi alla Newsletter direttamente in fase di
iscrizione al sito non sarà possibile embeddare i form creati su
ActiveCampaign e l'unica possibilità sarà quella di utilizzare il
componente Passweb "**Newsletter**" inserendolo all'interno del
Componente di primo livello **Registrazione Utente** e impostando, in
fase di configurazione, il campo "**Tipo di Integrazione**" sul valore
"**ActiveCampaign**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_activecampaign.bmp](./assets/media/image10.png)

Una volta completata la configurazione del componente, al salvataggio,
l'applicazione si preoccuperà di contattare ActiveCampaign, utilizzando
la relativa API Key inserita in fase di configurazione del sito (pagina
"*Sito -- Gestione Newsletter -- Email Marketing*"), **preleverà tutti i
campi Contatto Custom definiti sulla piattaforma terza e li inserirà,
assieme ai campi Contatto Standard anch'essi presenti su ActiveCampaign
(Nome, Cognome, Email ...), all'interno del form di Registrazione
Utente.**

A questo punto dovremo quindi decidere, tra tutti i campi importati da
ActiveCampaign, quali visualizzare all'interno del form di registrazione
nel momento in cui l'utente dovesse decidere di iscriversi al servizio,
quali nascondere e quali mappare con campi già presenti nello stesso
form di registrazione evitando così all'utente di inserire la stessa
informazione due volte.

Una volta configurato correttamente il componente in oggetto,
all'interno del form di registrazione al sito verrà visualizzato anche
un Radio Button con le due opzioni **Si / No**, **opzioni queste che**
**permetteranno all'utente di poter decidere se iscriversi o meno anche
alla Newsletter**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image11.png)

Nel caso in cui l'utente dovesse decidere di registrarsi al sito senza
iscriversi alla Newsletter (opzione **No**) non verrà visualizzato
nessuno dei campi importati da ActiveCampaign e, ovviamente, non verrà
inviata alla piattaforma terza nessun tipo di informazione.

Nel momento in cui l'utente dovesse invece decidere di iscriversi anche
alla Newsletter (opzione **Si**) verranno visualizzati **i campi
importati da ActiveCampaign** che si è deciso, in fase di
configurazione, di voler effettivamente visualizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione3.bmp](./assets/media/image12.png)

Per maggiori informazioni in merito a come poter gestire l'iscrizione
alla Newsletter direttamente in fase di registrazione al sito si rimanda
a quanto indicato all'interno del capitolo "*Componenti Interazione
Utente -- Componenti interni ai Componenti Interazione Utente --
Componente Newsletter -- Iscrizione alla Newsletter ActiveCampaign in
fase di registrazione al sito*" di questo manuale

