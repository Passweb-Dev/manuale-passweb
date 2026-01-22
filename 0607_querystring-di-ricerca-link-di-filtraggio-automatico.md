# QUERYSTRING DI RICERCA -- LINK DI FILTRAGGIO AUTOMATICO



Come per gli articoli presenti all'interno del proprio catalogo
Ecommerce, anche per i post CMS in determinate circostanze potrebbe
essere particolarmente utile disporre di appositi link mediante i quali
poter applicare automaticamente specifici filtri di ricerca agli
elementi presenti in archivio.

Anche in questo caso è infatti possibile generare, dal Wizard di
Passweb, la querystring corrispondente al filtro desiderato e utilizzare
poi questa stessa querystring per comporre il link mediante il quale
applicare automaticamente il corrispondente filtro al componente
"Archivio News".

Di seguito viene descritta la procedura da seguire per ottenere
querystring e corrispondente link di filtraggio:

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
    (Appunti) la relativa querystring ed incollarla in un qualsiasi
    editor di testo

![](./assets/media/image43.png)

> A questo punto per ottenere il link di filtraggio automatico sarà
> sufficiente **unire il percorso della pagina del sito in cui è
> presente il componente "Archivio News"** (e che dovrà quindi mostrare
> i risultati del filtro impostato) **alla querystring generata al punto
> precedente separando i due elementi da un carattere ?** ottenendo così
> un url del tipo
>
> **https://www.urlsito.it/pagina_Archivio_News?\<querystring_generata\>**
>
> [Esempio:]{.underline}
>
> <https://www.clobis.net/it/blog/archivio-notizie?pid=12957&fid=44548&fcv=q%3Dapple&typ=c>

7.  Da ultimo, è buona norma verificare che il link costruito al punto
    precedente sia corretto e che produca effettivamente i risultati
    sperati.

> Per far questo e sufficiente visitare questo stesso link inserendolo
> nella barra degli indirizzi del browser.

![](./assets/media/image44.png)

> **ATTENZIONE!** La pagina del sito utilizzata per costruire il link di
> filtraggio e a cui verrà quindi applicato il relativo filtro dovrà
> contenere, necessariamente, il componente "Archivio News".
>
> Nel caso in cui nella pagina di destinazione del filtro non dovesse
> essere presente il suddetto componente il filtro non produrrà
> ovviamente nessun tipo di risultato.
>
> Allo stesso modo occorre anche prestare particolare attenzione al
> fatto che la pagina di destinazione del link possa effettivamente
> mostrare i risultati desiderati. Se il filtro fosse stato costruito
> operando sull'intero Archivio CMS e, successivamente venisse poi
> applicato, ad esempio, ad una pagina in cui è presente si un
> componente "Archivio News" ma prefiltrato solo su alcune categorie, i
> risultati mostrati potrebbero non essere quelli effettivamente
> desiderati.
>
> Si consiglia, infine, di inserire nella pagina di destinazione del
> filtro anche un pannello di Ricerca CMS in maniera tale da consentire
> all'utente di poter, eventualmente, eliminare o modificare il filtro
> impostato automaticamente dal link.

