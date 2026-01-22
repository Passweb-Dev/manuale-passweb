# COMPONENTI E-COMMERCE -- PUNTI



Il Componente **"Punti"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_res.bmp](./assets/media/image533.png)

può essere inserito all'interno dei seguenti componenti ecommerce di
primo livello:

- Scheda Prodotto

- Offerte/Novità

- Popolarità Prodotto

- Catalogo

- Risultati Ricerca

- Selezione Regalo

- Abbinati

- Campionario E-Commerce

- Comparatore

- Lista Regalo

e permette di visualizzare, in relazione al sistema di raccolta punti
attualmente attivo sul sito, il numero di punti che un utente andrebbe a
guadagnare nel momento in cui dovesse acquistare il relativo articolo
**in quantità unitaria**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_fe.bmp](./assets/media/image257.png)

In generale, in merito all'effettiva visibilità del componente in
questione è bene ricordare sempre che:

- **il componente "Punti" visualizza sempre e soltanto il numero di
  punti che si andrebbero ad accumulare nel momento in cui l'utente
  dovesse decidere di acquistare quel determinato articolo in quantità =
  1**

- il numero di condizioni da verificare per poter applicare una
  determinata regola definita per il sistema di raccolta punti
  attualmente attivo sul sito, influisce anche sull' effettiva
  visibilità del componente "Punti"

In merito a quest'ultimo punto dunque, supponendo di avere a che fare
con una regola costituita dalle tre condizioni di seguito indicate:

- Articoli appartenenti alla categoria "Uomo"

- Quantità in carrello \>= 2

- Totale merce non ivato \>= 100€

e di avere impostato l'applicazione della regola al verificarsi di
almeno 2 delle suddette condizioni, il componente "Punti" inserito ad
esempio all'interno del "Catalogo Ecommerce" (dove viene considerato
sempre in quantità unitaria) verrà visualizzato solo in corrispondenza
di quegli articoli che appartengono effettivamente alla categoria "Uomo"
e il cui prezzo unitario non ivato risulti essere effettivamente
maggiore o uguale a 100€.

Ovviamente poi il numero di punti effettivamente accumulati in seguito
all'acquisto di un determinato prodotto dipenderà, oltre che dalle
regole di raccolta punti definite per il sistema in questione, anche
dalla quantità effettiva con cui quello stesso articolo viene inserito
in ordine.

Supponendo quindi di aver configurato una regola di raccolta punti con
un "Limite minimo del totale merce" impostato sul valore (ivato) di 200€
e di avere un articolo con prezzo unitario (anch'esso ivato) di 178.56€,
in corrispondenza di questo stesso articolo, come evidenziato in figura,
il componente "Punti" non verrà mai visualizzato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_fe2.bmp](./assets/media/image534.png)

coerentemente con il fatto che il suo prezzo unitario non supera il
"Limite minimo del totale merce" impostato per la regola di raccolta
punti.

Nel momento in cui l'utente dovesse però decidere di acquistare quello
stesso articolo, ad esempio, in quantità uguale a 2 (per un totale merce
complessivo di 357.12€) portandosi poi in carrello o direttamente in
checkout, nei totali del documento, verrà visualizzato correttamente il
numero di punti stabiliti dalla relativa regola di raccolta che si
andranno ad accumulare confermando l'acquisto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_fe3.bmp](./assets/media/image535.png)

Per maggiori informazioni in merito a come configurare le regole di
raccolta punti si veda anche quanto indicato nel capitolo "*Utenti --
Punti -- Creazione di un sistema di raccolta punti -- Regole di raccolta
punti*" di questo manuale

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_configurazione_res.bmp](./assets/media/image536.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" è possibile settare i
principali parametri di configurazione del componente stesso.

In particolare, per la tipologia di Componente in questione, è possibile
impostare un valore per i seguenti parametri:

- **Nome:** consente di impostare un nome per il Componente che si sta
  editando.

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Label**: consente di impostare una label personalizzata per il
  componente in esame

- **Abilita link alla pagina dell'articolo**: se selezionato consente di
  attivare sul componente un link di collegamento alla relativa pagina
  prodotto. Per ovvie ragioni questo parametro non sarà presente nel
  caso in cui il componente in oggetto sia inserito all'interno della
  scheda prodotto

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

