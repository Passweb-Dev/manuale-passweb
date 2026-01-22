# MATOMO



Matomo ( [[https://matomo.org/]{.underline}](https://matomo.org/) )
precedentemente noto come Piwik, è un software di web analytics open
source sviluppato in php su database MySQL che rappresenta, ad oggi, una
delle migliori alternative a Google Analytics.

Attualmente è utilizzato su oltre un milione di siti Web in più di 190
paesi ed è anche è il software scelto dalla Pubblica Amministrazione
italiana per il progetto Web Analytics Italia per la tutela della
privacy dei cittadini utilizzatori di siti pubblici.

La sezione "**Matomo**" del tab "**Tracciamento Dati**" consente quindi
di impostare tutti i parametri di configurazione necessari per attivare
il tracciamento del proprio sito Passweb mediante questa piattaforma di
web analytics.

![](./assets/media/image197.png)

**ATTENZIONE!** Matomo è uno strumento di web analytics che offre
diverse possibilità di configurazione e di gestione e che può essere
integrato nativamente con i siti Passweb attraverso l'impostazione di
semplici parametri ma rimane comunque un software di terze parti
indipendente da Passweb che richiede, al fine di poter essere utilizzato
al meglio in tutte le sue funzionalità, specifiche conoscenze tecniche.

All'interno di questo manuale è presente un'apposita sezione (*Matomo*)
per approfondire un po\' le conoscenze e l'utilizzo di questo strumento
avendo comunque sempre ben chiaro che lo scopo del presente manuale
**non è** **quello di offrire una guida completa all'utilizzo e alla
configurazione di Matomo.** Nel momento in cui l'esigenza dovesse essere
quella di approfondire ulteriormente questo argomento si consiglia
quindi di fare sempre riferimento alla documentazione ufficiale
disponibile a partire dai seguenti link

- Sito ufficiale di Matomo --
  [[https://matomo.org]{.underline}](https://matomo.org)

- Documentazione Matomo --
  [[https://matomo.org/guides/]{.underline}](https://matomo.org/guides/)

- Forum Matomo --
  [[https://forum.matomo.org/]{.underline}](https://forum.matomo.org/)

Fatta questa doverosa considerazione passiamo ora ad analizzare nel
dettaglio i diversi parametri che consentono di attivare e configurare
il collegamento diretto tra il proprio sito Passweb e Google Analytics.

**Codice di tracciamento:** consente di inserire lo snippet di codice
necessario per attivare il tracciamento lato client di Matomo,
tracciamento questo che verrà quindi effettuato via javascript con
l'installazione di determinati cookie sul browser dei visitatori.

Lo snippet di codice in questione potrà essere prelevato direttamente
dalla propria installazione Matomo all'interno della pagina "**Siti Web
-- Codice di Tracciamento**"

![](./assets/media/image198.png)

**ATTENZIONE!** A differenza di quello che avviene nell'integrazione
Passweb -- Google Analytics dove è sufficiente inserire l'Id di
monitoraggio, nell'integrazione Passweb -- Matomo **è necessario
inserire invece tutto lo snippet di codice**

In conseguenza di ciò, nel momento in cui, successivamente
all'inserimento in Passweb del codice di tracciamento, dovessero essere
abilitate, in Matomo, determinate opzioni (es. tracciamento dello user
id, gestione dei consensi built-in ...) che comportano anche una
modifica a questo stesso codice, sarà ovviamente necessario aggiornare
allo stesso modo anche il codice di tracciamento presente su Passweb.

**ATTENZIONE** Il codice di tracciamento evidenziato in figura consente
di gestire, inoltre, un tracciamento "standard" che riguarda
essenzialmente le sole visite alle diverse pagine del sito.

Nel momento in cui l'esigenza dovesse essere quella di gestire anche un
tracciamento ecommerce e/o le ricerche interne al sito sarà quindi
necessario (oltre ad aver attivato le relative funzionalità in fase di
configurazione del sito su Matomo) selezionare anche i due parametri
"**Abilita Tracciamento Ecommerce**" e "**Abilita Tracciamento
Ricerca**"

**Abilita Tracciamento Ecommerce**: consente, se selezionato di inviare
a Matomo, nelle varie fasi dell'esperienza di acquisto dell'utente sul
nostro sito, informazioni dettagliate relativamente ai prodotti che
l'utente ha visualizzato, a quelli attualmente in carrello e ad
eventuali ordini conclusi con successo. Nello specifico attivando il
parametro in esame verranno tracciati ed inviati a Matomo i seguenti
eventi:

- Visualizzazione Prodotto

- Aggiornamento Carrello

- Acquisto

Per maggiori informazioni relativamente alla gestione degli eventi
ecommerce e ai dati effettivamente tracciati assieme a tali eventi si
veda anche quanto indicato all'interno del capitolo "*Matomo --
Integrazione Passweb Matomo -- Monitoraggio Ecommerce*" di questo
manuale

**Abilita Tracciamento Ricerca**: consente, se selezionato, di inviare a
Matomo anche alcuni dati sulle ricerche effettuate dagli utenti
all'interno del sito ( posto ovviamente che per effettuare queste
ricerche siano stati utilizzati i componenti nativi di Passweb ).

Per maggiori informazioni relativamente alla gestione degli eventi di
ricerca e ai dati effettivamente tracciati assieme a tali eventi si veda
anche quanto indicato all'interno del capitolo "*Matomo -- Integrazione
Passweb Matomo -- Monitoraggio Ecommerce - Ricerca*" di questo manuale

**Abilita Tracciamento Server:** consente, se selezionato, di attivare,
in merito all'acquisizione di nuovi ordini, il tracciamento lato server
di Matomo.

Per maggiori informazioni in merito alla possibilità di sfruttare,
nell'ambito dell'integrazione Passweb -- Matomo, il tracciamento lato
server si veda anche quanto indicato all'interno del capitolo "*Matomo
-- Integrazione Passweb Matomo -- Tracciamento lato server*" di questo
manuale

**Dominio Matomo Server**: visibile solo nel caso in cui il precedente
parametro "**Abilita Tracciamento Server**" sia stato correttamente
selezionato.

Consente di indicare il dominio (privo del protocollo utilizzato e
quindi senza http o https) assegnato alla propria installazione Matomo
(in questo senso è consigliabile utilizzare un sottodominio del dominio
principale in uso al sito Passweb)

**Id Sito**: visibile solo nel caso in cui il precedente parametro
"**Abilita Tracciamento Server**" sia stato correttamente selezionato.

Consente di indicare l'Id assegnato da Matomo al sito che si intende
monitorare. Tale identificativo viene assegnato direttamente in fase di
configurazione del sito stesso su Matomo e può essere visualizzato
portandosi all'interno della pagina "Siti Web -- Amministrazione"
(parametro ID evidenziato in figura)

![](./assets/media/image199.png)

**ATTENZIONE!** "Id Sito" e "Dominio Matomo Server" sono parametri
obbligatori. Nel momento in cui uno di essi dovesse essere impostato in
maniera non corretta non sarà possibile attivare il tracciamento lato
server

**Utilizza User Id:** visibile solo nel caso in cui il precedente
parametro "**Abilita Tracciamento Server**" sia stato correttamente
selezionato.

Consente di inviare a Matomo, anche in relazione al tracciamento lato
server, lo User Id aumentando quindi l'accuratezza dei dati tracciati.
Attivando questo parametro infatti anche le transazioni tracciate lato
server potranno essere legate ad uno specifico utente e verranno quindi
inserite, su Matomo, all'interno della scheda anagrafica dell'utente
stesso. In questo senso, ovviamente, è richiesto il tracciamento dello
User Id anche lato Client

**ATTENZIONE!** Si ricorda che per il GDPR lo User Id viene trattato a
tutti gli effetti come un'informazione di identificazione personale
(PII) e questo anche nel momento in cui dovesse essere utilizzata, come
User Id, una generica stringa alfanumerica e/o si dovesse ricorrere alle
funzioni di anonimizzazione messe a disposizione da Matomo.

In conseguenza di ciò nel momento in cui si dovesse decidere di attivare
e gestire anche questo tipo di tracciamento sarà necessario, da una
parte, fornire nelle Norme sulla gestione della privacy del proprio sito
un'informativa adeguata circa l'utilizzo degli identificatori utilizzati
e, dall'altra parte, verificare di aver gestito in maniera corretta la
richiesta di consenso preventivo come effettivamente richiesto dal GDPR

