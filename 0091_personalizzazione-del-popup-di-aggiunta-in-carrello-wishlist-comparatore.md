# PERSONALIZZAZIONE DEL POPUP DI AGGIUNTA IN CARRELLO / WISHLIST / COMPARATORE



La sezione relativa alla gestione dei Testi e dei Messaggi utilizzati
all'interno del proprio sito consente anche di definire e personalizzare
la struttura dei Pop Up utilizzati dall'applicazione per notificare:

- L'aggiunta di prodotti in Carrello

- L'aggiunta di prodotti alla Wishlist

- L'aggiunta di prodotti al Comparatore

Per effettuare questo tipo di operazione è sufficiente portarsi nella
sezione relativa alla gestione dei **Testi dei Componenti**,
selezionare, rispettivamente, l'elemento **Aggiunta al Carrello**,
**Aggiunta alla Wishlist** e/o **Aggiunta al Comparatore** e cliccare
poi sul pulsante **Modifica Testi** presente nella barra degli strumenti

Tra i vari elementi personalizzabili per questa particolare tipologia di
componenti è presente anche il campo "**Aggiunta"** in corrispondenza
del quale verrà visualizzato un apposito editor HTML mediante il quale
poter definire e personalizzare il Popup che sarà poi visualizzato sul
sito nel momento in cui un utente dovesse aggiungere un articolo in
carrello, alla wishlist e/o al comparatore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\testi_messaggi_sito8.bmp](./assets/media/image459.png)

Volendo è possibile aprire l'editor in modalità full screen utilizzando
il tasto funzione **F11**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\testi_messaggi_sito9.bmp](./assets/media/image460.png)

Una volta entrati in modalità full screen è poi possibile ritornare alla
visualizzazione standard utilizzando il tasto **ESC**.

Il pulsante "**Preview**" presente nella parte alta della maschera
consente di visualizzare un'anteprima del template che si sta
realizzando per il relativo Popup, dove, ovviamente, al posto dei dati
relativi allo specifico articolo aggiunto in carrello/alla wishlist/al
comparatore, verranno visualizzati appositi segnaposto.

In modalità Preview è possibile selezionare uno qualsiasi degli elementi
presenti all'interno del Template. Cliccandoci sopra si passerà
automaticamente alla versione "**Sorgente**" del template con
evidenziata la riga di codice relativa all'elemento selezionato

La possibilità di intervenire direttamente sul codice HTML del template
offre d'altra parte dovendo intervenire direttamente sul codice HTML
questo tipo di personalizzazione richiede chiaramente specifiche
conoscenze tecniche.

In questo senso Passweb viene comunque in aiuto dell'utente in due modi
diversi.

Innanzitutto non è necessario creare da zero l'intero template; volendo,
infatti, è anche possibile partire da uno dei modelli preconfigurati
messi a disposizione direttamente da Passweb.

In questo senso cliccando sul pulsante "**Template**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\testi_messaggi_sito8a.bmp](./assets/media/image461.png)

verrà aperta la relativa galleria dei modelli preconfigurati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\testi_messaggi_sito8b.bmp](./assets/media/image462.png)

Il pulsante "**Visualizza**" presente in corrispondenza di ciascuno dei
modelli presenti in elenco consente di visualizzare, in un nuovo tab del
browser, un'immagine rappresentativa di quello che dovrebbe poi essere
il risultato finale.

Il pulsante "**Utilizza**" consente invece di caricare, nel campo
corrispondente, il codice HTML e CSS relativo al modello selezionato.

**ATTENZIONE!** i template messi a disposizione da Passweb sono soltanto
un punto di partenza e, nella maggior parte dei casi, dovranno quindi
essere customizzati, sia dal punto di vista grafico che in termini di
contenuti, secondo le specifiche esigenze del caso

Nel momento in cui il template messo a disposizione da Passweb non
dovesse quindi soddisfare le specifiche esigenze del caso, e ci fosse la
necessità di modificarlo e/o integrarlo a livello di contenuti ad
esempio con altre informazioni sarà possibile sfruttare uno degli
appositi segnaposto messi a disposizione da Passweb.

In questo senso una volta posizionato il cursore nel punto del template
in cui dovrà essere inserita la nuova informazione, sarà necessario
cliccare sul pulsante "**Seleziona un segnaposto ...**" in maniera tale
da visualizzare l'elenco di tutti i segnaposto disponibili.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\testi_messaggi_sito12.bmp](./assets/media/image463.png)

Selezionando quindi il segnaposto desiderato tra quelli presenti in
elenco, Passweb provvederà poi ad inserire automaticamente nel template
tutto il codice necessario per gestire quello specifico tipo di
informazione.

In particolare dunque l'elemento:

- **Titolo:** consente di inserire nel relativo Popup il Titolo
  dell'articolo aggiunto in carrello/alla wishlist/al comparatore

- **Immagine:** consente di inserire nel relativo Popup l'immagine
  dell'articolo aggiunto in carrello/alla wishlist/al comparatore

- **Codice Articolo:** consente di inserire nel relativo Popup il Codice
  dell'articolo aggiunto in carrello/alla wishlist/al comparatore

- **Prezzo -- solo per aggiunta in carrello:** consente di inserire nel
  relativo Popup il Prezzo dell'articolo aggiunto in carrello

> Di base verrà mostrato sempre il prezzo unitario dell'articolo in
> esame.
>
> Nel caso in cui dovessero invece essere aggiunti in carrello
> contemporaneamente, mediante l'utilizzo del configuratore tabellare,
> più articoli figlio con prezzi diversi, il prezzo mostrato nel pop up
> di aggiunta sarà la media dei prezzi unitari dei singoli articoli
> figlio e, per indiare ciò, sarà preceduto dal simbolo **∼**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popup_aggiunta_carrello_prezzo_medio.bmp](./assets/media/image464.png)

- **Subtotale -- solo per aggiunta in carrello:** consente di inserirei
  nel relativo Popup il subtotale (quantità articolo X prezzo unitario)
  del prodotto aggiunto in carrello.

> A differenza di quanto avviene per il prezzo in questo caso anche nel
> momento in cui dovessero essere aggiunti contemporaneamente, mediante
> l'utilizzo del configuratore tabellare, più articoli figlio con prezzi
> diversi il valore del subtotale sarà sempre la somma dei totali dei
> singoli prodotti

- **Quantità:** consente di inserire nel relativo Popup la quantità
  dell'articolo aggiunto in carrello/alla wishlist/al comparatore

> **ATTENZIONE!** i valori di **Quantità** e **Subtotale** mostrati nel
> pop up di aggiunta in carrello/alla wishlist/al comparatore possono
> variare anche in relazione alle impostazioni settate per il parametro
> "**Gestione articoli in carrello / wishlist**" presente alla pagina
> "**Configurazione Catalogo**" del Wizard (menu "*Catalogo -- Catalogo
> Mexal / Ho.Re.Ca.*") e quindi dal fatto che l'aggiunta in carrello del
> prodotto selezionato vada a creare una nuova riga articolo oppure ad
> aggiornare una riga dello stesso prodotto già presente in carrello
>
> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Componenti Ecommerce -- Componenti interni
> ai componenti ecommerce -- Aggiunta al carrello*" di questo manuale

- **Classi:** consente di inserire nel relativo Popup le classi CSS
  addizionali gestite automaticamente da Passweb per le diverse
  tipologie di articoli e, se presenti, anche quelle definite, per lo
  specifico prodotto, all'interno dei campi "**Classi Custom**" e
  "**Classi Regole**" della sua anagrafica Passweb.

> In questo modo sarà quindi possibile personalizzare il pop up anche in
> relazione ai diversi articoli che verranno effettivamente aggiunti in
> carrello / wishlist / compratore
>
> Per maggiori informazioni relativamente all'utilizzo dei campi "Classi
> Custom" e "Classi Regole" si rimanda a quanto indicato all'interno del
> relativo capitolo di questo manuale ("*Catalogo -- Gestione Articoli
> -- Articoli -- Anagrafica Articolo / Servizio -- Anagrafica Passweb --
> Classi CSS*")

- **Link Carrello:** consente di inserire nel Popup un pulsante per
  accedere direttamente alla pagina Carrello.

> **ATTENZIONE! Per poter garantire il corretto funzionamento del
> pulsante è necessario inserire l'elemento \$cartlink\$ come href di un
> apposito tag a**

- **Link Ordine:** consente di inserire nel Popup un pulsante per
  accedere direttamente alla pagina Ordine

> **ATTENZIONE! Per poter garantire il corretto funzionamento del
> pulsante è necessario inserire l'elemento \$checkoutlink\$ come href
> di un apposito tag a**

- **Link Wishlist -- disponibile per il componente "Aggiunta alla
  Wishlist"**

> Consente di inserire nel Popup un pulsante per accedere direttamente
> alla pagina Wishlist
>
> **ATTENZIONE! Per poter garantire il corretto funzionamento del
> pulsante è necessario inserire l'elemento \$wishlistlink\$ come href
> di un apposito tag a**

- **Chiusura Popup:** consente di inserire nel Popup un pulsante
  mediante il quale poter chiudere il Popup stesso e continuare con lo
  shopping

> **ATTENZIONE! Per poter garantire il corretto funzionamento del
> pulsante è necessario inserire l'elemento \$closepopup\$ come href di
> un apposito tag a**

- **Se l'utente appartiene al Gruppo ... -- disponibile per il
  componente "Aggiunta al Carrello"**

> I segnaposto di questo tipo consentono di inserire nel codice di
> definizione del popup delle istruzioni mediante le quali poter
> condizionare la visualizzazione di determinate informazioni
> all'appartenenza dell'utente ad uno dei Gruppi Utente gestiti
> all'interno del sito.
>
> Supponendo dunque di selezionare il segnaposto "**Se l'utente
> appartiene al Gruppo Utente Autenticato**" nel template verranno
> inserite le seguenti istruzioni
>
> **\$if(id_gruppo)\$**
>
> **\$endif\$**
>
> In questo modo il codice HMTL inserito tra le due istruzioni sopra
> evidenziate verrà visualizzato all'interno del Popup di aggiunta in
> Carrello, solo ed esclusivamente nel caso in cui l'utente che ha
> effettuato l'azione di aggiunta appartenga effettivamente al gruppo
> indicato nella condizione.
>
> **ATTENZIONE!** Questo tipo di condizioni diventa di fondamentale
> importanza, per ovvie ragioni, nel caso in cui, ad esempio, si voglia,
> da una parte visualizzare i prezzi degli articoli presenti sul sito ai
> soli utenti autenticati, e dall'altra parte lasciare comunque la
> possibilità di aggiungere articoli in carrello anche ad utenti non
> autenticati.

**ATTENZIONE!** i Testi e i Messaggi del sito sono multilingua e sono
anche gestiti a livello di Variante, per cui è necessario definire la
struttura del Popup di aggiunta articoli in carrello/alla wishlist/al
comparatore in ciascuna delle lingue e per ciascuna delle Varianti sito
gestite

