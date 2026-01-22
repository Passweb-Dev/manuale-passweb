# TRANSAZIONI GIFT CARD



Nel capitolo precedente di questo manuale abbiamo visto quello che un
utente dovrebbe fare per effettuare un ordine all'interno del sito
pagando con il saldo di eventuali Gift Card Fisiche o Virtuali caricate
sul proprio account.

Ora ci si potrebbe chiedere cosa dovesse avvenire nel momento in cui un
ordine pagato con Gift Card dovesse essere annullato, modificato o
sospeso e come verrebbero eventualmente riaccreditati e / o riaddebitati
gli importi delle Gift Card presenti all'interno di questo documento.

In questo senso è quindi bene chiarire che il programma può
effettivamente procedere a degli addebiti / accrediti automatici sul
saldo Gift Card di un cliente secondo le seguenti regole:

- **Nuovo Ordine**: nel momento in cui dovesse essere effettuato un
  nuovo ordine per il pagamento del quale si è scelto di utilizzare
  delle Gift Card, alla conferma dell'ordine il saldo Gift Card
  utilizzato all'interno di quel documento verrà addebitato e quindi
  scalato dal saldo Gift Card complessivo caricato sull'account
  dell'utente (nelle modalità descritte all'interno dei precedenti
  capitoli di questo manuale)

- **Modifica da sito di Ordine in sospeso**: gli importi delle carte
  regalo utilizzate all'interno del vecchio ordine (quello in stato
  sospeso) verranno riaccreditati sul saldo Gift Card complessivo
  dell'utente intestatario del documento.

> **ATTENZIONE!** l'effettivo riaccredito dell'importo utilizzato
> nell'ordine in sospeso avviene solo alla conferma di un'eventuale
> variazione di questo stesso ordine. In ogni caso, in fase di
> variazione dell'ordine sospeso, nel saldo Gift Card utilizzabile in
> Carrello o in Checkout sarà conteggiato anche l'importo utilizzato
> nell'ordine originale.
>
> Ovviamente alla conferma del nuovo ordine verranno anche addebitati
> sul saldo Gift Card del cliente i nuovi importi
>
> Supponiamo dunque di avere per il cliente A un saldo Gift Card di 880€
> e di andare a modificare un ordine in sospeso in cui erano stati
> utilizzati 120€ di credito.
>
> Controllando, in fase di modifica, il saldo delle Gift Card del
> cliente, troveremo sempre un valore di 880€. Andando però a modificare
> l'ordine in sospeso (aggiungendo o togliendo articoli), il saldo
> effettivamente utilizzabile in carrello non sarà di 880€ ma bensì di
> 1000€ (gli 880€ residui più i 120€ presenti sul documento in sospeso).
>
> Dopo aver confermato le variazioni apportate al documento, andando a
> controllare le transazioni sulla Gift Card utilizzata troveremo un
> accredito di 120€ e un addebito pari all'importo effettivamente
> utilizzato nel nuovo ordine.

- **Modifica ordine sul gestionale**: nel momento in cui dovesse essere
  variato, operando direttamente all'interno del gestionale, un ordine
  in cui sono state utilizzate delle carte regalo occorrerà considerare
  che:

  - se le variazioni apportate al documento non riguardano gli importi
    delle Gift Card allora, sotto questo punto di vista, verrà lasciato
    tutto inalterato

  - se le variazioni apportate dovessero invece riguardare proprio gli
    importi delle Gift Card utilizzate nel documento allora, al
    trasferimento dell'ordine sul sito, da una parte verranno
    riaccreditati sul saldo Gift Card complessivo dell' utente i vecchi
    importi e allo stesso tempo verranno anche addebitati i nuovi

- **Annullamento Ordine in sospeso:** nel momento in cui l'utente
  dovesse decidere di annullare un ordine in sospeso gli importi di
  eventuali Gift Card precedentemente utilizzati per pagare quello
  stesso documento verranno riaccreditati sul saldo Gift Card
  complessivo dell'utente

- **Cancellazione Ordine in stato di "Pagamento non confermato":** nel
  momento in cui l'amministratore del sito dovesse decidere di eliminare
  un ordine posto in stato di "Pagamento non confermato" e parte di
  quest'ordine dovesse essere stato pagato con una Gift Card, l'importo
  effettivamente utilizzato verrà riaccreditato sul saldo Gift Card
  complessivo dell'utente.

**ATTENZIONE!** Quelle sopra indicati sono tutte le tipologie di
addebito / accredito sul saldo Gift Card complessivo di un utente che
vengono effettuati automaticamente dal programma. Per qualsiasi altra
esigenza sarà quindi necessario procedere in maniera manuale modificando
il residuo del relativo codice Gift Card direttamente all'interno del
Wizard di Passweb.

