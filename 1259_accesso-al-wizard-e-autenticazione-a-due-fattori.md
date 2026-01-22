# ACCESSO AL WIZARD E AUTENTICAZIONE A DUE FATTORI



Come accennato nel precedente capitolo di questo manuale **per poter
accedere al back end del proprio sito Passweb è obbligatorio passare
attraverso un meccanismo di autenticazione a due fattori (MFA)** che
aumenta i criteri di sicurezza e protezione dei propri dati.

Questo meccanismo di autenticazione richiede infatti, obbligatoriamente,
oltre alle credenziali utente (Username e Password), l'inserimento anche
di un apposito codice a 6 cifre che potrà essere generato utilizzando
l'App "**Google Authenticator**" disponibile gratuitamente sullo store
del proprio smartphone (iOS o Android).

**ATTENZIONE! A partire dalla versione 2022A di Passweb l'accesso al
backend del proprio sito mediante autenticazione è obbligatorio e non
può essere disattivato**

Al momento del primo accesso, una volta inserite Username e Password,
cliccando sul pulsante di Login verrà quindi visualizzata un'ulteriore
schermata contenente il QR Code da utilizzare per attivare, all'interno
dell'App "**Google Authenticator**", la generazione dei codici necessari
per completare il processo di autenticazione oltre, ovviamente, al campo
di input in cui poter inserire questi stessi codici

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_2fa_6.bmp](./assets/media/image10.png){width="5.811805555555556in"
height="3.83125in"}

In sostanza dunque per poter superare l'autenticazione a due fattori
sarà necessario:

- Scaricare sul proprio smartphone l'applicazione **Google
  Authenticator** disponibile gratuitamente sia sul Play Store (per
  dispositivi Android) che sull' App Store (per dispositivi iOS)

- Cliccare sul pulsante di aggiunta di un nuovo account

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amministrazione_2fa_2.bmp](./assets/media/image11.png){width="1.7208333333333334in"
height="3.734027777777778in"}

- Selezionare l'opzione "**Scansiona un codice QR**"

![Videate\\amministrazione_2fa_3.bmp](./assets/media/image12.png){width="1.7208333333333334in"
height="3.734027777777778in"}

> e utilizzare quindi il proprio smartphone per scansionare il QR code
> visualizzato nella maschera di accesso al Wizard

- Inserire il codice a 6 cifre generato dall' App **Google
  Authenticator** all'interno dell'apposito campo presente, anch'esso,
  nella maschera di accesso Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_2fa_7.bmp](./assets/media/image13.png){width="5.811805555555556in"
height="3.83125in"}

> e cliccare quindi sul pulsante di Login
>
> Ovviamente i codici generati dall' App hanno validità limitata nel
> tempo per cui l'accesso al backend del proprio sito potrà essere
> effettuato solo nel momento in cui il codice inserito sia
> effettivamente quello attualmente visualizzato all'interno dell'App

**ATTENZIONE! Il QR Code necessario per attivare la generazione dei codi
a 6 cifre verrà visualizzato solo al primo accesso**

Una volta configurata correttamente la propria App di autenticazione
quindi, durante i successivi accessi al Wizard verrà visualizzato
solamente il campo di input in cui inserire il codice a 6 cifre
prelevato dall' App

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_2fa_2.bmp](./assets/media/image14.png){width="5.811805555555556in"
height="3.7729166666666667in"}

Il check "**Non chiedermelo per X giorni su questo browser**" consente
invece di decidere per quanti giorni potrà essere possibile effettuare
l'accesso al Wizard bypassando l'inserimento del codice a 6 cifre ed
utilizzando quindi solamente le proprie credenziali utente (Username e
Password).

**ATTENZIONE! per poter bypassare l'inserimento del codice a 6 cifre
verrà salvato sul browser dell'utente un apposito cookie con durata pari
al numero di giorni inseriti nell'apposito campo di input.**

In conseguenza di ciò nel momento in cui dovessero essere eliminati i
cookie del browser prima della scadenza indicata o, allo stesso modo, si
dovesse tentare di effettuare l'accesso al Wizard del proprio sito con
lo stesso utente ma da un browser / pc diverso da quello precedentemente
utilizzato, verrà richiesto nuovamente l'inserimento del codice a 6
cifre

Nel momento in cui non si dovesse disporre di uno smartphone su cui
poter installare l'App Google Authenticator sarà comunque possibile
generare i codici a 6 cifre necessari per superare l'autenticazione a
due fattori, utilizzando l' estensione di Chrome disponibile al seguente
link:

[[https://chrome.google.com/webstore/detail/authenticator/bhghoamapcdpbohphigoooaddinpkbai]{.underline}](https://chrome.google.com/webstore/detail/authenticator/bhghoamapcdpbohphigoooaddinpkbai)

Il funzionamento di questo plugin è del tutto analogo a quello dell'App
Google Authenticator appena descritta. Una volta installato sarà quindi
necessario cliccare sul pulsante di scansione del QR Code presente nella
pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_2fa_8.bmp](./assets/media/image15.png){width="5.811805555555556in"
height="4.298611111111111in"}

e selezionare quindi il QR Code mostrato a video.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_2fa_10.bmp](./assets/media/image16.png){width="5.811805555555556in"
height="3.83125in"}

Attivato l'account sarà poi sufficiente richiamare nuovamente il plugin
per visualizzare il codice a 6 cifre richiesto dall'autenticazione a due
fattori

