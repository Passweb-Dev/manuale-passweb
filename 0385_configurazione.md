# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_carrellino_configurazione_res.bmp](./assets/media/image180.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**ATTENZIONE!** Per maggiori informazioni relativamente al parametro
**Caricamento Javascript** si veda anche quanto indicato all'interno del
capitolo "*Configurazione Componenti -- Caratteristiche generali* --
*Staticizzazione e caricamento asincrono*" di questo manuale

**Visualizza Lista Ultimi Articoli:** se selezionato consente di
visualizzare all'interno del Componente una lista degli articoli
attualmente presenti in Carrello. In particolare verrà visualizzato il
Titolo (corrispondente alla Descrizione impostata sul gestionale) di
ogni singolo articolo. Il numero massimo di articoli visualizzati
dipenderà poi da quanto impostato nel campo "Numero di Ultimi Articoli
Visualizzati".

**Numero di Ultimi Articoli Visualizzati:** nel caso in cui sia stato
selezionato il parametro "Visualizza Lista Ultimi Articoli", consente di
specificare il numero massimo di articoli che verranno visualizzati
all'interno del Componente.

**Testo Articolo:** consente di impostare il testo che dovrà essere
visualizzato in corrispondenza di ogni riga articolo presente
all'interno del componente.

Il pulsante "**Aggiungi Segnaposto**" consente di inserire appositi
placeholder che verranno poi sostituiti a runtime con informazioni
relative allo specifico prodotto

**ATTENZIONE!** gli unici testi variabili a seconda del prodotto
presente in carrello sono quelli gestiti mediante i Segnaposto. **Ogni
altro testo verrà replicato allo stesso modo per ogni singolo
articolo.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrellino_testo_articoli.bmp](./assets/media/image181.png)

E' possibile utilizzare i seguenti segnaposto:

- **Codice**: consente di visualizzare in corrispondenza di ogni riga
  articolo il codice del relativo prodotto

- **Titolo**: consente di visualizzare in corrispondenza di ogni riga
  articolo il titolo del relativo prodotto

- **Prezzo Originale**: consente di visualizzare in corrispondenza di
  ogni riga articolo il prezzo originale del relativo prodotto

- **Sconto**: consente di visualizzare in corrispondenza di ogni riga
  articolo l'eventuale sconto applicato al relativo prodotto

- **Prezzo**: consente di visualizzare in corrispondenza di ogni riga
  articolo il prezzo del relativo prodotto al netto di eventuali sconti

**ATTENZIONE! il parametro in oggetto non è multilingua.** Quanto
inserito all'interno del campo "Testo Articolo" verrà quindi riproposto
allo stesso modo per ciascuna delle lingue attualmente gestite.

**Visualizza Immagine Articolo:** consente di visualizzare, in
corrispondenza di ogni riga articolo, l'immagine associata al relativo
prodotto

**Visualizza Importo Totale:** consente di visualizzare, se selezionato,
le seguenti informazioni:

- Totale Merce

- Iva

- Totale Merce ivato

In particolare, il dato effettivamente visualizzato all'interno del
componente, una volta attivato il parametro in questione, dipenderà
esattamente da quanto inserito alla pagina "**Testi Messaggi del Sito**"
per il componente "**Carrellino**" in relazione al testo "**Totale
Prezzo Articoli**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrellino_totali.bmp](./assets/media/image182.png)

In questo senso, all'interno del campo "**Testo**" evidenziato in
figura, è infatti possibile utilizzare i seguenti segnaposto

- **Totale**: consente di stampare il "**Totale Merce Ivato**" degli
  articoli attualmente presenti all'interno del componente

- **Subtotale**: consente di stampare il "**Totale Merce**" degli
  articoli attualmente presenti all'interno del componente

- **Iva**: consente di stampare l'**Iva** relativa agli articoli
  attualmente presenti all'interno del componente

Volendo poi il segnaposto "Iva" può essere utilizzato anche per definire
una condizione in base alla quale determinare cosa dovrà essere
effettivamente mostrato all'interno del componente.

Utilizzando, ad esempio, una condizione del tipo di quella qui di
seguito indicata

**\$if(vatprice)\$**

**Subtotale Merce: \$subtotalprice\$**

**IVA: \$vatprice\$**

**\$endif\$**

**Totale: \$totalprice\$**

il risultato che otterremo sarà quello di stampare all'interno del
carrellino le tre voci distinte (Totale merce non ivato, Iva e Totale
merce ivato) solo nel caso in cui il valore dell'Iva dovesse essere
effettivamente diverso da zero (condizione **\$if(vatprice)\$**
soddisfatta), e quindi solo nel caso in cui i prezzi visualizzati
dovessero essere iva esclusa (cosa che, tipicamente, dovrebbe avvenire
se ad effettuare l'ordine dovesse essere un utente di tipo Azienda)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrellino_totali_non_ivati.bmp](./assets/media/image183.png)

Se invece i prezzi visualizzati all'interno del sito dovessero essere
iva inclusa (perché ad esempio ad effettuare l'ordine è un utente
Privato) la condizione **\$if(vatprice)\$** non verrà soddisfatta e
quindi l'unico valore ad essere stampato all'interno del carrellino sarà
direttamente il Totale merce ivato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\carrellino_totali_ivati.bmp](./assets/media/image184.png)

**Visualizza Totale Articoli :** se selezionato consente di visualizzare
all'interno del Componente informazioni relative al numero o alla
quantità complessiva di articoli attualmente presenti in Carrello. Nello
specifico è possibile selezionare una delle seguenti opzioni:

- **Non visualizzare:** in questo caso non verrà visualizzata
  all'interno del componente nessuna informazione relativa al totale
  degli articoli attualmente presenti in carrello.

<!-- -->

- **Visualizza Totale numero Articoli:** in questo caso verrà
  visualizzato il numero totale di articoli presenti in carrello
  indipendentemente da quella che è la quantità di questi stessi
  articoli. Supponendo dunque di avere in carrello gli articoli
  ARTICOLO1 e ARTICOLO2 entrambi in quantità 3, all'interno del
  componente Carrellino verrà visualizzata l'informazione "Hai 2
  Articoli".

- **Visualizza Totale Numero di Quantità Articoli:** in questo caso
  verrà visualizzato il totale delle quantità di tutti gli articoli
  presenti in Carrello. Facendo quindi riferimento ancora una volta
  all'esempio precedente, in queste condizioni all'interno del
  componente Carrellino verrà visualizzata l'informazione "Hai 6
  articoli"

**Visualizza pulsante Rimuovi**: consente di visualizzare, se
selezionato, in corrispondenza di ogni articolo visualizzato all'interno
del componente un pulsante che consente di rimuovere l'articolo stesso
dal carrello.

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- L'elenco degli articoli presenti in carrello

- Il pulsante di collegamento alla pagina Carrello

- Il prezzo totale

- Il Totale degli articoli presenti in carrello

E' possibile selezionare uno dei seguenti valori:

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
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

**Allineamento Verticale dei campi delle righe degli articoli del
carrello:** consente di impostare il tipo di allineamento verticale che
dovranno assumere le informazioni presenti all'interno di ogni singola
riga articoli.

E' possibile selezionare uno dei seguenti valori:

- Centrato

- Sopra

- Sotto

- Custom

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'allineamento verticale dei vari campi presenti
all'interno di ogni singola riga articoli potrà essere variato
liberamente agendo sulle corrette proprietà CSS mediante lo style editor
di Passweb e/o mediante i relativi strumenti di editing avanzato.

**Mostra Promozioni in Carrello:** consente, se selezionato, di
visualizzare la "Descrizione" associata ad eventuali "Promozioni in
Carrello" e/o a sistemi di "Raccolta Punti" attivi sul sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\desc_promozioni_carrellino_2.bmp](./assets/media/image185.png)

Grazie a questo parametro è quindi possibile visualizzare, anche
all'interno del Carrellino, un testo mediante il quale informare
l'utente che al verificarsi di determinate condizioni (da dettagliare
all'interno del testo stesso) potrà beneficiare di specifiche promozioni
(es. "Mancano xxx€ per ottenere uno sconto di 20€ su tutto il carrello")

**ATTENZIONE!** il testo visualizzato all'interno del carrellino sarà
esattamente quello inserito in corrispondenza del campo
"**Descrizione**" presente nella maschera di configurazione della
specifica "Promozione in Carrello" e/o della specifica "Regola di
Raccolta Punti" attiva sul sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\desc_promozioni_carrellino.bmp](./assets/media/image186.png)

Per maggiori informazioni in merito a come poter associare una
Descrizione alle Promozioni in Carrello e/o alle Regole di Raccolta
punti si rimandata a quanto indicato nei relativi capitoli di questo
manuale ("*Ordini -- Promozioni -- Promozioni Carrello*" e "*Utenti --
Punti -- Creazione di un sistema di raccolta punti -- Regole di Raccolta
Punti*")

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
visualizzare, per la stessa Promozione e/o per la stessa Regola di
Raccolta Punti, due Descrizioni differenti, una all'interno della pagina
Carrello e una all'interno del componente Carrellino, sarà necessario,
per prima cosa, impostare i relativi messaggi in maniera tale da poterli
identificare univocamente, ad esempio mediante l'assegnazione di
apposite classi CSS. Successivamente sarà poi possibile nasconderli o
visualizzarli secondo le specifiche esigenze del caso, attraverso
l'applicazione di semplici regole CSS

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

