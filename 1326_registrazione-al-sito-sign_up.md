# REGISTRAZIONE AL SITO -- SIGN_UP



**Nome Evento**: sign_up

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Utente**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui un nuovo utente effettuerà la registrazione al sito

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'sign_up', {*

*method: 'Sito',*

*dateTime:'11/10/2022, 14:54:56'*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **method:** stringa identificativa del metodo utilizzato per
  effettuare la registrazione al sito. Può assumere uno dei seguenti
  valori:

  - **Sito:** valore assegnato nel caso in cui la registrazione venga
    effettuata mediante l'apposito form presente sul sito

  - **Facebook/Twitter/Google/PayPal ...**: valore assegnato nel caso in
    cui la registrazione venga effettuata tramite social

- **dateTime:** data e ora in cui si è verificato l'evento

