# COLLEGAMENTO DELL'ACCOUNT VENDITORE DI EBAY AL SITO PASSWEB



Riassumendo quanto detto nei precedenti capitoli per poter completare e
testare l'integrazione del nostro sito Ecommerce tanto sull'ambiente
Sandbox di eBay quanto su quello di Produzione sono necessari:

- **Un set di Chiavi di configurazione:** associate all'applicazione
  creata all'interno dell'ambiente developer di eBay e necessarie per
  poter realizzare l'integrazione tra il proprio sito Passweb e la
  piattaforma di eBay (sia a livello di Sandbox che di ambiente di
  Produzione)

> Per maggiori informazioni in merito si veda il capitolo *"Chiavi di
> Configurazione"* d questo manuale

- **Un Account di test di eBay di tipo Venditore:** necessario per
  mettere in vendita sulla Sandbox di eBay gli articoli presenti
  all'interno del proprio sito Ecommerce

- **Un Account di test di eBay di tipo Compratore:** necessario per
  poter effettuare acquisti sulla Sandbox di eBay e testare quindi tutto
  il processo di acquisizione ordini da eBay verso il proprio sito
  Ecommerce (e da qui verso il gestionale)

> Per maggiori informazioni relativamente a come poter creare account
> Venditore e Compratore di Test sulla Sandbox di eBay si vedano i
> precedenti capitoli di questo manuale

- **Account reale di eBay di tipo Venditore:** necessario per mettere in
  vendita gli articoli presenti all'interno del proprio sito Ecommerce
  sui marketplace reali d eBay

Una volta in possesso di tutti questi elementi il passo successivo sarà
quello di collegare all\'applicazione precedentemente creata su eBay (e
al relativo set di chiavi di configurazione) gli account di tipo
Venditore in maniera tale da mettere in vendita su questa piattaforma
gli articoli presenti all\'interno del nostro sito ecommerce.

Il fatto di mettere in vendita gli articoli sulla Sandbox di eBay o sui
marketplace reali dipenderà poi dal tipo di Account Venditore che
andremo a collegare.

In questo senso infatti la sezione \"**Gestione Account**\" accessibile
dalla voce di menu **"Catalogo -- eBay"** consente, come detto, di
collegare all\'applicazione realizzata su eBay tanto un Account
Venditore di Test quanto un Account Venditore reale

Cliccando sul pulsante **\"Aggiungi Account\"** ( ) presente nella barra
degli strumenti della maschera **"Lista degli Account eBay"** sarà
infatti possibile accedere alla maschera di configurazione del nuovo
Account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_nuovo_account.bmp](./assets/media/image39.png){width="5.902777777777778in"
height="3.441666666666667in"}

all\'interno della quale il campo:

- **Titolo**: consente assegnare un' etichetta identificativa
  all'Account Venditore che si sta configurando in maniera tale da
  poterlo poi riconoscere facilmente nelle successive fasi di
  pubblicazione degli articoli su eBay

- **Tipologia**: consente di definire la Tipologia dell'Account
  Venditore che si sta configurando. E' possibile selezionare uno dei
  seguenti valori:

  - **Produzione:** selezionando questa opzione l'Account configurato
    verrà collegato all'ambiente di produzione di eBay. In queste
    condizioni sarà quindi necessario fare riferimento all'Account
    Venditore reale di eBay.

> **ATTENZIONE**! Gli articoli messi in vendita tramite Account di
> questo tipo verranno pubblicati sui marketplace reali di eBay

- **Sandbox:** selezionando questa opzione l'Account configurato verrà
  collegato alla Sandbox di eBay. In queste condizioni sarà quindi
  necessario fare riferimento all'Account Venditore di test di eBay

> **ATTENZIONE!** gli articoli messi in vendita tramite Account di
> questo tipo verranno pubblicati solo ed esclusivamente nell'ambiente
> di test di eBay

**ATTENZIONE!** Si consiglia di non creare due Account dello stesso tipo
(Sandbox o Produzione) collegati allo stesso Account eBay di tipo
Venditore. Questo potrebbe infatti causare dei problemi in fase di
sincronizzazione ordini tra il proprio sito Passweb ed i Marketplace
eBay

**Nei successivi capitoli di questo manuale tutto il processo di
integrazione tra il sito Ecommerce e la piattaforma di eBay
(esportazione articoli, acquisizione ordini ecc\...) verrà descritto
facendo riferimento, per ovvie ragioni, alla Sandbox di eBay. Il
procedimento sarà però esattamente lo stesso anche nel momento in cui si
volesse utilizzare un Account Venditore reale per mettere in vendita i
propri articoli su uno qualsiasi dei marketplace eBay gestiti**

Una volta impostati i due parametri richiesti sarà poi necessario
effettuare il collegamento tra il nuovo Account e l'applicazione
precedentemente creata nell'ambiente developer di eBay

Per fare questo è sufficiente cliccare sul pulsante **"Connessione
Account eBay"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_35.bmp](./assets/media/image40.png){width="5.902777777777778in"
height="3.441666666666667in"}

In questo modo verrà infatti aperta una connessione con eBay e,
utilizzando il set di Chiavi di Configurazioni precedentemente
impostate, verrà visualizzata una nuova pagina web mediante la quale
dovremo specificare di voler collegare ed utilizzate il nostro Account
Venditore di eBay sull'applicazione precedentemente creata nell'ambiente
developer di questa stessa piattaforma.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_nuovo_account2.bmp](./assets/media/image41.png){width="5.643055555555556in"
height="2.714583333333333in"}

**ATTENZIONE! Inserire nei campi User ID e Password le credenziali dell'
Account eBay di tipo Venditore.**

Ovviamente nel caso in cui fossimo partiti configurando, nel Wizard di
Passweb, un Account di tipo Sandbox, sarà poi necessario utilizzare, in
questa fase, le credenziali dell'Account Venditore di Test di eBay.

Nel caso in cui fossimo invece partiti da un Account di tipo Produzione
sarà necessario utilizzare le credenziali dell'Account Venditore reale
di eBay

Una volta inserite le credenziali richieste e cliccato sul pulsante
"**Sign in**" verrà visualizzata un'ulteriore pagina web contente un
messaggio di accettazione delle condizioni del servizio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_nuovo_account3.bmp](./assets/media/image42.png){width="5.643055555555556in"
height="1.7854166666666667in"}

Sarà quindi necessario cliccare sul pulsante "**I Agree"** per
confermare l'utilizzo dell'Account Venditore in questione
sull'applicazione creata nell'ambiente developer di eBay.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_36.bmp](./assets/media/image43.png){width="5.649305555555555in"
height="1.5583333333333333in"}

Tornando a visualizzare la pagina di configurazione dell' Account
all'interno del Wizard di Passweb, sarà possibile verificare l'avvenuta
integrazione tra Passweb stesso ed eBay, grazie alla presenza di un
segno di spunta accanto al pulsante "**Connessione Account eBay**".

A questo punto sarà sufficiente cliccare sul pulsante **"Salva"** per
memorizzare in Passweb l'Account appena configurato, che verrà così
inserito tra quelli presente all'interno della maschera **"Lista degli
Account eBay"**

**ATTENZIONE!** Nel caso in cui dovessero verificarsi dei problemi in
fase di integrazione, a fianco del pulsante "Connessione Account eBay"
verrà visualizzato, al posto del segno di spunta verde, un punto
esclamativo e, ovviamente, non sarà possibile confermare il nuovo
account.

La sequenza delle operazioni sopra indicate fornisce a Passweb un
gettone che verrà poi utilizzato nelle chiamate alle API eBay e che sarà
quindi garante della corretta integrazione tra le due applicazioni.

In merito a ciò è bene sottolineare anche che, in accordo con le regole
imposte dalla piattaforma eBay:

- Sono consentite un massimo di 5000 chiamate giornaliere alle API

- Il gettone fornito a Passweb direttamente da eBay ha una data di
  scadenza superata la quale perderà di validità. Tale data è indicata
  nella maschera "**Lista degli Account eBay**" all'interno della
  colonna "**Scadenza**" presente in corrispondenza di ciascuno degli
  Account presenti in elenco

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_37.bmp](./assets/media/image44.png){width="5.902777777777778in"
height="3.441666666666667in"}

**ATTENZIONE! Nel caso in cui la data di scadenza del gettone dovesse
essere stata superata la procedura di esportazione e pubblicazione degli
articoli Passweb su eBay, così come il processo di acquisizione ordini,
non funzionerà più in maniera corretta.**

Per rinnovare il gettone è sufficiente selezionare l'account in
questione, cliccare sul pulsante "**Connessione Account eBay**" e
confermare nuovamente di voler utilizzare l'Account sull'applicazione
eBay.

I pulsanti presenti nella barra degli strumenti della maschera "Lista
degli Account eBay" consentono, infine, di:

- **Aggiungi Account** ( )**:** consente di aggiungere un nuovo account
  Veditore di eBay (collegato alla Sandbox o all'ambiente di Produzione,
  secondo quanto descritto in precedenza)

- **Elimina Account** ( )**:** consente di eliminare l'account
  attualmente selezionato in elenco.

- **Sincro Ordini** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sincro_ordini_ebay.bmp](./assets/media/image45.png){width="0.50625in"
  height="0.18194444444444444in"} ): consente, nel caso in cui l'Account
  selezionato in elenco sia stato configurato per interagire con eBay
  anche a livello di ordini, di effettuare la sincronizzazione tra le
  due piattaforme importando quini in Passweb eventuali nuovi ordini, e
  relativi clienti, acquisiti direttamente sul marketplace di eBay.

> **ATTENZIONE!** la sincronizzazione tra Passweb ed eBay, con la
> conseguente eventuale importazione di nuovi ordini, **avverrà anche,
> in maniera completamente automatica, a seguito di ogni
> "Sincronizzazione Totale"** (manuale o schedulata) tra il Sito ed il
> gestionale Passepartout
>
> Per maggiori informazioni in merito si veda anche il capitolo
> "*Acquisto articoli su eBay e sincronizzazione Ordini sul gestionale*"
> di questo manuale.

- **Modifica Account** ( )**:** consente accedere alle impostazioni di
  configurazione dell'Account selezionato in elenco.

Cliccando su quest'ultimo pulsante verrà infatti visualizzata la
maschera "**Dati Account**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_38.bmp](./assets/media/image46.png){width="5.467361111111111in"
height="3.623611111111111in"}

all'interno della quale sarà possibile visualizzare (sezione
"**Generale**") le seguenti informazioni:

- **Nome:** etichetta identificativa dell'Account eBay in esame

- **Tipologia:** consente di impostare la tipologia dell'Account eBay in
  esame scegliendo, ovviamente, tra Sandbox e Produzione

- **ID Utente:** consente di visualizzare lo Username dell' Utente
  Venditore di eBay configurato sull'Account in esame

- **Data di Scadenza:** consente di visualizzare la data di scadenza del
  gettone fornito a Passweb direttamente da eBay in fase di
  configurazione e attivazione dell'Account in esame

Il check "**Invia email articoli**", presente anch'esso all'interno
della sezione "Generale" consente invece di abilitare / disabilitare
l'invio delle email relative alle operazioni di pubblicazione articoli
sul relativo marketplace.

**ATTENZIONE!** Nel momento in cui tale check dovesse essere
disabilitato, al termine di una qualsiasi operazione di pubblicazione
articoli (comprese quelle relative a regole di "Messa / Modifica /
Rimessa in Vendita" e a regole di Blocco) non verrà più inviata alcuna
mail. In queste condizioni dunque per controllare l'esito di queste
operazioni sarà necessario utilizzare gli strumenti disponibili
all'interno del Wizard (Log Articolo e Log Liste di Vendita)

All'interno della sezione "**Articoli**" è necessario impostare i
Magazzini da collegare all'Account in esame, dato questo obbligatorio
anche nel momento in cui si dovesse decidere di non effettuare
un'integrazione completa.

**ATTENZIONE! I magazzini indicati all'interno di questa sezione saranno
quelli utilizzati nei vari calcoli di disponibilità in relazione alle
diverse regole per la pubblicazione/blocco automatica di articoli sul
marketplace**

All'interno della sezione "**Ordini**" sarà infine possibile decidere se
l'Account in esame dovrà interagire o meno con eBay anche a livello di
ordini ed eventualmente in che modo.

Nello specifico il campo:

**Creare ordini in Passweb:** consente di decidere se l'Account in esame
dovrà o meno interagire con eBay a livello di ordini. E' possibile
selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione l'Account in esame potrà
  interagire con eBay (a livello di Sandbox o di marketplace reale
  dipendentemente dalla tipologia di Account considerata) **solo ed
  esclusivamente a livello di esportazione articoli**.

> **ATTENZIONE!** In queste condizioni eventuali ordini acquisiti su
> eBay a seguito dell'acquisto di articoli messi in vendita a partire da
> sito Passweb non potranno in alcun modo essere importati su Passweb,
> ne tanto meno, all'interno del gestionale.

- **Si:** selezionando questa opzione l'integrazione tra Passweb ed eBay
  sarà completa.

> Sarà quindi possibile non solo esportare articoli **ma anche importare
> all'interno del proprio sito Passweb e da qui all'interno del
> gestionali, eventuali nuovi ordini (e relativi clienti) acquisiti
> direttamente sul marketplace di eBay**

**Magazzino Ordine:** consente di indicare lo specifico magazzino che
dovrà essere utilizzato e quindi movimentato in relazione agli ordini
ricevuti dal relativo marketplace eBay.

**ATTENZIONE!** A default il campo in esame viene valorizzato con il
magazzino impostato a livello generale come magazzino degli ordini
Passweb alla pagina "*Ordini -- Gestione Ordini -- Configurazione
Ordini*" del Wizard

**Sezionale degli Ordini:** consente di indicare uno specifico
sezionale, tra quelli codificati all'interno del gestionale, in cui
verranno memorizzati gli ordini acquisiti direttamente dal relativo
marketplace di eBay

**Codici Mastro dei Clienti (solo Ecommerce Mexal)**: consente di
indicare lo specifico codice Mastro del gestionale in cui verranno poi
memorizzati i clienti acquisiti direttamente dal relativo marketplace di
eBay

**Numero Causale Movimento di Magazzino Documento**: consente di
indicare il numero della Causale che dovrà essere utilizzata,
all'interno del gestionale, per indicare che l'ordine corrispondente è
stato originato sui marketplace eBay

**ATTENZIONE!** Nel momento in cui per il campo in esame non dovesse
essere indicato uno specifico valore, come Numero della Causale del
Movimento di Magazzino verrà utilizzato quello impostato in
corrispondenza dello stesso parametro presente alla pagina "**Ordini --
Configurazione Ordini**" del Wizard

**Numero del centro di Costo/Ricavo**: consente di indicare il numero da
attribuire al campo "**Costi/ricavi",** presente nella testata del
relativo documento gestionale, nel caso in cui l'ordine provenga da un
marketplace eBay

**ATTENZIONE!** Nel momento in cui per il campo in esame non dovesse
essere indicato uno specifico valore, come Numero del centro di
Costo/Ricavo verrà utilizzato quello impostato in corrispondenza dello
stesso parametro presente alla pagina "**Ordini -- Configurazione
Ordini**" del Wizard

