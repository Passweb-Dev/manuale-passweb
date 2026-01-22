# INTEGRAZIONE CRIBIS



Come accennato nel precedente capitolo di questo manuale, grazie
all'integrazione tra Passweb e CRIBS, nel momento in cui un Agente
dovesse effettuare la registrazione di un nuovo cliente, potrebbe
sfruttare la funzione di autocompletamento di alcuni campi del form
prelevando le informazioni necessarie direttamente dal database di
CRIBIS.

**ATTENZIONE! Per utilizzare la funzionalità in oggetto sul front end
del sito Ecommerce,** **è necessario aver attivato il relativo modulo
(Arricchimento Anagrafiche) nell'installazione Mexal collegata al sito
stesso**

Lato Wizard, come accennato nel precedente capitolo di questo manuale,
sarà possibile configurare i campi del form di **Registrazione Utente**
relativi alla "**Partita IVA**" e/o al "**Codice Fiscale**" in maniera
tale che i valori inseriti all'interno di questi campi facciano da
chiave per la ricerca della corrispondente anagrafica sul database di
CRIBIS.

Nello specifico per ottenere ciò sarà sufficiente selezionare il
parametro "**Abilita autocompletamento campi CRIBIS**" presente nella
maschera di configurazione del componente "Campo di Testo"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_cribis_1.bmp](./assets/media/image87.png){width="4.792361111111111in"
height="3.0520833333333335in"}

**ATTENZIONE!** il parametro "**Abilita autocompletamento campi
CRIBIS**" verrà visualizzato **solo nel momento in cui il componente
"Campo di Testo" sia stato correttamente mappato sulla Partita IVA o sul
Codice Fiscale** (parametro "Tipo di Dato di Destinazione = Campo
Cliente" e "Campo di Destinazione = Partita IVA / Codice Fiscale")

In queste condizioni quando un Agente andrà ad effettuare la
registrazione di un nuovo cliente troverà a fianco dei campi relativi
alla Partita IVA e / o al Codice Fiscale un pulsante di "Ricerca"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_cribis_3.bmp](./assets/media/image90.png){width="5.434722222222222in"
height="3.532638888888889in"}

Una volta inserita la Partita IVA (**senza IT**) e/o il Codice Fiscale
desiderato, cliccando sul pulsante evidenziato in figura verrà
effettuata una ricerca in tempo reale sul Database di CRIBIS e verranno
visualizzati all'interno di un apposito menu a tendina le possibili
anagrafiche che soddisfano i parametri di ricerca impostati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_cribis_4.bmp](./assets/media/image91.png){width="5.434722222222222in"
height="3.532638888888889in"}

Selezionando quindi una delle anagrafiche presenti in elenco verranno
automaticamente compilati, con i dati di questa stessa anagrafica, anche
altri campi presenti all'interno dello stesso form di registrazione
utente (es. Ragione Sociale, Telefono, Indirizzo ...).

Relativamente alla funzione di autocompletamento fornita
dall'integrazione Passweb -- CRIBS occorre comunque fare alcune
considerazioni di fondamentale importanza.

Nello specifico è sempre bene ricordare che:

- Non tutti i campi presenti all'interno del form di registrazione
  utente potrebbero essere compilati in automatico dalla funzionalità in
  oggetto. Il tutto dipende ovviamente dal tipo di campo inserito
  all'interno del form di registrazione e da quelle che sono le
  informazioni ottenute da CRIBS.

> In generale dunque nel momento in cui determinati campi del form di
> registrazione utente non dovessero essere auto compilati a seguito
> della ricerca effettuata in CRIBS, ciò starà ad indicare che CRIBS
> stesso non fornisce dati per quella specifica informazione.

- I valori inseriti a seguito dell'auto completamento sono sempre e
  soltanto valori propositivi. Sarà poi l'Agente a dover verificare la
  correttezza dei dati e a confermare manualmente la registrazione
  dell'utente.

- La funzione di autocompletamento è disponibile solo per gli utenti di
  tipo Agente

