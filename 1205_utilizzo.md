# UTILIZZO



Una volta completate tutte le configurazioni indicate nel precedente
capitolo, sarà possibile ricercare, in area riservata, documenti
memorizzati all'interno del gestionale nelle relative classi Docuvision
utilizzando sia le **Cartelle Docuvision** che il pannello "**Ricerca
Documenti**"

Nello specifico per quel che riguarda **l'utilizzo delle cartelle
Docuvision** sarà necessario, innanzitutto, cliccare sulla piccola
freccia posta a lato della Cartella Azienda corrispondente all'azienda
Passcom esportata sul sito e per la quale si stanno cercando dei
documenti.

Tra le sotto cartelle della cartella Azienda troveremo una cartella
chiamata "**Docuvision**" con a fianco un piccolo lucchetto rosso ad
indicare che, alla cartella in esame, sono assegnati i permessi di sola
lettura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_documenti_1_passcom.bmp](./assets/media/image126.png)

**ATTENZIONE!** la cartella Docuvision è presente SOLO per utenti
Passcom di tipo Azienda con delle classi Docuvision impostate per essere
pubblicate all'interno del sito ed è gestita in automatico
dall'applicazione. **Non è quindi possibile modificarne le proprietà e/o
caricare al suo interno generici documenti**.

Cliccando sulla piccola freccia posta a fianco della cartella in esame
verrà avviata una connessione in tempo reale con Passcom, verranno
identificate le classi documento Docuvision impostate per essere
pubblicate sul sito, gli anni gestiti per ciascuna di esse e le
eventuali tipologie di documento anch'esse impostate per essere
pubblicate sul sito e, sulla base di queste informazioni, verrà poi
creata la corrispondente struttura di cartelle.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_documenti_2_passcomm.bmp](./assets/media/image127.png)

**ATTENZIONE!** ovviamente come la Cartella Docuvision, anche tutte le
sue sotto cartelle avranno i permessi di sola lettura (icona lucchetto)
e non sarà quindi possibile caricare nuovi documenti al loro interno ne
tanto meno sarà possibile eliminare i documenti in esse presenti
(documenti che, di fatto, risiedono sul gestionale)

A questo punto sarà sufficiente selezionare una delle cartelle
Docuvision che non ha altre sotto cartelle al suo interno (es. la
cartella relativa ad un determinato anno).

In questo modo, infatti, verrà avviata una nuova connessione con Passcom
e, nella parte destra della pagina, verrà visualizzato l'elenco dei
documenti presenti all'interno del gestionale nella corrispondente
Classe Docuvision per l'anno indicato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_ricerca_documenti_da_albero.bmp](./assets/media/image114.png)

**ATTENZIONE!** in questa fase i singoli documenti non sono ancora stati
prelevati dal gestionale

Per visualizzare uno dei documenti presenti in elenco sarà sufficiente,
esattamente come avverrebbe per un qualsiasi altro documento presente
all'interno di Cartelle Standard, selezionarlo e cliccare sul pulsante
**Scarica** (
![Videate\\area_riservata_documenti_scarica_documento.bmp](./assets/media/image107.png) ) presente nella corrispondente barra
degli strumenti.

In questo modo verrà aperta un ultima connessione in tempo reale con il
gestionale, il documento selezionato verrà trasferito sul sito e
successivamente scaricato nel browser dell'utente che lo ha richiesto.

**ATTENZIONE!** Nel caso in cui sia stata selezionata per Docuvision la
gestione a Pagine e il documento in esame sia effettivamente composto da
più pagine, verrà avviato il download di un file .zip contenente tutte
le pagine (per maggiori informazioni relativamente all'attivazione lato
Passcom della gestione Docuvision a Pagine o a Revisioni si rimanda al
relativo manuale).

Ovviamente le stesse logiche di base valide per le Cartelle Docuvision,
valgono anche per il pannello "**Ricerca Documenti**".

In altri termini dunque anche nel momento in cui dovessimo decidere di
utilizzare questo pannello per ricercare in tempo reale documenti
presenti all'interno del gestionale, queste ricerche potranno essere
fatte solo ed esclusivamente sulle classi, i tipi e gli anni dei
documenti Docuvision che si è deciso di pubblicare all'interno del sito

Il pannello "**Ricerca Documenti**" consente però, rispetto alle
Cartelle Docuvision, di effettuare delle ricerche un po' più rapide e
intuitive.

In questo caso infatti l'unico parametro obbligatorio per poter
effettuare una ricerca sarà la data (eventualmente è possibile impostare
anche un range di date)

Oltre alla data è poi possibile affinare ulteriormente le ricerche,
specificando una determinata azienda e utilizzando gli altri campi
presenti all'interno del pannello come la classe, la tipologia e il
titolo dello specifico documento Docuvision da ricercare.

**ATTENZIONE! la ricerca per titolo del documento è una ricerca di tipo
"contiene"**

Un' altra cosa di fondamentale importanza da tenere sempre in
considerazione è che il pannello "Ricerca Documenti" consente di
ricercare non solo i documenti Docuvision ma anche quelli gestiti
direttamente dall'area riservata e caricati quindi all'interno di
Cartelle Standard e / o di Cartelle Azienda corrispondenti però ad
utenti Passweb (cioè non prelevati dal gestionale ma codificati
direttamente dal back end del sito).

Supponendo dunque di indicare un certo range di date ed un Titolo
Documento, cliccando sul pulsante "**Vai**" verrà effettuata una prima
ricerca dei documenti che soddisfano il filtro impostato all'interno
delle Cartelle Standard e delle Cartelle Azienda relative ad utenti
Passweb.

Prima di visualizzare i risultati di questa ricerca verrà poi effettuata
automaticamente una seconda ricerca, sempre con gli stessi parametri di
filtro, questa volta però utilizzando le Web Api Passcom e quindi
relativa ai documenti presenti all'interno del gestionale.

Una volta completato tutto il processo i risultati di entrambe le
ricerche verranno inseriti nella griglia presente immediatamente al di
sotto del pannello di ricerca e potranno quindi essere consultati ed
utilizzati normalmente secondo quanto descritto all'interno del
precedente capitolo ("*Gestione File*") di questo manuale

**ATTENZIONE!** i parametri "**Classe Documento**" e "**Tipo
Documento**" verranno presi in considerazione, ovviamente, solo in fase
di ricerca dei documenti Docuvision.

