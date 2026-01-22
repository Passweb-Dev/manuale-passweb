# BUONI SCONTO



La sezione **" Buoni Sconto",** accessibile dalla voce di menu
principale "**Ordini**" consente all'amministratore del sito di generare
e gestire diversi "**Buoni Sconto**" da comunicare agli utenti del sito
in vari modi (attraverso pubblicità su riviste, su altri siti web
ecc...) e tali da garantire, una volta utilizzati, l'applicazione di
determinate scontistiche, che potranno poi essere applicate in maniera
incondizionata oppure soltanto al raggiungimento di determinate
condizioni.

Ogni Buono Sconto, dunque, definisce una particolare tipologia di sconto
per la quale possono essere generati uno o più codici distinti.
L'inserimento di questi stessi codici all'interno del relativo campo del
modulo d'ordine potrebbe consentire agli utenti del sito di accedere
alla relativa scontistica.

L'effettiva validità di un Buono Sconto può infatti dipendere dal
raggiungimento o meno di determinate condizioni (es. un limite mimino
d'ordine, l'acquisto di certe categorie di articoli in una determinata
quantità, il fatto di aver già utilizzato o meno quello specifico codice
sconto ecc...) configurabili in fase di creazione del Buono Sconto
stesso.

La maschera **"Lista dei Buoni Sconto"** mostra un elenco di tutti i
Buoni Sconto, ordinati per data di attivazione, attualmente codificati
all'interno del proprio sito.

![](./assets/media/image564.png)

In particolare all'interno di questo elenco sono evidenziati in:

- **Rosso**: i Buoni Sconto Scaduti (la cui data di fine gestione è cioè
  inferiore alla data odierna)

- **Grassetto**: i Buoni Sconto attivati e (se non scaduti)
  effettivamente utilizzabili all'interno del sito

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata in corrispondenza del campo "Nome", consente di
filtrare i dati in griglia sulla base dei valori presenti all'interno
della colonna stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![](./assets/media/image2.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![](./assets/media/image3.png) )

**ATTENZIONE!** Le colonne **"Quantità"** e **"Utilizzo"** mostrano, per
ciascuno dei Buoni Sconto in elenco, rispettivamente, il numero massimo
di volte in cui il Buono Sconto potrà essere utilizzato (0 = utilizzo
illimitato) ed il numero di volte in cui il Buono Sconto è già stato
utilizzato.

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Modifica Buono**
(![](./assets/media/image565.png) )**:** consente di modificare il Buono
Sconto attualmente selezionato.

**Attiva Buono**
(![](./assets/media/image566.png) )**:** consente di attivare il Buono
Sconto attualmente selezionato.

**Disattiva Buono**
(![](./assets/media/image567.png) )**:** consente di disattivare il Buono
Sconto attualmente selezionato.

**Copia Buono**
(![](./assets/media/image568.png) )**:** consente di copiare il Buono
Sconto attualmente selezionato. Le copie, ovviamente, saranno impostate
a default come "Non Attive".

**Elimina Buono**
(![](./assets/media/image569.png) )**:** consente di eliminare
definitivamente il Buono Sconto attualmente selezionato.

**Aggiungi Buono**
**(**![](./assets/media/image570.png) **):** consente di definire un nuovo
Buono Sconto. Cliccando su questo pulsante verrà infatti visualizzata la
relativa maschera di creazione

![](./assets/media/image571.png)

attraverso cui poter definire tutti i parametri necessari per la
codifica e l'utilizzo del nuovo Buono Sconto.

In particolare è necessario, per prima cosa, impostare uno specifico
valore per i seguenti campi:

**Nome:** nome identificativo del Buono Sconto in oggetto

**Valuta di riferimento:** permette di selezionare, tra quelle gestite
all'interno del sito, la specifica valuta in cui dovranno essere
considerati gli importi relativi al Buono Sconto in oggetto

**Quantità Totale:** permette di impostare il numero massimo,
**totale,** di volte in cui il Buono Sconto in esame potrà essere
utilizzato

**ATTENZIONE!** Una volta raggiunto tale numero il Buono Sconto non
potrà più essere utilizzato da nessun utente.

**NOTA BENE:.** impostando questo campo sul valore 0, il relativo buono
sconto potrà essere utilizzato un numero illimitato di volte.

Nel caso in cui un' ordine contenente un Buono Sconto venga annullato
(lato gestionale o lato sito web), il numero di volte in cui questo
stesso buono potrà essere utilizzato aumenterà di un unità.

La stessa cosa accadrà anche nel caso in cui un utente decida, in fase
di modifica di un ordine in sospeso, di togliere l'indicazione del Buono
Sconto inizialmente inserito.

**Quantità per ogni utente:** permette di impostare il numero massimo di
volte, **per singolo utente,** in cui il Buono Sconto in esame potrà
essere utilizzato.

**ATTENZIONE!** Una volta raggiunto, da un certo utente, questo numero,
lo stesso utente non avrà più la possibilità di utilizzare il Buono
Sconto.

**NOTA BENE:.** impostando questo campo sul valore 0, il relativo buono
sconto **potrebbe** essere utilizzato da ogni utente un numero
illimitato di volte. In questo caso occorre infatti considerare sempre
anche quanto impostato all'interno del precedente campo "Quantità
Totale".

**Il numero massimo totale di utilizzi per un Buono Sconto ha infatti la
priorità rispetto al numero di utilizzi per singolo utente**, per cui
una volta raggiunto il limite impostato all'interno del precedente campo
"Quantità Totale", il Buono Sconto non potrà più essere utilizzato da
nessun utente (indipendentemente dal numero di utilizzi per singolo
utente).

Nel caso in cui dunque si voglia gestire un Buono Sconto con un limite
di utilizzo per singolo utente, si consiglia di impostare il campo
"Quantità Totale" sul valore 0.

**ATTENZIONE!** Nel caso in cui si dovesse utilizzare il modulo di One
Step Checkout all'interno del sito uno stesso utente potrebbe effettuare
più ordini in modalità Guest (decidendo cioè di non creare uno specifico
account) e ad ogni ordine verrà creata una relativa anagrafica utente.

**In queste condizioni un eventuale codice sconto configurato per essere
utilizzato una volta sola da ogni utente potrebbe essere validato ed
applicato correttamente per ogni acquisto effettuato in modalità Guest**

**Gestione Limite:** consente di indicare se i successivi valori
impostati all'interno dei campi "Limite Minimo / Massimo del totale
merce" dovranno essere considerati o meno privi di iva

**Limite Minimo del totale merce:** valore del totale merce al di sotto
del quale il buono sconto in esame non avrà validità.

Nel caso in cui dunque il totale merce del documento dovesse essere
minore del valore indicato all'interno di questo campo, il
corrispondente buono sconto non verrà mai attivato.

**ATTENZIONE!** l' importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**Limite Massimo del totale merce:** valore del totale merce al di sopra
del quale il buono sconto in esame non avrà validità.

Nel caso in cui dunque il totale merce (ivato) del documento dovesse
essere maggiore o uguale al valore indicato all'interno di questo campo,
il corrispondente buono sconto non verrà mai attivato.

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**NOTA BENE:** nel caso in cui l'utente che effettua l'ordine abbia una
valuta diversa da quella specificata all'interno del campo "Valuta di
riferimento" gli importi dei limiti minimo e massimo specificati
all'interno dei relativi campi verranno convertiti nella valuta in uso
dal cliente.

**Periodo di Validità:** consente di impostare l'intervallo temporale
entro cui potrà essere utilizzato il Buono Sconto in esame.

**ATTENZIONE!** Buoni sconto scaduti (con "Data Fine" inferiore alla
data odierna) così come Buoni Sconto con "Data Inizio" superiore alla
data odierna, non possono essere utilizzati.

**Valido per:** disponibile solo nel caso in cui sia stato attivato il
modulo di gestione dell'App mobile

Consente di decidere se il Buono Sconto in esame dovrà essere valido
solamente all'interno del sito, solamente all'interno dell'App Mobile
oppure da entrambe le parti. E' possibile selezionare uno dei seguenti
valori:

- **Solo App:** selezionando questa opzione il Buono Sconto in esame
  sarà valido e verrà quindi applicato solo ed esclusivamente
  all'interno dell'App mobile collegata al sito.

> Per maggiori informazioni relativamente alla gestione delle App mobile
> si veda anche il relativo capitolo ("*App Mobile e Progressive Web
> App*") di questo manuale

- **Solo Web:** selezionando questa opzione il Buono Sconto in esame
  sarà valido e verrà quindi applicato solo ed esclusivamente
  all'interno del sito Web

- **Web e App:** selezionando questa opzione il Buono Sconto in esame
  sarà valido e verrà quindi applicato sia all'interno del sito web che
  all'interno dell' App mobile

**Attivo:** flag che consente di attivare/disattivare il Buono Sconto in
esame.

**Zone Associate:** consente di definire, selezionandole tra quelle
definite all'interno della sezione "**Ordini -- Zone**" del Wizard, le
eventuali Zone di Spedizione in corrispondenza delle quali il Buono
Sconto potrà effettivamente essere applicato

**ATTENZIONE!** nel caso in cui il campo in esame dovesse essere
lasciato vuoto il Buono Sconto sarà sempre valido indipendentemente da
quello che potrebbe essere l'indirizzo di spedizione associato
all'utente che naviga il sito

Per associare una nuova Zona al Buono Sconto che si sta realizzando sarà
sufficiente cliccare sul pulsante "**Aggiungi una zona**" ed inserirla
quindi all'interno del corrispondente riquadro

![](./assets/media/image572.png)

Il campo "Aggiungi una zona" è ad autocompletamento per cui iniziando a
digitare il nome della Zona che si intende associare al Buono verrà
aperto un elenco contenente tutte le possibili Zone di spedizione
definite all'interno della corrispondente sezione del Wizard (per
maggiori informazioni relativamente a come codificare una Zona di
spedizione utilizzabile poi a livello di Promozioni si veda quanto
indicata all'interno del capitolo "*Ordini -- Zone*" di questo manuale)

![](./assets/media/image573.png)

Nel momento in cui digitando il nome della Zona non dovesse essere
proposta nessuna opzione, significa che la Zona indicata non è tra
quelle codificate all'interno della relativa sezione del Wizard e che
quindi **non dovrà essere associata al Buono Sconto in esame**

**ATTENZIONE! associando al Buono Sconto una o più Zone di spedizione,
questo potrà poi essere applicato solo nel momento in cui l'indirizzo di
spedizione dell'utente dovesse effettivamente rientrare in una delle
Zone indicate**

In questo senso è bene quindi ricordare che l'indirizzo di spedizione in
base al quale decidere se applicare o meno un Buono Sconto con delle
zone associate, verrà valutato in maniera diversa a seconda del fatto
che l'utente stesso abbia o meno effettuato il login al sito e a seconda
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
> che verranno effettivamente considerate in fase di validazione del
> Buono Sconto saranno soltanto quelle in cui è stato gestito l'intero
> paese.
>
> In conseguenza di ciò, se il paese di appartenenza dell'utente non
> autenticato dovesse essere, ad esempio, l'Italia e tra le Zone
> associate alla Promo dovessero esserci soltanto Zone per cui è stata
> definita non solo la Nazione Italia ma anche specifiche Regioni,
> Provincie, Località o Cap, queste non verranno validate e, di
> conseguenza, il Buono non verrà applicato.
>
> Al contrario, se tra le Zone associate al Buono dovesse essercene una
> definita solo per la Nazione Italia allora questa verrebbe validata e
> il Buono Sconto sarebbe quindi applicato

- **Utenti autenticati**: nel momento in cui un utente dovesse
  effettuare l'autenticazione al sito, l'indirizzo di spedizione
  valutato per determinare se un Buono Sconto dovrà o meno essere
  applicato sarà, in prima istanza, il suo indirizzo primario

- **Utilizzo del componente "Selezione Indirizzo"**: l'indirizzo di
  spedizione valutato per determinare se Buono Sconto dovrà o meno
  essere applicato sarà quello eventualmente impostato mediante il
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
  affinchè i codici sconto possano effettivamente essere ritenuti validi
  -- **sezione Condizioni**

- la specifica tipologia di sconto che dovrà effettivamente essere
  applicata -- sezione **Azione**

- le promozioni che dovranno eventualmente essere escluse
  dall'applicazione di un eventuale buono sconto -- sezione **Promozioni
  non consentite**

- gli specifici Gruppi Utente che potranno effettivamente utilizzarle i
  codici sconto in esame -- sezione **Gruppi**

- i codici da associare al buono sconto in oggetto -- **sezione Codici
  Coupon**

