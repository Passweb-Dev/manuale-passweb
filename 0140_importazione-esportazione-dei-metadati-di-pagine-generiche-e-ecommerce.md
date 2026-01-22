# IMPORTAZIONE / ESPORTAZIONE DEI METADATI DI PAGINE GENERICHE E ECOMMERCE



Come evidenziato nei precedenti capitoli di questo manuale è possibile,
volendo, importare ed esportare massivamente in formato csv i dati SEO
di tutte le pagine del sito che non sono legate a specifiche categorie
merceologiche, in sostanza dunque Pagine Generiche (bianche) e Pagine di
tipo Ecommerce (verdi).

In questo senso i due pulsanti **Esporta** / **Importa** presenti nella
barra degli strumenti della maschera "**Gestione Pagine**" consentono
rispettivamente di:

**Esporta** (
![](./assets/media/image98.png) )**:** consente di esportare all'interno
di un apposito file csv i dati delle pagine del sito che non sono legate
a specifiche categorie merceologiche.

Cliccando su questo pulsante nella parte destra della maschera "Gestione
Pagine" verrà visualizzato il form "**Esporta Valori**"

![](./assets/media/image120.png)

all'interno del quale poter indicare la lingua di riferimento (campo
"**Lingua**") per la creazione del file csv e il carattere da utilizzare
come separatore (campo "**Separatore**" in fase di creazione di questo
stesso file)

Il campo chiave, all'interno del file csv, è il "**permalinkPath**"
ossia l' url relativo della specifica pagina.

Per ogni singolo record del csv, e dunque per ogni singola pagina,
verranno esportate le informazioni presenti in corrispondenza dei
seguenti campi:

- **Titolo Pagina**

- **Keywords**

- **Description**

- **Head**

**Importa** (
![](./assets/media/image99.png) )**:** consente di importare in maniera
massiva, mediante un apposito file csv, i dati SEO (**Titolo Pagina,
Keywords, Description, Head**) di tutte le pagine del sito che non sono
legate a specifiche categorie merceologiche.

Cliccando su questo pulsante nella parte destra della maschera "Gestione
Pagine" verrà visualizzato il form "**Importa Valori**"

![](./assets/media/image121.png)

mediante il quale poter effettuare l'upload del file contenente le
informazioni desiderate. Nello specifico il campo:

- **File (csv-txt):** consente di selezionare il file txt o csv da
  uplodare e contenente i dati da inserire per ogni singola pagina

- **Lingua**: consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta e i
dati contenuti nel file possano essere associati alle relative pagine,
dovranno essere rispettate delle regole ben precise. Nello specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- L'intestazione, ossia la prima riga del file, deve essere del tipo di
  quella di seguito indicata

> **permalinkPath;title;keywords;description;metatag**
>
> Il campo **permalinkPath** verrà utilizzato come campo chiave. In
> corrispondenza di questo campo, per ogni singolo record del file,
> dovrà quindi essere inserito l' url relativo della specifica pagina
> (es. *catalogo-articoli/carrello* )

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.**

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso tra
> virgolette ("").
>
> **Inoltre nel momento in cui il valore da inserire all'interno di un
> campo (principalmente all'interno del campo Head) dovesse avere al suo
> interno elementi racchiusi da doppi apici (come potrebbe ad esempio
> avvenire nel caso di codice HTML) sarà necessario racchiudere tra
> virgolette, oltre all'intero campo, anche questi stessi elementi**.
>
> Supponendo dunque di voler inserire all'interno del campo Head di una
> determinata pagina il seguente meta tag
>
> \< meta name=\"apple-itunes-app\" content=\"app-id=123456789\"\>
>
> il valore da indicare per il campo metatag nel corrispondente record
> del file csv dovrà essere esattamente il seguente
>
> "\<meta name=""apple-itunes-app"" content=""app-id=123456789""\>"

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento.

Nel momento in cui non si dovesse essere certi della correttezza del
formato del file di importazione è consigliabile inserire manualmente,
per alcune pagine, i dati richiesti ed effettuare poi un'esportazione in
maniera tale da poter disporre di un esempio di quello che dovrebbe poi
essere il formato corretto del file da importare.

**ATTENZIONE!! La procedura di import sovrascriverà eventuali dati già
presenti all'interno del sito**

**ATTENZIONE!** **Nel momento in cui si dovesse decidere di effettuare
una modifica massiva dei contenuti SEO delle pagine mediante import di
file csv è sempre consigliabile effettuare prima un backup dei contenuti
attualmente gestiti mediante l'apposita funzione di export in maniera
tale da poterlo poi ripristinare nel caso in cui dovessero verificarsi
problemi di qualsiasi tipo**

