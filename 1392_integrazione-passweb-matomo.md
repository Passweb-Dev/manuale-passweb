# INTEGRAZIONE PASSWEB -- MATOMO



Come già evidenziato nei precedenti capitoli di questo manuale Matomo si
presenta, per certi aspetti, come un software molto simile alla versione
Universal di Google Analytics. Il tracciamento di quello che succede
all'interno del sito viene effettuato, almeno nella sua configurazione
standard, lato client quindi via javascript con l'installazione, nel
browser dei visitatori, di determinati cookie di
tracciamento/profilazione.

In conseguenza di ciò per poter iniziare a tracciare quello che avviene
all'interno del proprio sito Passweb utilizzando questo strumento sarà
sufficiente inserire nelle pagine del sito uno snippet di codice
prelevabile direttamente dalla propria installazione Matomo.

In questo senso, supponendo di aver già portato a termine in maniera
corretta l'installazione di Matomo (si ricorda che Passepartout non
fornisce alcun tipo di supporto in questo senso) la prima cosa da fare
sarà quella di andare ad inserire il sito da tracciare in maniera tale
da poter generare codice il di monitoraggio che dovrà poi essere
inserito all'interno del proprio sito Passweb.

Nello specifico sarà quindi necessario accedere al pannello di
Amministrazione della propria installazione Matomo (icona del piccolo
ingranaggio posta in alto a destra nella barra degli strumenti),
portarsi poi nella sezione "**Siti Web -- Amministrazione**" utilizzando
il menu posizionato sulla sinistra della pagina, e da qui cliccare sul
pulsante "**Aggiungi un nuovo sito**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_21.bmp](./assets/media/image21.png)

Nella successiva maschera ci verrà chiesto se quello che vogliamo
monitorare è un Sito "tradizionale" o un sito Intranet.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_22.bmp](./assets/media/image22.png)

Selezionando quindi l'opzione "**Sito**" verremo automaticamente
ricondotti alla maschera "**Gestione Misurabili**" dove dovranno essere
inseriti tutti i parametri di configurazione del sito da monitorare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_23.bmp](./assets/media/image23.png)

In questo senso, oltre ai classici parametri come possono essere
ovviamente l'url del sito da monitorare, un eventuale lista di indirizzi
IP o di User Agent che dovranno essere esclusi dalle statistiche ...
sarà particolarmente importante verificare di aver impostato
correttamente, in relazione sempre alla tipologia di tracciamento che si
vuole effettivamente implementare, i seguenti parametri:

- **Ecommerce:** consente, se impostato sull'opzione "**Ecommerce
  attivato**" di abilitare all'interno della sezione "**Obiettivi**"
  tutta una serie di report utili per il monitoraggio Ecommerce (es.
  carrelli abbandonati, ordini effettuati ecc...)

> **ATTENZIONE!** nel momento in cui l'esigenza dovesse essere quella di
> attivare, per il proprio sito Passweb, anche il monitoraggio Ecommerce
> questo parametro dovrà necessariamente essere impostato sull'opzione
> "Ecommerce attivato".
>
> In caso contrario, se anche dovessero essere impostati correttamente
> tutti i relativi parametri del proprio sito Passweb, non si avrebbe
> poi la possibilità di visualizzare su Matomo i corrispondenti dati
> Ecommerce

- **Valuta:** consente di impostare la valuta utilizzata all'interno del
  sito (fondamentale nel caso in cui si decida di attivare anche il
  monitoraggio Ecommerce)

- **Fuso Orario:** consente di impostare il fuso orario che dovrà essere
  utilizzato per gestire date e orari che verranno poi riportati
  all'interno del sistema per ogni vista o evento tracciato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_24.bmp](./assets/media/image24.png)

Una volta impostati tutti i parametri richiesti, cliccando sul pulsante
"Salva" presente nella parte bassa della maschera il sito in esame verrà
inserito tra quelli monitorati da Matomo e, contestualmente, verrà anche
generato il relativo codice di tracciamento.

Cliccando quindi sul collegamento "**Vedi codice Tracking**" evidenziato
in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_25.bmp](./assets/media/image25.png)

verremo automaticamente rediretti alla pagina "**Siti Web -- Codice di
Tracciamento**" del pannello di Amministrazione di Matomo relativo al
sito appena inserito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_26.bmp](./assets/media/image26.png)

A questo punto sarà quindi sufficiente copiare lo snippet di codice
presente all'interno della sezione "**Codice Javascript**" evidenziato
nella figura sopra riportata ed inserirlo all'interno del campo
"**Codice di tracciamento**" presente alla pagina "**Sito -- Preferenze
-- Tracciamento Dati**" (sezione "**Matomo -- Client**") del Wizard del
proprio sito Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_27.bmp](./assets/media/image27.png)

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

Il codice di tracciamento evidenziato in figura consente di gestire,
inoltre, un tracciamento "standard" che riguarda essenzialmente le sole
visite alle diverse pagine del sito.

Nel momento in cui l'esigenza dovesse essere quella di gestire anche un
tracciamento ecommerce e/o le ricerche interne al sito sarà quindi
necessario (oltre ad aver attivato le relative funzionalità in fase di
configurazione del sito su Matomo) selezionare anche i due parametri
"**Abilita Tracciamento Ecommerce**" e "**Abilita Tracciamento
Ricerca**" evidenziati in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_28.bmp](./assets/media/image28.png)

Per maggiori informazioni relativamente al monitoraggio ecommerce
presente nell'integrazione Passweb -- Matomo si veda anche quanto
indicato nel successivo capitolo ("*Monitoraggio Ecommerce*") di questo
manuale

Infine, come evidenziato nei precedenti capitoli di questo manuale,
oltre al tracciamento "tradizionale" effettuato lato client con
l'utilizzo dei cookie, Matomo offre la possibilità di implementare il
tracciamento di ciò che avviene all'interno del sito anche secondo altre
modalità che possono andare dall'utilizzo di un sistema proprietario di
gestione dei Tag e analogo a Google Tag Manager (
<https://matomo.org/guide/tag-manager/> ), a un sistema che non fa
assolutamente uso di cookie o, ancora, ad un sistema di tracciamento
lato server che utilizza le API messe a disposizione dalla piattaforma.

Per maggiori informazioni relativamente a quest'ultima opzione, e a come
essa viene implementata e gestita lato Passweb, si rimanda a quanto
indicato nel successivo capitolo ("*Tracciamento lato server*") di
questo manuale

