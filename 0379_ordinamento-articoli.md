# ORDINAMENTO ARTICOLI



Come evidenziato nel precedente capitolo la sezione "**Gestione Campi di
Ordinamento**" consente di stabilire la modalità secondo cui dovranno
essere ordinati gli articoli presenti in carrello

![Videate\\ordinamento_carrello.bmp](./assets/media/image162.png)

All'interno di questa sezione, sulla sinistra sono elencati gli elementi
di ordinamento attualmente codificati, sulla destra sono invece
riportate le proprietà dell'elemento attualmente selezionato in elenco.
Per modificare uno di questi elementi sarà quindi sufficiente
selezionarlo e agire poi sui parametri presenti all'interno della
sezione "**Modifica Campo Ordinamento**".

**ATTENZIONE!** a differenza di altri componenti (es. "Catalogo
Ecommerce") non è possibile variare a front end l'ordinamento stabilito,
in fase di configurazione del componente, per gli articoli in carrello.

**In conseguenza di ciò sarà ovviamente sufficiente codificare
all'interno della sezione sopra evidenziata un solo elemento di
ordinamento che sarà poi quello effettivamente applicato a front end.**

Per codificare un nuovo elemento sarà necessario cliccare sull'icona
raffigurante un piccolo + (
![Videate\\icona_aggiungi.bmp](./assets/media/image163.png) ) e definire poi le proprietà
dell'elemento stesso.

In particolare occorrerà specificare un valore per i seguenti campi:

**Testo:** etichetta identificativa dell'elemento di ordinamento che si
sta codificando.

**Tipo di ordinamento:** consente di specificare il campo sulla base del
quale dovranno essere ordinati gli articoli presenti all'interno del
componente nel momento in cui, lato sito, dovesse essere selezionato
l'elemento di ordinamento che si sta codificando.

E' possibile indicare una delle seguenti opzioni:

- **Campo Articolo:** selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Campo di
  Ordinamento**") lo specifico campo del gestionale che dovrà essere
  utilizzato per definire l'ordinamento degli articoli.

> Per maggiori informazioni relativamente ai diversi campi articolo su
> cui poter impostare l'ordinamento si veda anche quanto indicato, a
> proposito dello stesso parametro, per il componente "Catalogo
> Ecommerce" (*Componenti Ecommerce -- Componente Catalogo Ecommerce --
> Configurazione -- Ordinamento Articoli)*

- **Attributo Articolo**: selezionando questo valore sarà poi possibile
  specificare dal sottostante menu a tendina ("**Attributo di
  Ordinamento**") l'Attributo Articolo (sia esso di tipo Passweb, sia
  esso di tipo Mexal) che dovrà essere utilizzato per definire
  l'ordinamento degli articoli.

> E' possibile selezionare uno qualsiasi degli Attributi Articolo
> precedentemente codificati all'interno della corrispondente sezione
> del Wizard.

- **Creazione**: selezionando questo valore gli articoli presenti in
  Carrello verranno ordinati secondo il loro ordine di inserimento (non
  sarà quindi necessario specificare né un campo articolo né tanto meno
  un attributo) in maniera Crescente o Decrescente a seconda delle
  impostazioni settate per il successivo parametro "**Modo di
  Ordinamento**"

**Modo di Ordinamento:** consente di specificare se, in relazione
all'elemento che si sta codificando, dovrà essere applicato un
ordinamento di tipo Crescente o Decrescente. Tale campo non sarà
ovviamente presente nel caso in cui sia stato impostato un ordinamento
di tipo Casuale.

**Default:** se selezionato, il corrispondente elemento verrà
considerato come elemento sulla base del quale ordinare a default gli
articoli presenti all'interno del componente.

**ATTENZIONE!** Nel caso in cui non dovesse essere specificato nessun
ordinamento, gli articoli presenti in carrello verranno posizionati in
ordine di inserimento crescente con eventuali articoli di tipo spesa
sempre alla fine.

Si ricorda inoltre che, indipendentemente dall'ordinamento impostato per
il carrello, in checkout gli articoli verranno ordinati sempre e
comunque in base al loro ordine di inserimento.

Altra cosa importante da mettere in evidenza riguarda l'eventuale
presenza in Carrello di articoli di tipo Campionario e/o di eventuali
articoli di tipo Spesa.

Nello specifico per quel che riguarda **gli articoli di tipo
"Campionario" questi verranno messi sempre come ultimi articoli,
indipendentemente dallo specifico ordinamento impostato,** e comunque
sempre prima di eventuali articoli di tipo Spesa (cosa questa necessaria
per mantenere anche in fase di ordinamento la corretta gerarchia tra
articolo campionario e suoi componenti).

Per quel che riguarda invece **eventuali articoli di tipo Spesa questi
verranno sempre e comunque posizionati in fondo al Carrello** e saranno
ordinati tra loro in base al campo di ordinamento impostato.

Infine va anche ricordato che i campi sulla base dei quali poter
stabilire l'ordine di visualizzazione degli articoli presenti
all'interno del componente saranno sempre considerati come testuali. In
conseguenza di ciò, un articolo con il campo di ordinamento impostato,
ad esempio sul valore 10, verrà visualizzato nel caso di ordinamento
Crescente (Decrescente) prima (dopo) di un articolo con il campo di
ordinamento impostato sul valore 2.

