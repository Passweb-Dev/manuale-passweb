# CATEGORIE STATISTICHE



La sezione "**Categorie Statistiche**", accessibile in Passweb dalla
voce di menu ***"Catalogo -- Gestione Articoli"***, consente di
visualizzare l'elenco delle "Categorie Statistiche" codificate nel
gestionale e correttamente gestite anche all'interno del sito.

All'interno di questa sezione verrà quindi visualizzata la maschera
"**Lista delle Categorie Statistiche Articolo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_cat_statistiche.bmp](./assets/media/image436.png)

contenente l'elenco di tutte le Categorie Statistiche definite
all'interno del gestionale e correttamente impostate per essere gestite
anche all'interno del proprio sito ecommerce.

Per ciascuna delle categorie presenti in elenco è indicato:

- L'identificativo Passweb -- colonna **ID**

- Il codice gestionale -- colonna **Codice**

- La descrizione -- colonna **Descrizione**

Una cosa particolarmente importante da sottolineare è che **nel caso di
siti Ecommerce collegati a Mexal** all'interno di questa maschera
verranno visualizzate, e saranno conseguentemente gestite all'interno
del sito, solo ed esclusivamente quelle Categorie Statistiche cui è
stata associata in Mexal una specifica descrizione.

**NOTA BENE:** oltre alle Categorie Statistiche prive di descrizione
**non** verrà gestita all'interno del sito neppure la Categoria
Statistica **con codice 00**, e questo indipendentemente dal fatto che
ad essa sia stata associata o meno una specifica descrizione.

Nel momento in cui viene codificato un nuovo articolo all'interno del
gestionale infatti, Mexal associa automaticamente questo stesso articolo
alla categoria statistica 00, indipendentemente dal fatto che questa sia
o meno una categoria effettivamente esistente (nella relativa tabella
delle categorie statistiche) e che abbia o meno una specifica
descrizione associata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\cat_statistiche_2.bmp](./assets/media/image437.png)

Per evitare quindi possibili problemi legati a questa particolare logica
di funzionamento la Categoria Statistica con codice 00 non verrà
considerata in fase di sincronizzazione e non verrà mai gestita
all'interno del sito.

In definitiva dunque per poter correttamente gestire, all'interno del
proprio sito ecommerce, le informazioni relative alla Categoria
Statistica Mexal di appartenenza di un certo articolo sarà necessario
verificare che:

a)  L'articolo in esame sia associato ad una Categoria Statistica
    diversa da quella con codice 00

b)  Sia stata definita, per la Categoria Statistica cui è associato
    l'articolo, una ben precisa descrizione, operazione questa da
    effettuarsi all'interno della relativa Tabella Mexal

**NOTA BENE:** per maggiori informazioni relativamente alla gestione in
Mexal delle Categorie Statistiche articolo si rimanda allo specifico
manale.

In ogni caso nel momento in cui un certo articolo gestito all'interno
del sito dovesse essere associato ad una Categoria Statistica priva di
descrizione, questa, come detto, non verrà considerata e, in fase di
sincronizzazione, verrà ritornato un messaggio di errore indicante il
codice della Categoria Statistica che ha generato il problema.

Nel caso invece di **siti collegati ad un gestionale Ho.Re.Ca**.
all'interno della maschera "Lista delle Categorie Statistiche Articolo"
verranno visualizzate solo ed esclusivamente quelle Categorie
Statistiche codificate all'interno del gestionale e alle quali è stato
associato almeno un articolo esportato e gestito anche all'interno del
sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_cat_statistiche.bmp](./assets/media/image438.png)

**ATTENZIONE!** Nel caso in cui una delle categorie statistiche
codificate all'interno del gestionale non compaia tra quelle in elenco è
necessario verificare che tale categoria abbia almeno un articolo
associato e che tale articolo sia stato correttamente esportato anche
all'interno del sito

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image43.png) ): consente di modificare la descrizione
in Italiano e in Lingua associata alla categoria statistica attualmente
selezionata in elenco.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Modifica Categoria Statistica Articolo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\cat_statistiche_3.bmp](./assets/media/image439.png)

attraverso cui poter gestire, nelle varie lingue, la descrizione della
relativa categoria statistica.

In questo senso occorre poi ricordare che le descrizioni in italiano
delle categorie statistiche potranno essere o meno aggiornate
automaticamente alla sincronizzazione con i relativi valori presenti nel
gestionale, dipendentemente da come è stato impostato il parametro
"**Aggiornamento descrizioni in italiano dal Gestionale -- Tabella
Categorie Statistiche Articolo**" presente alla pagina "*Configurazione
-- Sincronizzazione*" del Wizard.

> **NOTA BENE:** per maggiori informazioni relativamente al parametro in
> oggetto si veda anche la sezione "Configurazione -- Parametri di
> Sincronizzazione" di questo manuale.

A differenza delle descrizioni in italiano, quelle in lingua non
potranno invece essere prese direttamente dal gestionale e dovranno per
forza di cose essere gestite all'interno di questa sezione del Wizard.

La Categoria Statistica di appartenenza di uno specifico articolo potrà:

- essere pubblicata all'interno del sito in componenti quali il
  "Catalogo E-commerce", la "Scheda Prodotto", gli "Abbinati E-commerce"
  ecc..., utilizzando per questo il componente "Dati Articolo"
  opportunamente configurato. **In questo senso verrà pubblicata la
  Descrizione della Categoria Statistica (e non il suo Codice)**

- essere utilizzata all'interno del componente "**Filtro/Ricerca
  Catalogo Ecommerce**" per realizzare appositi filtri di ricerca (che,
  anche in questo caso, prenderanno in considerazione la Descrizione
  della Categoria e non il suo Codice).

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image114.png) ): consente di eliminare la categoria
statistica attualmente selezionata in elenco. In questo senso occorre
sottolineare come sia possibile eliminare dall'elenco solo ed
esclusivamente quelle categorie statistiche che non risultano
attualmente utilizzate all'interno del sito.

Nel caso in cui si tenti infatti di eliminare una categoria statistica
ancora associata ad un articolo gestito all'interno del sito verrà
visualizzato un apposito messaggio di errore e la categoria non verrà
eliminata.

**Esporta** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta.bmp](./assets/media/image440.png) ): consente di esportare, all'interno di un apposito
file .csv, le descrizioni delle Categorie Statistiche attualmente
presenti in elenco. Cliccando su questo pulsante verrà infatti
visualizzata la maschera "**Esportazione Categorie Statistiche
Articolo**" all'interno della quale poter configurare l'esportazione dei
dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_categorie_statistiche.bmp](./assets/media/image441.png)

Nel caso di sito in multilingua è possibile selezionare, tra quelle
attualmente gestite, la lingua in relazione alla quale dovranno essere
esportati i dati (campo **Lingua**)

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che dovrà essere utilizzato
all'interno del file di esportazione come separatore per i vari campi.

I campi presenti all'interno del file di esportazione saranno
l'identificativo Passweb della relativa categoria, il suo codice
gestionale e la relativa descrizione nella lingua selezionata

**Importa** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa.bmp](./assets/media/image134.png) ): consente di importare in maniera massiva,
utilizzando un apposito file .csv o .txt, le descrizioni di tutte le
Categorie Statistiche attualmente presenti in elenco.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Importazione Categorie Statistiche Articolo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_categorie_statistiche.bmp](./assets/media/image442.png)

all'interno della quale poter configurare l'importazione dei dati in
oggetto. In particolare il campo

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  le descrizioni che dovranno essere associate alle rispettive Categorie
  Statistiche

- **Lingua:** consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta è
necessario che il file soddisfi determinate regole. Nello specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

- L'intestazione, ossia la prima riga del file, deve contenere i due
  record "codice" e "descrizione" separati dal carattere indicato in
  all'interno del campo "**Separatore**"

- Il primo campo del file dovrà essere obbligatoriamente il **Codice
  della Categoria Statistica**. La presenza di questo campo è ovviamente
  **indispensabile** in quanto è quella che assicurerà poi
  l'associazione dei dati alle relative Nature.

> **NOTA BENE:** se all'interno del file da importare non è presente il
> Codice della Categoria Statistica e/o se i codici inseriti all'interno
> di questo campo non coincidono con quelli effettivamente presenti
> all'interno del sito la procedura di import non valorizzerà,
> ovviamente, alcun campo dati

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.**

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso da
> virgolette.
>
> Inoltre nel caso in cui il valore di un campo abbia al suo interno
> elementi racchiusi da doppi apici sarà necessario racchiudere tra
> virgolette oltre all'interno campo anche questi stessi elementi.

