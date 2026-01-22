# FASE 3 -- INSERIMENTO DEI DATI UTENTE



In questa fase l'utente dovrà andare ad inserire, all'interno di un
apposito form, i propri dati anagrafici che verranno poi utilizzati per
registrare la prenotazione all'interno del gestionale.

![](./assets/media/image381.png)

Il form evidenziato in figura è gestito mediante l'inserimento
all'interno della "Prenotazione Risorse Custom" di un componente
"**Registrazione Utente**".

In fase di configurazione del componente sarà quindi possibile decidere
liberamente quali e quante informazioni richiedere all'utente tenendo
comunque sempre in considerazione il fatto che Nome Cognome e Indirizzo
Email dovrebbero essere dati da richiedere in maniera obbligatoria per
fare in modo che la prenotazione e la relativa anagrafica utente possano
poi essere inserite correttamente all'interno del gestionale.

Sotto questo aspetto occorre anche considerare che sul gestionale verrà
poi inserita una prenotazione (non un ordine) per cui non saranno
necessarie informazioni quali ad esempio un indirizzo di spedizione o di
fatturazione. Inoltre se ad effettuare la prenotazione dovesse essere
un'azienda questa avrà poi la possibilità di richiedere fattura una
volta arrivata in struttura.

Infine, dipendentemente da come viene realizzato e gestito il sito,
l'utente potrebbe avere anche la possibilità di registrarsi e
autenticarsi prima ancora di effettuare la prenotazione, creando quindi
un proprio Account utile per consultare in un secondo momento lo storico
delle proprie prenotazioni o per gestire i propri dati anagrafici.

Se così fosse in questo step del processo di prenotazione i dati
anagrafici dell'utente sarebbero già compilati in base alla login
effettuata.

