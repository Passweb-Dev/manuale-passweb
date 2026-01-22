# PUFFIN CRM



La sezione "**Puffin CRM**" consente di impostare i parametri di
configurazione richiesti per l'integrazione tra il proprio sito Passweb
e Puffin, integrazione questa che consentirà poi di inserire all'interno
del sito (ad esempio in apposite landing page) form in grado di creare
nuovi Lead all'interno del CRM

![](./assets/media/image138.png)

I campi presenti all'interno di questa sezione consentono dunque di:

**Tipologia Autenticazione Puffin CRM:** consente di attivare /
disattivare l'integrazione tra il proprio sito Passweb e Puffin.

**Url Installazione Puffin CRM**: consente di impostare l'url
dell'installazione Puffin da integrare con il proprio sito Passweb.

**ATTENZIONE!** l'url inserito in corrispondenza di questo parametro
dovrà essere nel formato "**topsoftsrl.idx1.prod.puffincrm.it**" e dovrà
quindi essere privo di https iniziale e anche di eventuali barre finali

**Token API**: consente di impostare la chiave necessaria per abilitare
la comunicazione tra le due piattaforme.

Per ottenere questa chiave è necessario accedere alla sezione
"**Impostazioni -- Configurazione -- Utenti -- Account CRM**" della
propria installazione Puffin

![](./assets/media/image139.png)

e creare un nuovo utente di servizio (pulsante "**Aggiungi**") di tipo
Amministratore in relazione al quale andare poi a generare la chiave da
inserire nel Wizard di Passweb

Una volta creato il nuovo utente sarà quindi necessario portarsi
all'interno della sezione "**Generazione Token**"

![](./assets/media/image140.png)

assegnare una data di validità alla chiave che si andrà poi a generare
(campi "**Data inizio validità**" e "**Data Fine Validità**") e
fleggare, all'interno del pannello "**Elenco Risorse**", i check di
seguito indicati

![](./assets/media/image141.png)

- **Lead** -- Lettura (GET) e Scrittura (POST)

- **Campi custom Form** -- Lettura (GET) e Scrittura (POST)

- **Tabella custom** -- Lettura (GET) e Scrittura (POST)

- **Tabella custom Struttura** -- Lettura (GET) e Scrittura (POST)

- **Tabella custom Options** -- Lettura (GET) e Scrittura (POST)

A questo punto sarà sufficiente cliccare sul pulsante "**Genera**"
presente in corrispondenza dell'intestazione "**Impostazioni Token**"
per ottenere la chiave richiesta che verrà così visualizzata all'interno
del campo "**Api-Key**"

![](./assets/media/image142.png)

Per completare il processo di integrazione sarà quindi sufficiente
copiare la chiave appena generata ed inserirla, assieme all' url della
propria installazione Puffin nella maschera di configurazione del Wizard
di Passweb precedentemente esaminata.

Il pulsante "**Test Connessione**" presente nella parte bassa di questa
stessa sezione consente infine di effettuare un test per verificare che
i parametri inseriti siano effettivamente corretti e che la connessione
tra le due piattaforme non presenti problemi.

**ATTENZIONE!** nel momento in cui si dovessero valorizzare i campi
presenti all'interno della sezione "Puffin CRM" la maschera "Sito --
Preferenze" del Wizard potrà essere salvata solo in assenza di problemi
di connessione tra Passweb e Puffin

**ATTENZIONE!** la chiave di configurazione inserita all'interno del
campo "Token API" resterà valida, ovviamente, fino alla data indicata su
Puffin in corrispondenza del campo "Data fino validità" precedentemente
evidenziato, dopo di che il consiglio è quello di revocare la vecchia
chiave e generarne una nuova.

Una volta completato con successo il processo di integrazione tra le due
piattaforme sarà possibile utilizzare il Componente Form di Passweb per
creare nuovi Lead all'interno di Puffin (per maggiori informazioni in
merito si rimanda a quanto indicato all'interno del capitolo
"*Componenti Comuni -- Componente Form -- Creazione Lead su Puffin CRM*"
di questo manuale)

##### CAMPI CUSTOM

Nel momento in cui l'esigenza dovesse essere quella di gestire
all'interno del form di creazione del Lead, oltre ai campi standard,
anche determinati campi Custom di Puffin, sarà necessario:

- Assicurarsi che l'utente di servizio utilizzato per gestire
  l'integrazione tra le due piattaforme abbia effettivamente la
  possibilità di gestire i Campi Custom

- Assicurarsi che la struttura di campi da utilizzare nel Form di
  acquisizione del Lead sia stata effettivamente associata, in Puffin,
  all'utente di servizio utilizzato per gestire l'integrazione tra le
  due piattaforme oltre che, ovviamente, a tutti gli utenti che dovranno
  poi visualizzare, sempre all'interno di Puffin, le anagrafiche dei
  Lead creati dai form Passweb

Nel primo caso, per fare in modo che l'utente di servizio abbia la
possibilità di gestire i Campi Custom, sarà necessario accedere alla sua
Anagrafica Puffin (dal menu "**Impostazioni -- Utenti -- Account
crm**"), selezionare il tab "**Funzionalità**" e verificare di aver
attivato il check "**Campi custom/Struttura campi custom**" presente
all'interno della sezione "**Campi Custom**" evidenziata in figura

![](./assets/media/image143.png)

Come detto però, il fatto di consentire all'utente di servizio (e quindi
a Passweb) di poter utilizzare i Campi Custom, di per sé non è
sufficiente considerando che, in Puffin, le diverse strutture di Campi
Custom devono anche essere assegnate in maniera specifica agli operatori
che dovranno poter visualizzare e gestire questi stessi campi.

In questo senso dunque, sarà di fondamentale importanza verificare,
indipendentemente dall'utente che in Puffin ha creato la struttura dei
campi custom da utilizzare nel form di acquisizione del lead, che questa
stessa struttura sia stata correttamente assegnata all'utente di
servizio (che dovrà poi valorizzare questi campi) e a tutti gli utenti
che dovranno visionare, all'interno di Puffin, i lead creati da Passweb.

Per far questo sarà necessario accedere alla sezione "**Impostazioni --
Configurazione -- Campi Custom -- Struttura campi custom**" evidenziata
in figura

![](./assets/media/image144.png)

selezionare, tra quelle presenti in elenco la struttura dei campi custom
che dovranno essere utilizzati all'interno del form Passweb

![](./assets/media/image145.png)

e verificare che tra gli "**Operatori selezionati**" (click sul numerino
posto a fianco della corrispondente etichetta) ci siano sia l'utente di
servizio utilizzato per l'integrazione tra le due piattaforme, sia tutti
gli utenti Puffin che dovranno poter accedere alle anagrafiche Lead
create da Passweb.

![](./assets/media/image146.png)

Nel momento in cui uno degli operatori interessati non dovesse essere
presente all'interno di questo elenco sarà sufficiente aggiungerlo
cliccando sul pulsante "**Aggiungi**" (
![](./assets/media/image147.png) )

**ATTENZIONE!** per maggiori informazioni sulla creazione / gestione
degli utenti Puffin e delle strutture di campi custom si consiglia di
fare riferimento sempre alla relativa documentazione di prodotto.

A questo punto, in fase di configurazione del form di acquisizione del
lead, quando andremo a mappare i campi di questo stesso form con i campi
Puffin, oltre a quelli standard troveremo anche i campi delle "Strutture
di campi custom" correttamente abilitate.

![](./assets/media/image148.png)

In realtà occorre fare anche un'ulteriore precisazione in merito a
quelli che sono i campi custom di Puffin che potranno essere
effettivamente gestiti all'interno di un form Passweb.

Al netto infatti di quanto sopra indicato occorre considerare anche che
in Passweb:

- sono gestite solamente le "Strutture di campi custom" in cui il campo
  "**Modulo**" e "**Sezione**" sono stati impostati rispettivamente sui
  valori "**Anagrafiche**" e "**Scheda Azienda / Lead**"

![](./assets/media/image149.png)

![](./assets/media/image150.png)

Inoltre tra i campi definiti all'interno di questo tipo di strutture
verranno prelevati e potranno quindi essere mappati nel form Passweb
solamente i campi di tipo:

- **Numero Intero**

- **Numero Decimale**

- **Testo**

- **Area di Testo**

- **Elenco**

- **Pulsante Radio**

- **Casella Checkbox**

- **Data**

**ATTENZIONE!** non è quindi possibile gestire all'interno di un Form
Passweb, campi custom di Puffin di tipo "Ora", "Data e Ora", "Password"
e "Campo da altra struttura"

Per maggiori informazioni relativamente a come costruire all'interno di
Passweb un form in grado di memorizzare su Puffin un'anagrafica lead si
rimanda a quanto indicato all'interno del capitolo "*Componenti Comuni
-- Componente Form -- Creazione Lead su Puffin CRM*" di questo manuale

