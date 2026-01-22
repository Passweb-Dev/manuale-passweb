# SINCRONIZZAZIONE DATI



Considerando che, come detto, il motore di Clerk.io si basa interamente
sui dati raccolti dal sito e-commerce, uno step fondamentale per tutto
il processo di integrazione è indubbiamente quello che riguarda il modo
in cui i dati del sito Passweb (articoli, ordini, clienti ...) potranno
effettivamente essere condivisi con Clerk

In questo senso va detto che lo scambio di informazioni tra le due
piattaforme avverrà in modi e in tempi diversi. Nello specifico:

- **attraverso apposite chiamate API**

- **attraverso la creazione di appositi feed**

Nel primo caso va detto che, relativamente alle informazioni inviate a
Clerk mediante apposite chiamate API (quindi lato server al verificarsi
di determinati eventi) queste riguarderanno nello specifico:

- gli ordini effettuati all'interno del sito successivamente
  all'attivazione e alla configurazione del modulo Clerk

- gli articoli coinvolti negli ordini effettuati all'interno del sito
  successivamente all'attivazione e alla configurazione del modulo Clerk

- i clienti che si registreranno sul sito, anche in questo caso,
  successivamente all'attivazione e alla configurazione del modulo Clerk

Per quel che riguarda invece i dati che le due piattaforme si
scambieranno mediante feed, Passweb si preoccuperà di generare dei feed
distinti (per Ordini, Clienti. Articoli, Categorie Merceologiche e
Pagine) che verranno esposti su di un determinato URL in maniera tale
che Clerk possa poi andarli a leggere, ad intervalli di tempo regolari,
mantenendo così le due piattaforme allineate.

Tali feed potranno o meno essere generati in maniera automatica ad ogni
sincronizzazione Sito -- Gestionale, conterranno tutte i dati
obbligatori richiesti da Clerk e, a seconda dello specifico feed,
potranno eventualmente essere integrati anche con informazioni
aggiuntive (maggiori saranno i dati che condivideremo con Clerk,
migliori saranno i risultati prodotti dai suoi algoritmi di intelligenza
artificiale)

Chiaramente all'interno di questi file potranno essere presenti
informazioni "sensibili" come nome, cognome, indirizzo mail, prodotti
acquistati ecc... per cui l'invio di questi dati dovrà essere, sicuro,
ed effettuato in maniera conforme a quanto richiesto dal GDPR.

Dal punto di vista della sicurezza Passweb gestisce la Token
Authentication di Clerk (
<https://help.clerk.io/it/integrations/any-webshop/data-feeds/> ) per
cui **i feed creati potranno effettivamente essere consumati solo a
seguito di connessioni crittografate (il sito dovrà quindi essere dotato
di certificato SSL) e solo se la richiesta arriva effettivamente da
Clerk**.

In altre parole richiamando l'url di un feed inserendolo semplicemente
nella barra degli indirizzi del browser verrà ritornato un errore 401 e
i dati del feed non verranno quindi mai visualizzati.

In queste condizioni, come detto, sarà comunque Clerk che dovrà andare a
leggersi i feed prodotti da Passweb per cui occorrerà configurare il
proprio store in maniera tale che tutto ciò possa avvenire
correttamente.

Per far questo è necessario agire dal menu "**Data -- Configuration**"
dello store con cui si desidera effettuare l'integrazione.

![](./assets/media/image10.png)

I campi presenti all'interno della sezione "**Data sync settings**"
evidenziata in figura dovranno essere impostati come di seguito
indicato:

- **Sync Method**: consente di impostare il metodo di sincronizzazione
  utilizzato da Clerk per importare i dati dal sito Ecommerce.

> Nel caso specifico dovrà quindi essere impostato sull'opzione
> "**Clerk.io JSON Feed V2**"

- **JSON Products URL**: consente di specificare l'url su cui verrà
  esposto il feed Articoli che Clerk dovrà poi andare a leggersi

> All'interno di questo campo dovrà quindi essere inserito l'url
> indicato in corrispondenza del campo "**URL Feed**" presente, su
> Passweb, all'interno del tab "**Articoli**" della maschera "**Dati
> Account**"

- **JSON Categories** **URL**: consente di specificare l'url su cui
  verrà esposto il feed delle Categorie Merceologiche che Clerk dovrà
  poi andare a leggersi

> All'interno di questo campo dovrà quindi essere inserito l'url
> indicato in corrispondenza del campo "**URL Feed**" presente, su
> Passweb, all'interno del tab "**Categorie**" della maschera "**Dati
> Account**"

- **JSON Orders URL**: consente di specificare l'url su cui verrà
  esposto il feed Ordini che Clerk dovrà poi andare a leggersi

> All'interno di questo campo dovrà quindi essere inserito l'url
> indicato in corrispondenza del campo "**URL Feed**" presente, su
> Passweb, all'interno del tab "**Ordini**" della maschera "**Dati
> Account**"

- **JSON Customers** **URL**: consente di specificare l'url su cui verrà
  esposto il feed Clienti che Clerk dovrà poi andare a leggersi

> All'interno di questo campo dovrà quindi essere inserito l'url
> indicato in corrispondenza del campo "**URL Feed**" presente, su
> Passweb, all'interno del tab "**Clienti**" della maschera "**Dati
> Account**"

- **JSON Pages** **URL**: consente di specificare l'url su cui verrà
  esposto il feed Pagine che Clerk dovrà poi andare a leggersi

> All'interno di questo campo dovrà quindi essere inserito l'url
> indicato in corrispondenza del campo "**URL Feed**" presente, su
> Passweb, all'interno del tab "**Pagine**" della maschera "**Dati
> Account**"

- **Paging size {{limit}}**: consente di indicare il valore di un
  parametro, che dovrebbe poi essere inserito anche in query string agli
  url dei vari feed, e che può consentire a Clerk di prelevare i dati
  dei feed stessi utilizzando una sorta di paginazione.

> Attualmente Passweb non gestisce questa funzionalità per cui il campo
> in oggetto (che è comunque un campo opzionale) può essere lasciato
> vuoto

- **Incremental time {{modified_after}}**: consente di indicare il
  valore di un parametro, che dovrebbe poi essere inserito anche in
  query string agli url dei vari feed, e che potrebbe consentire a Clerk
  di ragionare, in fase di importazione dei dati presenti all'interno di
  questi stessi feed, per differenza.

> **ATTENZIONE! Passweb attualmente non gestisce questa funzionalità per
> cui il campo in esame DEVE essere lasciato vuoto**
>
> **In queste condizioni eventuali elementi (articoli, clienti,
> categorie, pagine) non più presenti nei relativi feed, in fase di
> importazione dati verranno automaticamente eliminati anche dal
> database di Clerk**
>
> Nel momento in cui l'esigenza dovesse essere, ad esempio, quella di
> eliminare da Clerk un determinato articolo sarà quindi sufficiente
> fare in modo di non farlo più comparire nel feed generato da Passweb e
> la prossima volta che Clerk andrà a leggere tale feed non trovando il
> prodotto lo eliminerà anche dal suo database.
>
> **L'unica eccezione in questo senso, è rappresentata dal feed
> Ordini**. Una volta che un determinato ordine è stato correttamente
> importato in Clerk, infatti, questo resterà sulla piattaforma
> indipendentemente dal fatto che sia o meno presente anche nel relativo
> feed che Clerk stesso andrà di volta in volta a leggere (assieme
> all'ordine su Clerk resterà sempre anche il cliente intestatario)
>
> Il parametro Incremental time {{modified_after}} servirebbe proprio a
> modificare questo comportamento di default, presupponendo però da una
> parte che il feed json venga creato "al volo", quando cioè è Clerk
> stesso a richiederlo, e dall'altra parte che contenga solamente i dati
> che sono effettivamente cambiati negli ultimi N giorni dove N è
> proprio il valore che dovrebbe essere inserito in questo campo.
>
> Valorizzare il parametro in esame equivarrebbe infatti a dire a Clerk
> di smettere di eliminare automaticamente dal proprio database gli
> oggetti non più presenti in un determinato feed e di limitarsi invece
> solamente ad aggiornare o a inserire quegli oggetti che, nel feed che
> sta processando, sono effettivamente presenti.
>
> Ora, considerando che Passweb genera i vari feed non quando richiesto
> da Clerk ma alla sincronizzazione Sito -- Gestionale, o al limite
> manualmente dietro specifica richiesta dell'utente, e che lo fa
> considerando sempre tutta la base dati del sito e non solo quelli che
> sono gli articoli, i clienti, le categorie merceologiche ... che sono
> state effettivamente modificate negli ultimi N giorni, valorizzare il
> parametro in esame porterebbe da una parte ad aggiornare, ad esempio,
> sempre e comunque tutti gli articoli che vogliamo effettivamente
> gestire su Clerk, indipendentemente dal fatto che siano o meno stati
> variati negli ultimi N giorni, e dall'altra parte a non avere più un
> modo per eliminare invece quei prodotti che non dovrebbero più essere
> gestiti su Clerk.

- **Enable Token Authentication:** come precedentemente evidenziato
  Passweb gestisce la Token Authentication di Clerk e i feed prodotti
  possono effettivamente essere consumati solo a seguito di connessioni
  crittografate (il sito dovrà quindi essere dotato di certificato SSL)
  e solo se la richiesta arriva effettivamente da Clerk per cui il
  parametro in esame dovrà essere impostato sull'opzione Si

- **Sync Time:** consente di impostare un intervallo orario entro il
  quale Clerk dovrà andare a prelevare i vari feed. Scegliendo un orario
  specifico la sincronizzazione verrà eseguita solo all'interno di quel
  lasso di tempo (in ora UTC) cosa questa che può essere utile per
  ridurre il carico che l'operazione potrebbe avere sul sito
  localizzandola in un momento (es. la notte) in cui si presume che
  eventuali picchi non provocherebbero comunque problemi di alcun tipo.

> Lasciando invece il campo impostato su "**When Needed (Recommended)**"
> sarà Clerk stesso a decidere come e quando eseguire questa
> sincronizzazione in base al tempo impiegato per portare a termine il
> processo. Se ad esempio tutto il processo impiegasse meno di 10 minuti
> la sincronizzazione potrebbe anche essere eseguita ogni ora, per
> contro sincronizzazioni che dovessero impiegare più di 60 minuti
> potrebbero essere eseguite una sola volta al giorno.

- **Import Products/Categories/Orders/Customers/Pages:** consente di
  decidere quali feed dovranno essere effettivamente processati da Clerk
  alla sincronizzazione.

> **Tipicamente questi parametri dovrebbero essere tutti impostati a
> Si**

Per maggiori informazioni relativamente ai vari parametri di
sincronizzazione impostabili all'interno del proprio account Clerk si
consiglia di fare sempre riferimento alla relativa documentazione di
prodotto consultabile, ad esempio, ai seguenti link
<https://help.clerk.io/it/platform/data/sync/> -
<https://help.clerk.io/it/integrations/any-webshop/data-feeds/>

Per maggiori informazioni relativamente a come poter invece generare
all'interno di Passweb i vari feed si vedano i successivi capitoli di
questo manuale

