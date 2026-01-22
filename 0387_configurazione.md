# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web,

![](./assets/media/image188.png)

verrà aperta in automatico **la sua maschera di gestione e
configurazione**

![](./assets/media/image189.png)

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

**Periodo di Pubblicazione**: consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Numero di Wishlist da visualizzare per pagina**: consente di
specificare il numero di Wishlist che dovranno essere visualizzate
all'interno del relativo elenco, per ogni singola pagina.

**Numero di Pagine**: consente di impostare, selezionandolo dal relativo
menu a tendina, il numero di pagine che dovranno essere visualizzate nei
controlli di paginazione relativi all'elenco delle Wishlist. Ovviamente
oltre al numero indicato all'interno di questo campo nei controlli di
paginazione saranno sempre visibili anche la prima e l'ultima pagina
disponibili.

**Paginazione con Precedente e Successivo**: se selezionato, nei
controlli di paginazione relativi all'elenco delle Wishlist, verranno
visualizzati anche i pulsanti "Precedente" e "Successivo".

**Tipo di Paginazione:** consente di definire come dovrà comportarsi il
componente in oggetto ad ogni cambio di pagina. E' possibile selezionare
uno dei seguenti valori:

- **Senza caricamento della pagina:** in questo caso ad ogni cambio
  pagina verranno ricaricati solo ed esclusivamente i dati presenti
  all'interno del componente in oggetto

- **Con caricamento della pagina:** in questo caso ad ogni cambio pagina
  verrà ricaricata l'intera pagina web (con la possibilità da parte
  dell'utente, di dover utilizzare la scroll bar per visualizzare gli
  elementi presenti all'interno della nuova pagina)

**Visualizzazione Risultati:** se selezionato, consentirà di
visualizzare, relativamente all'elenco delle Wishlist, una stringa di
testo contenente il numero complessivo delle Wishlist presenti
all'interno del componente stesso.

**Aggiornamento Dati Articoli:** consente di impostare la modalità di
aggiornamento dei dati (quantità, note ...) relativamente agli articoli
attualmente presenti in Wishlist.

E' possibile selezionare uno dei seguenti valori:

- **Automatico:** in questo caso eventuali variazioni a quantità e/o
  note apportate ad uno degli articoli presenti in Wishlist verranno
  automaticamente salvate all'uscita del cursore dal relativo campo di
  input

- **Intera Wishlist:** in questo caso eventuali variazioni a quantità
  e/o note apportate ad uno o più articoli presenti in Wishlist dovranno
  essere confermate in blocco cliccando sul pulsante "**Aggiorna
  Wishlist**" presente nella parte bassa del componente.

![](./assets/media/image190.png)

> **ATTENZIONE!** Nelle condizioni indicate se l'utente **NON** dovesse
> cliccare sul pulsante evidenziato in figura, eventuali variazioni
> apportate ad una o più righe articolo non verranno salvate e
> potrebbero quindi andar perse se l'utente dovesse decidere di cambiare
> pagina

**Visualizzazione Paginazione Articoli:** consente di decidere se e dove
visualizzare (rispetto all'elenco degli articoli in Wishlist) i
collegamenti alle varie pagine che si attiveranno nel momento in cui il
numero complessivo di articoli presenti in Wishlist sia superiore a
quello impostato all'interno del successivo campo "**Numero Articoli da
Visualizzare**".

**Numero Articoli da Visualizzare:** consente di impostare il numero di
articoli che dovranno essere visualizzati per ogni singola pagina della
Wishlist. Nel caso in cui il numero complessivo di articoli presenti sia
superiore a quello impostato all'interno di questo campo, verrà attivato
un sistema di paginazione per consentire all'utente di visualizzare
tutti gli articoli presenti in lista.

**Numero di Pagine Articoli:** consente di impostare, selezionandolo dal
relativo menu a tendina, il numero di pagine che dovranno essere
visualizzate nei controlli di paginazione relativamente all'elenco di
articoli presenti in Wishlist. Ovviamente oltre al numero indicato
all'interno di questo campo, nei controlli di paginazione saranno sempre
visibili anche la prima e l'ultima pagina disponibili

**Paginazione Articoli con Precedente e Successivo:** se selezionato,
nei controlli di paginazione relativi all'elenco di articoli presenti in
Wishlist, verranno visualizzati anche i pulsanti "Precedente" e
"Successivo".

**Visualizzazione Risultati Articoli:** consente di visualizzare una
stringa di testo con il numero complessivo degli articoli attualmente
presenti in Wishlist

**Visualizzazione Ordinamento Articoli:** se selezionato, consentirà di
visualizzare, lato sito, una combo box contenente l'elenco degli
elementi sulla base dei quali poter effettuare l'ordinamento degli
articoli presenti all'interno del componente.

**ATTENZIONE!** i campi sulla base dei quali effettuare l'ordinamento
dovranno essere inseriti all'interno della relativa sezione **"Gestione
Campi di Ordinamento"**. Nel caso in cui all'interno di questa sezione
non dovesse essere inserito alcun campo la combo box di ordinamento non
verrà visualizzata e gli articoli in Wishlist continueranno ad essere
ordinati secondo l'ordine di inserimento (con eventuali articoli spesa
posti in fondo alla lista)

**Gestione Lista Regalo:** consente, se selezionato, di abilitare la
gestione delle Liste Regalo.

Selezionando questo parametro, nel form di salvataggio della Wishlist,
oltre al campo "**Nome**" comparirà infatti anche il campo
"**Tipologia**" dando quindi all'utente attualmente loggato la
possibilità di decidere, in fase di salvataggio della Wishlist, se
creare una "**Wishlist Personale**" oppure una "**Lista Regalo**".

![](./assets/media/image191.png)

Nel caso in cui, al contrario, il parametro in questione non dovesse
essere personalizzato, gli utenti del sito potranno creare solo ed
esclusivamente Wishlist di tipo "Personale"

**ATTENZIONE!** Per maggiori informazioni relativamente alle "Wishlist
Personali" e/o alle Wishlist di tipo "Lista Regalo" si vedano i
successivi capitoli di questo manuale. Per maggiori informazioni
relativamente alla gestione delle Liste Regalo si veda invece la sezione
"*Varianti Sito Responsive -- Lista Componenti Ecommerce -- Componente
Lista Regalo*" di questo manuale

**Colore dell'Animazione sui campi Obbligatori**: consente di
specificare il colore che verrà utilizzato da Passweb per evidenziare il
background dei campi obbligatori (nello specifico del campo in cui
l'utente dovrà indicare il nome con cui salvare la Wishlist corrente)
nel momento in cui al salvataggio del componente questi stessi campi non
dovessero essere stati valorizzati.

**Larghezza Colonna dei Bottoni:** consente di impostare la larghezza
che dovrà assumere, all'interno della griglia articoli, la colonna dei
pulsanti (aggiungi al carrello, rimuovi articolo).

![](./assets/media/image192.png)

Come per tutte le griglie responsive anche in questo caso la larghezza
di ogni colonna (compresa quella dei bottoni) si esprime definendo
quante delle 12 sezioni in cui risulta essere suddivisa ogni singola
riga, dovranno essere effettivamente occupate dalla colonna stessa.

**Posizionamento Colonna dei Bottoni**: consente di decidere se la
colonna dei bottoni dovrà essere posizionata a sinistra oppure a destra
delle informazioni relative allo specifico articolo

**Posizionamento dei pulsanti delle Azioni**: consente di definire come
dovranno essere posizionati i pulsanti delle azioni presenti
immediatamente al di sotto della Wishlist Corrente. E' possibile
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

Una volta settati i parametri di configurazione del Componente sarà poi
necessario, ovviamente, definirne i contenuti stabilendo innanzitutto il
numero di colonne in cui dovrà essere suddivisa ogni singola riga
articolo e, successivamente, andando ad inserire in queste stesse
colonne i componenti desiderati (Titolo, Prezzo, Immagine ecc...).

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

