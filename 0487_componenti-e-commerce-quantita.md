# COMPONENTI E-COMMERCE -- QUANTITA'



Il Componente **"Quantità"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_quantita_res.bmp](./assets/media/image537.png){width="2.5458333333333334in"
height="2.5395833333333333in"}

può essere inserito solo ed esclusivamente all'interno dei componenti
Ecommerce di primo livello "**Carrello Custom**" e "**Wishlist Custom**"
e permette di gestire, all'interno di questi stessi componenti, il
controllo necessario per variare le quantità degli articoli attualmente
presenti in Carrello/Wishlist

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_quantita_2.bmp](./assets/media/image538.png){width="5.190277777777778in"
height="3.6930555555555555in"}

Di base il componente è costituito dall'unità di misura utilizzata dallo
specifico articolo e da un semplice campo di input mediante il quale
poterne variare la quantità in Carrello e/o in Wishlist.

Dipendentemente dai parametri di configurazione del componente, accanto
al campo di input potranno poi essere visualizzati anche due pulsanti
incrementali, "+" e "-" mediante i quali poter variare progressivamente
la quantità attualmente presente in Carrello e/o in Wishlist.

Inoltre **nel caso in cui il Componente Quantità dovesse essere inserito
all'interno di un Componente Wishlist Custom**, in fase di
visualizzazione del dettaglio di una Wishlist**, e solo ed
esclusivamente nel caso in cui la Wishlist in oggetto sia di tipo "Lista
Regalo"**, accanto al campo di input per la gestione delle quantità
comparirà anche un ulteriore campo all'interno del quale verrà mostrata
la quantità ricevuta, ossia la quantità del corrispondente articolo che
è già stata acquistata all'interno della relativa Lista Regalo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_quantita_3.bmp](./assets/media/image539.png){width="5.190277777777778in"
height="3.270138888888889in"}

**ATTENZIONE!** Nel caso in cui l'articolo sia gestito a taglie/colori
verrà visualizzato un campo di input per ogni singola taglia/colore in
maniera tale da permettere all'utente di variare le quantità di ogni
singolo elemento.

Infine nel caso

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_quantita_configurazione_res.bmp](./assets/media/image540.png){width="4.607638888888889in"
height="2.392361111111111in"}

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

- **Visualizza pulsanti incrementali (+/-):** consente, se selezionato,
  di attivare i due pulsanti + e -- utili per variare in maniera
  progressiva la quantità del relativo articolo presente in Carrello e
  /o in Wishlist.

- **Step Incrementale dei pulsanti (+/-):** consente di definire se
  l'incremento progressivo (pulsanti + e -) della quantità del relativo
  articolo presente in Carrello e /o in Wishlist dovrà avvenire per step
  decimali o per singole unità.

- **Posizionamento dei campi delle quantità:** consente di posizionare
  gli elementi utilizzati per impostare la quantità degli articoli
  presenti in Carrello e/o in Wishlist, secondo uno schema prestabilito.

> Nello specifico, gli elementi soggetti al tipo di posizionamento
> impostato mediante questo parametro saranno:

- Pulsante "meno"

- Pulsante "più"

- Campo di input delle quantità

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\posizionamento_campi_quantita_carrello.bmp](./assets/media/image541.png){width="5.907638888888889in"
height="3.1166666666666667in"}

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

- **Ordinamento di visualizzazione dei campi delle quantità**:
  visualizzato solo nel caso in cui il precedente parametro non sia
  stato impostato sul valore Custom.

> Consente di definire l'ordine di visualizzazione degli elementi
> utilizzati per definire la quantità degli articoli attualmente
> presente in Carrello e/o in Wishlist, permettendo dunque, già in fase
> di configurazione del componente stesso di decidere quale elemento
> dovrà essere visualizzato prima e quale dopo.
>
> **ATTENZIONE**! Anche in questo caso l'opzione Custom, non attiva
> nessun tipo di preset per cui l'ordine di visualizzazione dei
> rispettivi elementi potrà essere variato liberamente agendo sulle
> corrette proprietà CSS mediante lo style editor di Passweb e/o
> mediante i relativi strumenti di editing avanzato.

- **Posizionamento del campo "quantità ricevuta" rispetto ai campi della
  quantità:** visibile solo ed esclusivamente nel caso in cui il
  componente "Campo Quantità" sia stato inserito all'interno di una
  Wishlist Custom.

> Permette di decidere se posizionare il campo relativo alle quantità
> ricevute (visibile a sua volta solo nel caso in cui la Wishlist in
> esame sia di tipo "Lista Regalo") a fianco oppure sotto il campo di
> input relativo alle quantità da acquistare

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

