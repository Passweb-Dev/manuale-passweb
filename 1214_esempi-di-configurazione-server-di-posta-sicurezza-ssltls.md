# ESEMPI DI CONFIGURAZIONE SERVER DI POSTA -- SICUREZZA SSL/TLS



Come indicato nel precedente capitolo di questo manuale relativamente
alle mail inviate in automatico dall'applicativo potrebbero verificarsi
situazioni in cui decidendo di utilizzare il server di posta
Passepartout indicando però come mittente (campo E-mail) un indirizzo
mail che faccia riferimento ad un server SMTP (es.
mioindirizzo@yahoo.it) diverso da quello Passepartout, le mail non
vengano correttamente inviate.

**Queste situazioni sono indipendenti tanto dall'applicativo Passweb
quanto dal server di posta Passepartout e sono dovute essenzialmente a
specifiche policy adottate dai differenti gestori, alcuni dei quali
permettono l'invio di mail utilizzando un loro indirizzo solo ed
esclusivamente nel caso in cui ad inviare la posta sia effettivamente un
loro server.**

Potrebbe quindi non essere possibile l'invio di mail impostando come
mittente, ad esempio, un indirizzo del tipo mioindirizzo@yahoo.it e
utilizzando allo stesso tempo il server di posta
Passepartout.(Tipologia=Interno)

In queste condizioni dovrà quindi essere utilizzato necessariamente un
server SMTP esterno o, in alternativa, dovrà essere modificato
l'indirizzo mail del mittente

Di seguito sono indicate, a titolo puramente esemplificativo, alcune
possibili configurazioni dei server SMTP più comunemente utilizzati (es.
alice, Gmail, Yahoo, Outlook.com ecc...).

**Per maggiori informazioni in merito si consiglia comunque di fare
sempre riferimento alla documentazione dello specifico fornitore.**

