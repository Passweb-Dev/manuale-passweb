# ESEMPIO



**Portale con cui effettuare l'integrazione**:
https://www.themoviedb.org/

Il portale in questione espone endpoint interrogabili per ottenere
informazioni su film e spettacoli tv
(<https://developer.themoviedb.org/reference/getting-started>).

Richiede una registrazione per poter ottenere chiavi e token necessari
per poter effettuare le relative chiamate API e gestisce due diversi
meccanismi di autenticazione, con Api Key e con Token di Autenticazione.

Una volta effettuata la registrazione al servizio
(<https://www.themoviedb.org/signup>) all'interno della sezione
"**Impostazioni -- API**" troveremo tutti i parametri necessari per
poter configurare correttamente l'integrazione tra questo portale e
Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\portali_esempio_utilizzo_1.bmp](./assets/media/image294.png)

Nello specifico all'interno del campo "**API Read Access Token**" è
indicato l'Access Token da utilizzare nel caso in cui si dovesse
decidere di integrare le due piattaforme in modalità "Authentication
with Token".

Nel campo "**Chiave API**" troveremo invece la chiave da utilizzare nel
caso in cui si dovesse decidere di integrare le due piattaforme in
modalità "Api Key".

**ATTENZIONE!** ovviamente i parametri e le modalità di autenticazione
variano in relazione a quelle che sono le diverse possibilità offerte
dalla specifica piattaforma con cui ci si deve integrare.

A questo punto dunque il primo passo sarà quello di configurare
l'integrazione tra le due piattaforme utilizzando uno dei metodi sopra
indicati.

