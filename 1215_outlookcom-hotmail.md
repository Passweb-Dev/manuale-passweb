# OUTLOOK.COM / HOTMAIL



**Tipo di sicurezza**: SSL/TLS

**Domini di riferimento**: outlook.com -- hotmail.com

**Server SMTP**: smtp-mail.outlook.com

**Porta**: 587

**Richiedi Accesso**: Si

**Nome Utente / Password**: credenziali di accesso della casella mail
indicata all'interno del precedente campo E-mail.

**ATTENZIONE! Outlook.com così come Hotmail possono gestire
l'autenticazione in due fattori, un metodo di autenticazione questo che
garantisce un ulteriore livello di sicurezza per il proprio account di
posta e che si basa sull'utilizzo congiunto di due distinti metodi di
accesso.**

**Nel momento in cui dovesse essere stata abilitata questo tipo di
autenticazione, non sarà quindi più possibile autenticarsi alla propria
casella di posta fornendo solamente login e password**.

Per maggiori informazioni relativamente a come abilitare e gestire
questo tipo di autenticazione si consiglia di fare riferimento alla
relativa documentazione dello specifico fornitore.

In queste condizioni dunque anche il server SMTP definito all'interno
del proprio sito Passweb dovrà essere configurato in maniera corretta.

Nello specifico sarà necessario accedere alla configurazione del proprio
profilo Outlook.com / Hotmail, cliccare sulla voce di menu relativa alle
impostazioni di sicurezza

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\server_smtp_outlook.bmp](./assets/media/image4.png){width="5.454166666666667in"
height="3.1597222222222223in"}

e da qui selezionare la voce "**Altre opzioni di sicurezza**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\server_smtp_outlook2.bmp](./assets/media/image5.png){width="5.454166666666667in"
height="3.31875in"}

All'interno della pagina "Altre opzioni di sicurezza" sarà quindi
possibile gestire l'attivazione/disattivazione dell' autenticazione in
due fattori (sezione "**Verifica in due Passaggi**")

![Videate\\server_smtp_outlook3.bmp](./assets/media/image6.png){width="5.454166666666667in"
height="3.31875in"}

Nel caso in cui sia stata attivata questo tipo di autenticazione sarà
quindi necessario generare una password specifica da poter poi inserire
lato Passweb in fase di configurazione del server SMTP esterno che si
intende utilizzare.

Per fare questo sarà sufficiente cliccare sul pulsante "**Crea una Nuova
Password per l'app**" presente all'interno della sezione "**Password
dell'app**" e copiare la password così generata all'interno del relativo
campo presente nella maschera di configurazione del server SMTP Esterno
sul Wizard del proprio sito Passweb.

