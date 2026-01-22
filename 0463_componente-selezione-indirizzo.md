# COMPONENTE SELEZIONE INDIRIZZO



Il Componente "**Selezione Indirizzo**" può essere utilizzato in una
qualsiasi pagina del sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_selezione_indirizzo.bmp](./assets/media/image413.png)

e consente di inserire all'interno della pagina stessa una combo box
contenente un piccolo form che l'utente potrà utilizzare per indicare
(specificando Nazione, Provincia, Città e Cap, oppure selezionando, se
autenticato, uno dei suoi indirizzi di spedizione) una ben precisa zona
di spedizione merce, zona questa in relazione alla quale verranno poi
valutati gli importi di eventuali Tasse Addizionali e/o Metodi di
Spedizione attualmente visualizzati all'interno del sito.

![Videate\\selezione_indirizzo.bmp](./assets/media/image414.png)

In particolare, per quel che riguarda la zona di spedizione in relazione
alla quale verranno valutati gli importi delle spese di trasporto e/o
delle tasse addizionali occorre ricordare che tali importi potrebbero
variare, innanzitutto, a seconda del fatto che l'utente che sta
navigando il sito abbia o meno effettuato l'autenticazione.

Nello specifico

- Per utenti **non autenticati** la zona di spedizione merce verrà
  determinata, inizialmente, utilizzando soltanto la Nazione ricavata
  sulla base delle impostazioni di lingua / paese del browser
  dell'utente o, qualora questo non fosse possibile, sulla base del suo
  indirizzo IP.

> **ATTENZIONE!** La corrispondenza Indirizzo IP -- Paese di provenienza
> è determinata automaticamente da Passweb sulla base di un servizio
> gratuito di tipo "light" la cui precisione potrebbe non essere quindi
> garantita al 100% soprattutto in virtù di eventuali riassegnazioni
> degli indirizzi IP da parte dei vari provider.

- Se l'utente che sta navigando il sito **ha effettuato il login**, la
  zona di spedizione merce verrà invece determinata, inizialmente,
  utilizzando il suo indirizzo primario vale a dire l'indirizzo di
  fatturazione associato alla sua anagrafica utente.

In ogni caso, indipendentemente dal fatto di aver effettuato o meno
l'autenticazione, l'utente potrebbe avere la necessità di inserire una
zona di spedizione merce diversa da quella inizialmente considerata, in
maniera tale da poter poi valutare l'ammontare delle tasse addizionali
e/o delle spese di trasporto anche in relazione ad essa.

In questo senso potrebbe quindi agire in tre modi diversi:

- Indicando uno specifico indirizzo di spedizione mediante l'apposito
  modulo di preventivo delle spese di trasporto presente in carrello

- Indicando uno specifico indirizzo di spedizione direttamente in fase
  di checkout

- Utilizzando il componente "Selezione Indirizzi"

**ATTENZIONE!** L'indirizzo indicato all'interno del componente
"Selezione Indirizzi" verrà utilizzato per valutare gli importi di
eventuali spese di spedizione e/o tasse addizionali in uso al sito **ma
non verrà impostato come effettivo indirizzo di spedizione merce da
utilizzare poi in fase di checkout.**

In conseguenza di ciò l'utente dovrà sempre indicare esplicitamente, in
fase di checkout, l'indirizzo di spedizione che intende effettivamente
utilizzare per l'ordine in essere.

