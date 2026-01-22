# CONFIGURAZIONE ACCOUNT PASSWEB



Una volta attivato l'account di Google Merchant per completare
l'integrazione tra le due piattaforme e fare in modo, quindi, che
Passweb e Google Merchant possano comunicare tra loro via API sarà
necessario creare un apposito account di servizio (in uno specifico
progetto della propria developer console) con associata una relativa
chiave JSON.

L'account di servizio dovrà poi essere inserito direttamente tra gli
utenti del proprio account Google Merchant; la chiave JSON associata a
questo stesso account di servizio dovrà invece essere inserita nella
configurazione dell'account all'interno del proprio sito Passweb.

Nello specifico sarà quindi necessario:

1.  Accedere alla developer console di google (
    <https://console.developers.google.com> ) utilizzando il proprio
    account (si può utilizzare lo stesso account utilizzato anche per
    accedere a Google Merchant)

![](./assets/media/image421.png)

> e cliccare poi sul pulsante "**Create Project**".

2.  Assegnare un nome al progetto e cliccare sul pulsante "**Create**"

![](./assets/media/image422.png)

3.  Una volta creato il nuovo progetto aprire il menu laterale cliccando
    sull'apposita icona presente nella parte alta della pagina.
    Selezionare la voce "**APIs & Services**" e cliccare su **Library**
    in maniera tale da accedere alla libreria delle API attivabili per
    il progetto in esame

![](./assets/media/image423.png)

4.  Selezionare l'API "**Content API for Shopping**" utilizzando
    l'apposito pannello di ricerca

![](./assets/media/image424.png)

> e abilitarla cliccando sul pulsante "**Enable**"

![](./assets/media/image425.png)

5.  Dopo aver attivato la Content API for Shopping accedere alla sezione
    "**Credential**" dal relativo menu laterale

![](./assets/media/image426.png)

6.  Cliccare sul pulsante "**Create Credentials**" e selezionare
    l'opzione "**Service account**"

![](./assets/media/image427.png)

7.  Assegnare un nome al nuovo account di servizio e copiare l'indirizzo
    mail che gli verrà assegnato in automatico

![](./assets/media/image428.png)

> **ATTENZIONE!** l'indirizzo mail associato all'account di servizio che
> stiamo creando è di fondamentale importanza inquanto ci servirà poi
> nel momento in cui dovremo andare ad aggiungere a Google Merchant
> questo stesso account di servizio
>
> Cliccare quindi su "**Create and Continue**"

8.  Nei successivi passaggi lasciare le impostazioni di default e
    cliccare su "**Done**"

![](./assets/media/image429.png)

9.  Una volta completata la creazione del nuovo account di servizio sarà
    ora necessario creare la chiave JSON ad esso associata e che dovremo
    poi andare ad inserire all'interno del nostro sito Passweb.

> Per far questo sarà necessario entrare nella maschera di
> configurazione dell'account appena creato cliccando sulla relativa
> icona di edit (o anche direttamente sull'indirizzo mail ad esso
> associato)

![](./assets/media/image430.png)

> e selezionare poi la voce "**Keys**" evidenziata in figura

![](./assets/media/image431.png)

10. Cliccare quindi sul pulsante "**ADD KEY**" e selezionare l'opzione
    "**Create new key**"

![](./assets/media/image432.png)

11. Nella successiva maschera di creazione della chiave selezionare
    l'opzione JSON

![](./assets/media/image433.png)

> e cliccare sul pulsante "**CREATE**"
>
> Verrà quindi creato e salvato sul nostro pc il file JSON contente la
> chiave che dovremo poi andare ad inserire nel back end del nostro sito
> Passweb in fase di configurazione dell'account Google Merchant (si
> vedano i successivi passaggi per ulteriori informazioni)

![](./assets/media/image434.png)

> Arrivati a questo punto dovremo ora andare ad aggiungere l'account di
> servizio appena creato come utente del Google Merchant Center

12. Effettuare quindi nuovamente l'accesso all'account di Google
    Merchant precedentemente creato, cliccare sull'icona della rotellina
    (Settings & Tools) presente in testata e selezionare l'opzione
    "**People and access**"

![](./assets/media/image435.png)

13. Cliccare quindi su "**Add user**"

![](./assets/media/image436.png)

> e aggiungere l'utente di servizio precedentemente creato (punti 7 e 8)
> utilizzando il suo indirizzo mail

![](./assets/media/image437.png)

14. Nella successiva maschere "User access" assegnare all'utente
    l'accesso come admin

![](./assets/media/image438.png)

> e cliccare quindi sul pulsante "**Add user**"

15. L'ultimo passaggio da eseguire, questa volta di fondamentale
    importanza anche per una corretta pubblicazione degli articoli, è
    quello che prevede di attivare direttamente all'interno del Merchant
    Center, almeno una spesa di spedizione. In caso contrario infatti,
    quando andremo poi a pubblicare degli articoli potremmo ottenere un
    errore legato proprio al fatto di non aver ancora gestito delle
    spese di spedizione

> **ATTENZIONE! Allo stato attuale le spese di spedizione vanno
> codificate e gestite direttamente sul Merchant Center di Google.
> Considerando poi che eventuali acquisti effettuati a partire da
> annunci Google Shopping si concluderanno comunque sul sito Ecommerce,
> le spese indicate sul Merchant Center dovranno essere (a livello di
> importo) le stesse di quelle effettivamente applicate all'interno del
> sito.**
>
> Per codificare le spese di trasporto sarà necessario agire all'interno
> della sezione "**Shipping and returns**"

![](./assets/media/image439.png)

> Una volta terminata la configurazione del Merchant Center il passo
> successivo sarà quello che prevede di configurare l'integrazione tra
> esso ed il nostro sito Ecommerce.

16. Portarsi quindi nel Wizard di Passweb, all'interno della sezione
    "**Catalogo -- Altri Marketplace -- Gestione Account**" e cliccare
    sul pulsante "Aggiungi Account" presente nella parte alta della
    pagina

17. All'interno della maschera "Dati Account" assegnare un nome
    all'Account che si sta configurando (campo **Descrizione**) e
    selezionare, all'interno del campo "**Marketplace**" l'opzione
    "**Google Merchant**"

![](./assets/media/image440.png)

18. Compilare i campi presenti all'interno della sezione
    "**Credenziali**" con i dati di seguito indicati:

    - **Merchant Id**: codice identificativo del proprio Account Google
      Merchant

> Per ottenere questa informazione è sufficiente accedere al proprio
> Account Merchant Center e prelevare il codice richiesto copiandolo da
> quanto riportato in alto a destra (dove sono indicate anche altre
> informazioni del nostro account)

![](./assets/media/image441.png)

> Copiare quindi il codice evidenziato in figura e inserirlo nel
> corrispondente campo Passweb

- **Account Service .json**: file .json associato all'account di
  servizio generato al punto 11

> Sarà quindi necessario uplodare il file richiesto, e precedentemente
> salvato sul proprio pc, trascinandolo all'interno della corrispondente
> area di drop

19. Cliccare sul pulsante "**Salva**" presente nella parte bassa della
    pagina in modo tale da salvare i dati immessi e attivare di fatto la
    connessione tra Passweb ed il Merchant Center di Google.

Una volta effettuato il salvataggio dei dati compariranno nuove sezioni
(Metodi di pubblicazione, Articoli, Schedulazione, Marketplace, Download
CSV) all'interno delle quali poter configurare in maniera più
dettagliata altri aspetti dell'integrazione.

Per maggiori informazioni in merito a ciascuna di queste sezioni si
vedano i successivi capitoli di questo manuale.

##### METODI DI PUBBLICAZIONE

All'interno di questa sezione è possibile decidere quale dovrà essere il
metodo adottato per la pubblicazione dei dati articolo sulla piattaforma
terza.

In questo senso Passweb offre due diverse modalità di esportazione dei
dati selezionabili attraverso l'apposito menu a tendina (parametro
"**Modalità pubblicazione articoli**"):

1.  **via API**: i dati articolo verranno trasferiti ed inseriti sulla
    piattaforma terza in maniera automatica sfruttando, appunto, le API
    messe a disposizione dalla piattaforma stessa

> **ATTENZIONE!** il processo di pubblicazione via API dipende
> ovviamente, oltre che dalle elaborazioni interne a Passweb, anche dai
> tempi di risposta e dai limiti imposti delle relative API. Per
> maggiori informazioni in merito a tali limiti si consiglia di fare
> riferimento alla documentazione ufficiale di Google (
> <https://developers.google.com/shopping-content/guides/limits> )

2.  **via CSV**: i dati articolo verranno pubblicati all'interno di
    appositi file csv. Tali file potranno poi essere:

    - scaricati direttamente dal Wizard di Passweb e uplodati
      manualmente sulla piattaforma terza

    - accessibili ad uno specifico url (sotto il dominio assegnato al
      proprio sito Passweb)

    - copiati automaticamente all'interno di un'area condivisa (Ftp,
      Google Drive ...) stabilita in fase di configurazione del proprio
      Account di integrazione

> Dipendentemente dalla destinazione scelta per la pubblicazione dei
> file csv, andrà poi configurata correttamente anche la piattaforma
> terza affinché possa recuperare i dati in maniera adeguata
>
> **ATTENZIONE!** anche la pubblicazione via CSV è sottoposta a
> determinati limiti dettati sempre dalla piattaforma terza. Tali limiti
> sono comunque meno stringenti rispetto a quelli che regolano la
> pubblicazione via API (la dimensione massima accettata per il file csv
> è, ad esempio, di 4 GB). Per maggiori informazioni in merito si
> consiglia comunque di fare sempre riferimento alla documentazione
> ufficiale di Google (
> <https://support.google.com/merchants/answer/188477?hl=it> )

Parlando sempre di limiti imposti dalla piattaforma terza in relazione
alla pubblicazione di articoli, una cosa di fondamentale importanza da
tenere sempre in considerazione **è che prodotti inseriti all'interno di
Google Merchant (via API o via CSV non fa differenza) che non dovessero
risultare variati per un certo periodo di tempo (attualmente 30 giorni)
verranno automaticamente rimossi.**

**ATTENZIONE!** Tale rimozione viene effettuata direttamente da Google
ed è quindi indipendente da Passweb.

Nel momento in cui l'esigenza dovesse essere quindi quella di mantenere
all'interno del Merchant Center determinati prodotti anche nel caso in
cui non dovessero essere variati (a livello di prezzi, quantità, titolo,
marca ...), sarà necessario ricordarsi di ripubblicare questi stessi
prodotti prima della scadenza dei 30 giorni.

In questo senso la pubblicazione via CSV può rivelarsi molto più utile
di quella effettuata via API.

Come avremo modo di vedere nei successivi capitoli di questo manuale
infatti, la pubblicazione via API utilizza determinate regole che
assicurano l'aggiornamento e quindi la ripubblicazione dei vari articoli
solo nel caso in cui i dati di questi stessi articoli dovessero
effettivamente risultare variati (ad esempio a livello di prezzi o di
quantità disponibili) rispetto all'ultima pubblicazione effettuata.

Con questo tipo di pubblicazione quindi potrebbero verificarsi
facilmente situazioni in cui determinati prodotti risultando non
variati, non verranno aggiornati / ripubblicati e quindi alla scadenza
dei 30 giorni verranno automaticamente rimossi da Google. **L'unica
soluzione in questo caso sarebbe quindi quella di effettuare manualmente
una pubblicazione via API degli articoli interessati prima della
scadenza dei 30 giorni.**

Utilizzando invece la pubblicazione via CSV, sarà poi possibile
configurare il Merchant Center in maniera tale che questo vada a
rileggere, ad intervalli di tempo regolari (ad esempio giornalmente), i
file CSV prodotti da Passweb. Considerando poi che tali file potranno
contenere sempre tutti gli articoli coinvolti nella pubblicazione
(indipendentemente dal fatto che risultino o meno variati rispetto
all'ultima pubblicazione effettuata) è semplice comprendere che,
operando in questo modo, potremo di fatto andare a ripubblicare, ad
intervalli di tempo regolari (ad esempio ogni giorno), tutta la base
dati dei prodotti presenti nel Merchant Center spostando quindi, ogni
volta, di un giorno in avanti la data di scadenza di questi stessi
prodotti che potranno così essere mantenuti nel Merchant Centre anche
oltre i 30 gironi previsti.

###### PUBBLICAZIONE VIA API

Per attivare questo tipo di pubblicazione è sufficiente impostare il
parametro "**Modalità pubblicazione articoli**" presente nella sezione
"**Metodi di pubblicazione**" della maschera "**Dati Account**"
sull'opzione **API**, come evidenziato nella figura di seguito riportata

![](./assets/media/image442.png)

In queste condizioni, come evidenziato anche nel precedente capitolo di
questo manuale, la pubblicazione dei dati articolo sulla piattaforma
terza avverrà sfruttando completamente le API messe a disposizione dalla
piattaforma stessa. Di base non saranno quindi richiesti altri parametri
configurazione.

###### PUBBLICAZIONE VIA CSV

Per attivare questo tipo di pubblicazione è sufficiente impostare il
parametro "**Modalità pubblicazione articoli**" presente nella sezione
"**Metodi di pubblicazione**" della maschera "**Dati Account**"
sull'opzione **CSV**, come evidenziato nella figura di seguito riportata

![](./assets/media/image443.png)

In questo caso occorrerà poi impostare anche tutta una serie di altri
parametri necessari per configurare in maniera corretta la creazione dei
file csv e il repository in cui andarli ad inserire.

Nello specifico dunque il campo

**Pubblica tutti gli articoli:** consente di decidere come dovrà
comportarsi l'applicativo nel momento in cui si dovessero effettuare
delle pubblicazioni manuali degli articoli coinvolti nelle diverse liste
di vendita.

In questo senso è di fondamentale importanza evidenziare che Passweb
potrà comportarsi in maniere diversa a seconda del fatto che si parli di
pubblicazioni automatiche, e quindi schedulate, oppure di pubblicazioni
manuali.

In particolare:

3.  nel caso di **pubblicazioni automatiche** verranno presi in
    considerazione, ed inseriti quindi nei relativi file csv, **sempre
    tutti gli articoli di tutte le liste di vendita legate all'account
    in esame** indipendentemente dal fatto che risultino o meno variati
    rispetto all'ultima pubblicazione effettuata

4.  nel caso di **pubblicazione manuali** invece il comportamento
    dell'applicativo dipenderà da come è stato impostato il parametro
    "Pubblica tutti gli articoli".

> **Nel momento in cui tale parametro dovesse essere selezionato** le
> pubblicazioni manuali si comporteranno esattamente come quelle
> automatiche. Anche in questo casco dunque verranno sempre presi in
> considerazione, ed inseriti nei relativi file csv, tutti gli articoli
> di tutte le liste vendita collegate all'account in esame,
> indipendentemente da quelli che sono o non sono stati selezionati
> manualmente prima di avviare la relativa pubblicazione.
>
> **Nel momento in cui invece il parametro "Pubblica tutti gli articoli"
> dovesse essere deselezionato**, a seguito di una pubblicazione manuale
> verranno inseriti nel relativo file csv solo ed esclusivamente quei
> prodotti che sono stati effettivamente selezionati nella lista di
> vendita prima di avviare la relativa pubblicazione

**Separatore File CSV:** consente di impostare, selezionandolo da un
apposito menu a tendina, il carattere da utilizzare, in fase di
creazione del file csv, come separatore dei campi

**Modalità scrittura file:** consente di decidere quale dovrà essere il
metodo utilizzato per gestire i contenuti dei file csv a seguito di
pubblicazioni successive.

Considerando che, come precedentemente evidenziato, le pubblicazioni
automatiche via CSV coinvolgono sempre tutti gli articoli di tutte le
liste collegate all'account in esame, cosa questa utile a spostare sul
Merchant Center, ogni volta, di un giorno in avanti la data di scadenza
dei vari articoli (potendoli così mantenere anche oltre i 30 gironi
previsti), e considerando anche la necessità di non modificare ad ogni
pubblicazione il nome del file csv prodotto (cosa questa che
comporterebbe poi la riconfigurazione delle impostazioni del feed anche
sulla piattaforma terza) l'unica opzione possibile per il parametro in
esame sarà "**Sovrascrivi**"

- **Sovrascrivi**: in queste condizioni i file generati a seguito di una
  determinata pubblicazione andranno sempre e comunque a sovrascrivere
  quelli attualmente presenti nel repository utilizzato (e relativi
  ovviamente alla stessa lista di vendita) mantenendo, generalmente,
  anche lo stesso nome. Nel momento in cui nel repository non dovesse
  essere presente un determinato file (perché ad esempio è stata
  aggiunta, rispetto all'ultima pubblicazione una nuova lista di
  vendita) questo verrà creato da zero.

> **In ogni caso, in queste condizioni, i file csv all'interno del
> repository conterranno sempre e soltanto i dati relativi all'ultima
> pubblicazione effettuata**

**Nome file CSV:** consente di personalizzare parte del nome dei file
csv prodotti da Passweb aggiungendogli una specifica stringa.

**ATTENZIONE!** Il campo "Nome file CSV" consente di personalizzare solo
parte del nome dei file prodotti da Passweb

In generale occorre infatti considerare che Passweb genererà un file csv
distinto per ogni singola lista di vendita con un nome del tipo:

**Articoli_idListaVendita_NomeFileCSV.csv**

dove

- **Articoli\_** è una parte non modificabile del nome file

- **idListaVendita\_** è una parte non modificabile del nome file che
  indica l'**id** della lista di vendita cui appartengono gli articoli
  presenti nel file csv.

- **NomeFileCSV** è la parte variante del nome file determinata sulla
  base della stringa impostata per il campo "Nome File CSV"

**ATTENZIONE!** una volta impostato un determinato valore all'interno
del campo "Nome file CSV" si consiglia di non andare poi a modificarlo.

In caso contrario infatti il nome dei file CSV prodotti da Passweb
cambierà e, tipicamente, sarà poi necessario andare a riconfigurare
anche le impostazioni del relativo Feed Articoli sulla piattaforma terza
per fare in modo che possa effettivamente essere recuperato il file
corretto.

In questo senso infatti è bene sottolineare che in fase di salvataggio
sul repository esterno dei file prodotti a seguito della pubblicazione
di una determinata lista articoli, Passweb controllerà, per prima cosa,
se nella cartella indicata sono già presenti file dello stesso tipo
inseriti a seguito di pubblicazioni precedenti (**il controllo verrà
effettuato analizzando le parti invarianti del nome file**) e:

- in caso positivo eliminerà questi file sostituendoli con quelli
  prodotti dalla pubblicazione in corso. Il nome dei nuovi file resterà
  dunque invariato a patto di non andare a modificare tra una
  pubblicazione e l'altra la sua parte invariante ossia quanto inserito
  all'interno del campo "Nome file CSV"

- in caso negativo Passweb provvederà semplicemente a creare da zero il
  nuovo file senza preoccuparsi di cancellare eventuali altri file
  presenti nella stessa cartella di appoggio

In queste condizioni dunque, nel momento in cui si dovesse modificare,
tra una pubblicazione e l'altra, per una qualsiasi ragione, uno degli
elementi invarianti del nome file, a seguito di una nuova pubblicazione
verranno creati sempre e comunque dei nuovi file seguendo le specifiche
indicate all'interno di questo capitolo.

**ATTENZIONE!** Il pulsante "**Scarica File CSV di esempio**" consente
di scaricare uno zip contenente degli esempi di file csv che possono
essere prodotti da Passweb a seguito di una pubblicazione articoli

Una volta compreso come impostare Passweb per creare i file CSV, resta
ora da capire come gestirne il contenuto e come renderli effettivamente
disponibili alla piattaforma terza.

In questo senso, per quel che riguarda la gestione dei contenuti il
tutto dipende, essenzialmente, da come verrà poi impostata l'Inserzione
utilizzata per la pubblicazione e da quelli che saranno i campi per essa
gestiti.

**E' con l'Inserzione che andremo a definire esattamente quali
informazioni dovranno essere passate alla piattaforma terza e quali
campi del file CSV dovranno quindi essere valorizzati per ogni singolo
prodotto coinvolto.**

Dal punto di vista strutturale infatti, i file csv prodotti da Passweb
per la pubblicazione verso Google Merchant avranno, in testata, tutti i
campi richiesti dalla piattaforma terza

Per quel che riguarda invece le singole entry dei file csv, i valori
presenti per ogni riga (e quindi per ogni articolo) in corrispondenza
della relativa colonna dipenderanno dal fatto di aver inserito o meno la
corrispondente specifica nell'Inserzione utilizzata per la pubblicazione
e, ovviamente, da come questa stessa specifica è stata mappata e
valorizzata.

In virtù di ciò, nel momento in cui nell'Inserzione utilizzata per la
pubblicazione dovesse essere gestita, ad esempio, la specifica
"**materiale (material)**" allora le righe del file csv relative agli
articoli pubblicati mediante l'Inserzione in esame avranno la
corrispondente colonna "**Material**" valorizzata con il "materiale" dei
corrispondenti prodotti, informazione questa che verrà prelevata
esattamente dal campo impostato in fase di mapping della relativa
specifica.

Se invece la specifiche "**materiale (material)**" non dovesse essere
gestita nell'Inserzione, il file csv manterrà comunque a livello di
intestazione la relativa colonna ma, in questo caso, per ogni articolo
coinvolto nell'Inserzione, e quindi per ogni singola riga del file csv,
il campo corrispondente a questa colonna sarà, ovviamente, privo di
valori.

Infine, occorre anche considerare che:

- determinati campi del file csv, per ovvie ragioni, saranno sempre
  valorizzati indipendentemente da quelle che sono le specifiche
  effettivamente gestite nella corrispondente Inserzione. E' il caso ad
  esempio:

  - del **codice articolo** che verrà sempre inserito in corrispondenza
    della colonna "**Id**"

  - del **prezzo articolo** che verrà sempre inserito in corrispondenza
    della colonna "**Price**"

  - ...

- Per i campi che accettano valori multipli e che sono gestiti in
  automatico da Passweb come carattere di separazione dei singoli valori
  verrà utilizzata sempre la ","

> Ovviamente nel momento in cui il campo che accetta valori multipli
> dovesse essere gestito con una specifica mappata, ad esempio, con un
> Attributo Passweb, la valorizzazione del relativo attributo dovrà
> essere gestita manualmente utilizzando anche come separatore dei
> singoli valori un carattere adeguato.

**ATTENZIONE!** Così come è indispensabile non modificare manualmente il
nome dei file prodotti da Passweb **allo stesso modo e per ovvie ragioni
è di fondamentale importanza non alterare in nessun modo neppure la
struttura di questi stessi file**

E' ovviamente possibile prelevare i file dal Repository in cui Passweb
andrà a salvarli per poi modificarli ed elaborarli secondo le specifiche
esigenze del caso ma fintantoché verranno lasciati all'interno di questo
repository, la loro struttura non dovrà essere modificata in alcun modo.
Andando infatti a eliminare, rinominare o aggiungere manualmente campi
alla struttura di base si correrà il rischio di compromettere le
successive pubblicazioni creando dei tracciati non più gestibili in
maniera corretta.

Per quel che riguarda infine la modalità attraverso cui rendere
disponibili i file prodotti da Passweb e come caricare effettivamente i
dati contenuti in questi file sulla piattaforma terza, il tutto
dipenderà essenzialmente da come verranno impostati i campi presenti
nella sezione "**Repository**" dal tab "Metodi di pubblicazione"

![](./assets/media/image444.png)

In questo senso infatti il campo:

**Repository CSV:** consente di impostare, selezionandola da un apposito
menu a tendina, la particolare tipologia di Repository in cui Passweb
dovrà andare a salvare i file csv prodotti a seguito di ogni
pubblicazione articoli. E' possibile selezionare uno dei seguenti
valori:

- **Non gestito**: selezionando questa opzione non verrà utilizzato
  nessun Repository per cui i file csv prodotti da Passweb a seguito di
  ogni pubblicazione dovranno essere poi scaricati manualmente operando
  all'interno del tab "**Download CSV**" presente nella maschera di
  configurazione dell'Account

- **FTP:** in questo caso, al termine di ogni pubblicazione, i file
  prodotti da Passweb verranno copiati in un' apposita cartella
  all'interno di un' area FTP

- **Google Drive:** in questo caso, al termine di ogni pubblicazione, i
  file prodotti da Passweb verranno copiati in una specifica cartella
  Google Drive

- **URL Passweb:** selezionando questa opzione i file prodotti da
  Passweb al termine di ogni pubblicazione non verranno copiati in
  nessun repository ma saranno accessibili direttamente via web a
  specifici indirizzi sotto il dominio assegnato al proprio connettore
  Passweb

Ovviamente a seconda della particolare tipologia selezionata andranno
poi settati altri parametri di configurazione necessari a Passweb per
potersi effettivamente connettere con quello specifico repository.

Per maggiori informazioni relativamente a come poter configurare il
collegamento con ciascuno dei repository sopra riportati si veda quanto
indicato nei successivi capitoli di questo manuale

####### **DOWNLOAD MANUALE**

Nel momento in cui l'esigenza dovesse essere quella di gestire i file
csv prodotti da Passweb in maniera completamente manuale, e senza quindi
ricorrere a nessun Repository, sarà sufficiente impostare il parametro
"**Repository CSV**" sull'opzione "**Non gestito**"

![](./assets/media/image445.png)

In queste condizioni dunque a seguito di ogni operazione di
pubblicazione articoli (indipendentemente dal fatto che sia una
pubblicazione lanciata manualmente o eseguita in automatico) i file CSV
prodotti da Passweb non verranno copiati in nessun Repository e dovranno
quindi essere scaricati in maniera manuale operando all'interno del tab
"**Download CSV**" presente anch'esso nella maschera di configurazione
del relativo Account

![](./assets/media/image446.png)

All'interno di questa sezione, visibile solo nel momento in cui per
l'Account in esame si stia utilizzando un metodo di pubblicazione
articoli via CSV, è infatti presente l'elenco dei vari file prodotti da
Passweb a seguito delle ultime pubblicazioni effettuate.

**ATTENZIONE! Passweb conserva uno storico dei file relativo alle ultime
10 pubblicazioni**

Per ciascuno degli elementi presenti in elenco è indicata (colonna
"**Data Ora Creazione**") data e ora in cui è stata effettuata la
pubblicazione articoli che ha prodotto poi i relativi file.

I pulsanti presenti in corrispondenza delle colonne "**Elimina**" e
"**Scarica**" consentono invece di:

**Elimina** (
![Videate\\pulsante_elimina_backup_marketplace.bmp](./assets/media/image447.png) ): consente di eliminare definitivamente
i file csv prodotti dalla corrispondente pubblicazione.

**Scarica** (
![Videate\\pulsante_scarica_backup_marketplace.bmp](./assets/media/image448.png) ): consente di effettuare il download
dei relativi file csv.

**ATTENZIONE!** In queste condizioni Passweb si preoccuperà solamente di
creare, a seguito di ogni pubblicazione, i relativi file CSV. Tali file
non saranno quindi disponibili attraverso nessuna area comune per cui
l'unica possibilità sarà poi quella di scaricarli dal Wizard e caricarli
manualmente all'interno del Merchant Center

Per far questo sarà necessario:

- Accedere al proprio account Merchant Center, cliccare sulla voce
  "**Prodotti -- Feed**" presente nel menu di sinistra

![](./assets/media/image449.png)

> e selezionare uno dei Feed presenti in elenco (sezione "**Feed
> Principali**")
>
> **ATTENZIONE!** Il caricamento manuale di un file CSV richiede che il
> Feed di destinazione sia già presente all'interno del Merchant Center
> per cui nel momento in cui non dovesse essere presente nessun Feed la
> prima cosa da fare sarà ovviamente quella di crearne uno (pulsante +).

- Nella maschera di dettaglio del Feed selezionato cliccare sul pulsante
  "**Carica file**"

![](./assets/media/image450.png)

> Selezionare quindi il file CSV prodotto da Passweb e cliccare sul
> pulsante "**CAricamento**"

![](./assets/media/image451.png)

> Il pulsante "**Carica come prova**" consente di effettuare
> un'importazione di prova senza incorporare effettivamente nel Feed i
> dati presenti all'interno del file

Per maggiori informazioni in merito al caricamento manuale di un file
CSV in un Feed prodotti del Merchant Center si consiglia di fare sempre
riferimento alla documentazione ufficiale di Google (
<https://support.google.com/merchants/answer/188477?hl=it#zippy=%2Ccaricamento-diretto%2Coperazioni-di-recupero-pianificate%2Ccaricamento-tramite-google-cloud-storage>
)

**ATTENZIONE!** Nel momento in cui si dovesse impostare come Repository
una delle opzioni FTP, Google Drive o URL Passweb sarà poi possibile
impostare il Feed Prodotti di Google Merchant in maniera tale che vada a
recuperare automaticamente, e ad intervalli di tempo prestabiliti, i
dati presenti all'interno del file prodotto da Passweb

####### **PUBBLICAZIONE VIA FTP**

La pubblicazione via FTP consente di inserire, in maniera completamente
automatica, i file prodotti da Passweb a seguito di ogni operazione di
pubblicazione articoli (indipendentemente dal fatto che sia una
pubblicazione lanciata manualmente o eseguita in automatico a seguito ad
esempio di una sincronizzazione e/o dell'applicazione di una determinata
regola) all'interno di un'apposita area FTP rendendoli così disponibili
anche alla piattaforma terza deputata alla loro elaborazione.

Per attivare questo tipo di repository è necessario, per prima cosa,
impostare il parametro "**Repository CSV**" sull'opzione "**FTP**"

![](./assets/media/image452.png)

Fatto questo sarà poi necessario impostare anche tutta una serie di
altri parametri necessari per consentire a Passweb di accedere all'area
FTP in esame.

Nello specifico dunque il campo:

- **Username:** consente di impostare lo username di accesso all'area
  FTP in cui dovranno essere copiati i file prodotti da Passweb

- **Password:** consente di impostare la password di accesso all'area
  FTP in cui dovranno essere copiati i file prodotti da Passweb

- **Host:** consente di indicare il percorso della cartella all'interno
  dell'area FTP in cui dovranno poi essere copiati i file prodotti da
  Passweb.

> **ATTENZIONE! E' necessario indicare il percorso completo della
> cartella (comprensivo quindi del nome della cartella stessa). La
> cartella deve inoltre essere già presente all'interno dell'area ftp**

- **Porta:** consente di indicare la porta di accesso su cui è attivo il
  servizio ftp

Nel momento in cui i parametri di accesso impostati non dovessero essere
corretti e/o la cartella di destinazione non dovesse essere già presente
nell'area ftp, in fase di pubblicazione verrà ritornato un apposito
messaggio di errore

Infine, per quel che riguarda la copia dei file prodotti da Passweb
all'interno di quest'area FTP occorre ricordare che:

- **Passweb produrrà file csv distinti per ogni singola lista di
  vendita**

- **Passweb non effettuerà operazioni di cancellazione di file
  eventualmente presenti all'interno della cartella**. Un'eventuale
  eliminazione dei file prodotti da Passweb dopo che il loro contenuto è
  stato correttamente processato ed importato all'interno del Merchant
  Center rimane dunque un' operazione in carico a chi gestisce la
  relativa area FTP

- Il metodo di scrittura dei file all'interno della cartella FTP è
  regolato dal parametro "**Modalità scrittura file**" precedentemente
  esaminato

- Per garantire un funzionamento corretto della procedura è necessario,
  ovviamente, non alterare in alcun modo né il nome dei file prodotti da
  Passweb né tanto meno la loro struttura. Nel momento in cui tale
  vincolo non dovesse essere rispettato si potrebbero riscontrare
  problemi relativi al fatto che ad ogni pubblicazione Passweb andrà a
  riscrivere un nuovo file indipendentemente da quanto impostato per il
  parametro "Modalità scrittura file" o, cosa peggiore, i dati
  all'interno del file potrebbero risultare corrotti causando poi
  problemi in fase di upload all'interno della piattaforma terza.

####### **PUBBLICAZIONE VIA GOOGLE DRIVE**

La pubblicazione via Google Drive consente di inserire, in maniera
completamente automatica, i file prodotti da Passweb a seguito di ogni
operazione di pubblicazione articoli (indipendentemente dal fatto che
sia una pubblicazione lanciata manualmente o eseguita in automatico a
seguito di una sincronizzazione e/o dell'applicazione di una determinata
regola) all'interno di un'apposita cartella in uno spazio Google Drive
disponibili anche alla piattaforma terza deputata alla loro
elaborazione.

Per attivare questo tipo di repository è necessario, per prima cosa,
impostare il parametro "**Repository CSV**" sull'opzione "**Google
Drive**"

![](./assets/media/image453.png)

Fatto questo sarà poi necessario impostare anche tutta una serie di
altri parametri necessari per consentire a Passweb di connettersi
correttamente al relativo spazio di Google Drive.

Di seguito viene indicata la procedura da seguire per poter creare in
maniera corretta una cartella Google Drive e per poter reperire tutti i
parametri di configurazione necessari per consentire a Passweb di
connettersi con tale cartella.

- Accedere all'indirizzo
  [[https://console.developers.google.com]{.underline}](https://console.developers.google.com)
  utilizzando il proprio account Google

![Videate\\social_web_login23.bmp](./assets/media/image454.png)

- Aprire il menu a tendina posizionato nella parte alta della pagina e
  creare poi un nuovo progetto cliccando sulla relativa voce

![Videate\\social_web_login71.bmp](./assets/media/image455.png)

- Una volta avviata la creazione di un nuovo progetto sarà necessario
  assegnargli un nome (es. "Google Drive Prestashop") e cliccare poi sul
  pulsante **Crea**

![Videate\\social_web_login25.bmp](./assets/media/image456.png)

- Completata la creazione, accedere alla sezione "**Api e servizi
  abilitati**" del relativo progetto utilizzando la voce di menu
  presente sulla sinistra della pagina

![Videate\\prestashop_google_drive.bmp](./assets/media/image457.png)

- Accedere quindi alla sezione "**Libreria**", utilizzando anche in
  questo caso il menu posto sulla sinistra della pagina

![Videate\\prestashop_google_drive16.bmp](./assets/media/image458.png)

> Selezionare l'API relativa a Google Drive utilizzando l'apposito
> pannello di ricerca

![Videate\\prestashop_google_drive17.bmp](./assets/media/image459.png)

> e attivarla cliccando per questo sul corrispondente pulsante
> "**Abilita**"

![Videate\\prestashop_google_drive18.bmp](./assets/media/image460.png)

- Una volta abilitata l'API relativa a Google Drive accedere alla
  sezione "**Schermata consenso OAuth**"

![Videate\\prestashop_google_drive19.bmp](./assets/media/image461.png)

> Nella successiva maschera di configurazione selezionare come "**User
> Type**" l'opzione Esterno e cliccare sul pulsante **Crea**

![Videate\\prestashop_google_drive1.bmp](./assets/media/image462.png)

> **ATTENZIONE!** come indicato dal relativo messaggio l'app che andremo
> a creare sarà avviata in modalità test e sarà disponibile soltanto
> agli utenti aggiunti all'elenco degli utenti di prova. Una volta
> verificato il corretto funzionamento potrebbe poi essere necessario
> passare l'app in produzione e questo potrebbe anche richiedere una
> verifica dell'app stessa.

- Completare il form con i dati richiesti per la creazione della
  Schermata di consenso e cliccare poi sul pulsante "**Salva e
  Continua**"

![Videate\\prestashop_google_drive2.bmp](./assets/media/image463.png)

- Saltare la schermata relativa alla configurazione degli ambiti senza
  compilare nessun campo e cliccando semplicemente sul pulsante "**Salva
  e Continua**" posto nella parte bassa della pagina

![Videate\\prestashop_google_drive3.bmp](./assets/media/image464.png)

- Nella maschera di configurazione degli utenti di prova, cliccare sul
  pulsante "**Add User**" e inserire l'indirizzo mail corrispondente
  all' account Google che dovrà poi essere utilizzato per accedere
  all'app che stiamo creando e, conseguentemente, alla relativa cartella
  di Google Drive

![Videate\\prestashop_google_drive4.bmp](./assets/media/image465.png)

- Verificare, nella schermata di riepilogo che i dati inseriti siano
  corretti e cliccare quindi sul pulsante "**Torna alla Dashboard**"

![Videate\\prestashop_google_drive5.bmp](./assets/media/image466.png)

- Completata la configurazione della Schermata di consenso OAuth
  accedere alla sezione "**Credenziali**" cliccando sulla corrispondente
  voce di menu posta sulla sinistra della pagina

![Videate\\prestashop_google_drive6.bmp](./assets/media/image467.png)

- cliccare quindi sul pulsante "**Crea Credenziali**" posto nella parte
  alta della pagina e selezionare dal relativo menu a tendina la voce
  "**ID client OAuth**"

![Videate\\prestashop_google_drive7.bmp](./assets/media/image468.png)

- Selezionare all'interno del campo "**Tipo Applicazione**" l'opzione
  "**Applicazione web**" e nella sezione relativa agli **URI di
  reindirizzamento abilitati** inserire il seguente url

> **https://www.dominiosito.it/wizard/marketplace/callbackoauth2marketplace/googledrive**

![Videate\\prestashop_google_drive8.bmp](./assets/media/image469.png)

> dove ovviamente www.dominioisto.it andrà sostituito con l' url
> assegnato al proprio connettore Passweb.

- Cliccando quindi sul pulsante "**Crea**" verrà visualizzata una
  schermata con le credenziali necessarie a Passweb per potersi poi
  connettere, mediante l'app in esame, alla cartella di Google Drive in
  dovranno essere copiati i file prodotti a seguito di ogni
  pubblicazione

![Videate\\prestashop_google_drive9.bmp](./assets/media/image470.png)

> Copiare quindi il contenuto dei campi "**Il tuo ID client**" e "**Il
> tuo client Secret**" ed inserirlo, nel Wizard di Passweb,
> rispettivamente in corrispondenza dei parametri "**Client ID**" e
> "**Client Secret**" presenti all'interno della sezione Repository nel
> tab "**Metodi di pubblicazione**"

![](./assets/media/image471.png)

- Restando sempre sul Wizard di Passweb indicare all'interno del campo
  "**Nome Cartella**" il nome da assegnare alla Cartella Google Drive in
  cui verranno poi copiati i file prodotti da Passweb a seguito di ogni
  pubblicazione

> **ATTENZIONE!** a differenza della pubblicazione via FTP in questo
> caso non è necessario creare preventivamente la cartella dentro il
> proprio spazio Google Drive, sarà Passweb stesso infatti a
> preoccuparsi di crearla in fase di pubblicazione. **Una volta creata
> questa cartella è però di fondamentale importanza non modificarne il
> nome né tanto meno eliminarla**

- Una volta impostato il nome della cartella, per effettuare la
  connessione e avviare il processo di creazione della cartella stessa
  sarà necessario cliccare sul pulsante "**Genera Token**".

![](./assets/media/image472.png)

> In questo modo si verrà ricondotti alla pagina di accesso all'account
> Google **e dovremo quindi effettuare l'accesso con le credenziali
> dell'account legato all'indirizzo mail precedentemente inserito come
> utente di test per la nostra app Google**

![Videate\\prestashop_google_drive13.bmp](./assets/media/image473.png)

- Completata la fase di accesso all'account google verremo ricondotti
  nuovamente sul Wizard di Passweb dove troveremo automaticamente
  compilato il campo "**Token**" con il token di accesso che Passweb
  utilizzerà per accedere alla cartella di Google Drive

- Una volta ottenuto anche il token di accesso la configurazione sarà
  completa. Cliccando quindi sul pulsante "**Salva**" Passweb potrà
  iniziare a inserire i file prodotti a seguito di ogni pubblicazione
  articoli, nella cartella indicata sullo spazio "Google Drive" appena
  configurato

![Videate\\prestashop_google_drive15.bmp](./assets/media/image474.png)

Infine, per quel che riguarda la copia dei file prodotti da Passweb
all'interno dello spazio Google Drive occorre ricordare che:

- **Passweb produrrà file csv distinti per ogni singola lista di
  vendita**

- **Passweb non effettuerà operazioni di cancellazione di file
  eventualmente presenti all'interno della cartella**. Un'eventuale
  eliminazione dei file prodotti da Passweb dopo che il loro contenuto è
  stato correttamente processato ed importato all'interno del Merchant
  Center rimane dunque un' operazione in carico a chi gestisce la
  relativa area FTP

- Il metodo di scrittura dei file all'interno della cartella Google
  Drive è regolato dal parametro "**Modalità scrittura file**"
  precedentemente esaminato

- Per garantire un funzionamento corretto della procedura è necessario,
  ovviamente, non alterare in alcun modo né il nome dei file prodotti da
  Passweb né tanto meno la loro struttura. Nel momento in cui tale
  vincolo non dovesse essere rispettato si potrebbero riscontrare
  problemi relativi al fatto che ad ogni pubblicazione Passweb andrà a
  riscrivere un nuovo file indipendentemente da quanto impostato per il
  parametro "Modalità scrittura file" o, cosa peggiore, i dati
  all'interno del file potrebbero risultare corrotti causando poi
  problemi in fase di upload all'interno della piattaforma terza.

####### **PUBBLICAZIONE VIA URL PASSWEB**

La pubblicazione via Url Passweb consente di rendere disponibili i file
prodotti da Passweb a seguito di ogni operazione di pubblicazione
articoli (indipendentemente dal fatto che sia una pubblicazione lanciata
manualmente o eseguita in automatico a seguito di una sincronizzazione
e/o dell'applicazione di una determinata regola) via web a specifici
indirizzi sotto il dominio assegnato al proprio sito Passweb.

Per attivare questo tipo di repository è necessario impostare il
parametro "**Repository CSV**" sull'opzione "**URL Passweb**"

![](./assets/media/image475.png)

In queste condizioni non sarà necessario impostare nessun'altro
parametro di configurazione essendo i file in esame disponibili
direttamente via web a specifici indirizzi.

In questo senso per ottenere l' url dei singoli file prodotti da Passweb
sarà necessario concatenare l'indirizzo indicato all'interno del campo
"**URL**" con il nome dello specifico file che si vuole ottenere. Per
maggiori informazioni relativamente al nome assegnato da Passweb ai file
prodotti a seguito di ogni operazione di pubblicazione si veda anche
quanto indicato nel precedente capitolo "*Metodi di Pubblicazione*" di
questo manuale

Supponendo dunque di fare riferimento alla figura sopra riportata (e
all'indirizzo indicato all'interno del campo URL) e di voler accedere al
file prodotto a seguito della pubblicazione di articoli semplici
appartenenti alla lista di vendita con id 16, l' url da considerare sarà
esattamente il seguente

**https://www.clobis.net/MarketplaceFeed/2/Articoli_16_clobis.csv**

**ATTENZIONE!** anche in questo caso i dati dell'ultima pubblicazione
saranno gli unici presenti all'interno del file

###### RECUPERO PROGRAMMATO DEI FILE DA BUSINESS MERCHANT

Come evidenziato nei precedenti capitoli di questo manuale abilitando la
pubblicazione via CSV e impostando come Repository una delle opzioni
FTP, Google Drive o URL Passweb sarà poi possibile configurare il Feed
Prodotti sul Merchant Center in maniera tale che questo vada a
rileggere, ad intervalli di tempo regolari, il file CSV prodotto da
Passweb.

Considerando poi che i file prodotti da Passweb, di base, potranno
contenere sempre tutti gli articoli coinvolti nella pubblicazione
(indipendentemente dal fatto che risultino o meno variati rispetto
all'ultima pubblicazione effettuata) è semplice comprendere che,
operando in questo modo, potremo di fatto andare a ripubblicare, ad
intervalli di tempo regolari (ad esempio ogni giorno), tutta la base
dati dei prodotti presenti nel Merchant Center spostando quindi, ogni
volta, di un giorno in avanti la data di scadenza di questi stessi
prodotti che potranno così essere mantenuti nel Merchant Center anche
oltre i 30 gironi previsti.

Nel momento in cui l'esigenza dovesse essere quindi quella di creare un
Feed Prodotti sul Merchant Center con recupero programmato dei dati da
uno dei file prodotti dalla pubblicazione CSV di Passweb sarà
necessario:

- Accedere al proprio account Merchant Center, selezionare la voce
  "**Prodotti -- Feed**" presente nel menu di sinistra e cliccare sul
  pulsante raffigurante un piccolo **+** posto in corrispondenza della
  sezione "**Feed Principali**" in maniera tale da avviare la procedura
  di creazione di un nuovo Feed.

> **ATTENZIONE!** Volendo è possibile configurare il recupero
> programmato anche su di un Feed già esistente a patto che il Feed
> scelto non sia stato creato e non venga quindi alimentato via API (per
> maggiori informazioni in merito a come poter configurare il recupero
> programmato su di un Feed esistente si veda quanto indicato nel
> seguito di questo capitolo)

![](./assets/media/image476.png)

- Completare la creazione del nuovo Feed inserendo i dati necessari e
  selezionando, quando richiesto, come modalità di connessione con il
  Merchant Center il "**Recupero programmato**"

![](./assets/media/image477.png)

- Una volta selezionata l'opzione indicata in figura, cliccando sul
  pulsante "**Continua**" verrà visualizzata un'ulteriore maschera
  all'interno della quale poter indicare tutti i dati necessari per
  configurare il recupero programmato

![](./assets/media/image478.png)

> Nello specifico il campo:

- **Nome file**: consente di indicare il nome del file csv, prodotto da
  Passweb, contenente i dati dei prodotti da pubblicare all'interno del
  Merchant Center.

- **Frequenza del recupero** **/ Ora del recupero / Fuso orario:**
  consentono di impostare, rispettivamente, la frequenza (giornaliera,
  settimanale o mensile), l'orario e il relativo fuso orario in cui
  Google dovrà andare a leggere e processare il file associato al Feed
  in esame

- **URL del file:** consente di indicare l'url di accesso al file
  contente i dati dei prodotti da pubblicare all'interno del Merchant
  Center

> **ATTENZIONE!** E' richiesto l'url completo del file nella forma
> https://www.moidominio.it/fileprodotti.csv. L' url della posizione del
> file deve iniziare con http://, https://, ftp:// o sftp://.

- **Nome Utente / Password --** campi opzionali: se l'accesso al file
  dovesse essere protetto da username e password (ad esempio perché il
  file è disponibile in un'apposita area ftp) tali credenziali dovranno
  essere inserite in corrispondenza di questi campi.

> **ATTENZIONE!** Come indicato nella documentazione ufficiale messa a
> disposizione da Google
> (<https://support.google.com/merchants/answer/1219255> ), in relazione
> al recupero programmato occorre sempre ricordare che:

- Le dimensioni del file contenente i dati dei prodotti devono essere
  inferiori a 4 gigabyte (GB) e gli user-agent "Googlebot" e
  "AdsBot-Google" non possono essere bloccati dalla directory che
  contiene il feed

- L'url del file associato al Feed deve rimandare esattamente al
  relativo file

- I protocolli accettati per effettuare il recupero programmato sono
  http, https, ftp e sftp.

- Nel caso in cui si intenda effettuare il recupero programmato
  utilizzando i protocolli http, https o ftp i campi "Nome Utente" e
  "Password" sono facoltativi e se non espressamente richiesti devono
  essere lasciati vuoti

- Nel caso in cui si intenda effettuare il recupero programmato
  utilizzando il protocollo sftp i campi "Nome Utente" e "Password" sono
  obbligatori

- Nei recuperi programmati non è possibile utilizzare il server FTP o
  SFTP di Google (ftp://uploads.google.com o
  sftp://partnerupload.google.com) come URL del feed.

<!-- -->

- Dopo aver impostato la configurazione del recupero programmato,
  completare la creazione del Feed cliccando per questo sul pulsante
  "**Crea feed**" presente nella parte bassa della maschera

![](./assets/media/image479.png)

> In questo modo verremo automaticamente portati sulla maschera di
> dettaglio del Feed appena creato ma, di fatto, **non avremo ancora
> caricato nessun prodotto all'interno del Merchant Center**
>
> I prodotti verranno inseriti solo dopo che Google avrà effettivamente
> processato il file associato al Feed e questo potrà avvenire,
> ovviamente, solo nel momento indicato in fase di configurazione del
> recupero programmato.
>
> In ogni caso nel momento in cui l'esigenza dovesse essere quella di
> caricare immediatamente i prodotti senza attendere il recupero
> programmato è possibile sia effettuare un primo upload manuale del
> file, pulsante "**Carica File**", sia forzare il recupero automatico
> cliccando per questo sul pulsante "**Recupera ora**"

![](./assets/media/image480.png)

- Una volta completato il recupero del file la sezione "**In
  elaborazione**", presente nella maschera di dettaglio del Feed,
  mostrerà i risultati dell'elaborazione effettuata

![](./assets/media/image481.png)

> Portandosi all'interno di questa maschera sarà quindi possibile
> verificare la data di ultimo caricamento del file, quali prodotti sono
> inseriti correttamente nel Merchant Center, quali hanno generato degli
> errori ...

Infine, nel momento in cui l'esigenza dovesse essere quella di
modificare la pianificazione appena impostata e/o configurare il
recupero programmato su di un Feed già presente all'interno del Merchant
Center (senza quindi doverne creare per forza di cose uno nuovo) sarà
sufficiente selezionare il Feed in esame tra quelli presenti all'interno
della maschera "**Prodotti -- Feed**" precedentemente analizzata e, una
volta effettuato l'accesso alla relativa maschera di dettaglio, portarsi
nel tab "**Impostazioni**"

![](./assets/media/image482.png)

La sezione "**Pianificazione recupero**" evidenziata in figura,
consentirà di modificare / aggiungere al Feed in esame il recupero
programmato.

![](./assets/media/image483.png)

##### ARTICOLI

All'interno del tab "**Articoli**" è possibile impostare i parametri di
configurazione del proprio Account in relazione alla pubblicazione dei
prodotti sul Marketplace.

![](./assets/media/image314.png)

Il parametro "**Magazzino degli articoli**" presente all'interno della
sezione "**Generale**" consente di specificare quelli che dovranno
essere i Magazzini da collegare all'Account in esame

**ATTENZIONE!** Per poter salvare correttamente l'Account è necessario
indicare almeno un Magazzino. **Inoltre i magazzini indicati all'interno
di questa sezione saranno poi quelli che verranno presi in
considerazione per valutare la disponibilità degli articoli in fase di
applicazione di una regola per la pubblicazione automatica di questi
stessi prodotti sulla piattaforma terza**

Il check "**Invia email articoli**", presente anch'esso all'interno
della sezione "Generale" consente invece di abilitare / disabilitare
l'invio delle email relative alle operazioni di pubblicazione articoli
sul relativo marketplace.

**ATTENZIONE**! Nel momento in cui tale check dovesse essere
disabilitato, al termine di una qualsiasi operazione di pubblicazione
articoli (comprese quelle relative a regole di "Messa / Modifica /
Rimessa in Vendita" e a regole di Blocco) non verrà più inviata alcuna
mail. In queste condizioni dunque per controllare l'esito di queste
operazioni sarà necessario utilizzare gli strumenti disponibili
all'interno del Wizard (Log Articolo e Log Liste di Vendita)

Il parametro "**Elimina l'articolo in fase di arresto**" (sezione
"**Parametri Articolo**") consente invece di definire il funzionamento
dell'applicativo nel momento in cui dovesse essere applicata una regola
di Blocco o si dovesse decidere di arrestare uno o più articoli in
maniera manuale mediante il corrispondente pulsante.

In particolare:

- nel caso in cui il parametro in questione dovesse rimanere
  deselezionato (opzione di default) l'operazione di "Arresta sul
  marketplace" imposterà, di fatto, per tutti gli articoli coinvolti una
  quantità pari a 0 ponendoli quindi nello stato di "Non Disponibile"
  (Out of Stock)

> Gli articoli in questo stato continueranno ad essere presenti sul
> Merchant Center ma visualizzando la loro scheda di dettaglio troveremo
> il campo "**disponibilità**" impostato sul valore "**Non
> Disponibile**" (Out of Stock)

- nel caso in cui invece il parametro in esame dovesse essere
  selezionato, l'operazione di "Arresta sul marketplace" **andrà ad
  eliminare in maniera definitiva** dal relativo marketplace tutti i
  prodotti coinvolti in questo tipo di operazione

> **ATTENZIONE!** in queste condizioni, a seguito di un arresto, i
> prodotti eliminati dal marketplace dovranno eventualmente essere
> ripubblicati da zero

##### SCHEDULAZIONE

All'interno di questa sezione, **visibile solo nel momento in cui sia
stato impostata la pubblicazione via CSV**, è possibile schedulare le
operazioni di creazione dei vari file che dovranno poi essere dati in
pasto alla piattaforma terza

![](./assets/media/image484.png)

Relativamente alle operazioni di pubblicazione automatica dei file CSV
occorre poi tenere in considerazione alcune cose di fondamentale
importanza.

Nello specifico:

- Indipendentemente dal fatto che la pubblicazione automatica sia stata
  originata dalla pianificazione impostata all'interno di questa sezione
  del Wizard e/o dall'applicazione di una determinata regola di
  pubblicazione (es. regola di blocco, regola di messa in vendita ...)
  definita per la corrispondente inserzione e scattata a seguito di una
  sincronizzazione Sito -- Gestionale, **verranno sempre e comunque
  pubblicati tutti gli articoli di tutte le liste associate all'Account
  Google in questione**

- Nel caso di pubblicazioni manuali invece, il fatto di pubblicare o
  meno tutti gli articoli presenti in tutte le liste associate
  all'Account Google in esame dipenderà da come è stato impostato il
  parametro "**Pubblica tutti gli articoli**" presente nella sezione
  "**Metodi di pubblicazione**" della maschera "Dati Account"

- Non è ovviamente possibile eseguire, contemporaneamente, due diverse
  pubblicazioni. Ciò significa dunque che se la pubblicazione automatica
  schedulata, ad esempio, all'interno di questa sezione del Wizard
  dovesse partire mentre è già in corso un'altra pubblicazione (generata
  ad esempio a seguito di una precedente sincronizzazione sito --
  gestionale con conseguente applicazione di una regola di
  pubblicazione) questa non verrà eseguita.

- La schedulazione delle operazioni di pubblicazione automatica dei file
  CSV dovrà essere, ovviamente, coerente con il recupero programmato
  impostato nel relativo Feed del Merchant Center. Occorre quindi
  prestare particolare attenzione a non modificare il file CSV proprio
  nel momento in cui questo verrà recuperato ed elaborato da Google.

##### MARKETPLACE

All'interno di questa sezione è possibile decidere di attivare e quindi
di esportare i prodotti del proprio sito Ecommerce non solo sul
marketplace Italiano ma anche su altri Marketplace esteri.

![](./assets/media/image485.png)

La colonna "**Attivato**" consente di verificare e modificare lo stato
di attivazione del relativo Marketplace. Nello specifico l'icona:

5.  ![Videate\\marketplace_ico_attivo.bmp](./assets/media/image486.png) **:**: indica che il marketplace in
    esame è stato correttamente attivato

6.  ![Videate\\marketplace_ico_disattivo.bmp](./assets/media/image487.png): indica che il marketplace in esame
    è attualmente disattivato

**ATTENZIONE!** **per modificare lo stato di un Marketplace facendolo
passare da non attivo ad attivo è sufficiente cliccare sulla relativa
icona di stato. Una volta attivato un marketplace non sarà poi più
possibile disattivarlo**

La colonna "**Stato**" consente invece di verificare se il relativo
Marketplace necessita o meno di un aggiornamento, ad esempio perché dal
momento in cui è stato attivato possono essere cambiate le categorie
merceologiche da esso gestite.

In particolare dunque l'icona:

- ![Videate\\marketplace_ico_aggiornato.bmp](./assets/media/image488.png): indica che il marketplace in esame è
  attivato e correttamente aggiornato

- ![Videate\\marketplace_ico_no_dati.bmp](./assets/media/image489.png): indica che il marketplace in esame è
  ancora da attivare e non è quindi disponibile su Passweb la relativa
  struttura dati (es. le categorie merceologiche)

- ![Videate\\marketplace_ico_da_aggiornare.bmp](./assets/media/image490.png): indica che il marketplace in esame è
  correttamente attivato ma necessita di un aggiornamento (ad esempio
  perché può essere cambiata, rispetto al momento dell'attivazione la
  struttura delle categorie merceologiche)

- ![Videate\\marketplace_ico_aggiornamento.bmp](./assets/media/image491.png): indica che il marketplace in esame è
  in corso di aggiornamento

In fase di creazione di un' Inserzione sarà poi possibile indicare, tra
i Marketplace attivati, quello verso il quale dovranno poi essere
esportati tutti gli articoli delle Liste di Vendita che faranno uso di
quella stessa inserzione.

Per maggiori informazioni relativamente alla creazione e alla gestione
di Inserzioni e Liste di vendita si vedano anche i precedenti capitoli
di questo manuale ("*Altri Marketplace -- Gestione Inserzioni / Gestione
Liste di Vendita*").

**ATTENZIONE!** L'attivazione di eventuali Marketplace diversi da quello
italiano è indispensabile nel momento in cui si dovesse optare per una
pubblicazione via API e l'esigenza dovesse essere effettivamente quella
di esportare gli articoli non solo sul Marketplace italiano ma anche su
quelli esteri.

Nel momento in cui si dovesse invece optare per una pubblicazione via
CSV, il fatto di attivare anche altri marketplace oltre a quello
italiano non ha molta importanza.

In questo caso infatti verrà sempre creato un file csv distinto per ogni
singola lista di vendita e i dati presenti all'interno di questi stessi
file saranno quelli prelevati dai campi relativi alla lingua italiana o
ad un eventuale lingua straniera in base a quelle che sono le lingue
effettivamente gestite all'interno del sito e, ovviamente, a quella che
è la lingua associata all'Inserzione cui fanno riferimento le singole
liste di vendita.

Supponendo dunque di gestire il sito in italiano e in inglese e di avere
due distinte inserzioni, una per lingua, i file csv prodotti a seguito
della pubblicazione delle liste collegate all'Inserzione "italiana"
avranno i contenuti in italiano, mentre quelli prodotti a seguito della
pubblicazione delle liste collegate all'Inserzione "inglese" avranno i
contenuti in inglese.

Detto ciò sarà direttamente sul Merchant Center, in fase di
configurazione del Feed, che dovremo poi associare al Feed stesso uno o
più paesi (e quindi marketplace) target, la relativa lingua e il file
corretto da processare.

![](./assets/media/image492.png)

##### DOWNLOAD CSV

All'interno di questa sezione, **visibile solo nel momento in cui si
dovesse decidere di adottare come metodo di pubblicazione dei prodotti
la pubblicazione via CSV** (indipendentemente dal tipo di repository
utilizzato), sarà possibile visualizzare e gestire in maniera manuale i
vari file prodotti da Passweb a seguito di una qualsiasi operazione
(automatica o manuale) di pubblicazione / arresto articoli

![](./assets/media/image485.png)

**ATTENZIONE! Passweb conserva uno storico dei file relativo alle ultime
10 pubblicazioni effettuate**

Si ricorda inoltre che anche eventuali operazioni di "Arresto Articoli"
indipendentemente dal fatto di essere effettuate manualmente o
automaticamente a seguito dell'applicazione di una determinata regola,
verranno ovviamente considerate come delle "pubblicazioni" e produrranno
quindi, all'interno della sezione in esame, i relativi file CSV.

