# ESPORTAZIONE ORDINI



Come indicato nei precedenti capitoli di questo manuale Passweb mette a
disposizione dell'utente la possibilità di esportare i dati di ordini,
bolle, fatture, preventivi ... presenti all'interno del sito in appositi
file csv.

Per far questo è sufficiente accedere alla maschera "**Lista Ordini**"
precedentemente analizzata

![Videate\\gestione_lista_ordini2.bmp](./assets/media/image681.png)

e cliccare sul pulsante **Esportazione Ordini** (
![Videate\\pulsante_esportazione_ordini.bmp](./assets/media/image682.png) ) presente nella relativa barra degli
strumenti.

In questo modo verrà infatti visualizzata la maschera "**Esportazione
Ordini**"

![Videate\\esportazione_ordini.bmp](./assets/media/image683.png)

all'interno della quale poter impostare la tipologia di esportazione che
si intende effettuare e, ovviamente, quali documenti dovranno essere poi
presenti all'interno del file di esportazione.

Nello specifico dunque il campo:

**Separatore**: consente di definire il carattere separatore che dovrà
essere utilizzato nella creazione dei vari file csv

**Tipologia di esportazione**: consente di impostare la tipologia di
esportazione da effettuare e, conseguentemente, quella che sarà poi la
struttura dei file di esportazione. E' possibile selezionare una delle
seguenti opzioni**:**

- **Standard**: selezionando questa opzione i dati dei documenti che
  andranno poi a soddisfare l'eventuale filtro impostato all'interno del
  successivo campo, verranno esportati in un formato di tipo
  "gestionale".

> Nello specifico, in queste condizioni, verranno creati tre distinti
> file:

- **Testata.csv --** file contenente i dati di testa degli ordini
  esportati

- **Righe.csv** -- file contente i dati di riga degli ordini esportati

- **Taglie.csv** (solo Ecommerce Mexal) **--** file contenente i dati
  relativi ad eventuali articoli a taglie presenti negli ordini
  esportati

> Il campo "**id**" presente all'interno del file "Testata.csv"
> rappresenta l'identificativo del relativo documento ed è collegato al
> campo "**idDocumento**" presente all'interno del file "Righe.csv".
> Grazie a questo collegamento è quindi possibile individuare tutte le
> righe relative ad uno specifico documento.
>
> Allo stesso modo il campo "**idRigaDocumento**" presente sia
> all'interno del file "Taglie.csv" che all'interno del file "Righe.csv"
> consente di legare i dati relativi ad eventuali taglie alla rispettiva
> riga del documento.

- **Google Ads**: selezionando questa opzione i dati dei documenti che
  andranno poi a soddisfare l'eventuale filtro impostato all'interno del
  successivo campo, verranno esportati in un unico file csv la cui
  struttura e i cui dati sono esattamente quelli richiesti da Google Ads
  per fare in modo che questi stessi dati possano poi essere uplodati
  all'interno di Ads nell'ambito della procedura di import delle
  conversioni offline (per maggiori informazioni in merito si rimanda a
  quanto indicato all'interno del capitolo "*Google Ads User Provided
  data e Conversioni Avanzate -- Import delle conversioni offline*" di
  questo manuale).

> In particolare, in queste condizioni, il file di esportazione avrà una
> struttura del tipo di quella di seguito indicata
>
> *Parameters:TimeZone=+0100*
>
> *Email,Phone Number,Conversion Name,Conversion Time,Conversion
> Value,Conversion Currency,Ad User Data,Ad Personalization,Order
> ID,Google Click ID*
>
> *4320a7f0c1410f644da83b6601b44dbcb3f45922d1826a112b24a67126b52ca8,2b937f7cd69b540584db1a0529e555b60e37755e23c25e26a5285490ebb4ff16,Acquisto
> Online,2020-11-17T09:51:48,1000.00,EUR,Granted,Granted,5232,*
>
> ...
>
> dove la colonna:

- **Email**: contiene l'email hashata dell'utente che ha effettuato il
  relativo ordine

- **Phone Number**: contiene il numero di telefono hashato dell'utente
  che ha effettuato il relativo ordine

- **Conversion Name:** contiene il valore impostato in corrispondenza
  del campo "**Nome azione conversione**" presente alla pagina "Sito --
  Preferenze" del Wizard (tab "**Tracciamento Dati**" sezione "**Google
  Ads**")

> **ATTENZIONE!** è di fondamentale importanza che il nome inserito
> all'interno di questo campo coincida esattamente, anche a livello di
> spazi, lettere maiuscole e minuscole, con quello assegnato su Ads alla
> relativa azione di conversione

- **Conversion Value:** contiene il totale del relativo ordine

- **Conversion Currency**: contiene la valuta (in formato ISO) in uso al
  relativo ordine

- **Ad User Data** / **Ad Personalization**: contiene lo stato (Granted
  o Denied) dei relativi consensi marketing prestati dall'utente nel
  momento di creazione dell'ordine

- **Order ID**: contiene l'identificativo Passweb del relativo ordine

- **Google Click ID**: contiene l'eventuale valore del gclid nel momento
  in cui è stato creato l'ordine

> **ATTENZIONE!** la presenza o meno del gclid nel file di esportazione
> verso Google Ads dipende prima di tutto da come è stato settato il
> parametro "Inserisci GCLID export csv" alla pagina "Sito --
> Preferenze" del Wizard (tab "Tracciamento Dati" sezione "Google Ads")
> e poi, ovviamente, anche dal fatto che l'ordine in esame sia stato
> effettivamente generato a seguito di una visita generata da un primo
> click su di un annuncio Google Ads

**Filtro**: consente di impostare il filtro di selezione dei documenti
che dovranno poi essere inseriti all'interno dei vari file di
esportazione.

![](./assets/media/image684.png)

E' possibile impostare un filtro sulla base dei seguenti campi:

- **Articoli**: codice / titolo degli articoli presenti in ordine

- **Codice utente di fatturazione**: codice gestionale dell'utente
  intestatario del documento

- **Data Documento**: data del documento

- **ID ordine Marketplace:** id ordine sul relativo marketplace esterno
  (presente, ovviamente, solo per ordini provenienti da Amazon, eBay
  ...)

- **Inviato GADS:** stato di esportazione dell'ordine verso Google Ads
  (Vero = documento già inviato a Google Ads, Falso = documento non
  ancora inviato a Google Ads)

- **Numero documento:** identificativo Passweb dell'ordine

- **Sigla Documento:** identificativo gestionale dell'ordine

- **Stato Documento:** stato del documento (Memorizzato, Nuovo, Sospeso
  ...)

- **Tipologia Documento:** tipologia del documento (Ordine o Matrice
  Passweb)

