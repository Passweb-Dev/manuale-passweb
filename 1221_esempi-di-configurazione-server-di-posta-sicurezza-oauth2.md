# ESEMPI DI CONFIGURAZIONE SERVER DI POSTA -- SICUREZZA OAUTH2



Come già indicato nei precedenti capitoli di questo manuale, in
generale, per poter effettuare l'autenticazione ad un server di posta
mediante il protocollo OAuth2 occorre, per prima cosa, che il provider
Email offra effettivamente questa tipologia di autenticazione,
successivamente sarà poi necessario creare sulla piattaforma del
provider stesso un App che consenta di ottenere il token necessario per
effettuare l'autenticazione.

In questo senso Passweb offre attualmente la possibilità di effettuare
l'autenticazione con protocollo OAuth2 verso i seguenti provider Email:

- **Google**

- **Microsoft**

In relazione ad essi, inoltre, non sarà necessario, per ottenere il
token di autenticazione, creare una propria App sulle relative
piattaforme (dovendo quindi passare attraverso il processo di
validazione richiesto, in questo senso, da Google o Microsoft) ma si
potrà tranquillamente utilizzare l'App già realizzata e messa a
disposizione direttamente da Passepartout, fornendole ovviamente le
relative autorizzazioni di accesso.

In sostanza dunque, nel momento in cui l'esigenza dovesse essere quella
di inviare le mail utilizzando come provider Microsoft o Google e OAuth2
come protocollo di autenticazione, sarà sufficiente indicare,
all'interno del relativo campo, l'indirizzo Email della casella di posta
con cui verranno poi spedite le varie mail (lo stesso indirizzo
utilizzato per effettuare l'accesso via web al proprio account di
posta), cliccare sul pulsante "Genera Token" e concedere all'App
Passepartout le autorizzazioni richieste.

Di seguito sono indicate, in maniera un po' più dettagliata le procedure
da seguire per utilizzare come server di posta una casella Gmail o
Microsoft e come protocollo di autenticazione OAuth2

