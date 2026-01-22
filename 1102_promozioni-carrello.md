# PROMOZIONI CARRELLO



All'interno della sezione "**Promozioni Carrello**", accessibile dalla
voce di menu "**Ordini -- Promozioni**", è possibile definire e gestire,
direttamente dal Wizard, una serie di Promozioni che potranno essere
applicate sulla base degli articoli presenti in carrello al verificarsi
o meno di determinate condizioni.

In particolare l'applicazione o meno di una Promozione potrà dipendere:

- dal totale merce raggiunto

- dal giorno in cui viene effettuato l'ordine

- dalla presenza o meno di specifici articoli in carrello

- dalla presenza in carrello di una certa quantità e/o di un certo
  numero di articoli

- dal particolare utente che sta effettuando l'acquisto

Ogni promozione, inoltre, potrà essere gestita:

- con l'applicazione di una determinata tipologia di sconto (e il
  conseguente inserimento in ordine di un articolo spesa di importo
  negativo)

- con l'inserimento in carrello di uno o più articoli in omaggio (o ai
  quali applicare un certo sconto)

- con l'assegnazione di uno specifico valore per le spese di spedizione.

**ATTENZIONE!** eventuali sconti dovuti all'applicazione di queste
Promozioni verranno applicati, lato gestionale, mediante l'utilizzo di
appositi articoli Spesa, inseriti in ordine con quantità negativa.

La maschera **"Lista delle Promozioni"** presente all'interno di questa
sezione del Wizard, mostra un elenco di tutte le Promozioni attualmente
codificate all'interno del proprio sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_promozioni.bmp](./assets/media/image478.png){width="5.5256944444444445in"
height="3.4611111111111112in"}

In particolare all'interno di questo elenco sono evidenziate in:

- **Rosso**: le Promozioni Scadute (la cui data di fine gestione è cioè
  inferiore alla data odierna)

- **Grassetto**: le Promozioni attive e (se non scadute) effettivamente
  utilizzabili all'interno del sito

Per ogni Promozione presente in elenco è indicato: lo Stato (Attiva/Non
Attiva), il suo livello di priorità, la Data di Inizio gestione, la Data
di Fine gestione

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata in corrispondenza del campo "Nome", consente di
filtrare i dati in griglia sulla base dei valori presenti all'interno
della colonna stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image2.png){width="7.777777777777778e-2in"
height="9.722222222222222e-2in"} ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image3.png){width="0.12361111111111112in"
height="0.14930555555555555in"} )

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Modifica Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_promozione.bmp](./assets/media/image479.png){width="0.83125in"
height="0.2013888888888889in"} )**:** consente di modificare la
Promozione attualmente selezionato.

**Attiva Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_promozione.bmp](./assets/media/image480.png){width="0.7340277777777777in"
height="0.2013888888888889in"} )**:** consente di attivare la Promozione
attualmente selezionata.

**Disattiva Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_disattiva_promozione.bmp](./assets/media/image481.png){width="0.8375in"
height="0.2013888888888889in"} )**:** consente di disattivare la
Promozione attualmente selezionata.

**Elimina Promozione**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_promozione.bmp](./assets/media/image482.png){width="0.7729166666666667in"
height="0.18819444444444444in"} )**:** consente di eliminare
definitivamente la Promozione attualmente selezionata.

**Aggiungi Promozione**
**(**![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_promozione.bmp](./assets/media/image483.png){width="0.8444444444444444in"
height="0.1951388888888889in"} **):** consente di definire una nuova
Promozione. Cliccando su questo pulsante verrà infatti visualizzata la
relativa maschera di creazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_promozione.bmp](./assets/media/image484.png){width="6.253472222222222in"
height="3.50625in"}

attraverso cui poter definire tutti i parametri necessari per la
codifica e l'utilizzo della nuova Promozione.

In particolare è necessario impostare uno specifico valore per i
seguenti campi:

**Nome:** nome identificativo della Promozione in oggetto

**Valuta di riferimento:** permette di selezionare, tra quelle gestite
all'interno del sito, la specifica valuta in cui dovranno essere
considerati gli importi relativi alla Promozione in oggetto

**Gestione Limite:** consente di indicare se i successivi valori
impostati all'interno dei campi "Limite Minimo / Massimo del totale
merce" dovranno essere considerati o meno privi di iva

**Limite Minimo del totale merce:** valore del totale merce al di sotto
del quale la Promozione in oggetto non ha validità.

Nel caso in cui dunque il totale merce del documento dovesse essere
minore del valore indicato all'interno di questo campo, la
corrispondente Promozione non verrà mai applicata.

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**Limite Massimo del totale merce:** valore del totale merce al di sopra
del quale la Promozione in oggetto non ha validità.

Nel caso in cui dunque il totale merce del documento dovesse essere
maggiore o uguale al valore indicato all'interno di questo campo, la
corrispondente Promozione non verrà mai applicata.

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**NOTA BENE:** nel caso in cui l'utente che effettua l'ordine abbia una
valuta diversa da quella specificata all'interno del campo "Valuta di
riferimento" gli importi dei limiti minimo e massimo specificati
all'interno dei relativi campi verranno convertiti nella valuta in uso
dal cliente.

**Periodo di Validità:** consente di impostare l'intervallo temporale
entro cui poter usufruire della Promozione in oggetto.

**ATTENZIONE!** Promozioni scadute (con "Data Fine" inferiore alla data
odierna) così come Promozioni con "Data Inizio" superiore alla data
odierna, ovviamente, non verranno mai applicate.

**Priorità:** intero a base 1. Consente di specificare l'ordine in cui
dovranno essere valutate le Promozioni. L'ordinamento è ascendente e
Promozioni prive di priorità verranno valutate per ultime.

Supponendo di aver codificato tre distinte Promozioni A, B e C
rispettivamente con Priorità 2, 1 e 3 nel momento in cui l'utente
effettuerà l'ordine sul sito, verranno valutate per prima cosa le
condizioni di applicabilità della Promozione B (che ha priorità 1), poi
quelle della Promozione A (che ha priorità 2) ed infine quelle della
Promozione C (che ha priorità 3).

**ATTENZIONE!** **Le Promozioni possono essere cumulabili tra loro**. In
virtù di questo fatto, nel momento in cui, per l'esempio sopra
considerato, dovessero essere soddisfatte le condizioni di applicabilità
di tutte e tre le Promozioni A, B e C l'utente potrà usufruire, per lo
stesso ordine, di ognuna di esse.

**Interrompi esecuzione regole:** se selezionato consente di
interrompere, a partire dalla Promozione in oggetto, la valutazione
delle condizioni di applicabilità di eventuali altre Promozioni con
grado di priorità superiore.

**Tale parametro consente quindi di definire il livello di
sovrapposizione e di cumulabilità delle diverse Promozioni in elenco.**

Per comprendere meglio la funzione e l'importanza di questo parametro,
supponiamo di aver codificato tre distinte Promozioni A, B e C
rispettivamente con Priorità 2, 1 e 3 e supponiamo inoltre di aver
selezionato il parametro in oggetto per la Promozione A.

In queste condizioni nel momento in cui l'utente effettuerà l'ordine sul
sito verranno valutate per prima cosa le condizioni di applicabilità
della Promozione B (che ha priorità 1) e, se soddisfatte, verrà
applicata la relativa promozione. Considerando poi che per la Promozione
B non è stato selezionato il parametro "Interrompi esecuzione regole"
verranno valutate anche le condizioni di applicabilità della Promozione
A (che ha priorità 2) e, se soddisfatte, verrà applicata anche questa
promozione. Per la promozione A è stato inoltre selezionato il parametro
"Interrompi esecuzione regole" il che farà terminare, esattamente in
questo punto, il processo di valutazione delle condizioni di
applicabilità di altre promozioni con priorità maggiore a 2. In
conseguenza di ciò le condizioni di applicabilità della Promozione C
(che ha priorità 3) non verranno neppure valutate per cui la Promozione
C non potrà mai essere cumulabile alla Promozione A e/o alla Promozione
B.

Considerando infine che per la Promozione C non è stato selezionato il
parametro "Interrompi esecuzione regole" tale promozione potrebbe invece
essere cumulabile con eventuali ulteriori promozioni di priorità
maggiore o uguale a 3.

**Valido per:** disponibile solo nel caso in cui sia stato attivato il
modulo di gestione dell'App mobile

Consente di decidere se la promozione in esame dovrà essere valida
solamente all'interno del sito, solamente all'interno dell'App Mobile
oppure da entrambe le parti. E' possibile selezionare uno dei seguenti
valori:

- **Solo App:** selezionando questa opzione la promozione in esame sarà
  valida e verrà quindi applicata solo ed esclusivamente all'interno
  dell'App mobile collegata al sito.

> Per maggiori informazioni relativamente alla gestione delle App mobile
> si veda anche il relativo capitolo ("*App Mobile e Progressive Web
> App*") di questo manuale

- **Solo Web:** selezionando questa opzione la promozione in esame sarà
  valida e verrà quindi applicata solo ed esclusivamente all'interno del
  sito Web

- **Web e App:** selezionando questa opzione la promozione in esame sarà
  valida e verrà quindi applicata sia all'interno del sito web che
  all'interno dell' App mobile

**Attivo:** flag che consente di attivare/disattivare la Promozione in
oggetto.

**Descrizione:** consente di specificare, in tutte le lingue attualmente
gestite all'interno del sito, un testo descrittivo della promozione in
oggetto, testo questo che potrà poi essere mostrato all'interno dei
componenti "**Carrello Custom**" e/o "**Carrellino**" al verificarsi
delle seguenti condizioni:

- Il carrello non è vuoto

- La promozione in oggetto non è ancora stata applicata perché il Totale
  Merce non rientra ancora nel range di applicabilità della promozione
  stessa (campi "Limite Minimo e Massimo del totale merce")

- La promozione in oggetto non è ancora stata applicata perché non sono
  ancora state soddisfatte le condizioni di applicabilità della
  promozione stessa.

> Per maggiori informazioni in merito alle condizioni di applicabilità
> di una specifica promozione si veda anche il successivo capitolo di
> questo manuale "**Promozione -- Condizioni**"

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
visualizzare, per la stessa Promozione, due Descrizioni differenti, una
all'interno della pagina Carrello e una all'interno del componente
Carrellino, sarà necessario, per prima cosa, impostare i relativi
messaggi in maniera tale da poterli identificare univocamente, ad
esempio mediante l'assegnazione di apposite classi CSS. Successivamente
sarà poi possibile nasconderli o visualizzarli secondo le specifiche
esigenze del caso, attraverso l'applicazione di semplici regole CSS

Grazie a questo parametro è quindi possibile definire un testo mediante
il quale poter informare l'utente del sito che, al verificarsi di
specifiche condizioni (da dettagliare all'interno del testo stesso)
potrà beneficiare di determinate promozioni.

In questo senso, cliccando sul pulsante "**Aggiungi Segnaposto**", sarà
possibile inserire all'interno del testo, anche i seguenti placeholder:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_segnaposto_descrizione.bmp](./assets/media/image485.png){width="4.941666666666666in"
height="2.9743055555555555in"}

- **Limite minimo**: consente di inserire all'interno del testo il
  segnaposto \$min_limit\$ che verrà poi sostituito, sul front end del
  sito, dall'importo in valuta relativo al limite minimo del totale
  merce che sarà necessario raggiungere per poter attivare la promozione
  in esame (campo Limite Minimo del totale merce)

- **Limite massimo**: consente di inserire all'interno del testo il
  segnaposto \$max_limit\$ che verrà poi sostituito, sul front end del
  sito, dall'importo in valuta relativo al limite massimo del totale
  merce oltre il quale non sarà più possibile attivare la promozione in
  esame (campo Limite Massimo del totale merce)

- **Differenza Limite Minimo**: consente di inserire all'interno del
  testo il segnaposto \$min_limit_diff\$ che verrà poi sostituito, sul
  front end del sito, con il valore della differenza tra il totale
  carrello dell' utente (ivato o non ivato a seconda di quanto impostato
  in corrispondenza del parametro "Gestione Limite") e il limite minimo
  di applicabilità della promozione.

> **ATTENZIONE!** nel caso in cui la "Differenza Limite Minimo" dovesse
> essere negativa (perché il totale in carrello supera il limite minimo
> impostato per la promozione) il valore di questo segnaposto non verrà
> visualizzato
>
> Nel momento in cui l'esigenza dovesse essere quella di nascondere, nel
> caso in cui la differenza in oggetto dovesse essere negativa, non solo
> il valore ma anche un eventuale testo utilizzato come label per il
> valore stesso (es. 'Per applicare la promo mancano ancora ...'), il
> tutto andrà racchiuso all'interno del segnaposto "**Se differenza
> Limite Minimo**"

- **Se differenza Limite Minimo:** consente di inserire all'interno del
  testo il seguente segnaposto condizionale:

> \$if(min_limit_diff)\$
>
> -- Testo da visualizzare nel caso in cui la "Differenza limite minino"
> dovesse avere un valore positivo --
>
> \$else\$
>
> -- Testo da visualizzare nel caso in cui la "Differenza limite minino"
> dovesse avere un valore negativo --
>
> \$endif\$
>
> In queste condizioni dunque quanto inserito tra le istruzioni
> \$if(min_limit_diff)\$ e \$else\$ verrà visualizzato solo nel caso in
> cui la differenza tra il totale in carrello e il limite minimo
> impostato per la promozione dovesse essere un valore positivo
> (condizioni di limite minimo non soddisfatta).
>
> Quanto inserito invece tra le istruzioni \$else\$ e \$endif\$ verrà
> visualizzato solo nel caso in cui la differenza tra il totale in
> carrello e il limite minimo impostato per la promozione dovesse essere
> un valore negativo (condizioni di limite minimo soddisfatta)

- **Sconto**: consente di inserire all'interno del testo il segnaposto
  \$discount\$ che verrà poi sostituito, sul front end del sito, dal
  valore dello sconto (in percentuale o in valuta) di cui l'utente potrà
  beneficiare al verificarsi delle condizioni di applicabilità della
  promozione in esame (promozione che dovrà ovviamente prevedere
  l'applicazione di un determinato sconto)

**ATTENZIONE!** il campo "Descrizione" verrà visualizzato anche per i
siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca ma solo ed
esclusivamente in corrispondenza di promozioni di tipo "Offerta MxN
Semplice" e "Offerta MxN Misti". In queste condizioni, inoltre, l'unico
segnaposto utilizzabile sarà quello relativo allo sconto associato alla
promozione.

**Descrizione promozione attivato:** consente di specificare, in tutte
le lingue attualmente gestite all'interno del sito, un testo descrittivo
che potrà essere visualizzato all'interno dei componente "**Carrello
Custom**" e/o "**Carrellino**" quando la promozione in esame verrà
effettivamente applicata

**ATTENZIONE!** Nel momento in cui l'esigenza dovesse essere quella di
visualizzare, per la stessa Promozione, due testi differenti, il primo
all'interno della pagina Carrello e il secondo all'interno del
componente Carrellino, sarà necessario, per prima cosa, impostare i
relativi messaggi in maniera tale da poterli identificare univocamente,
ad esempio mediante l'assegnazione di apposite classi CSS.
Successivamente sarà poi possibile nasconderli o visualizzarli secondo
le specifiche esigenze del caso, attraverso l'applicazione di semplici
regole CSS

Grazie a questo parametro è quindi possibile definire un testo mediante
il quale notificare all'utente che la promozione in esame è stata
effettivamente applicata, cosa questa che potrebbe rivelarsi
particolarmente utile nel caso, ad esempio, delle promo che azzerano le
spese di spedizione e che, come tali, non comportano l'inserimento
diretto in carrello di specifici articoli di tipo spesa

Anche in questo caso è possibile utilizzare gli stessi segnaposto
disponibili per il campo "Descrizione" precedentemente esaminato

**ATTENZIONE!** il campo "Descrizione promozione attivato" verrà
visualizzato anche per i siti Ecommerce collegati ad uno dei gestionali
Ho.Re.Ca ma solo ed esclusivamente in corrispondenza di promozioni di
tipo "Offerta MxN Semplice" e "Offerta MxN Misti". In queste condizioni,
inoltre, l'unico segnaposto utilizzabile sarà quello relativo allo
sconto associato alla promozione.

**Zone Associate:** consente di definire, selezionandole tra quelle
definite all'interno della sezione "**Ordini -- Zone**" del Wizard, le
eventuali Zone di Spedizione in corrispondenza delle quali la Promo
potrà effettivamente essere applicata

**ATTENZIONE!** nel caso in cui il campo in esame dovesse essere
lasciato vuoto la Promozione sarà sempre valida indipendentemente da
quello che potrebbe essere l'indirizzo di spedizione associato
all'utente che naviga il sito

Per associare una nuova Zona alla Promozione che si sta realizzando sarà
sufficiente cliccare sul pulsante "**Aggiungi una zona**" ed inserirla
quindi all'interno del corrispondente riquadro

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_zone_spedizione.bmp](./assets/media/image486.png){width="4.941666666666666in"
height="2.798611111111111in"}

Il campo "Aggiungi una zona" è ad autocompletamento per cui iniziando a
digitare il nome della Zona che si intende associare alla Promozione,
verrà aperto un elenco contenente tutte le possibili Zone di spedizione
definite all'interno della corrispondente sezione del Wizard (per
maggiori informazioni relativamente a come codificare una Zona di
spedizione utilizzabile poi a livello di Promozioni si veda quanto
indicata all'interno del capitolo "*Ordini -- Zone*" di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\promozioni_zone_spedizione_2.bmp](./assets/media/image487.png){width="4.941666666666666in"
height="2.798611111111111in"}

Nel momento in cui digitando il nome della Zona non dovesse essere
proposta nessuna opzione, significa che la Zona indicata non è tra
quelle codificate all'interno della relativa sezione del Wizard e che
quindi **non dovrà essere associata alla Promozione in esame**

**ATTENZIONE! associando alla Promozione una o più Zone di spedizione,
questa potrà poi essere applicata solo nel momento in cui l'indirizzo di
spedizione dell'utente dovesse effettivamente rientrare in una delle
Zone indicate**

In questo senso è bene quindi ricordare che l'indirizzo di spedizione in
base al quale decidere se applicare o meno una promozione con delle zone
associate, verrà valutato in maniera diversa a seconda del fatto che
l'utente stesso abbia o meno effettuato il login al sito e a seconda
anche di quello che sta effettivamente facendo sul sito.

In particolare:

- **Utenti non autenticati**: per questa tipologia di utenti l'indirizzo
  di spedizione verrà valutato prendendo in considerazione solamente la
  Nazione di appartenenza dell'utente, Nazione questa che verrà
  determinata, in prima istanza, sulla base della lingua impostata sul
  browser utilizzato per navigare il sito. Nel caso in cui tale lingua
  dovesse essere priva dell'indicazione dello specifico paese, la
  provenienza del visitatore verrà determinata sulla base del suo
  indirizzo IP.

> **ATTENZIONE! La corrispondenza Indirizzo IP -- Paese di provenienza è
> determinata automaticamente da Passweb sulla base di un servizio
> gratuito di tipo "light" la cui precisione potrebbe non essere quindi
> garantita al 100% soprattutto in virtù di eventuali riassegnazioni
> degli indirizzi IP da parte dei vari provider.**
>
> Se poi il paese ricavato dalla impostazioni del browser o
> dall'indirizzo IP non dovesse essere tra quelli attualmente gestiti
> all'interno del sito, la Nazione di appartenenza dell'utente verrà
> automaticamente impostata sul Paese di Default (per maggiori
> informazioni in merito all'associazione degli utenti non autenticati
> ad una determinata Nazione si veda anche quanto indicato all'interno
> della sezione "*Configurazione -- Parametri Paese Lingua e Valuta --
> Gestione Paese*" di questo manuale)
>
> Una cosa di fondamentale importanza da tenere in considerazione è che
> non avendo a disposizione, in queste condizioni, un indirizzo completo
> e potendo far riferimento soltanto alla Nazione, le Zone di spedizione
> che verranno effettivamente considerate in fase di validazione della
> Promo saranno soltanto quelle in cui è stato gestito l'intero paese.
>
> In conseguenza di ciò, se il paese di appartenenza dell'utente non
> autenticato dovesse essere, ad esempio, l'Italia e tra le Zone
> associate alla Promo dovessero esserci soltanto Zone per cui è stata
> definita non solo la Nazione Italia ma anche specifiche Regioni,
> Provincie, Località o Cap, queste non verranno validate e, di
> conseguenza, la Promo non verrà applicata.
>
> Al contrario, se tra le Zone associate alla Promo dovesse essercene
> una definita solo per la Nazione Italia allora questa verrebbe
> validata e la Promo sarebbe quindi applicata

- **Utenti autenticati**: nel momento in cui un utente dovesse
  effettuare l'autenticazione al sito, l'indirizzo di spedizione
  valutato per determinare se una Promozione dovrà o meno essere
  applicata sarà, in prima istanza, il suo indirizzo primario

- **Utilizzo del componente "Selezione Indirizzo"**: l'indirizzo di
  spedizione valutato per determinare se una Promozione dovrà o meno
  essere applicata sarà quello eventualmente impostato mediante il
  componente in esame (per maggiori informazioni relativamente
  all'utilizzo del componente "Selezione Indirizzi" si rimanda a quanto
  indicato all'interno del capitolo "*Componenti Ecommerce -- Componente
  Selezione Indirizzo*" di questo manuale)

- **Stima Spedizioni in Carrello**: in fase di preventivo delle spese di
  spedizione in carrello verrà considerato l'indirizzo di spedizione
  impostato all'interno del corrispondente modulo

- **Checkout**: in fase di checkout verrà valutato, ovviamente,
  l'indirizzo di spedizione effettivamente impostato dall'utente
  all'interno del relativo step

Oltre a questi parametri di configurazione generale, sarà poi necessario
specificare anche, come indicato nei successivi capitoli di questo
manuale:

- una o più condizioni che dovranno essere obbligatoriamente soddisfatte
  affinché la Promozione in oggetto possa effettivamente essere ritenuta
  valida -- **sezione Condizioni**

- la logica di funzionamento della promozione -- sezione **Azione**

- gli specifici Gruppi Utente che potranno effettivamente beneficiare
  della promozione in esame -- sezione **Gruppi**

