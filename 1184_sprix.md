# SPRIX



Per poter accedere a questa particolare sezione dell'Area Riservata è
necessario, innanzitutto, aver abilitato l'App Sprix operando per questo
all'interno dell'apposita sezione del Wizard accessibile dal menu "*Sito
-- Preferenze*".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_sprix_attivazione.bmp](./assets/media/image223.png){width="5.565277777777778in"
height="3.5131944444444443in"}

**ATTENZIONE! La sezione Sprix è disponibile solo per siti Ecommerce
collegati a Mexal**

Una volta attivata l'App, all'interno di questa sezione dell' area
riservata avrà poi la possibilità di visualizzare ed eseguire tutti gli
sprix (personali e standard) che è effettivamente in grado di gestire.

**ATTENZIONE!** per maggiori informazioni relativamente a come mappare
all'interno di Passweb uno specifico sprix (sia esso uno sprix personale
oppure uno sprix standard) e per come renderlo visibile o meno ad un
determinato gruppo di utenti si rimanda a quanto indicato all'interno
della sezione "**Configurazione -- Gestione Sprix**" di questo manuale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_sprix.bmp](./assets/media/image224.png){width="5.66875in"
height="3.422222222222222in"}

Per poter lanciare l'esecuzione, lato gestionale, di uno degli sprix
presenti in elenco è necessario per prima cosa selezionarlo e cliccare
poi sul pulsante **Configura** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_pulsante_configura.bmp](./assets/media/image225.png){width="0.5in"
height="0.18819444444444444in"} ) presente nella contestuale barra degli
strumenti.

In questo modo verrà infatti visualizzata la maschera di configurazione
dello sprix attraverso cui poter inserire tutti i parametri necessari
per il suo corretto funzionamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_sprix.bmp](./assets/media/image226.png){width="5.66875in"
height="3.428472222222222in"}

**NOTA BENE:** per maggiori informazioni relativamente a come gestire
questo form si veda anche la sezione "Configurazione -- Gestione Sprix"
di questo manuale.

Oltre ai parametri impostati sul Wizard, come primo campo all'interno di
questo form, verrà sempre visualizzato il campo **"Nome del file di
dati"** attraverso cui poter indicare il nome con cui dovrà essere
memorizzato all'interno del sito il file restituito dallo sprix (a
default il campo propone la descrizione dell'eseguibile sprix inserita
lato Wizard + il codice conto dell'utente attualmente connesso).

**NOTA BENE:** l'utilizzo dello Sprix Remoto necessita di un terminale
libero del gestionale

**ATTENZIONE! Uno stesso eseguibile sprix potrà essere lanciato più
volte. Nel caso però in cui venga utilizzato per due diverse
elaborazioni lo stesso valore per il campo "Nome del file di dati" i
risultati dell'ultima elaborazione andranno a sovrascrivere quelli delle
elaborazioni precedenti.**

Per i campi di tipo Stringa il cui valore di default è stato impostato
sul valore automatico "**Codice Conto**" verrà proposto, a default, ed
in maniera del tutto automatica, il codice conto dell'utente attualmente
loggato. **Nel caso in cui dunque un agente debba lanciare una
elaborazione sprix per uno dei suoi clienti, e desideri che tale campo
venga compilato in automatico, dovrà per prima cosa autenticarsi come lo
specifico cliente.**

Una volta compilati tutti i campi del form, ed inseriti quindi i
parametri necessari per la corretta esecuzione dello sprix, cliccando
sul check **"Conferma"** presente nella parte alta della maschera,
verranno avviati tutti i controlli di integrità sui parametri inseriti,
verrà quindi verificato che il tipo di dato inserito sia coerente con la
tipologia di campo definita lato Wizard, verrà controllato che tutti i
parametri, definiti lato Wizard, come obbligatori siano stati
effettivamente valorizzati ecc...

Nel caso in cui tutti i controlli vengano superati con successo, verrà
avviata all'interno del gestionale la corrispondente elaborazione sprix.

**NOTA BENE:** gli sprix verranno eseguiti in maniera sincrona. Una
volta lanciata l'esecuzione di uno sprix, l'utente dovrà quindi
attendere il risultato dell'elaborazione per poterne visualizzare i
risultati. Non sarà quindi possibile spostarsi in una diversa sezione
dell'area riservata se non utilizzando il tasto back del browser. In
quest'ultimo caso il risultato dell'elaborazione potrà poi essere
visualizzato, al termine dell'elaborazione stessa, all'interno
dell'apposita sezione "Risultati" .

Nel caso in cui lo sprix dovesse ritornare degli errori, questi
verrebbero visualizzati all'interno del form di esecuzione, nella parte
bassa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_sprix_errore.bmp](./assets/media/image227.png){width="5.66875in"
height="3.4090277777777778in"}

Nel caso in cui invece l'elaborazione vada a buon fine verrà aperto un
nuovo tab del browser all'interno del quale poter visualizzare
un'anteprima del contenuto del file restituito dall'elaborazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\preview_documento.bmp](./assets/media/image228.png){width="5.66875in"
height="3.422222222222222in"}

Tale risultato verrà poi memorizzato anche all'interno della sezione
**"Risultati"**, sezione questa dove l'utente verrà automaticamente
ridiretto al termine dell'elaborazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_sprix_risultati.bmp](./assets/media/image229.png){width="5.604166666666667in"
height="3.370138888888889in"}

All'interno di questa sezione, accessibile direttamente anche attraverso
l'apposito pulsante presente nella barra degli strumenti della sezione
Sprix (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_pulsante_risultati.bmp](./assets/media/image230.png){width="0.4479166666666667in"
height="0.16875in"} ), l'utente avrà quindi la possibilità di gestire,
relativamente ai vari sprix, tutti i risultati generati dalle successive
elaborazioni.

**NOTA BENE:** ogni utente abilitato ad accedere in Area Riservata e a
lanciare determinati sprix, avrà una sua sezione "Risultati\". Non sarà
quindi possibile condividere i file risultato tra utenti diversi.

Per ogni file dei risultati presente in elenco viene visualizzato il
nome, indicato all'atto dell'esecuzione dello sprix all'interno del
campo **"Nome del file di dati",** la data di esecuzione e la dimensione
del file stesso.

Una volta selezionato uno dei file dei risultati i pulsanti presenti
nella contestuale barra degli strumenti consentiranno di:

**Scarica Documento** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_pulsante_scarica_documento.bmp](./assets/media/image231.png){width="0.7270833333333333in"
height="0.175in"} ): consente di effettuare il download del file dei
risultati attualmente selezionato in elenco

**Anteprima** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_documenti_anteprima_documento.bmp](./assets/media/image232.png){width="0.5194444444444445in"
height="0.16875in"} ):: consente di visualizzare un' anteprima del file
dei risultati attualmente selezionato in elenco

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_elimina_documento.bmp](./assets/media/image233.png){width="0.3958333333333333in"
height="0.175in"} ): consente di eliminare il file dei risultati
attualmente selezionato in elenco

