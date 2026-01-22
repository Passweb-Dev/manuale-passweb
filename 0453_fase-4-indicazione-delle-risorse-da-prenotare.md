# FASE 4 -- INDICAZIONE DELLE RISORSE DA PRENOTARE



In questo step l'utente avrà la possibilità di indicare, partendo
direttamente dalla piantina associata al Centro di Produzione
selezionato durante la Fase 1, quali e quante risorse prenotare.

![](./assets/media/image382.png)

Le risorse (ombrelloni) visualizzate sulla piantina potranno assumere 3
diversi stati:

- **Disponibile** -- Risorsa di colore Verde Chiaro -- Identifica le
  risorse che possono essere effettivamente prenotate in relazione al
  periodo temporale indicato alla Fase 2

- **Selezionata** -- Risorsa di colore Verde Scuro -- Identifica le
  risorse che si è scelto di prenotare durante le sessione corrente

- **Non disponibile** -- Risorsa di colore Grigio -- Identifica le
  risorse che risultano già prenotate in relazione al periodo temporale
  indicato alla Fase 2

**ATTENZIONE!** I colori indentificativi dei diversi stati della risorsa
possono comunque essere modificati in fase di personalizzazione del
componente

Cliccando su uno degli ombrelloni disponibili per la prenotazione, verrà
aperto un pop up all'interno del quale saranno visualizzate **diverse
opzioni di selezione, una per ciascuno dei livelli della struttura cui
appartiene il prototipo associato alla risorsa selezionata (campo
"predefinito"), ad eccezione del livello utilizzato per gestire la
durata della prenotazione (livello questo appositamente marcato mediante
il parametro "Durata Servizio")**

![](./assets/media/image383.png)

In questa fase l'utente potrà quindi selezionare il numero di lettini e
/ o di sedie da aggiungere alla sua prenotazione.

**ATTENZIONE!** Come evidenziato nei precedenti capitoli di questo
manuale, il fatto di poter selezionare in questa fase una qualsiasi
combinazione di lettini + sedie o solamente le combinazioni
effettivamente ammesse, dipende dal fatto di aver esportato o meno sul
sito anche tutti gli articoli figli e da come è stata impostata, lato
Passweb, la relativa struttura ("Esplosa completamente" o "Vincolata al
precedente livello")

**ATTENZIONE! La struttura utilizzata per gestire questo tipo di
prenotazioni dovrà essere impostata, ovviamente, in modalità di
visualizzazione "Lineare"**

![](./assets/media/image384.png)

Nel momento in cui dovessero essere impostate altre tipologie di
visualizzazione, all'interno del pop up non verrà visualizzato nessun
tipo di controllo

Una volta indicato il numero di lettini e di sedie da aggiungere al
proprio ombrellone Passweb invierà al gestionale, in tempo reale, la
relativa combinazione di valori e, nel caso in cui tale combinazione:

- **corrisponda** ad uno degli articoli figli effettivamente gestiti, si
  otterrà come risposta il corrispondente prezzo che verrà quindi
  mostrato all'utente assieme al pulsante di "Conferma" necessario per
  validare la combinazione indicata e passare così allo step successivo

![](./assets/media/image385.png)

- **non corrisponda** a nessuno degli articoli effettivamente gestiti
  non verrà visualizzato nessun pulsante di "Conferma" né tanto meno di
  "Aggiungi altra risorsa", per cui con la combinazione indicata
  l'utente non avrà modo di passare allo step successivo. Inoltre verrà
  anche visualizzato un apposito messaggio per informarlo del fatto che
  la combinazione di risorse indicata non è gestita

![](./assets/media/image386.png)

**ATTENZIONE!** Nel caso in cui l'articolo utilizzato per gestire la
risorsa da prenotare dovesse essere un articolo semplice (es.
prenotazione della cabina) all'interno del pop verrà visualizzato
semplicemente il Titolo, la Descrizione e il Prezzo dell'articolo
stesso.

![](./assets/media/image387.png)

I pulsanti presenti nella parte bassa di questo pop up consentono
rispettivamente di:

- **Conferma**: permette di validare la combinazione di opzioni
  selezionata e di proseguire nel processo di prenotazione passando al
  successivo step di pagamento.

> Tale pulsante sarà visualizzato solo ed esclusivamente nel caso in cui
> la combinazione di opzioni indicata sia effettivamente prenotabile (e
> corrisponda quindi ad uno degli articoli presenti in Plan)

- **Chiudi**: permette di annullare la selezione corrente

- **Aggiungi altra risorsa**: permette di confermare la selezione
  corrente senza però passare immediatamente allo step successivo dando
  quindi all'utente la possibilità di aggiungere alla propria
  prenotazione ulteriori risorse (ombrelloni).

> Tale pulsante verrà visualizzato solo ed esclusivamente nel caso in
> cui il numero di risorse attualmente prenotate sia inferiore a quanto
> indicato per il parametro "**Numero massimo risorse prenotabili**"
> presente nella maschera di configurazione del componente "Prenotazione
> Risorse custom"

![](./assets/media/image388.png)

> Nel momento in cui il parametro evidenziato in figura dovesse essere
> impostato sul valore 1, in modo tale da consentire la prenotazione di
> una sola risorsa alla volta, il pulsante "Aggiungi altra risorsa",
> ovviamente, non verrà mai visualizzato.
>
> Inoltre anche questo pulsante, come quello di "Conferma" verrà
> visualizzato solo ed esclusivamente nel caso in cui la combinazione di
> opzioni indicata sia effettivamente prenotabile

Relativamente al prezzo delle risorse visualizzato in fase di
prenotazione è bene poi fare alcune considerazioni di fondamentale
importanza.

In particolare occorre considerare che:

- Il prezzo delle risorse selezionate non è memorizzato nel database di
  Passweb ma viene richiesto in tempo reale al gestionale in relazione
  alla specifica combinazione di elementi selezionati. Come
  precedentemente evidenziato, dunque, ogni combinazione di valori (es.
  lettini + sedie) consentirà di determinare uno specifico codice
  articolo che verrà inviato a Plan ottenendo come risposta il relativo
  prezzo del singolo articolo. Tale prezzo verrà poi moltiplicato per il
  numero di giorni della prenotazione e il totale verrà quindi
  visualizzato all'utente nel pop up di prenotazione.

> Supponendo dunque che la combinazione di valori indicati corrisponda
> ad un articolo che risulti avere in Plan prezzo di 10€ e che il
> periodo di prenotazione sia di 4 giorni, il prezzo visualizzato nel
> pop up di prenotazione sarà di 40€

- Nel caso in cui la combinazione di valori indicata in fase di
  prenotazione non corrisponda a nessuno degli articoli attualmente
  gestiti in Plan, il prezzo visualizzato sarà quello dell'articolo
  corrispondente alla prima combinazione utile gestita su Plan, dove con
  "prima combinazione utile" si intende quella dell'articolo relativo al
  numero di giorni immediatamente precedente a quello selezionato
  dall'utente in fase di prenotazione.

> Per comprendere meglio questo concetto, supponiamo di aver configurato
> il gestionale inserendo nell'insieme di valori relativo al livello
> della struttura utilizzato per gestire il periodo della prenotazione,
> i seguenti valori:
>
> 1,2,3,4,8
>
> Supponiamo anche, ovviamente, di aver codificato gli articoli figlio
> corrispondenti a questi valori e di aver assegnato, ad esempio
> all'articolo corrispondente a 4 giorni, il prezzo di 25€, e a quello
> corrispondente a 8 giorni il prezzo di 15€.
>
> In queste condizioni, nel momento in cui l'utente dovesse selezionare
> in fase di prenotazione sul sito:

- un periodo di 4 giorni il **prezzo unitario** considerato sarebbe di
  25€, determinato dal prezzo dell'articolo effettivamente presente
  all'interno del gestionale)

- un periodo di 5, 6 o 7 giorni, **il prezzo unitario** considerato
  sarebbe sempre di 25€, ossia il prezzo dell'articolo corrispondente al
  numero di giorni immediatamente precedente a quello selezionato
  dall'utente in fase di prenotazione

- un periodo di 8 giorni il **prezzo unitario** considerato sarebbe di
  15€, determinato dal prezzo dell'articolo effettivamente presente
  all'interno del gestionale)

<!-- -->

- Il prezzo delle risorse in Plan sarà gestito, tipicamente, mediante
  listini stagionali per cui per la stessa risorsa il prezzo
  visualizzato potrebbe essere differente anche in relazione alla data
  della prenotazione

- Nel caso in cui si siano prenotate più risorse all'interno della
  stessa sessione, il totale visualizzato nel pop up di prenotazione
  sarà sempre quello complessivo e terrà quindi conto di eventuali
  risorse già prenotate

