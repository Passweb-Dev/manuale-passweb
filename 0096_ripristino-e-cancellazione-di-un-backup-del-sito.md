# RIPRISTINO E CANCELLAZIONE DI UN BACKUP DEL SITO



Per eliminare una copia di backup, **aumentando così lo spazio su disco
residuo**, è sufficiente selezionare il Backup desiderato nell'elenco
dei backup salvati, e cliccare poi sul pulsante **"Elimina"** presente
nella relativa barra degli strumenti.

Per ripristinare invece una copia di backup, sarà sufficiente
selezionare la copia desiderata all'interno dell'elenco dei backup
salvati, e cliccare questa volta sul pulsante **"Ripristina".**

In particolare nel caso in cui si desideri **ripristinare un Backup
Grafico** la procedura di ripristino si comporterà esattamente allo
stesso modo di quella di importazione di un nuovo modello.

Per prima cosa, sarà quindi necessario considerare che **un Backup
Grafico verrà sempre ripristinato sulla Variante Sito attualmente
caricata all'interno del Wizard.** Prima di procedere al ripristino
occorre quindi fare particolare attenzione al fatto di avere
effettivamente caricato all'interno dell'ambiente di sviluppo la
Variante su cui si desidera effettuare il ripristino.

Inoltre, nel caso in cui all'interno del proprio ambiente di sviluppo
siano gestite più Varianti, prima di applicare la Copia di Backup
selezionata verrà richiesto di indicare il nome di una specifica
cartella, che verrà poi creata in "Gestione Risorse del sito" e
all'interno della quale verranno inserite tutte le risorse della copia
selezionata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importa_modello_variante.bmp](./assets/media/image468.png){width="2.279166666666667in"
height="1.3895833333333334in"}

**ATTENZIONE!!! Nel caso in cui l'utente decidesse di non indicare una
specifica cartella le risorse della copia selezionata potrebbero andare
a sovrascrivere eventuali file con lo stesso nome attualmente utilizzati
in altre Varianti (tra cui anche quella Online )**

Nel caso in cui invece all'interno del proprio ambiente di sviluppo sia
presente una sola Variante, ripristinando un Backup Grafico tutte le
risorse attualmente utilizzate per quella Variante verranno eliminate e
sostituite con quelle del Backup.

Per quel che riguarda invece le immagini articolo queste resteranno
comunque invariate, indipendentemente dalla particolare copia o variante
considerata, mentre per quel che riguarda le loro dimensioni occorre
considerare che:

- nel caso in cui all'interno del proprio ambiente di sviluppo sia
  presente una sola Variante, a seguito del ripristino di un Backup
  Grafico le immagini articolo verranno ridimensionate e adattate alla
  impostazioni presenti all'interno della Copia di Backup considerata

- nel caso in cui, invece, all'interno del proprio ambiente di sviluppo
  siano presenti più Varianti, a seguito del ripristino di un Backup
  Grafico sulla Variante attualmente caricata all'interno del Wizard, la
  dimensione delle immagini articolo resterà invariata e non verranno
  quindi considerate eventuali indicazioni in tal senso presenti
  all'interno della copia ripristinata. In questo modo si eviterà di
  alterare la grafica delle altre Varianti (compresa quella Online)
  presenti sul sito.

**Infine, a differenza di quanto avviene applicando un nuovo modello di
sito, ripristinando un backup grafico verrà ripristinata anche la
specifica struttura di tutte le pagine di tipo Catalogo e Prodotto
presenti all'interno della copia di backup.**

Sotto questo punto di vista occorre comunque ricordare che, se
all'interno del sito, nel momento in cui si decide di ripristinare un
backup grafico, non sono presenti le stesse categorie merceologiche e
conseguentemente le stesse pagine di tipo "Catalogo" presenti invece nel
momento in cui è stata effettuata la copia di backup che si intende
ripristinare, allora:

- le pagine di tipo Catalogo e quelle di tipo Prodotto presenti nella
  copia di backup e corrispondenti a categorie merceologiche non più
  gestite verranno eliminate.

- nuove categorie merceologiche, attualmente presenti all'interno del
  sito e non gestite all'interno della copia di backup, daranno origine,
  una volta effettuato il ripristino, a nuove pagine di tipo Catalogo e
  di tipo Prodotto con la stessa struttura grafica, e conseguentemente
  con lo stesso insieme di componenti, presenti all'interno,
  rispettivamente, della pagina "Negozio" e della pagina "Prodotto"
  della copia di backup che si sta ripristinando.

**NOTA BENE:** ripristinando un Backup Grafico non verranno alterati o
modificati in alcun modo ne i parametri di configurazione ne tanto meno
articoli, ordini o clienti attualmente presenti sul sito al momento del
ripristino**.**

