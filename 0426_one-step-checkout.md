# ONE STEP CHECKOUT



Il modulo di **One Step Checkout** consente, se attivato, di gestire una
procedura di checkout molto più fluida e rapida permettendo agli utenti
del sito di concludere l'ordine con un minor numero di click operando,
eventualmente, anche in modalità Guest senza cioè dover per forza di
cose creare un proprio account all'interno del sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_step_unico.bmp](./assets/media/image296.png){width="5.527777777777778in"
height="3.31875in"}

**ATTENZIONE!** Il modulo di One Step Checkout dovrà essere
eventualmente abilitato solo per Ecommerce collegati a Mexal. Nel
momento in cui si dovesse abilitare questa configurazione per siti
connessi ad uno dei gestionali Ho.Re.Ca. potranno poi verificarsi dei
problemi nel momento in cui uno stesso utente (stesso indirizzo mail)
dovesse effettuare più ordini diversi come utente Guest

**ATTENZIONE!** L' attivazione del modulo di One Step Checkout produrrà,
lato gestionale, la creazione di una nuova anagrafica utente per ogni
ordine effettuato in modalità ospite.

In conseguenza di ciò il modulo di One Step Checkout **dovrà essere
abilitato solo per Ecommerce collegati a Mexal**. Nel caso in cui si
dovesse abilitare questa configurazione per siti connessi ad uno dei
gestionali Ho.Re.Ca. potranno infatti verificarsi dei problemi nel
momento in cui uno stesso utente (stesso indirizzo mail) dovesse
effettuare più ordini operando sempre come utente Guest.

Infine anche **nel caso di Ecommerce collegati a Mexal, per evitare
possibili problemi relativi ad eliminazione di utenti che effettuano più
volte acquisti in modalità ospite è necessario verificare di aver
attivato correttamente, su Passweb, la gestione della partita iva
secondaria**

Per poter attivare questa particolare modalità di gestione è necessario,
per prima cosa impostare il campo "**One Page Checkout**", presente tra
i parametri di configurazione del componente:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_2.bmp](./assets/media/image299.png){width="4.582638888888889in"
height="2.9506944444444443in"}

sull'opzione "**Si**" oppure sull'opzione "**Si con Riepilogo**".

In entrambi i casi all'interno del checkout, comparirà infatti un'
ulteriore sezione denominata "**Informazioni Utente**" in cui poter
inserire il componente "Registrazione Utente" trasformando, di fatto, il
tradizionale checkout custom in un modulo di "One Step Checkout" che gli
utenti del sito potranno utilizzare per completare i loro acquisti anche
in modalità Guest (Ospiti), o comunque senza dover per forza di cose
passare prima dalla pagina di "Registrazione Utente" per creare un
account di accesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_3.bmp](./assets/media/image300.png){width="4.601388888888889in"
height="2.588888888888889in"}

Per inserire il componente di Registrazione all'interno del checkout
sarà poi sufficiente agire come per un qualsiasi altro componente
Passweb.

Una volta abilitata quindi la modalità di gestione dei componenti, sarà
necessario accedere per prima cosa ai componenti interni al "Checkout
Custom" cliccando per questo sull'apposita icona presente nel R.O.C. del
componente, abilitare la modalità di Aggiunta Nuovi Componenti,
selezionare il componente "Registrazione Utente" ed inserirlo nella
nuova sezione "Informazioni Utente" mediante una semplice operazione di
Drag and Drop.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_4.bmp](./assets/media/image301.png){width="5.159722222222222in"
height="3.484722222222222in"}

A questo punto la creazione e configurazione del form mediante il quale
richiedere all'utente i dati necessari per completare l'ordine potrà
avvenire, anche in questo caso, in maniera del tutto analoga a quella
con cui si crea, normalmente, un qualsiasi form di Registrazione Utente.

Per maggiori informazioni in merito si rimanda dunque al relativo
capitolo ("*Varianti Responsive --* *Lista Componenti di Interazione
Utente -- Componente Registrazione Utente*") di questo manuale.

Ovviamente le informazioni richieste in queste circostanze sono diverse,
generalmente, da quelle richieste in un tradizionale form di
registrazione utente. In queste condizioni infatti vengono richiesti
solo i dati strettamente necessari per poter completare l'ordine come ad
esempio, il Nome Utente, il Cognome o la Ragione Sociale nel caso in cui
l'utente sia un'Azienda, eventualmente, sempre nel caso di utenti di
tipo Azienda, la Partita IVA, un' indirizzo Email cui inoltrare le mail
di comunicazione relative ai vari stati dell'ordine ed i dati per gli
indirizzi di spedizione e/o fatturazione.

In virtù di tutto ciò il componente Registrazione inserito all'interno
di un Checkout Custom ha alcune particolarità che lo differenziano
leggermente dall'omonimo componente inserito però all'interno della
pagina di Registrazione e questo sia a livello di componenti, e quindi
campi gestibili al suo interno, sia a livello di funzionalità vere e
proprie.

Nello specifico relativamente ai campi gestibili all'interno del
Componente Registrazione Utente, è necessario prestare particolare
attenzione ai componenti "**Campo Checkbox**", "**Campo Radio**" e
"**Campo Lista Valori**" che, in queste condizioni, potranno essere
utilizzati per consentire all'utente che sta effettuando l'ordine di:

- creare o meno, contestualmente all'inserimento dell'ordine, anche un
  suo account sul sito

- utilizzare o meno gli stessi dati per l'indirizzo di spedizione e per
  quello di fatturazione

- selezionare come indirizzo di spedizione e / o di fatturazione uno
  degli indirizzi presenti nel suo Profilo o eventualmente crearne uno
  nuovo

Per maggiori informazioni in merito si vedano anche i successivi
capitoli di questo manuale

Per quel che riguarda il funzionamento del modulo di One Step Checkout è
bene sottolineare che nel momento in cui ad utilizzare questo modulo
dovesse essere un utente non autenticato, non appena compilati tutti i
campi obbligatori per la definizione dell'indirizzo di fatturazione ed,
eventualmente, quelli necessari per definire un diverso indirizzo di
spedizione, verranno ovviamente mostrate tutte le tipologie di
spedizione coerenti con l'indirizzo impostato. Inoltre verrà creata
immediatamente anche la relativa Anagrafica Utente di Passweb.

Nello specifico, in queste condizioni, l'utente risulterà essere un
**Utente di tipo Contatto** (perché non ha ancora concluso l'ordine) e
sarà marcato anche come utente di tipo **Ospite** (perché in questo
momento non ha ancora deciso di creare un proprio account di accesso al
sito)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_12.bmp](./assets/media/image302.png){width="4.607638888888889in"
height="2.6625in"}

**ATTENZIONE!** anche per gli utenti di tipo "**Ospite**" verrà eseguito
quanto di seguito indicato:

- Applicazione di eventuali regole definite sugli Attributi Utente

- Assegnazione dell'utente Ospite ai "Gruppi Utente" del sito secondo le
  regole impostate per lo specifico Gruppo

- Applicazione delle specifiche condizioni commerciali del Gruppo Utenti
  in cui l'utente Ospite risulta inserito

Proseguendo nella fase di checkout nel caso in cui l'utente dovesse
decidere di completare l'ordine come ospite, senza creare quindi uno
specifico account per l'accesso al sito, alla conferma dell'acquisto il
sistema provvederà ad inviare all'indirizzo da lui stesso inserito nel
modulo di checkout la prima mail Nuovo Ordine con il riepilogo di quanto
acquistato.

A questo stesso indirizzo mail verranno inoltre inviate tutte le altre
comunicazioni relative ai vari stati dell'ordine (mail di Conferma, di
Evasione ecc...) e queste saranno l'unico strumento a disposizione
dell'utente per controllare lo stato del suo ordine. Avendo infatti
deciso di effettuare l'acquisto in modalità ospite l'utente non avrà
modo di accedere al sito per controllare lo stato e/o lo storico di
tutti i suoi ordini.

Nel momento in cui l'ordine verrà inserito all'interno del gestionale
l'utente diverrà, come al solito, un **Utente di tipo Cliente** **che
però sarà sempre marcato anche come Ospite** in virtù della scelta da
lui effettuata di non creare un account di accesso al sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_13.bmp](./assets/media/image303.png){width="4.607638888888889in"
height="2.6625in"}

Se invece, proseguendo nella fase di checkout, l'utente dovesse decidere
di completare l'ordine creando anche un proprio account allora, non
appena compilati i campi relativi ad Username e Password, il sistema
provvederà a creare immediatamente il relativo account, ad inviare
all'indirizzo mail indicato dall'utente la mail di registrazione con il
riepilogo dei dati e ad autenticare l'utente stesso sul sito esattamente
come se avesse effettuato un normale processo di registrazione.

Ovviamente anche in queste condizioni, una volta completata la
registrazione verranno valutate eventuali regole di appartenenza a
specifici gruppi utente, condizioni commerciali associate a questi
stessi gruppi ecc..., in altri termini tutto procederà esattamente come
se questo utente avesse effettuato prima la registrazione, si fosse
autenticato e avesse deciso poi di effettuare un ordine.

In queste condizioni quindi, subito dopo aver inserito Username e
Password e aver creato di fatto il suo account di accesso al sito,
l'utente verrà marcato come **Utente di tipo Contatto** (perché non ha
ancora concluso l'ordine) **ma NON come Ospite**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_14.bmp](./assets/media/image304.png){width="4.607638888888889in"
height="2.6625in"}

Terminato l'acquisto e inserito l'ordine all'interno del gestionale,
come al solito, l'utente cambierà la sua tipologia passando da Contatto
a Cliente.

Sempre in relazione al funzionamento del modulo di One Step Checkout, è
bene evidenziare anche altre cose di fondamentale importanza. Nello
specifico:

- Il check "Crea Account" e gli eventuali campi di tipo Username,
  Password verranno visualizzati, per ovvie ragioni, solo ed
  esclusivamente se ad utilizzare il modulo di One Step Checkout sia un
  utente che non ha ancora effettuato l'autenticazione al sito e che
  quindi ha ancora la possibilità di decidere se continuare l'acquisto
  come ospite o se creare anche un proprio account.

- Nel caso in cui un utente decida di effettuare un ordine come guest,
  il sistema provvederà ad inviare tutte le mail connesse ai vari stati
  dell'ordine all'indirizzo fornito dall'utente stesso all'interno del
  modulo di One Step Checkout (dove il campo Email dovrà quindi essere
  inserito sempre come campo obbligatorio). Non avendo però creato un
  proprio account l'utente non avrà ovviamente la possibilità di
  effettuare successivi accessi al sito per controllare lo stato dei
  propri ordini.

- Nel momento in cui ad utilizzare il modulo di One Step Checkout
  dovesse essere un utente che ha già effettuato l'autenticazione al
  sito, all'interno della sezione "Informazioni Utente" verranno
  visualizzati, ovviamente, i suoi dati anagrafici (gli stessi che
  visualizzerebbe anche alla pagina Profilo Utente). Nello specifico i
  campi:

  - Indirizzo, Località, Provincia, Nazione e CAP visualizzeranno i dati
    presenti, per gli stessi campi nell'anagrafica gestionale
    dell'utente

  - Indirizzo n.2, Località n.2, Provincia n.2, Nazione n.2, CAP n.2 e
    Nominativo n.2 visualizzeranno i dati relativi al primo indirizzo di
    spedizione dell'utente in esame

  - Indirizzo n.3, Località n.3, Provincia n.3, Nazione n.3, CAP n.3 e
    Nominativo n.3 visualizzeranno i dati relativi al secondo indirizzo
    di spedizione dell'utente in esame

  - Indirizzo n.4, Località n.4, Provincia n.4, Nazione n.4, CAP n.4 e
    Nominativo n.4 visualizzeranno i dati relativi al terzo indirizzo di
    spedizione dell'utente in esame

> Ulteriori indirizzi di spedizione potranno, eventualmente, essere
> codificati e gestiti all'interno della pagina Profilo Utente mediante
> l'apposito componente "Rubrica Indirizzi"
>
> **ATTENZIONE! In queste condizioni, eventuali variazioni, apportate a
> questi dati si rifletteranno poi nell'Anagrafica Cliente del
> gestionale e/o nei relativi indirizzi di spedizione.**

- Nel caso in cui sia stata attivata la modalità di **registrazione
  utenti con "Attivazione Differita" o quella con "Verifica Mail" queste
  non verranno applicate, ovviamente, nel momento in cui l'utente
  dovesse decidere di creare un account direttamente all'interno del
  modulo di One Step Checkout**.

> In queste condizioni infatti, come precedentemente evidenziato, non
> appena compilati i campi relativi ad Username e Password, il sistema
> creerà immediatamente il relativo account e autenticherà l'utente sul
> sito senza attendere eventuali ulteriori conferme.

