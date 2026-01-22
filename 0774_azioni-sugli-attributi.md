# AZIONI SUGLI ATTRIBUTI



Tornando a prendere in considerazione la maschera principale
"**Attributi per il Catalogo**" i pulsanti presenti nella barra degli
strumenti consentono rispettivamente di:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_catalogo2.bmp](./assets/media/image113.png)

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image43.png) ): permette di modificare le
caratteristiche dell'attributo attualmente selezionato in elenco.

**Elimina**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image114.png) ): consente di eliminare definitivamente
l'attributo selezionato.

**Utilità**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_utilita.bmp](./assets/media/image115.png) ): consente di richiamare alcune
procedure automatiche che potranno essere effettuate sugli articoli
attualmente selezionati in elenco.

Cliccando infatti su questo pulsante verrà ricaricata la griglia degli
attributi (**che diventerà ora a selezione multipla**) e che
visualizzerà i soli attributi di tipo Passweb.

**NOTA BENE:** le procedure automatiche gestite all'interno di questa
sezione potranno essere lanciate solo ed esclusivamente in relazione ad
attributi articolo di tipo Passweb. Gli attributi articolo di tipo
Mexal, con i relativi valori, potranno infatti essere gestiti solo ed
esclusivamente all'interno del gestionale.

Nella barra degli strumenti compariranno ora nuove icone a ciascuna
delle quali sarà associata una specifica procedura.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_catalogo_utilita.bmp](./assets/media/image116.png)

In particolare il pulsante

**Default**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_default.bmp](./assets/media/image117.png) ): consente di impostare, per tutti gli
articoli appartenenti a categorie merceologiche cui è stato associato un
set di attributi che comprende uno degli attributi attualmente
selezionanti in elenco, il valore di questi stessi attributi al loro
attuale valore di default.

Come precedentemente evidenziato infatti il valore di default impostato
all'atto della definizione di un certo attributo di fatto altro non è se
non un valore propositivo. Per memorizzare, in relazione allo specifico
articolo, questo valore all'interno del database di Passweb occorre
lanciare necessariamente la procedura in oggetto.

**Azzera**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_azzera.bmp](./assets/media/image118.png) ): consente di rimuovere, per tutti gli
articoli appartenenti a categorie merceologiche cui è stato associato un
set di attributi che comprende uno degli attributi attualmente
selezionanti in elenco, il valore attualmente memorizzato, per questi
stessi articoli, nel database di Passweb, in relazione agli attributi
selezionati in elenco.

Una volta lanciata la procedura automatica associata al pulsante
Default, o più semplicemente, una volta salvata l'anagrafica Passweb di
un certo articolo, come precedentemente evidenziato, i valori degli
attributi di questo articolo verranno memorizzati nel database di
Passweb diventando quindi di proprietà esclusiva dell' articolo stesso.

In queste condizioni nel caso in cui dovesse poi essere specificato un
valore di default differente per gli attributi di questo articolo, tale
variazione non avrebbe conseguenze sull'articolo in oggetto e i suoi
attributi continuerebbero ad assumere i valori attualmente presenti nel
database.

La procedura associata al pulsante "**Azzera**" consente di eliminare i
valori attualmente memorizzati nel database riportando quindi i relativi
attributi nelle condizioni iniziali (in cui il valore di default è
considerato soltanto come un valore propositivo)

**Riorganizza**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_riorganizza.bmp](./assets/media/image119.png) ): consente di rimuovere i valori degli
attributi selezionati per tutti gli articoli appartenenti a categorie
merceologiche che non usano un set di attributi che include gli
attributi attualmente selezionati in elenco.

Spostando un articolo da una categoria merceologica ad un\'altra (ed
agendo per questo direttamente dal gestionale) potrebbero variare gli
attributi associati all'articolo. Le due categorie merceologiche di
partenza e di arrivo potrebbero infatti avere associati due set di
attributi completamente differenti.

In queste condizioni potrebbe quindi succedere che l'articolo in
questione pur visualizzando gli attributi della categoria di arrivo sia
ancora ricercabile all'interno del sito anche per gli attributi della
sua categoria merceologica di partenza. Questo perché lo spostamento di
categoria merceologica effettuato da Mexal non si preoccupa di
verificare le differenze tra gli attributi Passweb associati alle due
diverse categorie merceologiche, per cui nel database di Passweb, in
relazione a questo specifico articolo, continueranno ad essere presenti
sia gli attributi della vecchia categoria merceologica sia quelli della
nuova.

La procedura associata al pulsante "**Riorganizza**" effettua proprio
questo tipo di verifica, preoccupandosi di andare a vedere per tutti gli
articoli gestiti all'interno del sito, se gli attributi attualmente
selezionati in elenco appartengono o meno al set di attributi associato
allo specifico articolo. Nel caso in cui non sia così la procedura si
preoccuperà anche di eliminare per i vari articoli questi stessi
attributi.

**NOTA BENE**:nel caso in cui le procedure associate ai tre pulsanti
sopra indicati vengano lanciate senza aver selezionato alcun attributo,
queste stesse procedure verranno eseguite per tutti gli attributi in
elenco.

**Deseleziona**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_deseleziona.bmp](./assets/media/image120.png) ): consente di deselezionare in un colpo
solo tutti gli attributi attualmente selezionati in elenco.

**Gestione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_gestione.bmp](./assets/media/image121.png) ): consente di uscire dalla sezione
relativa alle Utilità tornando quindi alla normale gestione degli
Attributi Articolo.

