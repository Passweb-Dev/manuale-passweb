# CREAZIONE E GESTIONE DI UNA GERARCHIA PERSONALIZZATA



Per creare ora una nuova gerarchia occorrerà innanzi tutto definire il
suo gruppo radice. Per far questo sarà necessario portarsi alla pagina
"Utenti -- Gruppi Utenti Sito - Gruppi"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gruppi_utenti_passcom.bmp](./assets/media/image262.png)

e creare un nuovo gruppo cliccando sul corrispondente pulsante presente
nella barra degli strumenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_creazione_gruppo.bmp](./assets/media/image260.png)

Sarà quindi necessario definire il nome del gruppo radice ed
eventualmente le sue caratteristiche a livello di Gestione SMS e
Comunicazione Interna

Una volta creato il gruppo radice sarà necessario stabilire la struttura
della gerarchia definendo quindi i gruppi che ne faranno parte e i vari
legami tra un gruppo e l'altro.

Per poter far ciò sarà sufficiente selezionare il gruppo radice presente
nella parte sinistra della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_nuovo_gruppo_radice.bmp](./assets/media/image263.png)

e utilizzare i pulsanti presenti nella barra degli strumenti per creare
gruppi figli del gruppo radice, per eliminare o spostare gruppi
all'interno dell'albero e, ovviamente per definire gli utenti
appartenenti allo specifico gruppo.

In questo senso i pulsanti presenti nella barra degli strumenti
consentiranno di:

- **Nuovo Gruppo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo_gruppo.bmp](./assets/media/image165.png) ): consente di creare un nuovo gruppo
  figlio del gruppo attualmente selezionato. Nella parte destra della
  maschera sarà possibile definire le caratteristiche del gruppo che si
  sta realizzando.

> In particolare dunque per ogni nuovo gruppo occorrerà indicare:

- **Nome**: etichetta identificativa del gruppo che si sta
  creando/modificando. Tale campo è obbligatorio.

- **Gestione SMS:** se attivato, consente di abilitare, in Area
  Riservata, gli utenti del gruppo all'invio di SMS per notificare ai
  rispettivi destinatari l'inserimento di un nuovo messaggio, di una
  nuova attività in agenda, ecc...

> **ATTENZIONE!** per poter attivare effettivamente l'invio delle
> notifiche SMS è necessario aver impostato correttamente i parametri di
> configurazione presenti all'interno della sezione "**Configurazione
> SMS**" alla pagina "Account e-mail e SMS" del Wizard (menu "*Posta/SMS
> -- Impostazioni -- Configurazione*")
>
> Per maggiori informazioni in merito all'attivazione dell'account SMS
> si rimanda a quanto indicato nel relativo capitolo di questo manuale
> ("*Parametri Posta /SMS -- Configurazione*")

- **Gestione Telegram --** visualizzato solo nel caso in cui sia stato
  acquistato e correttamente configurato il modulo per l'integrazione
  Passweb -- Telegram

> Se attivato, consente di abilitare, in Area Riservata, gli utenti del
> gruppo all'invio delle notifiche Telegram relativamente
> all'inserimento di un nuovo messaggio, di una nuova attività in
> agenda, ecc...
>
> Per maggiori informazioni in merito all'integrazione Passweb --
> Telegram si rimanda a quanto indicato nel relativo capitolo di questo
> manuale ("*Passweb e Telegram*")

- **Gestione Whatsapp --** visualizzato solo nel caso in cui sia stato
  acquistato e correttamente configurato il modulo per l'integrazione
  Passweb -- WA Smart Business

> Se attivato, consente di abilitare, in Area Riservata, gli utenti del
> gruppo all'invio delle notifiche Whatsapp (tramite piattaforma WA
> Smart Business) relativamente all'inserimento di un nuovo messaggio,
> di una nuova attività in agenda, ecc...
>
> Per maggiori informazioni in merito all'integrazione Passweb -- WA
> Smart Business si rimanda a quanto indicato nel relativo capitolo di
> questo manuale ("*Passweb e WA Smart Business*")

- **Comunicazione interna:** se abilitata, consente la comunicazione,
  **a livello di scambio messaggi e documenti**, tra gli utenti dello
  stesso gruppo. A default la comunicazione tra utenti di pari livello è
  abilitata solo per alcuni gruppi della gerarchia automatica di
  Passcom;

- **Comunicazione Livello Superiore**: flaggando questo parametro, verrà
  abilitata in Area Riservata la possibilità di comunicare con i singoli
  utenti dei gruppi padre (collocati quindi ad un livello gerarchico più
  alto) del gruppo in esame. Nel caso in cui tale parametro non venga
  selezionato, la comunicazione verso l'alto potrà essere effettuata a
  livello di intero gruppo ma non a livello di singoli utenti.

<!-- -->

- **Elimina** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image95.png) ): consente di eliminare dalla
  gerarchia il gruppo attualmente selezionato.

> **NOTA BENE:** eliminando un gruppo NON verranno eliminati gli utenti
> in esso contenuti i quali dunque potranno essere gestiti, ed
> eventualmente associati a nuovi gruppi.

Cliccando su questo pulsante verrà visualizzato un messaggio del tipo di
quello qui di seguito riportato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\richiesta_elimina_gruppo.bmp](./assets/media/image168.png)

> consentendo quindi all'utente di decidere se eliminare il singolo
> gruppo oppure anche tutti i suoi gruppi figli. Nel primo caso,
> eliminando il singolo gruppo, gli eventuali gruppi figlio saliranno
> tutti di un livello all'interno della gerarchia. Nel secondo caso
> invece assieme al gruppo selezionato verranno eliminati
> definitivamente anche tutti i gruppi figlio.

- **Sposta** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_sposta.bmp](./assets/media/image167.png) ): consente di spostare il gruppo
  attualmente selezionato in una diversa posizione della gerarchia che
  si sta considerando. Occorrerà quindi selezionare il nuovo gruppo di
  destinazione e cliccare su di esso per effettuare lo spostamento
  (verrà in ogni caso richiesta una conferma per l'operazione che si sta
  effettuando)

- **Lista Utenti** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_lista_utenti.bmp](./assets/media/image166.png) ): consente di visualizzare la lista
  degli utenti attualmente presenti all'interno del gruppo selezionato.
  Cliccando su questo pulsante si verrà quindi ricondotti alla maschera
  "Lista Utenti -- Nome Gruppo"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_lista_utenti_N0.bmp](./assets/media/image264.png)

attraverso la quale poter gestire gli utenti del gruppo attualmente
selezionato.

I pulsanti presenti nella barra degli strumenti, consentono
rispettivamente di:

- **Esportazione Utenti** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_utenti.bmp](./assets/media/image112.png) ): consente di accedere alla maschera di
  esportazione degli utenti del sito in formato csv

- **Elimina Utente** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_utente.bmp](./assets/media/image68.png) ): consente di eliminare l'utente
  attualmente selezionato (**solo per utenti NON Passcom**)

- **Modifica Utente** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_utente.bmp](./assets/media/image10.png) ): consente di modificare l'anagrafica
  dell'utente attualmente selezionato

- **Crea Nuovo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_nuovo.bmp](./assets/media/image257.png) ): consente di creare un nuovo utente
  (**solo per utenti NON Passcom**)

- **Aggiungi al gruppo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_al_gruppo.bmp](./assets/media/image113.png) ): consente di associare al gruppo in
  esame, un qualsiasi utente del sito. Cliccando su questo pulsante
  verrà quindi visualizzata la maschera, **a selezione multipla**, dei
  possibili utenti da aggiungere al gruppo

> **NOTA BENE:** dall'elenco dei possibili utenti da aggiungere al
> gruppo verranno ovviamente esclusi quelli che dello specifico gruppo
> fanno già parte.
>
> Per associare uno più utenti al gruppo in esame sarà quindi
> sufficiente selezionarli all'interno della tabella sopra evidenziata
> (filtrabile attraverso l'apposito pannello di ricerca), e cliccare poi
> sul pulsante "**Aggiungi**" visualizzato nella contestuale barra degli
> strumenti.

