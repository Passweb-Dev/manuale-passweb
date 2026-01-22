# COMPONENTI PER IL FORM -- CAMPO LISTA VALORI



Il Componente per il form **"Campo Lista Valori"**

![](./assets/media/image563.png)

può essere inserito unicamente all'interno dei seguenti componenti
Ecommerce di primo livello:

- **Wishlist Custom**

Permette di gestire un campo di tipo "Select Box" (Menu a Tendina) **che
verrà visualizzato sul front end del sito solo ed esclusivamente nel
caso in cui la Wishlist in oggetto sia di tipo "Lista Regalo",** e che
potrà essere utilizzato dal creatore della relativa Lista per assegnare
al corrispondente articolo una specifica priorità di acquisto.

![](./assets/media/image564.png)

**ATTENZIONE!** Nel caso di articoli "Campionario / Box" (configurabili
e non) il campo in esame verrà visualizzato solo ed esclusivamente sul
"padre" e non sui singoli componenti del Campionario / Box

**ATTENZIONE!** Per maggiori informazioni relativamente alla gestione
delle "Liste Regalo" si veda anche la sezione "*Varianti Sito Responsive
-- Lista Componenti Ecommerce -- Componente Lista Regalo*" di questo
manuale.

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![](./assets/media/image565.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" è possibile settare i
principali parametri di configurazione del componente stesso.

In particolare, per la tipologia di Componente in questione, è possibile
impostare un valore per i seguenti parametri:

- **Nome:** consente di impostare un nome per il Componente che si sta
  editando.

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
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

- **Label:** consente di impostare un'etichetta che verrà visualizzata a
  fianco del corrispondente campo di selezione

- **Testo del controllo senza valori selezionati:** permette di definire
  un testo da utilizzare **come segnaposto** da poter visualizzare,
  inizialmente, all'interno del campo di selezione.

- **Tipo di valore:** consente di definire il tipo di valore che dovrà
  essere utilizzato per popolare la select box in oggetto.

> **E' possibile selezionare unicamente il valore "Priorità"**
>
> In queste condizioni la relativa select box sarà popolata con i valori
> definiti all'interno della sezione "*Utenti -- Wishlist -- Priorità*"
> del Wizard.

![](./assets/media/image566.png)

> Nello specifico i valori disponibili all'interno del menu a tendina
> coincideranno esattamente con la Descrizione assegnata ad ogni singola
> entry della tabella evidenziata in figura (per maggiori informazioni
> in merito si veda anche la sezione "*Utenti -- Wishlist -- Priorità"*
> di questo manuale).

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia la Select Box)

- Il Messaggio di errore

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

- **Ordinamento di visualizzazione dei campi:** visualizzato solo nel
  caso in cui il precedente parametro non sia stato impostato sul valore
  Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> principali del componente in esame, permettendo dunque, già in fase di
> configurazione del componente stesso di decidere quale elemento dovrà
> essere visualizzato prima e quale dopo.
>
> **ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**ATTENZIONE!** Si ricorda che, lato front end il componente in oggetto
verrà visualizzato all'interno delle singole righe presenti in Wishlist
solo ed esclusivamente nel caso in cui la Wishlist selezionata sia di
tipo "Lista Regalo"

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"Avanzate e Animazioni" e "Protezione", presenti nella maschera di
gestione e configurazione di tutti i componenti Passweb, si veda anche
il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

