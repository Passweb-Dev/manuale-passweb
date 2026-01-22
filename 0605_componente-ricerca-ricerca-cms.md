# COMPONENTE RICERCA -- RICERCA CMS



Il componente "**Ricerca sul sito**", se configurato correttamente,
consente di realizzare pannelli di ricerca mediante i quali poter
applicare determinati filtri ai post CMS presenti all'interno di un
"Archivio News"

**ATTENZIONE!** Per poter funzionare correttamente un pannello di
Ricerca CMS dovrà sempre lavorare in abbinamento con il componente
"**Archivio News**". E' infatti all'interno di questo componente che
verranno mostrati i risultati del filtro di ricerca impostato.

Volendo, questi stessi pannelli di ricerca potranno essere utilizzati
anche per creare apposite querystring da utilizzare per:

- costruire link di filtraggio automatico sul componente "**Archivio
  News**"

- applicare automaticamente, al componente "**Archivio News**", un
  determinato filtro iniziale

Per maggiori informazioni in merito si vedano anche i successivi
capitoli "*Querystring di ricerca -- Link di filtraggio automatico*" e
"*Querystring di ricerca -- Applicazione di un filtro iniziale*" di
questo manuale.

In ogni caso per poter creare correttamente un pannello di Ricerca CMS
la prima cosa da fare sarà quella di configurare il componente
"**Ricerca sul sito**", presente all'interno della sezione dei
Componenti Comuni, impostando il parametro "**Tipo**" sul valore
"**Ricerca sul CMS**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_cms0_res.bmp](./assets/media/image37.png)

**In queste condizioni il Componente "Ricerca" potrà ovviamente essere
inserito all'interno di una qualsiasi pagina del sito; al fine di
potergli consentire di espletare la funzione per cui è stato configurato
dovrà però essere sempre utilizzato in combinazione con un componente
CMS "Archivio News" oppure con un componente "Risultati Ricerca sul
sito" con abilitata la ricerca sui contenuti CMS**

> **NOTA BENE:** affinché la ricerca impostata possa produrre
> correttamente i risultati sperati, è necessario che per il
> corrispondente componente "Archivio News" sia stato selezionato il
> parametro "Abilita Filtro FullText".

