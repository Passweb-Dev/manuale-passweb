# STATI ORDINE EBAY



Gli ordini prelevati dai Marketplace eBay possono assumere, all'interno
del proprio sito Passweb, gli stati di seguito elencati:

- **Registrato:** un ordine eBay viene posto in questo stato nel momento
  in cui viene importato per la prima volta dal Marketplace all'interno
  del proprio sito Passweb.

> Tale importazione può avvenire:

- A seguito di una sincronizzazione Sito -- Gestionale (manuale o
  schedulata)

- A seguito di una sincronizzazione Sito -- Marketplace (pulsante
  "Sincro Ordini" in "Gestione Account eBay")

> **ATTENZIONE!** Un ordine eBay nello stato "Registrato" non è ancora
> stato inserito sul gestionale

- **Memorizzato: :** un ordine eBay viene posto in questo stato nel
  momento in cui, dopo essere stato importato sul Passweb, viene
  inserito correttamente anche all'interno del gestionale

> Normalmente, dunque, durante una sincronizzazione "Sito Gestionale"
> eventuali nuovi ordini eBay passano automaticamente da "Registrato" a
> "Memorizzato"

- **In Attesa di Annullamento:** un ordine eBay viene posto in questo
  stato in due diverse possibili situazioni:

  - Il contabile imposta, sul gestionale, tutte le righe del documento
    ad N e inserisce, in testata, una delle causali definite e
    utilizzate per marcare l'annullamento degli Ordini eBay. In queste
    condizioni, durante la prossima Sincronizzazione "Sito - Gestionale"
    Passweb porrà il relativo ordine nello stato di "In Attesa di
    Annullo".

  - L'amministratore del sito accede alla sezione "*eBay -- Ordini*" del
    Wizard, seleziona l'ordine che desidera annullare, clicca sul
    pulsante "Annulla" e imposta uno dei due motivi di annullamento. Al
    salvataggio delle impostazioni l'ordine passerà nello stato di "In
    Attesa di Annullo".

> Lo stato "In Attesa di Annullo" identifica quindi una particolare
> condizione in cui il documento è stato in qualche modo annullato ma
> l'annullamento non è ancora stato comunicato al Marketplace

- **Annullato:** è lo stato successivo a quello di "In Attesa di
  Annullamento" e identifica quindi non solo una condizione in cui il
  documento è stato annullato lato gestionale o lato Passweb, ma anche
  una condizione in cui tale annullamento è stato correttamente
  comunicato al relativo Marketplace.

> **ATTENZIONE! A seguito di una sincronizzazione "Sito Gestionale" gli
> ordini in stato di "In attesa di annullamento" passeranno (di norma)
> nello stato di Annullato**

- **In Attesa di Spedizione:** un ordine eBay viene posto in questo
  stato in due diverse possibili situazioni:

  - **Ecommerce Mexal** -- Il contabile imposta, lato gestionale, nei
    relativi campi il Vettore utilizzato per il trasporto, la data e
    l'ora di inizio trasporto e il Number Tracking assegnato all'ordine.

> In queste condizioni durante la prossima Sincronizzazione "Sito -
> Gestionale" Passweb porrà il relativo ordine nello stato di "In Attesa
> di Spedizione" e valorizzerà i campi "Vettore", "Data Inizio
> Trasporto" e "Number Tracking" della maschera "Parametri di
> Spedizione" sul Wizard del sito, campi questi che saranno ora in sola
> visualizzazione

- **Ecommerce Ho.Re.Ca. -** Il contabile imposta, lato gestionale, nei
  relativi campi del piede del documento il Vettore utilizzato per il
  trasporto (il nome indicato deve essere esattamente lo stesso di
  quello definito, in fase di configurazione del metodo di trasporto su
  Passweb, all'interno del campo "**Nome del Vettore**" ), la data e
  l'ora di inizio trasporto.

> In queste condizioni durante la prossima Sincronizzazione "Sito -
> Gestionale" Passweb porrà il relativo ordine nello stato di "In Attesa
> di Spedizione" e valorizzerà i campi "Vettore", "Data Inizio
> Trasporto" e "Number Tracking" della maschera "Parametri di
> Spedizione" sul Wizard del sito, campi questi che saranno ora in sola
> visualizzazione.

- L'amministratore del sito accede alla sezione "*eBay -- Ordini*" del
  Wizard, seleziona l'ordine che desidera spedire, clicca sul pulsante
  "Spedizione" e verifica i parametri relativi alla spedizione (Vettore,
  Data inizio trasporto, Number Tracking). Al salvataggio delle
  impostazioni l'ordine passerà nello stato di "In Attesa di
  Spedizione".

> Lo stato "In Attesa di Spedizione" identifica quindi una particolare
> condizione in cui l'ordine è stato in qualche modo spedito ma il
> cambiamento di stato non è ancora stato comunicato al Marketplace

- **Spedito:** è lo stato successivo a quello di "In Attesa di
  Spedizione" e identifica quindi non solo una condizione in cui
  l'ordine è stato spedito, ma anche una condizione in cui è stato
  correttamente comunicato al relativo Marketplace il cambio di stato.

> **ATTENZIONE! A seguito di una sincronizzazione "Sito Gestionale" gli
> ordini in stato di "In attesa di spedizione" passeranno (di norma)
> nello stato di "Spedito"**

- **In Attesa di Pagamento** un ordine eBay viene posto in questo stato
  in quando:

  - L'amministratore del sito accede alla sezione "*eBay -- Ordini*" del
    Wizard, seleziona l'ordine che desidera spedire, clicca sul pulsante
    "Pagamento" e imposta il parametro "Pagato" sul valore SI.

> Lo stato "In Attesa di Pagamento" identifica quindi una particolare
> condizione in cui l'ordine eBay è stato in qualche modo pagato ma il
> cambiamento di stato non è ancora stato comunicato al Marketplace

- **Pagato:** è lo stato successivo a quello di "In Attesa di Pagamento"
  e identifica quindi non solo una condizione in cui l'ordine è stato
  pagato, ma anche una condizione in cui è stato correttamente
  comunicato al relativo Marketplace il cambio di stato.

> **ATTENZIONE! A seguito di una sincronizzazione "Sito Gestionale" gli
> ordini in stato di "In attesa di pagamento" passeranno (di norma)
> nello stato di "Pagato"**

