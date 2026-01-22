# TEMPLATE



All'interno della sezione "**Template**" è possibile gestire e
personalizzare, agendo direttamente a livello di codice HTML, il
contenuto dell'elemento "**Dettaglio della Gift Card**", elemento questo
che verrà poi utilizzato in due diversi punti:

- nelle mail inviate in automatico dall'applicazione in relazione alle
  diverse fasi di attivazione e gestione delle Gift Card (mediante
  l'utilizzo del relativo segnaposto).

> Per maggiori informazioni in merito si veda anche quanto indicato nel
> precedente capitolo di questo manuale

- sul front end del sito, all'interno della pagina "Gift Card", nel
  momento in cui l'utente utilizzerà il link di condivisione di una Gift
  Card virtuale per riscattare il relativo codice

> Per maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Varianti Sito Responsive -- Lista
> Componenti Ecommerce -- Componente Gift Card*" di questo manuale.

![](./assets/media/image315.png)

**ATTENZIONE!** La possibilità di costruire e gestire l'elemento
"Dettaglio della Gift Card" intervenendo direttamente sul codice HTML di
questo stesso elemento offre, indubbiamente, ampie possibilità di
personalizzazione, sia grafiche che a livello di veri e propri
contenuti. **D'altra parte dovendo intervenire direttamente sul codice
HTML questo tipo di personalizzazione richiede chiaramente specifiche
conoscenze tecniche.**

Volendo è possibile aprire l'editor in modalità full screen utilizzando
il tasto funzione **F11.** Una volta entrati in modalità full screen è
poi possibile ritornare alla visualizzazione standard utilizzando il
tasto **ESC**.

Il pulsante "**Preview**" consente di visualizzare un'anteprima del
Template che si sta realizzando, dove, ovviamente, al posto dei dati
reali relativi ad articoli e clienti, verranno visualizzati appositi
segnaposto.

In modalità Preview è possibile selezionare uno qualsiasi degli elementi
presenti all'interno del Template. Cliccandoci sopra si passerà
automaticamente alla versione "**Sorgente**" del template con
evidenziata la riga di codice relativa all'elemento selezionato

Relativamente ai contenuti che possono essere inseriti, in maniera
specifica, all'interno dell'elemento "Dettaglio della Gift Card" è
possibile sfruttare i vari segnaposto messi a disposizione da Passweb.

In questo senso una volta posizionato il cursore nel punto del template
in cui dovrà essere inserita la nuova informazione, sarà necessario
cliccare sul pulsante "**Seleziona un segnaposto ...**" in maniera tale
da visualizzare l'elenco di tutti i segnaposto disponibili

![](./assets/media/image316.png)

Selezionando il segnaposto desiderato tra quelli presenti in elenco,
Passweb provvederà poi ad inserire automaticamente nel template tutto il
codice necessario per gestire quello specifico tipo di informazione.

In questo senso è possibile selezionare differenti tipologie di
segnaposto:

- **Campi**: all'interno di questa sezione è possibile trovare i
  segnaposto relativi alle informazioni della specifica Gift Card (es.
  Codice della Gift Card, Saldo, Link di condivisione, Scadenza, Utente
  di fatturazione ...)

> **ATTENZIONE!** Nel momento in cui si dovessero gestire delle Gift
> Card di tipo Ho.Re.Ca. sarà di fondamentale importanza verificare di
> aver correttamente inserito all'interno del Template il segnaposto
> relativo al "Codice" della Gift Card. In caso contrario infatti il
> buono regalo potrebbe non essere poi utilizzabile all'interno del
> sito.

- **Opzioni**: all'interno di questa sezione è possibile trovare i
  segnaposto relativi ai vari Set di opzioni gestiti all'interno del
  sito. Le corrispondenti informazioni possono quindi tornare utili, per
  dettagliare ulteriormente le informazioni della Gift Card nel momento
  in cui le dovesse essere stato assegnato anche uno specifico set di
  opzioni (come nel caso ad esempio di Gift Card ad importo libero).

- **Condizioni:** i segnaposto presenti all'interno di questa sezione
  permettono di inserire delle istruzioni condizionali mediante le quali
  poter decidere di visualizzare o meno determinate informazioni solo
  sul front end del sito piuttosto che solo all'interno di specifiche
  mail

> Supponendo dunque di selezionare il segnaposto "**Se Mail di
> Attivazione**" nel template verranno inserite le seguenti istruzioni
>
> **\$if(mailActivation)\$**
>
> **\$endif\$**
>
> In questo modo tutto il codice HMTL e i vari segnaposto inseriti tra
> le due istruzioni sopra evidenziate verranno visualizzati solo ed
> esclusivamente all'interno della mail di **Attivazione Gift Card**.

