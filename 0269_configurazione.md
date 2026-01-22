# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico la sua maschera di gestione e configurazione

![](./assets/media/image59.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile settare i
principali parametri di configurazione del componente stesso.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente al parametro
> **Statico** si veda anche quanto indicato all'interno del capitolo
> "*Configurazione Componenti -- Caratteristiche generali* --
> *Staticizzazione e caricamento asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

All'interno della sotto sezione "**Parametri Store Locator**"

![](./assets/media/image60.png)

è possibile gestire alcune opzioni di visualizzazione della mappa. Nello
specifico il parametro :

- **Zoom mappa:** consente di impostare il livello di ingrandimento
  sulla mappa. I valori consigliati sono da 10 a 15.

- **Tipo di Mappa:** consente di selezionare il tipo di mappa che dovrà
  essere utilizzato all'interno del componente. Come nel caso della
  Google Map è possibile selezionare uno dei seguenti valori:
  **Stradale, Satellitare, Terrestre, Ibrida**

- **Punti di interesse:** consente di decidere quali punti di interesse
  (Attrazioni Turistiche, Commercianti, Edifici Governativi ecc...)
  dovranno o meno essere visualizzati all'interno della Google Map oltre
  ai marker appositamente impostati.

> **ATTENZIONE!** I punti di interesse verranno visualizzati solo nel
> caso in cui per la mappa sia stato selezionato il tema Standard

- **Tema:** consente di impostare, selezionandolo dall'apposito menu a
  tendina, uno specifico tema grafico da applicare alla Google Map

All'interno della sotto sezione **"Lista Comandi"**

![](./assets/media/image61.png)

è possibile invece gestire alcune opzioni di visualizzazione
relativamente alla lista dei marker presenti sulla mappa.

Nello specifico il parametro:

- **Titolo:** consente di impostare un Titolo che verrà poi visualizzato
  come primo elemento della colonna contenente l'elenco degli elementi
  (es. Punti Vendita) presenti sulla mappa e i relativi controlli di
  selezione.

- **Posizione Lista Comandi:** permette di decidere dove collocare,
  rispetto alla mappa, la colonna contenente l'elenco dei Punti Vendita
  e i relativi controlli di selezione.

- **Larghezza Lista Comandi:** consente di impostare la larghezza che
  dovrà assumere, all'interno del componente, la colonna contenente
  l'elenco dei Punti Vendita e i relativi controlli di selezione.

![](./assets/media/image62.png)

> Come per tutte le griglie responsive anche in questo caso la larghezza
> di ogni colonna si esprime definendo quante delle 12 sezioni in cui
> risulta essere suddivisa ogni singola riga, dovranno essere
> effettivamente occupate dalla colonna stessa.
>
> **ATTENZIONE!** Indipendentemente dalla larghezza impostata per la
> "Lista Comandi" il comportamento responsivo della griglia principale
> dello Store Locator è tale per cui **in corrispondenza di risoluzioni
> inferiori ai 992 px la griglia stessa si linearizzerà disponendo le
> due colonne una sotto l'altra**

- **Colonne / Righe della Lista:** consente di impostare il numero di
  colonne / righe su cui dovrà essere disposto l'elenco degli elementi
  (es. Punti Vendita) presenti all'interno della "Lista Comandi"

> **ATTENZIONE!** Nel caso in cui il numero complessivo dei markers
> gestiti dovesse essere superiore al totale del numero di righe per il
> numero di colone si attiverà automaticamente la paginazione degli
> elementi in elenco mediante i pulsanti "Precedente" e "Successivo".

- **Visualizzazione risultati:** consente di visualizzare il numero
  complessivo degli elementi (es. Punti Vendita) presenti all'interno
  della "Lista Comandi"

- **Visualizza il percorso testuale:** consente di visualizzare, sulla
  mappa e tramite indicazioni testuali, il percorso da seguire per
  andare dal punto indicato all'interno del campo "Indirizzo" fino al
  marker ad esso più vicino

![](./assets/media/image63.png)

Una volta settati i parametri di configurazione dello Store Locator sarà
poi necessario impostare i vari marker che dovranno essere visualizzati
all'interno della mappa e le eventuali categorie di appartenenza agendo,
in questo senso, dalla sezione "**Gestione Markers e Categorie**"
presente nella maschera di configurazione di questa specifica tipologia
di componenti (per maggiori informazioni in merito si vedano i
successivi capitoli di questo manuale).

![](./assets/media/image64.png)

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

