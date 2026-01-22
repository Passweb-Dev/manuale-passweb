# COMPONENTE LISTA CATEGORIE



Il Componente **"Lista Categorie"** può essere inserito in una qualsiasi
pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_lista_categorie.bmp](./assets/media/image270.png)

e permette di creare, in maniera completamente automatica, un menu di
navigazione fra le varie categorie merceologiche gestite all'interno del
sito.

La struttura di navigazione del menu rifletterà esattamente la struttura
dell'albero delle categorie merceologiche definito sul gestionale,
mentre le immagini ed i testi associati ad ogni singola categoria
merceologica saranno esattamente quelli inseriti in Passweb per la
corrispondente pagina "Catalogo".

In particolare nel momento in cui il componente dovesse essere inserito:

- **all'interno di una pagina generica (pagine bianche) e/o all'interno
  di una pagina Ecommerce (pagine Verdi)** visualizzerà una cella per
  ogni categoria merceologica di livello 0 (categorie padri).

- **all'interno di una pagina catalogo (pagine blu)** potrà
  visualizzare, dipendentemente dalle impostazioni di configurazione
  (parametro "Contestuale alla pagina"), come nel caso precedente sempre
  e comunque una cella per ogni categoria merceologica di livello 0
  oppure una cella per ogni categoria figlia di quella corrispondente
  alla pagina catalogo in cui il componente stesso è stato inserito

Supponendo quindi di avere a livello zero nell'albero delle categorie
merceologiche le seguenti categorie: "Informatica", "Fotografia",
"Intrattenimento", "Televisori" e "Telefonia" inserendo il componente
all'interno della pagina Negozio o di una qualsiasi pagina generica,
esso visualizzerà, in queste condizioni, 5 distinte celle.

All'interno di ognuna di queste celle sarà poi possibile inserire
l'immagine e/o il testo della relativa categoria merceologica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_lista_categorie_esempio.bmp](./assets/media/image271.png)

Cliccando sull'immagine di una specifica categorie merceologica l'utente
potrà essere ricondotto alla relativa pagina catalogo, dove potrebbe
essere inserito un ulteriore componente "Lista categorie" che
dipendentemente dai parametri di configurazione potrebbe visualizzare
una cella per ogni singola sottocategoria merceologica figlia della
categoria associata alla Pagina Catalogo in cui il componente è stato
inserito.

In definitiva dunque l'utente potrebbe arrivare a visualizzare l'elenco
degli articoli appartenenti all'ultima categoria merceologica di un ramo
dell'albero (categoria foglia) avendo prima cliccato sull'immagine
rappresentativa delle varie categorie merceologiche padre.

