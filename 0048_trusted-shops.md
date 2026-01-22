# TRUSTED SHOPS



Trusted Shops è una piattaforma (<https://www.trustedshops.it/>) che si
occupa di fornire servizi grazie ai quali poter ottimizzare due punti
critici presenti nel processo di acquisto di ogni sito Ecommerce:

- l'entrata del potenziale acquirente nel negozio

- l'uscita del cliente dal sito al momento di confermare il pagamento

Per facilitare l'entrata del potenziale acquirente nel negozio on line
Trusted Shops mette a disposizione dei negozianti uno strumento molto
efficace per la raccolta e la visualizzazione delle recensioni, cosa
questa di fondamentale importanza considerando che una percentuale
altissima di utenti basa la propria decisione di acquisto proprio sulle
opinioni di altri clienti che hanno già effettuato acquisti su quello
stesso sito.

In questo senso il sistema utilizzato da Trusted Shops prevede che alla
conferma di un ordine vengano inviati automaticamente, dal sito
Ecommerce alla piattaforma terza, tutti i dati relativi all'acquisto
appena concluso.

Una volta acquisiti questi dati Trusted Shop si preoccuperà poi di
creare appositi inviti di recensione che verranno spediti via mail ai
relativi acquirenti secondo determinate regole impostabili direttamente
dal back end della piattaforma terza.

Ricevuto l'invito l'utente potrà quindi lasciare la propria recensione
sui prodotti acquistati utilizzando i collegamenti presenti all'interno
della mail e operando sempre all'interno della piattaforma di Trusted
Shops.

Queste recensioni, infine, potranno anche essere inserite all'interno
del sito Ecommerce cha ha generato l'acquisto dove saranno visibili e
disponibili, nelle relative pagine prodotto, anche per tutti gli altri
utenti del sito che potranno quindi essere rassicurati sul fatto di
avere a che fare con un negozio online serio ed affidabile.

Per quel che riguarda invece l'uscita dal sito al momento del pagamento
occorre considerare che, come evidenziato da tutti i sondaggi effettuati
nel corso degli anni, più del 90% degli acquirenti considera la
sicurezza una variabile fondamentale su cui basare la propria decisione
di acquisto.

In questo senso Trusted Shops aiuta gli esercenti offrendo essa stessa
una garanzia di rimborso ai clienti del negozio. Un cliente consapevole
di poter richiedere un eventuale rimborso ad una società terza
riconosciuta a livello europeo sarà indubbiamente più portato a
concludere l'acquisto senza essere frenato dall'idea di poter incorrere
in brutte sorprese.

Una volta compreso quelli che possono essere i servizi offerti da
Trusted Shops (**sistema di recensioni verificate e garanzia di
rimborso**) possiamo ora analizzare il processo di integrazione fra
questa stessa piattaforma ed il proprio sito Ecommerce, processo questo
che si compone, essenzialmente, di tre fasi:

- visualizzazione su tutte le pagine del sito del badge di
  certificazione Trusted Shops, necessario per informare gli utenti che
  il sito aderisce al circuito di Trusted Shops

- invio dei dati dell'ordine alla piattaforma terza per la creazione di
  inviti di recensione ed eventuale attivazione della garanzia di
  rimborso

- visualizzazione delle recensioni certificate nelle pagine del sito
  Ecommerce

Nei successivi capitoli di questo manuale verranno indicati tutti i
passaggi necessari per poter effettuare l'integrazione in esame.

##### INTEGRAZIONE PASSWEB -- TRUSTE SHOPS

Di seguito viene indicata passo passo la procedura da seguire per
integrare il proprio sito Ecommerce con la piattaforma Trusted Shops in
maniera tale da mettere a disposizione dei propri utenti il sistema di
recensioni verificate e la garanzia di rimborso offerti da questa
piattaforma.

- Il primo passo è quello che prevede di generare lo snippet di codice
  javascript necessario per visualizzare il Trustbadge (badge di
  certificazione Trusted Shops) in tutte le pagine del sito.

> Per far questo sarà necessario accedere al seguente url
>
> <https://support.trustedshops.com/it/apps/code-generator>
>
> ed inserire nel campo evidenziato in figura

![](./assets/media/image151.png)

> il proprio **Trusted Shops ID**, dato questo fornito all'esercente
> direttamente da Trusted Shops all'atto della sottoscrizione al
> servizio.

- Una volta inserito il proprio Trusted Shops ID verrà generato
  automaticamente, nel campo sottostante, lo snippet di codice da
  utilizzare per l'integrazione

![](./assets/media/image152.png)

> Sarà quindi necessario, come indicato anche dalle relative istruzioni,
> copiare questo snippet di codice ed inserirlo all'interno del campo
> "**Code Snippet -- FOOTER**" presente nel tab "**Integrazioni**" alla
> pagina "**Sito -- Preferenze**" del Wizard del proprio sito Passweb

![](./assets/media/image153.png)

- Una volta inserito il Trustbadge il passo successivo sarà ora quello
  che prevede di inserire il codice necessario per inviare alla
  piattaforma terza, alla conferma dell'ordine, tutti i dati necessari
  per consentire a Trusted Shops di creare e gestire gli inviti di
  recensione.

> Per fare questo sarà sufficiente portarsi alla pagina "**Ordini --
> Configurazione Ordini**" del Wizard, accedere alla sezione
> "**Documento**" ed inserire all'interno del campo "**Codice
> Completamento**" evidenziato in figura, il segnaposto
> "**TrustedShop**"

![](./assets/media/image154.png)

- L'ultimo passaggio, infine, è quello che prevede di inserire le
  recensioni all'interno del proprio sito Ecommerce.

> In questo senso sarà necessario, per prima cosa, recarsi nel back end
> del proprio account Trusted Shops selezionare, all'interno della
> sezione "**Marketing -- Widget Libreiria**", il widget da utilizzare
> per visualizzare le recensioni, generare quindi il relativo codice di
> integrazione ed inserirlo all'interno del proprio sito Passweb.
>
> In questa fase è bene evidenziare che i widget messi a disposizione da
> Trusted Shop sono di due tipi diversi e a seconda della tipologia
> considerata potranno essere inseriti in una qualsiasi pagina del sito
> o nelle sole pagine prodotto:

- **Recensioni servizio** (es. Carosello di recensioni) -- contengono
  recensioni relative al negozio e possono quindi essere inseriti in una
  qualsiasi pagina del sito

- **Recensioni prodotto** (es. Lista Completa delle recensioni) --
  contengono recensioni relative ai singoli prodotti e dovranno quindi
  essere inseriti nelle sole pagine Prodotto.

> **Questo tipo di widget richiede inoltre l'inserimento di codice
> aggiuntivo necessario per valorizzare dinamicamente il campo
> "data-sku" con il relativo codice articolo presente su Passweb**
>
> Di seguito vengono indicati nel dettaglio i passaggi da seguire per
> integrare all'interno del proprio sito entrambe le tipologie di widget

##### RECENSIONI SERVIZIO -- ES. CAROSELLO DI RECENSIONI

Per inserire questo tipo di widget all'interno del proprio sito Passweb
è necessario, per prima cosa, cliccare sul pulsante "**Configura**"
presente in corrispondenza del widget stesso

![](./assets/media/image155.png)

Nella maschera di configurazione così visualizzata sarà poi necessario
indicare la lingua in cui dovrà essere gestito il widget e cliccare sul
pulsante "**Crea il codice widget**"

![](./assets/media/image156.png)

In questo modo, verrà infatti visualizzato il codice da utilizzare per
l'integrazione, codice questo che, come evidenziato nella figura di
seguito riportata, è strutturato in due diverse parti.

![](./assets/media/image157.png)

La prima (**Inizializzazione**) necessaria per importare la libreria
javascript utilizzata per visualizzare il widget

**ATTENZIONE!** la libreria javascript utilizzata per visualizzare i
diversi widget di Trusted Shop è indipendente dal tipo di widget
considerato e deve quindi essere inserita una sola volta all'interno del
proprio sito

La seconda (**Collega il Widget**) necessaria per definire il
contenitore in cui dovranno poi essere visualizzate le recensioni

Per completare l'integrazione sarà quindi necessario:

- Copiare lo snippet di codice presente nella sezione
  "**Inizializzazione**" ed inserirlo (nel momento in cui non dovesse
  già essere presente) all'interno del campo "**Code Snippet -- HEAD**"
  nel tab "**Integrazioni**" presente alla pagina "**Sito --
  Preferenze**" del Wizard del proprio sito Passweb

![](./assets/media/image158.png)

- Copiare lo snippet di codice presente nella sezione "**Collega il
  Widget**" ed inserirlo, mediante un apposito componente HTML, nelle
  pagine del sito in cui dovrà essere visualizzato il widget

**ATTENZIONE!** Considerando che il tipo di widget in questione conterrà
recensioni generali effettuate in relazione all'intero sito, potrà
essere inserito in una qualsiasi pagina senza ulteriori operazioni.

![](./assets/media/image159.png)

##### RECENSIONI PRODOTTO -- ES. LISTA COMPLETA DELLE RECENSIONI

Per inserire questo tipo di widget all'interno del proprio sito Passweb
è necessario, per prima cosa, cliccare sul pulsante "**Configura**"
presente in corrispondenza del widget stesso

![](./assets/media/image155.png)

Nella maschera di configurazione così visualizzata sarà poi necessario
indicare la lingua in cui dovrà essere gestito il widget e cliccare sul
pulsante "**Crea il codice widget**"

![](./assets/media/image160.png)

In questo modo, verrà infatti visualizzato il codice da utilizzare per
l'integrazione, codice questo che, come evidenziato nella figura di
seguito riportata, è strutturato in diverse parti

![](./assets/media/image161.png)

Una prima parte (**Inizializzazione**) necessaria per importare la
libreria javascript utilizzata per visualizzare il widget

**ATTENZIONE!** la libreria javascript utilizzata per visualizzare i
diversi widget di Trusted Shop è indipendente dal tipo di widget
considerato e deve quindi essere inserita una sola volta all'interno del
proprio sito

Un'altra parte (**Collega il Widget**) necessaria per definire invece il
contenitore in cui dovranno poi essere visualizzate le recensioni.

Nel caso del widget "Lista Completa delle recensioni" è presente anche
una terza parte (**Estensioni del widget**) dovuta alla particolare
struttura di questo componente.

![](./assets/media/image162.png)

La "Lista Completa delle recensioni" infatti è un widget che conterrà le
recensioni dello specifico articolo, che dovrà essere inserito
all'interno della specifica pagina prodotto e che potrà essere composto
da due distinti elementi:

- L'elenco completo delle recensioni, tipicamente posizionato nella
  parte bassa della pagina prodotto.

![](./assets/media/image163.png)

> Lo snippet di codice necessario per visualizzare questo elemento è
> quello presente in corrispondenza della sezione "Collega il tuo
> widget"

- Una piccola anteprima delle stelle che riassumono la valutazione
  complessiva del prodotto.

![](./assets/media/image164.png)

> Questo elemento potrà essere posizionato in una qualunque parte della
> pagina prodotto e conterrà un collegamento diretto all'elenco completo
> delle recensioni.
>
> Lo snippet di codice necessario per visualizzare questo elemento è
> quello presente in corrispondenza della sezione "Estensioni del
> widget"

Per completare l'integrazione sarà quindi necessario:

- Copiare lo snippet di codice presente nella sezione
  "**Inizializzazione**" ed inserirlo (nel momento in cui non dovesse
  già essere presente) all'interno del campo "**Code Snippet -- HEAD**"
  nella sezione "**Integrazioni**" presente alla pagina "**Sito --
  Preferenze**" del Wizard del proprio sito Passweb

![](./assets/media/image158.png)

- Copiare lo snippet di codice presente nella sezione "**Collega il
  Widget**" ed inserirlo, mediante un apposito componente HTML,
  all'interno della pagina prodotto nella sezione in cui dovrà essere
  effettivamente visualizzato l'elenco completo delle recensioni
  prodotto

> **ATTENZIONE! In questa fase è di fondamentale importanza sostituire
> nello snippet di codice prelevato da Trusted Shops il valore presente
> per l'attributo "data-sku" con il segnaposto Passweb {{SKU}}**

![](./assets/media/image165.png)

> Solo in questo modo potremmo infatti avere la certezza che l'attributo
> in esame venga valorizzato per ogni prodotto con il valore corretto e
> che le recensioni visualizzate siano effettivamente quelle relative al
> prodotto attualmente visualizzato sul sito Ecommerce dai singoli
> utenti

- Copiare lo snippet di codice presente nella sezione "**Estensione del
  Widget**" ed inserirlo, sempre nella pagina prodotto e sempre con un
  apposito componente HTML, nel punto in cui dovrà poi essere
  visualizzata l'anteprima delle stelline che riassumono la valutazione
  complessiva dell'articolo

**ATTENZIONE!** il processo di integrazione del widget "Mini Stelle" è
del tutto analogo a quello appena analizzato. L'unica differenza è
rappresentata dal fatto che, vista la tipologia di elemento, questo
widget andrà inserito nelle celle articolo di componenti quali il
"Catalogo Ecommerce" le "Offerte / Novità" ...

##### SISTEMA DI RECENSIONI E GARANZIA DI RIMBORSO

Dopo aver completato l'integrazione tra il proprio sito Passweb e la
piattaforma di Trusted Shop secondo quanto indicato nei precedenti
capitoli di questo manuale, in una qualsiasi pagina del sito verrà
visualizzato il Trustbadge, un piccolo bollino posto tipicamente nella
parte bassa, utile per informare gli utenti relativamente al fatto che
il sito Ecommerce aderisce al relativo circuito

![](./assets/media/image166.png)

Cliccando su questo badge sarà possibile accedere a maggiori
informazioni relativamente alla certificazione Trusted Shops, alla
garanzia di rimborso inclusa e alla valutazione complessiva del sito

![](./assets/media/image167.png)

Una volta completato un ordine, nella pagina di conferma dell'acquisto,
il Trustbadge mostrerà automaticamente informazioni relative
all'assicurazione e alla garanzia di rimborso offerte all'utente
direttamente da Trusted Shop

![](./assets/media/image168.png)

In questa fase inoltre verranno inviate alla piattaforma terza tutte le
informazioni relative all'ordine appena concluso e necessarie per poter
consentire a Trusted Shop di attivare tutto il suo sistema di recensioni
verificate.

L'esercente potrà quindi trovare nell'applicazione di back end del
proprio account Trusted Shops (sezione **Inviti**) un nuovo invito
generato appunto a seguito dell'ordine appena concluso sul sito
Ecommerce

![](./assets/media/image169.png)

A questo punto Trusted Shop provvederà ad inviare all'acquirente,
secondo le regole definite sulla piattaforma stessa, due diverse mail,
una contenente informazioni relative alla garanzia di rimborso, garanzia
questa che, come già detto, sarà gestita interamente da Trusted Shops

![](./assets/media/image170.png)

L'altra contenente invece un invito a recensire l'acquisto effettuato
all'interno del sito Ecommerce

![](./assets/media/image171.png)

**ATTENZIONE!** Nel momento in cui si dovesse decidere di spedire gli
inviti di recensione in maniera automatica a seguito di ogni ordine,
sarà necessario indicare, nelle condizioni di privacy del proprio sito,
che alla conclusione dell' ordine l'indirizzo mail del cliente verrà
condiviso con la piattaforma Trusted Shops e che l'utente riceverà
apposite mail di invito alla recensione.

Volendo è anche possibile disabilitare l'invio automatico delle mail di
invito agendo per questo dal back end del proprio account Trusted Shops.

**ATTENZIONE!** Eventuali modifiche apportate in questo senso saranno
però valide solo per eventuali utenti non ancora presenti nel database
di Trusted Shops.

**In ogni caso è responsabilità dell'esercente verificare direttamente
con Trusted Shops, il funzionamento dei relativi parametri di
configurazione e con il proprio responsabile privacy cosa dover
effettivamente inserire nei termini e condizioni del proprio sito in
maniera tale da essere compliance con quanto richiesto dal GDPR**

Una volta ricevuto l'invito alla recensione cliccando sul pulsante
"Valuta Ora" presente all'interno della mail, l'utente verrà ricondotto
sul front end della piattaforma Trusted Shops dove potrà portare a
termine la propria recensione relativa sia al sito su cui è stato
effettuato l'acquisto che ai singoli prodotti presenti in ordine

![](./assets/media/image172.png)

![](./assets/media/image173.png)

La recensione effettuata farà cambiare stato al relativo invito presente
nel back end esercente di Trusted Shops

![](./assets/media/image174.png)

e, nel momento in cui dovessero essere stati inseriti dei widget
all'interno del proprio sito Ecommerce questa stessa recensione sarà
disponibile e visibile anche nelle relative pagine del sito stesso

![](./assets/media/image163.png)

