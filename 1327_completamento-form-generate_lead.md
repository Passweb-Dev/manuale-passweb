# COMPLETAMENTO FORM -- GENERATE_LEAD



**Nome Evento**: generate_lead

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Eventi Utente**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà completata con successo la compilazione di un form Passweb

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'generate_lead', {*

*form_name: 'Form Contatti',*

*dateTime:'11/10/2022, 14:54:56'*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **form_name:** Form + nome assegnato in passweb al componente form

- **dateTime:** data e ora in cui si è verificato l'evento

