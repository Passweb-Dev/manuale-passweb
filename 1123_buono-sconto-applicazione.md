# BUONO SCONTO -- APPLICAZIONE



A differenza delle promozioni che consentono di usufruire di determinati
sconti semplicemente sulla base degli articoli inseriti in Carrello, la
scontistica associata ai Buoni Sconto necessita, per poter essere
applicata, dell'inserimento e della verifica di appositi codici
all'interno del campo del "**Buono Sconto**", campo questo che potrà
essere visualizzato in Carrello (posto di aver selezionato in fase di
configurazione l'apposito parametro "Visualizza Applica Buono Sconto")

![](./assets/media/image596.png)

oppure direttamente in fase di checkout all'interno del modulo d'ordine

![](./assets/media/image597.png)

**ATTENZIONE! Il campo relativo all'inserimento dei codici sconto sarà
visibile solo ed esclusivamente nel caso in cui esista almeno un Buono
Sconto attivo e siano state soddisfatte anche tutte le regole di
validità per esso definite**

Una volta inserito il codice sconto, cliccando sul pulsante "**Aggiorna
Totali Carrello**" (se il codice sconto viene applicato all'interno
della pagina Carrello), oppure sul pulsante "**Applica**" (se il codice
sconto viene applicato direttamente all'interno del modulo d'ordine),
verranno effettuati tutti i controlli necessari e, nel caso in cui
vengano superati, verrà poi applicato il relativo sconto.

Nel caso in cui, invece, tali controlli non dovessero essere superati
(ad esempio perché con l'applicazione del relativo sconto si dovesse
scendere sotto un eventuale minimo d'ordine impostato per il cliente)
verrà visualizzato un apposito messaggio di errore (configurabile dalla
sezione *"Testi / Messaggi Sito"* del Wizard -- componente Checkout o
Checkout Custom)

Inoltre, in relazione all'effettivo utilizzo / applicazione di un codice
sconto e a quanto impostato in fase di configurazione del Buono per i
parametri "**Quantità Totale**" e "**Quantità per singolo utente**" è
bene sottolineare anche che:

- **Nuovo Ordine**: nel momento in cui viene confermato un nuovo ordine
  in cui è stato utilizzato un Codice Sconto, per quello stesso codice
  verrà ovviamente conteggiato un utilizzo.

- **Modifica da sito di ordine in sospeso:** nel momento in cui l'utente
  dovesse decidere di modificare un ordine in stato "Sospeso" per il
  quale aveva utilizzato un Codice Sconto, l'utilizzo di quello stesso
  codice verrà riaccreditato e potrà quindi essere nuovamente utilizzato
  per il nuovo ordine

- **Modifica ordine sul gestionale**: nel momento in cui dovessero
  essere apportate delle variazioni, operando direttamente all'interno
  del gestionale, su di un ordine in cui è stato utilizzato un codice
  sconto vanno distinti due casi diversi:

  - se a seguito delle modifiche effettuate nell'ordine (che viene poi
    riesportato sul sito), dovesse essere ancora presente l'articolo
    spesa utilizzato per gestire il codice sconto originale, tali
    modifiche non avranno alcun effetto dal punto di vista di eventuali
    riaccrediti del codice sconto

  - se, a seguito delle modifiche effettuate nell'ordine (che viene poi
    riesportato sul sito), l'articolo spesa utilizzato per gestire il
    codice sconto originale non dovesse più essere presente l'utilizzo
    di quello stesso codice sconto verrà riaccreditato e l'utente potrà
    quindi utilizzarlo una seconda volta

- **Annullamento ordine in sospeso**: nel momento in cui dovesse essere
  annullato un ordine sospeso in cui era stato utilizzato un codice
  sconto, quello stesso codice verrà riaccreditato e l'utente potrà
  quindi utilizzarlo una seconda volta

- **Cancellazione ordine in stato di "Pagamento non confermato"**: nel
  momento in cui dovesse essere eliminato da Wizard un ordine posto
  nello stato di "Pagamento non confermato" in cui era stato utilizzato
  un codice sconto, quello stesso codice verrà riaccreditato e l'utente
  potrà quindi utilizzarlo una seconda volta

