# PERSONALIZZAZIONE DEGLI ELEMENTI DI UNA SERIE DI TAGLIE / COLORI



Nel momento in cui l'esigenza dovesse essere quella di personalizzare le
descrizioni, i colori o la posizione dei vari elementi componenti una
determinata serie di Taglie / Colori, variando quindi i contenuti
prelevati dalle relative tabelle gestionali, è possibile procedere in
due modi diversi:

- Manualmente, andando a settare i parametri desiderati all'interno
  della maschera "Modifica Elementi della Serie"

- Massivamente, andando a creare ed importare appositi file .csv
  contenenti tutti i dati da inserire

Per procedere in maniera manuale è necessario selezionare, all'interno
della maschera **"Lista delle Serie"** precedentemente analizzata, la
serie in esame e cliccare poi sul pulsante **Modifica Taglie/Colori**
(![Videate\\pulsante_modifica_taglie_colori.bmp](./assets/media/image323.png) ) presente nella contestuale barra degli strumenti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_taglie_colori_generale.bmp](./assets/media/image324.png)

In questo modo sarà infatti possibile accedere alla maschera **"Modifica
Elementi della Serie"** attraverso la quale poter impostare le
descrizioni i colori e l'ordinamento dei vari elementi componenti la
serie attualmente selezionata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_elementi_serie.bmp](./assets/media/image325.png)

Nello specifico, per ciascun elemento della serie presente all'interno
di questa maschera il campo:

- **Testo:** consente di impostare manualmente, in tutte le lingue
  gestite all'interno del sito, la descrizione del relativo elemento
  della serie, sovrascrivendo eventualmente quella importata
  direttamente dal gestionale

<!-- -->

- **Colore:** consente di associare al relativo elemento della serie uno
  specifico colore

> Ovviamente il campo in esame non è obbligatorio ma si rivelerà
> particolarmente utile nel momento in cui la serie in esame dovesse
> essere utilizza per gestire dei colori soprattutto in relazione poi
> alla possibilità di attivare sul sito delle ricerche per colore
>
> **ATTENZIONE!** il colore associato ad ogni singolo elemento della
> serie non è multilingua per cui sarà esattamente lo stesso per tutte
> le lingue gestite all'interno del sito

- **Immagine di Background**: consente di associare al relativo elemento
  della serie una specifica immagine (utile ad esempio nel momento in
  cui il colore in esame non possa essere rappresentato con un semplice
  RGB).

> Anche l'Immagine di background non è, ovviamente, multilingua e non è
> neppure obbligatoria ma, come il Colore, può rivelarsi particolarmente
> utile in relazione, ad esempio, alla possibilità di attivare sul sito
> delle ricerche per colore
>
> **ATTENZIONE! "Colore" e "Immagine di background" sono due campi
> alternativi.**
>
> Ciò significa dunque che nel momento in cui dovessero essere entrambi
> valorizzati, all'interno del sito verrà comunque utilizzato uno solo
> di questi due campi **dando priorità all'Immagine di background**.
>
> La regola di base prevede dunque che, se presente nei vari controlli
> all'interno del sito, verrà visualizzata l'Immagine di background
> altrimenti (sempre se presente) verrà visualizzato il relativo Colore.

- **Posizione:** consente di indicare la posizione che dovrà assumere
  sul front end del sito, nell'elenco di selezione della taglia /
  colore, il relativo elemento della serie.

> **ATTENZIONE!** Il campo Posizione accetta solo valori numerici e
> **consente di ordinare l'elenco delle taglie / colori in maniera**
> **crescente**
>
> In considerazione di ciò è bene sottolineare anche che:

- Valorizzando il campo "Posizione" per di tutti gli elementi della
  serie, questi verranno poi ordinati, sul front end del sito in maniera
  crescente

- Nel caso in cui dovesse essere indicato un valore per il campo
  "Posizione" solo in corrispondenza di alcuni elementi della serie, sul
  front end del sito verranno visualizzati prima, con ordinamento
  crescente, gli elementi per cui è stato assegnato un valore e, a
  seguire, tutti gli altri (secondo l'ordinamento definito per essi
  all'interno del gestionale)

- Nel caso in cui per alcuni elementi della serie dovesse essere
  impostato lo stesso valore all'interno del campo "Posizione" questi
  verranno ordinati tra loro secondo quanto definito all'interno del
  gestionale

- Nel caso in cui non dovesse essere indicato alcun valore all'interno
  del campo "Posizione" per nessuno degli elementi della serie,
  l'ordinamento di questi stessi elementi sul front end del sito sarà
  esattamente quello definito all'interno del gestionale

**ATTENZIONE!** I valori inseriti per ogni elemento della serie in
corrispondenza dei campi "**Testo**", "**Colore**" o "**Immagine di
background**" saranno poi quelli visualizzati sul front end del sito:

- nel momento in cui si dovesse decidere di visualizzare in una cella
  articolo e/o nella scheda articolo le taglie/colori effettivamente
  gestite per quel determinato prodotto utilizzando in questo senso il
  componente "**Dati Articolo**" mappato sul campo "**Taglie**" o
  "**Taglie Disponibili**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dati_articolo_taglie_colori.bmp](./assets/media/image326.png)

> Per maggiori informazioni in merito alla possibilità di inserire in
> una cella articolo o nella scheda articolo le taglie/colori
> effettivamente gestite per quel determinato prodotto si veda anche
> quanto indicato all'interno del capitolo "*Varianti Sito Responsive --
> Lista Componenti Ecommerce -- Componenti interni ai componenti
> Ecommerce -- Componente Dati Articolo*" di questo manuale

- nei controlli di selezione della taglia / colore da acquistare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_colore_acquisto.bmp](./assets/media/image327.png)

- nel momento in cui si dovesse decidere di implementare dei filtri di
  ricerca articolo basati sulle taglie/colori utilizzando in questo
  senso i componenti "**Filtro Indice**", "**Filtro Checkbox**" o
  "**Filtro Lista**" mappati sul campo "**Taglie**" o "**Taglie
  Disponibili**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_articolo_taglie_colori.bmp](./assets/media/image328.png)

> **ATTENZIONE!** il colore associato al relativo elemento della serie
> di taglie/colori verrà visualizzata solo all'interno di **Filtri
> Indice,** **Filtri Checkbox** e nei **Filtri Lista**. In tutte le
> altre tipologie di controllo verrà quindi visualizzata sempre e solo
> la descrizione del relativo elemento
>
> Per maggiori informazioni in merito alla possibilità di gestire dei
> filtri di ricerca basati sulle taglie/colori si veda anche quanto
> indicato all'interno del capitolo "*Varianti Sito Responsive -- Lista
> Componenti Ecommerce -- Componenti interni ai componenti Ecommerce --
> Filtri di ricerca*" di questo manuale

Nel momento in cui l'esigenza dovesse essere invece quella di modificare
massivamente i parametri di configurazione (descrizione, posizione,
colore ...) dei vari elementi componenti la serie attualmente
selezionata in elenco sarà necessario cliccare sul pulsante "**Importa
Taglie**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_taglie.bmp](./assets/media/image322.png) ) presente anch'esso nella relativa barra degli
strumenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importa_taglie_generale.bmp](./assets/media/image329.png)

Cliccando su questo pulsante verrà infatti visualizzata la maschera
**"File Taglie"** mediante la quale poter effettuare l'upload del file
contenente tutte le informazioni desiderate.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\file_taglie.bmp](./assets/media/image330.png)

Nello specifico il campo:

- **File (csv-txt):** consente di selezionare il file txt o csv da
  uplodare contenente tutti i dati di configurazione delle singole
  taglie / colori definite per la serie in esame

- **Lingua**: consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta,
dovranno essere rispettate delle regole ben precise. Nello specifico

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- L'intestazione, ossia la prima riga del file, può contenere i campi
  "**codice**" (obbligatorio), "**descrizione**", "**colore**",
  "**immagineBackground**" e "**posizione**"

> Supponendo di aver scelto come carattere separatore il carattere ";"
> l'intestazione del file potrebbe essere del tipo
> **codice;descrizione;colore;immgineBackground;posizione**

- Per ogni singolo record del file in corrispondenza del campo
  "**codice**" sarà necessario indicare l'indice della specifica
  taglia/colore (es. 1,2,3 ecc...) cui associare la successiva
  descrizione.

![Videate\\codici_taglia.bmp](./assets/media/image331.png)

> In corrispondenza del campo "**descrizione**" (campo alfanumerico)
> andrà indicata la descrizione in lingua della relativa taglia/colore.
>
> In corrispondenza del campo "**colore**" sarà necessario indicare il
> colore da associare al relativo elemento della serie specificando il
> suo codice rgb (es. rgb(19, 163, 118) ) oppure il suo valore
> esadecimale (es. #ff2200)
>
> In corrispondenza del campo "**immagineBackground**" sarà necessario
> indicare il **percorso relativo** dell'immagine da associare alla
> relativa taglia / colore (immagine che dovrà ovviamente essere
> caricata in maniera preventiva tra le risorse utilizzabili all'interno
> del proprio sito)
>
> Supponendo dunque di aver caricato l'immagine blu.jpg all'interno
> della cartella Resources/Colori del sito il percorso da indicare nel
> file di importazione in corrispondenza del campo "immagineBackground"
> sarà "/Resources/colori/blu.jpg"
>
> Infine, in corrispondenza del campo "**posizione**" (campo numerico),
> andrà indicata, eventualmente, la posizione che il relativo elemento
> dovrà assumere, sul front end del sito, all'interno dell'elenco di
> selezione della taglia / colore.
>
> **ATTENZIONE!** L'unico campo obbligatorio è il campo codice. Tutti
> gli altri campi, volendo, possono anche essere omessi.
>
> Ovviamente nel momento in cui si dovesse decidere di non inserire uno
> dei campi in esame, questo andrà tolto sia dai singoli record che
> dall'intestazione

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.

> **ATTENZIONE**! In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso da
> virgolette.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento.

Infine, oltre all'import massivo dei dati di configurazione delle
singole Taglie / Colori, volendo è possibile avviare anche una procedura
di esportazione di questi stessi dati, operazione questa che potrebbe
rivelarsi particolarmente utile per avere un esempio chiaro di quella
che dovrà poi essere la struttura del file di importazione affinché la
relativa procedura possa terminare con successo

Cliccando quindi sul pulsante "**Esporta Taglie**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_taglie.bmp](./assets/media/image321.png) ) presente nella relativa barra degli strumenti verrà
visualizzata la maschera "**Esportazione Taglie**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_taglie.bmp](./assets/media/image332.png)

all'interno della quale poter configurare l'esportazione dei dati.

Nel caso di sito in multilingua è possibile selezionare, tra quelle
attualmente gestite, la lingua in relazione alla quale dovranno essere
esportati i dati (campo **Lingua**)

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che dovrà essere utilizzato
all'interno del file di esportazione come separatore per i vari campi.

I campi presenti all'interno del file di esportazione saranno ovviamente
il codice, la posizione, il colore, l'immagine di background e la
descrizione (nella lingua indicata) da associare alle singole taglie /
colori definite per la serie attualmente selezionata in elenco

