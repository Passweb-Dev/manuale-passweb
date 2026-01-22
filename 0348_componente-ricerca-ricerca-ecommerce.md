# COMPONENTE RICERCA -- RICERCA ECOMMERCE



Il componente "**Ricerca sul sito**", se configurato correttamente,
consente di realizzare pannelli di ricerca Ecommerce mediante i quali
poter applicare determinati filtri agli articoli presenti in Catalogo

**ATTENZIONE!** Per poter funzionare correttamente un pannello di
Ricerca Ecommerce dovrà sempre lavorare in abbinamento con il componente
"**Catalogo E-Commerce**" oppure con il componente " **Risultati
Ricerca**". E' infatti all'interno di questi due componenti che verranno
mostrati i risultati del filtro di ricerca impostato.

Volendo, questi stessi pannelli di ricerca potranno essere utilizzati
anche per creare apposite querystring da utilizzare per:

- costruire link di filtraggio automatico

- applicare un filtro iniziale sui componenti "**Catalogo E-Commerce**"
  e/o " **Risultati Ricerca**"

Per maggiori informazioni in merito si vedano anche i successivi
capitoli "*Querystring di ricerca -- Link di filtraggio automatico*" e
"*Querystring di ricerca -- Applicazione di un filtro iniziale*" di
questo manuale.

In ogni caso per poter creare correttamente un pannello di Ricerca
Ecommerce la prima cosa da fare sarà quella di configurare il componente
"**Ricerca sul sito**", presente all'interno della sezione dei
Componenti Comuni, impostando il parametro "**Tipo**" sul valore
"**Ricerca E-Commerce**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_ecommerce0_res.bmp](./assets/media/image24.png)

**Come già evidenziato parlando del componente comune "Ricerca sul
sito", una volta imposta la tipologia del pannello di ricerca che si
intende realizzare questa non potrà più essere modificata.**

Ciò significa quindi che un componente ricerca configurato per
realizzare filtri sugli articoli presenti all'interno dei componenti
"Catalogo E-Commerce" e/o " Risultati Ricerca", non potrà mai essere
trasformato, ad esempio, in un pannello di ricerca in grado di filtrare
eventuali post presenti all'interno di un archivio CMS.

**In queste condizioni il Componente "Ricerca sul sito" potrà ovviamente
essere inserito all'interno di una qualsiasi pagina; al fine di potergli
consentire di espletare la funzione per cui è stato configurato, ossia
filtrare gli articoli presenti all'interno del Catalogo e/o all'interno
del componente Risultati Ricerca, dovrà però essere sempre utilizzato in
combinazione con uno di questi due componenti.**

Il risultato di un filtro applicato tramite questo Componente sarà
ovviamente quello di visualizzare all'interno del "Catalogo E-Commerce"
e/o del componente "Risultati Ricerca" i soli articoli che soddisfano la
condizione di filtro impostata.

