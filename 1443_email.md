# EMAIL



Il modulo Email di Clerk rappresenta una soluzione avanzata per la
personalizzazione automatica dei contenuti all'interno delle email,
sfruttando la potenza della sua intelligenza artificiale. Grazie a
questo strumento, è possibile includere dinamicamente prodotti
raccomandati, personalizzati o contestuali direttamente nelle campagne
email, migliorando in modo significativo l'engagement, il click-through
rate e la conversione.

Questa funzionalità è pensata per integrarsi con i più diffusi provider
di invio email (ESP), come MailChimp, ActiveCampaign Sendinblue, e molti
altri e può essere utilizzata anche per importare direttamente da queste
piattaforme l'elenco di contatti.

Il modulo Email ha quindi lo scopo di:

- Inserire prodotti dinamici e personalizzati all'interno di email HTML

- Generare contenuti aggiornati in tempo reale al momento dell'apertura
  dell'email

- Potenziare le strategie di retargeting, fidelizzazione e
  cross-selling.

- Mantenere l'utente coinvolto anche dopo la visita o l'acquisto.

In definitiva questa funzione permette di trasformare ogni singola email
in una vetrina altamente personalizzata, basata sul comportamento
dell'utente, sul suo storico di acquisti e sulle performance dei
prodotti a catalogo.

Volendo poi può essere utilizzata anche per gestire interamente un
sistema di newsletter sia a livello marketing sia a livello di mail
automatizzate legate ad esempio ai carrelli abbandonati e/o alle
sessioni di visita al sito concluse senza portare a termine degli
ordini.

**Sotto questo punto di vista, al momento, l'integrazione Passweb --
Clerk non prevede però nulla di nativo**, il consiglio quindi è quello
di continuare ad utilizzare, per il servizio di Newsletter e di
Marketing Automation, una delle piattaforme attualmente integrabili in
Passweb (ActiveCampaign, MailChimp ecc...)

In questo senso è bene ricordare anche, come già evidenziato nei
precedenti capitoli di questo manuale, tutti gli utenti inviati da
Passweb a Clerk avranno il parametro "**subscribed**" impostato
automaticamente a "false".

Tale parametro è quello che determina la possibilità di inviare ai
relativi utenti, direttamente da Clerk (con la funzionalità di
Newsletter del modulo di Email) comunicazioni di carattere commerciale.

Ora, considerando che al momento non è attiva l'integrazione Passweb --
Clerk per quel che riguarda la gestione della Newsletter, Passweb dovrà
necessariamente impostare tale parametro a false. L'informazione
relativa alla possibilità di inviare comunicazioni di carattere
commerciale ai vari utenti (Iscrizione Newsletter Si/No) verrà infatti
salvata direttamente sulla specifica piattaforma (MailChimp,
ActiveCampaign ...) integrata con Passweb e utilizzata per gestire
questo tipo di servizio.

Questo non pregiudica la possibilità di integrare Clerk direttamente con
una delle piattaforme di Newsletter gestite da Passweb e quindi la
possibilità di creare direttamente da Clerk sulle altre piattaforme le
varie audience generate e gestite dalla sua IA.

Semplicemente Clerk non saprà a quale utente poter inviare comunicazioni
di carattere commerciale e a quale utente non poterlo fare perché non
sarà Clerk a gestire questi invii. Questo lo farà direttamente
ActiveCampaign o MailChimp che riceveranno l'informazione da Passweb nel
momento in cui un utente dovesse decidere di iscriversi o disiscriversi
alla Newsletter direttamente dal sito.

L'unica accortezza in questo caso dovrà essere dunque quella **di non
esportare direttamente da Clerk, sulla piattaforma utilizzata in Passweb
per gestire la Newsletter, i vari utenti (subscribers).**

Per far questo sarà necessario verificare di non aver attivato
all'interno della sezione "**Sync subscribers**" (modulo "**Email --
Configuration**") di Clerk degli esportatori verso la piattaforma di
Newsletter utilizzata su Passweb (ActiveCampaign, MailChimp ...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\export_utenti_mail_clerk.bmp](./assets/media/image16.png)

Nel momento in cui uno degli esportatori evidenziati in figura dovesse
essere attivato infatti, lo stato di iscrizione al relativo servizio di
Newsletter, inizialmente impostato da Passweb sulla base della scelta
effettuata dall'utente sul sito, potrebbe poi essere sovrascritto da
Clerk (dove come detto subscribed sarà sempre impostato a false) **con
il risultato che nessuno degli utenti presenti nelle varie liste di
ActiveCampaign o MailChimp potrà poi ricevere comunicazioni di carattere
commerciale**

Per quanto riguarda invece la possibilità di inserire nelle newsletter o
nelle mail gestite con altre piattaforme, magari anche integrate
direttamente con Passweb (es. MailChimp, ActiveCampaign), le
raccomandazioni di prodotto, tutto il sistema può e deve essere gestito
direttamente dal backend di Clerk e non ha un impatto diretto sul
backend di Passweb o sul front end del sito che non sia già previsto
dalle integrazioni con il modulo Search o Reccomendations

In conseguenza di ciò per maggiori informazioni relativamente
all'utilizzo di questo modulo e, a come poter inserire delle
raccomandazioni nelle varie mail si rimanda direttamente alla
documentazione di prodotto e/o al supporto Clerk.

