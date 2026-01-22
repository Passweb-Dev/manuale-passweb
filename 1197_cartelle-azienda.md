# CARTELLE AZIENDA



Le "**Cartelle Azienda**" sono quelle identificate all'interno
dell'albero dall'icona colorata di rosso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_cartelle_azienda.bmp](./assets/media/image86.png){width="5.311805555555556in"
height="3.3506944444444446in"}

e a differenza di quelle Standard, che possono essere liberamente create
da ogni utente abilitato ad accedere in area riservata, le cartelle di
tipo Azienda verranno generate in automatico dall'applicazione:

- sulla base degli utenti di tipo AZIENDA (Passcom e non)

- a seguito della creazione di cartelle di tipo Template.

Nello specifico per quel che riguarda le cartelle di tipo Azienda
relative ad utenti Passcom corrispondenti ad Aziende dell'installazione
esportate e gestite all'interno del sito, Passweb verificherà, ad ogni
sincronizzazione la presenza di eventuali nuovi utenti Passcom di questo
tipo correttamente abilitati ad accedere al sito e con la gestione
Docuvision attiva e, nel caso, crea automaticamente la relativa Cartella
Azienda.

Per quel che riguarda invece le cartelle di tipo Azienda relative ad
utenti creati manualmente all'interno del Wizard di Passweb, sarà
Passweb stesso, una volta creato l'utente a preoccuparsi di generare e
creare anche la relativa cartella Azienda.

Infine nel momento in cui dovessero essere create cartelle di tipo
Template, Passweb si preoccuperà di verificare la presenza di utenti di
tipo AZIENDA (Passcom e non) abilitati ad accedere al sito e, nel caso,
andrà a creare automaticamente le relative cartelle di tipo Azienda.

Per maggiori informazioni in merito a come le cartelle di tipo Template
vanno ad impattare sulla creazione e/o sull'eliminazione di cartelle di
tipo Azienda si veda anche quanto indicato nel successivo capitolo di
questo manuale.

**ATTENZIONE: in ogni caso comunque, non sarà mai possibile creare o
eliminare manualmente questo tipo di cartelle.**

Per quel che riguarda invece gli utenti abilitati ad accedere a queste
cartelle e a gestire eventuali documenti in esse contenuti, a differenza
di quanto avveniva per le cartelle Standard a cui potevano essere
associati più utenti e per ciascuno di essi era possibile definire i
relativi permessi di Lettura / Modifica / Scrittura, **ogni cartella di
tipo Azienda ha invece un solo utente associato corrispondente,
ovviamente, alla relativa AZIENDA.**

**ATTENZIONE!** non è possibile associare a questa tipologia di cartelle
utenti differenti da quello associatogli in automatico
dall'applicazione.

Nel momento in cui l'utente in esame dovesse poi essere inserito
all'interno di una determinata gerarchia di gruppi utente la sua
cartella, o meglio, i documenti presenti all'interno di questa cartella
e di sue eventuali sotto cartelle potranno, ovviamente, essere
visualizzati e gestiti non solo da lui ma anche da tutti gli utenti
collocati ad un livello gerarchico superiore al suo

Infine per quel che riguarda i documenti presenti all'interno di queste
cartelle il discorso cambia a seconda del fatto che la cartella in esame
sia relativa ad un utente di tipo Azienda creato manualmente dal back
end di Passweb, oppure ad un utente Azienda esportato direttamente dal
gestionale.

Nel primo caso infatti, gli utenti abilitati a gestire la cartella
corrispondente all'utente di tipo Azienda creato dal back end di
Passweb, avranno la possibilità di caricare nuovi documenti all'interno
di questa stessa cartella e di visualizzare e/o eliminare quelli già
presenti, operando, in questo senso, esattamente allo stesso modo di
quanto avviene per le cartelle Standard

Nel secondo caso invece, eventuali documenti presenti all'interno di
cartelle e sotto cartelle corrispondenti ad Aziende esportate dal
gestionale non potranno essere caricati operando dal front end del sito
ma dovranno per forza di cose essere gestiti direttamente all'interno
del gestionale e, nello specifico, dovranno essere inseriti in
Docuvision nelle classi documento gestite anche sul sito.

Per la stessa ragione, ovviamente, gli utenti abilitati a gestire tali
cartelle potranno solo visionare (prelevandoli in tempo reale dal
gestionale) i documenti presenti al loro interno senza poterli
eliminare.

Per maggiori informazioni relativamente alla possibilità di prelevare in
tempo reale documenti presenti all'interno del gestionale si veda anche
quanto indicato nei successivi capitoli di questo manuale.

