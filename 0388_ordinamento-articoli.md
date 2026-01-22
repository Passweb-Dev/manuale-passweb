# ORDINAMENTO ARTICOLI



Come evidenziato nel precedente capitolo il parametro "**Visualizza
Ordinamento**" presente nella maschera di configurazione del componente
"Wishlist Custom", consente se selezionato, di visualizzare, lato sito,
una combo box contenente l'elenco degli elementi sulla base dei quali
poter effettuare l'ordinamento degli articoli presenti all'interno del
componente (esattamente allo stesso modo di quanto già evidenziato per
il componente "Catalogo E-Commerce").

Anche in questo caso, come già per il Catalogo Ecommerce, la combo box
di selezione sarà preceduta da un testo indicativo, "Ordina per:",
modificabile nella sezione "Gestione Testi/Messaggi Sito" del Wizard.

**ATTENZIONE!** il valore selezionato inizialmente all'interno della
combo box sarà quello dell'elemento sulla base del quale è stato
impostato l'ordinamento di default.

Al cambio della selezione verrà ricaricato il componente (non l'intera
pagina) e il suo contenuto verrà ordinato in base al nuovo campo di
ordinamento.

**NOTA BENE:** nel caso in cui il componente sia paginato un'eventuale
variazione del campo di ordinamento riporterà il componente stesso sulla
prima pagina.

L'ordinamento inoltre, non verrà mantenuto in fase di navigazione del
sito. Questo significa dunque che, se dopo aver modificato l'ordinamento
del componente si dovesse continuare la navigazione del sito cambiando
pagina, al ritorno nella pagina che ospita il componente in oggetto, il
suo ordinamento sarà nuovamente quello di default.

Per impostare gli elementi sulla base dei quali poter effettuare
l'ordinamento degli articoli, è necessario agire dalla sezione
**"Gestione Campi di Ordinamento"**, presente anch'essa all'interno
della maschera di configurazione del componente

![](./assets/media/image193.png)

All'interno di questa sezione, sulla sinistra sono elencati gli elementi
di ordinamento attualmente codificati, sulla destra sono invece
riportate le proprietà dell'elemento attualmente selezionato in elenco.
Per modificare uno di questi elementi sarà quindi sufficiente
selezionarlo e agire poi sui parametri presenti all'interno della
sezione "**Modifica Campo Ordinamento**".

Allo stesso modo per codificare un nuovo elemento sarà necessario
cliccare sull'icona raffigurante un piccolo + (
![Videate\\icona_aggiungi.bmp](./assets/media/image163.png) ) e definire poi le proprietà
dell'elemento stesso.

In particolare per ogni singolo elemento di ordinamento occorrerà
specificare un valore per i seguenti campi:

**Testo:** etichetta identificativa dell'elemento di ordinamento che si
sta codificando. Tale etichetta comparirà poi, come possibile opzione di
selezione, all'interno della combo box visualizzata lato sito nel
momento in cui dovesse essere stato selezionato il parametro "Visualizza
Ordinamento".

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
  Wishlist verranno ordinati secondo il loro ordine di inserimento (non
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

**NOTA BENE:** è obbligatorio indicare un ordinamento di default. Nel
caso in cui questo non dovesse essere indicato al salvataggio del
componente verrà visualizzato un apposito messaggio di errore.

**ATTENZIONE!** nel caso in cui non dovesse essere impostato nessun
campo di ordinamento sul sito non verrà visualizzato il relativo
controllo (indipendentemente dal fatto di aver attivato o meno il
parametro "Visualizza Ordinamento") e gli articoli in Wishlist
continueranno ad essere ordinati secondo l'ordine di inserimento (con
eventuali articoli spesa posti in fondo alla lista)

Altra cosa importante da mettere in evidenza riguarda l'eventuale
presenza in Wishlist di articoli di tipo Campionario e/o di eventuali
articoli di tipo Spesa.

Nello specifico per quel che riguarda **gli articoli di tipo
"Campionario" questi verranno messi sempre come ultimi articoli,
indipendentemente dallo specifico ordinamento selezionato,** e comunque
sempre prima di eventuali articoli di tipo Spesa (cosa questa necessaria
per mantenere anche in fase di ordinamento la corretta gerarchia tra
articolo campionario e suoi componenti).

Per quel che riguarda invece **eventuali articoli di tipo Spesa questi
verranno sempre e comunque posizionati in fondo alla Wishlist** e
saranno ordinati tra loro in base al campo di ordinamento selezionato.

Infine va anche ricordato che i campi sulla base dei quali poter
stabilire l'ordine di visualizzazione degli articoli presenti
all'interno dei componenti saranno sempre considerati come testuali. In
conseguenza di ciò, un articolo con il campo di ordinamento impostato,
ad esempio sul valore 10, verrà visualizzato nel caso di ordinamento
Crescente (Decrescente) prima (dopo) di un articolo con il campo di
ordinamento impostato sul valore 2.

Il pulsante "**Aggiungi/Modifica** **Elemento**" presente nella parte
bassa della maschera consentirà di aggiungere in elenco l'elemento
appena codificato/modificato.

