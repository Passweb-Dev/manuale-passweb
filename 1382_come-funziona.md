# COME FUNZIONA



Come già evidenziato nei precedenti capitoli di questo manuale Matomo si
presenta come un software piuttosto semplice e molto simile alla
versione classica di Universal Analytics. Il data model di Matomo
infatti è analogo, per molti aspetti, a quello utilizzato da Universal
Analytics e questo rende possibile anche l'importazione dei dati da una
proprietà UA verso un'installazione di Matomo.

Di base il tracciamento di quello che succede all'interno del sito viene
effettuato lato client (via Javascript), in modo molto simile a quello
che avviene anche con Google Analytics, inserendo quindi un apposito
snippet di codice, prelevabile direttamente dalle impostazioni di
configurazione di Matomo, nelle pagine del proprio sito.

![](./assets/media/image6.png)

L\'utente che si collega e naviga sul sito così configurato verrà quindi
inserito in una sessione collegata generalmente a dei cookie.

**ATTENZIONE!** Lo script sopra evidenziato consente, se installato
correttamente, di attivare il monitoraggio standard tracciando solamente
le visite alle pagine del sito.

Nel momento in cui l'esigenza dovesse essere quella di attivare anche un
monitoraggio Ecommerce sarà quindi necessario gestire anche altre
impostazioni di configurazione che, nello specifico relativamente a
Passweb, riguarderanno l'attivazione di un semplice flag per consentire
all'applicativo di tracciare anche eventi quali la visualizzazione dei
prodotti, l'aggiunta in carrello, la creazione di un ordine ecc...

**ATTENZIONE!** Gli eventi Ecommerce tracciabili con Matomo dipendono,
ovviamente, dalle possibilità offerte dalla piattaforma stessa e non
coincidono esattamente con lo stesso tipo di eventi tracciabili, ad
esempio, con GA4

Questo tipo di tracking (via javascript) è il più semplice perché non
richiede particolari conoscenze tecniche per essere configurato.
Tuttavia è bene sottolineare anche che, così come avviene per altri
strumenti come appunto Google Analytics, in queste condizioni gli utenti
che disabilitano Javascript oppure rifiutano i cookie non verranno
tracciati.

Nel momento in cui l'esigenza dovesse essere quella di raggiungere
obiettivi più specifici, come ad esempio il remarketing, o comunque
quella di avere statistiche molto più precise, è opportuno valutare
anche l'utilizzo del tracciamento lato server, opzione questa già
prevista nativamente all'interno del proprio sito Passweb mediante la
configurazione di alcuni semplici parametri.

Oltre al tracciamento lato server (che utilizza apposite API messe a
disposizione dalla piattaforma) e al tracciamento tradizionale lato
client (che fa uso di javascript e cookie), Matomo offre poi anche altre
impostazioni avanzate di configurazione che consentono, ad esempio, di
tracciare gli utenti che hanno javascript disabilitato

![](./assets/media/image7.png)

e/o di attivare un tracciamento cookieless (che non prevede cioè
l'utilizzo di cookie)

![](./assets/media/image8.png)

Per maggiori informazioni relativamente a quest'ultima possibilità
(tracciamento cookieless) ed, eventualmente, a come poter gestire
correttamente questo tipo di configurazione assieme all'utilizzo dei
diversi banner di approvazione dei cookie offerti dalle diverse
piattaforme CMP si consiglia di fare riferimento a quanto indicato ai
seguenti link

<https://matomo.org/cookie-consent-banners/?menu>

<https://matomo.org/faq/new-to-piwik/how-do-i-use-matomo-analytics-without-consent-or-cookie-banner/>

<https://matomo.org/faq/new-to-piwik/how-can-i-still-track-a-visitor-without-cookies-even-if-they-decline-the-cookie-consent/>

<https://www.iubenda.com/it/help/3592-full-piwik-integration-guide>

Al seguente indirizzo <https://demo.matomo.cloud/> è invece possibile
visualizzare ed utilizzare una Demo Online gratuita per avere un'idea
più precisa di quelle che sono le funzionalità disponibili e di come
funziona effettivamente la piattaforma.

