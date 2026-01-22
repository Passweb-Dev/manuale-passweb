# CONDIZIONI DI VISIBILITA' E OBBLIGATORIETA' PER I CAMPI INTERNI AL FORM DI REGISTRAZIONE/PROFILO UTENTE



Per ogni controllo (Campo di Testo, Campo Radio, Campo Checkbox, Campo
Lista Valori ecc...) interno ad un Form di "**Registrazione Utente**"
e/o di "**Profilo Utente**" è possibile definire specifiche condizioni
di visibilità e/o obbligatorietà mediante le quali poter rendere il
controllo stesso visibile e/o obbligatorio sulla base dei seguenti
campi:

- **Nazione:** consente di impostare una condizione di visibilità /
  obbligatorietà definita sulla base della nazione dichiarata
  all'interno dell'apposito campo del form, dall'utente che sta
  navigando il sito.

> **ATTENZIONE! In queste condizioni affinchè il controllo di visibilità
> / obbligatorietà possa funzionare in maniera corretta è necessario
> inserire nello stesso form anche un campo "Lista Valori" mappato sul
> valore "Nazione Anagrafica Utente"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_visibilità_nazione_anagrafica_utente_res.bmp](./assets/media/image169.png)

> In questo modo è quindi possibile impostare il componente in esame
> come visibile / obbligatorio, dipendentemente dalla specifica Nazione
> selezionata dall'utente stesso all'interno del relativo controllo di
> tipo "Lista Valori"

![Videate\\campi_form_condizioni_obbligatorieta_nazione_res.bmp](./assets/media/image170.png)

> **ATTENZIONE! Nel caso in cui all'interno del form non sia presente
> alcun un controllo di tipo "Lista Valori" mappato sul Campo di
> Destinazione "Nazione Anagrafica Utente", la condizione di
> visibilità/obbligatorietà verrà valutata, in prima istanza, sulla base
> della lingua impostata sul browser utilizzato per navigare il sito.
> Nel caso in cui tale lingua sia priva dell'indicazione dello specifico
> paese, la provenienza del visitatore, e conseguentemente la condizione
> di visibilità, verrà valutata invece sulla base del suo indirizzo IP**
> (per maggiori informazioni in merito si veda anche la sezione "*Sito
> -- Gestione Lingue del sito -- Visualizzazione contenuti in lingua*"
> di questo manuale)

- **Privato:** consente di impostare una condizione di visibilità /
  obbligatorietà definita sulla base della scelta effettuata dall'utente
  all'interno del form di Registrazione in corrispondenza del controllo
  "**Persona Fisica / Azienda**"

![Videate\\campi_form_condizioni_obbligatorieta_privato_res.bmp](./assets/media/image171.png)

> In questo modo è quindi possibile impostare il componente in esame
> come visibile / obbligatorio, solo per utenti Privati (opzione
> "Persona Fisica") oppure solo per utenti di tipo Azienda (opzione
> "Azienda")

- **Fattura elettronica:** consente di impostare una condizione di
  visibilità / obbligatorietà definita sulla base della scelta
  effettuata dall'utente che sta compilando il form, in relazione ad un
  controllo di tipo Radio Button configurato impostando il parametro
  "**Tipo Valore**" su "**Scelta**" e "**Campo di Destinazione**" su
  "**Fattura Elettronica**", controllo questo che dovrà quindi essere
  necessariamente inserito all'interno dello form stesso

![Videate\\campi_form_condizioni_obbligatorieta_fa_res.bmp](./assets/media/image172.png)

> Con questa opzione è quindi possibile impostare il componente in esame
> come visibile / obbligatorio in base al fatto che l'utente abbia
> dichiarato di voler o non voler ricevere la fattura elettronica.
>
> Per maggiori informazioni in merito alla possibilità di mappare un
> componente "Radio Button" sul campo "Fattura elettronica" si veda
> anche il relativo capitolo di questo manuale "*Campo Radio
> (Registrazione e Profilo Utente)*"
>
> **ATTENZIONE!** Il fatto lasciare agli utenti del sito la possibilità
> di decidere se per essi debba o meno essere emessa fattura elettronica
> potrebbe essere fiscalmente non corretto. **Si consiglia dunque di
> fare particolare attenzione nel momento in cui si dovesse decidere di
> adottare questa opzione.**

- **Ente Pubblico:** consente di impostare una condizione di visibilità
  / obbligatorietà definita sulla base della scelta effettuata
  dall'utente che sta compilando il form, in relazione ad un controllo
  di tipo Radio Button configurato impostando il parametro "**Tipo
  Valore**" su "**Scelta**" e "**Campo di Destinazione**" su "**Ente
  Pubblico**", controllo questo che dovrà quindi essere necessariamente
  inserito all'interno dello form stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\campi_form_condizioni_obbligatorieta_pa_res.bmp](./assets/media/image173.png)

> Con questa opzione è quindi possibile impostare il componente in esame
> come visibile / obbligatorio in base al fatto che l'utente abbia
> dichiarato di essere o meno una pubblica amministrazione.
>
> Per maggiori informazioni in merito alla possibilità di mappare un
> componente "Radio Button" sul campo "Ente Pubblico" si veda anche il
> relativo capitolo di questo manuale "*Campo Radio (Registrazione e
> Profilo Utente)*"

- **Attributi Utente**: oltre ai campi precedentemente indicati è
  possibile impostare una condizione di visibilità / obbligatorietà
  definita sulla base del valore assunto da uno qualsiasi degli
  "Attributi Utente" (**ad eccezione di quelli di tipo File**)
  eventualmente inseriti all'interno del relativo form

Per poter definire le condizioni di visibilità e/o obbligatorietà è
necessario agire rispettivamente mediante i campi "**Condizione di
Visibilità**" e "**Condizione di Obbligatorietà**" presenti nella
maschera di configurazione di ogni singolo componente interno ai form di
"**Registrazione Utente**" e/o di "**Profilo Utente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizioni_visibilita_obbligatorieta_res.bmp](./assets/media/image174.png)

Nello specifico sarà quindi necessario cliccare, per prima cosa, sul
pulsante "**Aggiungi nuovo filtro**" e selezionare dal contestuale menu
a tendina il campo sulla base del quale andare poi ad impostare la
condizione di Visibilità / Obbligatorietà .

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campi_form_condizioni_obbligatorieta_res.bmp](./assets/media/image175.png)

Sarà poi necessario selezionare l'operatore relazionale da utilizzare
per definire la condizione di visibilità oltre che, ovviamente, i valori
per i quali la condizione di visibilità / obbligatorietà dovrà o meno
essere soddisfatta.

Cliccando, ad esempio, sull'etichetta "**Nazioni**" verrà aperta una
piccola finestra contenente l'elenco di tutte le nazioni utilizzabili
per definire la condizione di visibilità / obbligatorietà dello
specifico campo del form.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\condizione_visibilita_nazioni_registrazione_res.bmp](./assets/media/image176.png)

**ATTENZIONE! nella finestra sopra evidenziata verranno visualizzati
solo ed esclusivamente i paesi effettivamente abilitati per il proprio
sito** (vale a dire quelli selezionati alla pagina "Gestione Paesi" del
Wizard)

Una volta impostate le Nazioni in grado di soddisfare la condizione di
visibilità / obbligatorietà sarà poi sufficiente chiudere la finestra di
selezione del Paese (cliccando in un qualsiasi punto del box relativo al
parametro "Condizioni di Visibilità") e salvare il componente del form
che si sta modificando mediante l'apposito pulsante posto nella parte
alta della maschera.

Infine è bene sottolineare anche che:

- Nel caso in cui un dato campo del form risulti non visibile a seguito
  dell'applicazione di determinate condizioni di visibilità, lo stesso
  campo non verrà mai considerato come obbligatorio ai fini della
  corretta compilazione del form, indipendentemente dal fatto che, per
  esso, siano state impostate o meno eventuali condizioni di
  obbligatorietà.

- Nel caso in cui il parametro "Campo Obbligatorio" sia stato impostato
  sul valore SI e non siano state definite specifiche condizioni di
  obbligatorietà, il campo in esame sarà considerato sempre come
  obbligatorio per la corretta compilazione del form
