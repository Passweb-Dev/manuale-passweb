# USER ID



Anche per Matomo così come per Google Analytics il tracciamento mediante
User id (assegnato ai visitatori direttamente da Passweb mediante il
processo di Login) è sicuramente il metodo di identificazione più
accurato tra quelli di disponibili inquanto consente di riconoscere e
seguire facilmente l'utente in maniera cross device e cross platform.

**ATTENZIONE!** Come già indicato nei precedenti capitoli di questo
manuale **lo User Id è da considerarsi a tutti gli effetti come un dato
di identificazione personale** e questo anche nel momento in cui dovesse
essere utilizzata, come User Id, una generica stringa alfanumerica e/o
si dovesse ricorrere alle funzioni di anonimizzazione messe a
disposizione da Matomo.

In conseguenza di ciò nel momento in cui si dovesse decidere di attivare
e gestire anche questo tipo di tracciamento sarà necessario, da una
parte, fornire nelle Norme sulla gestione della privacy del proprio sito
un'informativa adeguata circa l'utilizzo degli identificatori utilizzati
e, dall'altra parte, verificare di aver gestito in maniera corretta la
richiesta di consenso preventivo.

Una volta appurato di essere in regola con quanto previsto dal GDPR per
attivare il tracciamento mediante User Id, lato client, sarà sufficiente
modificare il codice di tracciamento standard di Matomo inserendo la
seguente istruzione

**\_paq.push(\[\'setUserId\', {USER_ID}\]);**

![](./assets/media/image18.png)

dove **{UESER_ID}** è un segnaposto gestito dinamicamente da Passweb che
verrà sostituito a runtime con l'id assegnato da Passweb stesso ad ogni
utente al momento della sua autenticazione al sito.

Per quel che riguarda invece il tracciamento lato server, nel momento in
cui l'esigenza dovesse essere quella di passare a Matomo anche lo User
Id dell'utente che ha effettuato l'ordine, sarà sufficiente selezionare
il parametro "**Utilizza User id**" evidenziato in figura

![](./assets/media/image19.png)

Per maggiori informazioni relativamente al tracciamento lato server
disponibile nell'integrazione Passweb -- Matomo si rimanda a quanto
indicato nel relativo capitolo "*Matomo -- Tracciamento lato server*" di
questo manuale.

A questo indirizzo <https://matomo.org/guide/reports/user-ids/> è invece
possibile consultare la documentazione ufficiale Matomo relativamente al
tracciamento mediante User Id

