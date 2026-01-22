# ECOMMERCE HO.RE.CA. -- ARTICOLI COMPOSTI SEMPLICI



Come gli articoli Campionario all'interno di Mexal, anche un **Articolo
Composto** in un gestionale Ho.Re.Ca. (o Retail) altro non è se non un
articolo costituito da tanti singoli articoli componenti che possono
essere acquistati in blocco mediante l'inserimento in carrello del
Composto stesso.

Anche in queste condizioni (come già per i Campionari negli Ecommerce
Mexal) nel caso in cui l'articolo Composto sia stato impostato come
**NON CONFIGURABILE** e si sia quindi deciso di **non selezionare** il
parametro "**Abilita Configurazione**" presente nella maschera "**Dati
Articolo**" accessibile sul Wizard alla voce di menu "*Catalogo --
Gestione Articoli*"

![](./assets/media/image68.png)

il Componente **"Campionario E-commerce"** permetterà di inserire e di
visualizzare all'interno della Scheda Prodotto l'insieme di tutti gli
articoli del Composto attualmente selezionato.

![Videate\\articoli_composti1.bmp](./assets/media/image86.png)

> **NOTA BENE:** nel caso in cui il componente "Campionario E-Commerce"
> non venga inserito all'interno della scheda prodotto l'utente potrà
> comunque acquistare l'articolo Composto senza però poterne verificare
> i singoli componenti.

Tale componente è dunque indispensabile per poter gestire correttamente
all'interno del sito un Composto portando l'utente a conoscenza di tutti
gli articoli in esso contenuti.

In queste condizioni **l'utente non avrà alcuna possibilità di
variazione**, non potrà decidere cioè quali articoli del Composto
acquistare ed eventualmente in che quantità. La composizione sarà quindi
decisa unicamente dall'amministratore del sito in fase di codifica del
corrispondente articolo all'interno del gestionale.

Se l'esigenza dovesse invece essere quella di gestire un box
configurabile lasciando all'utente la possibilità di scegliere quali
articoli tra quelli del composto acquistare ed in che quantità, sarà
necessario ricorrere ad un Composto Configurabile (per maggiori
informazioni in merito si veda il successivo capitolo di questo manuale)

Affinchè l'articolo possa essere correttamente gestito all'interno del
sito, lato gestionale dovranno essere soddisfatte determinate
caratteristiche di configurazione.

Nello specifico sarà necessario:

- Esportare sul sito l'Articolo Composto e tutti i suoi Componenti
  selezionando per ciascuno di essi, nelle relative anagrafiche il campo
  "**Abilita Passweb**".

> **ATTENZIONE!** nel caso in cui alcuni articoli del Composto non
> vengano esportati, ci sarà, ovviamente, una differenza tra quanto
> impostato sul gestionale e quanto presente invece all'interno del sito
> E-commerce, relativamente all'elenco dei componenti e di conseguenza
> anche relativamente al prezzo del Composto stesso

- L'elenco degli articoli Componenti deve essere ben definito e
  realizzato quindi mediante l'opzione "**Articoli Prestabiliti**"

![Videate\\articoli_composti2.bmp](./assets/media/image87.png)

> **ATTENZIONE!** Non sono attualmente gestiti Articoli Composti in cui
> la lista dei Componenti è definita mediante le opzioni gestionali
> "Articoli presenti nella lista" o "Articoli presenti nelle categorie"

- I singoli componenti dovranno essere semplici articoli di magazzino.
  **Non dovranno quindi essere inseriti come componenti di un Composto
  Semplice, ad esempio, dei Prototipi**

- Sul sito verranno effettivamente considerati come singoli componenti
  del Composto, e quindi visualizzati all'interno del Campionario, i
  soli componenti, tra quelli presenti in elenco, che sono stati
  effettivamente esportati (campo "Abilita Passweb" selezionato) **e per
  i quali è stato selezionato anche il campo "Predefinito**"

![Videate\\articoli_composti3.bmp](./assets/media/image88.png)

> Nell'esempio riportato in figura il prodotto "acqua di Gio" è presente
> nella lista degli "Articoli Prestabiliti" del Composto "Cesto Regalo".
> Sul sito questo stesso articolo non verrà però considerato come
> elemento del "Cesto Regalo" in quanto non ha il parametro
> "Predefinito" selezionato.

Per quel che riguarda **la quantità con cui ogni singolo componente
viene inserito, lato sito, all'interno dell'Articolo Composto** è bene
sottolineare come questa **coincida esattamente con il valore impostato
per lo specifico componente all'interno del campo "Max" della relativa
tabella gestionale**

![Videate\\articoli_composti4.bmp](./assets/media/image89.png)

Con la configurazione evidenziata in figura dunque, sul sito all'interno
di ogni "Cesto Regalo" saranno presenti sempre 6 "Invictus" e l'utente
non avrà in alcun modo la possibilità di variare tale quantità.

Per quel che riguarda invece **la determinazione, lato sito, del prezzo
del Composto** è bene sottolineare come questo venga calcolato tenendo
conto di quelli che sono i componenti effettivamente gestiti sul sito e
di quanto impostato, lato gestionale, all'interno della sezione
"**Formula calcolo del prezzo di vendita**"

![](./assets/media/image90.png)

Nell'esempio riportato in figura dunque il prezzo del Composto sarà dato
dalla somma del Prezzo definito per l'articolo Composto in se più la
somma dei Prezzi dei 4 articoli componenti effettivamente gestiti sul
sito (ognuno moltiplicato per le relative quantità) il tutto
moltiplicato per 2.

Infine come già avveniva per gli articoli Campionario nei siti Ecommerce
collegati a Mexal, anche in questo caso ciascuno degli articoli presenti
nella lista dei componenti è, in generale, un link che porta
direttamente alla scheda del relativo prodotto rendendone quindi
possibile l'acquisto anche separatamente dal Composto cui esso
appartiene.

Nel caso in cui, al contrario, la necessità dovesse essere quella di
rendere acquistabili all'interno del sito i vari componenti solo ed
esclusivamente mediante l'acquisto di tutto il Composto (e non anche
come articoli singoli) sarà necessario ricorrere alla funzionalità
**"Visualizzazione Articoli in Negozio".**

Nel caso in cui, infatti, il corrispondente parametro presente
nell'anagrafica Passweb, non dovesse essere selezionato il relativo
articolo non solo non verrà più visualizzato all'interno di componenti
quali "Catalogo E-Commerce", "Offerte/Novità", "Articoli Abbinati"
ecc... ma, anche se presente all'interno della lista dei componenti,
verrà comunque disabilitato il link che riconduce alla sua scheda
prodotto rendendone di fatto impossibile l'acquisto separatamente dal
Composto di appartenenza.

Per maggiori informazioni in merito alla funzionalità "Visualizzazione
Articoli in Negozio" si veda anche la sezione *\"Configurazione
Gestionale -- Ho.Re.Ca. Parametri Configurazione Gestionale --
Funzionalità di gestione articoli -- Visualizzazione in Catalogo\"* di
questo manuale.

Per quel che riguarda le possibili richieste di disponibilità
(aggiornate all'ultima sincronizzazione o in tempo reale) per questo
particolare tipo di articoli, è bene sottolineare come ad ogni richiesta
**verrà restituita e visualizzata all'interno del sito la disponibilità
dell'intero Composto in relazione a quelle che sono non solo le
disponibilità dei singoli componenti ma anche in relazione a quella che
è la disponibilità del Composto in sé.**

Infine è bene sottolineare anche come:

- **All'interno dei componenti Carrello, Wishlist, Ordine e Reso**
  verranno sempre visualizzati, in relazione ai Composti Semplici, sia
  l'articolo Composto che l'elenco dei suoi componenti.

![](./assets/media/image91.png)

> Per l'articolo Composto sarà possibile modificare la quantità presente
> in carrello, eliminarlo dal carrello, inserire note di riga, date di
> scadenza ecc...
>
> **L'elenco dei componenti, al contrario è in sola visualizzazione**.
>
> Per ogni componente verranno visualizzate tutte le informazioni
> impostate in fase di configurazione del Carrello/Wishlist/Ordine/Reso
> ad eccezione del prezzo e del totale di riga (informazioni queste
> visualizzate a livello globale solo ed esclusivamente per l'intero
> articolo Composto).

- Il passaggio di un Composto Semplice tra i componenti Carrello,
  Wishlist, o Comparatore comporterà il passaggio anche di tutti suoi
  componenti. Nello specifico, **all'interno del Comparatore, verrà però
  visualizzato il solo articolo Composto** senza il dettaglio dell'
  elenco componenti.

