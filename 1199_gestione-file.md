# GESTIONE FILE



Come evidenziato nei precedenti capitoli di questo manuale nella parte
destra della maschera di gestione dei documenti possono essere elencati:

- tutti i file presenti nella cartella attualmente selezionata
  all'interno dell'albero presente nella parte sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_gestione_file_1.bmp](./assets/media/image90.png)

- tutti i file risultanti da una ricerca effettuata mediante il pannello
  "**Ricerca Documenti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_gestione_file_2.bmp](./assets/media/image91.png)

Per ogni documento presente in griglia vengono indicate le seguenti
informazioni:

![Videate\\comm_colonne_griglia_documenti.bmp](./assets/media/image92.png)

- **Nome**: nome del file (con relativa estensione)

- **Data**: data di pubblicazione del file. In particolare:

  - Per i file caricati direttamente da area riservata viene indicata la
    data di upload del file

  - Per i documenti docuvision viene indicata la data di inserimento del
    file, sul gestionale, nella corrispondente Classe Docuvision

- **Dimensione**: dimensione del file (**solo per file caricati
  direttamente da area riservata**)

- **Classe**: classe Docuvision cui è stato associato il file

- **Tipo**: tipologia del documento Docuvision cui è stato associato il
  file

- **Cartella**: cartella di appartenenza del file. In particolare:

  - per i file docuvision verrà visualizzata l'icona
    ![Videate\\icona_docuvision_ricerca_documenti.bmp](./assets/media/image93.png)

  - per i file caricati direttamente da area riservata verrà invece
    visualizzata l'icona
    ![Videate\\icona_cartella_ricerca_documenti.bmp](./assets/media/image94.png)

> In questo caso inoltre cliccando su quest' icona verrà automaticamente
> selezionata e aperta anche la cartella di appartenenza del relativo
> file

I pulsanti presenti nella barra degli strumenti posta immediatamente al
di sopra dell'elenco dei documenti consentono rispettivamente di:

**Carica** (
![Videate\\area_riservata_documenti_carica_documento.bmp](./assets/media/image95.png) ): consente di uplodare nuovi documenti all'interno
della cartella attualmente selezionata

**ATTENZIONE! per poter uplodare un nuovo file all'interno di una
determinata cartella è necessario avere su di essa i permessi di
Scrittura / Modifica oppure essere il suo creatore**

In conseguenza di ciò nel momento in cui la cartella selezionata
all'interno dell'albero dovesse essere **una cartella in sola Lettura**
oppure **una cartella Docuvision** (in entrambi i casi la cartella in
esame sarà marcata dalla presenza di un piccolo lucchetto rosso a fianco
del nome) **il pulsante "Carica" non verrà visualizzato**

**ATTENZIONE!** volendo sarebbe possibile caricare nuovi documenti anche
all'interno di Cartelle di tipo Template. Sulla base di quanto indicato
nei precedenti capitoli di questo manuale però questa operazione sarebbe
di fatto priva di significato

Una volta verificata la possibilità di uploadare nuovi file all'interno
della cartella selezionata cliccando sul pulsante in esame verrà
visualizzata la maschera "**Carica Documento**"

![Videate\\area_riservata_documenti_carica_file2_passcomm.bmp](./assets/media/image96.png)

Per completare l'upload del nuovo documento sarà quindi necessario:

- cliccare sul pulsante **"File" (**
  ![Videate\\pulsante_scegli_file.bmp](./assets/media/image78.png) **)**

- selezionare il file desiderato tra quelli presenti all'interno del
  proprio PC

- assegnargli un nome (campo **Nome**)

- cliccare infine sul pulsante **"Upload File" (**
  ![Videate\\pulsante_upload_file.bmp](./assets/media/image97.png) **)** presente nella parte bassa della
  maschera.

**ATTENZIONE! L'upload di nuovi file all'interno di una cartella può
essere effettuata anche con operazioni di Drag and Drop**

In questo senso, una volta selezionata, in area riservata, la cartella
all'interno della quale effettuare l'upload si potrebbe anche trascinare
il file da uplodare direttamente sull'elenco dei documenti presenti
nella cartella (nella colonna di destra della pagina). In questo modo
infatti verrà aperta automaticamente la maschera di "Upload File" sopra
evidenziata.

Rilasciando quindi il file all'interno della maschera **"Carica
Documento"** verrà compilato in automatico il campo file con il percorso
della risorsa da caricare. Sarà quindi possibile associare un nome al
file e confermare il caricamento con il relativo pulsante di Conferma.

**ATTENZIONE!** L'area di drop all'interno della quale rilasciare il
file da caricare è quella individuata dalla maschera **"Carica
Documento". Nel caso in cui il file dovesse essere rilasciato in una
posizione diversa anziché effettuare l'upload verrà aperto il file
all'interno del browser**

Nel caso in cui non venga specificato un nome per il file che si sta
caricando verrà utilizzato come nome della risorsa il nome del file
stesso.

**NOTA BENE:** nel caso in cui l'utente tentasse di inserire all'interno
della cartella un file con lo stesso nome di uno già presente, verrà
visualizzato un messaggio che chiede se il nuovo file dovrà
sovrascrivere il vecchio o se, invece, dovrà essere aggiunto come nuovo
file. In questo caso il nome del file verrà modificato in maniera
automatica aggiungendo un numeratore progressivo prima dell'estensione
del file stesso.

Infine, oltre al caricamento di un singolo File, volendo, è anche
possibile **caricare in blocco un'intera struttura di cartelle e
sottocartelle (con eventuali file già presenti in esse) partendo da un
archivio compresso (file .zip) precedentemente creato.**

Per far questo sarà sufficiente flaggare, prima dell'upload, il
parametro **"Archivio"** evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carica_zip_passcom.bmp](./assets/media/image98.png)

Attivando questo parametro l'applicazione saprà di dover trattare, in
fase di upload, un archivio compresso e si preoccuperà quindi di
valutare quanto presente all'interno del file .zip, di decomprimerlo, di
caricare in blocco i file presenti all'interno delle varie cartelle e di
creare se necessario eventuali nuove sottocartelle.

In particolare durante il procedimento di scansione del file .zip e di
creazione di eventuali nuove sottocartelle, verranno considerate le
seguenti regole:

- Nel caso in cui non sia già presente, allo stesso livello, una
  cartella con lo stesso nome di quella presente all'interno del file
  .zip, verrà creata una nuova cartella utilizzando per questo tutte le
  impostazioni della sua cartella padre

- Nel caso in cui sia già presente, allo stesso livello, una cartella
  con lo stesso nome di quella presente all'interno del file .zip, **ma
  questa cartella non risulti visibile all'utente che effettua l'upload
  dell'archivio compresso** **(perché non è stata a lui assegnata)**, a
  seguito del caricamento del file .zip verrà creata una nuova cartella,
  con lo stesso nome di quella già presente, seguito però da un numero
  progressivo (che servirà appunto per diversificare tra loro le due
  strutture di cartelle). Anche in questo caso verranno comunque
  utilizzate tutte le impostazioni della cartella padre.

- Nel caso in cui sia già presente, allo stesso livello, una cartella
  con lo stesso nome di quella presente all'interno del file .zip, **e
  questa cartella risulti visibile con permessi di Modifica o Scrittura
  anche all'utente che effettua l'upload dell'archivio compresso,** a
  seguito del caricamento del file .zip non verranno toccate le
  impostazioni delle cartelle preesistenti ma verranno semplicemente
  caricati al loro interno eventuali nuovi documenti presenti nel file
  .zip.

Per quel che riguarda invece i singoli file presenti all'interno
dell'archivio compresso, in fase di scansione del file .zip verrà
considerata la seguente regola:

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

**Elimina Documento** (
![Videate\\ar_pulsante_elimina_documento.bmp](./assets/media/image99.png) ): consente di eliminare il documento
attualmente selezionato.

**ATTENZIONE! l'eliminazione di un documento richiede che sia stata
selezionata una determinata cartella, che il file da eliminare non sia
stato caricato in Docuvision e che l'utente loggato abbia i permessi di
Modifica o di Scrittura sulla cartella in cui risiede il file**.

In particolare poi nel momento in cui l'utente loggato dovesse avere,
sulla cartella in esame i permessi di:

- **Modifica**: potrà eliminare un qualsiasi file presente all'interno
  della cartella

- **Scrittura**, potrà eliminare unicamente i file da lui stesso
  caricati.

> In queste condizioni una volta selezionato un file il pulsante
> "Elimina" verrà sempre visualizzato tra quelli presenti nella barra
> degli strumenti, ma tentando di eliminare un documento non caricato
> direttamente da lui, verrà visualizzato un apposito messaggio di
> avviso e il relativo file, ovviamente, non verrà eliminato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\eliminazione_file_permessi_scrittura.bmp](./assets/media/image100.png)

- **Lettura**: non potrà eliminare nessuno dei file presenti all'interno
  della cartella. In queste condizioni dunque il pulsante "Elimina" non
  verrà neppure visualizzato

In sostanza questo tipo di operazione potrà essere effettuata solo al
verificarsi di determinate condizioni. Nello specifico:

- Se è stata selezionata una determinata cartella all'interno del
  corrispondente albero

- Se la cartella selezionata non è una cartella "Docuvision" (i file
  gestiti all'interno del gestionale possono essere eliminati unicamente
  operando all'interno del gestionale stesso)

- Se l'utente ha, sulla cartella selezionata, il permesso di Scrittura

- Se l'utente ha, sulla cartella selezionata, il permesso di Modifica e
  il file da eliminare è un file da lui stesso caricato

In conseguenza di ciò nel momento in cui l'esigenza dovesse essere
quella di eliminare uno dei file ottenuti da una ricerca effettuata
mediante il pannello di "Ricerca Documenti", sarà necessario, per prima
cosa, accertarsi che il file in questione non sia contenuto all'interno
di una cartella Docuvision e che abbia quindi, in corrispondenza della
colonna "Cartella", l'icona
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_cartella_ricerca_documenti.bmp](./assets/media/image101.png) . Cliccando su questa stessa icona verrà
selezionata automaticamente la cartella in cui si trova il file e, a
questo punto, se tale cartella ha effettivamente il permesso di
Scrittura o quello di Modifica e il file selezionato era stato
precedentemente caricato dallo stesso utente, comparirà il pulsante
"Elimina" e il file potrà quindi essere cancellato

**Svuota** (
![Videate\\area_riservata_documenti_svuota.bmp](./assets/media/image102.png) ): consente di eliminare in blocco tutti
i documenti presenti all'interno della cartella selezionata

**ATTENZIONE! come per il pulsante "Elimina" anche il pulsante "Svuota"
richiede che sia stata selezionata una determinata cartella e che
l'utente attualmente loggato abbia su di essa i permessi di Modifica o
di Scrittura**

In particolare dunque nel momento in cui l'utente loggato dovesse avere,
sulla cartella in esame i permessi di:

- **Modifica**: cliccando sul pulsante "Svuota" verranno eliminati tutti
  i file presenti all'interno della cartella

- **Scrittura**: cliccando sul pulsante "Svuota" verranno eliminati
  dalla cartella i soli file inseriti dall'utente attualmente loggato

> In queste condizioni, inoltre, verrà visualizzato anche un apposito
> messaggio per informare l'utente che, sui file elencati, non ha i
> permessi per effettuare l'operazione richiesta

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\svuota_cartella_permessi_scrittura.bmp](./assets/media/image103.png)

- **Lettura**: in queste condizioni l'utente non può eliminare nessuno
  dei file presenti all'interno della cartella e quindi il pulsante
  "Svuota" non verrà neppure visualizzato

In sostanza questo tipo di operazione potrà essere effettuata solo al
verificarsi di determinate condizioni. Nello specifico:

- Se è stata selezionata una determinata cartella all'interno del
  corrispondente albero

- Se la cartella selezionata non è una cartella "Docuvision" (i file
  gestiti all'interno del gestionale possono essere eliminati unicamente
  operando all'interno del gestionale stesso)

- Se l'utente ha, sulla cartella selezionata, il permesso di Scrittura

- Se l'utente ha, sulla cartella selezionata, il permesso di Modifica.
  In questo caso verranno comunque eliminati dalla cartella i soli
  documenti caricati dallo stesso utente attualmente loggato

**ATTENZIONE!** ovviamente, a seguito di una ricerca effettuata mediante
il pannello di "Ricerca Documenti" il pulsante "Svuota" non verrà mai
visualizzato

**Sposta File** (
![Videate\\area_riservata_documenti_sposta_file.bmp](./assets/media/image104.png) ): consente di spostare il documento
attualmente selezionato all'interno di un'altra cartella della
struttura.

**ATTENZIONE! lo spostamento di un file richiede che sia stata
selezionata, all'interno del corrispondente albero, la cartella di
origine, che l'utente loggato abbia su tale cartella i permessi di
Scrittura o di Modifica, che il file da spostare non sia stato caricato
in Docuvision e che l'utente loggato abbia i permessi di Modifica o di
Scrittura anche sulla cartella di destinazione**

In particolare nel momento in cui l'utente loggato dovesse avere, sulla
cartella di origine i permessi di:

- **Modifica:** potrà spostare tutti i file presenti all'interno della
  cartella

- **Scrittura**: potrà spostare solamente i file presenti all'interno
  della cartella che sono stati da lui stesso caricati.

> In queste condizioni dunque, tentando di spostare un file che non è
> stato caricato dallo stesso utente attualmente loggato, verrà
> visualizzato un apposito messaggio di avviso e lo spostamento non
> verrà eseguito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sposta_file_permessi_scrittura.bmp](./assets/media/image105.png)

- **Lettura**: non potrà spostare nessuno dei file presenti all'interno
  della cartella. In questo caso dunque il pulsante "Sposta File" non
  verrà proprio visualizzato

In sostanza questo tipo di operazione potrà essere effettuata solo al
verificarsi di determinate condizioni. Nello specifico:

- Se è stata selezionata all'interno del corrispondente albero la
  cartella di origine in cui si trova il file da spostare

- Se la cartella di origine selezionata non è una cartella "Docuvision"
  (i file gestiti all'interno del gestionale non possono essere spostati
  in cartelle diverse da quella a cui appartengono)

- Se l'utente ha, sulla cartella di origine, il permesso di Scrittura

- Se l'utente ha, sulla cartella di origine, il permesso di Modifica e
  il file da spostare è effettivamente un file da lui stesso
  precedentemente caricato.

Per quel che riguarda invece **la cartella di destinazione, affinché lo
spostamento possa essere eseguito in maniera corretta, l'utente dovrà
avere anche su di essa i permessi di Modifica o di Scrittura**

Nel caso in cui i permessi sulla cartella di destinazione dovessero
essere di sola Lettura, tentando di effettuare lo spostamento verrà
visualizzato un apposito messaggio di avviso e l'operazione non verrà
eseguita.

Nello specifico poi per spostare un file all'interno di un'altra
cartella sarà necessario:

- Selezionare il file che si desidera spostare

- Cliccare sul pulsante "**Sposta File**" per attivare la modalità di
  spostamento

- A questo punto spostandosi col mouse sulla sezione di sinistra della
  pagina per selezionare la cartella di destinazione, il puntatore del
  mouse si modificherà assumendo la forma di quattro piccole frecce.

- Selezionare quindi la cartella di destinazione e cliccare su di essa
  per effettuare lo spostamento

- Come per lo spostamento di un intera cartella anche in questo caso
  verrà richiesta un' ultima conferma prima di poter effettuare lo
  spostamento indicato

![Videate\\conferma_sposta_file.bmp](./assets/media/image106.png)

**ATTENZIONE!** come per i pulsanti "Elimina" e "Svuota" anche il
pulsante "Sposta file", considerando quanto detto, non verrà mai
visualizzato nel momento in cui si dovesse selezionare un file risultato
di una ricerca effettuata mediante il pannello di "Ricerca Documenti"

**Scarica** (
![Videate\\area_riservata_documenti_scarica_documento.bmp](./assets/media/image107.png) ): consente di effettuare il download
del documento attualmente selezionato.

Il download di un documento presente all'interno di una determinata
cartella è, ovviamente, un'opzione sempre attiva.

Il pulsante in esame sarà quindi sempre visibile indipendentemente dai
permessi che l'utente loggato ha sulla cartella selezionata e dal fatto
che tale cartella sia o meno una Cartella Docuvision.

**Anteprima** (
![Videate\\area_riservata_documenti_anteprima_documento.bmp](./assets/media/image108.png) ): consente di visualizzare un'anteprima
del documento attualmente selezionato senza doverlo necessariamente
scaricare.

Come per il download, anche l'anteprima di un documento presente
all'interno di una determinata cartella è un'opzione sempre attiva.

Anche questo pulsante sarà quindi sempre visibile indipendentemente dai
permessi che l'utente loggato ha sulla cartella selezionata e dal fatto
che tale cartella sia o meno una Cartella Docuvision

Il fatto però di poter effettivamente visualizzare l'anteprima del
documento all'interno del browser dipende dal browser stesso e dalla
specifica tipologia di file considerato.

In ogni caso nel momento in cui il browser non possa effettuare
l'anteprima del documento selezionato verrà avviato, automaticamente, il
suo download

Infine, per quanto riguarda la visualizzazione di questa sezione
dell'area riservata nei dispositivi mobile a default verrà visualizzata
solo la colonna contenente la struttura delle cartelle gestite.

In queste condizioni per visualizzare i file presenti all'interno di una
specifica cartella sarà quindi necessario selezionarla e cliccare poi
sul pulsante "**Elenco Documenti**" (
![Videate\\pulsante_elenco_documenti_mobile.bmp](./assets/media/image57.png) )

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_documenti_mobile.bmp](./assets/media/image58.png)

In questo modo verrà visualizzata la griglia dei documenti attualmente
presenti all'interno della cartella in esame. Dopo aver selezionato uno
dei documenti presenti in elenco il pulsante raffigurante tre piccoli
puntini consentirà di accedere al menu delle azioni effettuabili sul
file selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\documenti_comm_azioni_file_mobile.bmp](./assets/media/image60.png)

