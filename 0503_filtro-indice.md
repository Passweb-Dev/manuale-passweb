# FILTRO INDICE



Il Componente **"Filtro Indice"**

![](./assets/media/image616.png)

**può essere inserito unicamente all'interno del componente Ecommerce di
primo livello "Ricerca"**.

Grazie a questo componente sarà possibile visualizzare all'interno del
pannello di ricerca un elenco di tutti i possibili valori assunti (per
gli articoli gestiti all'interno del sito) dall'Attributo Articolo o dal
campo Mexal che verrà fatto corrispondere al componente in esame (tali
valori potranno quindi essere eventualmente anche delle immagini).

Ogni singola voce di questo elenco, se cliccata, consentirà di filtrare
gli articoli in catalogo per l'attributo in esame e sulla base del
valore appena selezionato. A fianco di ogni singola voce potrà inoltre
comparire o meno (a seconda delle impostazioni del componente stesso)
l'esatto numero degli articoli in catalogo per i quali l'attributo in
esame assume quello specifico valore.

Rilasciando il Componente nella posizione desiderata all'interno della
pagina web, verrà visualizzata **la sua maschera di gestione e
configurazione**

![](./assets/media/image617.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di specificare il nome del Componente che si sta
realizzando

**Pubblico**: consente di impostare la visibilità lato sito web del
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

**Label**: consente di specificare un'etichetta identificativa del
componente che si sta realizzando. Tale etichetta verrà poi visualizzata
all'interno del pannello di ricerca in corrispondenza dei valori assunti
dal componente in oggetto

**Struttura**: visualizzato solo per filtri sul Campo Articolo
"**Strutture**".

Permette di selezionare l'eventuale struttura in relazione alla quale
effettuare la ricerca sulla base dei possibili valori assunti dai campi
della struttura stessa effettivamente abilitati per la funzionalità di
ricerca articoli

**ATTENZIONE!** all'interno di questo campo verranno visualizzate
solamente le strutture per le quali è stato correttamente selezionato il
parametro "**Abilita Ricerca**" (maschera "**Modifica Struttura
Articoli**")

Per maggiori informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Catalogo -- Gestione Articoli -- Strutture
Ecommerce Mexal / Horeca -- Ricerca Articoli su Campi Struttura*" di
questo manuale

**Campo di ordinamento**: visualizzato solo per filtri sul Campo
Articolo "**Categoria** **Merceologica**" ,"**Categoria**
**Merceologica** **e Sotto Categorie**" o "**Strutture**".

Consente di impostare, selezionandolo dall'apposito menu a tendina,
l'ordinamento degli elementi visualizzati all'interno del componente

**Serie Taglie**: visualizzato solo per filtri sui Campi Articolo
"**Taglie**" o "**Taglie Disponibili**" e solo per Ecommerce Mexal

Permette di selezionare la specifica serie di Taglie / Colori, in
relazione alla quale effettuare la ricerca sulla base dei valori
definiti per la Serie stessa all'interno della corrispondente tabella
gestionale articoli (per maggiori informazioni in merito si veda anche
quanto indicato all'interno del capitolo "*Catalogo -- Gestione Articoli
-- Taglie o Colori Ecommerce Mexal -- Ricerca Articoli per Taglia /
Colore*" di questo manuale)

**Visualizza il numero di elementi per le opzioni:** consente, se
selezionato, di visualizzare a fianco di ogni singola voce in elenco,
anche l'esatto numero degli articoli in catalogo per i quali l'attributo
in esame assume quello specifico valore

**Tipo di visualizzazione per dispositivi mobili \< 992px:** consente di
indicare come dovrà essere gestita la visualizzazione del componente per
dispositivi di risoluzione inferiore a 992px.

E' possibile selezionare una delle seguenti opzioni.

- **DropDown**: in queste condizioni, per dispositivi con risoluzione
  inferiore ai 992px, il componente verrà visualizzato mediante un
  controllo di tipo Drop Down. Nella pagina sarà quindi presente una
  label del tipo di quella evidenziata in figura.

![](./assets/media/image618.png)

> Cliccando sulla label evidenziata verrà aperto un piccolo Pop Up
> contenente tutte le diverse possibili opzioni di scelta offerte dal
> filtro in questione

- **Mantieni visualizzazione Desktop:** consente di mantenere lo stesso
  tipo di visualizzazione indipendentemente dalla risoluzione del
  dispositivo. In queste condizioni dunque, anche per risoluzioni
  inferiori ai 992px le diverse opzioni di selezione del componente
  saranno visualizzate direttamente all'interno della pagina web.

**Campo di ordinamento**: visualizzato solo ed esclusivamente nel caso
in cui il parametro "Tipologia Filtro" sia impostato sul valore "Filtro
su Campo Articolo" e, contestualmente, il parametro "Campo su cui far
filtro" sia impostato sul valore "Categoria Merceologica" o "Categoria
Merceologica e Sotto Categorie".

Consente di definire se l'ordinamento delle categorie e sotto categorie
merceologiche visualizzate all'interno del componente dovrà essere
determinato sulla base della loro **Descrizione**, del loro **Codice** o
del valore **Personalizzato** inserito all'interno del campo "Posizione
nel Menu Categoria" presente nella maschera di configurazione della
categoria stessa.

Per maggiori informazioni in merito a come poter indicare lo specifico
campo Mexal o lo specifico Attributo Passweb su cui dovrà essere
realizzato il filtro di ricerca che si intende implementare si veda
anche il precedente capitolo "*Componenti Ecommerce -- Filtri di
ricerca*" di questo manuale

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

