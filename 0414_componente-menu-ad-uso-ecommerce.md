# COMPONENTE MENU (AD USO ECOMMERCE)



Il Componente "Menu Categoria" precedentemente esaminato, consente, come
detto, di generare dei menu gestiti in maniera completamente automatica
da Passweb sulla base delle categorie merceologiche definite sul
gestionale.

In queste condizioni non è quindi possibile, ad esempio, andare a
personalizzare una singola voce di menu, aggiungendo magari per essa una
specifica immagine di sfondo o impostando anche soltanto una dimensione
differente.

Potrebbe quindi nascere l'esigenza da parte di un utente di voler
inserire all'interno del sito qualcosa di simile ad un menu di categoria
da poter però personalizzare per singola voce (a scapito ovviamente di
tutti gli automatismi legati al menu di categoria articoli).

Per soddisfare questo tipo di esigenze sarà necessario ricorrere al
Componente **"Menu"**, Componente questo che, nel caso di siti
E-Commerce, può offrire anche una struttura ed una gestione simili a
quelle appena esaminate per il Componente **"Menu Categoria"**.

Inserendo infatti un Componente "Menu" all'interno di una qualsiasi
pagina di un sito E-Commerce oltre ai normali parametri di
configurazione caratteristici di questo Componente comparirà anche il
parametro **"Link"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_generico_mapping_nodo_res.bmp](./assets/media/image268.png){width="4.613194444444445in"
height="2.9506944444444443in"}

**Link:** consente di impostare il tipo di link che dovrà essere
associato alle voci del menu che si stanno realizzando. E' possibile
selezionare uno tra i seguenti valori:

- **Crea un Link:** consente di creare un tradizionale menu di
  navigazione tra le pagine (comportamento classico del Componente
  "Menu") al quale dunque non verrà associato nessun particolare
  automatismo. Sarà quindi necessario **creare manualmente ogni singola
  voce di menu** e selezionare dal sottostante albero delle pagine (o
  dai relativi parametri) la destinazione da associare a ciascuna di
  esse.

> In queste condizioni l'esigenza iniziale potrebbe essere dunque
> soddisfatta creando in maniera manuale delle voci di menu collegate
> alle varie pagine di tipo "Catalogo" presenti all'interno del sito.
> **Ovviamente una qualsiasi variazione effettuata sul gestionale alle
> categorie merceologiche non avrebbe alcun impatto (neppure dopo una
> sincronizzazione) su questo tipo di menu che andrebbe quindi gestito
> completamente in maniera manuale.**

- **Crea una porzione di menu Autogenerata:** in questo caso una volta
  selezionata una specifica pagina radice all'interno del sottostante
  albero delle pagine, non verrà creata una singola voce di menu, ma
  verrà invece replicata in maniera completamente automatica l'intera
  struttura delle pagine presenti al di sotto di quella selezionata.

> Supponendo quindi di aver selezionato una pagina di categoria
> merceologica il risultato che otterremo sarà quello di replicare in
> maniera completamente automatica tutta la struttura di sottocategorie
> presenti a partire da quella attualmente selezionata in elenco.
>
> Nel caso in cui la pagina selezionata come Radice dovesse essere la
> pagina Catalogo sarà comunque possibile escludere dall'elenco delle
> voci di menu autogenerate pagine quali "Carrello", "Ordine" ,"Ordini"
> ecc... pagine queste che, a livello gerarchico sono collocate proprio
> sotto la pagina Catalogo, ottenendo così un vero e proprio menu di
> categoria articoli
>
> In questo senso dunque i parametri presenti all'interno della sezione
> "**Voce del Menu -- Ramo Autogenerato**" consentono rispettivamente
> di:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\voce_autogenerata_2_res.bmp](./assets/media/image269.png){width="4.613194444444445in"
height="2.938888888888889in"}

- **Includi solo le pagine di Categoria (presente solo per siti
  Ecommerce):** permette, se selezionato, di includere nell'elenco delle
  voci autogenerate solo ed esclusivamente le pagine di categoria.

> Tale parametro risulta quindi particolarmente utile nel momento in cui
> dovesse essere utilizzata come radice dell'autogenerazione la pagina
> "Catalogo".
>
> In queste condizioni sarà infatti possibile, selezionando il parametro
> in oggetto, escludere dall'elenco delle voci autogenerate pagine quali
> "Carrello", "Ordine" ,"Ordini" ecc... pagine queste che, a livello
> gerarchico sono collocate proprio sotto la pagina Catalogo, ottenendo
> così un vero e proprio menu di categoria articoli.

- **Nascondi le Categorie che non hanno articoli associati (presente
  solo per siti Ecommerce):** permette, se selezionato, di escludere
  dall'elenco delle voci autogenerate, le pagine di categoria che non
  hanno articoli associati.

- **Mappa un Ramo:** consente di selezionare la pagina Radice a partire
  dalla quale dovranno poi essere autogenerate le voci dimenu

- **Utilizza il nome dell'elemento linkato:** consente di utilizzare il
  nome di ogni singola pagina come etichetta delle varie voci di menu
  autogenerate

- **Profondità:** consente di impostare il livello di profondità per la
  visualizzazione delle voci di menu autogenerate. Impostando ad esempio
  questo campo sul valore 3 verranno visualizzate le voci di primo
  secondo e terzo livello (a partire dalla voce selezionata all'interno
  dell'albero delle pagine).

