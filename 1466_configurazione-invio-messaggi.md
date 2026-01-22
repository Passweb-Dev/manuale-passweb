# CONFIGURAZIONE INVIO MESSAGGI



La sezione "**Configurazione Invio Messaggi**" visibile all'interno
della maschera "**Dati Account**" solo dopo aver inserito e salvato i
parametri "**BOT Token**" e "**BOT Username**", consente di definire gli
eventi in relazione ai quali dovranno essere inviati dei messaggi
Telegram e di impostare anche il Template che dovrà essere utilizzato
per l'invio di questi stessi messaggi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_configurazione_messaggi.bmp](./assets/media/image17.png)

La griglia presente sul lato sinistro della sezione "**Template
Messaggi**" consente di visualizzare quelli che sono gli eventi già
configurati e in relazione ai quali verranno già inviati messaggi
Telegram utilizzando gli appositi Template.

I pulsanti presenti nella contestuale barra degli strumenti, consentono
rispettivamente di:

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image18.png) ): consente di eliminare l'evento attualmente
selezionato in elenco

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_modifica.bmp](./assets/media/image19.png) ): consente di modificare l'evento
attualmente selezionato in elenco.

**Aggiungi** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image20.png) ): consente di codificare un nuovo
evento ed il relativo messaggio Telegram

Cliccando su questo pulsante, verrà infatti visualizzata, sulla destra
della pagina la sezione "**Nuovo Template**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_nuovo_template.bmp](./assets/media/image21.png)

all'interno della quale poter definire l'evento e il gruppo di utenti in
relazione al quale dovrà essere inviato un messaggio Telegram e il
Template da utilizzare per questo stesso messaggio

Nello specifico dunque il parametro:

**Nome dell'azione**: consente di assegnare un nome all'evento che si
sta configurando in modo tale da poterlo poi individuare facilmente tra
tutti gli eventi già presenti in elenco

**Tipologia dell'azione**: consente di indicare, selezionandola da un
apposito menù a tendina, l'azione e quindi lo specifico evento in
relazione al quale dovrà essere inviato un messaggio Telegram

È possibile selezionare uno dei seguenti valori:

- **Notifica Stato Ordine:** selezionando questa opzione l'evento che
  scatenerà l'invio del messaggio Telegram, sarà il passaggio
  dell'ordine in uno degli stati indicati in corrispondenza del
  successivo parametro "**Stati Ordine Gestiti**".

> Il destinatario della notifica sarà invece l'intestatario dello
> specifico ordine.
>
> Nel caso in cui l'esigenza dovesse essere, ad esempio, quella di
> inviare un messaggio Telegram agli utenti del sito nel momento in cui
> il loro ordine dovesse essere nello stato di Confermato, sarà quindi
> sufficiente selezionare questo stato dal box di sinistra ed inserirlo
> in quello di destra cliccando sull'icona raffigurante una piccola
> freccia verde

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_nuovo_template_2.bmp](./assets/media/image22.png)

> Volendo è possibile selezionare anche più di uno stato
> contemporaneamente, in questo caso però il messaggio potrà variare
> solamente in relazione alle variabili dinamiche inserite nel Template
> utilizzato per l'invio.

- **Testo Pulsante Stato Ordine**: il testo definito per il Template
  associato a questa Tipologia di Azione non verrà utilizzato per
  l'invio di un messaggio Telegram.

> **Verrà utilizzato invece come testo del pulsante presente nei
> messaggi di "Stato Ordine"**
>
> Cliccando su questo pulsante l'utente verrà ricondotto automaticamente
> sul sito Ecommerce al dettaglio del corrispondente documento (posto
> ovviamente di aprire il collegamento sul browser e di aver già
> effettuato l'autenticazione al sito)

- **Notifica carrello abbandonato:** in queste condizioni l'evento che
  scatenerà l'invio del messaggio Telegram sarà la creazione di un
  carrello abbandonato.

> Il destinatario della notifica sarà invece l'utente che ha creato lo
> specifico carrello abbandonato
>
> In relazione a questa specifica tipologia di eventi è bene evidenziare
> che:

- **la creazione di un Template per l'invio dei messaggi relativi ai
  carrelli abbandonati non è retroattiva**. Ciò significa dunque che al
  salvataggio di questo Template, eventuali carrelli abbandonati
  presenti sul sito (e creati quindi prima dell'attivazione di questo
  stesso Template) verranno automaticamente impostati come già inviati.
  Tale impostazione è relativa ovviamente alle sole notifiche Telegram

- le notifiche di carrello abbandonato verranno inviate alla prima
  sincronizzazione utile successiva all'intervallo di tempo indicato in
  corrispondenza del parametro "**Intervallo per invio messaggio
  carrelli**" (per maggiori informazioni in merito si veda anche quanto
  indicato nei precedenti capitoli di questo manuale)

- indipendentemente dalle impostazioni settate, **non verranno mai
  inviate notifiche di carrelli abbandonati creati da Agenti**

- verrà considerato sempre e soltanto l'ultimo carrello abbandonato
  effettivamente creato dallo specifico utente. In conseguenza di ciò
  nel momento in cui il parametro "**Gestione Carrello al Login**"
  (pagina "**Configurazione Catalogo**" del Wizard) dovesse essere
  impostato sull'opzione "**Rileva Carrello Utente -- Gestione
  Separata**" ogni nuova copia dello stesso carrello sposterà in avanti
  la data di invio della notifica

<!-- -->

- **Testo Pulsante Carrello Abbandonato**: il testo definito per il
  Template associato a questa Tipologia di Azione non verrà utilizzato
  per l'invio di un messaggio Telegram.

> **Verrà utilizzato invece come testo del pulsante presente nei
> messaggi di "Notifica Carrello Abbandonato"**.
>
> Cliccando su questo pulsante l'utente verrà ricondotto automaticamente
> sul sito Ecommerce al dettaglio del corrispondente carrello (posto
> ovviamente di aprire il collegamento sul browser e di aver già
> effettuato l'autenticazione al sito)

- **Messaggio di benvenuto**: in queste condizioni l'evento che
  scatenerà l'invio del messaggio Telegram sarà l'autorizzazione
  espressa dal cliente alla ricezione di messaggi da parte
  dell'esercente.

> In sostanza il messaggio inviato in questo caso sarà esattamente
> quello che riceve l'utente subito dopo aver effettuato l'iscrizione al
> Bot tramite il "Widget di Login Telegram" inserito sul sito
>
> **ATTENZIONE!** per maggior informazioni relativamente al Widget di
> Login Telegram si veda anche quanto indicato nel successivo capitolo
> "*Configurazione Widget Login*" di questo manuale

- **Notifica invio messaggio**: l'evento che scatenerà la notifica
  Telegram sarà l'invio di un nuovo messaggio in Area Riservata.

> Il destinatario della notifica sarà invece il destinatario del
> messaggio stesso.

- **Notifica lettura messaggio**: l'evento che scatenerà la notifica
  Telegram sarà la lettura, da parte del destinatario, di un messaggio
  inviatogli in Area Riservata

> Il destinatario della notifica sarà invece il mittente del messaggio

- **Notifica cambio stato attività**: l'evento che scatenerà la notifica
  Telegram ad un determinato utente sarà il cambio di stato di una delle
  attività ad esso assegnate in Area Riservata

> Il destinatario della notifica sarà invece il creatore dell'attività

- **Notifica presa visione attività**: l'evento che scatenerà la
  notifica Telegram sarà la presa visione, da parte del relativo
  destinatario, di un'attività ad esso assegnata

> Il destinatario della notifica sarà invece il creatore dell'attività

- **Promemoria attività**: l'evento che scatenerà la notifica Telegram
  sarà la scadenza di un Promemoria assegnato ad una delle attività
  presenti in Area Riservata (sezione "Agenda")

> Il destinatario della notifica sarà invece l'utente che ha inserito,
> per la sua attività, uno specifico promemoria

- **Notifica Upload File**: l'evento che scatenerà la notifica Telegram
  sarà l'upload di un file nella sezione "Documenti" di Area Riservata
  (per i siti commercialista sono considerati sia gli Upload manuali che
  gli Upload in Docuvision a patto però di gestire correttamente le Web
  Api Mexal)

> Il destinatario del messaggio sarà invece l'amministratore associato
> alla cartella in cui viene caricato il file

- **Notifica Download File**: l'evento che scatenerà la notifica
  Telegram sarà il download (pulsante "Scarica") di un nuovo file
  precedentemente caricato nella sezione Documenti dell'Area Riservata

> Il destinatario sarà invece l'amministratore associato alla cartella
> in cui si trova il file

- **Notifica presa visione File**: l'evento che scatenerà la notifica
  Telegram sarà la presa visione (pulsante "Anteprima") di un file
  precedentemente caricato nella sezione Documenti dell'Area Riservata

> Il destinatario sarà invece l'amministratore associato alla cartella
> in cui si trova il file

**ATTENZIONE!** in relazione alle notifiche relative agli eventi di Area
Riservata è necessario, ovviamente, che i relativi destinatari abbiano
effettuato l'iscrizione al Bot Telegram mediante l'apposito pulsante da
inserire sul front end del sito (per maggiori informazioni in merito si
vedano i precedenti capitoli di questo manuale). In caso contrario
infatti nessuna di queste notifiche potrà essere ricevuta

Va detto anche che, a differenza dei messaggi relativi agli Stati Ordine
e/o ai Carrello Abbandonati, messaggi questi inviati in automatico
dall'applicazione al verificarsi del relativo evento, le notifiche
legate agli eventi di Area Riservata (es. Notifica Invio Messaggio)
verranno inviate invece solo nel momento in cui l'utente decida
effettivamente di voler inviare anche questo tipo di notifica (oltre ad
esempio alla notifica mail o SMS) selezionando per questo l'apposito
check

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_check_notifica_telegram.bmp](./assets/media/image23.png)

Per maggiori informazioni relativamente alle opzioni di notifica legate
agli eventi di area riservata si veda anche quanto indicato all'interno
del capitolo "*Siti Ecommerce Area Riservata e B2B*" di questo manuale

**ATTENZIONE!** per far sì che un utente possa avere la possibilità di
abilitare anche la notifica Telegram relativa ad uno degli eventi
gestiti in Area Riservata è necessario accertarsi che, per il suo gruppo
di appartenenza, sia stato selezionato, in fase di configurazione, il
check "**Gestione Telegram**" (per maggiori informazioni in merito si
veda anche quanto indicato all'interno del capitolo "*Utenti -- Siti
Ecommerce -- Gruppi Utenti Sito -- Configurazione di un Gruppo Utenti --
Sezione Area Riservata*" di questo manuale)

**Gruppi:** consente di impostare i Gruppi Utente in relazione ai quali
poter effettivamente attivare l'invio del relativo messaggio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_template_gruppi_utente.bmp](./assets/media/image24.png)

**ATTENZIONE!** nel momento in cui l'esigenza dovesse essere quella di
poter inviare il messaggio in esame a tutti gli utenti del sito,
indipendentemente dal loro gruppo di appartenenza, sarà sufficiente
verificare di non aver attivato, in corrispondenza di questo parametro,
nessun gruppo di utenti

Nel momento in cui l'esigenza dovesse essere invece quella di abilitare
l'invio del messaggio in esame solamente a specifici gruppi utente, sarà
sufficiente selezionare i gruppi desiderati dal box di sinistra ed
inserirli in quello di destra cliccando sulla piccola freccia verde.

**ATTENZIONE!** **una volta inseriti uno o più gruppi utente nel box di
destra, il messaggio in esame potrà poi essere inviato (coerentemente
con le altre impostazioni del sito) solo ed esclusivamente agli utenti
di quegli stessi gruppi**

Ovviamente il fatto di appartenere ad uno dei gruppi indicati non
garantisce che l'utente possa poi ricevere effettivamente il messaggio
in esame. Per poter ricevere tale messaggio infatti, oltre ad
appartenere al gruppo indicato, l'utente dovrà anche aver effettuato
l'iscrizione al bot telegram e dovrà anche non aver esercitato la
corrispondente opzione di opt out (per maggiori informazioni in merito
si veda anche quanto indicato nei successivi capitoli di questo manuale)

**Testo del Template**: consente di definire il corpo del messaggio
Telegram che verrà inviato al verificarsi dell'evento impostato in
corrispondenza del precedente parametro "**Tipologia dell'azione**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_testo_template.bmp](./assets/media/image25.png)

**ATTENZIONE!** è possibile utilizzare anche tag HTML **solo però nel
caso in cui il testo inserito non sia quello relativo ai pulsanti "Stato
Ordine" e "Carrello Abbandonato"** (Telegram non ammette infatti l'uso
di Tag HTML nel testo dei suoi pulsanti)

Il campo "**Seleziona un segnaposto**" consente di inserire all'interno
del messaggio dei segnaposto dinamici (es. Nome e Cognome Utente, Totale
dell'ordine, Numero Articoli in ordine ...) che verranno sostituiti in
fase di creazione del messaggio con i corrispondenti valori.

In relazione alla diversa tipologia di evento indicata sarà possibile
utilizzare uno dei seguenti segnaposto:

- **Cognome**: sostituito in fase di generazione del messaggio con il
  Cognome / Ragione Sociale dell'utente destinatario del messaggio

- **Nome**: sostituito in fase di generazione del messaggio con il Nome
  dell'utente destinatario del messaggio

- **Nominativo**: sostituito in fase di generazione del messaggio con il
  Nome e il Cognome/Ragione Sociale dell'utente destinatario del
  messaggio.

> **ATTENZIONE!** nel caso in cui la tipologia di azione selezionata
> dovesse essere "**Notifica Upload File**" il segnaposto "Nominativo",
> così anche come "Cognome" e "Nome", verranno sostituiti con il Nome e
> il Cognome/Ragione Sociale dell'utente che ha uplodato il file che,
> tipicamente, è diverso dall'utente destinatario del messaggio (ossia
> l'amministratore della cartella in cui è stato inserito il file)

- **Numero articoli**: sostituito in fase di generazione del messaggio
  con il numero degli articoli in ordine (esclusi articoli di tipo
  spesa)

- **Sigla Documento**: sostituito in fase di generazione del messaggio
  con la sigla dell'Ordine

- **Stato Documento**: sostituito in fase di generazione del messaggio
  con lo stato dell'Ordine

- **Totale Ordine**: sostituito in fase di generazione del messaggio con
  il totale Ordine

- **Numero articoli carrello**: sostituito in fase di generazione del
  messaggio con il numero di articoli in carrello (esclusi articoli di
  tipo spesa)

- **Totale Carrello**: sostituito in fase di generazione del messaggio
  con il totale Carrello

- **Oggetto Messaggio:** sostituito in fase di generazione del messaggio
  con l'Oggetto del messaggio inserito in Area Riservata

- **Testo Messaggio:** sostituito in fase di generazione del messaggio
  con il Testo del messaggio inserito in Area Riservata

- **Data Attività:** sostituito in fase di generazione del messaggio con
  la data dell'Attività inserita in Area Riservata (valido solo per la
  tipologia di azione di "Notifica cambio stato attività")

- **Oggetto Attività:** sostituito in fase di generazione del messaggio
  con l'Oggetto dell'Attività inserita in Area Riservata

- **Nuovo Stato:** sostituito in fase di generazione del messaggio con
  il Nuovo Stato dell'Attività inserita in Area Riservata

- **Vecchio Stato:** sostituito in fase di generazione del messaggio con
  il Nuovo Stato dell'Attività inserita in Area Riservata

- **Nome Cartella:** sostituito in fase di generazione del messaggio con
  il Nome della cartella in Area Riservata in cui è contenuto il file
  che ha generato l'invio del messaggio stesso

- **Nome File:** sostituito in fase di generazione del messaggio con il
  Nome del file che ha generato l'invio del messaggio stesso

- **URL Sito**: sostituito in fase di generazione del messaggio con
  l'url del sito

**ATTENZIONE!** nel caso di siti in multilingua sarà necessario
impostare un Template per ciascuna delle lingue attualmente gestite.

In questo senso occorre anche sottolineare che i "Messaggi Ecommerce"
(es. Stato Ordine, Carrello Abbandonato, Messaggio di benvenuto ...)
verranno poi inviati nella lingua con cui l'utente stava visitando il
sito durante la sessione di navigazione in cui è stato generato l'evento
che ha prodotto l'invio del messaggio. I messaggi legati invece agli
eventi di "Area Riservata" (es. Notifica Messaggio, Notifica Documenti
...) verranno inviati nella lingua associata all'utente destinatario del
messaggio stesso.

