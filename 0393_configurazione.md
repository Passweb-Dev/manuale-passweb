# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ecommerce_mini_wishlist_configurazione_res.bmp](./assets/media/image211.png){width="5.086111111111111in"
height="3.129166666666667in"}

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
presenti nella Wishlist corrente. In particolare, a default, verrà
visualizzato il Titolo (corrispondente alla Descrizione dell'Articolo)
di ogni singolo articolo. Il numero massimo di articoli visualizzati
dipenderà poi da quanto impostato nel successivo campo "Numero di Ultimi
Articoli Visualizzati".

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
presente in carrello sono quelli gestiti mediante i Segnaposto. Ogni
altro testo verrà replicato allo stesso modo per ogni singolo prodotto.

E' possibile utilizzare i seguenti segnaposto:

- **Codice**: consente di visualizzare in corrispondenza di ogni riga
  articolo presente all'interno del componente il codice del relativo
  prodotto

- **Titolo**: consente di visualizzare in corrispondenza di ogni riga
  articolo presente all'interno del componente il titolo del relativo
  prodotto

**ATTENZIONE!** il parametro in oggetto non è multilingua.

**Visualizza Immagine Articolo:** se selezionato consente di
visualizzare la miniatura dell'immagine associata all'articolo

**Visualizza Totale Articoli:** se selezionato consente di visualizzare
all'interno del Componente informazioni relative al numero o alla
quantità complessiva di articoli attualmente presenti nella Wishlist
corrente. Nello specifico è possibile selezionare una delle seguenti
opzioni:

- **Non visualizzare:** in questo caso non verrà visualizzata
  all'interno del componente nessuna informazione relativa al totale
  degli articoli attualmente presenti nella Wishlist corrente.

- **Visualizza Totale numero Articoli:** in questo caso verrà
  visualizzato il numero totale di articoli presenti nella Wishlist
  corrente indipendentemente da quella che è la quantità di questi
  stessi articoli. Supponendo dunque di avere inserito gli articoli
  ARTICOLO1 e ARTICOLO2 entrambi in quantità 3, all'interno del
  componente verrà visualizzata l'informazione "Hai 2 Articoli".

- **Visualizza Totale Numero di Quantità Articoli:** in questo caso
  verrà visualizzato il totale delle quantità di tutti gli articoli
  presenti nella Wishlist corrente. Facendo quindi riferimento ancora
  una volta all'esempio precedente, in queste condizioni all'interno del
  componente verrà visualizzata l'informazione "Hai 6 articoli"

**Visualizza Pulsante Rimuovi:** consente di visualizzare, se
selezionato, in corrispondenza di ogni articolo visualizzato all'interno
del componente un pulsante che consente di rimuovere l'articolo stesso
dalla Wishlist corrente.

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- L'elenco degli articoli presenti nella Wishlist

- Il pulsante di collegamento alla Wishlist

- Il Totale degli articoli presenti nella Wishlist

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

**Allineamento Verticale dei campi delle righe degli articoli della
Wishlist:** consente di impostare il tipo di allineamento verticale che
dovranno assumere le informazioni presenti all'interno di ogni singola
riga articoli.

E' possibile selezionare uno dei seguenti valori:

- Centrato

- Sopra

- Sotto

- Custom

**ATTENZIONE!** Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'allineamento verticale dei vari campi presenti
all'interno di ogni singola riga articolo potrà essere variato
liberamente agendo sulle corrette proprietà CSS mediante lo style editor
di Passweb e/o mediante i relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

