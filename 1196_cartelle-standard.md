# CARTELLE STANDARD



Come indicato nel precedente capitolo di questo manuale le "**Cartelle
Standard**" sono quelle identificate all'interno dell'albero dall'icona
colorata di giallo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_cartelle_standard.bmp](./assets/media/image69.png)

Tali cartelle:

- possono essere create da ogni utente

- consentono il caricamento e lo scambio di generici documenti tra gli
  utenti appartenenti alla gerarchia impostata sul sito

- è necessario associargli manualmente gli utenti abilitati ad accedervi
  ed i loro permessi di Lettura/Scrittura/Modifica.

- possono essere organizzate in una struttura gerarchia di cartelle e
  sotto cartelle operando però sempre e comunque all'interno di una
  gerarchia che ha come origine una cartella Standard. In altri termini
  dunque non è possibile inserire cartelle Standard all'interno di
  cartelle di tipo Azienda e/o di tipo Template

Considerando che ogni singolo documento dovrà, per forza di cose, essere
contenuto all'interno di una specifica cartella e che, come vedremo
meglio nei successivi capitoli di questo manuale le creazione di
cartelle di tipo Azienda e Template verrà gestita in automatico dall'
applicazione secondo determinate logiche al livello più alto della
struttura (**Documenti**) sarà possibile solamente creare delle nuove
cartelle all'interno delle quali andranno poi inseriti i vari documenti
piuttosto che eventualmente altre sottocartelle.

In queste condizioni dunque l'unico pulsante presente nella barra degli
strumenti sarà proprio quello per la creazione di nuove cartelle (
![Videate\\pulsante_ar_nuova_cartella.bmp](./assets/media/image70.png) )

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_documenti_2_passcomm.bmp](./assets/media/image71.png)

**ATTENZIONE!** ogni cartella creata attraverso la funzionalità **"Nuova
Cartella"** sarà di tipo **Standard**

Cliccando su questo pulsante verrà aperta la maschera di creazione della
nuova cartella

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_nuova_cartella_passcom.bmp](./assets/media/image72.png)

all'interno della quale poter indicare il nome (campo **"Nome"**) oltre
che gli utenti che dovranno avere accesso alla cartella stessa --
pulsante **Aggiungi Utente (**
![Videate\\ar_pulsante_inserisci_utente.bmp](./assets/media/image29.png) **)**

**ATTENZIONE!** nel caso in cui l'utente tentasse di creare una cartella
con lo stesso nome di una delle cartelle già presenti **allo stesso
livello**, verrà visualizzato un avviso con la richiesta di modificare
il nome della cartella.

Come per i messaggi, e sostanzialmente per ogni "entità" presente in
area riservata, anche in questo caso l'elenco dei possibili utenti cui
concedere accesso alla cartella che si sta realizzando può variare a
seconda dell' utente attualmente loggato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_nuova_cartella_utenti.bmp](./assets/media/image73.png)

Tra i possibili utenti di una cartella è possibile distinguere in:

- **Verde** i singoli utenti di tipo **AZIENDA**;

- **Azzurro** i singoli utenti di tipo **DIPENDENTE**;

- **Arancione** i singoli utenti di tipo **COMMERCIALISTA**;

- **Rosso** i vari gruppi utente (vedi anche sezione "Utenti --
  Gerarchie" di questo manuale);

**NOTA BENE**: per maggiori informazioni relativamente alle diverse
tipologie di utenti che possono avere accesso all'Area Riservata del
sito si veda anche la sezione "Utenti -- Utenti Area Riservata" di
questo manuale.

Nello specifico poi, per poter consentire ad un certo utente piuttosto
che ad un certo gruppo di utenti di accedere alla cartella che si sta
realizzando, e conseguentemente ai documenti in essa contenuti, è
sufficiente selezionarlo flaggando l'apposito check presente a fianco
del suo nome e, successivamente, cliccare sul pulsante di **Conferma**
presente nella parte bassa della maschera.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_documenti_inserimento_utenti.bmp](./assets/media/image74.png)

Per ciascuno degli utenti inseriti è poi possibile specificare se
l'accesso alla cartella dovrà avvenire in **modifica**, in **scrittura**
o in sola **lettura**.

Selezionando l'utente verrà infatti visualizzata un'ulteriore sezione
all'interno della quale poter specificare i permessi di
lettura/scrittura/modifica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_permessi_cartella.bmp](./assets/media/image75.png)

Queste le differenze tra le varie tipologie di permessi:

- **Lettura:** l'utente avrà unicamente la possibilità di visionare i
  documenti presenti all'interno della cartella in esame. Non avrà
  quindi la possibilità di variare le proprietà di questa cartella così
  come non avrà la possibilità di eliminare o spostare i documenti
  contenuti al suo interno. Allo stesso modo non avrà la possibilità di
  inserire nuovi documenti o di creare nuove sottocartelle.

> **Le cartelle con i permessi di sola lettura si distinguono dalle
> altre grazie alla presenza di un' icona al loro fianco raffigurante un
> piccolo lucchetto rosso**.
>
> **ATTENZIONE:** selezionando una cartella in sola lettura le uniche
> operazioni effettuabili in merito al suo contenuto saranno quelle
> mediante le quali poter scaricare i vari documenti (pulsante
> "**Scarica Documento**") o visualizzarne l'anteprima (pulsante
> "**Anteprima**")

- **Scrittura:** l'utente avrà la possibilità di visionare i documenti
  presenti all'interno della cartella in esame; avrà inoltre la
  possibilità di inserire, all'interno di questa cartella, nuovi file o
  di creare nuove sottocartelle, in relazione alle quali, in qualità di
  creatore, avrà sempre il completo controllo (potrà quindi eliminare o
  spostare file o cartelle da lui create oltre che modificarne le
  proprietà). Non avrà invece la possibilità di variare le proprietà
  delle cartelle già presenti all'interno della cartella in esame (e
  quindi non create da lui) ne, allo stesso modo, potrà eliminare queste
  cartelle o i documenti in esse contenuti.

> Nel caso in cui l'utente tenti di quindi eliminare un documento in
> relazione al quale non ha tale permesso verrà visualizzato un
> messaggio di errore e, ovviamente l'eliminazione non andrà a buon fine

- **Modifica:** l'utente avrà il pieno controllo della cartella in esame
  potendo quindi visionare i documenti presenti al suo interno,
  eliminarli, aggiungerne di nuovi o creare nuove sottocartelle, sulle
  quali, in qualità di creatore, avrà sempre il controllo completo
  (potrà quindi eliminare o spostare file o cartelle da lui create oltre
  che modificarne le proprietà).

> **ATTENZIONE!**: **I permessi di Modifica sono prioritari rispetto a
> quelli di Scrittura/Lettura**.

Una cosa di fondamentale importanza da tenere sempre in considerazione
relativamente ai permessi assegnati ad una cartella è che **tali
permessi non sono ereditari**. **In conseguenza di ciò è necessario
specificare i permessi desiderati per tutte le eventuali sottocartelle
della cartella padre.**

**NOTA BENE:** il creatore di una cartella, in qualità di proprietario,
avrà su di essa il pieno controllo (permessi di Modifica)

**ATTENZIONE!** **Consentendo l'accesso ad una cartella sia ad un gruppo
di utenti che singolarmente ad uno specifico utente dello stesso gruppo,
i permessi assegnati allo specifico utente sono prioritari rispetto a
quelli assegnati al gruppo**

Supponendo dunque di assegnare al gruppo il permesso di modifica e al
singolo utente il permesso di lettura, quest'ultimo avrà sulla specifica
cartella il permesso di Lettura.

La sezione **"Amministratore della Cartella"** presente nella maschera
di creazione Nuova Cartella permette di associare alla cartella in esame
uno specifico Amministratore selezionandolo tra gli utenti abilitati ad
accedere alla cartella stessa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_amministratore_cartella.bmp](./assets/media/image76.png)

Questo Amministratore potrà poi essere notificato, con una mail, con un
SMS, con un messaggio Telegram e/o con un messaggio Whatsapp
(dipendentemente dal **"Tipo di Notifica"** selezionato), ogni volta che
verrà inserito un documento all'interno della cartella in esame e ogni
volta che un documento presente all'interno di questa stessa cartella
verrà visionato (il tutto ovviamente a patto di aver specificato nei
propri dati personali un numero di cellulare e/o un indirizzo mail
valido).

**ATTENZIONE!** per maggiori informazioni in merito alla visibilità o
meno di questi check e alla gestione delle corrispondenti notifiche si
veda anche quanto indicato relativamente agli analoghi check presenti
nella sezione "Messaggi"

Considerando una struttura di cartelle costituita da una cartella
'Padre' e da varie 'Sottocartelle', assegnando un amministratore alla
cartella 'Padre', questo stesso amministratore verrà automaticamente
ereditato anche da tutte le eventuali 'Sottocartelle' della struttura.

In questo modo quindi, aggiungendo documenti all' interno delle varie
'Sottocartelle' potrà comunque essere notificato all'amministratore
della cartella 'Padre' l'inserimento del nuovo documento.

Volendo è inoltre possibile assegnare ad ogni Sottocartella un altro
amministratore oltre a quello ereditato in automatico dalla cartella
'Padre', e anche quest'ultimo verrà notificato tramite mail o SMS
all'inserimento di un nuovo documento.

**NOTA BENE:** non è possibile selezionare dei gruppi come
"Amministratore di Cartella".

Oltre alla notifica via mail / sms inviata all'amministratore della
cartella l'eventuale presenza di nuovi documenti verrà evidenziata, per
i relativi destinatari, anche all'interno dell'area riservata sia
mediante l'apposita icona delle notifiche

![Videate\\ar_menu_notifiche_dettaglio.bmp](./assets/media/image11.png)

sia in Bacheca all'interno dell'apposito box "**Documenti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_notifica_doc_docuvision_bacheca.bmp](./assets/media/image77.png)

**ATTENZIONE! all'interno del box Documenti verranno visualizzati tutti
i documenti che sono stati aggiunti in Docuvision piuttosto che
direttamente in area riservata all'interno di apposite cartelle
standard, successivamente all'ultimo accesso effettuato.**

Una volta visualizzato tale elenco, i documenti in esso presenti non
verranno più considerati come nuovi per cui effettuando un logout e
subito dopo un successivo login il box Documenti sarà, ovviamente, vuoto

Per quel che riguarda invece i collegamenti le azioni effettuabili sui
documenti presenti all'interno di questo box cliccando sul nome di un
documento caricato in docuvision, verrà avviato immediatamente il
download del documento stesso (per maggiori informazioni relativamente
alla gestione dei documenti Docuvision si veda anche quanto indicato nei
successivi capitoli di questo manuale)

Cliccando invece sul nome di un documento caricato all'interno di una
Cartella Standard l'utente verrà automaticamente ricondotto alla sezione
Documenti dell'area riservata dove troverà già aperta la cartella in cui
si trova il documento stesso (

Infine, un'ultima cosa interessante da sottolineare **è la possibilità
di creare in blocco un'intera struttura di cartelle e sottocartelle (con
eventuali file già presenti in esse) partendo da un archivio compresso
(file .zip) precedentemente creato.**

Per far questo è sufficiente cliccare sul pulsante **Scegli File** **(**
![Videate\\pulsante_scegli_file.bmp](./assets/media/image78.png) **)** presente, nella maschera di
creazione Nuova Cartella, a fianco dell'etichetta **"Zip con struttura
Cartelle"**

In questo modo sarà quindi possibile uplodare il file .zip desiderato
selezionandolo direttamente dalla propria macchina.

Durante il procedimento di scansione del file .zip e di creazione della
relativa struttura di cartelle verranno considerate le seguenti regole:

- La cartella padre, presente all'interno del file .zip, verrà creata
  con tutte le impostazioni (utenti e relativi permessi) settate nel
  form di creazione della nuova cartella, ad esclusione del campo nome
  che, anche se valorizzato, non verrà comunque considerato. Come nome
  delle cartelle verrà quindi utilizzato il nome presente per le
  cartelle stesse all'interno del file .zip

- Eventuali sotto cartelle presenti all'interno del file .zip
  erediteranno gli utenti e i permessi dalla cartella padre secondo le
  stesse regole e la stessa logica applicata nel momento in cui questo
  tipo di operazione (creazione di sottocartelle) dovesse essere
  effettuata in maniera manuale.

- Nel caso in cui sia già presente in Area Riservata, allo stesso
  livello, una cartella con lo stesso nome della cartella padre presente
  all'interno del file .zip, **ma questa cartella non risulti visibile
  all'utente che effettua l'upload dell'archivio compresso** **(perché
  non è stata a lui assegnata)**, a seguito del caricamento del file
  .zip verrà creata una nuova cartella padre, con lo stesso nome di
  quella già presente, seguito però da un numero progressivo (che
  servirà appunto per diversificare tra loro le due strutture di
  cartelle)

- Nel caso in cui sia già presente in Area Riservata, allo stesso
  livello, una cartella con lo stesso nome della cartella padre presente
  all'interno del file .zip, **e creata dallo stesso utente che effettua
  l'upload dell'archivio compresso**, a seguito del caricamento del file
  .zip non verrà creata nessuna nuova struttura di cartelle ma verrà
  semplicemente aggiornata la struttura preesistente secondo le nuove
  impostazioni settate in fase di upload.

- Nel caso in cui sia già presente in Area Riservata, allo stesso
  livello, una cartella con lo stesso nome della cartella padre presente
  all'interno del file .zip, **e questa stessa cartella risulti visibile
  con permessi di Modifica e/o Scrittura anche all'utente che effettua
  l'upload dell'archivio compresso** **(pur non essendo stata da lui
  stesso creata)**, a seguito del caricamento del file .zip la cartella
  preesistente non verrà sovrascritta mentre per eventuali sottocartelle
  le impostazioni relative all'amministratore e agli utenti saranno
  limitate agli utenti e ai gruppi associati alla cartella padre

Per quel che riguarda invece i singoli file eventualmente caricati
all'interno delle cartelle presenti nell'archivio compresso, in fase di
scansione del file .zip verrà considerata la seguente regola:

- Nel caso in cui il file non esista già all'interno della
  corrispondente cartella e nel caso in cui l'utente che effettua
  l'upload abbia i permessi di "Modifica" e/o "Scrittura" sulla cartella
  in cui dovrà essere inserito il file, il file stesso verrà
  correttamente caricato e salvato all'interno della cartella in esame.

- Nel caso in cui il file esista già all'interno della corrispondente
  cartella e nel caso in cui l'utente che effettua l'upload abbia i
  permessi di "Modifica" su questa stessa cartella, il file inizialmente
  presente verrà sovrascritto e sostituito da quello nuovo.

- Nel caso in cui l'utente abbia, sulla cartella in cui dovrebbe essere
  inserito il nuovo file i soli permessi di Lettura, anche a seguito del
  upload del file .zip all'interno di questa cartella non verrà inserito
  alcun file.

Nel momento in cui si dovesse selezionare una cartella, tra quelle
presenti all'interno dell'albero di navigazione, in relazione alla quale
si hanno i permessi di Modifica, nella barra degli strumenti
compariranno, oltre al pulsante "Nuova Cartella" anche altri pulsanti
identificativi di diverse azioni da poter effettuare sulla cartella in
esame.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_documenti_toolbar_cartelle_passcom.bmp](./assets/media/image79.png)

**ATTENZIONE!** i pulsanti presenti nella barra degli strumenti possono
variare in relazione alle proprietà e conseguentemente ai permessi che
l'utente attualmente loggato ha sulla cartella selezionata.

In particolare il pulsante:

**Nuova Cartella** (
![Videate\\pulsante_ar_nuova_cartella.bmp](./assets/media/image70.png) ): consente di creare, attraverso la
maschera di creazione cartella precedentemente analizzata, nuove
cartelle all'interno di quella attualmente selezionata. Richiede i
permessi di **Modifica** e/o di **Scrittura** sulla cartella
selezionata.

**ATTENZIONE:** in queste condizioni gli utenti di eventuali
sottocartelle potranno essere selezionati solamente tra tutti i
possibili utenti della cartella padre.

Nel caso in cui dunque dovesse essere necessario aggiungere un certo
utente ad una sottocartella, sarà necessario per prima cosa aggiungere
questo stesso utente alla relativa cartella padre.

**Elimina (Cartella)** (
![Videate\\ar_pulsante_elimina_cartella.bmp](./assets/media/image80.png) ): consente di eliminare la cartella attualmente
selezionata.

**ATTENZIONE! Questo tipo di operazione può essere fatta unicamente dal
creatore della cartella.**

Cliccando su questo pulsante verrà visualizzata un apposito messaggio
per chiedere all'utente se desidera eliminare solamente la cartella
selezionata oppure anche eventuali sotto cartelle:

![Videate\\elimina_cartella_selezione.bmp](./assets/media/image81.png)

Nel caso in cui si decida di eliminare anche le sottocartelle verranno
comunque eliminate solo ed esclusivamente quelle sottocartelle create
dall'utente attualmente connesso (solo quelle, cioè, per le quali è
abilitato il pulsante di Elimina).

**Ovviamente eventuali sottocartelle che non potranno essere eliminate
saliranno di un livello nella struttura gerarchica attualmente gestita
all'interno del sito.**

> **NOTA BENE:** in ogni caso eliminando delle cartelle verranno
> eliminati anche eventuali documenti in esse contenuti.

**Proprietà** (
![Videate\\area_riservata_documenti_proprietà_cartella.bmp](./assets/media/image82.png) ): consente di variare le proprietà
della cartella selezionata. Questa operazione può essere fatta
unicamente dal creatore della cartella. Cliccando su questo pulsante
verrà aperta la stessa maschera di creazione cartella precedentemente
analizzata, attraverso la quale poter quindi variare il nome della
cartella, gli utenti abilitati ad accedervi o i loro permessi, l'utente
Amministratore della cartella e la tipologia di notifica.

**Sposta Cartella** (
![Videate\\area_riservata_documenti_sposta_cartella.bmp](./assets/media/image83.png) ): consente di attivare la modalità di
spostamento di una cartella.

Per effettuare questa operazione sarà quindi necessario:

- Selezionare la cartella che si desidera spostare tra quelle presenti
  in elenco

- Cliccare sul pulsante "Sposta Cartella".

> In questo modo il cursore del mouse assumerà la forma di 4 piccole
> frecce come evidenziato nella figura di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_spostamento_cartella.bmp](./assets/media/image84.png)

- Selezionare, a questo punto, la cartella di destinazione ossia quella
  dentro cui dovrà essere effettivamente spostata la cartella
  inizialmente selezionata.

> In questo modo verrà visualizzata una maschera di conferma
> dell'operazione con indicato il tipo di spostamento che si sta
> effettuando

![Videate\\conferma_spostamento_cartella.bmp](./assets/media/image85.png)

- Cliccando sul pulsante "Conferma" la cartella sorgente verrà spostata
  dentro la destinazione

**ATTENZIONE**! **Questa operazione può essere fatta unicamente dal
creatore della cartella**. Inoltre la cartella di destinazione deve
necessariamente avere, per l'utente che effettua lo spostamento, i
permessi di Scrittura o di Modifica.

Nel momento in cui la cartella di destinazione non dovesse avere uno dei
due permessi sopra indicati verrà visualizzato un apposito messaggio di
avviso e lo spostamento, ovviamente, non potrà terminare in maniera
corretta.

