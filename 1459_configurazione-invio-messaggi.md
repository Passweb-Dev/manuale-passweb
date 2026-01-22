# CONFIGURAZIONE INVIO MESSAGGI



La sezione "**Configurazione Invio Messaggi**" visibile all'interno
della maschera "**Dati Account**" solo dopo aver impostato e salvato i
parametri di Configurazione, consente di definire gli eventi in
relazione ai quali dovranno essere inviati dei messaggi Whatsapp e di
impostare anche il Template che dovrà essere utilizzato per l'invio di
questi stessi messaggi.

![](./assets/media/image7.png)

La griglia presente sul lato sinistro della sezione "**Template
Messaggi**" consente di visualizzare quelli che sono gli eventi già
configurati e in relazione ai quali verranno già inviati messaggi
Whatsapp utilizzando appositi Template.

I pulsanti presenti nella contestuale barra degli strumenti, consentono
rispettivamente di:

**Elimina** (
![](./assets/media/image8.png) ): consente di eliminare l'evento attualmente
selezionato in elenco

**Modifica** (
![](./assets/media/image9.png) ): consente di modificare l'evento
attualmente selezionato in elenco.

**Aggiungi** (
![](./assets/media/image10.png) ): consente di codificare un nuovo
evento ed il relativo messaggio Whatsapp

Cliccando su questo pulsante, verrà infatti visualizzata, sulla destra
della pagina la sezione "**Nuovo Template**"

![](./assets/media/image11.png)

all'interno della quale poter definire l'evento in relazione al quale
dovrà essere inviato un messaggio Whatsapp e il Template da utilizzare
per questo stesso messaggio

Nello specifico dunque il parametro:

**Nome dell'azione**: consente di assegnare un nome all'evento che si
sta configurando in modo tale da poterlo poi individuare facilmente tra
tutti gli eventi già presenti in elenco

**Tipologia dell'azione**: consente di indicare, selezionandola da un
apposito menù a tendina, l'azione e quindi lo specifico evento in
relazione al quale dovrà essere inviato un messaggio Whatsapp

È possibile selezionare uno dei seguenti valori:

- **Notifica Stato Ordine:** selezionando questa opzione l'evento che
  scatenerà l'invio del messaggio Whatsapp, sarà il passaggio
  dell'ordine in uno degli stati indicati in corrispondenza del
  successivo parametro "**Stati Ordine Gestiti**".

> Il destinatario della notifica sarà invece l'intestatario dello
> specifico ordine.
>
> Nel caso in cui l'esigenza dovesse essere, ad esempio, quella di
> inviare un messaggio Whatsapp agli utenti del sito nel momento in cui
> il loro ordine dovesse essere nello stato di Confermato, sarà quindi
> sufficiente selezionare questo stato dal box di sinistra ed inserirlo
> in quello di destra cliccando sull'icona raffigurante una piccola
> freccia verde

![](./assets/media/image12.png)

> Volendo è possibile selezionare anche più di uno stato
> contemporaneamente, in questo caso però il messaggio potrà variare
> solamente in relazione alle variabili dinamiche inserite nel Template
> utilizzato per l'invio.

- **Notifica carrello abbandonato:** in queste condizioni l'evento che
  scatenerà l'invio del messaggio Whatsapp sarà la creazione di un
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

- **Notifica invio messaggio**: l'evento che scatenerà la notifica
  Whatsapp sarà l'invio di un nuovo messaggio in Area Riservata.

> Il destinatario della notifica sarà invece il destinatario del
> messaggio stesso.

- **Notifica lettura messaggio**: l'evento che scatenerà la notifica
  Whatsapp sarà la lettura, da parte del destinatario, di un messaggio
  inviatogli in Area Riservata

> Il destinatario della notifica sarà invece il mittente del messaggio

- **Notifica cambio stato attività**: l'evento che scatenerà la notifica
  Whatsapp ad un determinato utente sarà il cambio di stato di una delle
  attività ad esso assegnate in Area Riservata.

> Il destinatario della notifica sarà invece il creatore dell'attività

- **Notifica presa visione attività**: l'evento che scatenerà la
  notifica Whatsapp sarà la presa visione, da parte del relativo
  destinatario, di un'attività ad esso assegnata

> Il destinatario della notifica sarà invece il creatore dell'attività

- **Promemoria attività**: l'evento che scatenerà la notifica Whatsapp
  sarà la scadenza di un Promemoria assegnato ad una delle attività
  presenti in Area Riservata (sezione "Agenda")

> Il destinatario della notifica sarà invece l'utente che ha inserito,
> per la sua attività, uno specifico promemoria

- **Notifica Upload File**: l'evento che scatenerà la notifica Whatsapp
  sarà l'upload di un file nella sezione "Documenti" di Area Riservata
  (per i siti commercialista sono considerati sia gli Upload manuali che
  gli Upload in Docuvision a patto però di gestire correttamente le Web
  Api di Passcom)

> Il destinatario del messaggio sarà invece l'amministratore associato
> alla cartella in cui viene caricato il file

- **Notifica Download File**: l'evento che scatenerà la notifica
  Whatsapp sarà il download (pulsante "Scarica") di un nuovo file
  precedentemente caricato nella sezione Documenti dell'Area Riservata

> Il destinatario sarà invece l'amministratore associato alla cartella
> in cui si trova il file

- **Notifica presa visione File**: l'evento che scatenerà la notifica
  Whatsapp sarà la presa visione (pulsante "Anteprima") di un file
  precedentemente caricato nella sezione Documenti dell'Area Riservata

> Il destinatario sarà invece l'amministratore associato alla cartella
> in cui si trova il file

**ATTENZIONE!** in relazione alle notifiche relative agli eventi di Area
Riservata, **il consiglio è quello di verificare che i Template
utilizzati siano stati effettivamente assegnati, all'interno di WA Smart
Business, alla categoria "Utility".** In questo modo infatti, oltre ad
avere un costo più basso, tali notifiche potranno essere inviate ai
relativi destinatari indipendentemente dal fatto che questi abbiano o
meno prestato il consenso marketing

Va detto anche che, a differenza dei messaggi relativi agli Stati Ordine
e/o ai Carrello Abbandonati, messaggi questi inviati in automatico
dall'applicazione al verificarsi del relativo evento, le notifiche
legate agli eventi di Area Riservata (es. Notifica Invio Messaggio)
verranno inviate invece solo nel momento in cui l'utente decida
effettivamente di voler inviare anche questo tipo di notifica (oltre ad
esempio alla notifica mail o SMS) selezionando per questo l'apposito
check

![](./assets/media/image13.png)

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

![](./assets/media/image14.png)

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
appartenere al gruppo indicato, l'utente dovrà anche non aver esercitato
la corrispondente opzione di opt out e, a seconda della categoria
assegnata da Meta al template utilizzato per l'invio del messaggio,
potrebbe anche dover avuto acconsentire alla ricezione delle
comunicazioni marketing.

**Template**: consente di indicare, selezionandolo dal corrispondente
menu a tendina, il Template da utilizzare per l'invio del messaggio.

**ATTENZIONE!** è possibile selezionare solamente i Template creati su
WA Smart Business che sono stati correttamente approvati da Meta e che
possono quindi essere effettivamente utilizzati per l'invio di un
messaggio

![](./assets/media/image15.png)

**ATTENZIONE!** per maggiori informazioni relativamente a come creare un
Template all'interno di WA Smart Business e su come mandarlo in
approvazione a Meta si consiglia di fare riferimento alla relativa
documentazione di prodotto

**Testo del Template**: consente di visualizzare il corpo del messaggio
definito (su WA Smart Business) per il Template indicato in
corrispondenza del precedente parametro.

![](./assets/media/image16.png)

**ATTENZIONE!** il campo in esame è in sola visualizzazione

Nel momento in cui l'esigenza dovesse essere quella di modificare il
testo del messaggio sarà dunque necessario agire direttamente su WA
Smart Business andando a modificare il relativo Template

La sezione "**Variabili Template**" consente invece di mappare eventuali
segnaposto individuati nel corpo del messaggio (e indicati dai simboli
{{1}}, {{2}} ...) con determinate informazioni (es. Nome Utente, Stato
dell'ordine, Totale dell'ordine ...) selezionabili dal corrispondente
menu a tendina.

![](./assets/media/image17.png)

**ATTENZIONE!** è possibile gestire Template di messaggio con un massimo
di 5 variabili dinamiche

In particolare, in relazione alla diversa tipologia di evento indicata
sarà possibile utilizzare uno dei seguenti segnaposto:

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

- **URL Sito**: sostituito in fase di generazione del messaggio con:

  - **l'url di visualizzazione del carrello abbandonato** nel caso in
    cui la tipologia di azione selezionata sia "Notifica Carrello
    Abbandonato"

  - **l'url di visualizzazione del dettaglio ordine** nel caso in cui la
    tipologia di azione selezionata sia "Notifica Stato Ordine"

  - **l'url del sito** nel caso in cui la tipologia di azione
    selezionata sia relativa ad una delle notifiche di Area Riservata

Per maggiori informazioni relativamente a come poter inserire su WA
Smart Business variabili dinamiche all'interno di un Template di
messaggio si consiglia di fare riferimento alla relativa documentazione
di prodotto.

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

