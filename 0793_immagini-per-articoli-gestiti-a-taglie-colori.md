# IMMAGINI PER ARTICOLI GESTITI A TAGLIE / COLORI



Nel caso di articoli gestiti a Taglie / Colori, volendo, è possibile
**associare ad ogni elemento (quindi ad ogni singola taglia/colore) di
una serie una o più immagini che verranno poi visualizzate all'interno
della scheda prodotto solo ed esclusivamente nel momento in cui l'utente
dovesse selezionare quello specifico elemento.**

**NOTA BENE:** tutte le immagini dovranno comunque essere associate al
relativo articolo.

Questo potrebbe essere particolarmente utile, ad esempio, nel caso in
cui la tabella Taglie di Mexal venga in realtà utilizzata per gestire
diversi colori di uno stesso articolo.

Per poter far questo occorrerà portarsi alla pagina *"Catalogo --
Gestione Articoli --Articoli"* del Wizard, selezionare l'articolo a
taglie/colori desiderato e cliccare sul pulsante "Risorse" presente
nella barra degli strumenti (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_risorse.bmp](./assets/media/image201.png) ) accedendo così all'elenco delle risorse
collegate all'articolo selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\risorse_articolo2.bmp](./assets/media/image342.png)

All'interno di questa maschera verranno quindi visualizzate tutte le
risorse (immagini e schede tecniche) associate allo specifico articolo.
Selezionando un'immagine tra quelle presenti in elenco e cliccando poi
sul pulsante **"Collega Serie"** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_collega_serie.bmp](./assets/media/image343.png) ) presente nella barra degli strumenti
verrà visualizzata la maschera "Serie -- Colori"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_risorse_articolo_taglie2.bmp](./assets/media/image344.png)

attraverso cui poter associare l'immagine attualmente selezionata ad uno
specifico elemento (taglia o colore) della serie.

Il pulsante **"Scollega Serie"** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_scollega_serie.bmp](./assets/media/image345.png) ) presente nella barra degli strumenti
consente di eliminare l'associazione di un'immagine ad uno specifico
elemento della serie.

**ATTENZIONE!** Le immagini non associate in maniera specifica a nessun
elemento della serie verranno sempre visualizzate all'interno della
galleria immagini della scheda prodotto. Le immagini associate ad uno
specifico elemento della serie verranno invece visualizzate solo nel
momento in cui verrà selezionato quello specifico elemento (taglia o
colore) modificando il valore della select-box (se grafica minimale) o
cliccando su una taglia (se grafica estesa).

In queste condizioni potrebbero verificarsi casi in cui una volta
effettuato l'accesso alla scheda prodotto dell'articolo in esame venga
visualizzata solo l'immagine principale dell'articolo e questo perché le
immagini secondarie, relative magari, alle diverse opzioni di colore
sono state associate allo specifico elemento e verranno quindi
visualizzate solo nel momento in cui l'utente dovesse selezionare il
colore desiderato.

Nel caso in cui l'esigenza dovesse essere invece quella di visualizzare
inizialmente tutte le immagini relative all'articolo, indipendentemente
dal fatto che queste siano state associate o meno ad uno specifico
elemento della serie, sarà necessario agire mediante i due parametri
"**Abilita il Placeholder**" e "**Placeholder**" precedentemente
esaminati (per maggiori informazioni in merito si faccia riferimento a
quanto indicato nel precedente capitolo di questo manuale)

Infine nel momento in cui si sia deciso di associare determinate
immagini a specifici elementi della serie (es. immagine rossa associata
ad elemento rosso, immagine blu associata ad elemento blu ...) andando
poi ad aggiungere questi elementi in carrello l'immagine visualizzata
sarà, anche qui, la prima di quelle associate in maniera specifica al
relativo elemento.

**ATTENZIONE**! Per fare in modo che in carrello venga effettivamente
visualizzata la prima delle immagini associate allo specifico elemento
della serie è necessario configurare l'applicativo in modo che ad ogni
aggiunta venga sempre creata una nuova riga articolo, anche nel caso in
cui l'articolo aggiunto fosse già presente in Carrello

In caso contrario (aggiornamento della stessa riga articolo già presente
in carrello) dovendo gestire, in una stessa riga più taglie / colori
verrà visualizzata, ovviamente, sempre e soltanto l'immagine del
Catalogo.

Per maggiori informazioni in merito alle modalità di aggiunta articoli
in carrello si veda anche quanto indicato all'interno del capitolo
*"Catalogo -- Configurazione Parametri Catalogo -- Catalogo Mexal /
Ho.Re.Ca -- Modalità di inserimento in carrello*" di questo manuale.

