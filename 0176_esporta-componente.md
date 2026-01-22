# ESPORTA COMPONENTE



L'icona "**Esporta Componente**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\icona_esporta_componente.bmp](./assets/media/image269.png) ) presente nel R.O.C. del componente
e/o nella barra degli strumenti dell' Albero dei Componenti consente di
esportare il componente in esame in maniera tale da poterlo poi
importare e riutilizzare in una qualsiasi altra pagina della stessa
Variante e/o di Varianti differenti (presenti comunque all'interno dello
stesso ambiente di sviluppo e quindi dello stesso sito)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esporta_componente.bmp](./assets/media/image270.png)

**ATTENZIONE!** I componenti esportati possono essere riutilizzati
**solo ed esclusivamente** **all'interno dello stesso ambiente di
sviluppo,** nella stessa Variante o in Varianti differenti.

Nel caso in cui l'esigenza dovesse essere quella di utilizzare un dato
componente presente nel Sito A all'interno del Sito B, sarà quindi
necessario:

- Importare nel sito B la Variante del Sito A che contiene il componente
  in esame

- Accedere nel sito B alla Variante importata al punto precedente

- Esportare il Componente desiderato

- Importare e riutilizzare il componente esportato al punto precedente
  in una qualsiasi altra pagina di una qualsiasi altra Variante del sito
  B

Cliccando su questo pulsante verrà visualizzata la maschera
"**Esportazione Componente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\maschera_esporta_componente.bmp](./assets/media/image271.png)

all'interno della quale poter assegnare un valore ai seguenti parametri:

- **Nome:** consente di assegnare un nome al componente che si sta
  esportando in maniera tale da poterlo poi identificare facilmente in
  fase di importazione, tra quelli presenti in elenco

- **Tipologia Componente:** consente di definire, selezionandola dal
  relativo menu a tendina, la tipologia da associare al componente che
  si sta esportando. In questo senso è possibile assegnare al componente
  in esame anche una tipologia diversa da quella propria del componente
  stesso.

**ATTENZIONE! La tipologia assegnata ad un componente in fase di
esportazione è di fondamentale importanza in quanto definisce
esattamente l'elemento dal quale dovremo poi partire per poter importare
e riutilizzare il componente appena esportato in una qualsiasi altra
pagina della stessa Variante e/o di Varianti differenti.**

Supponendo quindi di assegnare, in fase di esportazione, al componente
in esame la tipologia "Contenitore", avremo poi la possibilità di
importare e riutilizzare questo stesso componente solo ed esclusivamente
a partire da un elemento della stessa tipologia.

Ciò significa dunque che, nel momento in cui dovessimo andare ad
inserire nella pagina un nuovo Componente di tipo Contenitore, cliccando
sul pulsante "**I miei componenti**" troveremo, nell'elenco dei
componenti importabili, anche quello appena esportato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\import_componenti_pulsante.bmp](./assets/media/image272.png)

Al contrario, se dovessimo inserire nella pagina, ad esempio, un
Componente di tipo Paragrafo cliccando sul pulsante "I miei componenti"
troveremo questa volta, nell'elenco dei componenti importabili, solo ed
esclusivamente altri componenti di tipo Paragrafo, e tra questi non sarà
ovviamente presente il componente appena esportato, essendogli stata
assegnata, in fase di esportazione, la tipologia di "Contenitore".

Per maggior informazioni relativamente alla procedura di "Importazione
Componenti" si veda anche il corrispondente capitolo di questo manuale
("*Varianti Sito Responsive* *-- Configurazione Componenti
Caratteristiche generali -- Importazione Componenti"*)

**ATTENZIONE! In fase di esportazione di un componente verranno
considerate (e quindi salvate) sia le proprietà di configurazione che
eventuali regole CSS utilizzate per stilizzare il componente in esame ed
inserite all'interno del campo "CSS" presente nella maschera di
configurazione del componente stesso (sezione "Avanzate e Animazioni")**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\avanzate_animazioni_css.bmp](./assets/media/image273.png)

Per maggiori informazioni relativamente alla gestione del campo
evidenziato in figura si veda anche la corrispondente sezione di questo
manuale ("*Varianti Sito Responsive* *-- Configurazione Componenti
Caratteristiche generali -- Avanzate e Animazioni"*)

**ATTENZIONE! Non verranno invece considerate, in fase di esportazione,
eventuali regole CSS e/o funzioni javascript aggiunte per il componente
in esame a livello di layout.**

Cliccando sul pulsante "Esporta" presente nella maschera di
"Esportazione Componente" precedentemente analizzata, verrà avviata la
procedura di esportazione al termine della quale il componente in
oggetto potrà essere visualizzato e gestito anche all'interno della
sezione "**Sito -- Componenti -- I miei Componenti**" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_componenti_esportati.bmp](./assets/media/image274.png)

Per maggiori informazioni in merito a questa specifica sezione del
Wizard si veda anche il corrispondente capitolo di questo manuale
("*Sito -- Componenti*")

