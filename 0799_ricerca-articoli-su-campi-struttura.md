# RICERCA ARTICOLI SU CAMPI STRUTTURA



Nel momento in cui l'esigenza dovesse essere quella di attivare
all'interno del proprio sito Ecommerce una ricerca articoli basata sulle
opzioni disponibili in corrispondenza dei diversi campi di una struttura
sarà necessario:

- Attivare, per prima cosa, la funzionalità di ricerca sull'intera
  struttura selezionando per questo il parametro "**Abilita Ricerca**"
  presente all'interno della maschera "**Modifica Struttura Articoli**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\struttura_abilita_ricerca.bmp](./assets/media/image396.png){width="5.616666666666666in"
height="3.4027777777777777in"}

> **ATTENZIONE!** l' effettiva selezione di questo parametro, e la
> conseguente attivazione della funzionalità di ricerca per la struttura
> in esame, dipende da quelle che sono le impostazioni settate per la
> struttura stessa e, conseguentemente, da quelle che saranno poi le
> diverse possibili combinazioni di articoli figlio da dover gestire
>
> Nel momento in cui si dovesse decidere di selezionare il parametro
> "**Abilita Ricerca**", al salvataggio della maschera verrà infatti
> avviato un controllo per determinare, in relazione a tutte le opzioni
> settate, se possa o meno essere effettivamente gestita la funzionalità
> di ricerca senza che questa vada a pregiudicare eccessivamente le
> prestazioni del sito.
>
> Se tale controllo dovesse dare esito negativo verrà visualizzato un'
> apposito messaggio di errore e, di fatto, la funzionalità di ricerca
> non potrà essere attivata

- Definire per quali campi della struttura dovrà essere attivata la
  funzionalità di ricerca e selezionare di conseguenza il parametro
  "**Abilita Ricerca**" presente, in corrispondenza del campo stesso,
  all'interno della maschera "**Modifica Campi Struttura**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_struttura_abilita_ricerca.bmp](./assets/media/image397.png){width="5.616666666666666in"
height="3.4027777777777777in"}

> **ATTENZIONE!** Dipendentemente dal numero dei campi della struttura
> abilitati per la ricerca e dalle impostazioni di configurazione e
> gestione della struttura stessa, le possibili opzioni visualizzate
> all'interno di un filtro potrebbero aumentare in maniera sensibile
> rallentando di conseguenza il caricamento della pagina web e
> aumentando il tempo di esecuzione della relativa query di ricerca.
>
> **In considerazione di ciò si consiglia sempre di valutare
> attentamente l'impatto che potrebbe avere sulle prestazioni del sito
> l'abilitazione di due o più campi di una struttura per la funzionalità
> di ricerca articoli**

- Inserire all'interno del pannello di ricerca un componente "**Filtro
  Indice**", "**Filtro Checkbox**" o "**Filtro Lista**" mappato sul
  Campo Articolo "**Strutture**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_strutture_filtro_indice.bmp](./assets/media/image398.png){width="4.947916666666667in"
height="3.0131944444444443in"}

> Per maggiori informazioni in merito all'inserimento di questi
> componenti all'interno di un pannello di ricerca e alla loro
> configurazione si veda anche quanto indicato al capitolo "*Varianti
> Sito Responsive -- Lista Componenti Ecommerce -- Componenti interni ai
> componenti Ecommerce -- Filtri di ricerca*" di questo manuale

In questo modo dunque, all'interno del pannello di ricerca verranno
visualizzate le diverse opzioni di filtro corrispondenti ai valori
assunti dagli articoli gestiti all'interno del sito, in relazione ai
campi della relativa struttura di appartenenza effettivamente abilitati
per la ricerca.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_campi_struttura.bmp](./assets/media/image399.png){width="5.454861111111111in"
height="3.4027777777777777in"}

In questo senso è bene sottolineare che nel momento in cui il filtro di
ricerca dovesse essere configurato impostando anche una specifica
struttura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_campi_struttura_2.bmp](./assets/media/image400.png){width="4.954861111111111in"
height="3.0in"}

le opzioni di selezione saranno ovviamente riferite sempre e solo ai
campi di quella stessa struttura abilitati per la funzione di ricerca,
**indipendentemente dalla pagina in cui è stato inserito il
corrispondente pannello di ricerca**

Se invece in fase di configurazione del filtro non dovesse essere
indicata nessuna struttura in particolare,

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_campi_struttura_3.bmp](./assets/media/image401.png){width="4.947916666666667in"
height="3.0131944444444443in"}

le opzioni di selezione visualizzate all'interno del pannello di ricerca
dipenderanno dalla specifica pagina in cui il pannello stesso è stato
inserito. In particolare:

- Se il pannello di ricerca dovesse essere inserito nella pagina
  "**Negozio**" le opzioni di selezione saranno relative ai campi,
  abilitati per la funzione di ricerca articoli, di una qualsiasi
  struttura a cui appartengono gli articoli presenti in catalogo

> E' semplice comprendere quindi come, in queste condizioni, le opzioni
> di selezione presenti all'interno del pannello di ricerca potrebbero
> anche essere particolarmente numerose, aumentando di conseguenza i
> tempi di caricamento della pagina e riducendo di fatto anche
> l'usabilità del corrispondente pannello di ricerca

- Se il pannello di ricerca dovesse invece essere inserito all'interno
  di una specifica pagina di categoria, le opzioni di selezione saranno
  relative ai campi, abilitati per la funzionalità di ricerca articoli,
  delle sole strutture cui appartengono gli articoli di quella specifica
  categoria

**ATTENZIONE! in considerazione di quanto detto, al fine di ottimizzare
le prestazioni del sito e l'usabilità stessa dei filtri, è sempre
consigliabile utilizzare questo tipo di ricerca non a livello generale
sull'intero catalogo ma solamente nelle specifiche pagine di categoria
in cui sono effettivamente presenti degli articoli strutturati**
(configurando quindi il filtro in maniera tale che lavori su di una
specifica struttura e non su tutte quelle che possono essere
effettivamente gestite all'interno sito)

In ogni caso per ciascun campo della struttura abilitato alla
funzionalità di ricerca verrà visualizzata, all'interno del relativo
pannello, una specifica sezione la cui intestazione coinciderà
esattamente con quanto inserito, per il campo stesso, in corrispondenza
del parametro "**Testo**" presente all'interno della maschera
"**Modifica Campi Struttura**" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_campi_struttura_4.bmp](./assets/media/image402.png){width="5.616666666666666in"
height="3.4027777777777777in"}

Ad ogni singola "sezione di ricerca" verrà inoltre associata anche una
specifica classe css (**optiongroup\_\<id campo\>**) utilizzabile nel
momento in cui l'esigenza dovesse essere quella di stilizzare in maniera
diversa le singole sezioni.

Per quel che riguarda invece il valore delle singole opzioni di
selezione questo coinciderà esattamente con quanto inserito per
l'opzione stessa in corrispondenza del campo "**Titolo**" presente
all'interno della maschera "**Modifica Elementi Campo Struttura**" del
Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_campi_struttura_5.bmp](./assets/media/image403.png){width="5.616666666666666in"
height="3.4027777777777777in"}

**ATTENZIONE!** solo per **Filtri Indice**, **Filtri Checkbox** e
**Filtri Lista**, nel momento in cui ad un' opzione dovesse essere
associato anche uno specifico colore, verrà visualizzato, all'interno
del pannello di ricerca, oltre al contenuto del campo "Titolo" anche il
relativo rettangolino colorato.

L'ordine in cui verranno visualizzate queste sezioni è stabilito dal
parametro "Campo di Ordinamento" presente nella maschera di
configurazione del relativo filtro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\filtro_strutture_ordinamento.bmp](./assets/media/image404.png){width="4.954861111111111in"
height="3.0in"}

In questo senso è possibile optare per due diverse tipologie di
ordinamento:

- **Descrizione**: selezionando questa opzioni i campi della struttura
  abilitati per la ricerca verranno ordinati in base alla loro
  descrizione e, quindi, in ordine alfabetico

- **Livello**: selezionando questa opzione i campi della struttura
  abilitati per la ricerca verranno ordinati in base al livello che il
  campo stesso assume all'interno della relativa struttura

Inoltre facendo riferimento ancora una volta alle possibili opzioni di
selezione visualizzate all'interno del pannello di ricerca è bene
sottolineare come queste possano variare non solo in relazione a quelli
che sono i campi di una struttura effettivamente abilitati per la
ricerca o alla pagina in cui il relativo filtro è stato inserito, ma
anche in relazione alla specifica modalità di gestione adotta per la
struttura in esame. In particolare:

- Nel caso in cui la struttura dovesse essere impostata su "**Esploso
  Completamente**" le opzioni di filtro presenti all'interno del
  pannello di ricerca saranno dettate da tutti i valori presenti nel
  corrispondente campo della cartella abbinamenti associata ai padri di
  struttura gestiti all'interno del sito

- Nel momento in cui la struttura dovesse invece essere gestita come
  "**Vincolata al precedente livello**", le opzioni di filtro presenti
  all'interno del pannello di ricerca saranno dettate unicamente dagli
  articoli figlio effettivamente esportati e gestiti all'interno del
  sito e da quelli che sono dunque i valori che questi stessi articoli
  andranno ad assumere per il relativo campo della struttura

Infine, in relazione alla possibilità di implementare all'interno del
proprio sito una ricerca articoli basata sui campi delle strutture è
sempre bene tenere in considerazione anche le seguenti osservazioni:

- Le diverse opzioni di selezione presenti all'interno di un pannello di
  ricerca saranno sempre "raggruppate per codice" (per maggiori
  informazioni in merito all'opportunità di raggruppare per codice le
  diverse opzioni del campo di una struttura si veda anche quanto
  indicato all'interno del precedente capitolo "*Modifica Elementi
  Struttura*")

- Come risultato di queste ricerche verranno ritornati i soli articoli
  padre di struttura presenti all'interno del sito i cui figli
  soddisfano il filtro di ricerca impostato

- **Il filtro per strutture potrebbe non aver senso se inserito
  all'interno di un pannello di ricerca impostato come "Vincolato al
  precedente livello".** In questo caso occorre ricordare infatti che il
  relativo filtro è gestito come un blocco unico e potrebbe avere al suo
  interno anche più sezioni distinte corrispondenti a diversi campi
  della struttura abilitati per la funzionalità di ricerca

- Nel momento in cui una determinata struttura dovesse essere gestita
  come "**Vincolata al precedente livello**" con "**Generazione degli
  elementi manuale**", nella barra degli strumenti della maschera
  "**Lista delle Strutture Articolo**" comparirà anche il pulsante
  "**Aggiorna Ricerca**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_strutture_aggiorna_ricerca.bmp](./assets/media/image394.png){width="5.785416666666666in"
height="3.49375in"}

> pulsante questo che dovrà essere utilizzato per aggiornare in maniera
> manuale la tabella di appoggio del database utilizzata per gestire il
> filtro strutture. Questo per evitare che a seguito di una qualsiasi
> modifica sugli elementi della struttura manuale (inserimenti,
> cancellazioni, modifiche ...) venga eseguita automaticamente, ogni
> volta, la procedura di aggiornamento della tabella di appoggio,
> procedura questa che potrebbe rivelarsi anche particolarmente onerosa.
>
> **In queste condizioni dunque sarà compito di chi opera sul Wizard
> lanciare manualmente la procedura di aggiornamento solo dopo aver
> effettuato tutte le modifiche necessarie ai vari elementi della
> struttura manuale.**
>
> **ATTENZIONE!** in caso di importazione degli elementi della struttura
> manuale tramite file, la procedura di aggiornamento verrà eseguita in
> maniera automatica al termine dell'importazione

