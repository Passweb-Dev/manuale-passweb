# CATEGORIE STATISTICHE



La pagina **"Categorie Statistiche"** accessibile, solo per i siti
Ecommerce collegati a Mexal, dalla voce di menu ***"Utenti --
Configurazione Utenti Sito"*** consente di visualizzare e gestire le
descrizioni delle Categorie Statistiche utente che potranno poi essere
utilizzate all'interno del sito in fase di registrazione di un nuovo
utente e/o di variazione dei dati di un utente già registrato.

All'interno di questa pagina verrà quindi visualizzata la maschera
**"Lista delle Categorie Statistiche Cliente"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_categorie_statistiche_cliente.bmp](./assets/media/image216.png)

contente tutte le 99 categorie definite all'interno del gestionale e
gestite anche all'interno del proprio sito ecommerce.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![Videate\\icona_elimina_filtro.bmp](./assets/media/image29.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![Videate\\icona_ordinamento_griglia.bmp](./assets/media/image37.png) )

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

**Modifica**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image116.png) ): consente di gestire la descrizione in
Italiano e in Lingua associata alla Categoria Statistica attualmente
selezionata in elenco.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Modifica Categoria Statistica Cliente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_categoria_statistica_cliente.bmp](./assets/media/image217.png)

attraverso cui poter gestire, nelle varie lingue, la descrizione della
relativa Categoria.

In questo senso occorre ricordare anche che le descrizioni in italiano
delle Categorie Statistiche cliente potranno essere o meno aggiornate
automaticamente alla sincronizzazione con i relativi valori presenti nel
gestionale, dipendentemente da come è stato impostato il parametro
"**Aggiornamento descrizioni in italiano dal Gestionale -- Tabella
Categorie Statistiche Clienti**" presente alla pagina "*Configurazione
-- Parametri di Sincronizzazione*" del Wizard.

> ***NOTA BENE:** per maggiori informazioni relativamente al parametro
> in oggetto si veda anche la sezione "Configurazione -- Parametri di
> Sincronizzazione" di questo manuale.*

A differenza delle descrizioni in italiano, **quelle in lingua non
potranno invece essere prese direttamente dal gestionale e dovranno per
forza di cose essere gestite all'interno di questa sezione del Wizard.**

**ATTENZIONE!** all'interno del sito verranno visualizzate, nel relativo
componente (Campo Lista Valori) solo ed esclusivamente le Categorie
Statistiche per le quali è stata impostata una specifica descrizione.

Per maggiori informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Componenti Interazione Utente -- Componenti
Interni ai Componenti Interazione Utente -- Campo Lista Valori*" di
questo manuale

**Esporta** (
![Videate\\pulsante_esporta.bmp](./assets/media/image218.png) ): consente di esportare, all'interno di un apposito
file .csv, le descrizioni delle Categorie Statistiche cliente
attualmente presenti in elenco. Cliccando su questo pulsante verrà
infatti visualizzata la maschera "**Esportazione Categorie Statistiche
Cliente**" all'interno della quale poter configurare l'esportazione dei
dati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_categorie_statiostiche_cliente.bmp](./assets/media/image219.png)

Nel caso di sito in multilingua è possibile selezionare, tra quelle
attualmente gestite, la lingua in relazione alla quale dovranno essere
esportati i dati (campo **Lingua**)

Il campo **Separatore** consente invece di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che dovrà essere utilizzato
all'interno del file di esportazione come separatore per i vari campi.

I campi presenti all'interno del file di esportazione saranno ovviamente
il codice della Categoria e la relativa descrizione nella lingua
selezionata

**Importa** (
![Videate\\pulsante_importa.bmp](./assets/media/image220.png) ): consente di importare in maniera massiva,
utilizzando un apposito file .csv o .txt, le descrizioni di tutte le
Categorie Statistiche attualmente presenti in elenco.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Importazione Categorie Statistiche Cliente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_categorie_statistiche_cliente.bmp](./assets/media/image221.png)

all'interno della quale poter configurare l'importazione dei dati in
oggetto. In particolare il campo

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  le descrizioni che dovranno essere associate alle rispettive Categorie

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
  l'associazione dei dati alle relative Categorie.

> ***NOTA BENE:** se all'interno del file da importare non è presente il
> Codice della Categoria e/o se i codici inseriti all'interno di questo
> campo non coincidono con quelli effettivamente presenti all'interno
> del sito la procedura di import non valorizzerà, ovviamente, alcun
> campo dati*

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.**

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, e/o lo stesso carattere
> utilizzato anche come separatore sia necessariamente racchiuso tra
> virgolette.
>
> Inoltre nel caso in cui il valore di un campo abbia al suo interno
> elementi racchiusi da doppi apici sarà necessario racchiudere tra
> virgolette oltre all'interno campo anche questi stessi elementi.

