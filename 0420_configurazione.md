# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_custom_configurazione_res.bmp](./assets/media/image283.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
settare i principali parametri di configurazione del componente stesso.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** permette di inserire un nome per il campo che si sta editando;

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Visualizza in Testata Data Scadenza/Consegna (solo Ecommerce Mexal):**
consente di decidere se visualizzare o meno nella testata del documento
la Data di Scadenza / Consegna (data questa che verrà poi inserita nella
testata del corrispondente documento gestionale)

**Tipologia Fase di Checkout:** consente di indicare il layout e la
modalità di funzionamento del checkout. E' possibile selezionare uno dei
seguenti valori:

- **Visualizzazione a step con Accordion**

- **Visualizzazione a Step Orizzontali**

- **Visualizzazione senza Step incolonnato**

- **Visualizzazione senza Step affiancato**

Per maggiori informazioni relativamente alle diverse tipologie di
checkout si veda quanto indicato all'interno dei successivi capitoli di
questo manuale.

**One Page Checkout:** consente di decidere se abilitare o meno il
modulo di One Step Checkout e se lasciare o meno attivo lo step di
riepilogo prima della conferma definitiva dell'ordine.

E' possibile selezionare uno dei seguenti valori:

- **No senza Riepilogo:** selezionando questa opzione non verrà
  abilitato né il modulo di "One Step Checkout" né lo step di riepilogo
  definitivo prima della conferma dell'ordine.

> In queste condizioni non sarà quindi possibile effettuare ordini come
> Guest (Ospiti) e una volta inseriti tutti i dati richiesti (indirizzo
> di spedizione, pagamento ...), per completare l'ordine non sarà
> necessario passare attraverso nessun altro step.

- **No con Riepilogo:** selezionando questa opzione il modulo di "One
  Step Checkout" non verrà abilitato. Sarà invece attivo lo step di
  riepilogo definitivo prima della conferma dell'ordine.

> Non sarà quindi possibile effettuare ordini come Guest (Ospiti) e gli
> utenti per poter concludere un ordine dovranno necessariamente passare
> dalla pagina di Registrazione e creare il proprio account di accesso
> al sito. Inoltre una volta inseriti tutti i dati richiesti (indirizzo
> di spedizione, pagamento ...) verrà mostrato all'utente un riepilogo
> dell'ordine in cui saranno indicati gli articoli che sta per
> acquistare, il pagamento e la spedizione selezionati ... e solo a
> questo punto dopo aver accettato i termini e le condizioni di vendita
> sarà effettivamente possibile concludere l'ordine.

- **Si senza Riepilogo:** selezionando questa opzione verrà abilitato il
  modulo di "One Step Checkout" **senza il riepilogo ordine**.

> All'interno del checkout comparirà quindi un'ulteriore sezione in cui
> poter inserire il componente "**Registrazione Utente**" trasformando,
> di fatto, il tradizionale checkout custom in un modulo di "One Step
> Checkout" che gli utenti del sito potranno utilizzare per completare i
> loro acquisti anche in modalità Guest (Ospiti), o comunque senza dover
> per forza di cose passare prima dalla pagina di "Registrazione Utente"
> per creare un account di accesso.
>
> Inoltre nel momento in cui l'utente dovesse cliccare sul pulsante di
> Conferma (e tutti i dati dovessero essere validati correttamente)
> **l'ordine verrà immediatamente confermato ed inserito all'interno del
> gestionale** senza la necessità di passare attraverso ulteriori step.

- **Si con Riepilogo:** selezionando questa opzione verrà abilitato il
  modulo di "One Step Checkout" mantenendo comunque attivo anche lo step
  di riepilogo ordine.

> Anche in questo caso sarà quindi possibile inserire il componente
> "Registrazione Utente" all'interno del modulo di Checkout dando così
> agli utenti del sito la possibilità di effettuare ordini come Guest
> (Ospiti).
>
> A differenza del caso precedente però, essendo attivo ora lo Step di
> riepilogo, **il pulsante "Conferma Ordine" non porterà all'immediata
> ed effettiva conferma del documento**; verrà prima visualizzato un
> riepilogo definitivo dell'ordine con tutti i dati inseriti
>
> L'utente potrà quindi visionare il dettaglio del proprio ordine e, nel
> momento in cui tutto fosse corretto, potrà accettare le condizioni di
> vendita e cliccare sul pulsante di Conferma per confermare l'acquisto
> in maniera definitiva.
>
> Per maggiori informazioni relativamente al modulo di One Step Checkout
> si veda anche il successivo capitolo *(One Step Checkout*") di questo
> manuale

In relazione alla particolare modalità di gestione adottata è sempre
bene ricordare che:

- Nel momento in cui si dovesse decidere di attivare il One Step
  Checkout per consentire agli utenti del sito di portare a termine
  acquisti come ospite, sarà necessario verificare di aver attivato
  correttamente sul proprio sito Passweb anche la gestione della partita
  iva secondaria.

> In caso contrario potrebbero infatti verificarsi dei problemi in fase
> di inserimento ordine sul gestionale nel momento in cui un utente di
> tipo Azienda dovesse effettuare due ordini diversi come "Ospite"
> utilizzando sempre la stessa partita iva.

- Nel momento in cui si dovesse optare per una configurazione "Senza
  Riepilogo" è sempre bene inserire il riepilogo degli articoli in
  ordine, oltre che i relativi totali, assieme agli step di inserimento
  dati agendo per questo mediante i relativi parametri "**Visualizza
  Totale**" e "**Mostra Riepilogo a fianco**" presenti nella maschera di
  configurazione del componente.

**Mostra Riepilogo a fianco:** consente di decidere se visualizzare o
meno, direttamente all'interno del checkout, un riepilogo di quelli che
sono gli articoli attualmente in ordine, riepilogo questo che verrà
visualizzato immediatamente al di sopra della sezione relativa ai totali
del documento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\checkout_riepilogo_ordine.bmp](./assets/media/image284.png)

**ATTENZIONE!** Il parametro è visibile solo per "Tipologia Fase
Checkout = Visualizzazione a Step Orizzontali / Senza Step Affiancato /
Senza Step Incolonnato

**I dati visualizzati per ogni articolo presente nel riepilogo
dell'ordine sono esattamente gli stessi utilizzati per costruire anche
il dettaglio dell'ordine.**

In virtù di ciò occorre sempre ricordare che nel momento in cui si
dovesse decidere, per una qualche ragione, di eliminare o aggiungere dei
campi dal riepilogo ordine, questi stessi campi verranno poi eliminati o
aggiunti anche nel template utilizzato per visualizzare il dettaglio
dell'ordine stesso.

Ovviamente vale anche il discorso inverso, per cui se si dovessero
aggiungere o eliminare campi dal dettaglio del documento questi stessi
campi verranno poi automaticamente aggiunti o eliminati anche dal
riepilogo documento.

**Nel momento in cui l'esigenza dovesse essere quella di visualizzare,
nel riepilogo ordine, un numero di informazioni inferiore (es. solo
immagine, titolo e codice articolo) rispetto a quelle effettivamente
presenti nel dettaglio del documento, sarà necessario nascondere,
all'interno del riepilogo, i relativi componenti assegnando loro la
classe addizionale "hidesummary"** (utilizzando per questo l'apposito
campo presente nella maschera di configurazione di ogni componente
Passweb)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\checkout_riepilogo_ordine_hidesummary.bmp](./assets/media/image285.png)

Nelle risoluzioni per smartphone l'eventuale riepilogo degli articoli in
ordine verrà posizionato all'interno di un contenitore collassabile,
inizialmente chiuso e che potrà o meno essere visualizzato al click su
di un apposito pulsante.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\checkout_riepilogo_ordine_mobile.bmp](./assets/media/image286.png)

**ATTENZIONE!** La visualizzazione o meno, nelle risoluzioni mobile, del
totale del documento in corrispondenza del pulsante di apertura /
chiusura del riepilogo ordine dipende dalle impostazioni settate per il
parametro "**Visualizza Totale**"

**Visualizza Totale:** consente, se selezionato, di visualizzare i
Totali del documento già all'interno del modulo di checkout senza dover
quindi attendere la pagina di riepilogo dati.

**Posizionamento delle condizioni di vendita -- solo per checkout con
"Visualizzazione a Step Orizzontali":** consente di decidere dove dovrà
essere visualizzato il check di approvazione delle condizioni di
vendita.

E' possibile selezionare una delle seguenti opzioni:

- **Ultimo Step**: selezionando questa opzione il check di approvazione
  delle condizioni d'ordine verrà visualizzato solo nell'ultimo step del
  checkout

- **In Fondo:** selezionando questa opzioni il check delle condizioni
  d'ordine verrà visualizzato nella parte bassa di ogni singolo step del
  checkout

**Set Opzioni:** consente di selezionare, tra quelli presenti in elenco,
l'eventuale set di opzioni da associare al componente in esame.

L'utilizzo di un Set di Opzioni permetterà di visualizzare sul front end
del sito, in fase di checkout, una serie di campi custom che l'utente
potrà utilizzare per fornire informazioni aggiuntive sull'ordine che sta
portando a termine. Per maggiori informazioni in merito si veda anche
quanto indicato all'interno del capitolo "*Ordini -- Ordini -- Set di
Opzioni*" di questo manuale

**ATTENZIONE!** **Per poter gestire i Set Opzioni a livello di Ordine è
necessario aver acquistato e attivato il modulo delle Custom Option**

**Visualizza Parametri Documento (solo Ecommerce Mexal):** consente di
decidere se visualizzare o meno in fase di conferma ordine, ed
eventualmente a chi, la sezione attraverso cui poter inserire:

- i riferimenti esterni all'ordine

- una specifica Data di Scadenza

- l'eventuale selezione della causale del movimento di magazzino da
  adottare per la memorizzazione, all'interno del gestionale, di quello
  specifico documento.

E' possibile selezionare uno dei seguenti valori:

- **No:** in queste condizioni la sezione relativa ai Parametri del
  Documento non verrà mai visualizzata indipendentemente dal fatto che
  ad effettuare l'ordine sia un Agente oppure un Cliente

- **Agente:** in queste condizioni la sezione relativa ai Parametri del
  Documento verrà visualizzata solo ed esclusivamente nel caso in cui ad
  effettuare l'ordine sia un Agente.

- **Agente e Cliente:** in queste condizioni la sezione relativa ai
  Parametri del Documento verrà sempre visualizzata indipendentemente
  dal fatto che ad effettuare l'ordine sia un Agente oppure un Cliente.

> **NOTA BENE:** i dati inseriti dall\'agente all\'interno di questi
> campi verranno poi riportati in Mexal assieme all\'ordine nella
> relativa tabella dei \"**Riferimenti Esterni**\"
>
> Il valore del campo **"Data Scadenza"** viene impostato, inizialmente,
> secondo quanto specificato per il parametro "**Scadenza Documento**"
> alla pagina "Configurazione Ordini" del Wizard.
>
> Allo stesso modo il campo "Causale Movimento" verrà impostato, a
> default, con uno dei valori settati per i parametri "**Numero della
> Causale del Movimento di Magazzino Documento / Preventivo**" presenti
> anch'essi alla pagina "Configurazione Ordini" del Wizard (posto
> ovviamente che le relative causali siano state correttamente attivate)

**Nascondi Nota:** se selezionato consente di non visualizzare in fase
di conferma ordine la sezione attraverso cui poter inserire una nota di
corpo sul documento.

Eventuali note inserite all'interno di questo campo verranno poi
riportate nel corrispondente documento gestionale come note di corpo,
riportabili o meno a seconda di quanto impostato per il parametro "Note
sul Documento" presente alla pagina "Configurazione Parametri
dell'Ordine" del Wizard.

**Nascondi Spese di Spedizione:** consente, se selezionato, di non
visualizzare in fase di conferma ordine la sezione relativa alle spese
di spedizione

**ATTENZIONE!** Nel caso in cui si decida di non visualizzare la sezione
per la selezione delle spese di spedizione, Passweb potrà comportarsi in
maniera differente a seconda del fatto che il sito Ecommerce sia
collegato a Mexal oppure ad uno dei gestionali Ho.Re.Ca.

Nello specifico dunque:

**[SITI ECOMMERCE COLLEGATI A MEXAL]{.underline}**

Nel momento in cui si dovesse decidere di non visualizzare la sezione
per la selezione delle spese di spedizione, Passweb potrà comportarsi in
due modi differenti:

a)  Se il parametro **"Gestione del Trasporto Abituale"** presente nella
    pagina di configurazione ordini è stato impostato su uno dei due
    valori "**Abilitato**" o "**Abilitato Esclusivo**" e il cliente che
    effettua l'ordine ha effettivamente impostato nelle sue condizioni
    commerciali Mexal un vettore abituale, allora l'ordine prenderà in
    considerazione tale vettore.

b)  Se il parametro **"Gestione del Trasporto Abituale"** presente nella
    pagina di configurazione ordini è stato impostato sul valore "**Non
    Abilitato**" e/o il cliente che effettua l'ordine non ha alcun
    vettore abituale impostato nelle sue condizioni commerciali allora,
    per l'ordine in esame, non verrà utilizzato nessun vettore e
    conseguentemente **non verrà applicata nessuna spesa di
    spedizione.**

> In queste condizioni nel dettaglio del documento non verrà
> visualizzata la sezione relativa ai dati di spedizione e, in
> conseguenza di ciò, non verrà visualizzato neppure un eventuale codice
> di spedizione associato al documento in esame.

**[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI
HO.RE.CA.]{.underline}**

Nel momento in cui si dovesse decidere di non visualizzare la sezione
per la selezione delle spese di spedizione il relativo ordine verrà
sempre generato senza tenere conto di nessuna spesa di trasporto.

**Procedi se non ci sono spedizioni:** permette di decidere come dovrà
comportarsi l'applicativo nel momento in cui, per una qualsiasi ragione,
non dovessero essere presenti, in fase di checkout, spedizioni
selezionabili. Nello specifico dunque:

- Selezionando il parametro in esame sarà poi possibile procedere alla
  conferma dell'ordine anche nel caso in cui, in fase di checkout, non
  dovessero essere presenti spese di spedizione selezionabili.

> **In queste condizioni l'ordine inserito all'interno del gestionale
> sarà privo di qualsiasi spesa di trasporto.**

- Nel caso in cui il parametro in esame NON dovesse essere selezionato
  per procedere alla conferma dell'ordine dovrà necessariamente essere
  disponibile, in fase di checkout, almeno una spedizione selezionabile
  dall'utente

> In queste stesse condizioni, inoltre, nel momento in cui l'utente
> dovesse essere bloccato in fase di conferma ordine a causa di
> un'errata configurazione del sito e, nello specifico, a causa
> dell'assenza di una qualche modalità di spedizione effettivamente
> selezionabile, Passweb provvederà ad inviare automaticamente
> all'amministratore un'apposita mail di notifica contenente
> l\'indicazione dell\'utente che ha effettuato l'ordine e l\'indirizzo
> di spedizione da esso selezionato.

**Mostra popup se non ci sono spedizioni:** consente, se selezionato, di
visualizzare all'utente, all'interno di un apposito pop up, un messaggio
per informarlo che, nelle condizioni considerate, non sono presenti
spedizioni selezionabili e che non è quindi possibile procedere alla
conferma dell'ordine.

Tale pop up verrà quindi visualizzato solo ed esclusivamente nelle
seguenti condizioni:

- Parametro "**Tipologia Fase di Checkout = Visualizzazione senza Step
  Affiancato / Incolonnato**"

- Parametro "**Mostra popup se non ci sono spedizioni** "
  **selezionato**

- Parametro "**Procedi se non ci sono spedizioni**" **deselezionato**

I testi di questo messaggio possono essere personalizzati (in tutte le
lingue gestite) agendo all'interno della sezione "*Sito -- Testi /
Messaggi del sito -- Testi dei Componenti*" del Wizard -- componente
"**Checkout Custom (Ordine)**" , campi "**Scelta spedizione -- Nessun
elemento -- Testo bottone Popup / Testo Popup / Titolo Popup**"

**Visualizza Google Map dei Punti Vendita:** consente, se selezionato,
di visualizzare nello step relativo alla selezione della modalità di
spedizione, l'elenco di eventuali punti vendita all'interno di una
Google Map.

Il parametro in esame ha ovviamente influenza solo ed esclusivamente su
quei metodi di trasporto con associati dei punti vendita. Per maggiori
informazioni relativamente alla gestione dei punti vendita e alla loro
associazione a determinati metodi di trasporto si vedano anche le
sezioni "*Ordini -- Configurazione Metodi di trasporto -- Trasporti di
tipo Passweb*" e "*Ordini -- Configurazione Punti Vendita*" di questo
manuale

**ATTENZIONE! Come indicato da Google, dal 16 Luglio 2018 è entrato in
vigore un nuovo piano tariffario basato sul consumo per Maps, Routes e
Places.**

L'effettiva possibilità di utilizzare le Mappe Google all'interno del
proprio sito è quindi sottoposta al fatto di aver ottemperato a tutte le
richieste effettuate da Google stessa in merito alla fruizione di questo
tipo di servizio. Per maggiori informazioni in merito si veda anche la
sezione "*Sito -- Preferenze -- Seo Integrazioni -- Google Maps Api*" di
questo manuale.

Nel momento in cui l'utente dovesse selezionare in fase di checkout,
all'interno dell'apposito step, una modalità di spedizione (es. Ritiro
in Negozio) con associati dei Punti Vendita, verrà poi visualizzato
anche l'elenco di tali punti vendita e, questi stessi punti vendita
potranno essere localizzati (posto di aver selezionato il parametro in
esame) all'interno di una Google Map

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\punti_vendita_ordine.bmp](./assets/media/image287.png)

**ATTENZIONE**! Nel momento in cui si dovesse decidere di non
visualizzare i Puti Vendita all'interno della Google Map (parametro non
selezionato), quando l'utente andrà a selezionare una spedizione con
associati dei Punti Vendita verrà visualizzato solamente l'elenco di
questi punti vendita comprensivo dell'indirizzo e dell'eventuale
descrizione di ognuno di essi.

I punti vendita inizialmente visualizzati all'interno della mappa
saranno, ovviamente, tutti quelli presenti nella Nazione e nella
provincia definite dall'indirizzo di spedizione impostato dall'utente
stesso nello step precedente del Checkout.

**ATTENZIONE!** Nel caso in cui l'utente abbia effettuato, prima di
passare al checkout, un preventivo, in carrello, delle spese di
spedizione, l'indirizzo di spedizione e l'eventuale selezione di un
punto vendita saranno già impostati a default sulla base di quanto
richiesto dal cliente stesso in fase di preventivo.

In ogni caso il campo "Provincia", presente immediatamente al di sopra
dell'elenco dei punti vendita, permetterà all'utente di selezionare una
qualsiasi altra provincia presente nella Nazione di appartenenza dell'
Indirizzo di spedizione in cui risultano essere presenti dei punti
vendita.

In definitiva dunque l'utente non solo potrà selezionare come spedizione
la modalità "Ritiro in Negozio" ma potrà anche decidere esattamente in
quale dei punti vendita abilitati recarsi per ritirare la merce.

Inoltre, al verificarsi delle seguenti condizioni:

- Il magazzino associato al punto vendita selezionato è anche uno di
  quelli indicati per il calcolo della disponibilità articolo (sezione
  'Disponibilità' della maschera "Configurazione Catalogo")

- Il parametro "Gestione Acquisto" (sezione "Disponibilità" della pagina
  "Configurazione Catalogo" del Wizard) è impostato su "Acquista solo se
  disponibile"

una volta selezionato il punto vendita verrà effettuato sul magazzino ad
esso associato, per gli articoli in ordine, un controllo della
disponibilità.

Se il controllo dovesse dare esito positivo, il punto vendita verrà
correttamente selezionato e si potrà procedere alla conferma
dell'ordine.

Nel caso in cui invece il controllo dovesse dare esito negativo verrà
visualizzato un apposito messaggio indicante le mancate disponibilità e
il punto vendita non potrà essere selezionato (il testo del messaggio
può essere modificato alla sezione "Testi/Messaggi del Sito" agendo sul
componente "Aggiunta al Carrello" e modificando il testo "Massima
disponibilità negozio")

Per maggiori informazioni relativamente a come poter associare un
magazzino ad un punto vendita si veda anche quanto indicato all'interno
del capitolo "*Ordini -- Punti Vendita*" di questo manuale.

La selezione di un ben determinato punto vendita farà si che:

- **nel piede del documento gestionale venga inserito esattamente
  l'indirizzo del punto vendita selezionato dall'utente.**

> In queste condizioni quindi non verrà considerato l'indirizzo di
> spedizione selezionato dall'utente nel relativo step del checkout
> (indirizzo questo che verrà quindi preso in considerazione ed inserito
> nel piede del documento solo ed esclusivamente nel caso in cui
> l'utente desideri farsi spedire la merce a casa)

- **se al punto vendita selezionato dovesse essere stato associato uno
  specifico magazzino**, tale magazzino verrà utilizzato al posto di
  quello indicato in "Configurazione Ordini", come magazzino di testata
  del relativo documento gestionale

**Nascondi Pagamento:** consente, se selezionato, di non visualizzare in
fase di conferma ordine la sezione relativa ai metodi di pagamento.

**ATTENZIONE!** Nel caso in cui si decida di non visualizzare la sezione
relativa alla selezione della modalità di pagamento Passweb potrà
comportarsi in due modi differenti:

a)  Se il parametro **"Gestione del Pagamento Abituale"** presente nella
    pagina di configurazione ordini è stato impostato sul valore SI e il
    cliente che effettua l'ordine ha effettivamente impostato nelle sue
    condizioni commerciali definite all'interno del gestionale un
    pagamento abituale, verrà allora applicato all'ordine questo
    specifico pagamento, con le relative eventuali spese accessorie.

b)  Se il parametro **"Gestione del Pagamento Abituale"** presente nella
    pagina di configurazione ordini è stato impostato sul valore NO o il
    cliente che effettua l'ordine non ha alcun pagamento abituale
    impostato nelle sue condizioni commerciali, allora **l'ordine
    nascerà con la tipologia di Pagamento non impostata.**

**Procedi se non ci sono Pagamenti:** permette di decidere come dovrà
comportarsi l'applicativo nel momento in cui, per una qualsiasi ragione,
non dovessero essere presenti, in fase di checkout, pagamenti
selezionabili. Nello specifico dunque:

- Selezionando il parametro in esame sarà poi possibile procedere alla
  conferma dell'ordine anche nel caso in cui, in fase di checkout, non
  dovessero essere presenti pagamenti selezionabili.

> **In queste condizioni l'ordine verrà inserito all'interno del
> gestionale con il campo relativo al pagamento non valorizzato.**

- Nel caso in cui il parametro in esame NON dovesse essere selezionato
  per procedere alla conferma dell'ordine dovrà necessariamente essere
  disponibile, in fase di checkout, almeno una modalità di pagamento
  effettivamente selezionabile dall'utente

> In queste stesse condizioni, inoltre, nel momento in cui l'utente
> dovesse essere bloccato in fase di conferma ordine a causa di
> un'errata configurazione del sito e, nello specifico, a causa
> dell'assenza di una qualche modalità di pagamento effettivamente
> selezionabile, Passweb provvederà ad inviare automaticamente
> all'amministratore un'apposita mail di notifica contenente
> l\'indicazione dell\'utente che ha effettuato l'ordine e l\'indirizzo
> di spedizione da esso selezionato.

**Mostra popup se non ci sono pagamenti:** consente, se selezionato, di
visualizzare all'utente, all'interno di un apposito pop up, un messaggio
per informarlo che, nelle condizioni considerate, non sono presenti
metodi di pagamento selezionabili e che non è quindi possibile procedere
alla conferma dell'ordine.

Tale pop up verrà quindi visualizzato solo ed esclusivamente nelle
seguenti condizioni:

- Parametro "**Tipologia Fase di Checkout = Visualizzazione senza Step
  Affiancato / Incolonnato**"

- Parametro "**Mostra popup se non ci sono pagamenti**" **selezionato**

- Parametro "**Procedi se non ci sono pagamenti**" **deselezionato**

I testi di questo messaggio possono essere personalizzati (in tutte le
lingue gestite) agendo all'interno della sezione "*Sito -- Testi /
Messaggi del sito -- Testi dei Componenti*" del Wizard -- componente
"**Checkout Custom (Ordine)**" , campi "**Scelta pagamento -- Nessun
elemento -- Testo bottone Popup / Testo Popup / Titolo Popup**"

**Visualizza Ricerca Indirizzo:** valido solo nel caso in cui non sia
stato abilitato il modulo di One Step Checkout. Consente di decidere se
abilitare o meno in fase di conferma ordine, nella sezione relativa
all'indicazione dell'indirizzo di spedizione merce, un apposito campo di
ricerca grazie al quale poter filtrare i vari indirizzi di spedizione
associati all'utente che sta effettuando l'ordine.

**Gestione Allegati:** consente di abilitare o meno la gestione degli
allegati sul componente di checkout.

Se impostato a SI, gli utenti del sito avranno quindi la possibilità di
allegare determinati file al proprio ordine direttamente dal modulo di
checkout.

Al contrario nel momento in cui il parametro in questione dovesse essere
impostato su No, eventuali allegati all'ordine potranno essere aggiunti
e gestiti solo ed esclusivamente dall'amministratore del sito operando
per questo dal gestionale (mediante Docuvision) oppure direttamente dal
Wizard di Passweb ma, in ogni caso, sempre dopo che l'ordine in esame
sia stato correttamente memorizzato.

**ATTENZIONE!** Per maggiori informazioni relativamente alla possibilità
di allegare determinati documenti agli ordini effettuati all'interno del
sito si veda anche il successivo paragrafo "**Ordini -- Gestione
Allegati**"

Infine, per comprendere al meglio il significato dei restanti parametri
presenti all'interno della maschera di configurazione del Componente
Ordine, è bene ricordare che una volta inserite e confermate le
informazioni richieste, verrà visualizzato, in un ulteriore step di
conferma oppure come riassunto dell'ordine appena effettuato, un
dettaglio con tutti i dati relativi agli articoli presenti in ordine, al
pagamento selezionato, al metodo di trasporto ecc...

In particolare per quel che riguarda l'elenco degli articoli in ordine
questo è strutturato (come già visto per il componente carello o per il
componente wishlist) su di una griglia responsiva le cui colonne possono
essere definite direttamente all'interno della sezione "**Gestione
Contenuti**" presente nella maschera di gestione e configurazione del
Componente stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ordine_custom_1_res.bmp](./assets/media/image288.png)

**ATTENZIONE!** Come precedentemente evidenziato all'interno di questo
stesso capitolo, i dati visualizzati per ogni articolo in ordine, sono,
a default, gli stessi che verranno visualizzati anche in un eventuale
riepilogo mostrato nelle precedenti fasi di checkout (parametro
"**Mostra Riepilogo Affiancato = Si**").

Nel momento in cui l'esigenza dovesse essere dunque quella di
visualizzare, nel riepilogo delle precedenti fasi di checkout, un numero
di informazioni inferiore (es. solo immagine, titolo e codice articolo)
rispetto a quelle effettivamente presenti nel dettaglio del documento
visualizzato invece in questa fase, sarà necessario **nascondere**,
all'interno del riepilogo, i relativi componenti assegnando loro la
classe addizionale "**hidesummary**" (utilizzando per questo l'apposito
campo presente nella maschera di configurazione di ogni componente
Passweb)

All'interno della griglia articoli, inoltre, può essere presente, nel
caso in cui si stia consultando il dettaglio di una matrice (Ecommerce
Mexal) importata dal gestionale, anche una colonna con due pulsanti
mediante i quali poter eliminare dalla matrice il corrispondente
articolo oppure aggiungerlo in carrello

Per maggiori informazioni relativamente alla gestione delle matrici si
veda anche la corrispondente sezione di questo manuale ("*Ordini --
Gestione Matrici*")

Fatta questa considerazione, possiamo ora comprendere in maniera più
semplice il significato degli ultimi parametri presenti nella maschera
di configurazione del componente Ordine.

Nello specifico dunque il parametro:

**Larghezza Colonna dei Bottoni:** consente di impostare la larghezza
che dovrà assumere, all'interno della griglia articoli, la colonna dei
pulsanti (aggiungi al carrello, elimina articolo).

**ATTENZIONE!** La colonna dei bottoni verrà visualizzata solo ed
esclusivamente nel momento in cui si stia consultando il dettaglio di
una matrice (Ecommerce Mexal) importata direttamente dal gestionale

Come per tutte le griglie responsive anche in questo caso la larghezza
di ogni colonna (compresa quella dei bottoni) si esprime definendo
quante delle 12 sezioni in cui risulta essere suddivisa ogni singola
riga, dovranno essere effettivamente occupate dalla colonna stessa.

**Posizionamento Colonna dei Bottoni**: consente di decidere se la
colonna dei bottoni dovrà essere posizionata a sinistra oppure a destra
delle informazioni relative allo specifico articolo

**Posizione dei campi di riepilogo dei Totali:** consente di definire
come dovranno essere posizionati i campi relativi al "Totale Merce",
"Iva", "Spese di trasporto" ecc... E' possibile selezionare una delle
seguenti opzioni:

- Allineati a Destra

- Allineati a Sinistra

- Centrati

- Opposti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ordine_riepilogo_totali.bmp](./assets/media/image289.png)

> Nell'esempio in figura il parametro "**Posizione dei campi di
> riepilogo dei Totali**" è stato impostato sul valore "**Allineati a
> destra**"

**ATTENZIONE!** Indipendentemente da quella che sarà la larghezza
impostata per ogni singola colonna della griglia articoli il suo
comportamento responsivo è tale per cui **in corrispondenza di
risoluzioni inferiori ai 992 px la griglia stessa si linearizzerà
disponendo tutte le colonne una sotto l'altra**

Una volta settati i parametri di configurazione del Componente sarà
quindi necessario definirne i contenuti stabilendo innanzitutto il
numero di colonne in cui dovrà essere suddivisa ogni singola riga
articolo e, successivamente, andando ad inserire in queste stesse
colonne i componenti desiderati (Titolo, Prezzo, Immagine ecc...).

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

