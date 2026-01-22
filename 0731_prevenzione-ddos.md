# PREVENZIONE DDOS



La pagina "**Gestione DDos**" consente di attivare e configurare le
regole per il blocco applicativo di eventuali richieste indesiderate in
arrivo sul proprio sito, stabilendo anche se tali regole dovranno agire
sulla base dell'indirizzo ip e/o dello user agent associato alla singola
richiesta

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_4.bmp](./assets/media/image273.png){width="5.571527777777778in"
height="3.422222222222222in"}

Nello specifico la sezione:

- "**Generale**" consente di attivare / disattivare la funzione di
  blocco automatico delle richieste indesiderate e di impostare i
  parametri che andranno a definire le condizioni necessarie per far
  scattare un determinato blocco

- "**Configurazione User -- Agent**" consente di attivare eventuali
  blocchi sulla base dello user agent delle richieste in arrivo al sito

- "**Configurazione Richieste IP**" consente di attivare eventuali
  blocchi sulla base dell'indirizzo ip delle richieste in arrivo al sito

Per maggior informazioni relativamente alle singole sezioni presenti in
questa pagina del Wizard e ai relativi parametri di configurazione si
rimanda a quanto indicato nei successivi capitoli di questo manuale.

Una volta impostati i parametri necessari a definire delle condizioni di
blocco, sarà poi necessario cliccare sul pulsante "Salva" posto nella
parte bassa della pagina per salvare le configurazioni impostate e,
successivamente, sul pulsante "**Applica le regole impostate**" in
maniera tale da rendere effettivamente attive tali regole

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_5.bmp](./assets/media/image274.png){width="5.707638888888889in"
height="3.4479166666666665in"}

**ATTENZIONE!** **Il pulsante "Salva" consente di salvare i parametri
settati all'interno di questa pagina ma non di applicare le relative
regole. In conseguenza di ciò per attivare tali regole è indispensabile
cliccare anche sul pulsante "Applica le regole impostate".**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_6.bmp](./assets/media/image275.png){width="5.707638888888889in"
height="3.4479166666666665in"}

**ATTENZIONE!** l'applicazione delle regole di blocco causerà, come
indicato dal relativo messaggio, un riciclo del pool del sito e sarà
quindi necessario effettuare nuovamente l'autenticazione al Wizard

Altra cosa di fondamentale importanza da tenere sempre in considerazione
è che, come precedentemente evidenziato, le eventuali regole di blocco
definite all'interno di questa sezione agiranno a livello applicativo.
Ciò significa, dunque, che **tutti i blocchi applicati e i relativi
contatori attivati a seguito di ban temporanei e / o di eventuali Long
ban saranno strettamente collegati al processo del sito.**

In conseguenza di ciò, **nel momento in cui si dovesse verificare un
riciclo del pool del sito**, **cosa questa che potrebbe avvenire
automaticamente a seguito di un certo periodo di inattività e/o a
seguito dell'applicazione di determinate configurazioni del sito** (come
può essere la stessa applicazione delle regole di blocco definite
all'interno di questa sezione) **tutti i blocchi temporanei
eventualmente attivi verranno eliminati e, allo stesso modo, verranno
resettati anche tutti i contatori di ban temporanei e / o di log ban
precedentemente attivati.**

