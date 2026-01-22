# COMPONENTE LISTA REGALO



Una **"Lista Regalo**" altro non è se non una particolare lista di
articoli, selezionati da un determinato utente (il creatore della
lista), che altri utenti opportunamente abilitati (con i quali è stata
cioè condivisa la lista) potranno acquistare, fino ad esaurimento della
lista stessa, accedendo all'apposita sezione del sito.

Per poter attivare e gestire correttamente una "Lista Regalo"
all'interno del proprio sito Passweb è necessario passare attraverso
diversi step, nello specifico:

- **Creazione della Lista Regalo.**

> Operazione effettuabile dal front end del sito direttamente
> dall'utente destinatario della lista e necessaria per costituire la
> base dati, ossia l'insieme di articoli che gli utenti opportunamente
> abilitati (che avranno cioè accesso alla lista stessa) potranno poi
> acquistare. **Richiede la corretta configurazione del componente
> "Wishlist Custom"**

- **Condivisione della Lista Regalo**

> Operazione effettuabile da front end del sito direttamente dall'utente
> destinatario della lista e necessaria per definire l'insieme degli
> "invitati", ossia degli utenti che avranno poi accesso alla relativa
> Lista Regalo potendone così acquistare i vari prodotti.
>
> Considerando che la condivisione delle Lista può avvenire via Social
> Network oppure via Email, **può richiedere la creazione di un'apposita
> Campagna di Newsletter e quindi la corretta integrazione del proprio
> sito Passweb con MailChimp**

- **Acquisto dalla Lista Regalo**

> Operazione effettuabile dagli "invitati" alla relativa lista.
>
> **Richiede la creazione della pagina "Lista Regalo" e la corretta
> configurazione dell'omonimo componente**

**ATTENZIONE!** Per maggiori informazioni in merito a ciascuno degli
step sopra indicati si faccia riferimento ai successivi capitoli di
questo manuale.

Il componente "**Lista Regalo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_lista_regalo.bmp](./assets/media/image219.png){width="2.3555555555555556in"
height="2.8159722222222223in"}

**per sua stessa natura, può quindi essere inserito unicamente
all'interno dell'omonima pagina** ed è di fondamentale importanza in
quanto, se configurato correttamente, sarà quello che consentirà poi
agli invitati alla lista di poterne acquistare i vari prodotti.

Gli articoli visualizzati all'interno di questo componente varieranno,
ovviamente, in relazione alla specifica Lista Regalo per cui nel momento
in cui un utente dovesse accedere alla pagina "Lista Regalo" senza aver
selezionato o indicato una specifica Lista il componente potrebbe essere
privo di articoli.

**In generale verrà comunque mantenuto in sessione l'identificativo
dell'ultima Lista Regalo visualizzata** per cui, una volta visualizzati
gli articoli presenti all'interno di una certa lista se, durante la
stessa sessione di navigazione, lo stesso utente dovesse accedere con lo
stesso browser alla pagina "Lista Regalo" verrà comunque visualizzata
l'ultima Lista Regalo consultata senza doverla per forza di cose
ricercare dall'apposito pannello di ricerca

**ATTENZIONE!** Non è possibile applicare filtri di ricerca alla Lista
Articoli

**ATTENZIONE! I prezzi degli articoli presenti in Lista Regalo sono
sottoposti ad eventuali particolarità prezzo e/o sconto associate
all'utente che sta effettuando l'acquisto e non ad eventuali
particolarità definite per il creatore/gestore della lista**

