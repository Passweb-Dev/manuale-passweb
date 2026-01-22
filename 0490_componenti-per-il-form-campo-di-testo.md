# COMPONENTI PER IL FORM -- CAMPO DI TESTO



Il Componente per il form **"Campo di Testo"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_interno_campo_testo.bmp](./assets/media/image548.png){width="2.5395833333333333in"
height="2.5458333333333334in"}

può essere inserito, dipendentemente dalla tipologia di sito
considerata, all'interno dei componenti Ecommerce di primo livello
"**Carrello Custom**" e/o "**Reso Custom (RMA)**".

In particolare, se inserito all'interno del componente:

- **Carrello Custom (solo Ecommerce Mexal):** permette di gestire un
  campo di input che potrà essere utilizzato dagli Agenti opportunamente
  abilitati per inserire e/o variare gli sconti e/o il prezzo di vendita
  degli articoli presenti in carrello.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campo_testo_carrello_custom.bmp](./assets/media/image549.png){width="5.097916666666666in"
height="3.6319444444444446in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campo_testo_carrello_custom2.bmp](./assets/media/image550.png){width="5.177777777777778in"
height="3.607638888888889in"}

> **ATTENZIONE! In queste condizioni il componente verrà visualizzato
> solo ed esclusivamente nel momento in cui ad effettuare l'ordine per
> conto di un cliente sia un Agente opportunamente abilitato, mediante
> il relativo parametro Mexal, alla modifica degli sconti e/o alla
> modifica dei prezzi.**

- **Reso Custom (RMA):** permette di gestire un campo di input mediante
  il quale l'utente potrà variare le quantità degli articoli presenti
  all'interno del documento di reso merce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campo_testo_reso_custom.bmp](./assets/media/image551.png){width="4.944444444444445in"
height="3.6319444444444446in"}

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_testo_custom_configurazione_res.bmp](./assets/media/image552.png){width="4.613194444444445in"
height="2.938888888888889in"}

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

- **Segnaposto:** permette di definire un testo da utilizzare **come
  segnaposto** da poter visualizzare all'interno del campo di input.

> **ATTENZIONE!** Al click dell'utente sul campo in esame il testo
> indicato scomparirà consentendo quindi all'utente di inserire il
> valore desiderato. Quanto indicato all'interno di questo campo non
> verrà quindi considerato alla conferma del form.

- **Valore di default:** consente di indicare un testo che verrà
  utilizzato (e visualizzato) **come valore di default** per il campo in
  esame.

> **ATTENZIONE!** A differenza di quanto indicato per il precedente
> parametro "Segnaposto", il testo inserito all'interno del campo
> "Valore di default" **non scomparirà** in automatico al click
> dell'utente sul campo di input ma, al contrario, verrà considerato
> come se fosse un vero e proprio valore indicato dall\'utente stesso in
> fase di compilazione.

- **Campo di destinazione:** consente di impostare la destinazione e,
  conseguentemente, la finalità del relativo campo di input per cui,
  sulla base di quanto precedentemente indicato, nel caso in cui il
  componente in oggetto sia stato inserito all'interno del componente
  ecommerce di primo livello:

  - **Carrello Custom (solo Ecommerce Mexal):** gli unici valori
    selezionabile per questo parametro saranno:

    - **Sconto:** in queste condizioni il componente permetterà di
      gestire un campo di input mediante il quale i soli Agenti
      opportunamente abilitati dalla relativa funzionalità Mexal,
      potranno inserire/variare sconti sugli articoli presenti in
      carrello.

    - **Prezzo:** in queste condizioni il componente permetterà di
      gestire un campo di input mediante il quale i soli Agenti
      opportunamente abilitati dalla relativa funzionalità Mexal,
      potranno modificare il prezzo di vendita degli articoli presenti
      in carrello.

> **ATTENZIONE!** Per maggiori informazioni relativamente alla
> possibilità da parte degli Agenti di modificare sconti e/o prezzi di
> vendita si veda anche la sezione "*Configurazione Gestionale -- Mexal
> Parametri Configurazione Gestionale -- Attivazione Passweb --
> Funzionalità Mexal Clienti -- Blocca Modifica Sconto / Modifica
> Prezzo*" di questo manuale.

- **Reso Custom (RMA):** l'unico valore selezionabile per questo
  parametro sarà "**Quantità**". In queste condizioni il componente
  consentirà quindi di gestire un campo di input per la variazione delle
  quantità degli articoli presenti all'interno del documento di reso
  merce.

<!-- -->

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

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"Avanzate e Animazioni" e "Protezione", presenti nella maschera di
gestione e configurazione di tutti i componenti Passweb, si veda anche
il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

