# FUNZIONALITA MEXAL -- CLIENTI



Come già visto per le Funzionalità Mexal Articolo allo stesso modo anche
per i clienti una volta selezionate e attivate, secondo quanto indicato
nei precedenti capitoli di questo manuale, le specifiche Funzionalità
Mexal sarà poi necessario portarsi nell'anagrafica del singolo utente e
valorizzare i nuovi campi aggiuntivi secondo le proprie specifiche
esigenze.

In questo senso, dunque, portandosi nell'anagrafica di un cliente e
cliccando sul pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)**

![](./assets/media/image71.png)

verrà visualizzata la relativa maschera contenente l'elenco di tutte le
videate aggiuntive clienti/fornitori attualmente presenti.

![](./assets/media/image72.png)

Selezionando quella relativa al sito su cui si desidera operare (il nome
della videata coincide con il nome assegnato al sito, nella sua
anagrafica, in fase di attivazione) e cliccando sul pulsante
**"Seleziona" (Invio)** verrà visualizzata la maschera **"Nome Sito"**
con al suo interno i campi della videata aggiuntiva/articoli
appositamente riservata per quello specifico sito e corrispondenti alle
sole Funzionalità Mexal effettivamente attivate.

![](./assets/media/image73.png)

> **NOTA BENE :**per maggiori informazioni relativamente all'attivazione
> delle specifiche "Funzionalità Mexal" si veda anche il capitolo
> "Configurazione Gestionale -- Attivazione Passweb" di questo manuale.

A questo punto quindi si tratterà di valorizzare i singoli campi
presenti all'interno di questa maschera secondo quanto richiesto dalla
specifica funzionalità.

Di seguito verranno esaminate nel dettaglio le singole funzionalità
cliente gestibili attraverso la maschera sopra evidenziata.

##### ESPORTAZIONE / ELIMINAZIONE DI CLIENTI MEXAL ALL'INTERNO DEL SITO E-COMMERCE

Oltre agli articoli è possibile esportare all'interno del sito Ecommerce
anche le anagrafiche di utenti che sono già presenti sul gestionale
Passepartout abilitandoli immediatamente all'acquisto via web.

**ATTENZIONE!** per abilitare gli utenti che sono già presenti sul
gestionale Passepartout ad effettuare acquisti sul sito **NON**
**utilizzare la pagina di registrazione**, ma esportare questi stessi
utenti direttamente dal gestionale Passepartout, assegnando loro una
login e una password.

Per poter decidere quali clienti Mexal esportare e gestire all'interno
de sito e-commerce è necessario rifarsi alla "Funzionalità Mexal"
**"Cliente/Fornitore sul sito".**

![](./assets/media/image74.png)

> **NOTA BENE:** per maggiori informazioni relativamente
> all'attivazione/disattivazione delle Funzionalità Mexal si veda anche
> quanto indicato all'interno del capitolo "Configurazione Gestionale --
> Attivazione Passweb" di questo manuale.

Come precedentemente evidenziato tale funzionalità attiva infatti, nella
videata aggiuntiva clienti/fornitori appositamente riservata per lo
specifico sito, un particolare campo, **"Trasferisci sul sito"**,
attraverso il quale poter decidere se lo specifico cliente dovrà o meno
essere esportato e gestito anche all'interno del sito web.

![](./assets/media/image75.png)

> **NOTA BENE:** la Funzionalità Mexal **"Cliente/Fornitore sul sito"**
> è impostata a default sul valore **S** e **tale valore non potrà
> essere modificato**. In conseguenza di ciò il campo **"Trasferisci sul
> sito" sarà sempre presente all'interno della maschera "Dati Passweb"**
> e non potrà mai essere eliminato.

Per poter dunque esportare e gestire all'interno del sito web un cliente
Mexal occorre:

1.  Verificare di aver predisposto, **in relazione allo specifico sito
    su cui si intende operare**, la struttura dati utilizzata per
    gestire le "Funzionalità Mexal", e di aver quindi impostato a
    **Si**, nell'anagrafica del sito stesso, il parametro **"E-Commerce
    Attivo"**

![](./assets/media/image25.png)

2.  Portarsi nell'anagrafica Mexal del cliente desiderato, cliccare sul
    pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e
    selezionare, tra quelle presenti in elenco, la videata aggiuntiva
    articoli relativa allo specifico sito su cui si intende operare.

![](./assets/media/image76.png)

3.  Impostare all'interno della successiva maschera il campo
    **"Trasferisci sul sito"** sul valore **S (gestito all'interno del
    sito)**

![](./assets/media/image75.png)

> **NOTA BENE:** dopo aver impostato per ogni singolo cliente Mexal il
> valore desiderato per il campo "Trasferisci sul sito", è di
> fondamentale importanza lanciare una sincronizzazione in modo tale da
> consentire a Passweb di .prelevare da Mexal tutti quei clienti che si
> è deciso di gestire e di esportare all'interno del proprio sito
> e-commerce.

Nel caso in cui invece si decida di eliminare e di non gestire più
all'interno del proprio sito e-commerce determinati clienti, fino a quel
momento correttamente gestiti, sarà sufficiente impostare per essi, in
Mexal, il campo **"Trasferisci sul Sito"**, sopra evidenziato, sul
valore **N** e lanciare poi una nuova sincronizzazione.

In definitiva dunque impostando il campo **"Trasferisci sul sito"** sul
valore:

- **S:** alla successiva sincronizzazione il cliente in esame verrà
  esportato all'interno del sito e-commerce; da questo momento in poi
  potrà quindi essere gestito all'interno del sito e potrà,
  autenticandosi con le proprie credenziali, effettuare acquisti via
  web.

- **N:** alla successiva sincronizzazione il cliente in esame, fino a
  quel momento correttamente gestito all'interno del sito e-commerce,
  verrà eliminato e da questo momento, quindi, non potrà più
  autenticarsi ne tanto meno effettuare acquisti all'interno del sito.

> **NOTA BENE:** nel caso in cui il campo **"Trasferisci sul sito" sia
> lasciato vuoto** verrà assunto per esso a default il valore **N** e il
> cliente non verrà quindi considerato tra quelli gestiti all'interno
> del sito.

Per quel che riguarda infine le credenziali di accesso al sito (Nome
Utente e Password), queste verranno gestite, in generale, mediante gli
appositi campi presenti all'interno della videata aggiuntiva
clienti/fornitori **riservata allo specifico sito** **su cui si sta
operando**, e collegati alle relative "Funzionalità Mexal" **"Gestione
Login -- Utente"** e **"Gestione Login -- Password".**

Tali funzionalità attivano nella videata aggiuntiva clienti/fornitori
riservata allo specifico sito due campi, **"Login: Utente"** e **"Login:
Password"**, attraverso i quali poter gestire le credenziali di accesso,
al relativo sito, per il cliente in esame.

![](./assets/media/image77.png)

> **NOTA BENE:** le Funzionalità Mexal **"Gestione Login -- Utente" e
> "Gestione Login -- Password"** sono impostate a default sul valore
> **S** e **tale valore non potrà essere modificato**. In conseguenza di
> ciò i campi **"Gest. Login: Utente"** e **"Gest. Login: Password"**,
> **saranno sempre presenti all'interno della maschera "E-Commerce"** e
> non potranno mai essere eliminati.

In particolare dunque all'interno del campo

- **Login Utente**: andrà inserito lo Username che l'utente dovrà
  utilizzare per effettuare l'accesso al sito

- **Password Utente**: andrà inserita la password di accesso al sito

Per quel che riguarda la login utente occorre poi sottolineare che nel
caso di:

- **esportazione sul sito di un nuovo utente, già presente tra le
  anagrafiche del gestionale**: prima di effettuare l'esportazione sarà
  ovviamente necessario assegnare un valore al relativo campo e,
  successivamente, comunicarlo all'utente che ne dovrà far uso

- **registrazione web di un nuovo utente**: il dato presente all'interno
  di questo campo verrà inserito alla sincronizzazione direttamente da
  Passweb e coinciderà con quanto indicato dall'utente stesso in fase di
  registrazione al sito

- **variazione dell'anagrafica utente sul sito:** nel momento in cui un
  utente già esportato e gestito all'interno del sito dovesse agire
  dalla pagina del suo profilo per modificare la login di accesso, alla
  successiva sincronizzazione anche il campo Mexal "Login Utente" verrà
  correttamente aggiornato

Per quel che riguarda invece la password di accesso nel caso di:

- **esportazione sul sito di un nuovo utente, già presente tra le
  anagrafiche del gestionale**: come per la login, anche in questo caso
  prima di effettuare l'esportazione sarà necessario assegnare
  all'utente una specifica password e, successivamente, comunicargliela.

> **ATTENZIONE! Una volta arrivata sul sito, per ragioni di privacy, la
> password verrà opportunamente crittografata e, da questo momento in
> avanti, sarà gestita solo ed esclusivamente all'interno del sito**
>
> Ciò significa dunque che nel momento in cui l'utente dovesse andare a
> modificare, dal proprio profilo, la password di accesso al sito, il
> nuovo valore resterà memorizzato, opportunamente crittografato, solo
> sul database di Passweb e NON verrà quindi riportato nel campo
> "Password Utente" di Mexal

- **registrazione web di un nuovo utente:** coerentemente con quanto
  indicato per il punto precedente, la password dei nuovi utenti che si
  sono registrati al sito resterà memorizzata, opportunamente
  crittografata, solo sul database di Passweb e NON verrà quindi mai
  riportata nel campo "Password Utente" di Mexal

##### GESTIONE MINIMO D'ORDINE

La "Funzionalità Mexal" **"Gestione Minimo Ordine"** consente di
attivare una particolare modalità di gestione a seguito della quale sarà
possibile specificare, per ogni singolo cliente, il valore minimo del
totale merce che lo stesso cliente dovrà necessariamente superare per
poter confermare l\'ordine.

**ATTENZIONE!** il Totale Merce utilizzato come base di calcolo, sarà
considerato comprensivo o meno di eventuali articoli spesa inserti in
carrello (a seguito dell'applicazione di determinate promozioni o buoni
sconto) dipendentemente dall'impostazione scelta per il parametro
"**Gestione Totale Merce**" presente nella sezione "*Catalogo --
Configurazione Parametri Catalogo*" del Wizard

**Per poter adottare questa particolare modalità di gestione sarà quindi
necessario attivare lato gestionale la Funzionalità Mexal "Gestione
Minimo Ordine".**

Una volta preparata dunque, all'interno del gestionale, la struttura
dati utilizzata per gestire le "Funzionalità Mexal", secondo quanto
descritto nel capitolo "Attivazione Passweb" di questo manuale, sarà poi
necessario richiamare la maschera **"Configurazione gestione dati web
cliente/fornitore"** qui di seguito riportata, e flaggare il campo
**"Gestione Minimo Ordine".**

![](./assets/media/image78.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati web
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for"** **(F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, il campo **Minimo Ordine Merce**
corrispondente alla "Funzionalità Mexal" precedentemente attivata.

![](./assets/media/image79.png)

A questo punto quindi occorrerà selezionare i clienti Mexal gestiti
all'interno del sito relativamente ai quali si vuole attivare questa
funzionalità e valorizzare il campo della videata aggiuntiva sopra
evidenziato **con il valore minimo del totale merce che essi dovranno
superare per poter effettivamente confermare un ordine all'interno del
sito**.

> **NOTA BENE:** nel caso in cui il campo in oggetto non venga
> valorizzato, il relativo cliente non sarà sottoposto ad alcun minimo
> d'ordine e potrà quindi effettuare ordini via web indipendentemente
> dal valore del loro totale merce .
>
> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni cliente gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.

Attivando questa funzionalità, dunque, sul sito web, se al cliente non è
stato assegnato nessun minimo d\'ordine (caso in cui per la videata
aggiuntiva in esame non sia stato impostato alcun valore o il valore 0)
lo stesso cliente potrà effettuare l\'ordine senza alcun vincolo sul
totale merce; nel caso in cui invece al cliente sia stato assegnato uno
specifico minimo d\'ordine se il totale merce risulterà inferiore a tale
valore il cliente non potrà confermare l\'ordine e gli verrà
visualizzato un messaggio per informarlo che non ha raggiunto un certo
valore minimo.

Il messaggio in questione è personalizzabile alla pagina "**Gestione
Testi/Messaggi del Sito**" del Wizard, in corrispondenza del componente
"**Checkout Custom**".

![](./assets/media/image80.png)

> **NOTA BENE:** la stringa {minorder} verrà sostituita dal valore del
> minimo d'ordine. Tale stringa non deve quindi essere alterata o
> variata in alcun modo.
>
> **NOTA BENE:** nel caso in cui in Mexal, nelle condizioni commerciali
> di uno specifico cliente, sia stato impostato il campo \"Fatturare
> A\", l\'eventuale minimo d\'ordine verrà gestito in relazione
> all\'utente destinatario della fattura**.**

Infine, volendo, è anche possibile impostare un minimo d'ordine di
"default" che verrà automaticamente applicato a tutti gli utenti del
sito per i quali non è stato specificatamente indicato un mimino
d'ordine all'interno di Mexal (compresi quindi i nuovi utenti che hanno
appena effettuato la registrazione e che non sono ancora presenti nelle
anagrafiche del gestionale).

Tale possibilità va attivata direttamente all'interno di Passweb agendo
per questo sul parametro "**Minimo Ordine**" presente nella sezione
"**Utenti -- Gestione Parametri Utenti Ecommerce -- Configurazione
Utenti**" del Wizard.

Per maggiori informazioni in merito si veda anche il relativo capitolo
di questo manuale.

##### ABILITAZIONE ACCESSO AREA RISERVATA

La "Funzionalità Mexal" **"Abilita all'area riservata"** consentirà, se
attivata, di decidere, per ciascuno dei clienti correttamente esportati
e gestiti sul sito, quali di essi potranno anche accedere all'Area
Riservata potendo quindi sfruttare tutte le funzionalità messe a
disposizione da questa specifica sezione del sito E-commerce.

Tipicamente tale funzionalità dovrà essere attivata e gestita nel caso
in cui il sito E-commerce che si intende realizzare sia di tipo Business
to Business. All'interno dell'Area Riservata di un sito E-commerce sarà
infatti possibile stabilire diversi livelli di comunicazione tra Agenti
e Clienti Mexal opportunamente abilitati.

Per poter attivare questa funzionalità sarà quindi necessario, una volta
preparata all'interno del gestionale, la struttura dati utilizzata per
gestire le "Funzionalità Mexal" (secondo quanto descritto nel capitolo
"Attivazione Passweb" di questo manuale) richiamare la maschera
**"Configurazione gestione dati web cliente/fornitore"** qui di seguito
riportata, e flaggare il campo **"Abilita all'area riservata".**

![](./assets/media/image81.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati web
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for"** **(F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, il campo "**Abil. Area Riservata"**
corrispondente alla "Funzionalità Mexal" precedentemente attivata.

![](./assets/media/image82.png)

A questo punto quindi occorrerà selezionare tra i clienti Mexal gestiti
all'interno del sito quelli ai quali si vuole concedere l'accesso
all'Area Riservata e valorizzare per essi il campo della videata
aggiuntiva sopra evidenziato a **S**.

> **NOTA BENE:** nel caso in cui il campo in oggetto non venga
> valorizzato, il relativo cliente non avrà accesso all'Area Riservata .
>
> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni cliente gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.

Nel momento in cui dunque un cliente per il quale è stata attivata la
funzionalità in oggetto andrà ad autenticarsi sul sito E-commerce verrà
automaticamente ricondotto al pannello dell'Area Riservata, dove avrà a
disposizioni diverse funzionalità coerenti con il suo ruolo di Cliente.

**ATTENZIONE! La funzionalità Mexal appena analizzata ha effetto
solamente per i clienti. Nel caso di siti B2B per consentire ad un
Agente Mexal di accedere all'Area Riservata del sito E-commerce sarà
sufficiente esportare e gestire questo stesso agente all'interno del
sito (per maggiori informazioni in merito si veda anche la sezione
*"Utenti -- Utenti Area Riservata"* di questo manuale)**

> **NOTA BENE:** nel momento in cui un Agente Mexal correttamente
> esportato andrà ad autenticarsi sul sito, utilizzando le credenziali
> di accesso che gli sono state assegnate in Mexal, verrà
> automaticamente ricondotto al pannello dell'Area Riservata
> indipendentemente da quanto impostato per esso all'interno del campo
> "Abil. Area Riservata".

##### BLOCCO ORDINE

La "Funzionalità Mexal" **"Blocco Ordine"** consente di attivare una
particolare modalità di gestione a seguito della quale sarà poi
possibile inibire ai clienti la possibilità di effettuare ordini via
web.

Tale funzionalità potrebbe essere utilizzata, ad esempio, nel momento in
cui un cliente dovesse andare fuori fido e, conseguentemente, si
vorrebbe bloccare a questo stesso cliente la possibilità di effettuare
ordini via web.

> **NOTA BENE:** le ragioni per cui bloccare ad un cliente la
> possibilità di effettuare ordini via web potrebbero essere le più
> svariate (non solo il fatto che il cliente sia andato fuori fido), per
> cui su questo campo non è gestito, lato Mexal, nessun automatismo.

**Per poter adottare questa particolare modalità di gestione sarà quindi
necessario attivare lato gestionale la Funzionalità Mexal "Blocco Ordine
se fuori fido".**

Una volta preparata dunque, all'interno del gestionale, la struttura
dati utilizzata per gestire le "Funzionalità Mexal", secondo quanto
descritto nel capitolo "Attivazione Passweb" di questo manuale, sarà poi
necessario richiamare la maschera **"Configurazione gestione dati web
cliente/fornitore"** qui di seguito riportata, e flaggare il campo
**"Blocco Ordine".**

![](./assets/media/image83.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati web
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for"** **(F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, il campo **"Blocco Ordine"**
corrispondente alla "Funzionalità Mexal" appena attivata.

![](./assets/media/image84.png)

A questo punto quindi occorrerà selezionare i clienti Mexal gestiti
all'interno del sito relativamente ai quali si vuole attivare questa
funzionalità e impostare il campo della videata aggiuntiva sopra
evidenziato a **S**.

> **NOTA BENE:** nel caso in cui il campo in oggetto non venga
> valorizzato, il relativo cliente non sarà sottoposto ad alcun blocco,
> potendo quindi continuare ad effettuare ordini via web.
>
> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni cliente gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.

Attivando questa funzionalità per uno specifico cliente dunque, nel caso
in cui questo stesso cliente tenti di effettuare un nuovo ordine, gli
verrà visualizzato, **in fase di check out**, un messaggio per
informarlo dell'impossibilità da parte sua di effettuare nuovi ordini.

**ATTENZIONE!** abilitando la funzionalità di "Blocco Ordine" per uno
specifico cliente, questo stesso cliente potrà comunque effettuare il
login al sito, entrare in Area Riservata (se opportunamente abilitato),
mettere articoli in carrello ecc**... L'effettivo blocco avverrà quindi
solo ed esclusivamente in fase di checkout Ordine**.

La stessa cosa avverrà anche nel momento in cui dovesse essere un Agente
a tentare di effettuare l'ordine per un cliente con il blocco ordini
attivo. L'Agente potrà quindi impersonificare il cliente e accedere a
tutte le sezioni del sito, quando però tenterà di chiudere un ordine per
quel cliente anche a lui verrà mostrato lo stesso messaggio di blocco
ordini

##### BLOCCA MODIFICA SCONTO

La "Funzionalità Mexal" **"Blocca Modifica Sconto"** consente di
attivare una particolare modalità di gestione a seguito della quale sarà
possibile decidere, per ogni singolo Agente, se questo potrà essere o
meno abilitato alla modifica degli sconti all'interno del sito.

> **NOTA BENE:** tale funzionalità è da considerarsi, ovviamente, in
> relazione ai soli siti di tipo B2B o Misto. Gli unici utenti
> eventualmente in grado, infatti, di modificare gli sconti all'interno
> del sito, potranno essere gli Agenti.

**Per poter adottare questa particolare modalità di gestione sarà quindi
necessario attivare lato gestionale la Funzionalità Mexal "Blocca
Modifica Sconto".**

Una volta preparata dunque, all'interno del gestionale, la struttura
dati utilizzata per gestire le nuove "Funzionalità Mexal", secondo
quanto descritto nel capitolo "Attivazione / Disattivazione Delle
Funzionalità Mexal" di questo manuale, sarà poi necessario richiamare la
maschera **"Configurazione gestione dati web cliente/fornitore"** qui di
seguito riportata, e flaggare il campo **"Blocca Modifica Sconto".**

![](./assets/media/image85.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati web
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for"** **(F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, il campo **"Blocca Modif. Sconto"**
corrispondente alla "Funzionalità Mexal" precedentemente attivata.

![](./assets/media/image86.png)

> **NOTA BENE:** il campo "Blocca Modif. Sconto" comparirà sia nelle
> anagrafiche dei conti di tipo Cliente che in quelle di tipo Fornitore.
> **Ovviamente ai fini del sito tale campo verrà considerato, e
> conseguentemente verrà attivata la relativa funzionalità, solo ed
> esclusivamente per i conti di tipo Fornitore che corrispondono ad
> Agenti correttamente gestiti all'interno del proprio sito E-commerce**
> .

A questo punto occorrerà quindi selezionare gli Agenti Mexal gestiti
all'interno del sito relativamente ai quali si vuole concedere la
possibilità di modificare gli sconti e valorizzare il campo della
videata aggiuntiva sopra evidenziato **con N.**

> **NOTA BENE:** nel caso in cui il campo in oggetto non venga
> valorizzato, verrà considerato come se per esso fosse stato impostato
> il valore **S** ed il relativo Agente non avrà quindi la possibilità
> di modificare gli sconti all'interno del sito.
>
> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni Agente gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.

Una volta attivata questa particolare modalità di gestione, nel caso in
cui ad effettuare un ordine sul sito sia un Agente opportunamente
abilitato alla modifica degli sconti, alla pagina Carrello verrà
visualizzato, per ogni articolo, il prezzo al netto di eventuali sconti.

Tali sconti verranno infatti inseriti all'interno di un campo di testo
liberamente modificabile dall'Agente stesso.

![](./assets/media/image87.png)

L'Agente avrà quindi la possibilità di inserire per ogni singolo
articolo in carrello degli sconti adottando, in questo senso la stessa
logica degli sconti Mexal.

I valori ammessi in questo campo saranno quindi:

1.  sconto a valore, anteponendo il carattere \'-\' alla cifra (es.
    -100);

2.  sconto in percentuale con un massimo di due cifre decimali (es.
    10,48);

3.  sconti a cascata con un massimo di 9 valori ammessi (es. 10 + 20 +
    30 + 40)

4.  sconto Merce con valori compresi tra 100 e 109.

Ovviamente affinché la modifica allo sconto possa essere applicata in
maniera corretta sarà necessario aggiornare la relativa riga del
carrello cosa questa che, dipendentemente dalla impostazioni settate per
il componente Carrello, potrà avvenire al click sul relativo pulsante di
aggiornamento oppure semplicemente togliendo il focus dal campo di
modifica dello sconto.

**ATTENZIONE!** nel caso in cui lo sconto applicato dovesse essere
superiore al prezzo effettivo dell'articolo, verrà visualizzato un
apposito messaggio di errore e lo sconto non verrà poi applicato (questo
per evitare poi eventuali errori che si avrebbero in fase di
sincronizzazione dell'ordine con il gestionale)

![](./assets/media/image88.png)

Il messaggio evidenziato in figura può essere personalizzato dal menu
"**Sito -- Testi / Messaggi del Sito -- Testi dei Componenti**"
selezionando il componente "**Carrello**" e impostando il testo
desiderato in corrispondenza dell'elemento "**Errore Sconto Agente**"

![](./assets/media/image89.png)

Un controllo analogo verrà effettuato anche nel caso in cui per un
determinato articolo dovesse essere stata attivata la funzionalità
"**Sconto Massimo articolo**". Anche in queste condizioni infatti nel
momento in cui l'Agente dovesse tentare di inserire per l'articolo in
esame uno sconto superiore al massimo valore ammesso, verrà visualizzato
un apposito messaggio di errore

![](./assets/media/image90.png)

Tale messaggio potrà essere personalizzato, come nel caso precedente,
dal menu "**Sito -- Testi / Messaggi del Sito -- Testi dei Componenti**"
selezionando il componente "**Carrello**" e impostando il testo
desiderato in corrispondenza, questa volta dell'elemento "**Errore
Sconto Massimo Agente**"

Infine nel caso in cui per un articolo sia già presente uno sconto, e
l'Agente decidesse di azzerare tale valore lasciando vuoto il relativo
campo, l'applicazione interpreterà questa azione come la volontà d parte
dell'Agente di non applicare all'articolo nessuno sconto.

> **NOTA BENE:** per gli articoli di tipo "Campionario" lo sconto
> indicato dall'agente verrà applicato a tutti i singoli articoli
> componenti il campionario stesso. Per gli articoli a confezioni lo
> sconto indicato dall'Agente verrà applicato sul singolo elemento della
> confezione.

**ATTENZIONE! Lo sconto massimo gestito per un certo articolo non è
legato ad un eventuale prezzo minimo impostato per l'articolo stesso.**

Ciò significa dunque che se un Agente è stato abilitato alla modifica
dei prezzi e non è stato impostato correttamente il campo relativo al
prezzo minimo, l'Agente potrebbe anche impostare un prezzo di vendita
che risulti essere inferiore a quello che si otterrebbe a seguito
dell'applicazione dello sconto massimo consentito.

##### MODIFICA PREZZO

La "Funzionalità Mexal" **"Modifica Prezzo"** consente di attivare una
particolare modalità di gestione a seguito della quale sarà possibile
decidere, per ogni singolo Agente, se questo potrà essere o meno
abilitato, in fase di ordine all'interno del sito, a modificare i prezzi
articolo.

> **NOTA BENE:** tale funzionalità è da considerarsi, ovviamente, in
> relazione ai soli siti di tipo B2B o Misto. Gli unici utenti
> eventualmente in grado, infatti, di modificare gli sconti all'interno
> del sito, potranno essere solo ed esclusivamente gli Agenti
> opportunamente abilitati.

**Per poter adottare questa particolare modalità di gestione sarà quindi
necessario attivare lato gestionale la Funzionalità Mexal "Modifica
Prezzo".**

Una volta preparata dunque, all'interno del gestionale, la struttura
dati utilizzata per gestire le nuove "Funzionalità Mexal", secondo
quanto descritto nel capitolo "Attivazione / Disattivazione Delle
Funzionalità Mexal" di questo manuale, sarà poi necessario richiamare la
maschera **"Configurazione gestione dati web cliente/fornitore"** qui di
seguito riportata, e impostare a **S** il campo in corrispondenza della
funzionalità **"Modifica Prezzo".**

![](./assets/media/image91.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati web
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for"** **(F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, il campo **" Modifica Prezzo"**
corrispondente alla "Funzionalità Mexal" precedentemente attivata.

![](./assets/media/image92.png)

> **NOTA BENE:** il campo "Modifica Prezzo" comparirà sia nelle
> anagrafiche dei conti di tipo Cliente che in quelle di tipo Fornitore.
> **Ovviamente ai fini del sito tale campo verrà considerato, e
> conseguentemente verrà attivata la relativa funzionalità, solo ed
> esclusivamente per i conti di tipo Fornitore che corrispondono ad
> Agenti correttamente gestiti all'interno del proprio sito E-commerce**
> .

A questo punto occorrerà quindi selezionare gli Agenti Mexal gestiti
all'interno del sito relativamente ai quali si vuole concedere la
possibilità di modificare i prezzi e valorizzare il campo della videata
aggiuntiva sopra evidenziato con S.

> **NOTA BENE:** nel caso in cui il campo in oggetto non venga
> valorizzato, verrà considerato come se per esso fosse stato impostato
> il valore **N** ed il relativo **Agente non avrà quindi la possibilità
> di modificare alcun prezzo**.
>
> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni Agente gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.

**ATTENZIONE!!! Nel caso in cui si dovesse decidere di attivare questo
tipo di funzionalità e di concedere quindi a determinati Agenti la
possibilità di modificare, in fase di ordine all'interno del sito, i
prezzi degli articoli, diventa di assoluta importanza impostare per
ciascuno di essi un prezzo minimo.**

In caso contrario infatti l'Agente abilitato alla modifica dei prezzi
non avrebbe alcun limite e, volendo, potrebbe anche azzerare
completamente il prezzo di vendita.

Per maggiori informazioni in merito alla possibilità di impostare, per
ogni singolo articolo gestito all'interno del sito un prezzo minimo, si
veda anche il precedente capitolo "Funzionalità Mexal Articoli -- Prezzo
Minimo" di questo manuale.

Una volta attivata questa particolare modalità di gestione, nel caso in
cui ad effettuare un ordine sul sito sia un Agente opportunamente
abilitato alla modifica dei prezzi, alla pagina Carrello potrà essere
visualizzato (dipendentemente da come è stato impostato e configurato il
componente "Carrello" o "Carrello Custom"), un apposito campo di input
che l'Agente potrà utilizzare per impostare il prezzo di vendita
dell'articolo stesso

![](./assets/media/image93.png)

Nel caso in cui per un certo articolo sia stata attivata anche la
funzionalità "**Prezzo Minimo**" (cosa questa assolutamente
indispensabile in questo tipo di gestione) e l'Agente tenti di impostare
per esso un prezzo inferiore a quello minimo consentito, , verrà
visualizzato un apposito messaggio di errore (personalizzabile nella
sezione "Testi / Messaggi" del Wizard agendo sulla voce "Errore Prezzo
minimo Agente" del componente Carrello / Carrello Custom) per informarlo
che il valore impostato non è corretto **e il prezzo dell'articolo verrà
automaticamente impostato sul prezzo minimo consentito**

![Videate\\prezzo_minimo_messaggio.bmp](./assets/media/image94.png)

**ATTENZIONE! Per gli articoli di tipo Campionario non è possibile
effettuare variazioni di prezzo**

**ATTENZIONE! Il prezzo minimo gestito per un certo articolo non è
legato ad un eventuale sconto massimo impostato per l'articolo stesso**

Ciò significa dunque che se un Agente è stato abilitato alla modifica
degli sconti e non è stato impostato correttamente il campo relativo
allo sconto massimo di vendita, l'Agente potrebbe anche applicare uno
sconto tale da portare il prezzo dell'articolo al di sotto del valore
impostato per il suo prezzo minimo

##### ULTERIORE DESCRIZIONE 1/2/3 (CLIENTI)

Le "Funzionalità Mexal" **"Ulteriore Descrizione 1/2/3"** attivano
specifici campi, nella videata aggiuntiva cli/for appositamente
riservata per Passweb, che potranno essere personalizzati a livello di
Descrizione e che potranno essere utilizzati quindi per gestire
informazioni aggiuntive (oltre a quelle tradizionali presenti in
anagrafica cli/for) sui clienti del proprio sito web.

**Per poter usufruire di questi campi aggiuntivi sarà quindi necessario
attivare lato gestionale le relative Funzionalità Mexal "Ulteriore
Descrizione 1/2/3".**

Una volta preparata dunque, all'interno del gestionale, la struttura
dati utilizzata per gestire le nuove "Funzionalità Mexal", secondo
quanto descritto nel capitolo "Attivazione / Disattivazione Delle
Funzionalità Mexal" di questo manuale, sarà poi necessario richiamare la
maschera **"Configurazione gestione dati web cliente/fornitore"** qui di
seguito riportata, e flaggare il campo **"Ulteriore Descrizione
1/2/3".**

![](./assets/media/image95.png)

> **NOTA BENE:** la maschera "Configurazione gestione dati
> cliente/fornitore" può essere richiamata in un qualsiasi momento
> grazie al pulsante **"Dati cli/for" (F6)** attivo in Mexal in
> corrispondenza della voce di menu "Anagrafica Azienda -- Dati
> Aziendali -- Configurazione Moduli -- Passweb"

Portandosi poi nell'anagrafica dello specifico cliente, cliccando sul
pulsante **"Dati Aggiuntivi/ eCommerce" (Shift + F8)** e selezionando,
tra quelle presenti in elenco, la videata aggiuntiva clienti/fornitori
relativa allo specifico sito su cui si intende operare, sarà possibile
trovare, nella successiva maschera, i campi **Ulteriore Descriz. 1/2/3**
corrispondenti alle "Funzionalità Mexal" precedentemente attivate.

![](./assets/media/image96.png)

A questo punto quindi sarà possibile utilizzare i campi sopra
evidenziati (sono campi alfanumerici) per gestire informazioni
aggiuntive (oltre a quelle tradizionali presenti in anagrafica)
relativamente ai clienti del proprio sito web. Tali campi potrebbero
essere utilizzati, ad esempio, per gestire informazioni quali la
Professione o il Titolo di studio, informazioni queste che non compaiono
tra quelle normalmente gestite nell'anagrafica clienti/fornitori di
Mexal.

Considerato quindi l'utilizzo che verrà fatto di questi campi, e
soprattutto considerato il fatto che le informazioni in esse contenute
potrebbero essere le più svariate, si consiglia, una volta attivati
questi campi, di personalizzarne la descrizione in maniera tale da avere
a disposizione dei riferimenti più significativi rispetto ai generici
"Ulteriore Descriz 1/2/3".

**ATTENZIONE!** Per variare e personalizzare la descrizione di questi
campi, secondo le proprie specifiche esigenze, è possibile agire dalla
voce di menu *"Servizi -- Personalizzazioni -- Passweb -- Videate
aggiuntive PC/Clienti/fornitori"* selezionando, ovviamente, lo specifico
sito per il quale si intende operare

> **NOTA BENE:** dopo aver attivato la "Funzionalità Mexal" in esame ed
> aver correttamente valorizzato il relativo campo della videata
> aggiuntiva di ogni articolo gestito all'interno del sito, sarà
> necessario lanciare una sincronizzazione in modo tale da riportare le
> variazioni effettuate in Mexal anche all'interno di Passweb.
>
> **NOTA BENE:** nel caso in cui i tre campi "Ulteriore Descrizione
> 1/2/3" non siano sufficienti è comunque possibile creare un'altra (o
> più) videata aggiuntiva con al suo interno tutti i campi necessari per
> visualizzare sul sito tutte le informazioni aggiuntive desiderate. Non
> sarà comunque possibile collegare in alcun modo a queste ulteriori
> videate eventuali

Una volta attivati in maniera corretta, tali campi saranno poi
disponibili all'interno del menu a tendina del campo **"Campo Mexal"**
presente alla pagina **"Utenti - Gestione Parametri Utenti ECommerce-
Gestione Attributi"** del Wizard e potranno quindi essere utilizzati per
mappare appositi Attributi Cliente.

Per maggiori informazioni relativamente all'associazione Campo Mexal --
Attributo Cliente si veda anche la relativa sezione di questo manuale
"Utenti Catalogo -- Gestione Attributi".

##### VARIAZIONE A BLOCCHI CAMPI DELLA VIDEATA AGGIUNTIVA PASSWEB / CLI/FOR

Anziché agire direttamente e manualmente sull'anagrafica di ogni singolo
utente, volendo, è anche possibile eseguire ( mediante la funzione di
servizio "***Servizi -- Variazioni -- Contabilità -- Varia Condizioni
clienti/fornitori***"), sui campi delle videate aggiuntive
cliente/fornitore appositamente riservate a Passweb, e quindi ai 9 siti
collegabili ad ogni singola azienda Mexal, apposite variazioni a
blocchi.

In particolare nella funzione di servizio sopra indicata sarà poi
possibile eseguire, normalmente, la selezione sulle anagrafiche utente
utilizzando i campi della finestra principale.

Inoltre risulterà attivo anche il pulsante **E-Commerce \[F8\]**.

Cliccando su questo pulsante verrà visualizzato l'elenco di tutti i siti
(attivi e non) attualmente configurati sull'azienda in esame.

![](./assets/media/image97.png)

Selezionando quindi lo specifico sito su cui si intende operare e
cliccando sul pulsante **OK (Invio)** verrà visualizzata la solita
maschera mediante la quale poter decidere se filtrare gli articoli in
Ricerca, oppure in Modifica

![](./assets/media/image98.png)

Scegliendo la voce **Ricerca** sarà poi possibile selezionare gli utenti
da variare in base ai campi presenti nella videata aggiuntiva
clienti/fornitori appositamente riservata per il sito precedentemente
selezionato.

Allo stesso modo la voce **Modifica** consentirà di impostare, in
blocco, per tutti gli utenti precedentemente filtrati, i campi della
videata aggiuntiva clienti/fornitori appositamente riservata per il sito
precedentemente selezionato

**RICERCA**

Questa funzione permette di selezionare gli utenti da variare in base ai
campi presenti nella videata aggiuntiva clienti/fornitori appositamente
riservata per il sito precedentemente selezionato

![](./assets/media/image99.png)

Inserendo un valore in un campo di ricerca verranno elaborati solo i
conti che contengono quel valore in quel campo.

Per selezionare i conti che hanno il campo vuoto, è attivo il pulsante
\[F5\] Se vuoto. Dopo aver immesso delle selezioni, premendo nuovamente
il pulsante \[F8\], viene segnalata la presenza di campi impostati con
la dicitura "(impostata)":

![](./assets/media/image69.png)

**MODIFICA**

Questa funzione permette di impostare il valore le voci da modificare.

![](./assets/media/image100.png)

Impostando un valore in un campo questo verrà inserito nei conti che
rispettano i parametri di selezione. Per azzerare un campo è attivo il
pulsante \[F5\] Azzera.

Dopo aver immesso dei valori nei campi, premendo nuovamente il pulsante
\[F8\] Passweb, viene segnalata la presenza di campi impostati con la
dicitura "(impostata)":

Definite le impostazioni di selezione sui dati anagrafici, di selezione
e variazione sui dati Passweb, confermando con \[F10\] la finestra
principale ha inizio l'elaborazione.

**ESEMPIO PRATICO**

Si desidera impostare la quantità "Minimo Ordine Merce" a 3 per tutti i
clienti con il campo anagrafico "Categoria statistica" uguale a "12" e
con il campo "Blocco Ordine Fuori Fido" della videata aggiuntiva Passweb
impostato a "S".

Per ottenere questo si deve innanzitutto impostare nella colonna RICERCA
della finestra principale il campo:

Categoria statistica: = 12

Poi si preme \[F8\] E-Commerce e si seleziona la voce Ricerca; si
imposta a "S" la voce "Blocco Ordine Fuori Fido" e si conferma con
\[F10\].

Si preme nuovamente \[F8\] E-Commerce e questa volta si seleziona la
voce Modifica; si imposta "3" sul campo "Minimo Ordine Merce" e si
conferma con \[F10\].

A questo punto il programma è posizionato sulla finestra principale e
per eseguire l'elaborazione occorre confermare nuovamente con \[F10\].

