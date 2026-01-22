# ORDINAMENTO ARTICOLI



Come evidenziato nel precedente capitolo il parametro "**Visualizza
Ordinamento**" presente nella maschera di configurazione del componente
"Risultati Ricerca", consente se selezionato, di visualizzare, lato
sito, una combo box contenente l'elenco degli elementi sulla base dei
quali poter effettuare l'ordinamento degli articoli presenti all'interno
del componente (esattamente allo stesso modo di quanto già evidenziato
per il componente "Catalogo E-Commerce").

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

![](./assets/media/image13.png)

Per maggiori informazioni relativamente a come poter impostare e gestire
i campi di ordinamento si veda anche quanto indicato all'interno del
capitolo "*Componenti Ecommerce -- Componente Catalogo Ecommerce --
Configurazione -- Ordinamento Articoli*" di questo manuale

**NOTA BENE:** è obbligatorio indicare un ordinamento di default. Nel
caso in cui questo non dovesse essere indicato al salvataggio del
componente verrà visualizzato un apposito messaggio di errore.

