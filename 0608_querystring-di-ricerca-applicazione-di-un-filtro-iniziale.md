# QUERYSTRING DI RICERCA -- APPLICAZIONE DI UN FILTRO INIZIALE



Come evidenziato nei precedenti capitoli di questo manuale, volendo, è
possibile configurare un pannello di ricerca CMS in maniera tale che
ogni volta in cui l'utente effettuerà l'accesso alla pagina contenente
tale pannello, venga automaticamente applicato uno specifico filtro
iniziale.

Per fare questo è necessario determinare la querystring corrispondente
al filtro che si desidera applicare inizialmente e copiarla poi
all'interno del parametro "**Ricerca Iniziale**" presente nella maschera
di configurazione del componente di ricerca

Di seguito viene descritta la procedura da seguire per ottenere il
valore che dovrà poi essere inserito in corrispondenza del parametro
"Ricerca Iniziale":

1.  Accedere al live editing del proprio sito e aprire la maschera di
    gestione delle Varianti

![](./assets/media/image40.png)

2.  Selezionare la Variante da utilizzare per generare il link di
    filtraggio automatico (tipicamente è la Variante sito attualmente
    online) e cliccare sul pulsante "**Accedi Sito**" in modo tale da
    caricare in locale, sul proprio browser, una versione "particolare"
    del front end del sito (per maggiori informazioni relativamente alla
    gestione delle Varianti Sito si veda il corrispondente capitolo di
    questo manuale), versione questa che andremo ad utilizzare per
    ottenere la querystring desiderata.

> **ATTENZIONE!** Non è strettamente necessario (anche se consigliato)
> utilizzare la Variante attualmente online per generare la querystring
> di filtraggio. L'importante è che il filtro applicato possa produrre
> effettivamente i risultati desiderati anche sulla Variante online.

3.  All'interno della Variante Sito appena caricata portarsi nella
    pagina utilizzata per gestire il componente "**Archivio News**",
    pagina questa in cui, oltre al suddetto componente, dovrà essere
    presente anche un pannello di ricerca utilizzato per filtrare le
    news presenti in archivio.

> **ATTENZIONE!** Al fine di poter generare correttamente la querystring
> di ricerca è necessario partire da un pagina in cui è presente un
> pannello di ricerca in grado di impostare il filtro desiderato. E'
> consigliabile, inoltre che nella stessa pagina sia presente anche il
> componente "Archivio News" in modo tale da poter verificare che il
> filtro impostato produca effettivamente i risultati desiderati

4.  Utilizzare il pannello di ricerca per impostare e applicare il
    filtro desiderato

![](./assets/media/image41.png)

> Nell'esempio in figura è stato impostato un filtro per ricercare tutte
> le news in archivio che contengono la parola "Apple"

5.  Una volta impostati i parametri di ricerca, portandosi con il mouse
    sul pulsante utilizzato per applicare il filtro, verrà visualizzata
    una piccola icona "**Copia**" grazie alla quale poter ottenere la
    querystring corrispondente al filtro appena impostato

![](./assets/media/image42.png)

6.  Cliccare quindi sull'icona "**Copia**" per copiare nella Clipboard
    (Appunti) la relativa querystring

![](./assets/media/image43.png)

> ed incollarla all'interno del parametro "**Ricerca Iniziale**"
> presente nella maschera di configurazione del pannello di ricerca

![](./assets/media/image45.png)

> **ATTENZIONE!** Una volta impostato il parametro "Ricerca Iniziale"
> come evidenziato in figura, ogni volta in cui un utente effettuerà
> l'accesso alla pagina contenente il pannello di ricerca in questione
> verrà automaticamente applicato il relativo filtro.

