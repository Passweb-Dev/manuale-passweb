# GESTIONE NEWSLETTER -- CAMPAGNE



All'interno di questa sezione l'utente avrà la possibilità di creare e
gestire delle Campagne per l'invio di Newsletter sfruttando, in questo
senso, le liste di iscritti ed i template precedentemente sincronizzati
da MailChimp e appositamente configurati.

La maschera "**Gestione Newsletter -- Gestione Campagne**" consente
visualizzare l'elenco di tutte le Campagne attualmente create e che
possono essere utilizzate per inviare delle Newsletter.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_campagne.bmp](./assets/media/image77.png)

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Crea Campagna** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_campagna.bmp](./assets/media/image78.png) ): consente di creare una nuova
Campagna.

Cliccando su questo pulsante verrà infatti visualizzata la maschera di
creazione di una nuova campagna

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_campagna2.bmp](./assets/media/image79.png)

all'interno della quale poter indicare:

- **Nome:** consente di associare un nome identificativo alla Campagna
  che si sta realizzando

- **Tipologia della Campagna:** consente di definire la tipologia della
  Campagna che si sta codificando. E' possibile selezionare uno dei
  seguenti valori:

  - **Semplice:** una "Campagna Semplice" è una Campagna in cui tutti i
    contenuti della Newsletter dovranno essere inseriti, in fase di
    invio della campagna stessa, **ogni volta, in maniera manuale**.

  - **CMS:** una "Campagna CMS" è una Campagna in cui i contenuti della
    Newsletter (tutti o in parte) potranno essere prelevati
    automaticamente da uno dei post CMS gestiti all'interno del proprio
    sito e appositamente configurati per questo scopo.

> Per maggiori informazioni relativamente a come impostare un contenuto
> CMS, in maniera tale da poterlo collegare all'invio di una Newsletter,
> si veda anche la sezione "Sito -- Gestione CMS" di questo manuale.

- **Articolo:** una "Campagna Articolo" è una Campagna in cui i
  contenuti della Newsletter (tutti o in parte) potranno essere
  prelevati automaticamente da uno dei prodotti attualmente gestiti
  all'interno del sito.

- **Disponibilità Articolo:** le Campagne di tipo "Disponibilità
  Articolo" verranno utilizzate dal sistema di notifiche automatiche
  verso gli utenti che hanno specificatamente richiesto di essere
  avvisati nel momento in cui un determinato prodotto presente sul sito
  torni ad essere disponibile e quindi acquistabile.

> Per maggiori informazioni in merito si veda anche il capitolo
> *"Notifiche Disponibilità -- Passweb e MailChimp"* di questo manuale

- **Lista Regalo:** una "Campagna Lista Regalo" è una Campagna in cui i
  contenuti della mail verranno prelevati (tutti o in parte) dalla
  specifica Lista Regalo che l'utente ha deciso di condividere via mail

<!-- -->

- **Template:** visualizzato solo dopo aver indicato la tipologia di
  Campagna che si intende creare.

> Consente di selezionare il Template che dovrà essere utilizzato dalla
> Campagna in oggetto.
>
> **ATTENZIONE!** All'interno di questo campo verranno visualizzati solo
> ed esclusivamente i Template correttamente configurati ed
> effettivamente utilizzabili all'interno di una Campagna (quindi quelli
> in stato **"OK").**
>
> Inoltre l'elenco dei Template effettivamente selezionabili può variare
> in relazione alla Tipologia di Campagna che si sta realizzando e,
> ovviamente, in relazione alla tipologia del Template stesso.
>
> Nello specifico per:

- **Campagne Semplici:** possono essere selezionati solo ed
  esclusivamente Template di tipologia **Semplice**

- **Campagne CMS:** possono essere selezionati solo ed esclusivamente
  Template di tipologia **Semplice** o **CMS**

- **Campagne Articolo:** possono essere selezionati solo ed
  esclusivamente Template di tipologia **Semplice** o **Ecommerce**

- **Campagne Disponibilità Articolo:** possono essere selezionati solo
  ed esclusivamente Template di tipologia **Semplice** o **Ecommerce**

- **Campagne Lista Regalo:** possono essere selezionati solo ed
  esclusivamente Template di tipologia **GiftRegistry** (per Liste
  Regalo)

**Elimina Campagna** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_campagna.bmp](./assets/media/image80.png) ): consente di eliminare la campagna
attualmente selezionata in elenco.

**ATTENZIONE!** L'eliminazione di una campagna comporterà l'eliminazione
anche di tutti gli invii associati alla campagna stessa. Inoltre
eliminando una campagna da Passweb, gli invii relativi a questa campagna
verranno eliminati in modo permanente anche all'interno del proprio
account di MailChimp.

**Modifica Campagna** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_campagna.bmp](./assets/media/image81.png) ): consente di visualizzare ed
eventualmente modificare i parametri e le proprietà della Campagna
attualmente selezionata in elenco.

**Gestisci Invii per la Campagna** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_gestisci_invii_campagna.bmp](./assets/media/image82.png) ): consente di gestire gli invii per la
Campagna attualmente selezionata in elenco, decidendo se inviare le
relative Newsletter in maniera immediata o schedulata, se inviarle ad
un'intera lista piuttosto che ai soli iscritti a determinati gruppi di
interesse, o ancora, definendo i contenuti della specifica Newsletter
che dovrà essere inviata.

Cliccando su questo pulsante verrà visualizzata una griglia contenente
l'elenco di tutti gli invii attualmente codificati per la Campagna in
esame

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestisci_invii.bmp](./assets/media/image83.png)

**Per ogni Campagna è quindi possibile codificare uno o più invii
distinti.**

> **NOTA BENE**: il fatto di codificare un invio non implica
> necessariamente l'effettivo invio della relativa Newsletter. Per
> questo sarà necessario agire attraverso i pulsanti **"Crea su
> MailChimp e Invia Ora"** (per un invio immediato della relativa
> Newsletter) o **"Crea su MailChimp e Schedula invio"** (per un invio
> schedulato della relativa Newsletter)

All'interno della griglia sopra indicata dunque:

- Gli invii codificati ma non ancora effettuati avranno stato "**OK**"

- Gli invii già effettuati verranno evidenziati in verde e avranno stato
  "**Inviato**".

- Gli invii schedulati verranno invece evidenziati in giallo e avranno
  stato "**Schedulato**".

I pulsanti presenti nella barra degli strumenti della maschera di
gestione degli invii consentono rispettivamente di

- **Nuovo Invio Campagna Semplice\\CMS\\Lista Regalo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo_invio_campagna_cms.bmp](./assets/media/image84.png) ): consente di codificare un nuovo
  invio per la Campagna attualmente selezionata.

> Cliccando su questo pulsante verrà infatti visualizzata, nella parte
> bassa della maschera, un'ulteriore sezione "**Nuova Campagna in
> Uscita**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_campagna_in_uscita.bmp](./assets/media/image85.png)

> all'interno della quale impostare tutti i parametri necessari per
> l'invio che si intende codificare. In particolare sarà necessario
> impostare un valore per i seguenti parametri:

- **Nome della Campagna in Uscita:** consente di definire un nome
  identificativo per l'invio che si sta codificando

- **Oggetto della Campagna:** consente di impostare l'oggetto che dovrà
  essere utilizzato nelle mail inviate dalla campagna in esame

- **Indirizzo del mittente:** consente di impostare l'indirizzo mail che
  dovrà essere utilizzato come indirizzo del mittente nelle mail inviate
  dalla campagna in esame

- **Nome del Mittente:** consente di impostare il nome del mittente che
  verrà associato all'indirizzo indicato nel campo precedente e che
  conseguentemente verrà visualizzato nei vari client di posta
  all'interno del campo "Da"

- **Nome del destinatario:** consente di impostare un nome
  identificativo per i destinatari delle mail inviate dalla campagna in
  esame (es. "Iscritti alla Newsletter di E-Sport Store"). Tale nome
  verrà poi visualizzato nei vari client di posta all'interno del campo
  "A"

- **Attivo --solo per campagne di tipologia "Disponibilità Articolo" o
  "Lista Regalo"**

> Consente di marcare come "Attiva" la corrispondente Campagna in
> uscita.
>
> **ATTENZIONE!** Il campo "Attivo" è di fondamentale importanza in
> quanto l'invio marcato come **Attivo** è quello che verrà poi
> effettivamente utilizzato in fase di condivisione di una Lista Regalo
> e/o di notifica disponibilità
>
> **Per questa ragione è ovviamente possibile marcare come Attivo un
> solo invio alla volta.**

- **Lista a cui inviare la Campagna:** consente di selezionare la
  specifica lista di iscritti cui inviare la Newsletter relativa alla
  campagna in esame.

> In questo senso sarà possibile selezionare una qualsiasi lista tra
> quelle precedentemente sincronizzate ed importate direttamente dal
> proprio account MailChimp.
>
> Una volta selezionata una specifica lista sarà poi possibile decidere
> di inviare la Newsletter a tutti gli iscritti della lista oppure solo
> ed esclusivamente agli utenti iscritti a determinati gruppi di
> interesse associati alla lista stessa.

- **Contenuto CMS da Inviare -- solo per Campagne di tipologia CMS:**
  consente di selezionare lo specifico articolo CMS da cui dovranno
  essere prelevati i contenuti da utilizzare per popolare in automatico
  le diverse sezioni del Template utilizzato per l'invio della
  Newsletter in questione.

- **Articolo -- solo per Campagne di tipologia Ecommerce:** consente di
  selezionare lo specifico prodotto da cui prelevare i dati richiesti
  per la compilazione automatica delle apposite sezioni del template.

- **Versione Testuale (campo non obbligatorio):** consente di impostare
  una versione testuale della mail che verrà inviata con la Newsletter
  in esame. La versione testuale verrà poi visualizzata solo ed
  esclusivamente da quei client di posta che non risultino avere
  abilitata la visualizzazione delle mail ricevute in formato HTML

- **Template Newsletter:** all'interno di questa sezione sarà possibile
  impostare, in maniera definitiva, i contenuti della mail che verrà
  spedita a seguito dell'invio che si sta codificando.

> In questo senso dunque, verrà visualizzato il Template precedentemente
> selezionato ed associato alla campagna in esame con le varie sezioni
> già configurate in relazione alla tipologia di contenuto che possono
> accogliere.
>
> In particolare:

- Le sezioni impostate per acquisire automaticamente contenuti da un ben
  preciso post CMS, da un ben preciso prodotto e/o da una data Lista
  Regalo, non risulteranno essere modificabili.

- Le sezioni impostate per accogliere dei "Valori forniti da Editor"
  oppure delle "Immagini Personalizzate" presenteranno, a default, gli
  stessi valori impostati in fase di configurazione del Template. Sarà
  comunque possibile modificare e personalizzare ulteriormente questi
  contenuti. Passando infatti col mouse sopra queste sezioni, con un
  semplice click verrà aperta la relativa maschera di personalizzazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_campagna_in_uscita2.bmp](./assets/media/image86.png)

- **Compila Invio Campagna** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_compila_invio_campagna.bmp](./assets/media/image87.png) ): consente di visualizzare ed
  eventualmente modificare i parametri di configurazione dell'invio
  attualmente selezionato in elenco (gli stessi definiti in fase di
  creazione dell'invio). **Visibile solo per invii codificati ma non
  ancora effettuati o schedulati (stato "OK")**

- **Elimina Invio Campagna** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_invio_campagna.bmp](./assets/media/image88.png) ): consente di eliminare da Passweb e
  corrispondentemente anche dal proprio account MailChimp lo specifico
  invio attualmente selezionato in elenco.

Una volta definiti i parametri di configurazione dello specifico invio
che si intende realizzare, i due ulteriori pulsanti presenti nella barra
degli strumenti permetteranno di inviare immediatamente la relativa
Newsletter oppure di schedularne l'invio in un momento ben preciso.

Nello specifico dunque il pulsante

- **Crea su MailChimp e Schedula invio** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_su_mailchimp_schedula.bmp](./assets/media/image89.png) ): consente di creare all'interno di
  MailChimp la Campagna necessaria per inviare la Newsletter in esame
  posticipandone l'effettivo invio ad un orario e ad una data ben
  precise selezionabili dall'apposito Calendario.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_campagna_in_uscita3.bmp](./assets/media/image90.png)

- **Crea su MailChimp e Invia Ora** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_su_mailchimp.bmp](./assets/media/image91.png) ): consente di creare all'interno di
  MailChimp la Campagna necessaria per inviare immediatamente la
  Newsletter in esame.

> **NOTA BENE**: l'invio effettivo delle Newsletter avverrà sempre e
> comunque dai server di MailChimp

- **Crea su MailChimp e Invia test** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_test_su_mailchimp.bmp](./assets/media/image92.png) ): consente di creare all'interno di
  MailChimp la Campagna necessaria per inviare ad uno specifico
  indirizzo di test la Newsletter in esame.

> Cliccando su questo pulsante verrà infatti visualizzata un'apposita
> maschera all'interno della quale inserire l'indirizzo mail di test cui
> dovrà essere inviata la newsletter

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_campagna_test.bmp](./assets/media/image93.png)

**ATTENZIONE!** I pulsanti "**Crea su MailChimp e Schedula invio**" e
"**Crea su MailChimp e Invia Ora**" non sono disponibili per invii
legati a Campagne di tipo "Disponibilità Articolo" o "Lista Regalo".

Per queste tipologie di Campagne l'effettivo invio delle mail verrà
infatti gestito in maniera completamente automatica da parte
dell'applicazione sulla base, nel primo caso (Campagne di tipo
"Disponibilità Articolo") del momento in cui un dato articolo dovesse
tornare disponibile per l'acquisto e nel secondo caso (Campagne di tipo
"Lista Regalo") del momento in cui il creatore di una data Lista Regalo
dovesse decidere di condividerla via mail.

##### GESTIONE NEWSLETTER -- CAMPAGNA SEMPLICE

Di seguito verranno indicati in maniera puntuale i vari passi da
effettuare per configurare correttamente una "**Campagna Semplice"** e
per poter inviare, dunque, direttamente dal proprio sito Passweb delle
Newsletter con contenuti scollegati da qualsiasi articolo CMS

1.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutte le liste
    di iscritti attualmente presenti su MailChimp

2.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutti i
    template attualmente presenti nella sezione "Templates" di MailChimp

3.  Configurare in maniera corretta i template importati in maniera tale
    da poterli poi utilizzare in fase di creazione e invio della
    Campagna.

> **In particolare per ogni singola sezione del Template scelto sarà
> necessario definire il nome della sezione e, soprattutto, sarà
> necessario impostare il tipo di contenuti che dovranno essere inseriti
> all'interno della sezione stessa su** "**Valore fornito da Editor**"

4.  Codificare una nuova Campagna di tipologia "**Campagna Semplice**",
    cliccando sul corrispondente pulsante ("Aggiungi Campagna Semplice")
    e selezionando per essa il template configurato al passo 3.

5.  Codificare un nuovo invio per la Campagna indicata al punto 4
    impostando tutti i parametri di configurazione necessari (oggetto,
    mittente, lista cui inviare la Campagna ecc...) e, eventualmente,
    personalizzando rispetto ai valori di default i contenuti presenti
    nelle varie sezioni del Template associato alla Campagna

6.  Cliccare sul pulsante **Crea su MailChimp e Invia Ora** per inviare
    immediatamente la Newsletter, oppure cliccare sul pulsante **Crea su
    MailChimp e Schedula Invio** per schedulare l'invio della Newsletter
    in un ben preciso momento temporale

##### GESTIONE NEWSLETTER -- CAMPAGNA CMS

Di seguito verranno indicati in maniera puntuale i vari passi da
effettuare per configurare correttamente una "**Campagna CMS"** e per
poter inviare, dunque, direttamente dal proprio sito Passweb delle
Newsletter i cui contenuti verranno prelevati automaticamente da alcuni
post CMS gestiti e pubblicati all'interno del proprio sito Passweb

1.  Definire almeno un articolo CMS come **"Inviabile per Newsletter con
    Campagna CMS"**

2.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutte le liste
    di iscritti attualmente presenti su MailChimp

3.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutti i
    template attualmente presenti nella sezione "Templates" di MailChimp

4.  Configurare in maniera corretta i template importati in maniera tale
    da poterli poi utilizzare in fase di creazione e invio della
    Campagna. **Nello specifico almeno un Template dovrà essere di tipo
    CMS e con stato Ok**

5.  Codificare una nuova Campagna di tipologia "**CMS**" selezionando
    per essa il template configurato al passo 4.

6.  Codificare un nuovo invio per la Campagna indicata al punto 5
    impostando tutti i parametri di configurazione necessari (oggetto,
    mittente, lista cui inviare la Campagna ecc...), tra cui ovviamente
    anche lo specifico post CMS da cui prelevare i contenuti e, se
    necessario, personalizzando, rispetto ai valori di default,
    eventuali contenuti presenti nelle sezioni del Template impostate
    per accogliere dei valori forniti da Editor

7.  Cliccare sul pulsante **Crea su MailChimp e Invia Ora** per inviare
    immediatamente la Newsletter, oppure cliccare sul pulsante **Crea su
    MailChimp e Schedula Invio** per schedulare l'invio della Newsletter
    in un ben preciso momento temporale

##### GESTIONE NEWSLETTER -- CAMPAGNA ARTICOLO

Di seguito verranno indicati in maniera puntuale i vari passi da
effettuare per configurare correttamente una "**Campagna Articolo"** e
per poter inviare, dunque, direttamente dal proprio sito Passweb delle
Newsletter i cui contenuti verranno prelevati automaticamente dai dati
relativi ad uno dei prodotti gestiti all'interno del sito

1.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutte le liste
    di iscritti attualmente presenti su MailChimp

2.  Sincronizzare il sito Passweb con il proprio account MailChimp in
    maniera tale da importare all'interno del sito stesso tutti i
    template attualmente presenti nella sezione "Templates" di MailChimp

3.  Configurare in maniera corretta i template importati in maniera tale
    da poterli poi utilizzare in fase di creazione e invio della
    Campagna. **Nello specifico almeno un Template dovrà essere di tipo
    Ecommerce e con stato Ok**

4.  Codificare una nuova Campagna di tipologia "**Articolo**"
    selezionando per essa il template configurato al passo 3.

5.  Codificare un nuovo invio per la Campagna indicata al punto 4
    impostando tutti i parametri di configurazione necessari (oggetto,
    mittente, lista cui inviare la Campagna ecc...), tra cui ovviamente
    anche lo specifico prodotto cui prelevare i contenuti e, se
    necessario, personalizzando, rispetto ai valori di default,
    eventuali contenuti presenti nelle sezioni del Template impostate
    per accogliere dei valori forniti da Editor

6.  Cliccare sul pulsante **Crea su MailChimp e Invia Ora** per inviare
    immediatamente la Newsletter, oppure cliccare sul pulsante **Crea su
    MailChimp e Schedula Invio** per schedulare l'invio della Newsletter
    in un ben preciso momento temporale

##### GESTIONE NEWSLETTER -- CAMPAGNA DISPONIBILITA' ARTICOLO

Per maggiori informazioni in merito alla gestione di questa particolare
tipologia di Campagne si rimanda alla sezione "*MailChimp -- Notifiche
Disponibilità Passweb e MailChimp*" di questo manuale

##### GESTIONE NEWSLETTER -- CAMPAGNA PER LISTE REGALO

Per maggiori informazioni in merito alla gestione di questa particolare
tipologia di Campagne si rimanda alla sezione "*Varianti Sito Responsive
-- Lista Componenti Ecommerce -- Componente Lista Regalo -- Condivisione
di una Lista Regalo*" di questo manuale.

