# IMPORTAZIONE COMPONENTI



I due pulsanti presenti nella parte alta della maschera di
configurazione di ogni componente consentono rispettivamente di:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_componenti_1_res.bmp](./assets/media/image95.png){width="5.141666666666667in"
height="3.089583333333333in"}

**I miei Componenti**: consente di importare all'interno della pagina
web Componenti precedentemente esportati da una qualsiasi Variante dello
stesso sito.

**ATTENZIONE!** Il pulsante "I miei Componenti" comparirà solo ed
esclusivamente nel caso in cui siano stati precedentemente esportati e
salvati all'interno della sezione "**Sito -- Componenti -- I miei
Componenti**" del Wizard, Componenti dello stesso tipo di quello in
esame.

Cliccando su questo pulsante verrà quindi visualizzata la maschera "**I
miei Componenti -- Tipo Componente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_componenti_2_res.bmp](./assets/media/image96.png){width="3.7909722222222224in"
height="2.6638888888888888in"}

maschera questa all'interno della quale poter visualizzare l'elenco di
tutti i componenti, della stessa tipologia di quello attualmente
considerato, e che sono stati precedentemente esportati a partire da una
qualsiasi Variante dello stesso Sito.

In questo senso è bene ricordare che la tipologia assegnata ad un
componente in fase di esportazione è di fondamentale importanza in
quanto definisce esattamente l'elemento dal quale dovremo poi partire
per poter importare e riutilizzare il componente appena esportato in una
qualsiasi altra pagina della stessa Variante e/o di Varianti differenti.

Supponendo quindi di assegnare, in fase di esportazione, al componente
in esame la tipologia "Contenitore", avremo poi la possibilità di
importare e riutilizzare questo stesso componente solo ed esclusivamente
a partire da un elemento della stessa tipologia.

Ciò significa dunque che, nel momento in cui dovessimo andare ad
inserire nella pagina un nuovo Componente di tipo Contenitore, cliccando
sul pulsante "**I miei componenti**" troveremo, nell'elenco dei
componenti importabili, anche quello appena esportato.

Al contrario, se dovessimo inserire nella pagina, ad esempio, un
Componente di tipo Paragrafo cliccando sul pulsante "I miei componenti"
troveremo questa volta, nell'elenco dei componenti importabili, solo ed
esclusivamente altri componenti di tipo Paragrafo, e tra questi non sarà
ovviamente presente il componente precedentemente esportato, essendogli
stata assegnata, in fase di esportazione, la tipologia di "Contenitore".

**ATTENZIONE!** Per maggiori informazioni relativamente alla procedura
di Esportazione Componenti si veda anche il corrispondente capitolo di
questo manuale (*"Live Editing per Varianti Responsive -- Componenti --
Azioni Componente -- Esporta Componente"*)

Per ogni componente presente in elenco è indicato il nome ad esso
assegnato in fase di esportazione e la relativa data di esportazione.

Il pulsante raffigurante un piccolo bidone (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\pulsante_bidone.bmp](./assets/media/image97.png){width="0.15694444444444444in"
height="0.18680555555555556in"} ), posto a fianco di ciascun componente
presente in elenco, consente di eliminare definitivamente dalla Galleria
il Componente stesso.

**ATTENZIONE!** L'eliminazione di un Componente dalla Galleria non ha
alcun effetto su eventuali componenti dello stesso tipo già importati ed
inseriti in altre pagine del sito

Il pulsante "**Importa Componente**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\pulsante_importa_componente.bmp](./assets/media/image98.png){width="0.8208333333333333in"
height="0.15694444444444444in"} ) consente invece di avviare la
procedura di importazione al termine della quale il componente in esame
verrà inserito nella pagina web potendo quindi essere tratto e gestito,
da questo momento in avanti, come un qualsiasi altro Componente Passweb.

In particolare poi, durante la procedura di importazione, Passweb andrà
ad analizzare il Componente in esame per verificare se per esso sono
stati utilizzati o meno, in fase di creazione, determinati Attributi
(colore o immagine).

Nel caso in cui, dunque, per la creazione del Componente in esame,
dovessero effettivamente essere stati utilizzati specifici Attributi e
nel caso in cui questi stessi attributi non dovessero essere già
presenti nel Tema in uso per la Variante di destinazione, verrà
visualizzata la maschera **"Gestione Temi -- Nuovi Attributi"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_componenti_3_res.bmp](./assets/media/image99.png){width="5.134027777777778in"
height="1.3729166666666666in"}

maschera questa all'interno della quale l'utente potrà decidere, prima
di terminare l'importazione e di inserire quindi il componente nella
pagina, come gestire questi stessi attributi e con cosa sostituirli.

Nello specifico dunque il campo:

- **Nome Attributo**: indica il nome dell'Attributo utilizzato in fase
  di creazione del componente che si sta importando.

- **Sostituisci con:** consente di definire lo specifico colore o la
  specifica immagine (dipendentemente dalla tipologia di attributo
  trattata) da utilizzare per sostituire l'attributo in esame.

> Il pulsante "**Seleziona Colore**" consente di selezionare il colore
> desiderato mediante l'apposito picker anziché digitare manualmente il
> codice colore nel relativo campo di input
>
> Allo stesso modo il pulsante "**Selezione risorsa**" consente di
> selezionare la risorsa desiderata tra quelle disponibili per il
> proprio sito anziché inserire manualmente il percorso di questa stessa
> risorsa nel relativo campo di input.
>
> In queste condizioni, una volta terminata la procedura di importazione
> verrà creato e inserito automaticamente tra gli Attributi in uso per
> il Tema in cui si desidera importare il Componente, un nuovo Attributo
> il cui nome sarà esattamente quello indicato all'interno del
> precedente campo "Nome Attributo" ed il cui valore sarà esattamente
> quello inserito all'interno del campo "Sostituisci con"

- **Sostituisci con attributo:** consente di sostituire l'attributo
  originale con uno di quelli attualmente in uso per il Tema in cui si
  desidera importare il Componente, selezionandolo per questo, dal
  relativo menu a tendina.

Il pulsante "**Aggiorna**" presente nella parte bassa della maschera,
consente di aggiornare i dati del componente con i nuovi valori passando
così alla gestione e alla sostituzione dell'eventuale successivo
Attributo.

**Galleria Componenti**: consente di importare all'interno della pagina
web Componenti completi, sia a livello grafico che di contenuti, messi a
disposizione direttamente da Passepartout e acquistabili all'interno del
sito [passstore.passepartout.net](https://passstore.passepartout.net/).

**ATTENZIONE!** Il pulsante "Galleria Componenti" comparirà solo ed
esclusivamente nel caso in cui nella Galleria dei Componenti messi a
disposizione da Passepartout siano presenti Componenti dello stesso tipo
di quello in esame

Cliccando su questo pulsante verrà quindi visualizzata la maschera
"**Galleria Componenti -- Tipo Componente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\importazione_componenti_4_res.bmp](./assets/media/image100.png){width="5.209027777777778in"
height="3.4923611111111112in"}

maschera questa all'interno della quale verrà visualizzata la Galleria
dei Componenti realizzati direttamente da Passepartout ed ovviamente
della stessa tipologia del Componente attualmente considerato.

Per ciascuno dei Componenti presenti in elenco è presente un'immagine
rappresentativa del Componente stesso, il suo Nome e una sua breve
descrizione.

Il pulsante "**Vai alla PassApp**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\pulsante_passApp.bmp](./assets/media/image101.png){width="1.0673611111111112in"
height="0.18680555555555556in"} ), presente in corrispondenza dei
componenti non ancora acquistati, consente di visualizzarne i dettagli
direttamente all'interno del sito
[passstore.passepartout.net](https://passstore.passepartout.net/) dove
si potrà poi, eventualmente, anche decidere di acquistarli.

Il pulsante "**Importa Componente**" (
![Videate\\pulsante_importa_componente.bmp](./assets/media/image102.png){width="0.8208333333333333in"
height="0.15694444444444444in"} ) presente invece in corrispondenza dei
componenti già acquistati e quindi a tutti gli effetti utilizzabili
all'interno del proprio sito, consente di avviare la procedura di
importazione, durante la quale verrà richiesto all'utente, esattamente
come nel caso precedente, come gestire eventuali Attributi utilizzati
per il componente in esame e non ancora presenti tra quelli attualmente
in uso nel Tema di destinazione.

**ATTENZIONE! Nel caso in cui lo stesso componente dovesse essere
importato ed utilizzato più volte all\'interno della stessa Variante è
sempre consigliabile gestire il codice CSS aggiuntivo a livello di
Layout e non di singolo Componente.**

In quest'ultimo caso infatti eventuali modifiche apportare alle regole
CSS presenti nella maschera di configurazione di uno qualsiasi dei
componenti importati potrebbero, da una parte ovviamente, andare ad
influire anche sugli altri componenti dello stesso tipo e, dall\'altra
parte, potrebbero portare a replicare più volte e inutilmente le stesse
regole CSS all\'interno del file components.css rendendo quindi la loro
gestione particolarmente complessa.

In queste condizioni, una volta importato il componente, si consiglia
quindi di trasferire eventuali regole CSS inizialmente impostate sul
componente stesso, a livello di Layout eliminandole dunque dal campo CSS
presente nella sua maschera di configurazione (sezione "Avanzate e
Animazioni), ed inserendole nella sezione CSS del Layout di Pagina o di
Variante.

