# PAYPAL EXPRESS CHECKOUT -- PAGAMENTO SUL SITO PASSWEB



Una volta abilitata ed impostata correttamente la modalità di pagamento
"PayPal Express Checkout", comparirà, nella pagina Carrello del proprio
sito e-commerce il pulsante "**PayPal Express Checkout**" visibile sia
ad utenti autenticati che a normali visitatori del sito che non hanno
ancora effettuato la registrazione.

![](./assets/media/image183.png)

**ATTENZIONE!** Nel caso di prenotazione di servizi con possibilità di
pagamento on line (Ecommerce Ho.Re.Ca.), il pulsante "**PayPal Express
Checkout**" verrà invece visualizzato direttamente all'interno del
Catalogo assieme al pulsante "**Prenota**".

**Questa modalità di pagamento consentirà quindi anche ad utenti non
ancora registrati sul proprio sito e-commerce di portare comunque a
termine un acquisto**

Indipendentemente dal fatto di essere o meno già registrati e
autenticati all'interno del sito e-commerce, nel momento in cui un
utente, dopo aver messo articoli in carrello, dovesse cliccare sul
pulsante "**PayPal Express Checkout**" verrà infatti automaticamente
ridiretto al gateway di pagamento di PayPal.

![](./assets/media/image184.png)

Nel caso in cui l'utente che effettua l'acquisto dovesse già disporre di
un proprio conto PayPal potrà quindi autenticarsi sul gateway di
pagamento utilizzando questo stesso account in maniera tale da poter poi
sfruttare tutte le informazioni personali memorizzate direttamente sul
sito di PayPal e necessarie per poter completare l'acquisto (carte di
credito, indirizzi di spedizione ecc...)

In ogni caso una volta inseriti i dati richiesti da PayPal verrà
mostrata all'utente una maschera riepilogativa del tipo di quella qui di
seguito riportata

![](./assets/media/image185.png)

Cliccando quindi sul pulsante **"Continua"** l'utente verrà ricondotto
alla pagina di checkout del sito e-commerce dove dovrà, eventualmente,
compilare gli step necessari alla conferma dell'ordine e al suo
inserimento all'interno del gestionale.

A questo punto è necessario però fare una distinzione relativamente al
comportamento di Passweb in relazione al fatto che l'utente che sta
effettuando l'acquisto e il pagamento su PayPal fosse o meno già
registrato e/o autenticato sul sito e-commerce prima di essere ridiretto
al gateway di PayPal.

Nello specifico occorre quindi considerare che:

a)  Nel caso in cui l'utente che effettua l'acquisto e il pagamento con
    modalità "PayPal Express Checkout" non fosse ancora registrato sul
    sito e-commerce, quando, dopo aver inserito sul sito di PayPal tutti
    i dati necessari al completamento della transazione, cliccherà sul
    pulsante Continua, il gateway di PayPal si preoccuperà non solo di
    ridirigere l'utente sul sito e-commerce in maniera tale da
    consentirgli di inserire eventuali ulteriori informazioni necessarie
    per il completamento dell'ordine, ma trasferirà anche a Passweb
    tutte le informazioni necessarie per la creazione di una nuova
    anagrafica utente all'interno del database del sito e-commerce e
    conseguentemente del gestionale ad esso collegato.

> **Passweb effettuerà quindi una registrazione totalmente automatica
> del nuovo utente sfruttando, per quanto possibile, le informazioni
> (nome, cognome, indirizzo mail ecc...) ritornate dal sito di PayPal,
> utilizzando come login l'indirizzo mail inserito dall'utente su PayPal
> e generando una specifica password da associare al nuovo utente**.
>
> **L'indirizzo di spedizione inserito all'interno di PayPal verrà
> considerato come indirizzo primario ed inserito quindi nella relativa
> anagrafica utente Passweb**.
>
> Dopo essere stato reindirizzato sul sito e-commerce l'utente si
> troverà quindi automaticamente loggato su questo stesso sito e
> riceverà, all'indirizzo mail indicato su PayPal, la mail di "Nuovo
> utente" configurata su Passweb, con il riepilogo di tutte i suoi dati.
>
> **NOTA BENE**: affinchè la procedura possa terminare in maniera
> corretta è obbligatorio gestire sul proprio sito ecommerce
> **l'Attivazione utenti in maniera Immediata**. In caso contrario
> potranno completare l'acquisto con questa modalità solo gli utenti già
> registrati sul sito. Per maggiori informazioni in merito si veda la
> sezione "Utenti -- Configurazione Parametri Utenti Ecommerce" di
> questo manuale.

b)  **Nel caso in cui l'utente che effettua l'acquisto e il pagamento
    con modalità "PayPal Express Checkout" fosse già registrato sul sito
    e-commerce ma non ancora autenticato,** il comportamento
    dell'applicazione potrebbe cambiare in relazione a diversi fattori
    come ad esempio il fatto che chi effettua l'acquisto utilizzi sempre
    lo stesso account PayPal, la stessa carta di credito o lo stesso
    indirizzo mail già associato alla sua anagrafica Passweb.

> Nel caso in cui l'utente che effettua l'acquisto sul sito ecommerce
> utilizzi sempre lo stesso account PayPal per effettuare il pagamento,
> non ci sono problemi, nel senso che PayPal associa ad ogni account un
> identificativo univoco che viene poi ritornato (ovviamente dopo aver
> effettuato e confermato il primo ordine con questa modalità di
> pagamento) e memorizzato nel database di Passweb.
>
> Per acquisti successivi al primo Passweb sarà quindi in grado, sulla
> base dei dati ritornati da PayPal, di agganciare l'anagrafica utente
> corretta, effettuare automaticamente l'autenticazione senza dover
> quindi creare nessuna nuova anagrafica.
>
> Nel caso in cui invece l'utente che effettua l'acquisto sul sito
> ecommerce non utilizzi un' account PayPal ma inserisca, ogni volta,
> tutte le informazioni necessarie per confermare una transazione,
> allora vanno distinti diversi casi.
>
> In questo senso occorre infatti sottolineare che PayPal associa ad
> ogni carta di credito utilizzata per effettuare un pagamento, un
> "PayerId" univoco che viene poi restituito al sito ecommerce per
> consentirgli di agganciare eventualmente un anagrafica già presente
> nel suo database.
>
> In particolare dunque nel caso in cui venga utilizzata esattamente la
> stessa carta di credito che è stata utilizzata per l'ultimo acquisto
> sullo stesso sito ecommerce con questa stessa modalità di pagamento
> (quindi un PayerId già presente nel database Passweb) acquisendo i
> dati di ritorno da PayPal, Passweb riuscirà ad agganciare l'anagrafica
> utente già presente all'interno del suo database evitando quindi di
> effettuare registrazioni automatiche di nuovi utenti.
>
> Nel caso un cui venga invece utilizzata una carta di credito
> differente da quella utilizzata per l'ultimo acquisto effettuato (e
> quindi un PayerId non presente nel database Passweb) acquisendo i dati
> di ritorno da PayPal, Passweb effettuerà un controllo sull'indirizzo
> mail. Nel momento in cui dovesse trovare tra le sue anagrafiche un
> indirizzo mail già presente, prima di effettuare il login automatico e
> di andare sostituire al PayerId associato all'anagrafica del relativo
> utente quello nuovo appena ritornato da PayPal, chiederà all'utente
> stesso una verifica della propria identità.
>
> In particolare, in queste condizioni, al ritorno sul sito ecommerce
> verrà presentata all'utente **una apposita maschera in cui inserire un
> codice di verifica, codice questo che verrà inviato alla mail inserita
> dall'utente stesso in fase di pagamento su PayPal.**
>
> Solo inserendo il codice richiesto e confermando quindi la propria
> identità Passweb potrà agganciare correttamente l'anagrafica utente
> già presente nel suo database, effettuare l'autenticazione automatica
> e mettere l'utente nelle condizioni di portare a termine il proprio
> ordine.
>
> Nel momento in cui dovesse essere correttamente agganciata
> l'anagrafica di un utente già presente in Passweb, l'applicazione si
> preoccuperà poi di gestire anche l'indirizzo di spedizione
> ritornatogli da PayPal.
>
> In particolare se l'indirizzo di spedizione selezionato o inserito in
> PayPal dovesse coincidere con uno degli indirizzi di spedizione
> associati in Passweb all'utente in questione non verranno aggiunte, in
> questo senso ulteriori informazioni. Nel momento in cui invece
> l'utente dovesse indicare su PayPal un nuovo indirizzo di spedizione,
> questo verrebbe considerato da Passweb come nuovo indirizzo primario
> andando quindi a sovrascrivere quello attualmente presente
> nell'anagrafica dell'utente il quale, a sua volta, verrà
> automaticamente trattato come indirizzo di spedizione secondario
>
> Infine nel caso in cui venga utilizzata su PayPal una nuova carta di
> credito (e quindi un PayerId non ancora presente nel database Passweb)
> e anche un nuovo indirizzo mail, Passweb non riuscirà, ovviamente, ad
> agganciare nessuna anagrafica e in conseguenza di ciò effettuerà una
> nuova registrazione esattamente come nel caso a) precedentemente
> esaminato.

c)  **Nel caso in cui l'utente che effettua l'acquisto e il pagamento
    con modalità "PayPal Express Checkout" fosse già registrato e anche
    autenticato sul sito e-commerce** e nel caso in cui alla sua
    anagrafica non sia stato ancora aggiunto nessun PayerId, Passweb
    utilizzerà i dati ritornati da PayPal per associare a questo stesso
    utente il PayerId corrispondente alla carta di credito attualmente
    utilizzata (in maniera tale da consentire, ai successivi accessi di
    individuare univocamente questo utente anche nel caso in cui
    l'acquisto venga effettuato senza aver prima fatto
    l'autenticazione): Nel caso in cui l'utente abbia già un PayerId
    associato e utilizzi una nuova carta di credito non verrà invece
    aggiunta nessuna informazione e verranno utilizzate semplicemente le
    informazioni già presenti in Passweb per quello stesso utente.

> Anche in questo caso verranno poi gestiti, nelle modalità
> precedentemente indicate, gli indirizzi di spedizione dell'utente in
> relazione a quelli inseriti o aggiunti direttamente all'interno di
> PayPal

In ogni caso, dopo essere stato ricondotto alla pagina di checkout del
sito ecommerce**, l'utente, come detto, potrebbe trovarsi nelle
condizioni di dover inserire eventuali ulteriori informazioni necessarie
alla conferme dell'ordine e al suo inserimento nel gestionale,
informazioni queste (tipo di documento da generare, eventuali note,
parametri esterni all'ordine ecc...) che dipenderanno dalle particolari
impostazioni settate all'interno di Passweb, ad esempio, sul componente
"Checkout Ordine" o nella maschera di configurazione ordini.**

**NOTA BENE**: in questa fase non verrà comunque più richiesta
all'utente la selezione della modalità di pagamento, mentre la sezione
relativa agli indirizzi di spedizione sarà già impostata sull'indirizzo
scelto dall'utente sul sito di PayPal.

Infine nel caso in cui, in fase di ritorno da PayPal al sito Passweb per
la conferma definitiva dell'ordine, si dovessero verificare dei problemi
di qualsiasi tipo legati alla transazione effettuata all'interno di
PayPal, l'ordine resterà memorizzato all'interno di Passweb nello stato
di "**Pagamento non Confermato**" e, in questo senso andrà quindi
trattato manualmente come avviene per tutte le altre metodologie di
pagamento mediante carta di credito disponibili in Passweb.

In queste condizioni sarà quindi compito dell'esercente verificare
effettivamente l'avvenuto accredito all'interno del suo conto PayPal per
poi eventualmente validare l'ordine, consentendone quindi l'inserimento
all'interno del gestionale (alla prossima sincronizzazione utile) oppure
eliminarlo definitivamente dal database di Passweb.

