# ISCRIZIONE ALLA NEWSLETTER IN FASE DI MODIFICA DEI DATI UTENTE



Oltre che in fase di registrazione al sito, ci potrebbe essere la
necessità di consentire agli utenti di effettuare l'iscrizione alla
Newsletter anche in un secondo momento operando direttamente all'interno
del loro profilo.

Per soddisfare questo tipo di esigenza sarà quindi necessario inserire
il componente "**Newsletter**" all'interno del componente di primo
livello "**Profilo Utente**".

La configurazione e la gestione del componente sarà in tutto e per tutto
analoga a quando già descritto nei precedenti capitoli di questo
manuale. Il funzionamento del componente, inoltre, sarà sempre lo stesso
indipendentemente dalla piattaforma terza (MailChimp, ActiveCampaign o
Brainlead) che si è deciso di integrare.

In questo senso infatti, la cosa di cui tener conto è cosa è successo in
fase di registrazione al sito.

In sostanza dunque **nel momento in cui in fase di registrazione al sito
l'utente non dovesse essersi iscritto anche alla newsletter**, accedendo
al proprio profilo comparirà esattamente lo stesso Radio Button presente
anche all'interno del form di Registrazione impostato a default sul
valore **No**.

Cambiando l'impostazione di questo campo e selezionando dunque l'opzione
**Si**, verranno visualizzati i campi del form di iscrizione alla
Newsletter (esattamente allo stesso modo di quanto avveniva anche in
fase di registrazione al sito) e l'utente potrà quindi completare la sua
prima iscrizione al servizio.

**Nel momento in cui l'utente dovesse invece aver deciso, in fase di
registrazione al sito, di iscriversi anche alla Newsletter**, il
comportamento del componente cambierà a seconda del fatto che
l'indirizzo mail utilizzato per l'iscrizione alla Newsletter sia o meno
lo stesso di quello utilizzato anche per l'iscrizione al sito.

In particolare nel caso in cui, all'interno del componente di
Registrazione Utente, il campo Mail presente nel form di iscrizione alla
Newsletter:

- **sia stato mappato con il campo Mail utilizzato per l'iscrizione al
  sito**, nel Profilo Utente il radio button relativo all'Iscrizione
  Newsletter sarà impostato automaticamente sul valore **SI**,
  evidenziando quindi che l'utente è già iscritto anche alla Newsletter.

> In queste condizioni inoltre eventuali ulteriori campi del form di
> iscrizione alla Newsletter saranno già valorizzati secondo quanto
> impostato dall'utente stesso in fase di registrazione al sito.

- **NON sia stato mappato con il campo Mail utilizzato per l'iscrizione
  al sito,** nel Profilo Utente il radio button relativo all'Iscrizione
  Newsletter sarà impostato automaticamente sul valore **NO.**

> In queste condizioni dunque l'utente non avrà modo di verificare,
> all'interno del proprio profilo, se è o meno iscritto già anche alla
> Newsletter ( ne tanto meno con quali dati, con quali permessi o a
> quali gruppi di interesse).
>
> Potrà comunque effettuare l'iscrizione e/o modificare i propri dati
> esattamente come poteva farlo in fase di registrazione al sito
> impostando quindi il relativo radio button sul valore SI.
>
> Va detto però che in questo caso, nel momento in cui l'utente dovesse
> indicare esattamente lo stesso indirizzo mail utilizzato per la
> precedente registrazione al sistema di Newsletter verranno
> correttamente modificati i dati precedentemente inseriti.
>
> Nel caso in cui dovesse invece indicare un nuovo indirizzo mail verrà
> effettuata, ovviamente, una nuova iscrizione.

**ATTENZIONE! per ovvie ragioni si consiglia di mappare sempre (tanto
all'interno del componente Registrazione Utente quanto all'interno del
componente Profilo Utente) il campo Mail di iscrizione alla Newsletter
con il campo Mail utilizzato per la registrazione al sito.**

