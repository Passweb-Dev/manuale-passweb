# UTENTI AREA RISERVATA



Tra le diverse tipologie di utenti del sito web rivestiranno,
indubbiamente, una particolare importanza quegli utenti abilitati ad
accedere anche all'Area Riservata, soprattutto nel caso in cui il sito
E-commerce sia collegato a Mexal e sia destinato alla gestione di una
rete commerciale opportunamente strutturata **(Business to Business)**.

Tali utenti, infatti, (siano essi Agenti Mexal o Clienti opportunamente
autorizzati) avranno a disposizione, in questa sezione del sito, una
serie di funzionalità, variabili in relazione alla tipologia di utente
considerata, attraverso cui poter interagire tra loro in diverse
maniere: scambiandosi messaggi, inserendo attività o appuntamenti in
agenda, scambiandosi documenti ecc ...

In questo senso, ovviamente, giocherà un ruolo determinante anche la
particolare posizione occupata dallo specifico utente all'interno della
struttura gerarchica dei gruppi e degli utenti che si è deciso di
gestire all'interno del sito.

**NOTA BENE:** per maggiori informazioni in merito alla creazione di una
struttura gerarchia di gruppi e di utenti abilitati ad accedere all'Area
Riservata di un sito E-commerce si veda anche il successivo capitolo
"Gruppi Utenti Sito" di questo manuale.

Verranno ora analizzate più nel dettaglio le diverse tipologie di utenti
abilitati ad accedere all'Area Riservata di un sito E-commerce
evidenziando anche le funzionalità messe a disposizione per ciascuna di
queste tipologie da questa particolare sezione del sito.

##### TIPOLOGIA UTENTI AREA RISERVATA

Gli utenti abilitati ad accedere all'Area Riservata di un sito
E-commerce possono essere suddivisi in due grandi macrocategorie:

- Utenti di tipo **Agente**: sono **Agenti Mexal** correttamente
  esportati e gestiti anche all'interno del sito web. Tale tipologia di
  utenti è presente ovviamente solo nel caso di siti Ecommerce collegati
  a Mexal.

- Utenti di tipo **Cliente Area Riservata**: sono utenti registrati al
  sito E-commerce ed opportunamente abilitati ad accedere all'Area
  Riservata

A seconda della tipologia dello specifico utente, potranno essere
disponibili o meno, all'interno dell'Area Riservata, determinate
funzionalità.

Di seguito vengono indicate le caratteristiche e le funzionalità
disponibili per ciascuna delle due diverse possibili tipologie di utenza
sopra indicate.

In generale varranno comunque sempre le regole secondo cui:

- il livello di comunicazione di un utente (con chi cioè l'utente in
  esame può o non può comunicare, scambiando messaggi, documenti ecc ...
  ) dipende dal suo gruppo di appartenenza, dalle particolari
  impostazioni settate per questo stesso gruppo e, ovviamente, dalla
  posizione in cui tale gruppo viene collocato all'interno della
  struttura gerarchica.

- le funzionalità disponibili per un utente (il fatto ad esempio che un
  Agente Mexal possa accedere ai documenti di tutti i suoi clienti o
  effettuare ordini per essi) dipendono dalla particolare tipologia di
  utente considerata.

###### UTENTI DI TIPO "AGENTE"

Come detto gli utenti dell'Area Riservata di un sito E-commerce di tipo
**Agente** altro non sono se non Agenti codificati in Mexal
correttamente esportati e gestiti anche all'interno del sito.

**Per poter consentire quindi ad un Agente Mexal di accedere all'Area
Riservata del sito E-commerce collegato al gestionale (realizzando di
fatto un sito di tipo B2B) è sufficiente esportare questo stesso Agente
all'interno del sito impostando per esso il campo Passweb "Trasferisci
sul sito" sul valore S ed assegnandogli, ovviamente, una login ed una
password di accesso. (campi Passweb "Login:Utente" e "Login:Password")**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\accesso_agenti.bmp](./assets/media/image105.png){width="4.50625in"
height="1.8375in"}

> **NOTA BENE:** dopo aver impostato per un Agente il campo Passweb
> "Trasferisci sul sito" a S, sarà necessario lanciare una
> sincronizzazione per consentire di fatto l'esportazione di questo
> utente all'interno del sito.

Nel momento in cui, dunque, un Agente correttamente esportato andrà ad
autenticarsi sul sito, utilizzando le credenziali di accesso che gli
sono state assegnate in Mexal, verrà automaticamente ricondotto al
pannello dell'Area Riservata, dove avrà a disposizioni diverse
funzionalità coerenti con il suo ruolo di Agente.

In particolare un utente di tipo **Agente** accedendo all'Area Riservata
del sito E-commerce collegato a Mexal avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi di tipo Agente o
  Cliente Area Riservata) appartenenti a gruppi utente figli del gruppo
  cui esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchica; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni utente di tipo **Agente** avrà la
  possibilità di inviare messaggi ad utenti appartenenti a gruppi padre
  del gruppo cui esso appartiene e collocati quindi ad un livello più
  alto della struttura gerarchica, anche in questo caso sia a livello di
  messaggi inviati al singolo utente che a livello di messaggi inviati
  ad interi gruppi utente.

**NOTA BENE:** a livello di scambio messaggi la comunicazione tra utenti
di pari livello, appartenenti quindi allo stesso gruppo potrà avvenire
unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente nella
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comunicazione_livello_superiore.bmp](./assets/media/image106.png){width="5.792361111111111in"
height="3.422222222222222in"}

- Inserire attività, scadenze o appuntamenti nella propria agenda, nelle
  agende condivise, e in quelle di utenti (siano essi di tipo Agente o
  Cliente Area Riservata) appartenenti a gruppi figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchica (questo sia a livello di singolo utente che a
  livello di interi gruppi utente) .

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati ad un qualsiasi altro
  utente (sia esso di tipo Agente o Cliente Area Riservata) appartenente
  a gruppi figli del gruppo cui esso appartiene e collocati quindi ad un
  livello più basso della struttura gerarchica; questo sia a livello di
  singolo utente che a livello di interi gruppi utente. Allo stesso modo
  ogni utente di tipo **Agente** avrà la possibilità di creare cartelle
  all'interno delle quali inserire poi documenti destinati ad utenti
  appartenenti a gruppi padre del gruppo cui esso appartiene e collocati
  quindi ad un livello più alto della struttura gerarchica, anche in
  questo caso sia a livello di singolo utente che a livello di interi
  gruppi utente.

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente nella
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Gestire i propri clienti Mexal oltre che i clienti di eventuali
  sottoagenti, ossia di altri utenti di tipo Agente collocati ad un
  livello più basso della struttura gerarchica. In particolare per
  ciascuno di questi clienti un Agente avrà la possibilità di:

  - Autenticarsi come lo specifico cliente effettuando per esso degli
    ordini (utilizzando quindi le esatte condizioni commerciali definite
    in Mexal per lo specifico cliente)

  - Visualizzare gli ordini/bolle/fatture relativi allo specifico
    cliente

  - Visualizzare le risorse memorizzate in Docuvision per lo specifico
    cliente (documenti anagrafici e/o documenti relativi a movimenti di
    magazzino)

  - Visualizzare la situazione contabile dello specifico cliente in
    relazione ad un eventuale stato di fuori fido

> **NOTA BENE:** per informazioni più dettagliate relativamente alle
> modalità di inserimento messaggi, di inserimento attività ecc ... si
> rimanda alla sezione "Business to Business -- Area Riservata" di
> questo manuale.

Tenendo conto di quanto detto fino ad ora, e principalmente del fatto
che il livello di comunicazione di un utente dipende dal suo gruppo di
appartenenza e dalla posizione in cui tale gruppo viene collocato
all'interno della struttura gerarchica, **occorre fare particolare
attenzione nel momento in cui si andrà a definire la struttura
gerarchica dei gruppi e degli utenti che andrà poi a regolare le
comunicazioni in Area Riservata** a livello di scambio messaggio,
inserimento attività, scadenze o appuntamenti in agenda e scambio di
generici documenti (NON Docuvision).

**In particolare occorrerà prestare particolare attenzione a collocare
al di sotto del gruppo di appartenenza di un certo Agente solamente quei
Clienti Mexal che lo stesso agente può effettivamente gestire anche
all'interno del gestionale**, in modo tale da non correre il rischio che
questo stesso agente possa vedere e/o comunicare (inviando ad esempio
messaggi) anche con clienti che in realtà non potrebbe gestire in Mexal.

**In ogni caso un'eventualità di questo tipo è limitata alle sole
funzionalità di messaggistica, di agenda appuntamenti e di scambio di
generici documenti.**

**Relativamente alla possibilità di effettuare ordini per un certo
cliente e/o di consultare i documenti Docuvision o la situazione
contabile di questi stessi clienti, infatti, varranno sempre soltanto le
associazioni Agente -- Cliente realizzate in Mexal.**

In conseguenza di ciò un Agente potrà effettuare ordini, consultare i
documenti Docuvision o la situazione contabile unicamente per quei
clienti che sono stati ad esso associati in Mexal o che, sempre in
Mexal, sono stati associati ad Agenti collocati, nella gerarchia
definita in Passweb, ad un livello più basso rispetto a quello di
appartenenza dell'Agente in esame (indipendentemente dunque da eventuali
utenti di tipo Cliente Area Riservata che sono stati specificatamente
collocati ad un livello più basso della gerarchia).

###### UTENTI DI TIPO "CLIENTI AREA RISERVATA"

Come precedentemente evidenziato gli utenti dell'Area Riservata di un
sito E-commerce di tipo **Cliente Area Riservata** altro non sono se non
utenti registrati al sito E-commerce ed opportunamente abilitati ad
accedere all'Area Riservata.

Tale abilitazione è gestita diversamente a seconda del fatto di
considerare un sito Ecommerce collegato a Mexal oppure ad uno dei
gestionali Ho.Re.Ca.

**[E-COMMERCE MEXAL]{.underline}**

Per i siti Ecommerce collegati a Mexal l'abilitazione per l'accesso in
Area Riservata da parte di uno specifico cliente è gestita attraverso il
parametro "**Abilita all'area Riservata**" presente all'interno del
gestionale (per maggiori informazioni in merito si veda anche la sezione
"*Configurazione Gestionale -- Mexal Parametri Configurazione Gestionale
-- Mexal Attivazione Passweb -- Funzionalità Mexal Clienti --
Abilitazione Accesso Area Riservata"* di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\abilita_ar_cliente_mexal.bmp](./assets/media/image107.png){width="5.0in"
height="1.9868055555555555in"}

**In queste condizioni dunque per poter consentire ad un Cliente Mexal
di accedere all'Area Riservata del sito E-commerce non sarà sufficiente
esportarlo all'interno del sito, ma occorrerà anche impostare per esso
il campo Passweb "Abil. Area Riservata" sul valore S.**

**[E-COMMERCE HO.RE.CA.]{.underline}**

Per i siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.
l'abilitazione per l'accesso in Area Riservata da parte di uno specifico
cliente è gestita invece all'interno del Wizard di Passweb mediante il
campo "**Tipologia**" presente nell'anagrafica Passweb dello specifico
utente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\cliente_area_riservata.bmp](./assets/media/image108.png){width="5.785416666666666in"
height="4.467361111111111in"}

**In queste condizioni dunque per poter consentire ad un Cliente dei
gestionali Ho.Re.Ca. di accedere all'Area Riservata del sito Ecommerce,
non è sufficiente esportarlo e gestirlo all'interno del sito, ma
occorrerà anche impostare per esso il campo "Tipologia" della sua
Anagrafica Passweb sul valore "Cliente Area Riservata"**

**ATTENZIONE!** Considerando che, per ogni utente, la possibilità di
accedere o meno in Area Riservata viene decisa, in ogni caso,
dall'amministratore all'interno del gestionale o all'interno del Wizard,
è chiaro che **un nuovo utente appena registrato non potrà mai**
**entrare immediatamente** **in Area Riservata** ma dovrà sempre
attendere la sua abilitazione da parte dell'amministratore

Una volta ottenuta questa abilitazione, entrando poi in Area Riservata
l'utente avrà la possibilità di:

- Inviare messaggi a tutti gli utenti (siano essi di tipo Agente o
  Cliente Area Riservata) appartenenti a gruppi utente figli del gruppo
  cui esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchica; questo sia a livello di messaggi inviati al
  singolo utente che a livello di messaggi inviati ad interi gruppi
  utente. Allo stesso modo ogni utente di tipo **Cliente Area
  Riservata** avrà la possibilità di inviare messaggi ad utenti
  appartenenti a gruppi padre del gruppo cui esso appartiene e collocati
  quindi ad un livello più alto della struttura gerarchica, anche in
  questo caso sia a livello di messaggi inviati al singolo utente che a
  livello di messaggi inviati ad interi gruppi utente.

**NOTA BENE:** a livello di scambio messaggi la comunicazione tra utenti
di pari livello, appartenenti quindi allo stesso gruppo potrà avvenire
unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente nella
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio messaggi la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comunicazione_livello_superiore.bmp](./assets/media/image106.png){width="5.792361111111111in"
height="3.422222222222222in"}

- Inserire attività, scadenze o appuntamenti nella propria agenda, nelle
  agende condivise, e in quelle di utenti (siano essi di tipo Agente o
  Cliente Area Riservata) appartenenti a gruppi figli del gruppo cui
  esso appartiene e collocati quindi ad un livello più basso della
  struttura gerarchica (questo sia a livello di singolo utente che a
  livello di interi gruppi utente).

**NOTA BENE:** a livello di inserimento attività scadenze o appuntamenti
in agenda la comunicazione tra utenti di pari livello, appartenenti
quindi allo stesso gruppo potrà avvenire unicamente nel caso in cui, per
il gruppo in esame, sia stato selezionato il parametro **"Comunicazione
interna"** presente nella maschera di configurazione dello specifico
gruppo.

- Creare cartelle con permessi di Lettura/Scrittura/Modifica all'interno
  delle quali inserire poi documenti destinati ad un qualsiasi altro
  utente (sia esso di tipo Agente o Cliente Area Riservata) appartenente
  a gruppi figli del gruppo cui esso appartiene e collocati quindi ad un
  livello più basso della struttura gerarchica; questo sia a livello di
  singolo utente che a livello di interi gruppi utente. Allo stesso modo
  ogni utente di tipo **Cliente Area Riservata** avrà la possibilità di
  creare cartelle all'interno delle quali inserire poi documenti
  destinati ad utenti appartenenti a gruppi padre del gruppo cui esso
  appartiene e collocati quindi ad un livello più alto della struttura
  gerarchica, anche in questo caso sia a livello di singolo utente che a
  livello di interi gruppi utente.

**NOTA BENE:** a livello di scambio documenti la comunicazione tra
utenti di pari livello, appartenenti quindi allo stesso gruppo potrà
avvenire unicamente nel caso in cui, per il gruppo in esame, sia stato
selezionato il parametro **"Comunicazione interna"** presente nella
maschera di configurazione dello specifico gruppo.

**NOTA BENE:** a livello di scambio documenti la comunicazione verso i
singoli utenti di gruppi collocati ad un livello gerarchico più alto,
potrà avvenire unicamente nel caso in cui, per il gruppo in esame, sia
stato selezionato il parametro **"Comunicazione Utenti Livello
Superiore"** presente all'interno della maschera di configurazione dello
specifico gruppo. Nel caso in cui tale parametro non sia stato
selezionato la comunicazione con gruppi collocati ad un livello
gerarchico più alto potrà avvenire solo a livello di interi gruppi.

- Visualizzare il dettaglio dei propri documenti (ordini, bolle, fatture
  , resi merce ecc...)

- Visualizzare le proprie risorse memorizzate in Docuvision (documenti
  anagrafici e/o documenti relativi a movimenti di magazzino)

> **NOTA BENE:** per informazioni più dettagliate relativamente alle
> modalità di inserimento messaggi, di inserimento attività ecc ... si
> rimanda alla sezione "Business to Business -- Area Riservata" di
> questo manuale.

