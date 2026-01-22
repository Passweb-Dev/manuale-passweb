# TIPOLOGIE UTENTI AREA RISERVATA



Gli utenti abilitati ad accedere all'Area Riservata di un sito web
"Commercialista" possono essere suddivisi, come precedentemente
accennato, in due grandi macro categorie: **Utenti Passcom** ed **Utenti
NON Passcom**.

- **Utenti Passcom:** sono gli utenti definiti direttamente all'interno
  del gestionale. Tali utenti saranno quindi presenti unicamente nel
  caso in cui il sito sia collegato ad un installazione di Passcom e la
  loro gestione, sia a livello di abilitazione all'accesso all'Area
  Riservata del sito web sia a livello di definizione della tipologia
  utente è interamente demandata al gestionale.

> **NOTA BENE:** non è possibile eliminare o creare nuovi Utenti
> Passcom, indipendentemente dalla loro tipologia, direttamente
> all'interno del Wizard di Passweb.
>
> Considerata dunque la forte integrazione col gestionale, per gli
> Utenti Passcom saranno disponibili, una volta effettuata
> l'autenticazione, funzionalità aggiuntive rispetto a quelle
> disponibili invece per gli Utenti NON Passcom.
>
> È possibile creare per questi utenti un'intera gerarchia in maniera
> completamente automatica importandola direttamente dal gestionale. Per
> poter far ciò occorre agire attraverso il parametro **"Crea gerarchia
> Utenti Passcom"** presente alla pagina **"Parametri di
> Configurazione"** del Wizard.
>
> Selezionando questo parametro, verrà infatti creata alla successiva
> sincronizzazione, la gerarchia automatica di PassWeb per gli Utenti
> Passcom prelevando tutto ciò che serve per realizzare tale gerarchia
> (gruppi, utenti, legami "gruppo padre -- gruppo figlio" ecc...)
> direttamente da Passcom (vedi anche pagina "Gerarchia Utenti Passcom"
> di questo manuale).
>
> È comunque possibile, non selezionando il parametro in esame,
> importare dal gestionale i soli utenti, senza dover dunque
> necessariamente creare la gerarchia automatica, in modo tale da poter
> poi inserire gli Utenti Passcom all'interno di una qualsiasi altra
> gerarchia liberamente creata.

- **Utenti NON Passcom:** sono gli utenti definiti direttamente
  all'interno di Passweb attraverso la relativa maschera di creazione
  Nuovo Utente.

> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_nuovo_utente.bmp](./assets/media/image242.png)
>
> Tali utenti potranno quindi essere presenti indipendentemente dal
> fatto che il sito sia collegato o meno ad un'installazione di Passcom
> e la loro gestione, sia a livello di abilitazione all'accesso all'Area
> Riservata del sito web sia a livello di definizione della tipologia
> utente è interamente demandata al Wizard di Passweb.
>
> **NOTA BENE:** gli Utenti NON Passcom possono essere creati o
> eliminati partendo unicamente dal Wizard di Passweb.

È possibile collocare tali utenti all'interno di una qualsiasi gerarchia
sia essa liberamente creata sia essa la gerarchia automatica di Passweb
per gli Utenti Passcom. In ogni caso per gli Utenti NON Passcom non
verranno mai attivate le funzionalità strettamente correlate
all'integrazione col gestionale.

All'interno di ognuna delle due macro categorie sopra indicate è inoltre
possibile distinguere tre differenti tipologie di utente in relazione
alle quali potranno essere attive o meno determinate funzionalità
dell'area riservata:

- utenti di tipo **COMMERCIALISTA;**

- utenti di tipo **DIPENDENTE;**

- utenti di tipo **AZIENDA.**

**ATTENZIONE!** la tipologia utente verrà utilizzata anche come classe
CSS assegnata al tag body della pagina nel momento in cui un determinato
utente dovesse effettuare l'autenticazione al sito

Grazie a queste classi, volendo, sarà quindi possibile applicare
determinate regole CSS in base alla specifica tipologia di utenza
attualmente loggata sul sito.

Nello specifico verranno gestite le seguenti classi CSS:

- **commercialista**: assegnata al tag body nel momento in cui l'utente
  loggato sul sito dovesse essere un **utente di tipo Commercialista**

- **dipendente**: assegnata al tag body nel momento in cui l'utente
  loggato sul sito dovesse essere un **utente di tipo Dipendente**

- **azienda**: assegnata al tag body nel momento in cui l'utente loggato
  sul sito dovesse essere un **utente di tipo Azienda**

Di seguito verrà fornita una descrizione specifica delle caratteristiche
e delle particolarità di ciascuna delle tre tipologie di utente sopra
indicate.

##### UTENTI PASSCOM

Gli Utenti Passcom sono tutti quegli utenti definiti direttamente
all'interno del gestionale. Tali utenti saranno presenti quindi
unicamente nel caso in cui il sito sia collegato ad un installazione di
Passcom e la loro gestione, sia a livello di abilitazione all'accesso
all'Area Riservata del sito web sia a livello di definizione della
tipologia utente è interamente demandata al gestionale.

**NOTA BENE:** non è possibile eliminare o creare nuovi Utenti Passcom,
indipendentemente dalla loro tipologia, partendo dal Wizard di Passweb.

Considerata dunque la forte integrazione col gestionale, per gli Utenti
Passcom saranno disponibili, una volta effettuata l'autenticazione,
funzionalità aggiuntive rispetto a quelle disponibili invece per gli
Utenti NON Passcom. Tali funzionalità potranno inoltre variare a seconda
della particolare tipologia di Utente Passcom che si sta considerando.

Di seguito vengono indicate le caratteristiche e le funzionalità
disponibili per ciascuna delle tre diverse possibili tipologie di Utente
Passcom (COMMERCIALISTA, DIPENDENTE, AZIENDA).

**ATTENZIONE!** anche per gli Utenti Passcom la tipologia verrà
utilizzata anche come classe CSS assegnata al tag body della pagina nel
momento in cui un determinato utente dovesse effettuare l'autenticazione
al sito

Nello specifico verranno gestite le seguenti classi CSS:

- **cliente**: assegnata al tag body nel momento in cui l'utente loggato
  sul sito dovesse essere un **utente di tipo Cliente** (non abilitato
  ad accedere in area riservata)

  - **privato**: assegnata al tag body nel momento in cui l'utente
    loggato sul sito dovesse essere un **utente di tipo Cliente
    Privato**

  - **azienda**: assegnata al tag body nel momento in cui l'utente
    loggato sul sito dovesse essere un **utente di tipo Cliente
    Azienda**

  - **agente**: assegnata al tag body nel momento in cui l'utente
    loggato sul sito dovesse essere un **Agente**

  - **clienteareariservata**: assegnata al tag body nel momento in cui
    l'utente loggato sul sito dovesse essere **un utente di tipo Cliente
    abilitato ad accedere in Area Riservata**

  - **contatto**: assegnata al tag body nel momento in cui l'utente
    loggato sul sito dovesse essere un **utente di tipo Contatto**

In generale vale comunque sempre la regola secondo cui:

- il livello di comunicazione di un utente (con chi cioè l'utente in
  esame può o non può comunicare) dipende dal suo gruppo di appartenenza
  e dalla posizione in cui tale gruppo viene collocato all'interno della
  struttura gerarchica dei gruppi e degli utenti gestita all'interno del
  sito;

- le funzionalità disponibili per un utente (il fatto ad esempio di
  poter accedere ai Documenti Docuvision) dipendono dalla particolare
  tipologia di utente.

###### UTENTI PASSCOM DI TIPO [COMMERCIALISTA]{.underline}

Gli Utenti Passcom di tipo COMMERCIALISTA sono rappresentati da tutti
gli utenti che fanno parte di quel particolare gruppo definito in
Passcom e con nome uguale a quello specificato nel campo **"Gruppo del
Gestionale dei Commercialisti"** presente alla pagina **"Parametri di
Configurazione"** del Wizard (vedi anche sezione "CONFIGURAZIONE -
Parametri Configurazione" di questo manuale).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gerarchia_utenti_passcom_1.bmp](./assets/media/image243.png)

Per poter definire questa tipologia di utenti occorre dunque, per prima
cosa, creare attraverso le apposite funzioni di servizio uno specifico
gruppo di utenti chiamato, ad esempio, DOTTCOMM:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gerarchia_utenti_1.comm.bmp](./assets/media/image244.png)

All' interno di questo gruppo andranno quindi inseriti tutti gli quegli
utenti che, per il sito web, dovranno essere considerati come Utenti
Passcom di tipo COMMERCIALISTA:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gerarchia_utenti_2.comm.bmp](./assets/media/image245.png)

Per maggiori informazioni relativamente alla creazione di gruppi e
utenti in Passcom si rimanda all'apposito manuale.

Lato Passweb occorrerà invece indicare all'interno del campo **"Gruppo
Passcom dei Commercialisti"** presente alla pagina **"Parametri di
Configurazione"** del Wizard, il nome del gruppo appena definito
all'interno del gestionale:

**NOTA BENE:** per poter garantire il corretto funzionamento delle
operazioni di sincronizzazione tra il sito ed il gestionale è di
fondamentale importanza creare, lato gestionale, un gruppo
"Commercialista". Nel caso in cui tale gruppo non venga creato le
operazioni di sincronizzazione tra sito e gestionale potranno non
terminare correttamente.

**NOTA BENE:** l'utente amministratore di Passcom, verrà inserito
automaticamente tra gli utenti del gruppo "Commercialista".

Una volta completate queste due operazioni e terminata la realizzazione
del sito, una semplice sincronizzazione consentirà all'applicazione di
leggere gli utenti presenti all'interno del "Gruppo Commercialista"
appena dichiarato dando loro, quindi, la possibilità di accedere
all'area riservata del sito con tutti i permessi relativi ad un Utente
Passcom di tipo COMMERCIALISTA.

**NOTA BENE:** l'accesso all'area riservata del sito web per questa
tipologia di utente, avviene esattamente con le stesse credenziali di
accesso al gestionale. La gestione di tali credenziali (Login e
Password) è quindi demandata interamente a Passcom e alle relative
funzioni di servizio.

**NOTA BENE:** un Utente Passcom di tipo COMMERCIALISTA,
indipendentemente dall'eventuale elenco di aziende vietate/consentite
specificato all'interno del gestionale (nell'apposito campo delle chiavi
di accesso), avrà comunque accesso sempre a tutte le aziende gestite
all'interno del sito potendo quindi inviare loro messaggi, inserire loro
delle attività in agenda oltre che consultarne i documenti memorizzati
all'interno di Docuvision.

In particolare dunque un Utente Passcom di tipo COMMERCIALISTA accedendo
al sito avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente Passcom di tipo COMMERCIALISTA
  avrà la possibilità di inviare messaggi ad utenti appartenenti a
  gruppi padre del gruppo cui esso appartiene e collocati quindi ad un
  livello più alto della struttura gerarchica, anche in questo caso sia
  a livello di messaggi inviati al singolo utente che a livello di
  messaggi inviati ad interi gruppi utente;

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione interna"** presente alla
> maschera di configurazione dello specifico gruppo.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_gruppo_passcom.bmp](./assets/media/image246.png)

**NOTA BENE:** il gruppo automatico **Dottore Commercialista** nasce a
default con i parametri "Comunicazione tra utenti" e "Gestione SMS"
selezionati e conseguentemente con le relative funzionalità abilitate.

- Inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente;

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare Cartelle Template;

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati ad un qualsiasi altro
  utente (sia esso Passcom o NON Passcom) appartenente a gruppi figli
  del gruppo cui esso appartiene e collocati quindi ad un livello più
  basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente Passcom di tipo COMMERCIALISTA avrà la possibilità di creare
  cartelle all'interno delle quali inserire poi documenti destinati ad
  utenti appartenenti a gruppi padre del gruppo cui esso appartiene e
  collocati quindi ad un livello più alto della struttura gerarchica,
  anche in questo caso sia a livello di singolo utente che a livello di
  interi gruppi utente;

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente alla
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Consultare on-line i documenti memorizzati all'interno di Docuvision
  per un qualsiasi Utente Passcom di tipo AZIENDA, indipendentemente dal
  suo gruppo di appartenenza e dalla sua conseguente collocazione
  all'interno della struttura gerarchica.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc ... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

###### UTENTI PASSCOM DI TIPO DIPENDENTE

Gli Utenti Passcom di tipo DIPENDENTE sono rappresentati dagli utenti
facenti parte di un qualsiasi gruppo definito in Passcom e con nome
diverso da quello specificato nel campo **"Gruppo del Gestionale dei
Commercialisti"** presente alla pagina **"Parametri di Configurazione"**
del Wizard.

Per poter definire questa tipologia di utenti occorre dunque, per prima
cosa, creare attraverso le apposite funzioni di servizio un gruppo di
utenti con nome diverso da quello utilizzato per identificare gli Utenti
Passcom di tipo COMMERCIALISTA.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gerarchia_utenti_4.comm.bmp](./assets/media/image247.png)

Occorrerà quindi associare a questo gruppo un' insieme di aziende da
poter gestire e ovviamente occorrerà inserire al suo interno tutti gli
quegli utenti che, per il sito web, dovranno essere considerati come
Utenti Passcom di tipo DIPENDENTE.

Una volta completata questa operazione e terminata la realizzazione del
sito, una semplice sincronizzazione consentirà all'applicazione di
leggere gli utenti presenti all'interno dei vari gruppi definiti nelle
chiavi di accesso del gestionale dando loro, quindi, la possibilità di
accedere all'area riservata del sito con tutti i permessi relativi ad un
Utente Passcom di tipo DIPENDENTE .

**NOTA BENE:** l'accesso all'area riservata del sito web per questa
tipologia di utente, avviene esattamente con le stesse credenziali di
accesso al gestionale. La gestione di tali credenziali (Login e
Password) è quindi demandata interamente a Passcom e alle relative
funzioni di servizio.

Mentre un Utente Passcom di tipo COMMERCIALISTA, come detto, ha sempre
la possibilità di accedere a tutte le aziende gestite all'interno del
sito, un Utente Passcom di tipo DIPENDENTE potrà invece gestire,
all'interno del sito web, solamente quelle aziende che gli sono state
assegnate all'interno del gestionale.

In particolare dunque un Utente Passcom di tipo DIPENDENTE accedendo al
sito avrà la possibilità di:

- inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente Passcom di tipo DIPENDENTE avrà
  la possibilità di inviare messaggi ad utenti appartenenti a gruppi
  padre del gruppo cui esso appartiene e collocati quindi ad un livello
  più alto della struttura gerarchica, anche in questo caso sia a
  livello di messaggi inviati al singolo utente che a livello di
  messaggi inviati ad interi gruppi utente;

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione interna"** presente alla
> maschera di configurazione dello specifico gruppo.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_gruppo_passcom.bmp](./assets/media/image246.png)

**NOTA BENE:** il gruppo automatico **Dipendenti** nasce a default con i
parametri "Comunicazione tra utenti" e "Gestione SMS" selezionati e
conseguentemente con le relative funzionalità abilitate.

- inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente;

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati ad un qualsiasi altro
  utente (sia esso Passcom o NON Passcom) appartenente a gruppi figli
  del gruppo cui esso appartiene e collocati quindi ad un livello più
  basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente Passcom di tipo DIPENDNENTE avrà la possibilità di creare
  cartelle all'interno delle quali inserire poi documenti destinati ad
  utenti appartenenti a gruppi padre del gruppo cui esso appartiene e
  collocati quindi ad un livello più alto della struttura gerarchica,
  anche in questo caso sia a livello di singolo utente che a livello di
  interi gruppi utente;

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente alla
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Consultare on-line i documenti memorizzati all'interno di Docuvision
  per i soli Utenti Passcom di tipo AZIENDA che è abilitato a gestire,
  ed indipendentemente dal loro gruppo di appartenenza e dalla loro
  conseguente collocazione all'interno della struttura gerarchica.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc ... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

###### UTENTI PASSCOM DI TIPO AZIENDA

Gli Utenti Passcom di tipo AZIENDA sono rappresentati dalle aziende
dell'installazione Passcom opportunamente abilitate ad accedere all'Area
Riservata del sito web.

Per poter definire, dunque, questa tipologia di utenti occorre
selezionare all'interno di Passcom l'azienda in esame, accedere alla
maschera "*Dati Aziendali (F4 da "Anagrafica Azienda") -- Configurazione
Moduli -- Collegamento sito commercialista*" qui di seguito riportata:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_sito_19-a.comm.bmp](./assets/media/image248.png)

e impostare il valore del parametro "Stato" ad **Attivato.**

> **NOTA BENE:** il parametro **"Stato"** è unico per tutte le sotto
> aziende eventualmente gestite. Ciò significa dunque che variando il
> valore del parametro per una sotto azienda la modifica verrà
> automaticamente propagata anche a tutte le altre sotto aziende.

In questo modo a partire dalla prossima sincronizzazione l'azienda in
esame verrà inserita tra le aziende "Gestite" all'interno del sito web e
avrà, quindi, la possibilità di accedere all'area riservata del sito con
tutti i permessi relativi ad un Utente Passcom di tipo AZIENDA.

Relativamente alle credenziali che questa tipologia di utente dovrà poi
utilizzare per accedere in area riservata vanno distinti due casi (la
discriminante è la possibilità da parte di questi utenti di accedere o
meno anche al gestionale):

a)  Utenti di tipo AZIENDA identificativi di aziende dell'installazione
    che **NON hanno la possibilità di accedere via predesk al
    gestionale**;

> In queste condizioni l'accesso all'area riservata dovrà essere
> effettuato utilizzando le credenziali inserite all'interno dei campi
> Login e Password presenti nella maschera *Collegamento sito
> commercialista* precedentemente analizzata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_sito_19-b.comm.bmp](./assets/media/image249.png)

> **ATTENZIONE!** Oltre ad attivare l'azienda per l'esportazione sul
> sito, sarà necessario, prima di eseguire la sincronizzazione,
> assicurarsi di aver valorizzato anche i campi Login e Password
>
> Una volta effettuato l'accesso questi utenti avranno comunque la
> possibilità di modificare la propria login e/o la propria password
> agendo per questo dall'apposito box presente, in Area Riservata, nella
> pagina di gestione del proprio Profilo.
>
> Se necessario, per questa tipologia di utenti, è possibile reimpostare
> le credenziali di accesso al sito agendo direttamente all'interno del
> gestionale.
>
> Per effettuare questo tipo di operazione è sufficiente, accedere alla
> maschera "Dati Aziendali (F4 da "Anagrafica Azienda") --
> *Configurazione Moduli -- Collegamento sito commercialista*" ed
> impostare il valore del parametro "Stato" sul valore **Reimposta**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_sito_19-c.comm.bmp](./assets/media/image250.png)

> In questo modo i campi Login e Password verranno automaticamente
> impostati sui seguenti valori:
>
> **LOGIN = CODICE FISCALE**
>
> **PASSWORD = PARTITA IVA (COMPRENSIVA DI IT)**
>
> In questo modo a partire dalla prossima sincronizzazione l'utente in
> esame potrà accedere al sito come utilizzando come login e password,
> rispettivamente, quanto inserito nei campi Codice Fiscale e Partita
> IVA (comprensiva di IT) dell'anagrafica azienda di Passcom.
>
> **ATTENZIONE!** Nel caso in cui si desideri resettare le credenziali
> di accesso in area riservata, utilizzando dei valori diversi da Codice
> Fiscale e Partita IVA sarà necessario, dopo aver impostato il
> parametro Stato su R, specificare questi valori all'interno dei
> rispettivi campi.

**NOTA BENE:** il valore R ha effetto unicamente per aziende che fanno
parte di gruppi Studio. Nel caso in cui, infatti, un'azienda
appartenesse ad un gruppo "Utenti Azienda AlwaysON/AutoON", l'accesso
all'area riservata del sito web avverrebbe con le stesse credenziali
definite per l'accesso al gestionale.

b)  Utenti di tipo AZIENDA identificativi di aziende dell'installazione
    Passcom che **hanno la possibilità di accedere via predesk al
    gestionale**.

> In queste condizioni l'accesso all'area riservata del sito web avviene
> esattamente con le stesse credenziali di accesso al gestionale. La
> gestione di tali credenziali (Login e Password) è quindi demandata
> interamente alle relative funzioni di servizio.

Un Utente Passcom di tipo AZIENDA accedendo al sito avrà la possibilità
di:

- Inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente Passcom di tipo AZIENDA avrà la
  possibilità di inviare messaggi ad utenti appartenenti a gruppi padre
  del gruppo cui esso appartiene e collocati quindi ad un livello più
  alto della struttura gerarchica, anche in questo caso sia a livello di
  messaggi inviati al singolo utente che a livello di messaggi inviati
  ad interi gruppi utente.

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro il parametro **"Comunicazione interna"**
> presente alla maschera di configurazione dello specifico gruppo.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_gruppo_passcom.bmp](./assets/media/image246.png)

- inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente;

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati a tutti gli utenti (siano
  essi Utenti Passcom o Utenti NON Passcom) appartenenti a gruppi utente
  figli del gruppo cui esso appartiene e collocati quindi ad un livello
  più basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente Passcom di tipo AZIENDA avrà la possibilità di creare cartelle
  all'interno delle quali inserire poi documenti destinati ad utenti
  appartenenti a gruppi padre del gruppo cui esso appartiene e collocati
  quindi ad un livello più alto della struttura gerarchica, anche in
  questo caso sia a livello di singolo utente che a livello di interi
  gruppi utente.

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato **"Comunicazione interna"** presente alla maschera di
configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Consultare on-line i propri documenti memorizzati all'interno di
  Docuvision.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc ... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

##### UTENTI NON PASSCOM

Gli Utenti NON Passcom sono tutti quegli utenti definiti direttamente
all'interno del Wizard di Passweb attraverso la relativa maschera di
creazione Nuovo Utente.

Per poter creare e gestire utenti di questo tipo occorre agire dalla
relativa sezione, accessibile dal Menu Principale di Passweb attraverso
la voce *"Utenti -- Utenti Sito".*

All'interno di questa sezione verrà infatti visualizzata la maschera
"**Lista Utenti"** precedentemente analizzata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_utenti_NOBP_2.comm.bmp](./assets/media/image223.png)

e attraverso cui poter visualizzare e gestire le anagrafiche di tutti
gli utenti abilitati ad accedere all'Area Riservata del sito web.

Attraverso questa pagina sarà quindi possibile creare nuovi utenti **NON
Passcom**, ricercare uno specifico utente, visualizzarne l'anagrafica ed
eventualmente associarlo ad uno o più gruppi opportunamente creati.

**NOTA BENE:** per maggiori informazioni in merito si veda anche al
sezione "Utenti -- Utenti Sito -- Utenti" di questo manuale.

Di seguito vengono indicate le caratteristiche e le funzionalità
disponibili per ciascuna delle tre diverse possibili tipologie di Utente
NON Passcom (COMMERCIALISTA, DIPENDENTE, AZIENDA).

**NOTA BENE:** considerando gli utenti NON Passcom non hanno nulla a che
vedere col gestionale, verranno a mancare per essi alcune delle
funzionalità, disponibili invece per gli Utenti Passcom, all'interno
dell'Area Riservata del sito web..

In generale vale comunque sempre la regola secondo cui:

- il livello di comunicazione di un utente (con chi cioè l'utente in
  esame può o non può comunicare) dipende dal suo gruppo di appartenenza
  e dalla posizione in cui tale gruppo viene collocato all'interno della
  struttura gerarchica dei gruppi e degli utenti gestita all'interno del
  sito;

- le funzionalità disponibili per un utente dipendono dalla particolare
  tipologia di utente**.**

###### UTENTI NON PASSCOM DI TIPO COMMERCIALISTA

Gli Utenti NON Passcom di tipo COMMERCIALISTA sono tutti quegli utenti
definiti all'interno di Passweb attraverso l'apposita maschera di
creazione Nuovo Utente e per i quali il parametro **"Tipologia"** è
stato impostato sul valore **Commercialista.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_utente_NOBP1.bmp](./assets/media/image251.png)

**NOTA BENE:** una volta confermata l'anagrafica, la tipologia
dell'utente non potrà più essere modificata.

Accedendo all'Area Riservata del sito web, un Utente NON Passcom di tipo
AMMINISTRATORE avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente NON Passcom di tipo
  COMMERCIALISTA avrà la possibilità di inviare messaggi ad utenti
  appartenenti a gruppi padre del gruppo cui esso appartiene e collocati
  quindi ad un livello più alto della struttura gerarchica, anche in
  questo caso sia a livello di messaggi inviati al singolo utente che a
  livello di messaggi inviati ad interi gruppi utente.

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo, potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione interna"** presente alla
> maschera di configurazione dello specifico gruppo.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente.

> **NOTA BENE:** a livello di inserimento attività scadenze o
> appuntamenti in agenda la comunicazione tra utenti di pari livello,
> appartenenti quindi allo stesso gruppo potrà avvenire unicamente nel
> caso in cui, per il gruppo in esame, sia stato selezionato il
> parametro **"Comunicazione interna"** presente nella maschera di
> configurazione dello specifico gruppo.

- Creare Cartelle Template.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati a tutti gli utenti (siano
  essi Utenti Passcom o Utenti NON Passcom) appartenenti a gruppi utente
  figli del gruppo cui esso appartiene e collocati quindi ad un livello
  più basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente NON Passcom di tipo COMMERCIALISTA avrà la possibilità di
  creare cartelle all'interno delle quali inserire poi documenti
  destinati ad utenti appartenenti a gruppi padre del gruppo cui esso
  appartiene e collocati quindi ad un livello più alto della struttura
  gerarchica, anche in questo caso sia a livello di singolo utente che a
  livello di interi gruppi utente.

> **NOTA BENE:** a livello di scambio documenti la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione interna"** presente alla
> maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

###### UTENTI NON PASSCOM DI TIPO DIPENDENTE

Gli Utenti NON Passcom di tipo DIPENDENTE sono tutti quegli utenti
definiti all'interno di PassWeb attraverso l'apposita maschera di
creazione Nuovo Utente e per i quali il parametro **"Tipologia"** è
stato impostato sul valore **Dipendente.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_utente_NOBP1a.bmp](./assets/media/image252.png)

**NOTA BENE:** una volta confermata l'anagrafica, la tipologia
dell'utente non potrà più essere modificata.

Accedendo all'Area Riservata del sito web, un Utente NON Passcom di tipo
DIPENDENTE avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente NON Passcom di tipo DIPENDENTE
  avrà la possibilità di inviare messaggi ad utenti appartenenti a
  gruppi padre del gruppo cui esso appartiene e collocati quindi ad un
  livello più alto della struttura gerarchica, anche in questo caso sia
  a livello di messaggi inviati al singolo utente che a livello di
  messaggi inviati ad interi gruppi utente.

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione tra utenti"**.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente.

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati a tutti gli utenti (siano
  essi Utenti Passcom o Utenti NON Passcom) appartenenti a gruppi utente
  figli del gruppo cui esso appartiene e collocati quindi ad un livello
  più basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente Passcom di tipo DIPENDNENTE avrà la possibilità di creare
  cartelle all'interno delle quali inserire poi documenti destinati ad
  utenti appartenenti a gruppi padre del gruppo cui esso appartiene e
  collocati quindi ad un livello più alto della struttura gerarchica, in
  questo caso però non a livello di singolo utente ma soltanto a livello
  di interi gruppi utente

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente alla
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc ... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

###### UTENTI NON PASSCOM DI TIPO AZIENDA

Gli Utenti NON Passcom di tipo AZIENDA sono tutti quegli utenti definiti
all'interno di Passweb attraverso l'apposita maschera di creazione Nuovo
Utente e per i quali il parametro **"Tipologia"** è stato impostato sul
valore **Azienda.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_utente_NOBP1b.bmp](./assets/media/image253.png)

**NOTA BENE:** una volta confermata l'anagrafica, la tipologia
dell'utente non potrà più essere modificata.

Accedendo all'Area Riservata del sito web, un Utente NON Passcom di tipo
AZIENDA avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi Utenti Passcom o
  Utenti NON Passcom) appartenenti a gruppi utente figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchia; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni Utente Passcom di tipo AZIENDA avrà la
  possibilità di inviare messaggi ad utenti appartenenti a gruppi padre
  del gruppo cui esso appartiene e collocati quindi ad un livello più
  alto della struttura gerarchica, anche in questo caso sia a livello di
  messaggi inviati al singolo utente che a livello di messaggi inviati
  ad interi gruppi utente.

> **NOTA BENE:** a livello di scambio messaggi la comunicazione tra
> utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
> avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
> selezionato il parametro **"Comunicazione interna"** presente alla
> maschera di configurazione dello specifico gruppo.
>
> **NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
> singoli utenti di gruppi collocati ad un livello gerarchico più alto,
> potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
> stato selezionato il parametro **"Comunicazione Utenti Livello
> Superiore"** presente all'interno della maschera di configurazione
> dello specifico gruppo. Nel caso in cui tale parametro non sia stato
> selezionato la comunicazione con gruppi collocati ad un livello
> gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Inserire attività o scadenze nella propria agenda oltre che in quella
  di utenti (siano essi Utenti Passcom o Utenti NON Passcom)
  appartenenti a gruppi utente figli del gruppo cui esso appartiene e
  collocati quindi ad un livello più basso della struttura gerarchia;
  questo sia a livello di singolo utente che a livello di interi gruppi
  utente.

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati a tutti gli utenti (siano
  essi Utenti Passcom o Utenti NON Passcom) appartenenti a gruppi utente
  figli del gruppo cui esso appartiene e collocati quindi ad un livello
  più basso della struttura gerarchia; questo sia a livello di singolo
  utente che a livello di interi gruppi utente. Allo stesso modo ogni
  Utente Passcom di tipo AZIENDA avrà la possibilità di creare cartelle
  all'interno delle quali inserire poi documenti destinati ad utenti
  appartenenti a gruppi padre del gruppo cui esso appartiene e collocati
  quindi ad un livello più alto della struttura gerarchica, in questo
  caso però non a livello di singolo utente ma soltanto a livello di
  interi gruppi utente.

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro il parametro **"Comunicazione interna"**
presente alla maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

Per informazioni più dettagliate relativamente alle modalità di
inserimento messaggi, di inserimento attività ecc ... si rimanda alla
sezione "Struttura Sito - Area Riservata" di questo manuale.

