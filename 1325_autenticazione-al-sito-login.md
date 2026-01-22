# AUTENTICAZIONE AL SITO -- LOGIN



**Nome Evento**: login

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Utente**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà un utente effettuerà il login al sito

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'login', {*

*method: 'Sito',*

*dateTime:'11/10/2022, 14:54:56'*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **method:** stringa identificativa del metodo utilizzato per
  effettuare l'autenticazione al sito. Può assumere uno dei seguenti
  valori:

  - **Sito:** valore assegnato nel caso in cui l'autenticazione venga
    effettuata mediante un account registrato sul sito

  - **Facebook/Twitter/Google/PayPal ...**: valore assegnato nel caso in
    cui l'autenticazione venga effettuata con un social

- **dateTime:** data e ora in cui si è verificato l'evento

