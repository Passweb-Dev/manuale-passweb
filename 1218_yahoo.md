# YAHOO



**Domini di riferimento**: yahoo.com -- yahoo.it

**Server SMTP**: smtp.mail.yahoo.it / smtp.mail.yahoo.com

**Porta**: 587

**Tipo di sicurezza**: SSL/TLS

**Richiedi Accesso**: Si

**Nome Utente / Password**: credenziali di accesso della casella mail
indicata all'interno del precedente campo E-mail.

**ATTENZIONE! Yahoo può gestire l'autenticazione in due fattori, un
metodo di autenticazione questo che garantisce un ulteriore livello di
sicurezza per il proprio account di posta e che si basa sull'utilizzo
congiunto di due distinti metodi di accesso.**

**Nel momento in cui dovesse essere stata abilitata questo tipo di
autenticazione, non sarà quindi più possibile autenticarsi alla propria
casella di posta fornendo solamente login e password.**

Per maggiori informazioni relativamente a come abilitare e gestire
questo tipo di autenticazione si consiglia di fare riferimento alla
relativa documentazione dello specifico fornitore.

In queste condizioni dunque anche il server SMTP definito all'interno
del proprio sito Passweb dovrà essere configurato in maniera corretta.

Nello specifico sarà necessario accedere alla pagina di configurazione
del proprio Account Yahoo cliccando per questo sulla voce "**Info
Account**" presente all'interno del menu evidenziato in figura

![](./assets/media/image14.png)

Sarà quindi necessario portarsi nella sezione relativa alla "**Sicurezza
dell'Account**"

![](./assets/media/image15.png)

e cliccare sul pulsante "**Genera Password dell'app**" come indicato
nella figura sopra riportata.

Nella successiva maschera selezionare quindi l'opzione "**Altra App**" e
indicare un nome come richiesto.

Cliccando infine sul pulsante "**Generate**" verrà cerata la password
che dovrà poi essere copiata all'interno del relativo campo presente
nella maschera di configurazione del server SMTP Esterno sul Wizard del
proprio sito Passweb.

**ATTENZIONE!** Nel caso in cui si sia deciso di non abilitare
l'autenticazione in due passaggi e si renda comunque necessario
utilizzare il server di posta di Yahoo potrebbe essere necessario
attivare l'opzione "Consenti le app che utilizzano un accesso meno
sicuro" come evidenziato nella figura di seguito riportata

![](./assets/media/image16.png)

