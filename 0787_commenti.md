# COMMENTI



La sezione **"Commenti"** accessibile dalla voce di menu ***"Catalogo --
Gestione Articoli"*** consente di visualizzare e gestire i commenti
effettuati all'interno del sito dai vari utenti in relazione ai prodotti
presenti in catalogo.

All'interno di questa pagina verrà quindi visualizzata la maschera,
**"Gestione Articoli -- Commenti"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_cms_commenti_prodotti.bmp](./assets/media/image246.png){width="5.8375in"
height="3.545138888888889in"}

contenente l'elenco di tutti i commenti effettuati all'interno del sito
sugli articoli attualmente presenti in catalogo.

**ATTENZIONE!** E' possibile visualizzare i commenti relativi ad uno
specifico Articolo partendo dalla maschera "**Gestione Articoli**",
selezionando il prodotto desiderato tra quelli presenti in elenco e
cliccando sul pulsante "**Commenti**" presente nella contestuale barra
degli strumenti. Per maggiori informazioni in merito si veda anche il
precedente capitolo *"Gestione Articoli"* di questo manuale.

Per ogni singolo commento in elenco sarà possibile visualizzare parte
del suo contenuto (colonna "**Commento**"), il prodotto cui il commento
fa riferimento (colonna "**Articolo**"), la data del commento (colonna
"**Data**") e il fatto che il commento in esame sia stato o meno già
pubblicato all'interno del sito (colonna "**Stato**").

Il pulsante raffigurante una piccola i posto in corrispondenza di ogni
singolo commento, consente poi di visualizzare il dettaglio completo del
commento stesso, oltre al suo autore e alla data di pubblicazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_commento_prodotti2.bmp](./assets/media/image307.png){width="5.8375in"
height="3.545138888888889in"}

Il pannello di ricerca, presente nella parte alta della maschera,
consente di ricercare specifici commenti, tra quelli presenti in elenco.

Selezionando uno dei commenti in elenco verranno abilitati, nella barra
degli strumenti, diversi pulsanti mediante i quali poter gestire il
commento selezionato.

In particolare il pulsante:

**Modifica Commento**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_commento.bmp](./assets/media/image248.png){width="0.7145833333333333in"
height="0.175in"} ):consente di accedere al dettaglio del commento
selezionato in elenco e, eventualmente, di modificarne il contenuto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_commento.bmp](./assets/media/image308.png){width="5.090972222222222in"
height="3.1041666666666665in"}

**Elimina Commento** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_commento.bmp](./assets/media/image250.png){width="0.6555555555555556in"
height="0.16875in"} ):consente di eliminare il commento selezionato in
elenco

**Pubblica Commento**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_pubblica_commento.bmp](./assets/media/image251.png){width="0.7013888888888888in"
height="0.175in"} ): consente di pubblicare il commento selezionato in
elenco.

**ATTENZIONE!! In merito al pulsante "Pubblica Commento" è bene
ricordare che i commenti visualizzati all'interno di questa sezione del
Wizard non sono necessariamente visibili anche sulla parte pubblica del
sito.**

Il momento in cui un commento effettuato da un utente del sito verrà
effettivamente pubblicato e sarà quindi visibile a tutti dipende infatti
da come si è configurato il componente "**Commenti Associati**" e, nello
specifico, dal fatto che per la gestione dei commenti si sia deciso di
attivare o meno la funzione del "Moderatore". Più esattamente dunque:

- **Nel caso in cui si sia deciso di NON attivare la funzione del
  moderatore**, i nuovi commenti verranno visualizzati immediatamente
  nella parte pubblica del sito. In queste condizioni l'effettiva
  visualizzazione da parte di altri utenti del commento in oggetto
  dipenderà dunque unicamente dal tempo di refresh impostato per il
  componente.

- **Nel caso in cui si sia deciso di attivare la funzione del
  moderatore,** l'effettiva pubblicazione all'interno del sito di un
  nuovo commento non sarà immediata ma dovrà necessariamente essere
  validata ed approvata dal moderatore.

In presenza di un moderatore dunque, a seguito della creazione di un
nuovo commento da parte di un utente del sito, il moderatore verrà
avvisato via mail con un'apposita messaggio contenente anche il testo
del commento effettuato.

Sarà quindi compito del moderatore portarsi all'interno di questa
sezione del Wizard, selezionare dall'elenco il commento appena
effettuato e decidere di eliminarlo o pubblicarlo utilizzando i
rispettivi pulsanti presenti nella barra degli strumenti.

**NOTA BENE**: i commenti pubblicati possono essere visibili a tutti gli
utenti del sito o ai soli utenti autenticati dipendentemente dalle
impostazioni settate per il componente "Commenti Associati".

Per maggiori informazioni sulla gestione e sui parametri di
configurazione del componente "Commenti Associati" si veda anche
l'apposita sezione di questo manuale (*Live Editing -- Lista Componenti
Ecommerce -- Commenti Associati*)

**Ricarica Commenti**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_ricarica_commenti.bmp](./assets/media/image252.png){width="0.675in"
height="0.18194444444444444in"} ): consente di ricaricare i commenti
presenti in elenco in modo tale da poter visualizzare eventuali nuovi
commenti postati all'interno del sito.

Infine, nel caso in cui venissero effettuati nuovi commenti all'interno
del sito mentre il moderatore dovesse trovarsi in questa sezione del
Wizard, oltre ad essere avvisato via mail, il moderatore potrà
accorgersi del nuovo commento anche grazie alla comparsa di un'apposita
notifica.

