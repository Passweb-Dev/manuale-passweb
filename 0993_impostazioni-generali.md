# IMPOSTAZIONI GENERALI



All'interno della sezione "**Impostazioni Generali**" è possibile
settare i principali parametri di configurazione del sistema di raccolta
punti che si intende attivare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\creazione_raccolta_punti_2.bmp](./assets/media/image368.png)

Nello specifico dunque il campo:

- **Nome:** consente di impostare il nome identificativo della Raccolta
  Punti in esame, in maniera tale da poterla poi distinguere tra tutte
  le altre presenti in elenco

<!-- -->

- **Attivo:** consente, se selezionato, di attivare la Raccolta Punti in
  esame.

> **ATTENZIONE!** è possibile attivare una sola Raccolta Punti alla
> volta per cui attivando un determinato sistema di raccolta punti
> mediante il parametro in oggetto o mediante l'apposito pulsante
> presente nella barra degli strumenti della maschera "Raccolta Punti"
> tutte le altre raccolte verranno automaticamente disattivate

- **Importo coperto dai punti:** consente di specificare cosa potrà
  effettivamente coprire la conversione dei punti accumulati mediante la
  raccolta in esame. E' possibile selezionare una delle seguenti
  opzioni:

  - **Totale Ordine:** selezionando questa opzione i punti accumulati
    mediante la raccolta in esame potranno essere utilizzati per coprire
    (completamente o parzialmente) il Totale Ordine (comprensivo quindi
    anche di eventuali spese di trasporto)

  - **Totale Merce Ivato:** selezionando questa opzione i punti
    accumulati mediante la raccolta in esame potranno essere utilizzati
    per coprire (completamente o parzialmente) il **Totale Merce
    ivato**.

> Selezionando questa opzione quindi **i punti non potranno essere
> utilizzati per coprire eventuali spese di trasporto.**
>
> In queste stesse condizioni, inoltre, sarà possibile definire in
> maniera specifica anche gli articoli in relazione ai quali potranno
> poi essere utilizzati i punti accumulati (campo "Filtro Articoli")

- **Totale Merce non Ivato**: selezionando questa opzione i punti
  accumulati mediante la raccolta in esame potranno essere utilizzati
  per coprire (completamente o parzialmente) il **Totale Merce non
  ivato**.

> Selezionando questa opzione quindi **i punti non potranno essere
> utilizzati per coprire né l'iva né tanto meno eventuali spese di
> trasporto.**
>
> Come per l'opzione precedente, inoltre, anche in questo caso sarà
> possibile definire in maniera specifica gli articoli in relazione ai
> quali potranno poi essere utilizzati i punti accumulati (campo "Filtro
> Articoli")

- **Filtro Articoli (solo per Importo coperto dai punti = Totale Merce
  Ivato)**: consente di impostare uno specifico filtro articoli utile
  per definire esattamente i prodotti in relazione ai quali potranno poi
  essere utilizzati i punti accumulati dagli utenti del sito (per
  maggiori informazioni in merito alla creazione di un filtro articoli
  si veda anche la sezione "*Utenti -- Gruppi Utenti Sito -- Filtri
  Utente e Filtri Articolo -- Filtri Articolo*" di questo manuale)

> **ATTENZIONE!** il campo "Filtro Articoli" verrà visualizzato solo ed
> esclusivamente nel caso in cui il precedente parametro "**Importo
> coperto dai punti**" sia stato impostato sul valore "**Totale Merce
> Ivato**"
>
> Nel momento in cui si dovesse decidere di impostare un filtro
> articoli, i punti accumulati con il sistema di raccolta in oggetto
> potranno quindi essere utilizzati solo ed esclusivamente per coprire
> il totale merce ivato degli articoli in ordine che soddisfano il
> filtro stesso.
>
> In questo senso poi occorre sottolineare che, **relativamente agli
> articoli di tipo Campionario**, la validazione del filtro impostato
> verrà fatta prendendo in considerazione l'articolo Campionario in sé
> piuttosto che i singoli Componenti dipendentemente da come è stato
> impostato il parametro "**Gestione Articoli Box**" alla pagina
> "**Configurazione Catalogo**" del Wizard.
>
> In particolare nel caso in cui il parametro in questione dovesse
> essere impostato sul valore:

- **Considera il Box** -- **opzione di default**: verrà preso in
  considerazione soltanto l'articolo Campionario.

> In questo caso dunque, la condizione che determina se per un
> determinato articolo possono o meno essere utilizzati i punti
> accumulati verrà validata prendendo in considerazione solo l'articolo
> Campionario in sé, indipendentemente dal fatto che i suoi componenti
> possano poi soddisfare o meno lo stesso filtro

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, la condizione che determina se per un
> determinato articolo possono o meno essere utilizzati i punti
> accumulati verrà validata prendendo in considerazione i componenti del
> Campionario ma non l'articolo Campionario in sé che, quindi, potrebbe
> anche non soddisfare il filtro impostato.

- **Arrotondamento punti copertura:** consente di indicare il tipo di
  arrotondamento che dovrà essere utilizzato per determinare i punti
  effettivamente utilizzabili in fase di ordine. E' possibile
  selezionare uno dei seguenti valori:

  - **Inferiore:** selezionando questa opzione il numero di punti
    effettivamente utilizzabili in fase di ordine verrà arrotondato per
    difetto rispetto al Totale Merce / Ordine.

> Supponendo dunque di essere nelle condizioni in cui un punto vale 2€ e
> di avere un totale, in relazione al quale poter utilizzare il saldo
> punti, di 47€ l'applicazione proporrà l'utilizzo massimo di 23 punti
> (pari a 46€)

- **Superiore:** selezionando questa opzione il numero di punti
  effettivamente utilizzabili in fase di ordine verrà arrotondato per
  eccesso rispetto al Totale Merce / Ordine.

> Supponendo dunque di essere nelle condizioni in cui un punto vale 2€ e
> di avere un totale, in relazione al quale poter utilizzare il saldo
> punti, di 47€ l'applicazione proporrà l'utilizzo massimo di 24 punti
> (pari a 48€)

- **Step Punti:** consente di impostare uno step di applicazione dei
  punti. Nel momento in cui si dovesse decidere di impostare questo
  campo, ad esempio, sul valore 10 i clienti potranno quindi utilizzare
  i punti accumulati a step di 10 alla volta (10, 20, 30 ...).

- **Conversione:** consente di indicare quello che dovrà essere, in
  relazione alla raccolta in esame, l'importo corrispondente ad un
  singolo punto.

- **Valuta di Riferimento:** consente di indicare, selezionandola tra
  quelle attualmente gestite sul sito, la valuta in cui dovrà essere
  considerato l'importo inserito per il precedente parametro
  "Conversione"

> Supponendo dunque di aver impostato il parametro "Conversione" sul
> valore 5 e aver indicato per la "Valuta di Riferimento" l'euro, ogni
> punto accumulato con la raccolta in esame avrà esattamente un valore
> di 5€

- **Articolo Utilizzo:** consente di indicare l'articolo spesa da
  inserire nel relativo documento gestionale nel momento in cui un
  utente, in fase di acquisto, dovesse decidere di utilizzare il proprio
  saldo punti.

<!-- -->

- **Limite Minimo punti Ordine:** consente di indicare il numero minimo
  di punti che dovranno essere utilizzati in fase di ordine.

> Supponendo dunque di aver impostato il parametro in oggetto sul valore
> 30 e di essere nel caso in cui per un determinato ordine il numero
> massimo di punti utilizzabili dall'utente sia di 25 (perché ad esempio
> con quei punti verrebbe coperto l'interno totale ordine), in queste
> condizioni l'applicazione non proporrà all'utente la possibilità di
> utilizzare i punti precedentemente accumulati.

- **Limite Massimo punti Ordine:** consente di specificare il numero
  massimo di punti utilizzabili in fase di Ordine

> Impostando , ad esempio, il parametro in oggetto sul valore 10 in fase
> di ordine non sarà mai possibile utilizzare un numero di punti
> superiore a 10, indipendentemente da quello che possa essere il saldo
> punti complessivo dell'utente e i vari totali del documento.

- **Data inizio utilizzo punti:** consente di impostare una data a
  partire dalla quale i punti accumulati dagli utenti potranno
  effettivamente essere utilizzati

- **Notifica Scadenza (giorni):** consente di indicare quanti giorni
  prima della scadenza dei punti dovrà essere inviata, in automatico
  dall'applicazione, la mail di "Notifica Scadenza"

> Nel caso in cui il campo dovesse essere impostato sul valore 0, la
> mail di notifica verrà inviata il giorno stesso della scadenza dei
> punti.
>
> **ATTENZIONE!** Affinchè la mail di "Notifica Scadenza" possa essere
> inviata correttamente non è sufficiente settare il parametro in esame
> ma occorre anche configurare correttamente la relativa mail
> impostandone il testo e soprattutto l'oggetto ( che determina
> l'effettiva attivazione della mail)
>
> Per maggiori informazioni in merito si veda anche il successivo
> capitolo di questo manuale

