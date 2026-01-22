# SITI COMMERCIALISTA -- SINCRONIZZAZIONE



In un sito Commercialista la procedura di **Sincronizzazione** è quella
particolare operazione che consente a Passweb di prelevare, dal
gestionale, le aziende opportunamente abilitate per essere gestite anche
all'interno del sito, e di concedere dunque alle relative utenze la
possibilità di accedere in area riservata.

A differenza di quanto avviene per i siti Ecommerce, in un sito
Commercialista esiste una sola tipologia di sincronizzazione che può
essere lanciata manualmente, operando all'interno del Wizard del proprio
sito, oppure schedulata ed eseguita automaticamente a precisi intervalli
di tempo.

La maschera "**Parametri Sincronizzazione**", accessibile dalla voce di
menu **"Configurazione - Sincronizzazione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_parametri_sincronizzazione.bmp](./assets/media/image200.png){width="5.7659722222222225in"
height="3.33125in"}

consente quindi di indicare con che frequenza dovranno essere effettuate
le operazioni di sincronizzazione gestite in automatico
dall'applicazione, specificando eventualmente anche l'ora esatta in cui
dovrà partire la sincronizzazione.

E' possibile, in particolare, indicare anche gli specifici giorni della
settimana (selezionando "**Ogni settimana**") in cui dovrà essere
effettuata tale operazione.

I giorni selezionati con il relativo segno di spunta sono i giorni
ammessi; pertanto se, ad esempio, si volesse evitare di lanciare
sincronizzazioni la domenica, occorrerà togliere il segno di spunta in
corrispondenza del campo "domenica".

**NOTA BENE**: il controllo sui giorni della settimana viene effettuato
unicamente dal servizio di sincronizzazione automatica. Nulla vieta
all'utente di avviare una sincronizzazione manuale anche nei giorni non
specificatamente indicati.

Il campo **E-Mail** consente di specificare uno o più indirizzi di posta
elettronica (eventualmente separati dal carattere ';') cui dovrà essere
inviata una mail per avvisare dell'avvenuta operazione di
sincronizzazione (ovviamente questa funzionalità sarà attivata solamente
nel caso in cui si sia deciso di attivare la gestione delle mail
indicando un indirizzo valido alla pagina "Posta/SMS" del Wizard).

La sezione "**Sincronizzazione**" consente infine di:

- Visualizzare il messaggio relativo all'esito dell'ultima
  sincronizzazione effettuata, indipendentemente dal fatto che questa
  sia stata una sincronizzazione manuale oppure una sincronizzazione
  automatica (casella "Esito ultima Sincronizzazione")

- Effettuare una sincronizzazione manuale (pulsante
  "**Sincronizzazione**" ) e controllarne lo stato di avanzamento
  attraverso la relativa progress bar.

