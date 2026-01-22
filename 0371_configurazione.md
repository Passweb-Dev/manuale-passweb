# CONFIGURAZIONE



**Il Componente "Configuratore" può essere inserito, per sua stessa
natura, unicamente all'interno del componente "Scheda Prodotto".**

![](./assets/media/image116.png)

In particolare, lavorando all'interno della pagina "Prodotti" generica,
accessibile dalla corrispondente voce del menu "Gestione Pagine" o
all'interno di una Pagina Prodotto corrispondente ad una specifica
categoria merceologica, il Configuratore non potrà, ovviamente,
utilizzare informazioni reali, relative cioè ad uno specifico articolo.
Al posto di queste informazioni verranno quindi inseriti all'interno del
componente dei segnaposto identificativi dello specifico campo e
conseguentemente della specifica informazione che si vorrà visualizzare
in quella specifica posizione.

Lavorando invece **all'interno della pagina Prodotto relativa ad uno
specifico articolo padre di struttura**, il Componente utilizzerà
informazioni reali, relative allo specifico articolo, simulando quindi
l'esatto comportamento che assumerà all'interno del sito web.

Lavorando infine **all'interno della pagina Prodotto relativa ad un
normale articolo di Magazzino NON padre di struttura,** sarà comunque
possibile inserire il componente all'interno della scheda prodotto ma
questo non verrà visualizzato e non potrà quindi essere personalizzato
in maniera corretta.

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e di configurazione**

![](./assets/media/image117.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome**: consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione**: consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Visualizza il messaggio sui campi Obbligatori:** selezionando questo
  parametro, nel momento in cui un utente dovesse tentare di aggiungere
  in carrello un prodotto non completamente configurato verrà
  visualizzato un apposito messaggio di errore

> Il messaggio di notifica può essere personalizzato inserendo
> l'apposito codice HTML all'interno del campo "**Testo Popup**"
> presente nella sezione "Gestione Testi / Messaggi del Sito" in
> corrispondenza del componente "**Configuratore**"

![](./assets/media/image118.png)

- **Tempo di chiusura popup messaggio (ms):** consente di indicare
  l'intervallo di tempo (in millisecondi) trascorso il quale il popup di
  notifica, impostato mediante il precedente parametro, verrà chiuso in
  automatico

- **Colore dell'Animazione sui campi Obbligatori**: consente di
  specificare il colore da utilizzare nell'animazione che verrà avviata
  nel momento in cui si tenti di inserire in carrello un articolo non
  completamente configurato

- **Colore dell'Animazione sul Prezzo**: consente di specificare il
  colore da utilizzare nell'animazione che verrà avviata nel momento in
  cui la configurazione di un prodotto finito porti alla modifica del
  prezzo originariamente visualizzato in corrispondenza dell'articolo
  padre.

- **Posizionamento dei Campi:** consente di posizionare gli elementi di
  selezione delle diverse possibili opzioni di configurazione gestiti
  mediante select box (menu a tendina), secondo uno schema prestabilito.

> E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

> **ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
> preset presenti in elenco poi il posizionamento degli elementi sarà
> esattamente quello indicato e non potrà essere modificato in alcun
> modo.
>
> **L'opzione Custom consente invece di non applicare nessun preset
> particolare.** **In queste condizioni dunque il posizionamento dei
> vari elementi potrà essere variato liberamente agendo sulle corrette
> proprietà CSS mediante lo style editor di Passweb e/o mediante i
> relativi strumenti di editing avanzato.**
>
> **Posizionamento dei radio button**: consente di posizionare gli
> elementi di selezione delle diverse possibili opzioni di
> configurazione gestiti mediante radio button, secondo uno schema
> prestabilito. E' possibile selezionare uno dei seguenti valori:

- Incolonnati

- Allineati

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

Per quel che riguarda la logica di gestione del suo contenuto, anche
**il Componente "Configuratore" può essere considerato a tutti gli
effetti come un "Componente di tipo Contenitore".**

Per maggiori informazioni relativamente alla gestione dei componenti
interni al Configuratore si veda anche il successivo capitolo di questo
manuale

