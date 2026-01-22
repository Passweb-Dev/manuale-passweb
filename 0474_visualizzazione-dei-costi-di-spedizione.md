# VISUALIZZAZIONE DEI COSTI DI SPEDIZIONE



Nel momento in cui l'esigenza dovesse essere quella di utilizzare il
componente "Spedizione" per visualizzare all'interno di Componenti
Ecommerce di primo livello quali la Scheda Prodotto, il Catalogo
Ecommerce, gli Abbinati ..., il costo di spedizione dei relativi
articoli, sarà necessario:

- Selezionare il parametro "**Abilita stima costi/consegna**" presente
  nella maschera di configurazione del metodo di trasporto di cui si
  vogliono visualizzare i costi di spedizione

> **ATTENZIONE!** Il componente "Spedizione" prenderà in considerazione
> solo ed esclusivamente i metodi di trasporto per i quali è stato
> flaggato il parametro "**Abilita stima costi/consegna**"
>
> **ATTENZIONE!** Per poter visualizzare il parametro "**Abilita stima
> costi/consegna**" è necessario attivare, su Passstore, il modulo
> "Stima Trasporto"

- Verificare di aver inserito all'interno del campo "**Template
  Spedizione**", presente nella maschera di configurazione del
  componente "Spedizione", il segnaposto "**Prezzo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spedizione_segnaposto_prezzo.bmp](./assets/media/image451.png)

Supponendo dunque di aver soddisfatto le due condizioni sopra indicate e
di aver inserito il componente "Spedizione" all'interno, ad esempio,
della scheda prodotto, potremo ottenere un risultato del tipo di quello
evidenziato in figura.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spedizione_segnaposto_prezzo_1.bmp](./assets/media/image452.png)

L'importo della spedizione effettivamente visualizzato all'interno del
componente dipenderà poi, ovviamente, da come è stato configurato il
corrispondente metodo di trasporto oltre che dall'indirizzo di
spedizione della merce, indirizzo questo che verrà determinato in
maniera diversa, ad esempio, a seconda del fatto che l'utente che sta
navigando il sito abbia o meno effettuato il login.

In particolare:

- Per utenti **non autenticati** la zona di spedizione della merce (da
  cui dipenderà poi l'effettivo importo dei costi di spedizione) verrà
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
  zona di spedizione della merce (da cui dipenderà poi l'effettivo
  importo dei costi di spedizione) verrà invece determinata,
  inizialmente, utilizzando il suo indirizzo primario vale a dire
  l'indirizzo di fatturazione associato alla sua anagrafica utente. In
  questo caso verrà quindi valutata non solo la Nazione ma, ad esempio,
  anche la Provincia e il CAP potendo quindi definire la zona di
  spedizione, e i relativi costi, in maniera sicuramente più precisa.

In ogni caso, indipendentemente dal fatto di aver effettuato o meno
l'autenticazione, l'utente potrebbe avere anche la necessità di inserire
un indirizzo di spedizione merce diverso da quello inizialmente
considerato, in maniera tale da poter poi valutare l'ammontare dei costi
anche per quella specifica zona di spedizione.

In questo senso dunque, è opportuno inserire e gestire correttamente
all'interno del sito anche il componete "**Selezione Indirizzo**".

Grazie a questo componente infatti l'utente avrà a disposizione un
piccolo form mediante il quale poter indicare (specificando Nazione,
Provincia, Città e Cap, oppure selezionando, se autenticato, uno dei
suoi indirizzi di spedizione) una ben precisa zona in relazione alla
quale valutare i costi di trasporto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_indirizzo.bmp](./assets/media/image453.png)

Per maggiori informazioni relativamente al componente "Selezione
Indirizzo" si veda anche quanto indicato nel relativo capitolo di questo
manuale ("*Varianti Sito Responsive -- Lista Componenti Ecommerce --
Componente Selezione Indirizzo*")

Oltre al componete "Selezione Indirizzo" l'utente potrebbe poi impostare
uno specifico indirizzo di spedizione lavorando anche in carrello
(mediante l'apposito modulo di preventivo delle spese di spedizione) o
direttamente in checkout. Anche in questo caso verranno automaticamente
ricalcolati, sulla base di queste nuove impostazioni, tutti gli importi
visualizzati all'interno del componente "Spedizione" e, allo stesso
modo, verrà ovviamente aggiornato anche l'indirizzo visualizzato
all'interno del componente "Selezione Indirizzo".

In definitiva dunque, potrebbe verificarsi una situazione del tipo di
quella qui di seguito indicata:

- **L'utente effettua il primo accesso al sito**.

> In questa fase, non avendo ancora effettuato l'autenticazione, la zona
> di spedizione utilizzata per determinare i relativi costi di trasporto
> verrà valutata, come detto, facendo riferimento unicamente alla
> Nazione ricavata dalle impostazioni di lingua/paese del browser
> dell'utente o, in alternativa, sulla base del suo indirizzo IP.
>
> Supponendo dunque che il browser dell'utente sia impostato sulla
> lingua Italiana, verranno mostrate le spese di spedizione relative,
> genericamente, alla nazione Italia.

- **L'utente effettua l'autenticazione**.

> La zona di spedizione utilizzata per determinare i relativi costi di
> trasporto verrà aggiornata facendo riferimento ora all'indirizzo
> primario dell'utente.
>
> Supponendo dunque che tale indirizzo sia "Via Flaminia 123, 47922
> Rimini (RN)" in questa fase verranno calcolati e visualizzati i costi
> di trasporto relativi, non più a tutta l'Italia, ma quelli relativi in
> maniera più specifica all'Emilia Romagna o, se presenti, quelli ancora
> più specifici relativi alla provincia di Rimini e al CAP 47922

- **L'utente utilizza il componente "Selezione Indirizzo" per impostare
  una Zona di Spedizione diversa da quella attualmente considerata
  dall'applicativo.**

> La zona di spedizione utilizzata per determinare i relativi costi di
> trasporto verrà aggiornata sulla base dell'indirizzo inserito
> dall'utente.
>
> Supponendo dunque che l'indirizzo inserito dall'utente sia "Via Pietro
> Gori 40, 50019 Sesto Fiorentino FI" verranno calcolati e visualizzati
> ora i costi di trasporto relativi alla Toscana o , se presenti, quelli
> ancora più specifici relativi alla provincia di Firenze, alla città di
> Sesto Fiorentino e al CAP 50019

- **L'utente si porta nella pagina Carrello o nella pagina Checkout e
  seleziona un indirizzo di spedizione diverso da quello di
  fatturazione**.

> La zona di spedizione utilizzata per determinare i relativi costi di
> trasporto verrà nuovamente aggiornata facendo riferimento ora allo
> specifico indirizzo di spedizione indicato dall'utente in questa fase.
>
> Supponendo che tale indirizzo sia "Via Giuseppe Garibaldi 13, 10122
> Torino (TO)" verranno quindi calcolati e visualizzati i costi di
> trasporto relativi al Piemonte o, se presenti, quelli ancora più
> specifici relativi alla provincia di Torino e al CAP 10122
>
> Allo stesso tempo verrà aggiornato anche la zona di spedizione
> eventualmente visualizzata all'interno del componente "Selezione
> Indirizzo"

- **L'utente effettua il logout**

> Si ritorna nella condizione iniziale in cui la zona di spedizione
> utilizzata per determinare i relativi costi di trasporto verrà
> valutata, facendo riferimento unicamente alla Nazione ricavata dalle
> impostazioni di lingua/paese del browser dell'utente o, in
> alternativa, sulla base del suo indirizzo IP.
>
> In questa fase torneranno quindi ad essere visualizzate le spese di
> spedizione relative genericamente alla nazione Italia

Sulla base di quanto detto dunque potrebbe rivelarsi particolarmente
utile inserire, ad esempio nella scheda prodotto, un testo per avvisare
gli utenti che i costi di spedizione attualmente visualizzati sono
riferiti ad una determinata zona e che, modificando questo dato, gli
stessi costi potrebbero ovviamente subire delle variazioni.

Per questo è possibile utilizzare il segnaposto "**Zona Spedizione**"
presente all'interno dei componenti "**Paragrafo**" e "**HTML**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_zona_spedizione.bmp](./assets/media/image454.png)

segnaposto questo che verrà poi sostituito in fase di generazione della
pagina web con i dati relativi alla zona in relazione alla quale sono
attualmente calcolati i costi di spedizione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spedizione_segnaposto_prezzo_2.bmp](./assets/media/image455.png)

**ATTENZIONE!** per evitare di rileggere ad ogni caricamento della
pagina web tutte le spedizioni attualmente gestite e velocizzare così la
stima dei costi di spedizione, viene utilizzata un'apposita variabile di
sessione. In conseguenza di ciò, nel momento in cui dovessero essere
effettuate delle modifiche alla configurazione dei metodi di trasporto
attualmente in uso, prima di poter verificare la correttezza dei nuovi
dati sarà necessario eliminare i cookie del browser.

Un' altra cosa di fondamentale importanza da tenere sempre in
considerazione è che i costi di trasporto visualizzati all'interno del
componente "Spedizione" **verranno valutati facendo riferimento sempre e
soltanto alla singola unità di prodotto**. In conseguenza di ciò nel
momento in cui su di un determinato metodo di trasporto dovesse essere
impostato, ad esempio, uno specifico "Limite minimo/massimo del totale
merce" questo verrà valutato facendo riferimento al prezzo unitario del
relativo articolo.

Allo stesso modo se le spese di spedizione dovessero essere determinato
sulla base di una certa percentuale del Totale Merce / Imponibile
l'importo effettivamente visualizzato all'interno del Componente
Spedizione verrà determinato utilizzando come base di calcolo il prezzo
del singolo articolo.

In ogni caso, indipendentemente dal fatto di considerare spese di
trasporto fisse o in percentuale, l'importo effettivamente visualizzato
all'interno del componente "Spedizione" sarà o meno comprensivo di IVA a
seconda, ovviamente, di come è stato impostato il parametro "**Tipo di
Costo**" presente nella maschera di configurazione del trasporto stesso,
e di quelle che sono le impostazioni settate all'interno della pagina
"**Configurazione Catalogo**" del Wizard (menu "*Catalogo --
Configurazione Parametri -- Catalogo Mexal / Ho.Re.Ca.*").

Nello specifico gli importi visualizzati saranno:

- **Ivati** se sono verificate le seguenti condizioni:

  - Campo "**Prezzo**" alla pagina "Configurazione Catalogo" del Wizard
    impostato sul valore "**Con Iva**" oppure sul valore "**Iva
    Cliente**" e l'utente che sta navigando il sito non è ancora
    autenticato oppure è autenticato come cliente Privato

  - Per il metodo di spedizione in esame viene utilizzata **un'aliquota
    iva fissa e non ripartita**

- **Non Ivati** se sono verificate le seguenti condizioni:

  - Campo "**Prezzo**" alla pagina "Configurazione Catalogo" del Wizard
    impostato sul valore "**Senza Iva**" oppure sul valore "**Iva
    Cliente**" e l'utente che sta navigando il sito è autenticato come
    cliente Azienda

  - Per il metodo di spedizione in esame viene utilizzata **un'aliquota
    iva fissa e non ripartita**

**ATTENZIONE!** Nel momento in cui per la spedizione in esame non
dovesse essere utilizzata un'aliquota Iva fissa, gli importi
visualizzati all'interno del componente "Spedizione" coincideranno
sempre e comunque con l'esatto importo della spedizione,
indipendentemente da chi sta effettuando l'ordine e da come è stato
impostato il campo "Prezzo" alla pagina "Configurazione Catalogo" del
Wizard

**ATTENZIONE!** Al fine di rendere più esplicito per gli utenti il fatto
che i costi di trasporto attualmente visualizzati siano o meno
comprensivi di IVA è possibile attivare il parametro "Mostra indicazione
IVA" presente alla pagina "Configurazione Catalogo" del Wizard. Per
maggiori informazioni in merito a questo parametro si veda quanto
indicato nel relativo capitolo di questo manuale ("*Catalogo --
Configurazione Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca.*")

