# COMPONENTI PER IL FORM -- CAMPO DATA



Il Componente per il form **"Campo Data"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_interno_campo_data.bmp](./assets/media/image553.png){width="2.5395833333333333in"
height="2.5458333333333334in"}

può essere inserito solo ed esclusivamente all'interno del componente
Ecommerce di primo livello "**Carrello Custom**" e **solo ed
esclusivamente nel caso di siti Ecommerce collegati a Mexal.**

Permette di gestire un campo di input contenente un apposito controllo
di tipo "Calendario" mediante il quale poter impostare la data di
scadenza di riga su ogni singolo articolo presente in carrello.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\data_scadenza_custom.bmp](./assets/media/image554.png){width="4.920138888888889in"
height="3.6256944444444446in"}

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\data_scadenza_custom_configurazione_res.bmp](./assets/media/image555.png){width="4.607638888888889in"
height="2.926388888888889in"}

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
  fianco del corrispondente campo di input

- **Campo di destinazione:** consente di impostare la destinazione e,
  conseguentemente, la finalità del relativo campo di input per cui,
  sulla base di quanto precedentemente indicato, l'unico valore
  selezionabile per questo parametro sarà **"Data Scadenza"**

- **Tipologia di selezione (solo per varianti Desktop):** consente di
  indicare la specifica tipologia di controllo che verrà poi utilizzato
  per la selezione della data. E' possibile indicare uno dei seguenti
  valori:

  - **Default:** selezionando questa opzione il controllo per la
    selezione della data sarà costituito da un semplice calendario in
    cui l'utente dovrà utilizzare apposite frecce per passare da un mese
    all'altro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_default.bmp](./assets/media/image556.png){width="1.1347222222222222in"
height="1.0368055555555555in"}

- **Mostra menu Mesi:** selezionando questa opzione il controllo per la
  selezione della data sarà costituito da un calendario in cui la
  selezione del mese potrà avvenire anche mediante un apposito menu a
  tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_mesi.bmp](./assets/media/image557.png){width="1.1347222222222222in"
height="1.3618055555555555in"}

- **Mostra menu Anni:** selezionando questa opzione il controllo per la
  selezione della data sarà costituito da un calendario in cui la
  selezione dello specifico anno potrà avvenire mediante un apposito
  menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_anni.bmp](./assets/media/image558.png){width="1.1347222222222222in"
height="1.4111111111111112in"}

- **Mostra menu Mesi e menu Anni:** selezionando questa opzione il
  controllo per la selezione della data sarà costituito da un calendario
  in cui la selezione dello specifico mese così come quella dello
  specifico anno potrà avvenire mediante un apposito menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\calendario_menu_mesi_anni.bmp](./assets/media/image559.png){width="1.1347222222222222in"
height="1.4111111111111112in"}

**ATTENZIONE!** Nel caso in cui si desideri dare la possibilità di
modificare la data di scadenza di riga ai soli Agenti sarà necessario,
per prima cosa, creare un apposito gruppo utenti contenente i soli
Agenti abilitati ad accedere al sito e, successivamente, agire sui
permessi di visibilità (sezione "Protezione") di questo stesso
componente.

- **Posizionamento dei Campi:** consente di posizionare gli elementi
  principali del componente secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia il Campo di input)

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

Il pulsante "Salva" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"Avanzate e Animazioni" e "Protezione", presenti nella maschera di
gestione e configurazione di tutti i componenti Passweb, si veda anche
il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

