# STATICIZZAZIONE E CARICAMENTO ASINCRONO DEI COMPONENTI



Altri due campi particolarmente importanti e comuni a molti dei
componenti Passweb sono quelli relativi ai due parametri "**Caricamento
Javascript**" e "**Statico**", parametri questi che, in determinate
condizioni, possono abbattere i tempi di caricamento della pagina web.

Per comprendere meglio il significato e l'utilizzo di questi parametri
occorre però fare alcune precisazioni.

I siti Passweb sono siti dinamici per cui ogni pagina del sito viene
costruita a runtime nel momento stesso in cui viene richiesta prelevando
tutti i dati necessari direttamente dal server web.

Se, da una parte, questo costituisce un enorme vantaggio perché
consente, ad esempio, di visualizzare contenuti diversi (prezzi,
prodotti, condizioni commerciali ecc...) a seconda dell'utente che sta
navigano il sito, dall'altra parte occorre anche considerare che i tempi
di caricamento della pagina web possono essere superiori rispetto a
quelli di pagine statiche che mostrano sempre gli stessi contenuti a
tutti gli utenti.

In questo senso occorre infatti considerare che per ogni componente
presente all'interno della pagina web dovranno essere fatte,
dipendentemente dalla tipologia di componente considerata, diverse
interrogazioni lato server in maniera tale da poter prelevare i
contenuti corretti da inserire all'interno della pagina.

Considerando quindi che, di base, il caricamento di tutti i componenti
Passweb avviene in maniera sincrona, prima di poter visualizzare la
pagina web occorre attendere che per tutti i componenti presenti
all'interno della pagina stessa siano state prelevate le informazioni
corrette, anche se un determinato componente non dovesse essere
immediatamente visibile o utilizzabile dall'utente (perché ad esempio
posto nella parte bassa della pagina, in un contenitore offcanvas ...).

Per poter abbattere, dove possibile, i tempi di caricamento della pagina
web, alcuni componenti mettono quindi a disposizione, in fase di
configurazione, i due parametri "Caricamento Javascript" e "Statico"
che, nello specifico, consentono rispettivamente di:

- **Caricamento Javascript**: consente, se selezionato, di caricare il
  relativo componente in maniera asincrona al termine del caricamento
  della pagina web.

> In queste condizioni dunque la pagina verrà caricata, inizialmente,
> senza i contenuti del componente in esame, contenuti questi che
> verranno poi inseriti in maniera asincrona solo dopo che la pagina
> stessa è stata interamente caricata.
>
> Questo parametro potrebbe quindi consentire di ottenere un tempo di
> risposta migliore soprattutto se utilizzato per quei componenti che
> non devono essere immediatamente visualizzati all'interno della pagina
> (pensiamo ad esempio a componenti posti in contenitori collassabili,
> offcanvas o semplicemente posti nella parte bassa della pagina web) o
> che dovessero essere particolarmente "pesanti" in termini di
> interrogazioni lato server (pensiamo ad esempio a menu di categorie
> con migliaia di voci).
>
> **ATTENZIONE!** Nel momento in cui a richiedere la pagina dovesse
> essere un bot o uno spider il parametro in esame verrà ignorato in
> maniera tale da garantire comunque che lo spider possa navigare e
> indicizzare correttamente tutte le pagine del sito

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico. In caso affermativo, al salvataggio del
  componente, verrà generato il codice HTML relativo al componente in
  esame in tutte le lingue gestite e, in fase di visualizzazione della
  pagina web, verrà mostrato il contenuto corrispondente a questo stesso
  codice HTML senza effettuare ulteriori interrogazioni lato server.

> In sostanza dunque, se in precedenza per determinare e visualizzare il
> contenuto di un determinato componente potevano essere necessarie
> diverse interrogazioni lato server, una volta staticizzato sarà
> sufficiente una sola query per ottenere e visualizzare questo stesso
> contenuto.
>
> **ATTENZIONE!** Il codice HTML che viene generato è esattamente quello
> necessario per visualizzare il contenuto del componente nella pagina
> del Wizard in cui questo stesso componente è stato staticizzato
>
> Inoltre, se il componente in esame dovesse avere delle interazioni
> javascript (es. paginazione in componenti come Catalogo Ecommerce o
> applicazione di filtri su pannelli di ricerca) nel momento in cui
> l'utente dovesse effettuare questo tipo di interazione, il componente
> tornerà ad assumere la sua dinamicità prelevando i contenuti corretti
> direttamente dal server.
>
> Come è semplice comprendere l'utilizzo di questo parametro, e quindi
> il fatto di staticizzare o meno determinati componenti, potrebbe
> impattare in maniera considerevole sul numero di interrogazioni lato
> server necessarie per visualizzare il contenuto di una pagina
> diminuendo, conseguentemente, i tempi di caricamento della pagina
> stessa.
>
> D'altra parte occorre sempre prestare particolare attenzione anche a
> cosa significa staticizzare un componente e a quelle che sono le
> condizioni in cui quel componente può o non può effettivamente essere
> staticizzato.
>
> **In questo senso infatti, occorre aver sempre ben chiaro il concetto
> che una** **volta staticizzato un componente poi i contenuti da esso
> visualizzati sul front end del sito saranno sempre gli stessi
> indipendentemente dall'utente che sta navigando e/o dalla pagina in
> cui il componente stesso si trova. In conseguenza di ciò:**

- **Se il componente in esame deve mostrare dati diversi a seconda
  dell'utente che naviga il sito**

- **Se il componente è distribuito su più pagine e, a seconda della
  pagina in cui si trova, deve mostrare informazioni diverse**

> **allora, in queste condizioni, chiaramente non andrebbe staticizzato
> perché si correrebbe il rischio di visualizzare sul front end
> informazioni non corrette**
>
> Pensiamo ad esempio al componente "Catalogo Ecommerce" che
> tipicamente:

- viene distribuito su tutte le pagine di categoria

- mostra articoli diversi a seconda della pagina di categoria in cui è
  inserito

- può mostrare informazioni diverse (prezzi, sconti, dati articolo ....)
  a seconda dell'utente che naviga il sito

> Staticizzare questo tipo di componente, nelle suddette condizioni non
> avrebbe ovviamente alcun senso.
>
> Potrebbe invece aver senso staticizzare un componente "offerte/novità"
> o "popolarità prodotto" posto sempre che le informazioni al suo
> interno (prezzi, sconti ecc...) siano effettivamente le stesse per
> ogni utente del sito.
>
> Allo stesso modo potrebbe aver senso staticizzare, ad esempio, un menu
> di categoria piuttosto pesante (con centinaia di voci), soprattutto se
> le variazioni apportate alla categorie gestite dovessero essere
> piuttosto rare. In queste condizioni si potrebbe optare per una
> soluzione statica che eviti, ad ogni caricamento di pagina,
> interrogazioni lato server per determinare quelle che sono le voci del
> menu, gli articoli presenti in ogni categoria ecc..., avendo però
> sempre presente che nel momento in cui si dovessero variare i dati del
> menu (perché ad esempio sono state aggiunte o tolte delle categorie)
> andrebbe poi rigenerato il codice HTML del relativo componente.
>
> **L'altro aspetto importante da tenere sempre in considerazione
> infatti è che, ogni qualvolta dovessero variare i contenuti di un
> componente statico, andrà poi rigenerato il relativo codice HTML e
> questo può essere fatto in modi diversi:**

- **entrando nella maschera di configurazione del singolo componente
  statico ed effettuando un nuovo salvataggio**

> **ATTENZIONE!** il salvataggio di un componente Statico rigenera
> esclusivamente il codice HTML di quello stesso componente.

- **utilizzando il pulsante "Genera HTML" presente nel menu di editing
  del sito**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_genera_html.bmp](./assets/media/image70.png)

> **ATTENZIONE!** il pulsante "Genera HTML" rigenera il codice HTML di
> tutti i componenti statici presenti all'interno del sito

- **in maniera automatica al termine di ogni sincronizzazione sito --
  gestionale**. Oltre alle due operazioni manuali appena analizzate
  infatti, al termine di ogni sincronizzazione sito -- gestionale (sia
  per variati che totale) verrà sempre rigenerato il codice HTML di
  tutti i componenti statici presenti all'interno del sito

