# TRANSAZIONI PUNTI PREMIO



Nel capitolo precedente di questo manuale abbiamo visto quelli che sono
gli step principali necessari per attivare un sistema di raccolta punti
e quello che un utente dovrebbe fare per effettuare un ordine pagando
con il proprio saldo punti

Ora ci si potrebbe chiedere cosa avverrà nel momento in cui un ordine in
cui sono stati utilizzati dei punti premio dovesse essere annullato,
modificato o sospeso o nel momento in cui dovesse trovarsi negli stati
di "Pagamento non Confermato" o "Da Verificare" e come verrebbero
eventualmente riaccreditati e / o riaddebitati i relativi punti.

In questo senso è quindi bene chiarire che il programma può
effettivamente procedere a degli addebiti / accrediti automatici sul
saldo punti di un cliente secondo le seguenti regole:

- **Nuovo Ordine**: nel momento in cui dovesse essere effettuato un
  nuovo ordine e l'utente dovesse aver scelto di pagarlo (interamente o
  solo in parte) con i suoi punti premio, alla conferma:

  - i punti utilizzati verranno sottratti

  - i punti guadagnati verranno aggiunti al saldo dell'utente sotto la
    voce "**Punti Provvisori**"

- **Esportazione sul sito di Bolle / Fatture originate da Ordini che
  hanno prodotto un accumulo di punti**: solo in questo momento Passweb
  potrà avere la certezza che l'ordine originale che ha prodotto
  l'accumulo di punti è stato effettivamente pagato e quindi sarà
  esattamente in questo momento che i punti accumulati in quello
  specifico ordine passeranno dalla voce "Punti Provvisori" alla voce
  "Punti Guadagnati" e potranno quindi essere effettivamente utilizzati
  nei successivi ordini.

> **ATTENZIONE!** si ricorda che i punti relativi ad ordini in stato
> diverso da "**Trasformato**" o "**Annullato**" verranno sempre e
> comunque considerati come punti "**Provvisori**"

- **Modifica da sito di Ordine in sospeso**: i punti spesi e guadagnati
  nell'ordine iniziale verranno rispettivamente riaccreditati e
  sottratti al saldo attuale dell'utente. I punti relativi al nuovo
  ordine (quello modificato) verranno invece sottratti e aggiunti
  normalmente alla conferma del documento stesso

> **ATTENZIONE!** l'effettivo riaccredito dei punti utilizzati
> nell'ordine in sospeso avviene solo alla conferma di un'eventuale
> variazione di questo stesso ordine. In ogni caso, in fase di
> variazione dell'ordine sospeso, nel saldo punti utilizzabile in
> Carrello o in Checkout saranno conteggiati anche i punti utilizzati
> nell'ordine originale.
>
> Ovviamente alla conferma del nuovo ordine verranno anche sottratti al
> saldo del cliente i nuovi punti eventualmente utilizzati.
>
> Supponiamo dunque di avere per il cliente A un saldo punti di 880 e di
> andare a modificare un ordine in sospeso in cui ne erano stati
> utilizzati 120.
>
> Controllando, in fase di modifica, il saldo del cliente, troveremo
> sempre un valore di 880. Andando però a modificare l'ordine in sospeso
> (aggiungendo o togliendo articoli), il saldo effettivamente
> utilizzabile in carrello non sarà di 880 ma bensì di 1000 (gli 880
> residui più i 120 presenti sul documento in sospeso).
>
> Dopo aver confermato le variazioni apportate al documento, andando a
> ricontrollare il saldo punti del cliente troveremo un accredito di 120
> e un addebito pari al numero di punti eventualmente utilizzati nel
> nuovo ordine.

- **Annullamento Ordine in sospeso dal sito:** nel momento in cui
  l'utente dovesse decidere di annullare un ordine in sospeso i punti
  per esso utilizzati verranno riaccreditati, quelli guadagnati verranno
  invece sottratti al saldo del cliente

- **Annullamento Ordine da gestionale:** nel momento in cui un ordine
  dovesse essere annullato da gestionale e ovviamente riesportato sul
  sito (dove arriverà quindi nello stato di "Annullato") i punti per
  esso utilizzati verranno riaccreditati, quelli guadagnati verranno
  invece sottratti al saldo del cliente

<!-- -->

- **Ordine in stato di "Pagamento non Confermato" / "Da Verificare":**
  nel momento in cui un utente dovesse generare un ordine in questo
  stato:

  - I punti accumulati verranno comunque assegnati all'utente ma
    inseriti tra i "**Punti Provvisori**" e, ovviamente, **non potranno
    essere spesi fintanto che l'ordine resterà in questo stato**

  - I punti spesi **verranno eventualmente riaccreditati solo dopo che
    l'ordine sarà stato correttamente annullato o eliminato**

<!-- -->

- **Cancellazione / Annullamento Ordine in stato di "Pagamento non
  confermato":** nel momento in cui l'amministratore del sito dovesse
  decidere di eliminare / annullare un ordine posto in stato di
  "Pagamento non confermato" i punti per esso utilizzati verranno
  riaccreditati, quelli guadagnati verranno invece sottratti al saldo
  del cliente.

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

Quelle sopra indicate sono tutte le tipologie di addebito / accredito
punti gestite automaticamente dal programma. Per qualsiasi altra
esigenza sarà quindi necessario procedere in maniera manuale modificando
il saldo punti del cliente direttamente all'interno del Wizard di
Passweb.

**ATTENZIONE! eventuali modifiche apportate direttamente sul gestionale
ad ordini in cui sono stati utilizzati punti premio non produrranno
alcun tipo di variazione sul saldo punti attuale del relativo cliente**

