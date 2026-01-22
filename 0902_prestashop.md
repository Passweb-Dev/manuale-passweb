# PRESTASHOP



**ATTENZIONE! Questo tipo di integrazione sfrutta le API messe a
disposizione dalla specifica installazione Prestashop**

Grazie all'integrazione tra Passweb e Prestashop è possibile:

25. Esportare gli articoli presenti su Passweb in maniera tale da
    alimentare il catalogo dei prodotti gestiti su Prestashop decidendo
    che tipo di informazioni trasferire (prezzo, descrizioni, immagini,
    attributi ...) e aggiornando automaticamente, in fase di
    sincronizzazione, queste stesse informazioni.

> **ATTENZIONE!** Allo stato attuale l'integrazione prevede la gestione
> delle seguenti tipologie di prodotti Prestashop:

- **Prodotti Semplici**

- **Prodotti con combinazioni**

> corrispondenti, di base, ad articoli Mexal di tipo A semplici, a
> confezione, a taglie / colori, e/o strutturati (articoli figlio)
>
> Il processo di esportazione dei dati articolo sulla piattaforma terza
> può avvenire in due modi differenti:

- **via API**: i dati articolo verranno trasferiti ed inseriti sulla
  piattaforma terza in maniera automatica sfruttando, appunto, le API
  messe a disposizione dalla piattaforma stessa

> In questo caso il processo di pubblicazione dipende ovviamente, oltre
> che dalle elaborazioni interne a Passweb, anche dai tempi di risposta
> delle relative API.
>
> Ipotizzando un tempo di pubblicazione del singolo articolo attorno ai
> 5 secondi la pubblicazione di 1000 articoli impiegherebbe un tempo
> pari all\'incirca a 1.5 ore. Nel momento in cui i tempi di
> pubblicazione del singolo articolo dovessero raddoppiare passando a 10
> secondi la pubblicazione di 1000 articoli impiegherebbe all\'incirca
> un tempo pari a 3 ore.
>
> **ATTENZIONE! In considerazione di ciò la pubblicazione di articoli
> via API è consigliata solo per un numero di articoli inferiore a
> 10000**
>
> Allo stesso modo si consiglia sempre di valutare preventivamente
> quelli che sono gli effettivi tempi di risposta della propria
> installazione Prestashop.

- **via CSV**: i dati articolo verranno pubblicati all'interno di
  appositi file csv. Tali file potranno poi essere scaricati
  direttamente dal Wizard di Passweb e uplodati manualmente sulla
  piattaforma terza oppure, al termine della pubblicazione, potranno
  essere copiati automaticamente all'interno di un'area condivisa (Ftp,
  Google Drive ...) stabilita in fase di configurazione dell'Account o,
  ancora, potranno essere accessibili ad un determinato url.

> In questo caso sarà possibile avere un maggior controllo relativamente
> a quelle che sono le informazioni da inserire sulla piattaforma terza
> potendo sviluppare processi personalizzati di elaborazione dei dati
> presenti all'interno dei file csv prodotti da Passweb. Allo stesso
> modo sarà possibile utilizzare anche uno dei tanti moduli di
> importazione massiva disponibili per la piattaforma terza. Infine non
> dovendo passare da chiamate API ma potendo inserire il contenuto dei
> file prodotti da Passweb direttamente nel database del proprio sito
> Prestashop anche i tempi di upload delle informazioni potrebbero
> ridursi sensibilmente rispetto ad una pubblicazione via API
>
> **ATTENZIONE**! **In ogni caso in questa configurazione un' eventuale
> elaborazione dei file csv prodotti da Passweb così come l'effettivo
> upload dei relativi dati nella piattaforma terza restano operazioni in
> carico a chi gestisce effettivamente lo specifico sito Prestashop**
>
> Per maggiori informazioni relativamente alle due diverse metodologie
> di pubblicazione articoli sulla piattaforma terza si veda anche quanto
> indicato all'interno del relativo capitolo di questo manuale
> ("*Prestashop -- Configurazione Account -- Metodi di pubblicazione*")

26. Importare in Passweb (e conseguentemente nel gestionale
    Passepartout) ordini effettuati direttamente sul sito Prestashop.
    L'inserimento di un ordine Prestashop sul gestionale Passepartout
    comporterà, eventualmente, la creazione automatica della relativa
    anagrafica cliente e di eventuali articoli non ancora presenti nella
    base dati del gestionale.

> **ATTENZIONE! A differenza della pubblicazione articoli,
> l'importazione ordini da Prestashop può avvenire unicamente via API**

