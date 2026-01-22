# QUERYSTRING DI RICERCA -- APPLICAZIONE DI UN FILTRO INIZIALE



Come evidenziato nei precedenti capitoli di questo manuale, volendo, è
possibile configurare un pannello di ricerca ecommerce in maniera tale
che ogni volta in cui l'utente effettuerà l'accesso alla pagina
contenente tale pannello, venga automaticamente applicato uno specifico
filtro articoli.

Per fare questo è necessario determinare la querystring corrispondente
al filtro iniziale che si desidera applicare e copiarla all'interno del
parametro "**Ricerca Iniziale**" presente nella maschera di
configurazione del componente di ricerca

Di seguito viene descritta la procedura da seguire per ottenere il
valore che dovrà poi essere inserito in corrispondenza del parametro
"Ricerca Iniziale":

1.  Accedere al live editing del proprio sito e aprire la maschera di
    gestione delle Varianti

![Videate\\variante_4_res.bmp](./assets/media/image47.png)

2.  Selezionare la Variante che dovrà essere utilizzata per determinare
    il filtro iniziale da applicare al pannello di ricerca (tipicamente
    è la Variante sito attualmente online) e cliccare sul pulsante
    "**Accedi Sito**" in modo tale da caricare in locale, sul proprio
    browser, una versione "particolare" del front end del sito (per
    maggiori informazioni relativamente alla gestione delle Varianti
    Sito si veda il corrispondente capitolo di questo manuale), versione
    questa che andremo ad utilizzare per ottenere la querystring
    desiderata.

> **ATTENZIONE!** Non è strettamente necessario (anche se consigliato)
> utilizzare la Variante attualmente online per generare la querystring
> di filtraggio. L'importante è che il filtro applicato possa produrre
> effettivamente i risultati desiderati anche sulla Variante online.

3.  All'interno della Variante Sito appena caricata portarsi, ad
    esempio, nella pagina "Negozio" in cui dovranno essere presenti,
    ovviamente, il Catalogo Ecommerce e il pannello di ricerca articoli
    al quale dovrà poi essere applicato il filtro iniziale.

> **ATTENZIONE!** Al fine di poter generare correttamente la querystring
> relativa al filtro iniziale è necessario partire da un pagina in cui è
> presente un pannello di ricerca in grado di impostare il filtro
> desiderato. E' consigliabile, inoltre che nella stessa pagina sia
> presente anche il componente "Catalogo Ecommerce" o il componente
> "Risultati Ricerca" in modo tale da poter verificare che il filtro
> impostato produca effettivamente i risultati desiderati

4.  Utilizzare il pannello di ricerca per impostare e applicare al
    Catalogo Ecommerce il filtro desiderato

![](./assets/media/image52.png)

> Nell'esempio in figura è stato impostato un filtro per ricercare i
> soli articoli effettivamente disponibili

5.  Una volta impostati i parametri di ricerca, portandosi con il mouse
    sul pulsante utilizzato per applicare il filtro, verrà visualizzata
    una piccola icona "**Copia**" grazie alla quale poter ottenere la
    querystring corrispondente al filtro appena impostato

![](./assets/media/image53.png)

6.  Cliccare quindi sull'icona "**Copia**" per copiare nella Clipboard
    (Appunti) la relativa querystring

![](./assets/media/image54.png)

> ed incollarla all'interno del parametro "**Ricerca Iniziale**"
> presente nella maschera di configurazione del pannello di ricerca

![](./assets/media/image55.png)

> **ATTENZIONE!** Una volta impostato il parametro "Ricerca Iniziale"
> come evidenziato in figura, ogni volta in cui un utente effettuerà
> l'accesso alla pagina contenente il pannello di ricerca in questione
> verrà automaticamente applicato il relativo filtro articoli.

