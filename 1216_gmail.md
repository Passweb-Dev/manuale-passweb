# GMAIL



**Domini di riferimento**: gmail.com

**Server SMTP**: smtp.gmail.com

**Porta**: 587

**Tipo di sicurezza**: SSL/TLS

**Richiedi Accesso**: Si

**Nome Utente / Password**: credenziali di accesso della casella mail
indicata all'interno del precedente campo E-mail.

**ATTENZIONE! Gmail può gestire l'autenticazione in due fattori, un
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
del proprio Account Google (<https://myaccount.google.com/u/2/> ),
entrare nella sezione relativa alle impostazioni di "**Accesso e
Sicurezza**"

![](./assets/media/image7.png)

e, nella sezione relativa ai "**Metodi di Accesso e Password**",
cliccare sulla voce "**Password per le app**"

![](./assets/media/image8.png)

A questo punto sarà quindi sufficiente impostare nel campo "**Seleziona
Applicazione**" il valore "**Posta**" e nel campo "**Seleziona
dispositivo**" il valore "**Computer Windows**"

![](./assets/media/image9.png)

Cliccando quindi sul pulsante **Genera** verrà cerata la password che
dovrà poi essere copiata all'interno del relativo campo presente nella
maschera di configurazione del server SMTP Esterno sul Wizard del
proprio sito Passweb.

