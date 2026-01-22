# ELIMINAZIONE AUTOMATICA DI DOCUMENTI NON PIU' PRESENTI A GESTIONALE



Come indicato nei precedenti capitoli di questo manuale, a seguito di
determinate operazioni effettuate lato gestionale alcuni documenti
potrebbero essere "eliminati" in maniera automatica senza però che
questa informazione venga poi notificata al sito in fase di
sincronizzazione.

Alcuni esempi, in questo senso, possono essere:

- **Trasformazione di un preventivo in Ordine**

> In fase di sincronizzazione viene trasferito sul sito il nuovo ordine
> ma non viene notificato al sito stesso che tale ordine ha avuto
> origine da un determinato Preventivo.
>
> In conseguenza di ciò, dio base, il Preventivo di origine continuerà
> ad essere presente su Passweb anche se il corrispondente documento non
> è più presente all'interno del gestionale

- **Fusione di più documenti in un unico documento dello stesso tipo**
  (es. Fusione di più Bolle in un'unica Bolla)

> In fase di sincronizzazione verranno trasferite le modifiche apportate
> al documento di destinazione della fusione ma non verrà notificato al
> sito l'elenco dei documenti che sono stati fusi assieme.
>
> In conseguenza di ciò i documenti che, lato gestionale, sono
> "scomparsi" perché fusi nell' unico documento ora gestito,
> continueranno, di base, ad essere presenti su Passweb

- **Cancellazione di un documento**

> Nel momento in cui dovesse essere eliminato, all'interno del
> gestionale, un determinato documento presente anche in Passweb, in
> fase di sincronizzazione questa informazione non verrà comunicata al
> sito.
>
> In conseguenza di ciò il documento interessato, di base, continuerà ad
> essere presente all'interno del sito

- ...

In generale dunque, nelle condizioni sopra indicate, per eliminare i
documenti rimasti "appesi" in Passweb sarà necessario operare in maniera
manuale attraverso il pulsante "**Elimina Ordine**" presente all'interno
della maschera "**Lista Ordini**"

**ATTENZIONE! Nel caso di siti collegati a Mexal volendo è possibile
automatizzare la procedura di cancellazione dei documenti rimasti
"appesi" in Passweb**

Questo richiede però l'utilizzo delle Web Api Mexal che dovranno quindi
essere correttamente configurate sia lato gestionale che lato Passweb.

Per maggiori informazioni in merito all'attivazione e alla gestione
delle Web Api all'interno di Mexal si rimanda alla relativa
documentazione di prodotto.

Per quel che riguarda invece l'abilitazione del sito all'utilizzo delle
Web Api Mexal si veda quanto indicato all'interno del capitolo
"*Configurazione -- Mexal Configurazione Gestionale -- Web Api Mexal*"
di questo manuale

Una volta attivate le Web Api all'interno del gestionale e impostate i
relativi parametri di configurazione presenti alla pagina
"**Configurazione -- Configurazione Gestionale**" (sezione Web Api) del
Wizard

![Videate\\parametri_conf_Mexal_webAPI_locale.bmp](./assets/media/image694.png){width="5.870138888888889in"
height="3.558333333333333in"}

in fase di sincronizzazione (per Variati o Totale) verranno poi
effettuate apposite chiamate (una per ogni tipologia di documento
gestita) per ottenere l'elenco dei documenti effettivamente presenti sul
gestionale. Tale elenco verrà poi confrontato con quelli che sono i
documenti presenti sul sito e quelli che risulteranno non essere più
presenti all'interno del gestionale verranno eliminati automaticamente
anche dal sito

**ATTENZIONE!** la procedura automatica di eliminazione dal sito dei
documenti non più presenti all'interno del gestionale richiede
necessariamente l'utilizzo delle Web Api Mexal e, in conseguenza di ciò,
potrà essere applicata solo ed esclusivamente ai siti Ecommerce
collegati a Mexal

Inoltre, considerando che tale operazione avviene in fase di
sincronizzazione sito -- gestionale, per non allungare eccessivamente i
tempi di questa procedura (soprattutto la prima volta che verrà eseguita
dove il numero di documenti da eliminare potrebbe anche essere
particolarmente elevato) **verranno rimossi un massimo di 50 documenti
per ogni sincronizzazione eseguita**

Nel momento in cui dunque i documenti da eliminare dovessero essere più
di 50 sarà necessario procedere a step attraverso sincronizzazioni
successive.

