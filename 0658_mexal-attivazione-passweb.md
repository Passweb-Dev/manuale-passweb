# MEXAL -- ATTIVAZIONE PASSWEB



Come precedentemente evidenziato per poter garantire una corretta
integrazione sito -- gestionale, è necessario:

- **Lato Passweb**, impostare correttamente tutti i parametri di
  configurazione necessari per consentire al sito di collegarsi con il
  gestionale

- **Lato gestionale**, attivare correttamente Passweb dichiarando quanti
  e quali siti dovranno essere collegati alla specifica azienda
  dell'installazione, quali funzionalità articoli o clienti dovranno
  essere abilitate e quali articoli/clienti/ordini dovranno essere
  esportati e gestiti sullo specifico sito

In particolare per poter attivare Passweb, lato gestionale, e collegare
quindi uno o più siti ecommerce alle aziende gestite all'interno della
propria installazione Mexal è necessario, innanzitutto, selezionare, tra
quelle presenti nella propria installazione, l'azienda cui si vuole
collegare il sito web e portarsi poi nella maschera "**E-Commerce"** qui
di seguito riportata accessibile dalla voce di menu ***"Anagrafica
Azienda -- Dati Aziendali -- Configurazione Moduli -- Passweb"***

![](./assets/media/image15.png)

**ATTENZIONE! E' possibile collegare ad ogni singola azienda presente
nella propria installazione Mexal fino ad un massimo di 9 siti
differenti.**

All'interno della maschera E-Commerce è possibile visualizzare i siti
attualmente collegati all'azienda su cui si sta operando (colonna
"**Nome Sito Web**") e quanti di essi sono attualmente attivi (colonna
"**Attivo**").

Per poter collegare un nuovo sito all'azienda è sufficiente selezionare,
all'interno della maschera sopra evidenziata, uno degli slot liberi e
cliccare successivamente sul pulsante **OK** **(Invio)**.

Verrà in questo modo visualizzata la maschera di attivazione del nuovo
sito ecommerce

![](./assets/media/image16.png)

all'interno della quale il campo:

- **Nome Sito Web:** consente di assegnare un nome al sito che si
  desidera collegare all'azienda Mexal su cui si sta operando.
  Considerando che ad ogni singola azienda possono essere associati,
  come detto, fino ad un massimo di 9 siti differenti, il nome indicato
  all'interno di questo campo servirà poi per identificare, all'interno
  del gestionale, a quale dei 9 siti faranno riferimento i dati di
  specifiche maschere.

> In definitiva, dunque, in tutte le funzioni del gestionale collegate
> in qualche modo al sito Ecommerce, verrà visualizzato, innanzitutto,
> l'elenco dei siti gestiti sulla specifica azienda con il nome indicato
> per ciascuno di essi all'interno di questo campo, in maniera tale da
> poter selezionare esattamente su quale di essi si intende operare.

- **E-Commerce attivo:** consente, se impostato a **Si**, di attivare in
  Mexal tutta l'infrastruttura necessaria per poter collegare e gestire
  sull'azienda in esame il sito indicato nel precedente campo.

> Nello specifico, una volta impostato a Si questo campo e salvati
> correttamente i dati della maschera verranno create in Mexal due
> videate aggiuntive, una Articoli e una Clienti/Fornitori,
> appositamente riservate per Passweb ed utilizzate per gestire alcune
> delle principali funzionalità del sito Ecommerce direttamente da
> Mexal.
>
> **ATTENZIONE! In caso di disattivazione di un sito verranno eliminate
> entrambe le videate aggiuntive (articoli e clienti/fornitori) create
> all'attivazione del sito stesso. In conseguenza di ciò verranno,
> ovviamente, cancellati anche tutti i dati e le impostazioni
> precedentemente gestite mediante l'uso dei campi di queste videate.**

- **Indirizzo Sito Web:** consente di indicare l' url del sito Passweb
  che si desidera collegare all'azienda Mexal su cui si sta operando

> **ATTENZIONE! Ai fini di una corretta integrazione sito -- gestionale
> è necessario indicare all'interno del campo "Indirizzo sito web" l'
> url primario che si è deciso di gestire sul proprio sito Passweb.**
>
> Nel caso in cui si desideri utilizzare per il proprio sito l' url di
> terzo livello (es. www.nomesito.passweb.it) fornito gratuitamente da
> Passepartout ed indicato nelle mail inviate da Passepartout stessa
> all'atto dell'acquisto del sito, sarà quindi necessario inserire tale
> url all'interno del campo Mexal "Indirizzo Sito web" .
>
> Nel caso in cui si desideri invece utilizzare un dominio di secondo
> livello (es. www.nomesito.it) acquistato e gestito da fornitori
> diversi da Passepartout, oltre a comunicare a Passepartout tale
> indirizzo, sarà poi necessario inserirlo anche all'interno del campo
> in questione.
>
> **NOTA BENE:** in fase di sincronizzazione sito -- gestionale verrà
> effettuato un controllo di coerenza tra l' url indicato all'interno
> del campo Mexal "Indirizzo Sito Web" e quello effettivamente
> utilizzato sul sito. In caso di esito negativo la sincronizzazione non
> potrà terminare in maniera corretta.

- **Aggiorna OC automaticamente:** consente di configurare i documenti
  di tipo OC effettuati direttamente sul gestionale in maniera tale che
  possano essere esportati all'interno del corrispondente sito Passweb.

> Nel momento in cui si dovesse decidere di attivare questo parametro
> **i documenti di tipo OC** nati sul gestionale assumeranno
> automaticamente la configurazione mostrata in figura

![](./assets/media/image17.png)

> rendendo quindi il relativo documento direttamente esportabile
> all'interno del sito
>
> **ATTENZIONE!** Solo uno dei 9 siti gestibili può avere il parametro
> in oggetto selezionato

- **Videata Aggiuntiva Riservata per Dati Clienti/Fornitori:** campo
  gestito dalla procedura che identifica l'archivio riservato ai dati
  dei clienti e fornitori collegati all'e-commerce

- **Videata Aggiuntiva Riservata per Dati Articolo:** campo gestito
  dalla procedura che identifica l'archivio riservato ai dati degli
  articoli collegati all'e-commerce.

Una volta compilata l'anagrafica del nuovo sito E-Commerce confermando
col il pulsante **OK (F10)** la procedura si preoccuperà di creare
automaticamente, **assegnandogli le prime due lettere libere**, le nuove
videate aggiuntive articoli e clienti/fornitori che, come
precedentemente evidenziato, serviranno ora per gestire alcune delle
principali funzionalità del sito Ecommerce direttamente da Mexal.

> **NOTA BENE:** una volta terminata la configurazione del sito e create
> quindi le relative videate aggiuntive Mexal, i campi **"Vid.
> aggiuntiva riservata per dati cli/for"** e **"Vid. aggiuntiva
> riservata per dati articolo"** non potranno più essere modificate.

A questo punto verranno quindi aperte in successione le due maschere
**"Configurazione gestione dati web articolo"** e **"Configurazione
gestione dati web cliente/fornitore"**

![](./assets/media/image18.png)

![](./assets/media/image19.png)

mediante cui poter decidere quale "Funzionalità Mexal" attivare
rispettivamente per gli articoli e per i clienti gestiti all'interno del
sito.

> **NOTA BENE:** le due maschere sopra evidenziate potranno essere
> richiamate in un qualsiasi momento grazie ai due pulsanti **"Dati
> Articolo"** **(F5)** e **"Dati cli/for"** **(F6)** attivi in Mexal in
> corrispondenza della relativa "Anagrafica sito Web"

![](./assets/media/image20.png)

Per poter attivare una delle funzionalità indicate all'interno di queste
maschere è sufficiente flaggare il campo corrispondente alla
funzionalità desiderata. Lasciando il campo deselezionato la relativa
funzionalità verrà invece disattivata.

**ATTENZIONE! La procedura appena evidenziata consente unicamente di
preparare, all'interno di Mexal, la struttura dati necessaria per
gestire l'integrazione sito -- gestionale.**

Sarà poi necessario agire sul singolo articolo/cliente valorizzando i
campi aggiuntivi secondo le proprie esigenze ed effettuare quindi una
sincronizzazione per riportare le variazioni effettuare in Mexal anche
all'interno del sito Ecommerce

Le nuove videate aggiuntive così create potranno essere visualizzate e
personalizzate, per quanto possibile, alla voce di menu "*Servizi --
Personalizzazioni -- Passweb -- Videate aggiuntive PC/Clienti/fornitori
/ articoli*" dopo aver selezionato, ovviamente, lo specifico sito per il
quale si intende operare

> **NOTA BENE:** relativamente a tali videate sarà possibile variare
> unicamente la Descrizione (**Campo "Descrizione**"), l'Obbligatorietà
> (**Campo "O"**) e l'Ordine di Inserimento (**Campo "IN"**) dei campi
> corrispondenti a "Funzionalità Mexal" effettivamente attivate.

Di seguito viene riportato un elenco, rispettivamente, delle
funzionalità Mexal articolo e cliente che è possibile
attivare/disattivare.

**DATI WEB ARTICOLO**

![](./assets/media/image18.png)

**Articolo sul sito: selezionato a default e** **non modificabile**. Non
rappresenta una vera e propria "Funzionalità Mexal" ma è comunque di
fondamentale importanza in quanto grazie a esso sarà poi possibile
decidere articolo per articolo quale di questi dovrà essere esportato e
gestito all'interno del sito Web. Tale funzionalità attiva infatti uno
specifico campo, nella videata aggiuntiva articoli appositamente
riservata per Passweb, attraverso il quale poter decidere se lo
specifico articolo dovrà essere o meno esportato e gestito all'interno
del sito web.

> **NOTA BENE:** per maggiori informazioni relative alle modalità di
> selezione e di esportazione degli articoli all'interno del sito
> e-commerce si veda l'apposita sezione di questo manuale ("Esportazione
> / Eliminazione di articoli all'interno del sito e-commerce").

**Pubblica:** attivando questa funzionalità sarà poi possibile oscurare
temporaneamente la visibilità di uno o più articoli all'interno del
negozio web senza doverli necessariamente eliminare in maniera
definitiva. Per maggiori informazioni relativamente all'utilizzo ed
all'attivazione di questa funzionalità si veda anche il successivo
capitolo **"Pubblicare /Nascondere articoli all'interno del negozio
web"**.

**Visualizza in Negozio:** attivando questa funzionalità sarà poi
possibile decidere quali articoli, tra quelli gestiti, dovranno essere o
meno visualizzati all\'interno del Negozio web. Per maggiori
informazioni relativamente all'utilizzo e all'attivazione di questa
funzionalità si veda anche il successivo capitolo **"Visualizzazione
articoli in Negozio"**.

**Prezzo a richiesta:** selezionando questo campo verrà attivata una
particolare "Funzionalità Mexal" a seguito della quale sarà poi
possibile non visualizzare, all\'interno del sito web, il prezzo di
determinati articoli. Per maggiori informazioni relativamente
all'utilizzo ed all'attivazione di questa funzionalità si veda anche il
successivo capitolo **"Prezzo articoli a richiesta"**.

**Gestione unità di misura:** attivando questa funzionalità sarà poi
possibile decidere di utilizzare per ogni singolo articolo l'unità di
misura principale o secondaria. Per maggiori informazioni relativamente
all'utilizzo ed all'attivazione di questa funzionalità si veda anche il
successivo capitolo **"Gestione Unità di misura
principale/secondaria"**.

**Confezione Multipla bloccata:** attivando questa funzionalità sarà poi
possibile acquistare determinati articoli presenti in negozio unicamente
secondo quantità multiple stabilite articolo per articolo. Per maggiori
informazioni relativamente all'utilizzo ed all'attivazione di questa
funzionalità si veda anche il successivo capitolo **"Gestione multipli e
confezioni"**.

**Quantità massima di vendita:** attivando questa funzionalità sarà poi
possibile decidere, per ogni singolo articolo, il numero massimo di
pezzi acquistabili. Per maggiori informazioni relativamente all'utilizzo
ed all'attivazione di questa funzionalità si veda anche il capitolo
**"Vendita articoli per quantità massima"** di questo Capitolo.

**Sconto massimo di vendita:** attivando questa funzionalità sarà poi
possibile impostare, per ogni singolo articolo, lo sconto massimo che
ogni Agente, opportunamente abilitato alla modifica degli sconti, potrà
effettuare su di esso.

**Gestione articoli in offerta:** attivando questa funzionalità sarà poi
possibile decidere quali degli articoli presenti in negozio dovranno
essere considerati come articoli in offerta (ad es. articoli del sito
attraverso il Componente E-commerce "Offerte e Novità" inseriti in
Homepage). Per maggiori informazioni relativamente all'utilizzo e
all'attivazione di questa funzionalità si veda anche il successivo
capitolo **"Gestione articoli in offerta/fine serie/novità".**

**Gestione articoli novità:** attivando questa funzionalità sarà poi
possibile decidere quali degli articoli presenti in negozio dovranno
essere considerati come Novità. Per maggiori informazioni relativamente
all'utilizzo e all'attivazione di questa funzionalità si veda anche il
successivo capitolo **"Gestione articoli in offerta/fine
serie/novità".**

**Gestione articoli fine serie:** attivando questa funzionalità sarà poi
possibile decidere quali degli articoli presenti in negozio dovranno
essere considerati come articoli in fine serie. Per maggiori
informazioni relativamente all'utilizzo e all'attivazione di questa
funzionalità si veda anche il successivo capitolo **"Gestione articoli
in offerta/fine serie/novità".**

**Disponibilità indicativa:** selezionando questo campo verrà attivato
uno specifico campo, nella videata aggiuntiva articoli appositamente
riservata per Passweb, all'interno del quale sarà poi possibile indicare
per ogni singolo articolo una disponibilità indicativa da visualizzare
all'interno del sito web. Per maggiori informazioni relativamente
all'utilizzo e all'attivazione di questa funzionalità si veda anche il
successivo capitolo **"Gestione disponibilità indicativa"**.

**Spese di trasporto a Scaglioni:** attivando questa funzionalità sarà
poi possibile gestire le spese di trasporto secondo degli scaglioni ben
definiti. Per maggiori informazioni relativamente all'utilizzo ed
all'attivazione delle spese di trasporto a scaglioni si veda anche il
capitolo **"Gestione delle spese di trasporto a scaglioni"** di questo
manuale

**Ulteriore Descrizione 1/2/3:** se selezionati verranno poi attivati
specifici campi, nella videata aggiuntiva articoli appositamente
riservata per Passweb, che potranno essere personalizzati a livello di
Descrizione e che potranno essere utilizzati quindi per fornire
informazioni aggiuntive (oltre a quelle tradizionali presenti in
anagrafica articoli) sugli articoli gestiti e venduti all'interno del
negozio web. Per maggiori informazioni relativamente all'utilizzo ed
all'attivazione di questi campi si veda anche il successivo capitolo
**"Ulteriore Descrizione 1/2/3 (articoli)".**

> **NOTA BENE:** nel caso in cui i tre campi "Ulteriore Descrizione
> 1/2/3" non siano sufficienti è comunque possibile creare un'altra (o
> più) videata aggiuntiva articoli con al suo interno tutti i campi
> necessari per visualizzare sul sito le informazioni aggiuntive
> relative agli articoli gestiti. Non sarà comunque possibile collegare
> in alcun modo a queste ulteriori videate eventuali funzionalità Mexal.

**Prezzo Minimo:** attivando questa funzionalità sarà poi possibile
impostare per ogni singolo articolo, un valore minimo oltre il quale gli
Agenti, opportunamente abilitati alla modifica dei prezzi, non potranno
mai scendere.

**Gruppi Merceologici:** attivando questa funzionalità sarà poi
possibile definire per ogni singolo articolo le categorie merceologiche
secondarie cui l'articolo stesso dovrà essere associato all'interno del
sito.

**Gestione Confezioni:** attivando questa funzionalità sarà poi
possibile decidere per ogni singolo articolo come questo stesso articolo
dovrà essere effettivamente venduto all'interno del sito: in quantità
singola, a confezioni oppure a multipli

**DATI WEB CLIENTE FORNITORE**

![](./assets/media/image19.png)

**Cliente/fornitore sul sito:** Non rappresenta una vera e propria
"Funzionalità Mexal" ma è comunque di fondamentale importanza in quanto
grazie a essa **sarà poi possibile decidere per ogni singolo cliente se
questo dovrà essere o meno esportato e gestito all'interno del sito
Web**. Tale funzionalità attiva infatti uno specifico campo, nella
videata aggiuntiva clienti/fornitori appositamente riservata per
Passweb, attraverso il quale poter decidere se lo specifico cliente
dovrà essere o meno esportato e gestito all'interno del sito web.

> **NOTA BENE:** per maggiori informazioni relative alle modalità di
> selezione e di esportazione dei clienti Mexal all'interno del sito
> e-commerce si veda l'apposita sezione di questo manuale ("Esportazione
> / Eliminazione di clienti Mexal all'interno del sito e-commerce").

**Gestione login -- utente/password: selezionati a default** e **non
modificabili.** Attivano all'interno dell'apposita videata aggiuntiva
clienti/fornitori di Mexal i campi necessari per gestire le credenziali
(nome utente e password) di accesso al sito.

**Gestione minimo ordine:** attivando questa funzionalità sarà poi
possibile specificare per ogni singolo cliente il valore minimo del
totale merce che lo stesso cliente dovrà necessariamente superare per
poter confermare l\'ordine. Per maggiori informazioni relativamente
all'utilizzo e all'attivazione di questa funzionalità si veda anche il
successivo capitolo **"Gestione minimo d'ordine"** .

**Abilita all'area riservata (solo per siti B2B o Misti):** se
selzionato attiva una particolare "Funzionalità Mexal" a seguito della
quale sarà poi possibile specificare per ogni singolo cliente se questo
è abilitato o meno ad accedere all'area riservata del sito web e a
sfruttarne dunque le relative funzionalità. Per maggiori informazioni
relativamente all'utilizzo e all'attivazione di questa funzionalità si
veda anche il successivo capitolo **"Abilitazione accesso all'Area
Riservata"**.

**Blocco ordine se fuori fido:** attivando questa funzionalità sarà poi
possibile decidere se impedire o meno ai clienti fuori fido di
effettuare ordini all'interno del sito web. Per maggiori informazioni
relativamente all'utilizzo e all'attivazione di questa funzionalità si
veda anche il successivo capitolo **"Blocco ordine se fuori fido"** .

**Ulteriore Descrizione 1/2/3:** se selezionati attivano specifici
campi, nella videata aggiuntiva clienti/fornitori appositamente
riservata per Passweb, che potranno essere personalizzati a livello di
Descrizione e che potranno essere utilizzati quindi per gestire
informazioni aggiuntive (oltre a quelle tradizionali presenti in
anagrafica clienti/fornitori) sui clienti del proprio sito e-commerce.
Per maggiori informazioni relativamente all'utilizzo ed all'attivazione
di questi campi si veda anche il successivo capitolo **"Ulteriore
Descrizione 1/2/3 (clienti)"**.

> **NOTA BENE:** nel caso in cui i tre campi "Ulteriore Descrizione
> 1/2/3" non siano sufficienti è comunque possibile creare un'altra (o
> più) videata aggiuntiva clienti/fornitori con al suo interno tutti i
> campi necessari per visualizzare sul sito tutte le informazioni
> aggiuntive desiderate. Non sarà comunque possibile collegare in alcun
> modo a queste ulteriori videate eventuali funzionalità Mexal.

Per maggiori informazioni relativamente all'attivazione ed alla gestione
lato Mexal delle suddette funzionalità (articoli o clienti) si veda
anche l'apposito manuale Mexal.

**Blocca Modifica Sconto:** attivando questa funzionalità sarà poi
possibile decidere, per ogni singolo Agente esportato e gestito
all'interno del sito, se questo, in fase d'ordine potrà essere o meno
abilitato anche alla modifica degli sconti.

**Modifica Prezzo:** attivando questa funzionalità sarà poi possibile
decidere, per ogni singolo Agente esportato e gestito all'interno del
sito, se questo, in fase d'ordine potrà essere o meno abilitato anche
alla modifica dei prezzi.

