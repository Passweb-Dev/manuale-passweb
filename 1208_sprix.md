# SPRIX



All'interno di questa sezione l'utente attualmente loggato ha la
possibilità di visualizzare ed eseguire tutti gli sprix (personali e
standard) correttamente mappati all'interno del Wizard e che l'utente è
effettivamente in grado di gestire.

**NOTA BENE:** per maggiori informazioni relativamente a come mappare
all'interno di Passweb uno sprix e /o a come concedere o meno, ad un
utente abilitato ad accedere in Area Riservata, anche il permesso di
eseguire determinati sprix si veda anche la sezione "Configurazione --
Gestione Sprix" di questo manuale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_sprix_passcom.bmp](./assets/media/image174.png)

**ATTENZIONE!** Per poter accedere a questa sezione è necessario aver
abilitato la relativa App operando per questo all'interno dell'apposita
sezione del Wizard accessibile dal menu "*Sito -- Preferenze*".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_sprix_attivazione_passcom.bmp](./assets/media/image175.png)

Per poter lanciare l'esecuzione, lato gestionale, di uno degli sprix
presenti in elenco è necessario per prima cosa selezionarlo e cliccare
poi sul pulsante **Configura** (
![Videate\\ar_pulsante_configura.bmp](./assets/media/image176.png) ) presente nella contestuale barra degli
strumenti.

In questo modo verrà infatti visualizzata la maschera di configurazione
dello sprix attraverso cui poter inserire tutti i parametri necessari
per il suo corretto funzionamento

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_sprix_passcom.bmp](./assets/media/image177.png)

**NOTA BENE:** per maggiori informazioni relativamente a come gestire
questo form si veda anche la sezione "Configurazione -- Gestione Sprix"
di questo manuale.

Oltre ai parametri impostati sul Wizard, come primo campo all'interno di
questo form, verrà sempre visualizzato il campo **"Nome del file di
dati"** attraverso cui poter indicare il nome con cui dovrà essere
memorizzato all'interno del sito il file restituito dallo sprix (a
default il campo propone la descrizione dell'eseguibile sprix inserita
lato Wizard + il codice conto dell'utente attualmente connesso).

**ATTENZIONE! Uno stesso eseguibile sprix potrà essere lanciato più
volte. Nel caso però in cui venga utilizzato per due diverse
elaborazioni lo stesso valore per il campo "Nome del file di dati" i
risultati dell'ultima elaborazione andranno a sovrascrivere quelli delle
elaborazioni precedenti.**

Per i campi di tipo Stringa il cui valore di default è stato impostato
sul valore automatico "**Codice Conto**" verrà proposto, a default, ed
in maniera del tutto automatica, il codice conto dell'utente attualmente
loggato.

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

![Videate\\form_sprix_errore.bmp](./assets/media/image178.png)

Nel caso in cui invece l'elaborazione vada a buon fine verrà aperta una
finestra all'interno della quale poter visualizzare un'anteprima del
contenuto del file restituito dall'elaborazione.

Tale risultato verrà poi memorizzato all'interno della sezione
**"Risultati"** dove l'utente verrà automaticamente ridiretto al termine
dell'elaborazione stessa.

![Videate\\form_sprix_risultati.bmp](./assets/media/image179.png)

All'interno di questa sezione, accessibile direttamente anche attraverso
l'apposito pulsante presente nella barra degli strumenti della sezione
Sprix (
![Videate\\ar_pulsante_risultati.bmp](./assets/media/image180.png) ), l'utente avrà quindi la possibilità di gestire,
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
![Videate\\ar_pulsante_scarica_documento.bmp](./assets/media/image181.png) ): consente di effettuare il download del file dei
risultati attualmente selezionato in elenco

**Anteprima** (
![Videate\\area_riservata_documenti_anteprima_documento.bmp](./assets/media/image108.png) ):: consente di visualizzare un' anteprima del file
dei risultati attualmente selezionato in elenco

**Elimina** (
![Videate\\sprix_elimina_documento.bmp](./assets/media/image182.png) ): consente di eliminare il file dei risultati
attualmente selezionato in elenco

