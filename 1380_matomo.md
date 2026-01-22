# MATOMO



Matomo ( [[https://matomo.org/]{.underline}](https://matomo.org/) ),
precedentemente noto come Piwik, è un software di web analytics open
source sviluppato in php su database MySQL che rappresenta, ad oggi, una
delle migliori alternative a Google Analytics.

![Videate\\matomo_1.bmp](./assets/media/image1.png){width="5.565972222222222in"
height="3.532638888888889in"}

Attualmente è utilizzato su oltre un milione di siti Web in più di 190
paesi ed è anche è il software scelto dalla Pubblica Amministrazione
italiana per il progetto Web Analytics Italia per la tutela della
privacy dei cittadini utilizzatori di siti pubblici.

Una delle cose più importanti da considerare relativamente a Matomo
riguarda infatti la proprietà dei dati. **Con Matomo la proprietà e
l'accesso ai dati resta sotto l'esclusivo controllo di chi li
raccoglie** (generalmente il proprietario del sito) e questo grazie alle
modalità di installazione disponibili per questo software.

In questo senso infatti è possibile scegliere di installare Matomo
on-premise e gratuitamente su di un proprio server (o comunque su di un
servizio di hosting anche condiviso che offre questa possibilità, come
può essere ad esempio Aruba), oppure optare per una soluzione cloud, a
pagamento, già tutta configurata e pronta all'uso sottoscrivendo un
abbonamento mensile o annuale. In entrambe le configurazioni comunque il
proprietario del sito manterrà sempre il totale controllo dei dati
acquisiti evitando, soprattutto, di inviarli a terze parti come avviene
invece con Google Analytics o altri strumenti di analisi del traffico
web che possono anche raccogliere i dati in server europei per poi però
trasferirli negli Stati Uniti violando così quanto previsto dal GDPR.

Si ricorda infatti che i motivi principali per cui il 23 Giugno 2022 il
Garante della Privacy italiano ha dichiarato non conforme al GDPR
l'utilizzo di Google Analytics (nella versione di Universal Analytics)
sono essenzialmente due:

- da un lato i dati raccolti da Google Analytics vengono trasferiti
  negli Stati Uniti o comunque se anche raccolti in server europei
  restano in ogni caso sotto il controllo di un'azienda Americana che
  non permette un livello di protezione come quello dell'Unione europea

- dall'altro Universal Analytics può tracciare l'indirizzo IP dei
  visitatori (che è da considerarsi come un dato di identificazione
  personale) in modo completo

Se con l'introduzione di GA4 il secondo punto può anche essere
considerato sanabile, resta comunque aperto, anche nel caso di GA4, il
problema del trasferimento dei dati negli Stati Uniti, problema questo
che con Matomo invece non si pone (a patto ovviamente di non installarlo
su di un server hostato in America) sia per l'utilizzo di un server
proprietario sia perché comunque Matomo fa capo ad una società europea
tenuta quindi a rispettare tutte le normative previste dalla stessa
Unione Europea in materia di GDPR.

**ATTENZIONE! Anche Matomo andrà comunque configurato e settato in un
certo modo per poter essere effettivamente utilizzato in maniera
conforme a quanto previsto dal GDPR**

Ovviamente, in tutto ciò è sempre bene considerare anche l'altro lato
della medaglia. E' vero infatti che potendo utilizzare un server
proprietario, l'amministratore del sito avrà sempre il pieno controllo
dei dati ma, dall'altra parte, è anche vero che se poi, per qualche
ragione, dovessero verificarsi problemi di sicurezza relativamente al
server che ospita Matomo, con conseguente fuoriuscita dei dati, anche
questo tipo di responsabilità risulterebbe essere in capo
all'amministratore del sito con tutte le conseguenze del caso.

Dal punto di vista dell'usabilità Matomo si presenta come un software
piuttosto semplice e molto simile alla versione classica di Analytics
(Universal Analytics).

Utilizza ancora i concetti di pagina, hits, eventi, goal (o obiettivi)
... inoltre allo stesso modo di UA consente di monitorare:

- le visite in tempo reale

- il numero di utenti e di sessioni in un determinato periodo

- la provenienza geografica delle visite

- il Bounce Rate

- le pagine più visitate

- il dispositivo, il browser e i motori di ricerca utilizzati

- l'analisi delle conversioni

- gli eventi ecommerce (acquisti, aggiunte in carrello, prodotti più
  visti ...) mediante un set di report già preconfigurati e pronti
  all'uso

- ...

![Videate\\matomo_4.bmp](./assets/media/image2.png){width="5.565972222222222in"
height="3.532638888888889in"}

Volendo invece dare un rapido sguardo alle principali differenze
funzionali tra Analytics e Matomo, una prima cosa da prendere in
considerazione riguarda sicuramente **la mole di dati raccolti**.

Come noto infatti oltre determinate soglie, Google Analytics utilizza
procedure di campionamento dei dati per generare i report, approssimando
alcuni valori. Matomo non effettua invece nessun tipo di approssimazione
per cui i dati sono più verosimili. Ovviamente se la mole di dati da
trattare inizia ad essere importante il server che ospita Matomo e lo
strumento stesso dovranno essere configurati in un certo modo per
evitare problemi e rallentamenti nell'utilizzo quotidiano.

Un'altra differenza piuttosto interessante tra le due piattaforme
riguarda gli **strumenti per la CRO** (Conversion Rate Optimization).
Sotto questo punto di vista infatti Google Analytics non offre nessun
tipo di strumento integrato costringendo quindi gli utenti ad utilizzare
tool specifici come possono essere ad esempio Hotjar o Yandex Metrica

Matomo invece integra nativamente alcuni tra i principali strumenti
utilizzabili per ottimizzare il tasso di conversione come ad esempio:

- Le **heatmaps** (mappe di calore), in sostanza una rappresentazione
  grafica della pagina del sito con evidenziate le zone che hanno
  registrato una maggior interazione da parte degli utenti. Più un
  elemento (pulsante, link ...) viene cliccato dagli utenti più la
  corrispondente zona della pagina acquisirà un colore caldo (rosso).
  Colori più freddi (verde, azzurro, blu) indicheranno invece una minore
  attività in quella zona

![Videate\\matomo_2.bmp](./assets/media/image3.png){width="3.217361111111111in"
height="2.0722222222222224in"}

- Registrazione delle sessioni

- Funnel per seguire passo passo la user journey di ogni utente

- Form Analytics per analizzare nei dettagli il comportamento degli
  utenti sui vari form presenti all'interno del sito

- A/B Testing

- ...

Matomo inoltre è estremamente personalizzabile. Si possono creare
diverse Dashboard in modo da raggruppare i KPI a seconda delle esigenze
e le sue caratteristiche possono essere estese attraverso plugin esterni
selezionabili all'interno del marketplace presente sulla piattaforma
stessa

![Videate\\matomo_3.bmp](./assets/media/image4.png){width="5.565972222222222in"
height="3.3618055555555557in"}

Offre una certa continuità a livello di tracciamento e di gestione dello
storico considerando che, a differenza di GA4 (che come noto utilizza un
data model completamente differente da quello di Universal Analytics)
permette anche l'importazione dei dati raccolti in proprietà UA (per
maggiori informazioni in merito a come poter importare in Matomo i dati
di proprietà Universal Analytics si consiglia di fare riferimento a
quanto indicato ai seguenti link
<https://matomo.org/guide/installation-maintenance/import-google-analytics/>
<https://plugins.matomo.org/GoogleAnalyticsImporter> )

Infine la vera differenza rispetto a Google Analytics, a discapito
questa volta di Matomo, è rappresentata sicuramente dalla difficoltà a
integrare con questo strumento i servizi di Google (Google Ads, Google
Search console, Google Data studio).

Per quel che riguarda la Search Console e Google Data Studio esistono
alcune soluzioni, comunque piuttosto complesse dal punto di vista
tecnico, implementabili mediante l'utilizzo di appositi plugin.

Per quel che riguarda invece Google Ads è bene sottolineare che, a
default, gli annunci creati all'interno di questa piattaforma non
vengono monitorati e tracciati in maniera corretta da Matomo. Volendo è
comunque possibile fare in modo che ciò avvenga aggiungendo
semplicemente alcuni parametri all'URL dei vari annunci creati in Google
Ads.

Per maggiori informazioni in merito è possibile fare riferimento al
seguente indirizzo
[[https://matomo.org/blog/track-google-ads-campaigns-matomo/]{.underline}](https://matomo.org/blog/track-google-ads-campaigns-matomo/)

**ATTENZIONE!** **Ovviamente lo scopo di questo manuale non è quello di
fornire una guida dettagliata all'utilizzo di Matomo, che pur essendo
integrabile con il proprio sito Passweb rimane comunque uno strumento di
terze parti.**

Per approfondire questi argomenti e per imparare ad utilizzare questo
tipo di strumento è necessario quindi fare sempre riferimento alla
specifica documentazione di prodotto.

In questo senso di seguito sono indicati alcuni riferimenti utili da cui
poter partire:

- Sito ufficiale di Matomo --
  [[https://matomo.org]{.underline}](https://matomo.org)

- Documentazione Matomo --
  [[https://matomo.org/guides/]{.underline}](https://matomo.org/guides/)

- Forum Matomo --
  [[https://forum.matomo.org/]{.underline}](https://forum.matomo.org/)

