# ESPORTAZIONE/ELIMINAZIONE DI SERVIZI/TRATTAMENTI DAL GESTIONALE HO.RE.CA AL SITO WEB.



Per poter esportare e gestire all'interno del sito web uno specifico
servizio/trattamento presente nel gestionale Ho.Re.Ca. è sufficiente
agire dall'anagrafica del trattamento stesso.

In particolare sarà necessario:

1.  Abilitare il servizio/trattamento desiderato affinché questo possa
    essere correttamente esportato all'interno del sito

2.  Assegnare al servizio/trattamento da gestire all'interno del sito le
    specifiche risorse che dovranno essere prenotabili via web

> **NOTA BENE:** le risorse associate ai trattamenti/servizi gestiti via
> web, non vengono inviate al sito in fase di sincronizzazione, ma
> vengono gestite ed inviate in modo dinamico nel momento stesso in cui,
> in fase di prenotazione web, verrà richiesta la disponibilità dello
> specifico trattamento/servizio.

Portandosi quindi all'interno dell'anagrafica dello specifico servizio,
nella scheda "**Lista Articoli e Listini**" sarà possibile trovare il
campo **"Abilita Passweb"** che, se selezionato, consentirà, a partire
dalla prossima sincronizzazione, di esportare e gestire il trattamento
stesso anche all'interno del corrispondente sito Passweb.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\anagrafica_servizi1.bmp](./assets/media/image112.png)

- **Abilita Passweb**: se selezionato consentirà, **a partire dalla
  prossima sincronizzazione**, di esportare e gestire il trattamento in
  esame all'interno del corrispondente sito Passweb.

> **NOTA BENE:** dopo aver impostato per ogni singolo trattamento il
> valore desiderato per il campo "Abilita Passweb", è di fondamentale
> importanza lanciare una sincronizzazione in modo tale da consentire a
> Passweb di prelevare dal gestionale Ho.Re.Ca. tutti quei trattamenti
> che si è deciso di gestire e di esportare all'interno del proprio
> sito.

Nel caso in cui si decida invece di eliminare e di non gestire più
all'interno del proprio sito determinati trattamenti, fino a quel
momento correttamente gestiti, sarà sufficiente deselezionare il
parametro in oggetto e lanciare poi una nuova sincronizzazione.

> **NOTA BENE:** il numero complessivo di trattamenti/servizi che è
> possibile gestire all'interno del sito varia in relazione alla
> tipologia di contratto sottoscritto.

Per quel che riguarda invece l'assegnazione allo specifico
trattamento/servizio delle varie risorse che dovranno essere prenotabili
via web, sarà necessario agire sempre dall'anagrafica del relativo
trattamento, questa volta però all'interno della scheda "**Risorse".**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\anagrafica_servizi2.bmp](./assets/media/image113.png)

In particolare all'interno della tabella "**Tipi risorsa**" sarà
possibile indicare gli eventuali tipi di risorse che dovranno poi essere
inviati al sito ai fini di una prenotazione via web dello specifico
trattamento.

> **NOTA BENE:** a default i valori presenti all'interno di questa
> tabella vengono ereditati dagli analoghi valori impostati sulla
> categoria merceologica di appartenenza del trattamento stesso

Ad esempio, nel caso di un trattamento del tipo "Emotional Massage",
sarà possibile decidere di far prenotare via web una delle tre risorse
associate a questo tipo di servizio scegliendo tra il Massaggiatore
specializzato, il Lettino o l'estetista.

In questo senso dunque le colonne **"Qta minima"** e , **"Qta"**
indicano rispettivamente la quantità di risorse obbligatorie e la
quantità totale di risorse facoltative che dovranno essere considerate
per lo specifico trattamento.

La colonna **"Passweb"** consente invece di specificare se la
corrispondente risorsa dovrà o meno essere inviata al sito ai fini di
una sua prenotazione via web.

In ogni caso va comunque ricordato che solo una delle risorse proposte
potrà effettivamente essere resa prenotabile via web.

**IMPORTANTE: Relativamente alla prenotazione via web (attraverso il
corrispondente sito Passweb) dei servizi/trattamenti con più risorse
associate, è necessario indicare una sola risorsa obbligatoria, l'unica
che verrà di fatto inviata al sito, con Qta minima = 1. Tutte le altre
risorse eventualmente associate allo specifico trattamento/servizio,
dovranno essere impostate con Qta minima = 0.**

**In sostanza dunque ai fini della prenotazione via web i
trattamenti/servizi multi risorsa dovranno essere considerati come
quelli mono risorsa. Le eventuali ulteriori risorse, impostate come
facoltative sulla base dei parametri presenti all'interno della tabella
"Tipi risorsa", dovranno quindi essere associate al trattamento/servizio
dal gestore, operando direttamente all'interno del gestionale Ho.Re.Ca.
sulla prenotazione che questo ha ricevuto dal sito web.**

> **NOTA BENE:** nel caso in cui vengano configurate più risorse come
> obbligatorie (quindi con Qta minima =1) in fase di prenotazione web
> del corrispondente servizio/trattamento potrebbe essere ritornato un
> messaggio di errore (lo stesso visualizzato nel caso di overbooking
> della risorsa).

In particolare il controllo sull'obbligatorietà delle risorse verrà
effettuato o meno, dipendentemente dal fatto di aver selezionato,
all'interno del gestionale, il corrispondente parametro **"Abilita
Controllo Risorse"** (menu "Opzioni di installazione" scheda "Opzioni
Avanzate")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prenotazione_10.bmp](./assets/media/image114.png)

Ciò significa quindi che nel caso in cui il parametro sopra evidenziato
sia stato effettivamente selezionato all'atto dell'inserimento di una
nuova prenotazione verrà effettuato un controllo relativamente al fatto
che tutte le risorse impostate come obbligatorie per lo specifico
trattamento siano state effettivamente selezionate.

In queste condizioni, considerando che ,via web, è comunque possibile
prenotare una sola risorsa, se il trattamento fosse stato configurato
con due o più risorse obbligatorie alla conferma della prenotazione, con
il conseguente tentativo da parte di Passweb di inserire la prenotazione
stessa all'interno del gestionale, verrebbe ritornato un errore di
risorsa non disponibile e la prenotazione del trattamento non verrebbe
quindi inserita.

Nel caso in cui invece il parametro sopra indicato non fosse stato
selezionato, non verrebbe avviato, all'atto dell'inserimento di una
nuova prenotazione, nessun controllo di obbligatorietà per cui, in
queste condizioni, anche se per lo specifico trattamento fossero state
impostate due o più risorse come obbligatorie e anche se da web è
comunque possibile prenotarne una sola, la relativa prenotazione web
verrebbe comunque inserita e codificata all'interno del gestionale.

> **NOTA BENE:** i controlli di obbligatorietà sulle risorse associate
> ad un trattamento verranno considerati, per le prenotazioni via web,
> solo ed esclusivamente nel caso in cui queste stesse prenotazioni
> siano state pagate (prenotazione web che nasce nel gestionale nello
> stato di "Confermata").

**Nel caso in cui in fase di configurazione del sito si sia scelto di
non mostrare lo step per la selezione del pagamento, la relativa
prenotazione verrà sempre inserita nel gestionale nello stato di
"Preventivo", indipendentemente da eventuali situazioni di overbooking
e/o di risorse obbligatorie non selezionate**

