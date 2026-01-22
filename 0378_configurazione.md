# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello_custom_configurazione_res.bmp](./assets/media/image137.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" è possibile inserire il
contenuto e settare i principali parametri di configurazione del
componente stesso.

In particolare, per la tipologia di Componente in questione, è possibile
impostare un valore per i seguenti parametri:

**Nome**: consente di definire un nome per il Componente che si sta
editando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato, il
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

**Gestione Wishlist:** consente di abilitare o meno l'interazione tra il
**"Carrello Custom"** e il componente **"Wishlist"**.

In particolare, dunque, selezionando tale parametro, all'interno del
Carrello verrà visualizzato, in corrispondenza di ogni singola riga, un
ulteriore pulsante (**Wishlist**) attraverso cui l'utente potrà
aggiungere il relativo articolo (comprensivo dell'esatta quantità
attualmente impostata) alla propria lista dei desideri.

Abilitando questo parametro verrà visualizzato inoltre anche il pulsante
**"Aggiungi tutto alla Wishlist"** mediante il quale poter aggiungere
alla propria lista dei desideri tutti gli articoli (con le relative
quantità) attualmente presenti in Carrello.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_custom_2.bmp](./assets/media/image138.png)

Per maggiori informazioni relativamente alla gestione in Passweb delle
"Liste dei desideri" (Wishlist) si veda anche la sezione di questo
manuale relativa al componente E-commerce "Wishlist".

**Aggiornamento dati:** consente di impostare la modalità di
aggiornamento dei dati (quantità, note, sconti, date di scadenza)
relativamente agli articoli attualmente presenti in carrello. E'
possibile selezionare uno dei seguenti valori:

- **Singola Riga:** in questo caso eventuali variazioni a quantità, date
  di scadenza, note e/o sconti apportate ad uno degli articoli presenti
  in carrello dovranno essere necessariamente confermate cliccando sul
  pulsante "**Aggiorna Dati**" presente all'interno della relativa riga
  articolo

![Videate\\carrello_custom_3.bmp](./assets/media/image139.png)

> **ATTENZIONE!** Nel momento in cui l'utente NON dovesse cliccare sul
> pulsante di aggiornamento, eventuali variazioni apportate ad una riga
> articolo non verranno salvate e potrebbero quindi andar perse se
> l'utente dovesse decidere di cambiare pagina

- **Intero Carrello:** in questo caso eventuali variazioni a quantità,
  date di scadenza, note e/o sconti apportate ad uno o più articoli
  presenti in carrello dovranno essere confermate in blocco cliccando
  sul pulsante "**Aggiorna Carrello**" presente nella parte bassa del
  componente

![Videate\\carrello_custom_4.bmp](./assets/media/image140.png)

> **ATTENZIONE!** Nel momento in cui l'utente NON dovesse cliccare sul
> pulsante evidenziato in figura, eventuali variazioni apportate ad una
> o più righe articolo non verranno salvate e potrebbero quindi andar
> perse se l'utente dovesse decidere di cambiare pagina

- **Automatico:** in questo caso eventuali variazioni a quantità, date
  di scadenza, note e/o sconti apportate ad uno degli articoli presenti
  in carrello verranno automaticamente salvate spostando semplicemente
  il cursore da un campo all'altro della stessa riga e/o da una riga
  all'altra del carrello.

**Visualizzazione Paginazione:** consente di decidere se e dove
visualizzare (rispetto al Componente stesso) i collegamenti alle varie
pagine che si attiveranno nel caso in cui il numero complessivo di
articoli presenti in carrello sia superiore a quello impostato
all'interno del campo "Numero di articoli da Visualizzare".

**Numero di Articoli da Visualizzare:** consente di impostare il numero
di articoli che dovranno essere visualizzati per ogni singola pagina.
Nel caso in cui il numero complessivo di articoli presenti in carrello
sia superiore a quello impostato all'interno di questo campo, verrà
attivato un sistema di paginazione per consentire all'utente di
visualizzare tutti gli articoli presenti

**Numero di Pagine:** consente di impostare, selezionandolo dal relativo
menu a tendina, il numero di pagine che dovranno essere visualizzate nei
controlli di paginazione. Ovviamente oltre al numero indicato
all'interno di questo campo, nei controlli di paginazione saranno sempre
visibili anche la prima e l'ultima pagina disponibili.

**Paginazione con Precedente e Successivo:** se selezionato, nei
controlli di paginazione, verranno visualizzati anche i pulsanti
"Precedente" e "Successivo".

**Visualizzazione Risultati:** consente di visualizzare, nella parte
bassa del componente, una stringa di testo con il numero complessivo di
righe articolo attualmente presenti in carrello.

**Mostra Riepilogo Quantità Articoli:** consente di visualizzare un
riepilogo relativo al numero totale di articoli attualmente presenti in
carrello, suddivisi o meno per categorie merceologiche.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_custom_5.bmp](./assets/media/image141.png)

E' possibile selezionare uno dei seguenti valori:

- **Non Visualizzare:** in questo caso non verranno visualizzate
  informazioni relativamente al numero o alla quantità complessiva di
  articoli in carrello

- **Solo Totale Quantità:** selezionando questa opzione verrà
  visualizzata la quantità totale di articoli (Totale articoli) e il
  numero di righe articolo (Numero Articoli) presenti in carrello.

> Ovviamente nel calcolo del numero di articoli presenti in carrello non
> verranno considerati eventuali articoli di tipo spesa utilizzati ad
> esempio per gestire promozioni e/o buoni sconto.

- **Quantità suddivisa per categoria:** come nel caso precedente, anche
  in queste condizioni, verrà visualizzata la quantità e il numero
  totale di articoli in carrello. In queste condizioni, inoltre, la
  quantità totale di articoli in carrello, verrà ulteriormente
  dettagliata e suddivisa per categoria merceologica.

> **ATTENZIONE!** Relativamente ad articoli gestiti a confezioni, verrà
> considerato, nel calcolo della quantità totale di articoli in
> carrello, il numero dei colli piuttosto che le singole unità presenti
> in ciascuna confezione, dipendentemente dalle impostazioni settate per
> il parametro "**Totale Quantità Articoli**" presente alla maschera
> *"Configurazione Catalogo Mexal*" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\totale_quantita_articoli.bmp](./assets/media/image142.png)

> Per maggiori informazioni in merito al parametro evidenziato in figura
> si veda anche la sezione "*Catalogo -- Configurazione Parametri
> Catalogo -- Catalogo Mexal -- Gestione Confezione*" di questo manuale

**Visualizza 'Continua con lo Shopping':** consente di visualizzare, se
selezionato, un pulsante attraverso il quale implementare un
collegamento alla pagina "Negozio" del sito.

**Visualizza Saldo Gift Card:** consente di visualizzare, se
selezionato, la sezione "Gift Card" all'interno della quale comparirà il
check "Usa il saldo" con a fianco l'importo di eventuali Gift Card,
caricate sull'account dell'utente, e spendibile per l'ordine in esame

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\attivazione_giftcard_4.bmp](./assets/media/image143.png)

Ovviamente affinché la sezione "Gift Card" possa essere effettivamente
visualizzata non è sufficiente selezionare il parametro in questione ma
è anche necessario che:

- l'utente abbia già effettuato la login al sito

- l'utente abbia un saldo Gift Card effettivamente spendibile per
  l'ordine in esame.

Dovranno quindi essere presenti sull'account dell'utente Gift Card
attive con saldo diverso da zero e configurate con condizioni di
applicabilità tali da soddisfare quelli che sono effettivamente gli
articoli presenti in carrello.

**ATTENZIONE!** l'importo visualizzato in corrispondenza del check
"**Usa il saldo**" **è quello effettivamente spendibile per l'ordine
corrente e non il saldo globale delle Gift Card caricate sull'account
dell'utente (**che è invece visibile solo all'interno del componente
"Gift Card")

Verranno quindi già determinati, in maniera completamente automatica,
gli importi effettivamente spendibili per l'ordine corrente sulla base
di quanto indicato, in fase di configurazione di ogni singola Gift Card,
in relazione ai campi "**Applicazione utilizzo**" e "**Condizioni**".

**NOTA BENE:** per maggiori informazioni relativamente a come poter
pagare degli ordini utilizzando una Gift Card si veda la corrispondente
sezione di questo manuale (Varianti sito responsive -- Lista Componenti
Ecommerce -- Componente Gift Card -- Come effettuare acquisti
utilizzando un Carta Regalo ).

**Visualizza "Scarico Punti":** consente di visualizzare, se
selezionato, la sezione "**Punti Premio**" all'interno della quale
comparirà il check "**Usa il saldo**" con a fianco l'indicazione del
numero massimo di punti gestibili per l'ordine in esame e il
corrispondente importo espresso nella valuta corrente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\punti_premio_carrello.bmp](./assets/media/image144.png)

Ovviamente affinché la sezione "Punti Premio" possa essere
effettivamente visualizzata non è sufficiente selezionare il parametro
in questione ma è anche necessario che:

- l'utente abbia già effettuato la login al sito

- l'utente abbia un Saldo Punti non nullo

Relativamente al numero di punti visualizzati all'interno di questa
sezione e al corrispondente importo in valuta, occorre poi considerare
che:

- Il numero di punti utilizzabili verrà arrotondato per difetto o per
  eccesso (rispetto al Totale Merce / Ordine) dipendentemente
  dall'impostazione settata per il campo "**Arrotondamento punti
  copertura**" presente tra i parametri di configurazione generali della
  raccolta punti attualmente attiva sul sito**.**

- Nel computo totale dei punti utilizzabili verranno considerati per
  primi, in automatico, quelli con la scadenza più prossima

- In caso di modifica di un ordine sospeso verranno riconsiderati anche
  gli eventuali punti spesi nell'ordine iniziale

- L'importo in valuta visualizzato in corrispondenza del check "**Usa il
  saldo**" dipende da come è stato configurato il sistema di raccolta
  punti attualmente attivo sul sito e, nello specifico, dal valore
  assegnato al singolo punto

Per maggiori informazioni in merito alla possibilità di attivare
all'interno del proprio sito ecommerce un sistema di raccolta punti si
veda anche quanto indicato nel capitolo "*Utenti -- Punti*" di questo
manuale

Per maggiori informazioni relativamente invece a come poter pagare degli
ordini utilizzando i punti accumulati a seguito di precedenti acquisti
si veda quanto indicato all'interno della sezione "*Varianti sito
responsive -- Lista Componenti Ecommerce -- Componente Punti Premio --
Come effettuare acquisti utilizzando Punti Premio"* di questo manuale.

Infine, nel momento in cui sul sito dovesse essere attivo un sistema di
raccolta punti, nel riepilogo dei totali in carrello verranno
visualizzate, tra le altre, anche le voci "**Punti Guadagnati**" e
"**Punti Spesi**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\punti_premio_carrello_2.bmp](./assets/media/image145.png)

con l'indicazione rispettivamente dei punti che l'utente andrebbe
effettivamente a guadagnare nel momento in cui dovesse chiudere quel
carrello e dei punti che verrebbero invece sottratti dal suo saldo nel
momento in cui dovesse decidere di utilizzare quelli fin' ora
accumulati.

**ATTENZIONE!** I punti accumulati potranno essere utilizzati solo ed
esclusivamente per ordini successivi a quelli che hanno prodotto il
relativo accumulo

**Visualizza "Applica Buono Sconto":** consente di visualizzare, se
selezionato, un modulo attraverso il quale l'utente potrà applicare
eventuali codici sconto in suo possesso e verificare, già all'interno
del carrello, come i relativi sconti andranno a modificare il totale
merce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello-preventivo-buono-sconto.bmp](./assets/media/image146.png)

L'utente dovrà quindi inserire all'interno dell'apposito modulo il
Codice Sconto in suo possesso e cliccare successivamente sul pulsante
"**Aggiorna Totali Carrello**".

L'applicazione si preoccuperà di verificare la correttezza e la validità
del codice inserito e di aggiornare conseguentemente il Totale Carrello
tenendo conto dello sconto associato al Codice inserito dall'utente.

**NOTA BENE:** per maggiori informazioni relative alla gestione dei
Buoni Sconto si veda la corrispondente sezione di questo manuale (Ordini
-- Configurazione Buoni Sconto).

**Visualizza "Stima dei Costi di Spedizioni":** consente di
visualizzare, se selezionato, un modulo attraverso il quale l'utente
potrà ottenere un preventivo dei costi di spedizione direttamente
all'interno della pagina carrello e volendo, dunque, senza aver ancora
effettuato l'autenticazione al sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello-preventivo-spedizioni.bmp](./assets/media/image147.png)

**ATTENZIONE!** Indipendentemente dal fatto di aver attivato o meno il
parametro in esame, nel momento in cui in carrello dovessero essere
presenti solo articoli di tipo "**Gift Card Virtuali**" il modulo per il
preventivo dei costi di spedizione non verrà mai visualizzato (per
maggiori informazioni in merito alla gestione delle Gift Card si veda il
relativo capitolo "*Utenti -- Gift Card*" di questo manuale)

Una volta abilitato il modulo l'utente dovrà poi inserire all'interno
degli appositi campi i riferimenti (Nazione, Provincia e CAP) in
relazione ai quali desidera richiedere il preventivo dei costi di
spedizione. Cliccando quindi sul pulsante "**Ottieni un preventivo**"
verranno visualizzati tutti i metodi di trasporto opportunamente
codificati all'interno dell'apposita sezione del Wizard, e legati alla
zona geografica indicata dall'utente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello-preventivo-spedizioni2.bmp](./assets/media/image148.png)

Nel caso in cui l'utente dovesse selezionare un metodo di trasporto con
associati dei Punti Vendita (es. Ritiro in Negozio) verrà visualizzato
l'elenco di tali punti vendita e, questi stessi punti vendita potranno
anche essere localizzati (dipendentemente da come è stato impostato il
successivo parametro "**Visualizza Google Map dei Negozi**") all'interno
di una Google Map

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\punti_vendita_carrello.bmp](./assets/media/image149.png)

I punti vendita inizialmente visualizzati all'interno della mappa
saranno tutti quelli presenti nella Nazione e nella provincia
precedentemente selezionata dall'utente.

Nel caso in cui l'utente prima di richiedere il preventivo delle spese
di spedizione abbia indicato solamente la nazione verranno visualizzati
tutti i punti vendita di quella stessa nazione indipendentemente dalla
loro provincia di appartenenza.

Il campo "Provincia" presente immediatamente al di sopra dell'elenco dei
punti vendita consentirà poi di restringere ulteriormente la ricerca
selezionando una specifica provincia tra quelle in cui risultano essere
presenti dei punti vendita.

In definitiva dunque l'utente non solo potrà selezionare come spedizione
la modalità "Ritiro in Negozio" ma potrà anche decidere esattamente in
quale dei punti vendita abilitati recarsi per ritirare la merce.

**In queste condizioni nel piede del documento gestionale verrà inserito
esattamente l'indirizzo del punto vendita selezionato dall'utente**

**ATTENZIONE!** Per maggiori informazioni relativamente alla gestione
dei punti vendita e alla loro associazione a determinati metodi di
trasporto si vedano anche le sezioni "*Ordini -- Configurazione Metodi
di trasporto -- Trasporti di tipo Passweb*" e "*Ordini -- Configurazione
Punti Vendita*" di questo manuale

Una volta selezionato il metodo di trasporto (ed eventualmente lo
specifico punto vendita) desiderato, il pulsante "**Aggiorna Totale**"
consentirà all'utente di completare il preventivo aggiornando il totale
merce del carrello con l'importo relativo al metodo di trasporto
selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello-preventivo-spedizioni3.bmp](./assets/media/image150.png)

Il metodo di trasporto selezionato all'interno del carrello in fase di
preventivo, verrà poi riportato e mantenuto anche all'interno del
checkout ordine (compresa la selezione di un eventuale punto vendita),
solo ed esclusivamente nel caso in cui sia uno dei metodi di trasporto
consentiti per l'utente che andrà poi ad effettuare il login per portare
a termine l'ordine.

In ogni caso dopo aver effettuato il login sarà sempre possibile variare
il metodo di trasporto selezionato direttamente all'interno del
checkout.

**ATTENZIONE!** **L'indirizzo di spedizione merce potrebbe influire
anche sull'importo di eventuali tasse addizionali (es. CONAI, RAEE ...)
o Tasse IVA cui potrebbe essere soggetto un determinato articolo** (per
maggiori informazioni in merito si veda anche quanto indicato
all'interno del capitolo "*Ordini -- Tasse*" di questo manuale).

Nel momento in cui si dovessero gestire dunque articoli soggetti a Tasse
Addizionali o Tasse di tipo IVA, **è assolutamente consigliato abilitare
sempre la "Stima dei Costi di Spedizione"** in maniera tale che
l'utente, già in questa fase, possa indicare un ben preciso indirizzo di
spedizione merce e valutare in relazione ad esso anche l'esatto importo
che verrebbe a pagare nel momento in cui dovesse poi decidere di
chiudere l'ordine con quel determinato indirizzo di spedizione.

**Visualizza Google Map dei Negozi:** consente, se selezionato, di
visualizzare nel pannello relativo al preventivo delle spese di
spedizione, l'elenco di eventuali punti vendita all'interno di una
Google Map. Selezionando questo parametro la descrizione di un punto
vendita verrà visualizzata nel fumetto del relativo marker presente
all'interno della Google Map.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\punti_vendita_carrello.bmp](./assets/media/image149.png)

**ATTENZIONE! Come indicato da Google, dal 16 Luglio 2018 è entrato in
vigore un nuovo piano tariffario basato sul consumo per Maps, Routes e
Places.**

L'effettiva possibilità di utilizzare le Mappe Google all'interno del
proprio sito è quindi sottoposta al fatto di aver ottemperato a tutte le
richieste effettuate da Google stessa in merito alla fruizione di questo
tipo di servizio. Per maggiori informazioni in merito si veda anche la
sezione "*Sito -- Preferenze -- Seo Integrazioni -- Google Maps Api*" di
questo manuale.

Nel caso in cui si decida di non abilitare questo parametro, nel momento
in cui l'utente dovesse poi selezionare, all'interno del pannello
relativo al preventivo sulle spese di spedizione, un metodo di trasporto
con dei punti vendita associati, verrà visualizzato solamente l'elenco
di questi punti vendita comprensivo dell'indirizzo e dell'eventuale
descrizione di ognuno di essi

**ATTENZIONE!** Il parametro in esame ha ovviamente influenza solo ed
esclusivamente su quei metodi di trasporto con associati dei punti
vendita

**Visualizza Stima dei Costi di Pagamento:** consente di visualizzare,
se selezionato, un modulo attraverso il quale l'utente potrà
visualizzare l' elenco dei possibili pagamenti in maniera tale da
riuscire ad ottenere, già in carrello, un preventivo di spesa anche in
relazione a questo specifico elemento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello-preventivo-pagamenti.bmp](./assets/media/image151.png)

**L'elenco dei possibili pagamenti visualizzati all'interno di questo
modulo potrebbe variare in relazione a diversi fattori.** Qualora, ad
esempio, si sia deciso di attivare anche il modulo per la stima dei
costi di spedizione, una volta selezionata e confermata una ben precisa
modalità di trasporto verrà automaticamente aggiornato anche l'elenco
dei possibili pagamenti escludendo quelli non ammessi per il trasporto
selezionato.

Per maggiori informazioni relativamente alla possibilità di legare un
particolare pagamento ad una specifica modalità di spedizione, ad un
gruppo utente o al raggiungimento di un valore minimo del totale merce
si veda anche la sezione "*Ordini -- Configurazione Metodi di
Pagamento*" di questo manuale

Una volta selezionato il pagamento desiderato, il pulsante "**Aggiorna
Totale**" consentirà all'utente di completare il preventivo aggiornando
il totale merce del carrello con l'importo relativo ad eventuali costi
aggiuntivi legati al pagamento indicato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrello-preventivo-pagamenti2.bmp](./assets/media/image152.png)

**ATTENZIONE!** Se in seguito alla selezione di uno specifico pagamento
e alla conseguente aggiunta in carrello dei costi aggiuntivi ad esso
associati l'importo del totale merce, la particolare modalità di
trasporto selezionata o il gruppo di appartenenza dell'utente loggato,
dovessero portare all'esclusione del pagamento inizialmente selezionato,
la voce di spesa relativa a tale pagamento verrà automaticamente rimossa
dai totali del carrello.

Il pagamento indicato all'interno della pagina carrello in fase di
preventivo, verrà poi riportato e mantenuto anche all'interno del
checkout ordine solo ed esclusivamente nel caso in cui siano ancora
valide tutte le condizioni di applicabilità di questo stesso pagamento.

In ogni caso dopo aver effettuato il login sarà sempre possibile variare
il pagamento selezionato direttamente all'interno del checkout ordine.

**Visualizza anche le Taglie a Quantità uguale a zero (solo Ecommerce
Mexal):** consente di decidere se dovranno o meno essere visualizzate in
carrello, nel caso di articoli gestiti a taglie/colori, anche le opzioni
a quantità zero. E' possibile selezionare uno dei seguenti valori:

- **No:** in queste condizioni, per articoli gestiti a taglie/colori,
  verranno visualizzate in carrello le sole opzioni a quantità diversa
  da zero. Nel caso in cui l'utente dovesse quindi aggiungere al proprio
  ordine una nuova taglia/colore dovrà necessariamente farlo dalla
  relativa pagina prodotto.

- **Agente:** in queste condizioni solo nel caso in cui ad effettuare
  l'ordine sia un Agente (per conto di un suo cliente) verranno
  visualizzate in carrello, per articoli gestiti a taglie/colori, anche
  le opzioni a quantità zero. Nel caso in cui l'Agente dovesse quindi
  aggiungere al proprio ordine una nuova taglia/colore, potrà farlo
  direttamente dalla pagina Carrello senza dover per forza di cose
  tornare alla relativa pagina prodotto

- **Agente e Cliente:** in queste condizioni per articoli gestiti a
  taglie/colori, verranno sempre visualizzate in carrello anche le
  opzioni a quantità zero. In queste condizioni dunque nel caso in cui
  l'utente (sai esso un cliente o un Agente) dovesse quindi aggiungere
  al proprio ordine una nuova taglia/colore, potrà farlo direttamente
  dalla pagina Carrello senza dover per forza di cose tornare alla
  relativa pagina prodotto.

**Posizione campo Autocompletamento:** consente di definire la posizione
in cui dovrà essere visualizzata, all'interno del carrello custom,
l'eventuale riga contenente il modulo per la ricerca e l'inserimento
rapido di articoli in carrello.

E' possibile selezionare uno dei seguenti valori:

- **Inizio:** selezionando questa opzione l'eventuale riga contenente il
  modulo per l'inserimento rapido di articoli in carrello verrà
  posizionata sempre come prima riga del carrello

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_custom_7.bmp](./assets/media/image153.png)

- **Prima delle promozioni:** selezionando questa opzione l'eventuale
  riga contenente il modulo per l'inserimento rapido di articoli in
  carrello verrà posizionata come ultima riga del carrello ma comunque
  **sempre prima di eventuali righe non editabili** relative, ad
  esempio, ad articoli aggiunti automaticamente in carrello a seguito
  dell'applicazione di determinate promozioni e/o di determinati sconti
  o spese aggiuntive.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_custom_9.bmp](./assets/media/image154.png)

- **Fine:** selezionando questa opzione l'eventuale riga contenente il
  modulo per l'inserimento rapido di articoli in carrello verrà
  posizionata sempre come ultima riga del carrello

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_custom_8.bmp](./assets/media/image155.png)

Per maggiori informazioni relativamente al modulo di inserimento rapido
di articoli in carrello si veda anche il capitolo "*Live Editing per
Varianti Responsive -- Lista Componente Ecommerce -- Componenti Interni
ai Componenti Ecommerce -- Autocompletamento (Carrello Custom)*" di
questo manuale

**Posizionamento campo Checkout**: consente di decidere dove dovrà
essere visualizzato il pulsante di Checkout. E' possibile selezionare
una delle seguenti opzioni:

- Dopo i totali

- Insieme agli altri bottoni

**Ordinamento righe carrello**: consente di definire l'ordinamento che
verrà poi applicato agli articoli inseriti in carrello. E' possibile
selezionare una delle seguenti opzioni:

- Ordinamento data crescente

- Ordinamento data decrescente

- Titolo A-Z

- Titolo Z-A

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere, ad
esempio, quella di fare in modo che l'ultimo articolo inserito in
carrello sia il primo della lista sarà sufficiente impostare il
parametro in esame sull'opzione "Ordinamento data decrescente"

Per comprendere al meglio il significato dei successivi parametri di
configurazione del Carrello è necessario evidenziare quelli che sono i
singoli elementi che andranno a comporre, sul front end del sito, questo
tipo di Componente.

In questo senso dunque possiamo dire che ogni Componente Carrello è
composto da una griglia principale, perfettamente responsiva e
strutturata su due diverse colonne, la "**Colonna Articoli**" e la
"**Colonna Totali**" contenenti rispettivamente:

- L'elenco degli Articoli attualmente presenti in carrello

- I moduli per l'applicazione dei Buoni Sconto, il calcolo dei
  Preventivi e i Totali documento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res1.bmp](./assets/media/image156.png)

Per quel che riguarda l'elenco degli articoli attualmente presenti in
carrello (Colonna Articoli) questo è strutturato, a sua volta, su di una
griglia responsiva le cui colonne possono essere definite direttamente
all'interno della sezione "**Gestione Contenuti**" presente nella
maschera di gestione e configurazione del Carrello stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res2.bmp](./assets/media/image157.png)

Infine, immediatamente al di sotto della "Griglia Articoli" vengono
posizionati tutta una serie di pulsanti identificativi delle diverse
possibili azioni che possono essere effettuate dall'utente che sta
completando l'ordine (es. Aggiungi tutto alla Wishlist, Svuota Carrello,
Continua con lo Shopping ecc...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res3.bmp](./assets/media/image158.png)

Il pulsante per la conferma del Carrello ed il conseguente passaggio
alla fase di checkout è collocato invece immediatamente al di sotto dei
totali documento.

Una volta individuati i singoli elementi componenti il Carrello,
possiamo ora comprendere in maniera più semplice i restanti parametri di
configurazione del componente.

Nello specifico dunque il parametro:

**Larghezza Colonna dei Bottoni:** consente di impostare la larghezza
che dovrà assumere, all'interno della griglia articoli, la colonna dei
pulsanti (aggiungi alla wishlist, elimina articolo ecc...).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res4.bmp](./assets/media/image159.png)

Come per tutte le griglie responsive anche in questo caso la larghezza
di ogni colonna (compresa quella dei bottoni) si esprime definendo
quante delle 12 sezioni in cui risulta essere suddivisa ogni singola
riga, dovranno essere effettivamente occupate dalla colonna stessa.

**Posizionamento Colonna dei Bottoni**: consente di decidere se la
colonna dei bottoni dovrà essere posizionata a sinistra oppure a destra
delle informazioni relative allo specifico articolo

**Larghezza Colonna Articoli**: come precedentemente evidenziato il
Carrello è composto da una griglia principale, perfettamente responsiva
e strutturata su due diverse colonne, la "**Colonna Articoli**" e la
"**Colonna Totali**". Mediante questo parametro è quindi possibile
impostare la larghezza della Colonna Articoli definendo, nello
specifico, quante delle 12 sezioni in cui risulta essere suddivisa la
griglia principale dovranno essere occupate da questa stessa colonna

**Larghezza Colonna dei Totali**: consente di impostare la larghezza
della Colonna dei Totali definendo, anche in questo caso, quante delle
12 sezioni in cui risulta essere suddivisa la griglia principale
dovranno essere occupate da questa stessa colonna

**ATTENZIONE!** Indipendentemente dalla larghezza impostata per la
"Colonna Articoli" e per la "Colonna dei Totali," il comportamento
responsivo della griglia principale del carrello è tale per cui **in
corrispondenza di risoluzioni inferiori ai 992 px la griglia stessa si
linearizzerà disponendo le due colonne una sotto l'altra**

**Posizione dei campi di riepilogo dei Totali**: consente di definire
come dovranno essere posizionati, all'interno della Colonna dei Totali,
i campi relativi al "Sub Totale Carrello", "Iva", "Totale Carrello"
ecc... E' possibile selezionare una delle seguenti opzioni:

- Allineati a Destra

- Allineati a Sinistra

- Centrati

- Opposti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res5.bmp](./assets/media/image160.png)

Nell'esempio in figura il parametro "**Posizione dei campi di riepilogo
dei Totali**" è stato impostato sul valore "**Opposti**"

**Tipo di Accordion per i campi selezionabili**: consente di decidere se
i tre moduli per l'applicazione dei buoni sconto, per il calcolo delle
spese di spedizione e per il calcolo delle spese aggiuntive sui
pagamenti, presenti all'interno della Colonna dei Totali, dovranno
essere gestiti o meno mediante appositi accordion.

In caso affermativo è inoltre possibile decidere se tali accordion
dovranno essere, al caricamento della pagina, aperti oppure
chiusi[.]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_parametri_res7.bmp](./assets/media/image161.png)

Nell'esempio in figura il parametro "**Tipo di Accordion per i campi
selezionabili**" è stato impostato sul valore "**Accordion aperti al
caricamento della pagina**". In queste condizioni cliccando sul
corrispondente pulsante di chiusura/apertura sarà possibile
chiudere/aprire il relativo pannello contenente i dati dello specifico
modulo

**Posizionamento dei pulsanti delle Azioni**: consente di definire come
dovranno essere posizionati i pulsanti delle azioni presenti
immediatamente al di sotto della griglia articoli. E' possibile
selezionare una delle seguenti opzioni:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento dei pulsanti delle
azioni sarà esattamente quello indicato e non potrà essere modificato in
alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
pulsanti potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

La sezione "**Gestione Campi di Ordinamento**" consente, infine di
stabilire la modalità secondo cui dovranno essere ordinati gli articoli
presenti in carrello

![Videate\\ordinamento_carrello.bmp](./assets/media/image162.png)

**ATTENZIONE!** a differenza di altri componenti (es. "Catalogo
Ecommerce") non è possibile variare a front end l'ordinamento stabilito,
in fase di configurazione del componente, per gli articoli in carrello.

Per maggiori informazioni in merito alle diverse possibilità di
ordinamento si veda anche quanto indicato nel successivo capitolo di
questo manuale

Una volta settati i parametri di configurazione del Componente sarà poi
necessario, ovviamente, definirne i contenuti stabilendo innanzitutto il
numero di colonne in cui dovrà essere suddivisa ogni singola riga
articolo e, successivamente, andando ad inserire in queste stesse
colonne i componenti desiderati (Titolo, Prezzo, Immagine ecc...).

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

