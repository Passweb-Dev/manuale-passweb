# SPRIX STANDARD -- ESTRATTO CONTO



Attraverso questo sprix è possibile mettere a disposizione in Area
Riservata, per gli utenti appositamente abilitati, uno specifico form
precablato attraverso il quale questi stessi utenti avranno poi la
possibilità di richiedere al gestionale, in tempo reale, **informazioni
relativamente all'estratto conto di uno specifico cliente**.

**ATTENZIONE!** in questo caso l'eseguibile che verrà mappato
all'interno del gestionale è uno sprix precablato e verrà richiamato
utilizzando Sprix Remoto

Per poter definire uno sprix di questo tipo è sufficiente cliccare sul
pulsante **"Nuovo"** **(**
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo.bmp](./assets/media/image204.png) **)** presente nella barra degli
strumenti della maschera "Gestione Sprix", e impostare poi il parametro
"**Tipologia**" sul valore "**Estratto Conto**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_estrattoconto.bmp](./assets/media/image214.png)

Il campo "**Descrizione**", presente all'interno della maschera sopra
evidenziata, consente di associare allo sprix in esame una specifica
descrizione, in maniera tale da poterlo poi identificare rispetto ad
altri eventuali sprix presenti in elenco.

Il parametro "**Visibile da**" consente invece di definire i gruppi di
utenti cui rendere disponibile questo stesso sprix all'interno dell'Area
Riservata del sito. E' possibile selezionare una delle seguenti opzioni:

- **Tutti:** il corrispondente sprix verrà messo a disposizione e potrà
  quindi essere lanciato da tutti gli utenti del sito abilitati ad
  accedere in Area Riservata

- **Solo i gruppi specificati:** il corrispondente sprix verrà messo a
  disposizione in Area Riservata e potrà quindi essere lanciato solo ed
  esclusivamente dagli utenti appartenenti ai gruppi selezionati
  all'interno dell'albero sottostante ("**Gruppi che hanno accesso allo
  sprix**")

![Videate\\gruppi_sprix.bmp](./assets/media/image207.png)

Il pulsante "**Salva**" presente nella parte bassa della maschera
consente, infine, di salvare lo sprix in esame.

Una volta salvato questo sprix, sarà poi possibile, accedere anche alla
maschera di definizione di tutti i parametri necessari per il corretto
funzionamento dello sprix stesso.

Per far questo è sufficiente selezionare lo sprix in oggetto all'interno
della maschera "Gestione Sprix" e cliccare poi sul pulsante **"Modifica
Parametri"** **(** **)** presente nella barra degli strumenti.

Verrà quindi visualizzata la maschera "**Gestione Parametri per lo Sprix
Estratto Conto Cliente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_estrattoconto_parametri.bmp](./assets/media/image215.png)

attraverso cui poter appunto gestire tutti i parametri necessari per il
corretto funzionamento dello sprix in esame.

**In particolare, essendo lo sprix in questione uno sprix "Standard" che
fa riferimento cioè ad una ben precisa stampa del gestionale, non sarà
ovviamente possibile eliminare i parametri presenti in elenco ne tanto
meno sarà possibile aggiungerne di nuovi.**

Sarà invece possibile variare alcune delle proprietà di questi
parametri. Selezionando uno dei parametri presenti in elenco e cliccando
sul pulsante "**Modifica Parametro Sprix**" verrà infatti visualizzata
la maschera qui di seguito riportata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_estrattoconto_parametri2.bmp](./assets/media/image216.png)

Come già visto per lo Scadenzario Cliente, anche in questo caso sarà
possibile personalizzare la Descrizione dello specifico parametro (campo
"**Descrizione**"), la sua **Tipologia** (solo per il parametro
"Cliente"), un suo eventuale valore di default (campo "**Valore di
Default**") e il fatto di rendere o meno Modificabile e/o Obbligatorio
il corrispondente campo all'interno del Form che dovrà poi essere
compilato in Area Riservata (flag "**Valore Modificabile**" e "**Valore
Obbligatorio**").

Sarà quindi possibile personalizzare la Descrizione dello specifico
parametro (campo "**Descrizione**"), la sua **Tipologia** (non per tutti
i parametri) un suo eventuale valore di default (campo "**Valore di
Default**") e il fatto di rendere o meno Modificabile e/o Obbligatorio
il corrispondente campo all'interno del Form che dovrà poi essere
compilato in Area Riservata (flag "**Valore Modificabile**" e "**Valore
Obbligatorio**").

In particolare per quel che riguarda il parametro "**Cliente**" sarà
possibile intervenire sul campo:

**Tipo Parametro:** consente di specificare la tipologia del parametro
in esame e, conseguentemente, la tipologia del controllo che verrà poi
inserito all'interno del form di compilazione dello sprix e che l'utente
dovrà utilizzare per valorizzare il parametro in oggetto.

E' possibile selezionare uno dei seguenti valori:

- **Stringa:** il parametro dovrà essere necessariamente una stringa
  alfanumerica.

> All'interno del form di compilazione dello sprix verrà quindi inserito
> un semplice campo di testo in gradi di accettare stringhe
> alfanumeriche.

- **Lista Valori:** consente di inserire all'interno del form di
  compilazione dello sprix un menu a tendina che l'utente potrà
  utilizzare per selezionare, tra le possibili opzioni di scelta
  proposte per il parametro in oggetto, quella desiderata.

- **Autocompletamento:** consente di inserire all'interno del form di
  compilazione dello sprix un campo di tipo testo che, sulla base di
  quanto digitato dall'utente, mostrerà una serie di possibili opzioni
  da selezionare per auto completare il valore immesso all'interno di
  questo stesso campo.

**Tipo Valore: visualizzato solo ed esclusivamente nel caso in cui per
il precedente campo "Tipo Parametro" sia stata selezionata l'opzione
"Lista Valori" o "Autocompletamento".** Consente di definire l'elenco
delle possibili opzioni che verranno visualizzate all'interno del menu a
tendina o come possibili opzioni di auto completamento del campo.

E' possibile selezionare uno dei seguenti valori:

- **Clienti:** le possibili opzioni di scelta da visualizzare
  all'interno del menu a tendina o come possibili opzioni di
  auto-completamento del campo, corrisponderanno all'elenco dei clienti
  che un determinato agente è effettivamente in grado di gestire
  all'interno del sito.

> Tale elenco potrà quindi comprendere, dipendentemente da come è stato
> impostato il parametro "**Gestione clienti Agente**" presente nella
> maschera di "**Configurazione Ordini**" del Wizard, i soli clienti
> effettivamente associati all'agente all'interno del gestionale
> (opzione "**L'agente gestisce i suoi clienti**") e/o anche quelli
> inseriti manualmente, attraverso le apposite funzioni del Wizard di
> Passweb, in eventuali sottogruppi del gruppo utenti cui esso
> appartiene (opzione "**L'agente gestisce i suoi clienti e quelli
> assegnati nei gruppi Passweb**").
>
> Resta ovviamente valido il concetto gerarchico grazie al quale ogni
> Agente ha sempre la possibilità di gestire anche clienti associati
> all'interno del gestionale a quelli che, nella gerarchia utenti di
> Passweb, vengono considerati come suoi Sotto Agenti.
>
> **In queste condizioni il valore del campo passato allo sprix in fase
> di esecuzione sarà il codice conto del cliente selezionato.**
>
> **ATTENZIONE!** Nel caso di auto-completamento la ricerca del cliente
> viene effettuata sulla base del suo Cognome/Ragione Sociale. **Per
> avviare la ricerca e visualizzare delle possibili opzioni, l'utente
> dovrà quindi digitare i caratteri iniziali del Cognome/Ragione Sociale
> del cliente che sta cercando.**

**Valore di Default** : consente di specificare un valore di default per
il parametro in esame. E' possibile selezionare una delle seguenti
opzioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_scadenzario_parametri4.bmp](./assets/media/image217.png)

- **Codice Conto Agente**: in questo modo in fase di presentazione del
  form dello sprix all'interno dell'Area Riservata, il parametro in
  questione verrà automaticamente valorizzato a default con il codice
  conto Mexal dell'Agente attualmente loggato

- **Codice Conto:** in questo modo in fase di presentazione del form
  dello sprix all'interno dell'Area Riservata, il parametro in questione
  verrà automaticamente valorizzato a default con il codice conto Mexal
  dell'utente attualmente considerato (indipendentemente dal fatto che
  il cliente in questione abbia associato o meno in Mexal un "Fatturare
  a")

- **Codice Conto fatturazione:** in questo modo in fase di presentazione
  del form dello sprix all'interno dell'Area Riservata, il parametro in
  questione verrà automaticamente valorizzato a default con il codice
  conto Mexal del cliente associato, all'interno del gestionale, come
  "Fatturare a" all'utente attualmente considerato. Nel caso in cui il
  cliente attualmente considerato non abbia in Mexal un "Fatturare a"
  come valore di default del parametro verrà utilizzato il suo codice
  conto.

**Lunghezza Massima Parametro:** consente di definire quella che potrà
essere la lunghezza massima del parametro in esame.

**Numero minimo di caratteri: visualizzato solo ed esclusivamente nel
caso in cui per il campo "Tipo Parametro" sia stata selezionata
l'opzione "Autocompletamento".** Consente di impostare il numero minimo
di caratteri che l'utente dovrà digitare prima di poter visualizzare le
possibili opzioni di scelta offerte per l'auto-completamento del campo.

**ATTENZIONE!** Sono accettati solamente valori maggiori o uguali a 3

**Valore Modificabile:** se selezionato il corrispondente parametro (e
il suo eventuale valore di default) potranno essere modificati dagli
utenti abilitati ad eseguire lo sprix in esame.

**Valore Obbligatorio:** se selezionato il corrispondente parametro
andrà necessariamente valorizzato prima di poter lanciare l'elaborazione
dello sprix.

**ATTENZIONE! Per i parametri diversi da "Cliente" non è mai possibile
agire sulla "Tipologia" o sulla "Lunghezza Massima" del parametro stesso
(che saranno quindi determinati in automatico dall'applicazione).**

In definitiva dunque, grazie a questa tipologia di sprix, gli utenti
appositamente abilitati avranno la possibilità di richiedere all'interno
dell'Area Riservata, la stampa dell'estratto conto di uno specifico
cliente specificando anche l'intervallo temporale in relazione al quale
richiedere questa stampa.

In Mexal, ovviamente, il numero di parametri necessari per effettuare la
stampa dell'estratto conto è superiore rispetto a quelli richiesti per
effettuare questa stessa stampa partendo dall\'Area Riservata del
proprio sito ecommerce.

**In questo senso occorre quindi considerare che per quei parametri,
indispensabili per poter effettuare all\'interno del gestionale questo
tipo di stampa, verrà considerato, nel momento in cui la stessa stampa
dovesse essere richiesta dal sito, il loro valore di default.**

Ciò significa che in riferimento, ad esempio, al parametro "**Stampa"**,
che deve necessariamente essere valorizzato all\'interno di Mexal per
poter ottenere la stampa dell'estratto conto, nel momento in cui questa
stessa stampa venisse richiesta dal sito, verrà considerato per esso il
valore R (il valore cioè assegnato a default da Mexal stesso a questo
parametro).

**In questo senso quindi le stampe del Estratto Conto richiamabili
dall\'Area Riservata del proprio sito web potranno essere solamente
stampe in formato ridotto.**

Per maggiori informazioni relativamente alle modalità di esecuzione di
questi sprix, si veda anche la sezione *"Business to Business Area
Riservata"* di questo manuale.

