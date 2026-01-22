# IMPORTAZIONE / ESPORTAZIONE MASSIVA DEI PUNTI VENDITA



Come indicato nel precedente capitolo di questo manuale, volendo, è
possibile esportare e/o importare in maniera massiva i dati dei punti
vendita gestiti all'interno del proprio sito utilizzando file .csv /
.txt appositamente strutturati.

In questo senso la cosa importante da tenere sempre ben presente **è che
l'operazione di import mediante file csv consente unicamente di
modificare in maniera massiva i dati dei punti vendita attualmente
presenti in elenco ma non di crearne di nuovi**

La creazione di un nuovo punto vendita all'interno del sito dovrà quindi
avvenire, dipendentemente dalla tipologia di gestionale utilizzata,
secondo quanto indicato nel precedente capitolo di questo manuale.

I due pulsanti **Esporta**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta.bmp](./assets/media/image367.png) ) / **Importa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa.bmp](./assets/media/image368.png) ) presenti nella barra degli strumenti
della machera "Lista dei Punti Vendita" consentono di avviare le
relative procedure.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\import_esport_punti_vendita.bmp](./assets/media/image369.png)

Nello specifico dunque il pulsante:

**Esporta**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta.bmp](./assets/media/image367.png) ) consente di esportare, all'interno di un apposito
file .csv i dati di tutti i Punti Vendita attualmente presenti in
elenco. Cliccando su questo pulsante verrà infatti visualizzata la
maschera "**Esportazione Punti Vendita**" all'interno della quale poter
configurare l'esportazione dei dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esporta_punti_vendita.bmp](./assets/media/image370.png)

Nel caso di sito in multilingua è possibile selezionare, tra quelle
attualmente gestite, la lingua in relazione alla quale dovranno essere
esportati i dati (campo **Lingua**)

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che dovrà essere utilizzato
all'interno del file di esportazione come separatore per i vari campi.

All'interno del file di esportazione saranno presenti i seguenti campi:

- **id**: identificativo del punto vendita

- **abilitato**: SI se abilitato, NO se non è abilitato

- **ragioneSociale**: ragione sociale del punto vendita

- **nazione**: nazione del punto vendita

- **provincia**: provincia del punto vendita

- **localita**: localita del punto vendita

- **indirizzo**: indirizzo del punto vendita

- **cap**: cap del punto vendita

- **telefono**: telefono del punto vendita

- **fax**: fax del punto vendita

- **email**: email del punto vendita

- **coordinate**: coordinate google map del punto vendita

- **magazzino**: magazzino associato al punto vendita

- **gestionale**: SI se va indicato l\'indirizzo del punto vendita nel
  piede del documento del gestionale, NO se non va indicato

- **pagina**: pagina di dettaglio del punto vendita nella variante
  online

- **paginaApp**: pagina di dettaglio del punto vendita nell\'app del
  sito

- **descrizione**: descrizione, nella lingua indicata, del punto vendita

**Importa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa.bmp](./assets/media/image368.png) ): consente di importare, e
conseguentemente di modificare, in maniera massiva i dati di tutti i
Punti Vendita attualmente presenti in elenco.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Importa Punti Vendita**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importa_punti_vendita.bmp](./assets/media/image371.png)

all'interno della quale poter configurare l'importazione dei dati in
oggetto. In particolare il campo

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  i dati dei Punti Vendita da modificare

- **Lingua:** consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta è
necessario che il file soddisfi determinate regole. Nello specifico:

- Il file da importare deve avere estensione .csv o .txt

<!-- -->

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.**

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso da
> virgolette.

- L'intestazione, ossia la prima riga del file, deve necessariamente
  contenere l'elenco dei nomi dei campi che dovranno poi essere
  valorizzati con i dati presenti all'interno del file stesso.

> Di seguito viene fornito l'elenco dei campi (e conseguentemente delle
> intestazioni) che sarà possibile / obbligatorio gestire all'interno
> del file di importazione

- **id**: identificativo del punto vendita -- **campo obbligatorio**

> **ATTENZIONE!** se all'interno del file da importare non è presente
> l'identificativo del Punto Vendita e/o se gli identificativi
> utilizzati non coincidono con quelli effettivamente presenti
> all'interno del sito la procedura di import non valorizzerà,
> ovviamente, alcun campo dati

- **abilitato**: SI se abilitato, NO se non è abilitato

- **ragioneSociale**: ragione sociale del punto vendita -- **solo per
  siti collegati con gestionali Ho.Re.Ca.**

- nazione: nazione del punto vendita. Deve essere indicato il nome della
  nazione -- **solo per siti collegati con gestionali Ho.Re.Ca.**

- **provincia**: provincia del punto vendita. Deve essere indicato il
  nome della provincia -- **solo per siti collegati con gestionali
  Ho.Re.Ca.**

- **localita**: localita del punto vendita -- **solo per siti collegati
  con gestionali Ho.Re.Ca.**

- **indirizzo**: indirizzo del punto vendita -- **solo per siti
  collegati con gestionali Ho.Re.Ca.**

- **cap**: cap del punto vendita -- **solo per siti collegati con
  gestionali Ho.Re.Ca.**

- **telefono**: telefono del punto vendita -- **solo per siti collegati
  con gestionali Ho.Re.Ca.**

- **fax**: fax del punto vendita -- **solo per siti collegati con
  gestionali Ho.Re.Ca.**

- **email**: email del punto vendita -- **solo per siti collegati con
  gestionali Ho.Re.Ca.**

- **coordinate**: coordinate google map del punto vendita

- **magazzino**: magazzino associato al punto vendita. Deve essere
  indicato il nome del magazzino

- **gestionale**: SI se va indicato l' indirizzo del punto vendita nel
  piede del documento del gestionale, NO se non va indicato

- **pagina**: pagina di dettaglio del punto vendita nella variante
  online. Deve essere indicato il permalinkPath della pagina nella
  variante online.

> Es. se l\'url della pagina è http://www.sito.it/negozi/negozio1 il
> permalinkPath da indicare per il campo in questione sarà
> "negozi/negozio1"

- **paginaApp**: pagina di dettaglio del punto vendita nell'app del
  sito. Deve essere indicato il permalinkPath della pagina nella
  variante online.

- **descrizione**: descrizione nella lingua indicata del punto vendita

> **ATTENZIONE! L'unico campo obbligatorio è il campo id. Tutti gli
> altri campi, volendo, possono anche essere omessi.**
>
> Ovviamente nel momento in cui si dovesse decidere di non inserire uno
> dei campi in esame, questo andrà tolto sia dai singoli record che
> dall'intestazione

