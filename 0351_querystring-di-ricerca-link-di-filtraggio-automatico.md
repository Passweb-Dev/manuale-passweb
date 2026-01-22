# QUERYSTRING DI RICERCA -- LINK DI FILTRAGGIO AUTOMATICO



In determinate circostanze potrebbe essere particolarmente utile
disporre di appositi link mediante i quali applicare automaticamente
specifici filtri di ricerca agli articoli presenti in catalogo.

Supponiamo, ad esempio, di dover pubblicizzare una selezione di articoli
non raggruppabili all'interno di una determinata categoria merceologica
e quindi non raggiungibili mediante un url "standard" di pagina, e
supponiamo anche di non poter, o di non voler, risolvere questo tipo di
esigenza andando a creare apposite pagine del sito in cui inserire poi
singoli componenti di tipo "Risultati Ricerca" appositamente
prefiltrati.

In queste condizioni è comunque possibile soddisfare l' esigenza in
esame generando, dal Wizard di Passweb, la querystring corrispondente al
filtro desiderato e utilizzando poi questa stessa querystring per
comporre il link mediante il quale applicare automaticamente il
corrispondente filtro al Catalogo Ecommerce.

Di seguito viene descritta la procedura da seguire per ottenere
querystring e corrispondente link di filtraggio:

1.  Accedere al live editing del proprio sito e aprire la maschera di
    gestione delle Varianti

![Videate\\variante_4_res.bmp](./assets/media/image47.png){width="5.159722222222222in"
height="2.490972222222222in"}

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

3.  All'interno della Variante Sito appena caricata portarsi, ad
    esempio, nella pagina "Negozio" in cui dovranno essere presenti,
    ovviamente, il Catalogo Ecommerce e un pannello di ricerca articoli
    che andremo ad utilizzare per impostare il filtro richiesto

> **ATTENZIONE!** Al fine di poter generare correttamente la querystring
> di ricerca è necessario partire da un pagina in cui è presente un
> pannello di ricerca in grado di impostare il filtro desiderato. E'
> consigliabile, inoltre che nella stessa pagina sia presente anche il
> componente "Catalogo Ecommerce" o il componente "Risultati Ricerca" in
> modo tale da poter verificare che il filtro impostato produca
> effettivamente i risultati desiderati

4.  Utilizzare il pannello di ricerca per impostare e applicare al
    Catalogo Ecommerce il filtro desiderato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_3.bmp](./assets/media/image48.png){width="5.588888888888889in"
height="3.4972222222222222in"}

> Nell'esempio in figura è stato impostato un filtro per ricercare tutti
> gli articoli a catalogo con marca "Apple" e tipologia "Accessori"

5.  Una volta impostati i parametri di ricerca, portandosi con il mouse
    sul pulsante utilizzato per applicare il filtro, verrà visualizzata
    una piccola icona "**Copia**" grazie alla quale poter ottenere la
    querystring corrispondente al filtro appena impostato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_4.bmp](./assets/media/image49.png){width="5.079861111111111in"
height="3.4972222222222222in"}

6.  Cliccare quindi sull'icona "**Copia**" per copiare nella Clipboard
    (Appunti) la relativa querystring ed incollarla in un qualsiasi
    editor di testo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_5.bmp](./assets/media/image50.png){width="5.079861111111111in"
height="3.4972222222222222in"}

7.  A questo punto per ottenere il link di filtraggio automatico sarà
    sufficiente **unire il percorso della pagina del sito in cui è
    presente il "Catalogo Ecommerce"** (e che dovrà quindi mostrare i
    risultati del filtro impostato) **alla querystring generata al punto
    precedente separando i due elementi da un carattere ?** ottenendo
    così un url del tipo

> **https://www.urlsito.it/pagina_Catalogo?\<querystring_generata\>**
>
> [Esempio:]{.underline}
>
> <https://www.clobis.net/it/catalogo-articoli?pid=12942&fid=43881&fcv=codice%3D%26titolo%3D%26categoriastatistica%3D%26prezzo%3D%26prezzo-min%3D0%26prezzo-max%3D6100%2633%3DAPPLE%26subcategoriamerceologica%3D%26174%3DAccessori&csd=true&fct=codice%3Dtext%26titolo%3Dautocomplete%26categoriastatistica%3Dselect%26prezzo%3Dhidden%26prezzo-min%3Dtext%26prezzo-max%3Dtext%2633%3Dcheckboxlist%26subcategoriamerceologica%3Dhidden%26174%3Dhidden&typ=e>

8.  Da ultimo, è buona norma verificare che il link costruito al punto
    precedente sia corretto e che produca effettivamente i risultati
    sperati.

> Per far questo e sufficiente visitare questo stesso link inserendolo
> nella barra degli indirizzi del browser.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_6.bmp](./assets/media/image51.png){width="5.539583333333334in"
height="1.3069444444444445in"}

> **ATTENZIONE!** La pagina del sito utilizzata per costruire il link di
> filtraggio e a cui verrà quindi applicato il relativo filtro dovrà
> contenere, necessariamente, il componente "Catalogo Ecommerce" o il
> componente "Risultati Ricerca".
>
> Nel caso in cui nella pagina di destinazione del filtro non dovesse
> essere presente nessuno dei suddetti componenti il filtro non produrrà
> ovviamente nessun tipo di risultato.
>
> **Allo stesso modo occorre anche prestare particolare attenzione al
> fatto che la pagina di destinazione del link possa effettivamente
> mostrare i risultati desiderati**. Se il filtro fosse stato costruito
> operando sull'intero Catalogo e, successivamente venisse poi
> applicato, ad esempio, non alla pagina "Negozio" ma ad una specifica
> pagina di Categoria merceologica, i risultati mostrati potrebbero non
> essere quelli effettivamente desiderati.
>
> Si consiglia, infine, di inserire nella pagina di destinazione del
> filtro anche un pannello di ricerca contenente i campi utilizzati per
> costruire il filtro stesso, in maniera tale da consentire all'utente
> di poter, eventualmente, eliminare o modificare il filtro impostato
> automaticamente dal link.

