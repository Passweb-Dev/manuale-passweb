# COMPONENTE RICERCA -- RICERCA TESTUALE



Come precedentemente evidenziato una delle possibilità offerte dal
componente "**Ricerca sul sito**" è quella di realizzare dei pannelli di
ricerca grazie ai quali poter effettuare delle ricerche sui principali
elementi di tipo testuale inseriti all'interno delle pagine del proprio
sito web.

**ATTENZIONE!** Per poter funzionare correttamente un pannello di
Ricerca Testuale dovrà sempre lavorare in abbinamento con il componente
"**Risultati Ricerca sul sito**". E' infatti all'interno di questo
componente che verranno mostrati i risultati del filtro di ricerca
impostato.

Volendo, questi stessi pannelli di ricerca testuale potranno essere
utilizzati anche per creare apposite querystring da utilizzare per:

- costruire link di filtraggio automatico sul componente "**Risultati
  Ricerca sul sito**"

- applicare automaticamente, al componente "**Risultati Ricerca sul
  sito**", un determinato filtro iniziale

Per maggiori informazioni in merito si vedano anche i successivi
capitoli "*Querystring di ricerca -- Link di filtraggio automatico*" e
"*Querystring di ricerca -- Applicazione di un filtro iniziale*" di
questo manuale.

In ogni caso per poter creare correttamente un pannello di Ricerca
Testuale la prima cosa da fare sarà quella di configurare il componente
"**Ricerca sul sito**", presente all'interno della sezione dei
Componenti Comuni, impostando il parametro "**Tipo**" sul valore
"**Ricerca Testuale**"

![](./assets/media/image199.png)

**Come già evidenziato all'interno del precedente capitolo di questo
manuale, una volta imposta la tipologia del pannello di ricerca che si
intende realizzare questa non potrà più essere modificata.**

Ciò significa quindi che un componente ricerca configurato per
realizzare ricerche di tipo testuale, non potrà mai essere trasformato,
ad esempio, in un pannello di ricerca in grado di filtrare eventuali
post presenti all'interno di un archivio CMS.

**In queste condizioni il Componente "Ricerca sul sito" potrà ovviamente
essere inserito all'interno di una qualsiasi pagina, ma, al fine di
potergli consentire di espletare correttamente la funzione per cui è
stato configurato, visualizzando quindi eventuali risultati di una
ricerca di tipo testuale, dovrà essere necessariamente utilizzato in
combinazione con il componente "Risultati Ricerca sul Sito" (anch'esso
presente nella sezione dei "Componenti Comuni").**

E' infatti all'interno di quest'ultimo componente che verranno
visualizzati tutti i risultati prodotti da ricerche effettuate
utilizzando il componente di "Ricerca sul sito" configurato nella
maniera indicata.

In questo senso poi il parametro "**Destinazione**" presente all'interno
della maschera "**Modifica Ricerca sul Sito**" precedentemente
esaminata, consente di impostare la specifica pagina di destinazione
all'interno della quale dovranno essere visualizzati i risultati della
ricerca effettuata. E' possibile decidere di rimanere all'interno della
stessa pagina (opzione **"Rimani su questa pagina"**) oppure selezionare
una pagina specifica dal sottostante albero delle pagine (opzione
**"Rimanda alla pagina"**), l'importante, comunque è collocare
all'interno della pagina scelta come destinazione per la visualizzazione
dei risultati il componente "**Risultati Ricerca sul Sito**"

> **NOTA BENE:** nel caso in cui non venga inserito, all'interno del
> pagina scelta come destinazione per la visualizzazione dei risultati
> della ricerca, il componente "Risultati Ricerca sul Sito" non sarà
> possibile in alcun modo visualizzare i risultati prodotti dalla
> ricerca in esame.

Per maggiori informazioni su come configurare il componente "**Risultati
Ricerca sul Sito**" e su come poter quindi visualizzare e gestire i
risultati prodotti da ricerche di tipo testuale si veda il
corrispondente capitolo di questo manuale *("Live Editing per Varianti
Responsive -- Lista Componenti Comuni -- Componente Risultati Ricerca
sul Sito"*).

**Utilizzando questo componente è possibile effettuare ricerche di più
keywords differenti, considerate in AND tra loro, semplicemente
indicando all'interno del pannello di ricerca le varie keywords separate
da uno spazio. All'interno dei risultati sarà poi possibile evidenziare
ogni singola occorrenza delle keywords indicate.**

**E' inoltre possibile ricercare anche intere frasi. In questo caso però
la frase da ricercare dovrà essere inserita all'interno del pannello di
ricerca racchiusa tra " " e per produrre dei risultati dovrà essere
presente all'interno del sito esattamente la stessa frase (spazi
compresi) indicata all'interno del pannello di ricerca**

