# FILTRO SET ATTRIBUTI



Il Componente "**Filtro Set Attributi**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_filtro_set_res.bmp](./assets/media/image637.png){width="2.5340277777777778in"
height="2.5458333333333334in"}

**può essere inserito unicamente all'interno del componente Ecommerce di
primo livello "Ricerca"**.

Grazie a questo componente ,in particolare, sarà possibile inserire
all'interno del pannello di ricerca, in un colpo solo, tutti gli
Attributi Articolo (siano essi di tipo Mexal, siano essi di tipo
Passweb) presenti all'interno di uno specifico Set ed impostati in
maniera tale da dover esser visualizzati all'interno di questo
componente (parametro "Visualizza nel componente Filtro Set Attributi"
del singolo attributo impostato a SI).

**ATTENZIONE! Nel caso di articoli associati a più categorie
merceologiche verrà considerato il set di attributi relativo alla
categoria merceologica principale, vale a dire quella associata
all'articolo stesso direttamente all'interno del relativo gestionale
Passepartout**

Per poter realizzare un filtro di ricerca sulla base di un certo
Attributo Articolo è quindi possibile procedere in due modi differenti:

1.  Inserire all'interno del pannello di ricerca uno dei componenti
    E-commerce precedentemente considerati (Filtro Testo, Filtro Lista o
    Filtro Indice) facendolo poi corrispondere all'Attributo Articolo
    desiderato.

2.  Codificare l'Attributo desiderato in maniera tale da poterlo
    visualizzare all'interno del componente "Filtro Set di Attributi"
    (parametro "Visualizza nel componente Filtro Set Attributi"
    dell'attributo stesso impostato a SI) ed inserire poi questo stesso
    componente all'interno del pannello di ricerca. Ovviamente in
    quest'ultimo caso il pannello di ricerca consentirà di realizzare
    filtri non solo sull'attributo desiderato ma su tutti quelli
    configurati per essere visualizzati all'interno di questo
    componente.

Relativamente al tipo di controllo di input, visualizzato all'interno di
questo componente in corrispondenza di ogni singolo attributo (semplice
campo di testo, drop down, filtro indice con o senza contatore di
elementi), tale controllo dipenderà da come è stato codificato
l'Attributo stesso.

E' infatti in fase di codifica dell'Attributo che, oltre a decidere se
visualizzarlo o meno all'interno del componente "Filtro Set di
Attributi", si dovrà decidere anche il tipo di controllo che dovrà
essere per esso utilizzato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_attributi_gestione_visualizzazione.bmp](./assets/media/image638.png){width="5.638194444444444in"
height="3.5458333333333334in"}

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> degli Attributi Articolo ed al processo di categorizzazione degli
> articoli gestiti all'interno del sito si rimanda alla relativa sezione
> di questo manuale (Catalogo -- Gestione Attributi Articoli).

Sulla base di quanto detto fino a questo momento dunque, a differenza
dei componenti precedentemente analizzati, il componente "Filtro Set
Attributi" in se non dovrà corrispondere a uno specifico campo del
gestionale o a uno specifico Attributo Articolo (saranno gli elementi al
suo interno a realizzare questa corrispondenza).

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata **la sua maschera di gestione e
configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_set_attributi_configurazione_res.bmp](./assets/media/image639.png){width="4.644444444444445in"
height="2.325in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di specificare il nome del Componente che si sta
realizzando

**Pubblico:** consente di impostare la visibilità lato sito web del
componente che si sta realizzando.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Contestuale alla pagina:** se impostato a SI all'interno del
componente verranno visualizzati gli attributi appartenenti al Set
assegnato alla categoria merceologica corrispondente alla pagina in cui
il componente stesso è stato inserito (e per i quali ovviamente il
parametro "Visualizza nel componente Filtro Set Attributi" è stato
impostato a SI).

> **NOTA BENE:** in queste condizioni ovviamente il componente dovrà
> essere inserito necessariamente in una Pagina Catalogo cui è stato
> assegnato uno specifico Set di Attributi. In caso contrario il
> componente risulterà vuoto.

Se impostato a NO sarà invece necessario indicare lo specifico Set di
Attributi che determinerà quali elementi visualizzare all'interno del
componente, selezionandolo per questo tra quelli precedentemente
codificati nella corrispondente sezione del Wizard e presenti
all'interno del campo **"Set di Attributi da visualizzare"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_filtro_set_attributi_configurazione2_res.bmp](./assets/media/image640.png){width="4.644444444444445in"
height="2.490972222222222in"}

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

