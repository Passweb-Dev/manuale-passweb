# VISITOR: NULL



Utilizzando questa impostazione (*visitor: null*) non verrà generato
nessun id di sessione e non verrà quindi raccolto nessun dato sui
visitatori del sito.

Va da sé che, in queste condizioni, non ci saranno particolari obblighi
GDPR da prendere in considerazione. Non sarà quindi necessario inserire
l'opzione di Opt-out nel modulo di Registrazione / Profilo Utente né
tanto meno sarà necessario sottoporre l'attivazione dello script di
configurazione all'accettazione dei cookie.

In queste condizioni i moduli di Clerk eventualmente implementati
all'interno del sito continueranno a funzionare normalmente tranne per
quelle che sono le funzionalità legate alle azioni dei visitatori (come
ad esempio le raccomandazioni basate sulla cronologia di navigazione o
l'invio di mail relative al termine di una sessione di navigazione senza
aver effettuato acquisti).

Allo stesso modo anche eventuali vendite originate a partire da uno dei
moduli Clerk presenti sul sito non potranno essere attribuite a Clerk e
questo potrebbe chiaramente portare ad una sottostima di quelli che sono
i risultati effettivamente prodotti dall'utilizzo di questa piattaforma

Detto che, per ovvie ragioni, questa impostazione è sicuramente la meno
consigliata da applicare, è anche bene sottolineare come potrebbe invece
essere utile se attivata solo per eventuali utenti di test (modificando
quindi dinamicamente lo script di configurazione dopo il login) per fare
in modo che i dati relativi a questi stessi utenti non vadano a
inquinare i risultati reali prodotti dalla piattaforma, oppure se
utilizzata in combinazione alle opzioni *visitor: 'persistent'* o
*visitor: 'CUSTOM'* per evitare il blocco completo dei moduli
eventualmente implementati all'interno del sito nel momento in cui un
utente dovesse decidere di non prestare i relativi consensi.

Per maggiori informazioni relativamente a come Passweb combina
l'utilizzo delle due opzioni *visitor: null* e *visitor: CUSTOM* si veda
anche quanto indicato nel successivo capitolo

