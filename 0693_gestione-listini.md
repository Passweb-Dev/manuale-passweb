# GESTIONE LISTINI



La pagina **"Gestione Listini"** consente di associare ai vari paesi
gestiti (ed in cui dunque il sito e-commerce dovrà funzionare in maniera
corretta) uno specifico Listino.

All'interno di questa pagina verrà quindi visualizzata la maschera,
**"Lista dei Listini"**, qui di seguito riportata

![](./assets/media/image168.png)

in cui verranno elencati tutti i listini codificati all'interno del
gestionale. Per ciascuno dei listini presenti in elenco è indicato sia
il Nome che il relativo codice gestionale

**NOTA BENE:** l'elenco dei listini presenti all'interno della maschera
sopra evidenziata viene prelevato direttamente dalla relativa Tabella
del gestionale

**ATTENZIONE!** Per i siti Ecommerce collegati ad uno dei gestionali
Ho.Re.Ca. sono gestiti anche i Listini Parziali

Per maggiori informazioni relativamente alla gestione dei listini
all'interno del gestionale si rimanda all'apposito manuale di prodotto

**NOTA BENE:** nel caso in cui vengano apportate delle variazioni alla
Tabella Listini è poi necessario una sincronizzazione manuale o
attendere la prossima sincronizzazione automatica in modo tale da
riportare tali variazioni anche all'interno del sito web.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![](./assets/media/image169.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![](./assets/media/image170.png) )

Per associare ai vari paesi gestiti all'interno del sito uno specifico
listino, sarà quindi sufficiente selezionare il listino desiderato e
cliccare sul pulsante **"Modifica listino"** (
![](./assets/media/image171.png) ) presente nella barra degli strumenti.

In questo modo verrà infatti aperta la maschera **"Gestione del
Listino"** qui di seguito riportata

![](./assets/media/image172.png)

attraverso la quale poter associare il listino selezionato ad uno o a
più paesi tra quelli effettivamente gestiti.

**NOTA BENE:** nella List Box di sinistra verranno indicati
esclusivamente i paesi effettivamente gestiti, secondo quando impostato
dunque nella relativa maschera "Gestione dei Paesi", e ai quali non è
ancora stato associato uno specifico listino.

Per poter realizzare questa associazione sarà sufficiente selezionare il
paese o i paesi desiderati dall'elenco di sinistra, inserirli nel
riquadro di destra cliccando sulla piccola freccia rivolta verso destra
e cliccare infine sul pulsante "Salva" presente nella parte bassa della
maschera.

Allo stesso modo, per annullare questa associazione sarà sufficiente
selezionare il paese o i paesi desiderati dall'elenco di destra
reinserirli nel riquadro di sinistra cliccando sulla piccola freccia
rivolta verso sinistra e ancora una volta cliccare sul pulsante "Salva"
presente nella parte bassa della maschera.

Nel caso in cui il paese desiderato non si trovi tra quelli presenti in
elenco occorrerà per prima cosa attivare tale paese inserendolo nella
lista dei paesi gestiti secondo quanto indicato nel paragrafo
**"Gestione Paese"** di questo manuale.

**NOTA BENE:** uno stesso listino può essere associato a più paesi
diversi.

**NOTA BENE:** allo stesso paese non possono essere associati due
listini differenti

Il pulsante **"Listino Default"** (
![](./assets/media/image173.png) ) presente nella barra degli strumenti
consente di impostare il listino attualmente selezionato come Listino di
default da utilizzare ad esempio nel caso in cui il paese di
appartenenza dell'utente attualmente collegato al sito non sia tra
quelli gestiti, o semplicemente nel caso in cui non sia stata effettuata
una specifica associazione "paese -- listino" per il paese in questione.

**NOTA BENE:** il listino di Default verrà evidenziato in grassetto

**ATTENZIONE!** Per maggiori informazioni relativamente alle modalità di
determinazione del paese di provenienza dell'utente che naviga il sito
si veda anche quanto indicato all'interno dei capitoli e "*Sito-
Gestione Lingue del sito*" e *"Configurazione Gestionale -- Parametri
Paese Lingua e Valuta -- Gestione Listini*" di questo manuale.

Nel caso in cui per il paese in questione sia stata effettuata una
specifica associazione "Paese -- Listino" secondo quanto precedentemente
indicato, per gli articoli presenti in negozio verranno visualizzati i
prezzi del listino che soddisfa tale associazione.

Nel caso in cui invece tale associazione non sia presente per gli
articoli in negozio verranno visualizzati i prezzi del listino di
Default.

**NOTA BENE:** per gli utenti non ancora autenticati, la visualizzazione
del prezzo con o senza Iva nel catalogo dipende da quanto impostato in
Passweb nel menu "Catalogo - Catalogo Mexal" alla voce "Prezzo". Per
maggiori informazioni si veda l'apposita sezione di questo manuale.

Se poi il nuovo utente che si registra per effettuare un acquisto
risulta essere un'Azienda, alla pagina Ordine verrà effettuato lo
scorporo dell'IVA mostrando così solo a questo punto i prezzi dei vari
articoli in carrello al netto dell'IVA. Nel caso in cui invece il nuovo
utente che si registra per effettuare un acquisto risulta essere un
privato, i prezzi dei vari articoli saranno considerati comprensivi di
IVA e non verrà effettuato alla pagina Ordine nessuno scorporo.

**NOTA BENE:** nel caso di siti Ecommerce collegati a Mexal, la valuta
di visualizzazione dei listini può dipendere dal paese di appartenenza
dell'utente attualmente connesso al sito secondo quanto impostato nella
relativa maschera "Gestione delle Valute. Per maggiori informazioni si
veda l'apposita sezione di questo manuale.

In ogni caso è sempre possibile inserire all'interno del sito il
componente e-commerce "Cambio Valuta" per permettere all'utente di
visualizzare i prezzi degli articoli nelle varie valute gestite.

**Considerata la forte integrazione con il gestionale, Passweb assegna
sempre una priorità più elevata alle specifiche impostazioni del
gestionale.**

Nel caso in cui dunque l'utente attualmente connesso al sito sia già un
cliente codificato all'interno del gestionale che ha, nelle sue
condizioni commerciali uno specifico listino, dopo che l'utente ha
effettuato il login, e si è quindi fatto riconoscere dall'applicazione,
**i prezzi** degli articoli verranno visualizzati nel listino indicato
nelle sue condizioni commerciali ed eventualmente convertiti nella
valuta corrente (secondo quanto impostato in Mexal nella relativa
tabella delle conversioni). che può essere quella determinata dal paese
di appartenenza dell'utente oppure quella selezionata all'interno del
apposito componente di "Cambio Valuta".

**NOTA BENE:** nel caso in cui siano state definite in Mexal delle
particolarità prezzo legate al listino associato al paese di
appartenenza dell'utente che sta visitando il sito, queste verranno
applicate e visualizzate indipendentemente dal fatto che l'utente abbia
effettuato o meno l'autenticazione e indipendentemente dal fatto che
l'applicazione sia stata impostata per riconoscere o meno lo specifico
cliente.

