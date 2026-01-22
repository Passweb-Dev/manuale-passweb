# CONFIGURAZIONE RICHIESTE IP



La sezione "**Configurazione Richieste IP**" consente di attivare
eventuali blocchi sulla base dell'indirizzo ip delle richieste in arrivo
al sito

![](./assets/media/image282.png)

Nello specifico il parametro:

**Abilita:** consente di attivare / disattivare le regole automatico di
blocco delle richieste sulla base del singolo indirizzo ip associato
alla richiesta stessa.

Attivando questo parametro dunque, nel momento in cui dovessero poi
arrivare da uno stesso indirizzo ip, nell'intervallo di tempo indicato
(parametro "Intervallo Richieste" della sezione "Generale") un numero di
richieste superiore a quello indicato (parametro "Numero Massimo di
Richieste" della sezione "Generale") quello stesso indirizzo ip verrà
automaticamente bloccato per un periodo di tempo pari a quello indicato
all'interno del relativo campo ("Intervallo Divieto") della sezione
"Generale"

**Abilita blocco per Subnet Mask:** consente di attivare / disattivare
le regole automatiche di blocco per intere Subnet mask di indirizzi ip

Nello specifico, attivando questo parametro per valutare l'applicazione
o meno di un determinato blocco non verrà più preso in considerazione
l'intero indirizzo ip ma, al contrario, verranno esaminati solamente i
primi 3 ottetti degli indirizzi ip associati alle diverse richieste.

**ATTENZIONE!** si ricorda che un indirizzo IP è composto da numeri a 32
bit, solitamente scritti in notazione con punto, ad esempio
73.227.130.85. I numeri tra i punti sono chiamati ottetti (8 bit)

Supponendo dunque di ricevere nell'intervallo di tempo indicato
(parametro "Intervallo Richieste" della sezione "Generale") un numero di
richieste superiore a quello indicato (parametro "Numero Massimo di
Richieste" della sezione "Generale") e provenienti da indirizzi ip
diversi ma tutti con gli stessi primi 3 ottetti (quindi indirizzi del
tipo **73.227.130**.15 / **73.227.130**.16 / **73.227.130**.52 ...) ad
essere bloccato non sarà più il singolo indirizzo ip ma tutti quelli con
i primi 3 ottetti uguali a quelli che hanno determinato l'applicazione
della regola di blocco.

L'attivazione di questo parametro potrebbe essere particolarmente utile
nei confronti di quegli "attacchi" provenienti da bot net acquistate su
spazi cloud che producono un numero eccessivo di visite al sito da ip
differenti ma solitamente appartenenti tutti ad una stessa classe (primi
3 ottetti uguali).

**ATTENZIONE!** il parametro "Abilita blocco per Subnet Mask", per
quanto utile, potrebbe portare anche ad un ban temporaneo di alcuni
indirizzi ip corretti

**ATTENZIONE!** le regole di blocco definite all'interno della sezione
"Configurazione Richieste IP" verranno prese in considerazione solo nel
caso in cui il parametro "**Abilita Prevenzione DDos**" (sezione
"Generale") sia stato correttamente attivato

