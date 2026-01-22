# QUERYSTRING DI RICERCA -- LINK DI FILTRAGGIO AUTOMATICO



Nel caso in cui l'esigenza dovesse essere quella di aver a disposizione
appositi link mediante i quali potersi collegare ad una pagina del sito
vedendosi applicare automaticamente un determinato filtro di ricerca
testuale, e visualizzando quindi i relativi risultati della ricerca,
sarà necessario:

- Individuare la querystring corrispondente al filtro di ricerca
  desiderato

- Costruire il link di filtraggio unendo il percorso della pagina del
  sito che contiene il componente "Risultati Ricerca sul sito" con la
  querystring individuata al punto precedente separando i due elementi
  con un carattere ?

Di seguito viene descritta la procedura da seguire per ottenere
querystring e corrispondente link di filtraggio:

1.  Accedere al live editing del proprio sito e aprire la maschera di
    gestione delle Varianti

![Videate\\variante_4_res.bmp](./assets/media/image200.png){width="5.155555555555556in"
height="2.49375in"}

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
    (Appunti) la relativa querystring ed incollarla in un qualsiasi
    editor di testo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_testuale_3.bmp](./assets/media/image203.png){width="6.00625in"
height="3.49375in"}

> A questo punto per ottenere il link di filtraggio automatico sarà
> sufficiente **unire il percorso della pagina del sito in cui è
> presente il componente "Risultati Ricerca sul sito"** (e che dovrà
> quindi mostrare i risultati del filtro impostato) **alla querystring
> generata al punto precedente separando i due elementi da un carattere
> ?** ottenendo così un url del tipo
>
> **https://www.urlsito.it/pagina_Risultati_Ricerca?\<querystring_generata\>**
>
> [Esempio:]{.underline}
>
> <https://www.clobis.net/it/risultati-ricerca?q=supporto>

7.  Da ultimo, è buona norma verificare che il link costruito al punto
    precedente sia corretto e che produca effettivamente i risultati
    sperati.

> Per far questo e sufficiente visitare questo stesso link inserendolo
> nella barra degli indirizzi del browser.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\querystring_ricerca_testuale_4.bmp](./assets/media/image204.png){width="6.013194444444444in"
height="1.4416666666666667in"}

> **ATTENZIONE!** La pagina del sito utilizzata per costruire il link di
> filtraggio e a cui verrà quindi applicato il relativo filtro dovrà
> contenere, necessariamente, il componente "Risultati Ricerca sul
> sito".
>
> Nel caso in cui nella pagina di destinazione del filtro non dovesse
> essere presente il suddetto componente il filtro non produrrà
> ovviamente nessun tipo di risultato.

