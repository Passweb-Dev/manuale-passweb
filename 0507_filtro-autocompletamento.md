# FILTRO AUTOCOMPLETAMENTO



Il Componente "**Filtro Autocompletamento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_filtro_autocompletamento_res.bmp](./assets/media/image630.png){width="2.5340277777777778in"
height="2.5458333333333334in"}

**può essere inserito unicamente all'interno del componente Ecommerce di
primo livello "Ricerca".**

Grazie a questo componente sarà possibile visualizzare all'interno del
pannello di ricerca una lista di possibili opzioni da selezionare che
varieranno in base al testo digitato dall'utente, oltre che ovviamente
sulla base dello specifico campo/attributo con il quale è stato mappato
il componente in esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_autocompletamento.bmp](./assets/media/image631.png){width="5.545833333333333in"
height="3.2576388888888888in"}

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata **la sua maschera di gestione e
configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_autocompletamento_configurazione_res.bmp](./assets/media/image632.png){width="5.159722222222222in"
height="3.097916666666667in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di definire un nome per il Componente che si sta
editando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Label:** consente di impostare la label da associare al campo di input
che si sta realizzando

**Segnaposto:** permette di definire un testo che verrà poi utilizzato
**come segnaposto** e quindi visualizzato all'interno del campo di input
utilizzato dagli utenti del sito per ricercare i vari articoli.

**ATTENZIONE!** Al click dell'utente sul campo in esame il testo
indicato scomparirà consentendo quindi all'utente di inserire il valore
desiderato. Quanto indicato all'interno di questo campo non verrà quindi
considerato alla conferma del form.

**Valore di default:** consente di indicare un testo che verrà
utilizzato (e visualizzato) **come valore di default** per il campo in
esame.

**ATTENZIONE!** A differenza di quanto indicato per il precedente
parametro "Segnaposto", il testo inserito all'interno del campo "Valore
di default" **non scomparirà** in automatico al click dell'utente sul
campo di input ma, al contrario, verrà considerato come se fosse un vero
e proprio valore indicato dall\'utente stesso in fase di compilazione.

Per poter visualizzare l'elenco delle possibili opzioni di scelta è
quindi indispensabile apportare una qualche variazione ad eventuali
"Valori di Default" gestiti per il componente in esame.

**Numero minimo di caratteri da digitare:** consente di specificare,
selezionandolo da un apposito menu a tendina, l'esatto numero di
caratteri che dovranno necessariamente essere digitati dall'utente prima
di poter visualizzare l'elenco delle possibili opzioni di scelta.

**Numero massimo di opzioni da mostrare:** consente di specificare il
numero massimo di opzioni che dovranno essere visualizzate all'interno
dell'elenco dei risultati del relativo campo di autocompletamento

**ATTENZIONE!** Nel caso in cui i possibili risultati di un
autocompletamento dovessero essere particolarmente numerosi, per non
impattare eccessivamente nelle prestazioni del sito (oltre che
ovviamente per rendere i risultati stessi effettivamente utilizzabili)
si consiglia di aumentare il "Numero mimino di caratteri da digitare"
prima di mostrare i risultati dell'autocompletamento oppure di impostare
un adeguato "Numero massimo di opzioni da mostrare"

La sotto sezione "**Informazioni sul filtro**" consente di impostare il
campo Mexal o l'Attributo Passweb su cui dovrà essere realizzato il
filtro di ricerca che si intende implementare (per maggiori informazioni
in merito si veda anche il precedente capitolo "*Componenti Ecommerce --
Filtri di ricerca*" di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_autocompletamento_configurazione_res_2.bmp](./assets/media/image633.png){width="4.65in"
height="2.9506944444444443in"}

Dipendentemente poi dai valori selezionati per i campi "**Tipologia di
Filtro**" e "**Campo su cui far Filtro**" potranno comparire all'interno
di questa sezione ulteriori parametri di configurazione in grado di
modificare anche il comportamento del componente.

In particolare, nel momento in cui il parametro **"Campo su cui far
Filtro"** dovesse essere impostato su una delle seguenti opzioni:

- Codice Articolo

- Codice Articolo + Codici Alias Articolo

- Codice Articolo + Descrizione Articolo

- Codice Articolo + Titolo Articolo

- Codice Articolo + Titolo Articolo + Descrizione Articolo

compariranno, all'interno di questa sezione, due ulteriori campi
"**Abilita Link sul testo**" e "**Template**" che consentono
rispettivamente di:

- **Abilita Link sul testo:** consente, se selezionato, di attivare sui
  risultati mostrati all'interno del filtro di autocompletamento il link
  diretto alla relativa pagina prodotto.

> In queste condizioni dunque cliccando su uno dei risultati proposti
> non verrà applicato il filtro ma si verrà rediretti direttamente alla
> pagina prodotto del relativo articolo.
>
> Nel momento in cui l'opzione proposta all'interno del filtro di
> autocompletamento dovesse invece essere selezionata mediante il tasto
> "Invio" questa verrà inserita all'interno del campo di ricerca e il
> pannello manterrà il suo comportamento standard applicando quindi il
> relativo filtro articoli.

- **Template**: consente di definire il template da utilizzare per la
  visualizzazione dei risultati mostrati all'interno del filtro di
  autocompletamento (per maggiori informazioni in merito si veda anche
  il successivo capitolo di questo manuale)

**ATTENZIONE!** i parametri "**Abilita Link sul testo**" e
"**Template**" verranno attivati solo ed esclusivamente nel momento in
cui il parametro "**Campo su cui far Filtro**" soddisfi le condizioni
sopra indicate

Nel momento in cui il parametro "**Campo su cui far filtro**" dovesse
essere invece impostato sull'opzione:

- FullText

oltre ai due parametri appena analizzati comparirà anche il campo
"**Metodo di Ordinamento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_autocompletamento_fulltext.bmp](./assets/media/image634.png){width="3.9756944444444446in"
height="3.0555555555555554in"}

- **Metodo di Ordinamento**: consente di impostare l'ordinamento che
  verrà poi applicato ai risultati della ricerca. E' possibile
  selezionare una delle seguenti opzioni:

  - **Codice:** selezionando questa opzione i risultati della ricerca
    verranno ordinati per codice articolo

  - **Inizia con:** selezionando questa opzione i risultati della
    ricerca verranno ordinati inserendo prima gli articoli per i quali
    il campo FullText inizia esattamente con la stringa di ricerca
    indicata e, successivamente, quelli per i quali il campo FullText
    contiene la stringa di ricerca indicata.

> In conseguenza di ciò, nel momento in cui l'esigenza dovesse essere,
> ad esempio, quella di visualizzare prima gli articoli il cui Titolo
> inizia esattamente con la stringa di ricerca indicata sarà quindi
> necessario accertarsi di aver inserito il campo "Titolo" come primo
> campo tra quelli abilitati per la ricerca FullText
>
> **ATTENZIONE!** l'opzione di ordinamento "Inizia Con" richiede, per
> poter funzionare in maniera corretta, che il parametro "**Ricerca sul
> campo FullText**" presente alla pagina "**Configurazione Catalogo**"
> del Wizard sia impostato sull'opzione "FullText"

Un'ultima cosa di fondamentale importanza da tenere in considerazione è
che nel momento in cui il filtro autocompletamento dovesse essere
impostato su uno dei campi articolo sopra indicati, ai risultati
restituiti verranno applicate anche:

- le classi CSS che identificano le diverse tipologie di articoli (es.
  structureproduct, structurefather, boxproduct ecc...)

- le classi CSS che consentono di identificare se un determinato
  prodotto è già stato inserito o meno in carrello / wishlist (incart /
  inwishlist)

- le classi CSS gestite mediante il parametro "Classi Custom" presente
  nell'anagrafica Passweb del relativo articolo

- le classi CSS gestite mediante il parametro "Classi Regole" presente
  nell'anagrafica Passweb del relativo articolo

**ATTENZIONE!** anche le classi CSS sopra indicate (così come i
parametri "Abilita link sul testo" e "Template") verranno applicate ai
risultati restituiti dal filtro di autocompletamento solo ed
esclusivamente nel caso in cui il parametro "Campo su cui far filtro"
sia stato impostato su uno dei valori precedentemente indicati.

Per poter applicare tali classi nella maniera corretta è infatti
indispensabile che ci sia una corrispondenza univoca tra l'opzione
mostrata nei risultati del filtro di autocompletamento e il
corrispondente articolo.

Nel momento in cui dovesse infatti essere utilizzato come campo di
filtro, ad esempio, un attributo "Colore" i risultati mostrati
dall'autocompletamento, che potrebbero essere "Giallo", "Rosso", "Verde"
... non identificherebbero in maniera univoca un determinato articolo ma
potrebbero anche essere riferirti ad una serie di prodotti ed in questo
caso non sarebbe ovviamente possibile assegnare al risultato una
determinata classe CSS che ne identifichi, ad esempio, la tipologia.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

##### DEFINIZIONE DEL TEMPLATE PER I RISULTATI DEL FILTRO DI AUTOCOMPLETAMENTO

Come evidenziato nel precedente capitolo di questo manuale nel momento
in cui la configurazione del componente "Filtro Autocompletamento"
dovesse soddisfare determinate condizioni, sarà possibile definire e
personalizzare sia graficamente che a livello di contenuti il formato
dei risultati mostrati all'interno di questo stesso filtro.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\autocompletamento_template_1.bmp](./assets/media/image635.png){width="5.625694444444444in"
height="3.2944444444444443in"}

In questo senso infatti, il campo "**Template**" presente nella maschera
di configurazione del componente stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\autocompletamento_template_2.bmp](./assets/media/image636.png){width="4.65in"
height="2.9569444444444444in"}

consente di intervenire direttamente a livello di codice HTML
specificando dunque il markup e le relative informazioni che dovranno
essere visualizzate per ciascun risultato ottenuto mediate il filtro di
autocompletamento

Volendo è possibile aprire l'editor in modalità Full Screen utilizzando
per questo il tasto funzione **F11**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\autocompletamento_carrello_configurazione5.bmp](./assets/media/image501.png){width="5.625694444444444in"
height="3.2944444444444443in"}

Una volta entrati in modalità full screen è poi possibile ritornare alla
visualizzazione standard utilizzando il tasto **ESC**.

Il pulsante "**Preview**" presente nella parte alta della maschera
consente invece di visualizzare un'anteprima del Template che si sta
realizzando, dove, ovviamente, al posto dei dati reali relativi ad
articoli, verranno visualizzati appositi segnaposto.

In modalità Preview è possibile selezionare uno qualsiasi degli elementi
presenti all'interno del Template.

Cliccandoci sopra si passerà automaticamente alla versione
"**Sorgente**" del template con evidenziata la riga di codice relativa
all'elemento selezionato

La possibilità di intervenire direttamente sul codice HTML del template
offre, indubbiamente, ampie possibilità di personalizzazione, sia
grafiche che a livello di veri e propri contenuti.

**D'altra parte dovendo intervenire direttamente a livello di codice
questo tipo di personalizzazione richiede chiaramente specifiche
conoscenze tecniche.**

Relativamente alle informazioni visualizzabili per ogni singolo articolo
presente tra i risultati di ricerca Passweb mette a disposizione
dell'utente la possibilità di utilizzare appositi segnaposto.

In questo senso una volta posizionato il cursore nel punto del template
in cui dovrà essere inserita la nuova informazione, sarà necessario
cliccare sul pulsante "**Seleziona un segnaposto ...**" in maniera tale
da visualizzare l'elenco di tutti i segnaposto disponibili

Selezionando quindi il segnaposto desiderato Passweb provvederà ad
inserire automaticamente nel template il codice necessario per gestire
quello specifico tipo di informazione.

E' possibile selezionare uno dei seguenti segnaposto:

- **Immagine**: verrà sostituito in fase di generazione del template con
  l'immagine catalogo del relativo articolo

- **Titolo**: verrà sostituita in fase di generazione del template con
  il titolo del relativo articolo

- **Codice**: verrà sostituito in fase di generazione del template con
  il codice del articolo

- **Codice Alternativo**: verrà sostituito in fase di generazione del
  template con il codice alternativo del relativo articolo (solo siti
  collegati a Mexal)

- **Campo**: verrà sostituito in fase di generazione del template con il
  valore del campo indicato in corrispondenza del parametro "Campo su
  cui far Filtro"

