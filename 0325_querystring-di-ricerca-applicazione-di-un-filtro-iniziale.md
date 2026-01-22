# QUERYSTRING DI RICERCA -- APPLICAZIONE DI UN FILTRO INIZIALE



Nel caso in cui l'esigenza dovesse essere quella di applicare
automaticamente un filtro iniziale ai risultati di ricerca testuali del
sito, sarà necessario:

- Individuare la querystring corrispondente al filtro di ricerca
  desiderato

- Copiare la querystring di cui al punto precedente all'interno del
  parametro "**Ricerca Iniziale**" presente nella maschera di
  configurazione del relativo pannello di ricerca

Di seguito viene descritta la procedura da seguire per ottenere la
querystring da copiare poi all'interno del parametro "Ricerca Iniziale":

1.  Accedere al live editing del proprio sito e aprire la maschera di
    gestione delle Varianti

![Videate\\variante_4_res.bmp](./assets/media/image200.png){width="5.155555555555556in"
height="2.49375in"}

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

3.  All'interno della Variante Sito appena caricata portarsi nella
    pagina utilizzata per gestire il componente "**Risultati Ricerca sul
    sito**", pagina questa in cui, oltre al suddetto componente, dovrà
    essere presente anche un pannello di ricerca testuale.

> **ATTENZIONE!** Al fine di poter generare correttamente la querystring
> di ricerca è necessario partire da un pagina in cui è presente un
> pannello di ricerca in grado di impostare il filtro desiderato. E'
> consigliabile, inoltre che nella stessa pagina sia presente anche il
> componente "**Risultati Ricerca sul sito**" in modo tale da poter
> verificare che il filtro impostato produca effettivamente i risultati
> desiderati.

4.  Utilizzare il pannello di ricerca per impostare e applicare il
    filtro desiderato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_testuale_1.bmp](./assets/media/image201.png){width="6.00625in"
height="3.49375in"}

> Nell'esempio in figura è stato impostato un filtro di ricerca testuale
> sulla stringa "supporto"

5.  Una volta impostati i parametri di ricerca, portandosi con il mouse
    sul pulsante utilizzato per applicare il filtro, verrà visualizzata
    una piccola icona "**Copia**" grazie alla quale poter ottenere la
    querystring corrispondente al filtro appena impostato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_testuale_2.bmp](./assets/media/image202.png){width="6.00625in"
height="3.49375in"}

6.  Cliccare quindi sull'icona "**Copia**" per copiare nella Clipboard
    (Appunti) la relativa querystring

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_testuale_3.bmp](./assets/media/image203.png){width="6.00625in"
height="3.49375in"}

> ed incollarla all'interno del parametro "**Ricerca Iniziale**"
> presente nella maschera di configurazione del pannello di ricerca

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_testuale_iniziale_1.bmp](./assets/media/image205.png){width="5.110416666666667in"
height="3.071527777777778in"}

> **ATTENZIONE!** Una volta impostato il parametro "Ricerca Iniziale"
> come evidenziato in figura, ogni volta in cui un utente effettuerà
> l'accesso alla pagina contenente il pannello di ricerca in questione
> verrà automaticamente applicato il relativo filtro.

