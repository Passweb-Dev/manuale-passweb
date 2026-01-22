# ORDINI



Ovviamente oltre a Clienti, Articoli e Carrelli Abbandonati, Passweb
invierà allo Store MailChimp anche tutte le informazioni relative agli
ordini effettuati all'interno del nostro sito Ecommerce.

Nello specifico è bene quindi ricordare che:

- Ogni nuovo ordine effettuato all'interno del sito sarà inviato anche
  allo Store MailChimp, nello stato di "**Pending**", **contestualmente
  all'inserimento di questo stesso ordine all'interno del gestionale**.

> **ATTENZIONE!** eventuali nuovi ordini verranno inviati allo Store
> MailChimp solo ed esclusivamente nel momento in cui questi stessi
> ordini saranno inseriti anche all'interno del gestionale
>
> Nel caso in cui, dunque, un nuovo ordine dovesse rimanere, per
> qualsiasi ragione, localizzato solamente all'interno di Passweb (ad
> esempio in stato di "Pagamento non confermato") questo non verrà mai
> inviato allo Store MailChimp.
>
> Per sbloccare questa situazione ed inviare quindi anche questo tipo di
> ordini allo Store Mailchimp è necessario, per prima cosa, fare in modo
> che questi stessi ordini vengano inseriti anche all'interno del
> gestionale.

- Nel momento in cui un determinato ordine dovesse passare, a seguito di
  una sincronizzazione Sito -- Gestionale, nello stato di
  "**Annullato**", questo stesso documento verrà inviato, al termine
  della stessa sincronizzazione, anche allo Store MailChimp nello stato
  di "**Cancelled**".

> Ovviamente nel caso in cui l'ordine dovesse già essere presente nello
> Store MailChimp, ad esempio nello stato di "Pending", al termine della
> sincronizzazione verrà semplicemente aggiornato il suo stato (in
> realtà se necessario verrà aggiornato anche il corpo di questo stesso
> documento)

- Nel momento in cui un determinato ordine dovesse passare, a seguito di
  una sincronizzazione Sito -- Gestionale, nello stato di "**Bollato**",
  al termine della stessa sincronizzazione lo stesso documento verrà
  inviato anche allo Store MailChimp nello stato di "**Shipped**"

> Ovviamente nel caso in cui l'ordine dovesse già essere presente nello
> Store MailChimp, ad esempio nello stato di "Pending", al termine della
> sincronizzazione verrà semplicemente aggiornato il suo stato

- Nel momento in cui un determinato ordine dovesse passare, a seguito di
  una sincronizzazione Sito -- Gestionale, nello stato di "Fatturato",
  al termine della stessa sincronizzazione lo stesso documento verrà
  inviato anche allo Store MailChimp nello stato di "**Paid**"

> Ovviamente nel caso in cui l'ordine dovesse già essere presente nello
> Store MailChimp, ad esempio nello stato di "Pending", al termine della
> sincronizzazione verrà semplicemente aggiornato il suo stato

Inoltre sempre in merito al trasferimento ordini da Passweb verso lo
Store MailChimp è bene sottolineare altre due cose di fondamentale
importanza:

- Allo stato attuale non esiste un'operazione di sincronizzazione
  manuale che consenta di importare gli ordini attualmente presenti su
  Passweb all'interno dello Store Mail Chimp. Tale operazione, se
  necessaria, viene infatti eseguita automaticamente da Passweb al
  termine di ogni sincronizzazione Sito -- Gestionale (Totale o per
  Variati).

> Nel caso in cui l'esigenza dovesse essere dunque non solo quella di
> trasmettere a MailChimp informazioni relative a nuovi ordini ma anche
> quella di **trasferire sullo Store MailChimp una "Storico ordini",
> sarà necessario per prima cosa variare questi stessi ordini
> all'interno del gestionale** e attendere poi la prima sincronizzazione
> schedulata o, eventualmente, lanciarne una manuale, prima di poter
> verificare la presenza di questo tipo di dati all'interno dello Store
> MailChimp

- A seguito di ogni sincronizzazione Sito -- Gestionale verranno
  trasmessi allo Store MailChimp solo ed esclusivamente ordini intestati
  a clienti presenti anche all'interno della Lista collegata allo Store
  MailChimp.

**ATTENZIONE!** Lato Mailchimp è possibile abilitare e configurare dei
Trigger tali per cui al cambiamento di stato di un ordine possano essere
inviate in maniera automatica specifiche mail transazionali.

**Nel caso in cui si decida di attivare questi trigger l'utente, al
cambio di stato di un ordine (ad esempio da "Memorizzato" a "Fatturato")
potrebbe ricevere due distinte mail, una inviata da Passweb ed una
inviata da MailChimp.**

Per maggiori informazioni relativamente alle mail inviate in automatico
da Passweb al cambio di stato di un ordine (ed eventualmente a come
disattivarle) si rimanda all'apposito capitolo ("*Ordini --
Configurazione Ordini -- Dati Email*") di questo manuale.

Per maggiori informazioni relativamente a come poter configurare lato
MailChimp trigger che scatenino l'invio di apposite mail al cambio di
stato di un ordine si rimanda alla specifica documentazione di prodotto
([www.mailchimp.com](http://www.mailchimp.com))

**ATTENZIONE!** Una volta configurato correttamente lo Store MailChimp,
al termine della sincronizzazione verrà inviata anche una mail
contenente un report relativo alle attività di sincronizzazione tra
Passweb e MailChimp.
