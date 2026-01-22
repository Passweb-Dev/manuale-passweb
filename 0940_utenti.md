# UTENTI



**Gli utenti "Passweb" sono tutti gli utenti abilitati ad accedere
all'ambiente di sviluppo di Passweb (Wizard) per modificare e variare,
secondo lo schema di permessi ad essi associato, contenuti e
configurazioni del sito web.**

All'interno di Passweb è quindi possibile impostare le azioni e i
permessi che le diverse tipologie di utenza possono avere relativamente
alla costruzione e alla gestione del proprio sito web.

In questo senso Passweb consente di gestire **2 diverse tipologie di
Ruolo:**

- **Amministratore**

- **Utente**

ciascuna delle quali definisce i permessi che i singoli utenti
appartenenti allo specifico Ruolo, potranno avere all'interno del
Wizard.

**ATTENZIONE! E' possibile creare più Ruoli della stessa tipologia,
assegnando a ciascuno di essi un diverso schema di permessi**

In maniera più precisa dunque ogni Ruolo consente di definire, **per
tutti gli utenti ad esso appartenenti**:

- le funzionalità dell'applicazione che potranno essere utilizzate;

- le classi di componenti gestibili;

- le possibili azioni (modifica, editing, creazione ecc ... ) sui
  componenti che sono abilitati a gestire;

- le pagine cui potranno accedere;

- le azioni che potranno effettuare sulle pagine che sono abilitati a
  gestire;

Le due diverse tipologie di Ruolo gestite in Passweb sono organizzate
secondo una struttura gerarchica ad albero dove, al livello più alto, è
collocata la tipologia Ruolo **Amministratore,** che non sarà quindi
sottoposta a limitazioni di alcun tipo.

La tipologia ruolo **"Utente"** viene collocata invece al secondo
livello di questa struttura gerarchica e sarà quindi sottoposta alle
eventuali limitazioni impostate per essa dagli utenti appartenenti alla
tipologia Amministratore.

In generale varranno quindi le seguenti regole:

Tipologia Ruolo **Amministratore**:

- non è sottoposta ad alcun tipo di limitazione;

- non può modificare il proprio schema di permessi;

- può definire uno specifico schema di permessi da associare alla
  tipologia Ruolo **Utente**;

- può creare un nuovo Ruolo di tipo **Amministratore o Utente;**

- può inserire utenti all'interno delle tipologie Ruolo
  **Amministratore** e **Utente**.

- può modificare le impostazione del Ruolo **Amministratore** e
  **Utente** in relazione alle statistiche visualizzabili nella
  Dashboard del Wizard

Tipologia Ruolo **Utente**:

- è sottoposta alle limitazioni definite dallo schema di permessi ad
  essa associato dagli utenti di tipo **Amministratore**;

- non può modificare il proprio schema di permessi;

- può creare un nuovo Ruolo di tipo **Utente**

- può inserire utenti all'interno della tipologia Ruolo **Utente**.

- può modificare le impostazione del Ruolo **Utente** in relazione alle
  statistiche visualizzabili nella Dashboard del Wizard

La maschera "**Gestione Ruoli**" visibile accedendo alla sezione
"*Utenti -- Utenti Passweb - Utenti*" del Wizard

![](./assets/media/image1.png)

consente di visualizzare e gestire i Ruoli attualmente codificati
all'interno del proprio ambiente di sviluppo.

**ATTENZIONE! A default in ogni sito Passweb è presente un Ruolo di tipo
Amministratore ed uno di tipo Utente. I Ruoli creati a default
dall'applicativo sono evidenziati in grassetto**

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in corrispondenza del campo "Nome Ruolo", consente di filtrare
i dati in griglia sulla base dei valori presenti all'interno della
relativa colonna.

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

**Aggiungi Ruolo** (
![](./assets/media/image2.png) ): consente di aggiungere un nuovo
Ruolo. Cliccando su questo pulsante verrà quindi visualizzata la
maschera "Nuovo Ruolo"

![](./assets/media/image3.png)

All'interno della sezione "**Generale**" è possibile indicare un valore
per i seguenti parametri:

- **Nome:** consente di assegnare un nome al Ruolo che si sta
  codificando

- **Descrizione:** consente di assegnare una specifica descrizione al
  Ruolo che si sta codificando

- **Tipologia:** consente di definire, selezionandola dal relativo menu
  a tendina, la tipologia di Ruolo che si sta codificando. In questo
  senso la possibilità di creare nuovi Ruoli di tipo Amministratore o
  Utente dipende esattamente da chi sta creando il nuovo Ruolo. Nello
  specifico:

  - Utenti appartenenti ad un Ruolo di tipo Amministratore avranno la
    possibilità di creare Ruoli sia di tipo Amministratore che di tipo
    Utente

  - Utenti appartenenti ad un Ruolo di tipo Utente avranno invece la
    possibilità di creare unicamente nuovi Ruoli di tipo Utente

**ATTENZIONE! Una volta definita Tipologia, Nome e Descrizione questi
non potranno più essere modificati**

La sezione "**Dashboard**" consente invece di decidere quali dati
statistici potranno o meno essere visualizzati, per gli utenti
appartenenti al Ruolo in esame, nella Dashboard del Wizard (per maggiori
informazioni relativamente a questi dati statistici si veda quanto
indicato nel relativo capitolo di questo manuale)

In particolare il parametro:

**Ordini** (solo siti Ecommerce, Comodati e Connettori): consente, se
attivato, di visualizzare nella Dashboard del Wizard i dati relativi a:

- Totale Vendite

- Numero Ordini

- Valore Medio Ordini

- Ultimi 10 Ordini

- Articoli più Visti

- Articoli più Venduti

- Clienti

**Ordini Marketplace** (siti Ecommerce, Comodati e Connettori):
consente, se attivato, di visualizzare nella Dashboard del Wizard i dati
relativi a:

- Numero Ordini Marketplace

**Pagamenti** (siti Ecommerce, Comodati e Connettori): consente, se
attivato, di visualizzare nella Dashboard del Wizard i dati relativi a:

- Pagamento più utilizzato

**Trasporti** (siti Ecommerce, Comodati e Connettori): consente, se
attivato, di visualizzare nella Dashboard del Wizard i dati relativi a:

- Trasporto più utilizzato

**Resi** (siti Ecommerce, Comodati e Connettori): consente, se attivato,
di visualizzare nella Dashboard del Wizard i dati relativi a:

- Numero Resi

**Carrelli abbandonati** (siti Ecommerce e Comodati): consente, se
attivato, di visualizzare nella Dashboard del Wizard i dati relativi a:

- Numero Carrelli Abbandonati

- Valore Carrelli Abbandonati

**Visite** (siti Ecommerce, Comodati, Commercialista, Partner, Passweb):
consente, se attivato, di visualizzare nella Dashboard del Wizard i dati
relativi a:

- Statistiche in tempo reale

- Visitatori

- Tasso di Conversione

**Clienti** (siti Ecommerce e Comodati): consente, se attivato, di
visualizzare nella Dashboard del Wizard i dati relativi a:

- Clienti Abituali

**Importi** (siti Ecommerce, Comodati e Connettori): consente di
definire la tipologia degli importi che verranno poi visualizzati nelle
statistiche relative a "Ordini" e "Carrelli Abbandonati". E' possibile
selezionare una delle seguenti opzioni:

- **Totale**: selezionando questa opzione le statistiche relative ad
  Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Ordine**" e il "**Totale Carrello**"

- **Totale Merce**: selezionando questa opzione le statistiche relative
  ad Ordini e Carrelli Abbandonati mostreranno, rispettivamente, il
  "**Totale Merce Ordine**" e il "**Totale Merce Carrello**"

**Gestione Iva** (siti Ecommerce, Comodati e Connettori): consente di
indicare come dovrà essere gestita l'IVA nelle statistiche presenti
nella Dashboard del Wizard. E' possibile selezionare una delle seguenti
opzioni:

- **Ivato**: selezionando questa opzione nelle statistiche della
  Dashboard del Wizard verranno visualizzati importi Ivati

- **Non Ivato**: selezionando questa opzione nelle statistiche della
  Dashboard del Wizard verranno visualizzati importi non Ivati

**ATTENZIONE!** nel momento in cui dovessero essere variate delle
impostazioni per il Ruolo cui appartiene l'utente attualmente connesso,
sarà necessario effettuare logout e login per poter visualizzare le
modifiche apportate

Il pulsante "**Salva**" presente nella parte bassa della maschera
consente di salvare i dati impostati creando di fatto il nuovo Ruolo

**Modifica Ruolo** (
![](./assets/media/image4.png) ): consente di modificare, per il Ruolo attualmente
selezionato, le impostazioni relative ai dati statistici che gli utenti
potranno poi visualizzare nella Dashboard del Wizard.

Cliccando su questo pulsante verrà quindi visualizzata la maschera
"**Modifica Ruolo**"

![](./assets/media/image5.png)

all'interno della quale poter modificare i parametri della sezione
"Dashboard" precedentemente analizzata

**Elimina Ruolo** (
![](./assets/media/image6.png) ): visibile solo nel caso in cui il Ruolo selezionato
in elenco non sia uno di quelli Standard presenti a default in ogni sito
Passweb.

Consente di eliminare il Ruolo attualmente selezionato in elenco.

**ATTENZIONE! l'eliminazione di un Ruolo comporta, ovviamente, anche la
rimozione di tutti gli utenti legati a quello stesso ruolo**

**Gestisci gli Utenti per questo Ruolo** (
![](./assets/media/image7.png) ): consente di definire gli utenti appartenenti al
Ruolo attualmente selezionato in elenco.

Cliccando su questo pulsante verrà quindi visualizzata la maschera
**"Lista Utenti Ruolo -- Nome Ruolo"**

![](./assets/media/image8.png)

all'interno della quale verrà visualizzato l'elenco di tutti gli utenti
attualmente associati al Ruolo in oggetto.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

- **Nuovo Utente** (
  ![](./assets/media/image9.png) ): consente di creare un nuovo utente
  da associare alla tipologia di Ruolo in oggetto.

- **Modifica Utente**
  (![](./assets/media/image10.png) ) : consente di modificare
  l'anagrafica dell'utente attualmente selezionato.

- **Elimina Utente**
  (![](./assets/media/image11.png) ) : consente di eliminare l'anagrafica
  dell'utente attualmente selezionato.

**Modifica Permessi**
(![](./assets/media/image12.png) ): consente di definire lo schema di permessi da
associare al Ruolo attualmente selezionato

**NOTA BENE**: non è possibile modificare lo schema di permessi del
Ruolo a cui si appartiene.

Cliccando su questo pulsante verrà quindi visualizzata la maschera
**"Gestione Ruolo Utente"**

![](./assets/media/image13.png)

attraverso la quale poter definire lo schema di permessi da associare
alla tipologia ruolo in oggetto. Tale maschera è suddivisa in due
distinte sezione:

- **Permessi del Wizard**: consente di impostare le azioni che tutti gli
  utenti appartenenti al Ruolo in esame potranno o non potranno
  effettuare all'interno del Wizard

- **Permessi sulle Pagine:** consente di definire le specifiche pagine
  cui potranno o non potranno avere accesso, all'interno del Wizard,
  tutti gli utenti appartenenti al Ruolo in esame

