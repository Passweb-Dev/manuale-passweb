# CONFIGURAZIONE USER AGENT



La sezione "**Configurazione User Agent**" consente di attivare
eventuali regole di blocco sulla base dello user agent delle richieste
in arrivo al sito

![](./assets/media/image281.png)

**ATTENZIONE!** Lo User Agent è un campo del protocollo HTTP tramite il
quale possono essere date delle informazioni più o meno approfondite
riguardo al dispositivo che effettua la richiesta della pagina web.

In sostanza dunque analizzando lo user agent di una richiesta in arrivo
al sito si può capire se tale richiesta proviene da un browser come
Chrome, Firefox, Safari ... , se arriva da qualche tool che in maniera
più o meno lecita sta tentando di visitare il sito, se è una richiesta
mal formata (e quindi probabilmente malevola) perché manca proprio di
user agent ecc...

Il problema in tutto ciò è rappresentato dal fatto che mascherare lo
user agent di una richiesta web per farla sembrare quella di un browser
tradizionale è un'operazione piuttosto semplice e, generalmente, è anche
la prima cosa che fanno i tool di scraping o di chi tenta di scansionare
il web solo per prendere dati o causare problemi.

Non è assolutamente detto dunque che una richiesta che si presenta come
buona a livello di user agent (perché magari utilizza esattamente lo
stesso user agent di Chrome) sia effettivamente tale per cui un primo
meccanismo di difesa che si può adottare e quello di cercare di capire
se la frequenza di questo tipo di richieste possa o meno essere
assimilabile a visite umane o no e, in quest'ultimo caso, bloccarle.

Oltre a questo poi esistono anche una miriade di software o servizi che
scansionano continuamente il web, anche con degli user agent noti e
riconducibili proprio a specifici servizi che possono essere lanciati
volutamente dagli amministratori del sito per fare, ad esempio, degli
audit SEO ma che possono anche scansionare il sito ad insaputa
dell'amministratore (e soprattutto senza curarsi di farlo in maniera
tale da non causare danni) semplicemente per acquisire informazioni da
inserire nei loro database.

In questo senso nel box di sinistra della sezione "Configurazione User
Agent" è riportato un elenco di user agent di questo tipo e
riconducibili a servizi più o meno noti (per maggiori informazioni in
merito a questi user agent, a cosa fanno, a quale sia il servizio ad
essi collegato e soprattutto a come questi dovrebbero comportarsi in
merito ad eventuali direttive fornite mediante file robots.txt).

Per poter attivare dunque delle regole di blocco relative a richieste
collegabili ad uno o più di questi user agent e che rispondano sempre ai
parametri precedentemente impostati all'interno della sezione
"Generale", sarà sufficiente:

- Attivare il parametro "**Abilita**"

- Selezionare uno o più user agent tra quelli presenti nel box di
  sinistra e spostarli in quello di destra cliccando sul pulsante
  raffigurante una piccola freccia verde.

Allo stesso modo nel momento in cui l'esigenza dovesse essere quella di
escludere degli user agent dall'applicazione delle regole automatiche di
blocco delle richieste sarà sufficiente selezionarli dal box di destra
ed inserirli nuovamente in quello di sinistra cliccando sul pulsante
raffigurante una piccola freccia rossa.

**ATTENZIONE!** le regole di blocco definite all'interno della sezione
"Configurazione User Agent" verranno prese in considerazione solo nel
caso in cui entrambi i parametri "**Abilita**" (presente all'interno di
questa stessa sezione) e "**Abilita Prevenzione DDos**" siano stati
correttamente attivati

Allo stesso modo si ricorda anche che per poter rendere immediatamente
attive tali regole non è sufficiente cliccare sul pulsante Salva
presente nella parte bassa della maschera ma occorre anche cliccare sul
pulsante "Applica le regole impostate"

