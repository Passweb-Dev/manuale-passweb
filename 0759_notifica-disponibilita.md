# NOTIFICA DISPONIBILITA'



Come precedentemente evidenziato all'interno della sezione
"Disponibilità" è possibile attivare anche il componente "**Notifica
Disponibilità**" abilitando quindi il sistema di gestione delle
notifiche relative alla richiesta di disponibilità dei vari prodotti.

![](./assets/media/image29.png)

**Gestione Notifica Disponibilità:** consente di attivare il componente
**"Notifica Disponibilità"** determinando anche la sua specifica
modalità di funzionamento.

E' possibile selezionare uno dei seguenti valori:

- **No:** selezionando questo valore **il componente "Notifica
  Disponibilità" non verrà attivato** e, di fatto, non sarà quindi
  possibile abilitare il sistema di gestione delle notifiche relative
  alle disponibilità dei vari prodotti.

> In queste condizioni, inserendo il componente "Notifica Disponibilità"
> all'interno del sito, verrà quindi visualizzato un apposito messaggio

![](./assets/media/image30.png)

- **Ai soli utenti Registrati:** selezionando questo valore il
  componente "Notifica Disponibilità" verrà correttamente attivato ma
  sarà disponibile ai soli utenti registrati.

> In queste condizioni, dunque, nel momento in cui un utente dovesse
> visitare, ad esempio, la pagina prodotto di un articolo attualmente
> non disponibile in cui è stato inserito il componente "Notifica
> Disponibilità", senza aver ancora effettuato l'autenticazione, in
> corrispondenza di questo stesso componente verrà visualizzato un
> apposito messaggio (personalizzabile alla sezione "Gestione Testi /
> Messaggi Sito" del Wizard) per informarlo relativamente alla necessità
> di effettuare l'autenticazione al sito prima di poter richiedere di
> essere avvisato quando il prodotto dovesse tornare ad essere
> disponibile.

![](./assets/media/image31.png)

> Il messaggio in questione sarà inoltre un link che ricondurrà l'utente
> direttamente alla pagina di accesso al sito, alla pagina di
> registrazione o ad una qualsiasi altra pagina scelta in fase di
> configurazione del componente "Notifica Disponibilità".
>
> Una volta effettuata l'autenticazione, l'utente sarà automaticamente
> ricondotto alla precedente pagina prodotto dove il componente
> "Notifica Disponibilità" visualizzerà ora un messaggio diverso

![](./assets/media/image32.png)

> Cliccando su questo messaggio, e richiedendo espressamente di essere
> avvisato nel momento in cui l'articolo dovesse tornare disponibile,
> l'utente riceverà una mail non appena la disponibilità (**memorizzata
> in Passweb**) dell'articolo in esame torni ad essere maggiore di zero

- **A tutti:** selezionando questo valore il componente "Notifica
  Disponibilità" verrà correttamente attivato e sarà disponibile per
  tutti gli utenti del sito, registrati e non.

> In queste condizioni dunque nel momento in cui un utente autenticato
> dovesse visitare, ad esempio, la pagina prodotto di un articolo
> attualmente non disponibile in cui è stato inserito il componente
> "Notifica Disponibilità", visualizzerà esattamente lo stesso messaggio
> del caso precedente.

![](./assets/media/image32.png)

> La mail cui verrà inviata la notifica, sarà, ovviamente, come nel caso
> precedente, quella inserita dall'utente stesso in fase di
> registrazione al sito.
>
> A differenza del caso precedente però, nel momento in cui a visitare
> la pagina dovesse essere ora un utente **non autenticato**, il
> componente "Notifica Disponibilità" visualizzerà un apposito campo di
> input all'interno del quale l'utente, pur non essendo ancora
> registrato al sito, potrà comunque inserire la mail cui dovrà essere
> inviata la notifica di "prodotto nuovamente disponibile"

![](./assets/media/image33.png)

Per maggiori informazioni sulla gestione e configurazione del componente
"Notifica Disponibilità" si veda anche la sezione *"Live Editing --
Lista Componenti Ecommerce -- Componenti interni ai Componenti Ecommerce
-- Componente Notifica Disponibilità"*

Per maggiori informazione relativamente invece al sistema di gestione
delle notifiche di disponibilità prodotto si veda anche la sezione
*"MailChimp -- Notifiche Disponibilità -- Passweb e MailChimp"* di
questo manuale

**ATTENZIONE! Si ricorda che il sistema di gestione delle notifiche di
disponibilità dei prodotti è attivo solo ed esclusivamente in relazione
a quegli articoli per i quali il parametro "Gestione Acquisto" sia stato
impostato sul valore "Acquista solo se disponibile" e l'effettiva
disponibilità degli articoli sia quindi demandata interamente ai valori
memorizzati nel database del sito e aggiornati all'ultima
sincronizzazione utile.**

