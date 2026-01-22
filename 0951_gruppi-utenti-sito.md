# GRUPPI UTENTI SITO



La sezione **"Gruppi Utenti Sito"**, accessibile dalla voce di menu
principale "**Utenti**", consente di visualizzare e gestire i vari
gruppi in cui possono essere suddivisi gli utenti del sito, sia a
livello di Gerarchie di Agenti e Clienti abilitati ad accedere all'Area
Riservata, sia a livello di normali gruppi utente cui associare, ad
esempio, dei filtri articolo.

> **NOTA BENE:** con il termine "Gerarchia Utenti" si intende un insieme
> di gruppi organizzati secondo una struttura gerarchica ad albero.

All'interno di questa sezione dell'applicazione comparirà quindi la
maschera **"Gruppi Utenti"**

![](./assets/media/image109.png)

in cui verranno visualizzati in:

- **Azzurro** i gruppi utente che rappresentano il gruppo radice di una
  certa gerarchia.

> Tali gruppi avranno quindi anche dei gruppi figli visualizzabili e
> gestibili cliccando sul pulsante **"Modifica"** presente nella
> contestuale barra degli strumenti

- **Bianco** i gruppi utente che non appartengono a nessuna gerarchia e
  che non hanno quindi nessun gruppo figlio.

- **Verde** i gruppi **Standard** "**Utente Autenticato**" e "**Utente
  Non Autenticato**".

> **Utente Autenticato:** apparterranno a questo gruppo tutti gli utenti
> che hanno effettuato il login al sito. Nel momento in cui, dunque, un
> qualsiasi cliente effettui l'accesso al sito verrà automaticamente
> inserito all'interno di questo gruppo.
>
> **Utenti Non Autenticati:** apparterranno a questo gruppo tutti gli
> utenti che visitano il sito senza effettuare l'autenticazione.
>
> In relazione a questi due gruppi occorre poi fare un'ulteriore
> osservazione.
>
> Mentre il gruppo standard "Utenti Autenticati" è unico, per quel che
> riguarda gli "**Utenti non Autenticati**" oltre al gruppo standard
> creato in automatico dall'applicazione **e non eliminabile**, sarà
> sempre possibile definire anche altri gruppi di questo tipo
> differenziandoli sulla base di uno specifico filtro utenti che
> distingue in relazione alla nazione di appartenenza dell'utente che
> visita il sito (determinata sulla base dell'indirizzo IP del
> visitatore)
>
> **I gruppi di utenti "Non Autenticati" creati manualmente (e sempre
> eliminabili) verranno visualizzati in giallo**
>
> Per maggiori informazioni relativamente ai gruppi Standard si veda
> anche il successivo capitolo di questo manuale.

Sulla base di quanto detto appare evidente che all'interno della
maschera "Gruppi Utenti" verranno, in ogni caso, visualizzati i soli
gruppi di utenti che non hanno un gruppo padre.

I pulsanti presenti nella contestuale barra degli strumenti
consentiranno rispettivamente di:

**Lista Utenti Gruppo** (
![](./assets/media/image110.png) ): consente di visualizzare l'elenco degli utenti
appartenenti al gruppo attualmente selezionato.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Lista Utenti -- Nome Gruppo**"

![](./assets/media/image111.png)

contenente l'elenco degli utenti appartenenti al gruppo in esame. I
pulsanti presenti nella barra degli strumenti consentono di:

- **Esportazione Utenti**
  (![](./assets/media/image112.png) ): consente di esportare **in formato .csv**
  l'elenco degli utenti del gruppo

> Per maggiori informazioni relativamente alla procedura di esportazione
> utenti si veda anche la sezione *"Utenti -- Utenti Sito -- Utenti"* di
> questo manuale

- **Aggiungi al Gruppo**
  (![](./assets/media/image113.png) ): visibile solo per i Gruppi cui non è
  stato associato uno specifico filtro utenti.

> Consente di associare al gruppo in esame, un qualsiasi utente del
> sito. Cliccando su questo pulsante verrà quindi visualizzata la
> maschera, **a selezione multipla**, dei possibili utenti da aggiungere
> al gruppo
>
> **NOTA BENE:** dall'elenco dei possibili utenti da aggiungere al
> gruppo verranno ovviamente esclusi quelli che dello specifico gruppo
> fanno già parte.
>
> Per associare uno più utenti al gruppo in esame sarà quindi
> sufficiente selezionarli all'interno della relativa tabella e cliccare
> poi sul pulsante "**Aggiungi**" visualizzato nella contestuale barra
> degli strumenti.
>
> **NOTA BENE:** non è possibile associare ad un gruppo utenti di tipo
> "Contatto Non Attivo".

- **Modifica Utente** (
  ![](./assets/media/image10.png) ): consente di accedere ai dati
  anagrafici dell'utente attualmente selezionato in elenco. Cliccando su
  questo pulsante verrà infatti aperta la maschera **"Dati Utente"**

![](./assets/media/image114.png)

> attraverso cui poter gestire, eventualmente, anche l'associazione
> "Utente -- Gruppo" (si veda anche la sezione *"Utenti -- Utenti Sito"*
> di questo manuale).

- **Rimuovi dal gruppo** (
  ![](./assets/media/image115.png) ): consente di eliminare
  l'associazione tra il gruppo in esame e l'utente attualmente
  selezionato in elenco.

> **ATTENZIONE!** La rimozione di un utente da uno specifico gruppo,
> **non elimina l'utente dal sito**. L'utente rimosso continuerà quindi
> ad essere presente tra gli "Utenti Sito".

- **Elimina Utente:**
  (![](./assets/media/image68.png) ) consente di eliminare l'utente
  attualmente selezionato dal database di Passweb

> **ATTENZIONE! La corretta procedura di eliminazione di un utente dal
> sito è quella che prevede di agire direttamente all'interno del
> gestionale impostando l'anagrafica del cliente in modo tale che non
> venga più esportato e gestito all'interno del sito.**
>
> Nel caso in cui si dovesse comunque decidere di procedere
> all'eliminazione tramite questo pulsante, è comunque necessario
> intervenire anche lato gestionale; in caso contrario lo specifico
> utente potrebbe comunque essere riesportato a seguito di una futura
> sincronizzazione.
>
> Eliminando un utente dal sito (mediante il pulsante "Elimina Utente"
> o, in maniera più corretta, operando per questo direttamente
> all'interno del gestionale) verranno automaticamente eliminate anche
> tutte le cartelle presenti in Area Riservata (sezione Documenti)
> create da quello stesso utente, che non risultano essere legate ad
> altri gruppi e che non hanno file al loro interno.
>
> Per maggiori informazioni relativamente alle diverse sezioni e
> funzionalità dell'Area Riservata si veda anche la sezione *"Business
> to Business Area Riservata"* di questo manuale.
>
> **ATTENZIONE!** Eventuali cartelle legate ad utenti eliminati dal sito
> che, per qualche ragione, non possono essere eliminate contestualmente
> all'eliminazione dell'utente potranno essere gestite all'interno della
> sezione "**Cartelle Non Assegnate**"

**Modifica** (
![](./assets/media/image116.png) ): consente di gestire le proprietà del
gruppo attualmente selezionato oltre, eventualmente, alla gerarchia cui
esso da origine.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
**"Gerarchia Utenti -- Nome gruppo radice"**

![](./assets/media/image117.png)

all'interno della quale sarà possibile gestire, attraverso l'apposito
albero presente nella parte sinistra l'eventuale gerarchia.

Nella parte destra della maschera verranno invece visualizzate, e
potranno quindi essere gestite, le proprietà del gruppo attualmente
selezionato all'interno dell'albero.

**Elimina** (
![](./assets/media/image95.png) ): consente di eliminare il gruppo
attualmente selezionato.

**NOTA BENE:** nel caso in cui al gruppo sia associata anche una
gerarchia, eliminando il gruppo verrà eliminata anche l'intera struttura
di sottogruppi.

**Nuovo Gruppo Utenti Non Autenticati** (
![](./assets/media/image118.png) )**:** consente di creare un nuovo
gruppo di "Utenti Non Autenticati" oltre a quello standard creato a
default dall'applicazione

Per maggiori informazioni relativamente ai gruppi standard si veda il
successivo capitolo di questo manuale.

**Nuovo Gruppo Utenti** (
![](./assets/media/image119.png) ): consente di creare un nuovo gruppo
oltre che di associargli, eventualmente, anche una gerarchia di sotto
gruppi.

Cliccando su questo pulsante si verrà infatti ricondotti alla maschera
**"Creazione Gruppo"**

![](./assets/media/image120.png)

attraverso cui poter definire tutte le proprietà del gruppo stesso.

In particolare per ogni nuovo gruppo sarà possibile indicare oltre al
nome tutta una serie di parametri di configurazione racchiusi
all'interno delle diverse sezioni: Area Riservata, Filtri, Condizioni
commerciali associate all'utente e Codici Mastro.

Per maggiori informazioni in merito ai diversi parametri presenti
all'interno di ciascuna di queste sezioni, si veda anche il successivo
capitolo (*Configurazione di un gruppo Utenti*) di questo manuale

**Importa** (
![](./assets/media/image121.png) ): consente variare in maniera massiva, mediante
l'upload di un apposito file csv i dati di configurazione dei Gruppi
Utente **NON STANDARD**

**ATTENZIONE! la procedura in oggetto non consente di variare in alcun
modo i Gruppi Utente Standard gestiti da Passweb** (per maggiori
informazioni relativamente a questa tipologia di Gruppi Utente si vedano
anche i successivi capitoli di questo manuale)

Cliccando sul pulsante in esame verrà visualizzata la maschera
"**Importazione Dati Gruppi**" mediante la quale poter effettuare
l'upload del file contenente le informazioni desiderate.

![](./assets/media/image122.png)

Nello specifico all'interno di questa sezione sarà necessario indicare:

- **File (csv-txt):** consente di selezionare il file txt o csv da
  uplodare e contenente i dati dei gruppi utente da modificare

- **Lingua**: consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta e i
dati contenuti nel file possano essere associati ai relativi gruppi
utente, dovranno essere rispettate delle regole ben precise. Nello
specifico:

- Prima di avviare la procedura di import dovranno già essere stati
  creati all'interno di Passweb, tutti i gruppi utente i cui parametri
  di configurazione dovranno essere valorizzati attraverso questa
  procedura.

> **ATTENZIONE! La procedura di import non crea in alcun modo nuovi
> Gruppi Utente**

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- L'intestazione, ossia la prima riga del file, deve necessariamente
  contenere l'elenco dei nomi dei campi articolo che dovranno poi essere
  valorizzati con i dati presenti all'interno del file stesso.

<!-- -->

- Il primo campo del file, **obbligatorio e utilizzato come chiave**,
  dovrà essere **l'identificativo Passweb** **del relativo gruppo
  utente**, dato questo reperibile in corrispondenza del relativo campo
  presente nel file che potrà essere generato dalla procedura di
  esportazione dei Gruppi Utente

> **NOTA BENE:** se all'interno del file da importare non è presente
> l'identificativo del gruppo utente passweb e/o se tale valore non
> corrisponde a quello di un gruppo non standard effettivamente gestito
> all'interno del proprio sito la procedura di import non valorizzerà,
> ovviamente, alcun campo

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180**

<!-- -->

- È necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

Di seguito viene indicato l'elenco dei campi che potranno essere
inseriti all'interno del file csv e che potranno quindi essere
valorizzati in maniera massiva mediante la procedura in esame:

- **id**: identificativo del gruppo utente reperibile in corrispondenza
  del relativo campo presente nel file che potrà essere generato dalla
  procedura di esportazione dei Gruppi Utente

> **ATTENZIONE! il campo id è obbligatorio e verrà utilizzato come campo
> chiave**

- **nome**: corrispondente al campo **Nome** presente nella sezione
  "**Generale**" della maschera di configurazione del gruppo

> Consente di impostare il nome del relativo Gruppo Utente
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** L'utente può effettuare il login al sito

- **NO 🡪** L'utente non può effettuare il login al sito

<!-- -->

- **sms**: corrispondente al campo "**Gestione Sms**" presente nella
  sezione "**Area Riservata**" della maschera di configurazione del
  gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire gli sms
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire gli sms

- **NO 🡪** Gli utenti del gruppo non potranno gestire gli sms

<!-- -->

- **whatsapp**: corrispondente al campo "**Gestione Whatsapp**" presente
  nella sezione "**Area Riservata**" della maschera di configurazione
  del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire le notifiche collegate ai diversi eventi gestiti via Whatsapp
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire le notifiche Whatsapp

- **NO 🡪** Gli utenti del gruppo non potranno gestire le notifiche
  Whatsapp

> **ATTENZIONE!** il campo in esame dovrà essere gestito solo nel caso
> in cui sia stato attivato il modulo relativo all'integrazione Passweb
> -- WA Smart Business. Per maggiori informazioni si rimanda a quanto
> indicato nel relativo capitolo ("*Passweb e WA Smart Business*") di
> questo manuale

- **telegram**: corrispondente al campo "**Gestione Telegram**" presente
  nella sezione "**Area Riservata**" della maschera di configurazione
  del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire le notifiche collegate ai diversi eventi gestiti via Telegram
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire le notifiche Telegram

- **NO 🡪** Gli utenti del gruppo non potranno gestire le notifiche
  Telegram

> **ATTENZIONE!** il campo in esame dovrà essere gestito solo nel caso
> in cui sia stato attivato il modulo relativo all'integrazione Passweb
> -- Telegram. Per maggiori informazioni si rimanda a quanto indicato
> nel relativo capitolo ("*Passweb e Telegram*") di questo manuale

- **comunicazioneInterna**: corrispondente al campo "**Comunicazione
  Intera**" presente nella sezione "**Area Riservata**" della maschera
  di configurazione del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> comunicare tra di loro
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno comunicare tra di loro

- **NO 🡪** Gli utenti del gruppo non potranno comunicare tra di loro

<!-- -->

- **comunicazioneUp**: corrispondente al campo "**Comunicazione Utenti
  Livello superiore**" presente nella sezione "**Area Riservata**" della
  maschera di configurazione del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> comunicare con gli utenti dei gruppi padri
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno comunicare con gli utenti dei
  gruppi padri

- **NO 🡪** Gli utenti del gruppo non potranno comunicare con gli utenti
  dei gruppi padri

<!-- -->

- **agenteCliente**: corrispondente al campo "**Mostra Agente Cliente**"
  presente nella sezione "**Area Riservata**" della maschera di
  configurazione del gruppo. Disponibile **solo per i siti Ecommerce
  collegati aMexal**

> Consente di indicare se nella sezione "Clienti" dell'area riservata,
> per gli utenti del gruppo in esame, debba o meno essere mostrato
> l'agente associato al cliente
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** dovrà essere mostrato l'agente associato al cliente

- **NO 🡪** non dovrà essere mostrato l'agente associato al cliente

<!-- -->

- **filtroArticoli**: corrispondente al campo "**Filtri articoli**"
  presente nella sezione "**Filtri**" della maschera di configurazione
  del gruppo. Disponibile **solo per i siti Ecommerce**

> Consente di indicare il filtro articoli da applicare agli utenti del
> gruppo

- **filtroUtenti**: corrispondente al campo "**Filtri utenti**" presente
  nella sezione "**Filtri**" della maschera di configurazione del
  gruppo. Disponibile **solo per i siti Ecommerce**

> Consente di indicare il filtro utenti da applicare agli utenti del
> gruppo

- **filtroClientiAgente:** corrispondente al campo "**Filtri clienti
  agente**" presente nella sezione "**Filtri**" della maschera di
  configurazione del gruppo. Disponibile **solo per i siti Ecommerce**

> Consente di indicare il filtro sugli utenti degli agenti

**ATTENZIONE!** **i filtri articolo, utente e clienti agente, da
inserire all'interno del file di importazione dovranno seguire una
determinata sintassi.**

In questo senso, per ottenere il valore corretto da inserire in
corrispondenza di questi campi, si consiglia sempre di creare prima il
filtro desiderato direttamente all'interno del Wizard e utilizzare poi
il relativo pulsante "**Copia Filtro**" per ottenere la stringa da
inserire nel file di importazione

![](./assets/media/image123.png)

**ATTENZIONE!** nel momento in cui dovesse essere indicato, all'interno
del file, per un determinato gruppo un filtro utenti, in fase di
importazione verranno ovviamente variate le utenze appartenenti a quello
specifico gruppo secondo quando indicato nel filtro in esame

- **prioritaCondizioni** corrispondente al campo "**Priorità Condizione
  Commerciale**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare la priorità da associare al relativo gruppo.
>
> **ATTENZIONE!** Il valore di questo campo deve essere univoco, per cui
> non possono esserci più gruppi con la stessa priorità

- **applicationCondizioni**: corrispondente al campo "**Applicazione
  Condizioni**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare quando applicare le condizioni. I valori ammessi
> sono:

- **0**: Assegnazione in fase di registrazione

- **1**: Assegnazione in fase di registrazione e profilo

<!-- -->

- **listino**: corrispondente al campo "**Listino**" presente nella
  sezione "**Condizioni Commerciali associate all'utente**" della
  maschera di configurazione del gruppo. Disponibile **solo per i siti
  Ecommerce**

> Consente di indicare il nome del listino da associare al gruppo

- **VAT**: corrispondente al campo "**Aliquota IVA (VAT)**" presente
  nella sezione "**Condizioni Commerciali associate all'utente**" della
  maschera di configurazione del gruppo. Disponibile **solo per i siti
  Ecommerce**

> Consente di indicare l'aliquota iva da associare al gruppo

- **minimoOrdine**: corrispondente al campo "**Minimo d'Ordine**"
  presente nella sezione "**Condizioni Commerciali associate
  all'utente**" della maschera di configurazione del gruppo. Disponibile
  **solo per i siti Ecommerce**

> Consente di definire il minimo d'ordine da associare al gruppo

- **pagamento**: corrispondente al campo "**Pagamento Abituale**"
  presente nella sezione "**Condizioni Commerciali associate
  all'utente**" della maschera di configurazione del gruppo. Disponibile
  **solo per i siti Ecommerce**

> Consente di indicare il nome del pagamento da associare al gruppo

- **categoriaStatisticheCliente**: corrispondente al campo "**Categoria
  Statistica**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare il nome della categoria statistica cliente da
> associare al gruppo

- **zoneCliente**: corrispondente al campo "**Zona**" presente nella
  sezione "**Condizioni Commerciali associate all'utente**" della
  maschera di configurazione del gruppo. Disponibile **solo per i siti
  Ecommerce**

> Consente di indicare il nome della zona cliente da associare al gruppo

- **agente**: corrispondente al campo "**Agente**" presente nella
  sezione "**Condizioni Commerciali associate all'utente**" della
  maschera di configurazione del gruppo. Disponibile **solo per i siti
  Ecommerce**

> Consente di indicare il codice conto dell'agente da associare ai
> clienti del gruppo

- **categorieProvvigioniCliente**: corrispondente al campo "**Categoria
  Provvigioni**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare il nome della categoria provvigione cliente da
> associare al gruppo

- **applicationSconti**: corrispondente al campo "**Applicazione
  Sconti**" presente nella sezione "**Condizioni Commerciali associate
  all'utente**" della maschera di configurazione del gruppo. Disponibile
  **solo per i siti Ecommerce**

> Consente di indicare quando applicare gli sconti. I valori ammessi
> sono:

- **0**: Applicazione in fase di registrazione

- **1**: Applicazione in caso di assenza di valori

- **2**: Assegnazione in fase di registrazione e profilo

<!-- -->

- **categorieScontoCliente**: corrispondente al campo "**Categoria**
  **Sconto Cliente**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare il nome della categoria sconto cliente da
> associare al gruppo

- **sconto**: corrispondente al campo "**Sconto Incondizionato**"
  presente nella sezione "**Condizioni Commerciali associate
  all'utente**" della maschera di configurazione del gruppo. Disponibile
  **solo per i siti Ecommerce**

> Consente di indicare lo sconto incondizionato da associare ai clienti
> del gruppo

- **serie**: corrispondente al campo "**Numero Serie del Documento**"
  presente nella sezione "**Condizioni Commerciali associate
  all'utente**" della maschera di configurazione del gruppo. Disponibile
  **solo per i siti Ecommerce**

> Consente di indicare il numero della serie da utilizzare nel caso in
> cui ad effettuare l'ordine dovesse essere direttamente il cliente

- **seriePreventivo**: corrispondente al campo "**Numero Serie del
  Preventivo**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare il numero della serie da utilizzare nel caso in
> cui ad effettuare il preventivo dovesse essere direttamente il cliente

- s**erieAgente**: corrispondente al campo "**Numero Serie del Documento
  per Agente**" presente nella sezione "**Condizioni Commerciali
  associate all'utente**" della maschera di configurazione del gruppo.
  Disponibile **solo per i siti Ecommerce**

> Consente di indicare il numero della serie da utilizzare nel caso in
> cui ad effettuare l'ordine dovesse essere un Agente che impersonifica
> un cliente

- serieAgentePreventivo: corrispondente al campo "**Numero Serie del
  Preventivo per Agente**" presente nella sezione "**Condizioni
  Commerciali associate all'utente**" della maschera di configurazione
  del gruppo. Disponibile **solo per i siti Ecommerce**

> Consente di indicare il numero della serie da utilizzare nel caso in
> cui ad effettuare il preventivo dovesse essere un Agente che
> impersonifica un cliente

**Esporta** (
![](./assets/media/image124.png) ): consente di esportare, all'interno di un apposito
file csv, i dati dei gruppi utente, NON STANDARD, attualmente gestiti
all'interno del sito.

**ATTENZIONE!** I campi presenti nel file csv sono gli stessi indicati
per la procedura di importazione dati

