# CONFIGURAZIONE



All'interno della sezione "**Configurazione**" accessibile dalla voce
del menu principale "Posta / SMS", è possibile abilitare le varie
funzionalità di invio mail ed sms offerte da Passweb.

**ATTENZIONE! Passweb non dispone di server di posta interni o di
servizi integrati di invio SMS. In conseguenza di ciò per attivare le
relative funzionalità e necessario appoggiarsi a servizi / provider
esterni**

Una volta effettuato l'accesso a questa sezione del Wizard verrà
visualizzata la maschera "**Account e-mail e SMS**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\posta_sms.bmp](./assets/media/image1.png){width="5.760416666666667in"
height="3.4784722222222224in"}

all'interno della quale il campo:

- **E-Mail:** consente di specificare l'indirizzo E-mail del Webmaster,
  indirizzo questo che sarà poi utilizzato come mittente delle varie
  mail inviate in automatico dall'applicazione.

- **Firma sulle Email:** consente di specificare la firma che verrà
  apposta, in automatico, alla fine di tutte le mail inviate in
  automatico dall'applicazione.

**ATTENZIONE! Le varie mail inviate in automatico dall'applicazione (es.
mail di ricezione ordini, mail di registrazione, mail di notifica sul
raggiungimento dei limiti contrattuali ecc...) verranno inviate solo ed
esclusivamente nel caso in cui la pagina in oggetto sia stata compilata
correttamente**

La sezione "**Configurazione Server di Posta**" permette invece di
impostare i parametri di configurazione necessari per effettuare la
connessione con il server di posta da utilizzare per l'invio delle mail.

Nello specifico il campo:

**Tipo di sicurezza:** consente di impostare il protocollo di accesso da
utilizzare per connettersi al server di posta. E' possibile indicare uno
dei seguenti valori:

- **Nessuno**: la connessione al server di posta verrà effettuata senza
  nessun meccanismo di sicurezza

- **SSL/TLS**: la connessione al server di posta verrà effettuata
  utilizzando il protocollo SSL/TLS

- **OAuth2**: la connessione al server di posta verrà effettuata
  utilizzando il protocollo OAuth2

A seconda del Tipo di Sicurezza impostata sarà poi necessario indicare
altri specifici parametri di configurazione

In particolare nel caso in cui il "**Tipo di Sicurezza**" dovesse essere
impostato sulle opzioni "**Nessuno**" o "**SSL/TLS**" sarà poi
necessario indicare i parametri di connessione allo specifico server
SMTP che si intente utilizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\posta_sms_configurazione_1.bmp](./assets/media/image2.png){width="5.760416666666667in"
height="3.4784722222222224in"}

- **Server SMTP:** consente di indicare l'indirizzo del server SMTP che
  dovrà essere utilizzato per l'invio delle mail

- **Porta**: consente di indicare la porta utilizzata dal server SMTP
  indicato all'interno del campo precedente

- **Richiedi accesso:** se impostato a Si consente di indicare
  all'interno dei successivi campi "**Nome Utente**" e "**Password**",
  le credenziali necessarie per effettuare l'autenticazione sul server
  SMTP indicato.

Nel momento in cui il "**Tipo di Sicurezza**" dovesse invece essere
impostato sull' opzione "**OAuth2**" sarà necessario indicare,
selezionandolo tra quelli attualmente gestiti da Passweb, il servizio di
OAuth da utilizzare per collegare Passweb al relativo provider Email.

In generale, per poter effettuare l'autenticazione ad un server di posta
mediante il protocollo OAuth2 occorre, innanzitutto, che il provider
Email offra questa metodologia di accesso e, tipicamente, sarà poi
necessario creare sulla piattaforma del provider stesso un App che
consenta di ottenere il token necessario per effettuare
l'autenticazione.

In questo senso Passweb offre attualmente la possibilità di effettuare
l'autenticazione con protocollo OAuth2 verso i seguenti provider Email:

- **Google**

- **Microsoft**

In relazione ad essi, inoltre, non sarà necessario, per ottenere il
token di autenticazione, creare una propria App sulle relative
piattaforme ma si potrà tranquillamente utilizzare l'App già realizzata
e messa a disposizione direttamente da Passepartout.

In sostanza dunque, nel momento in cui l'esigenza dovesse essere quella
di inviare le mail utilizzando come provider Microsoft o Google e OAuth2
come protocollo di autenticazione, sarà sufficiente indicare,
all'interno del relativo campo l'indirizzo Email della casella di posta
con cui verranno poi spedite le varie mail (lo stesso indirizzo
utilizzato per effettuare l'accesso via web al proprio account di posta)
e cliccare poi sul pulsante "Genera Token" per ottenere il token di
autenticazione sfruttando l'App messa a disposizione direttamente da
Passepartout

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\posta_sms_configurazione_2.bmp](./assets/media/image3.png){width="5.760416666666667in"
height="3.4784722222222224in"}

In queste condizioni dunque il campo:

- **Tipologia di OAuth**: consente di indicare, selezionandolo dal
  relativo menu a tendina, il servizio di OAuth da utilizzare per
  collegare Passweb al proprio provider Email.

> **ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
> inviare mail utilizzando una casella Gmail si consiglia di selezionare
> Google come servizio di OAuth. Allo stesso modo nel momento in cui
> l'esigenza dovesse essere quella di inviare mail da un' account
> Microsoft (es. outlook.com, outlook 365 ...) il consiglio è quello di
> utilizzare Microsoft come servizio di OAuth.

- **Nome Utente OAuth**: consente di indicare l'indirizzo mail che verrà
  poi utilizzato per effettuare il login sulla piattaforma terza.
  All'interno di questo campo va quindi inserito l'indirizzo dalla
  casella mail da collegare a Passweb e che verrà poi utilizzata per
  l'invio di tutte le mail gestite dall'applicativo

Per maggiori informazioni in merito a come configurare un account
Microsoft o Gmail come server di posta utilizzando il protocollo OAuth2
si veda anche quanto indicato nei successivi capitoli di questo manuale
("*Esempi di configurazione server di posta -- Sicurezza OAuth2*")

Il pulsante "**Test Invio Mail**" consente di inviare una mail di prova
utilizzando il server di posta appena definito in maniera tale da
verificare che la configurazione indicata sia effettivamente quella
corretta.

**ATTENZIONE! La configurazione del server di posta dipende ovviamente
dallo specifico server SMTP che si desidera utilizzare.**

Nel successivo capitolo di questo manuale verranno indicate, a titolo
puramente esemplificativo, alcune possibili configurazioni dei server
SMTP più comuni (es. alice, Gmail, Yahoo, Outlook.com ecc...).

Per maggiori informazioni in merito si consiglia comunque di fare sempre
riferimento alla documentazione dello specifico fornitore.

**ATTENZIONE! Nel momento in cui la configurazione del server di posta
da utilizzare non dovesse essere effettuata correttamente l'applicazione
non potrà inviare nessun tipo di Email**

La sezione "Configurazione SMS" consente infine di impostare le
credenziali di accesso al servizio di invio SMS.

- **Login SMS**: login di accesso al servizio di invio sms;

- **Password SMS**: password di accesso al servizio di invio sms.

**ATTENZIONE! Per poter attivare il servizio di invio sms è necessario
innanzitutto che l'amministratore si registri sul sito
http://www.smshosting.it, che acquisti un pacchetto di sms ed infine che
inserisca nei due campi sopra evidenziati, la login e la password
specificate in fase di registrazione al servizio di invio sms.**

Una volta inserite e validate correttamente le credenziali, verranno
visualizzate anche informazioni relative al credito residuo e al numero
di sms ancora inviabili.

