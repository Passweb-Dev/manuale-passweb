# SPRIX PERSONALI



Come precedentemente evidenziato all'interno della sezione "Gestione
Sprix" è possibile definire anche degli sprix "personali" che fanno
riferimento cioè a specifici eseguibili creati direttamente dall'utente
all'interno di Mexal.

Tali eseguibili potranno poi essere richiamati mediante Sprix Remoto
oppure mediante Web Api e, a seconda della specifica interfaccia
utilizzata per richiamarli, dovranno essere configurati e strutturati in
un certo modo.

**ATTENZIONE!** in ogni caso il risultato di queste elaborazioni verrà
gestito sempre mediante il salvataggio, all'interno del sito, di un
apposito file.

Per codificare uno sprix di questo tipo è sufficiente cliccare sul
pulsante sul pulsante **"Nuovo"**
**(**![Videate\\pulsante_nuovo.bmp](./assets/media/image218.png) **)** presente nella barra degli
strumenti della maschera "Gestione Sprix", e impostare poi il parametro
"**Tipologia**" sul valore "**Altro**".

![Videate\\sprix_personali.bmp](./assets/media/image219.png)

In questo modo verranno visualizzati, all'interno della maschera "Nuovo
Sprix", i parametri di configurazione necessari per mappare in maniera
corretta il corrispondente eseguibile Mexal.

Nello specifico sarà quindi necessario impostare un valore anche per i
seguenti parametri:

**Interfaccia**: consente di definire l'interfaccia da utilizzare per
richiamare il corrispondente eseguibile all'interno del gestionale. E'
possibile selezionare una delle seguenti opzioni:

- **Sprix Remoto**

> In questo caso per fare in modo che gli sprix creati all'interno del
> gestionale possano essere effettivamente lanciati dall' Area Riservata
> del sito, mostrando poi all'utente che li ha eseguiti il risultato
> della loro elaborazione, dovranno essere soddisfatti alcuni requisiti
> di fondamentale importanza
>
> **In particolare ogni eseguibile sprix di questo tipo dovrà gestire i
> risultati delle elaborazioni tramite le istruzioni PUTREM_DATI e
> PUTREM_ERR** (per maggiori informazioni si rimanda al manuale sprix
> relativamente alla funzione **SPXREMOTO\$**).

- **Web Api**

> In questo caso sarà possibile lanciare dall'Area Riservata appositi
> "Collage Server Remoti" definiti all'interno del gestionale.
>
> Per poter far questo sarà necessario, per prima cosa, verificare di
> aver correttamente abilitato il Sito all'utilizzo delle Web Api (per
> maggiori informazioni in merito si veda anche quanto indicato
> all'interno del capitolo "*Configurazione -- Mexal Configurazione
> Gestionale -- Web Api Mexal*" di questo manuale)
>
> Inoltre sarà anche necessario:

- strutturare il Collage Server Remoto in maniera tale che restituisca
  come valore di ritorno del json, un campo di nome "file" in cui dovrà
  essere inserita la stringa che verrà poi salvata, sul sito, come file
  e che sarà, di fatto, il risultato dell'elaborazione visualizzato
  dall'utente (l'estensione di questo file sarà esattamente quella
  indicata in fase di configurazione dello sprix stesso)

> **ATTENZIONE!** nel momento in cui nel json ritornato dal Collage
> Server Remoto non dovesse essere presente il campo di nome file, il
> file salvato sul sito come risultato dell'elaborazione gestionale
> conterrà l'intero json (indentato) restituito dalla Web Api

- impostare i campi del form utilizzato per gestire i parametri di
  ingresso al Collage Server Remoto in maniera tale che ciascuno di essi
  abbia il campo "Id/Name" valorizzato esattamente con il nome del
  relativo parametro di ingresso

**Descrizione:** consente di associare allo sprix in esame una specifica
descrizione, in maniera tale da poterlo poi identificare rispetto ad
altri eventuali sprix presenti in elenco

**Nome File Sprix su server:** nome assegnato, sul server Mexal, allo
sprix che dovrà essere eseguito lato gestionale.

**NOTA BENE**: il nome indicato all'interno di questo campo deve
corrispondere esattamente con il nome di uno sprix presente
nell'installazione e nell'azienda Mexal collegata al sito E-commerce.

**Carattere Separatore di Parametri --** solo per "Interfaccia = Sprix
Remoto"

Consente di indicare il carattere utilizzato, lato gestionale, per
separare eventuali parametri passati allo sprix.

Tale parametro è di fondamentale importanza, occorre infatti considerare
che **eventuali parametri necessari per la corretta esecuzione, lato
Mexal, dello sprix verranno passati al gestionale stesso come un'unica
stringa (di lunghezza massima pari a 255 caratteri)**. Lato sprix sarà
quindi necessario suddividere questa stessa stringa sulla base del
carattere utilizzato come separatore, in modo tale da poter estrarre da
essa i singoli parametri richiesti dallo sprix.

**NOTA BENE**: è di fondamentale importanza gestire all'interno dello
sprix tutta la logica necessaria per l'estrazione dei singoli parametri
a partire dall'unica stringa in arrivo dal sito web.

A default verrà proposto ed utilizzato come carattere separatore il
carattere "&".

**Etichetta Collage** -- **solo per "Interfaccia = Web Api"**

Consente di indicare l'etichetta assegnata all'interno del gestionale al
Collage Server Remoto che verrà poi richiamato da Area Riservata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_web_api_etichetta_collage.bmp](./assets/media/image220.png)

**Codice App** -- **solo per "Interfaccia = Web Api"**

Consente di indicare il codice dell'App gestionale corrispondente al
Collage Server Remoto che verrà poi richiamato da Area Riservata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_web_api_codice_app.bmp](./assets/media/image221.png)

**Estensione file di ritorno:** estensione del file ritornato come
risultato dallo sprix

**ATTENZIONE!** l'estensione indicata all'interno di questo campo sarà
poi quella assegnata al file salvato sul sito, file questo che conterrà
il risultato dell'elaborazione effettuata lato gestionale dal
corrispondente eseguibile

Il valore impostato in corrispondenza di questo parametro è quindi
indispensabile per una corretta visualizzazione del risultato.

**Visibile da:** consente invece di definire i gruppi di utenti cui
rendere disponibile questo stesso sprix all'interno dell'Area Riservata
del sito. E' possibile selezionare una delle seguenti opzioni:

- **Tutti:** il corrispondente sprix verrà messo a disposizione e potrà
  quindi essere lanciato da tutti gli utenti del sito abilitati ad
  accedere in Area Riservata

- **Solo i gruppi specificati:** il corrispondente sprix verrà messo a
  disposizione in Area Riservata e potrà quindi essere lanciato solo ed
  esclusivamente dagli utenti appartenenti ai gruppi selezionati
  all'interno dell'albero sottostante ("**Gruppi che hanno accesso allo
  sprix**")

![Videate\\gruppi_sprix.bmp](./assets/media/image207.png)

Una volta definita l'interfaccia da utilizzare per richiamare un
determinato eseguibile presente sul gestionale, e impostati anche tutti
i parametri indispensabili per poter mappare in maniera corretta questo
stesso eseguibile, il passo successivo sarà quello di definire il form
che l'utente dovrà poi utilizzare per impostare i parametri di ingresso
necessari per il corretto funzionamento dello sprix.

In questo senso sarà quindi necessario selezionare lo sprix desiderato,
tra quelli presenti in elenco, e cliccare poi sul pulsante **"Modifica
Parametri"** **(** ) in maniera tale da accedere alla maschera
"**Gestione Parametri per lo Sprix 'Nome Sprix'** "

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_sprix_remoto.bmp](./assets/media/image222.png)

Per aggiungere un nuovo parametro, e conseguentemente un nuovo campo del
form, sarà quindi sufficiente cliccare sul pulsante **"Nuovo Parametro
Sprix"** **(**
![Videate\\pulsante_nuovo_parametro_sprix.bmp](./assets/media/image223.png) **)**.

In questo modo verrà infatti visualizzata la maschera "**Nuovo Parametro
Sprix**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_parametro_sprix.bmp](./assets/media/image224.png)

all'interno della quale poter impostare un valore per i seguenti campi:

**Descrizione:** consente di specificare un'etichetta identificativa del
parametro che si sta codificando e, quindi, del corrispondente campo del
form utilizzato per richiamare lo sprix

**Id/Name**: consente di assegnare un valore alle proprietà Id/Name del
relativo campo del form utilizzato per richiamare lo sprix

**ATTENZIONE!** **Tale campo è obbligatorio e di fondamentale importanza
nel momento in cui si sia deciso di utilizzare le Web Api come
interfaccia di esecuzione del corrispondente sprix.**

In questo caso infatti, **il valore inserito in corrispondenza di questo
campo sarà poi quello utilizzato nel body della richiesta Web Api
inviata al gestionale e dovrà quindi coincidere esattamente con il nome
del relativo parametro effettivamente utilizzato dallo sprix in
questione**

**Tipo Parametro:** consente di specificare la tipologia del parametro
in esame e, conseguentemente, la tipologia del controllo che verrà poi
inserito all'interno del form di compilazione dello sprix e che l'utente
dovrà utilizzare per valorizzare il parametro in oggetto.

E' possibile selezionare uno dei seguenti valori:

- **Intero:** il parametro dovrà necessariamente essere un numero intero
  (positivo o negativo).

> All'interno del form di compilazione dello sprix verrà inserito un
> semplice campo di testo in grado di accettare soltanto numeri interi.

- **Stringa:** il parametro dovrà essere necessariamente una stringa
  alfanumerica.

> All'interno del form di compilazione dello sprix verrà quindi inserito
> un semplice campo di testo in gradi di accettare stringhe
> alfanumeriche.

- **Data:** il parametro dovrà essere necessariamente una data.

> All'interno del form di compilazione dello sprix verrà quindi
> visualizzato un calendario attraverso cui l'utente potrà selezionare
> la data desiderata.

![Videate\\sprix_data.bmp](./assets/media/image225.png)

- **Lista Valori:** consente di inserire all'interno del form di
  compilazione dello sprix un menu a tendina che l'utente potrà
  utilizzare per selezionare, tra le possibili opzioni di scelta
  proposte per il parametro in oggetto, quella desiderata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_lista_valori.bmp](./assets/media/image226.png)

- **Autocompletamento:** consente di inserire all'interno del form di
  compilazione dello sprix un campo di tipo testo che, sulla base di
  quanto digitato dall'utente, mostrerà una serie di possibili opzioni
  da selezionare per auto completare il valore immesso all'interno di
  questo stesso campo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sprix_autocompletamento.bmp](./assets/media/image227.png)

**Tipo Valore -- solo per "Tipo Parametro = Lista Valori" o " Tipo
Parametro = Autocompletamento".**

Consente di definire l'elenco delle possibili opzioni che verranno
visualizzate all'interno del menu a tendina o come possibili opzioni di
auto completamento del campo. E' possibile selezionare uno dei seguenti
valori:

- **Custom:** in questo caso le possibili opzioni di scelta da
  visualizzare all'interno del menu a tendina o come possibili opzioni
  di auto-completamento del campo, dovranno essere codificate in maniera
  manuale.

> Selezionando questo valore (e, nel caso di parametri di tipo "Lista
> Valori" effettuando anche un primo salvataggio del parametro) verrà
> infatti visualizzata la sezione **"Gestione Opzioni"** attraverso cui
> poter definire, appunto, tutti i valori ammessi per lo specifico
> parametro.

![Videate\\sprix_parametri_lista_valori.bmp](./assets/media/image228.png)

> Per inserire una nuova opzione di scelta in elenco è sufficiente
> cliccare sul pulsante raffigurante un piccolo segno + e,
> successivamente, inserire nel form **"Nuova Opzione"** l'etichetta
> identificativa del nuovo elemento (**Etichetta del campo**) il valore
> (**Valore del Campo**) che verrà poi passato allo sprix in fase di
> esecuzione, e se tale elemento dovrà o meno essere selezionato e
> visualizzato a default (flag "**Selezionato**" valido solo per
> parametri di tipo "Lista Valori").
>
> **ATTENZIONE!** Nel caso di auto-completamento la ricerca delle
> possibili opzioni proposte sulla base di quanto attualmente digitato
> dall'utente è effettuata prendendo in considerazione le etichette
> associate alle varie opzioni di scelta. **Per avviare la ricerca e
> visualizzare delle possibili opzioni l'utente dovrà quindi digitare i
> caratteri iniziali di queste etichette.** Una volta selezionato uno
> degli elementi proposti l'etichetta verrà automaticamente sostituita
> con il corrispondente valore passato poi allo sprix in fase di
> esecuzione.

- **Clienti:** in questo caso le possibili opzioni di scelta da
  visualizzare all'interno del menu a tendina o come possibili opzioni
  di auto-completamento del campo, corrisponderanno all'elenco dei
  clienti che un determinato agente è effettivamente in grado di gestire
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

- **Sub-Agenti:** in questo caso le possibili opzioni di scelta da
  visualizzare all'interno del menu a tendina o come possibili opzioni
  di auto-completamento del campo, corrisponderanno all'elenco di agenti
  appartenenti a gruppi figli del gruppo cui appartiene l'agente
  attualmente loggato sul sito (per maggiori informazioni relativamente
  alla gerarchia agenti si veda anche la sezione *"Utenti -- Gruppi
  Utenti Sito -- Creazione di una gerarchia agenti"* di questo manuale).

> **In queste condizioni il valore del campo passato allo sprix in fase
> di esecuzione sarà il codice conto dell'agente selezionato.**
>
> **ATTENZIONE!** Nel caso di auto-completamento la ricerca del sotto
> agente viene effettuata sulla base del suo Cognome. **Per avviare la
> ricerca e visualizzare delle possibili opzioni, l'utente dovrà quindi
> digitare i caratteri iniziali del Cognome dell'agente che sta
> cercando**

- **Articoli:** in questo caso le possibili opzioni di scelta da
  visualizzare all'interno del menu a tendina o come possibili opzioni
  di auto-completamento del campo, corrisponderanno all'elenco di
  articoli pubblicati sul sito e che il cliente/agente attualmente
  loggato è effettivamente in grado di gestire.

> **In queste condizioni il valore del campo passato allo sprix in fase
> di esecuzione sarà il codice dell'articolo selezionato**
>
> **ATTENZIONE!** Nel caso di auto-completamento la ricerca di uno
> specifico articolo viene effettuata sulla base del suo codice e/o
> della sua descrizione Mexal (corrispondente a quanto pubblicato sul
> sito in corrispondenza del componente "Titolo"). **Per avviare la
> ricerca e visualizzare delle possibili opzioni, l'utente dovrà quindi
> digitare i caratteri iniziali del codice o della descrizione Mexal
> dell'articolo che sta cercando.**

- **Categorie merceologiche:** in questo caso le possibili opzioni di
  scelta da visualizzare all'interno del menu a tendina o come possibili
  opzioni di auto-completamento del campo, corrisponderanno all'elenco
  delle categorie merceologiche cui appartengono gli articoli pubblicati
  sul sito e che il cliente/agente è effettivamente in grado di gestire.

> **In queste condizioni il valore del campo passato allo sprix in fase
> di esecuzione sarà il codice della categoria merceologica
> selezionata.**
>
> **ATTENZIONE!:** Nel caso di auto-completamento la ricerca di una
> specifica categoria merceologica viene effettuata per sottostringa
> considerando il percorso completo della categoria merceologia, dal
> padre al figlio. **Per avviare la ricerca e visualizzare delle
> possibili opzioni, è quindi sufficiente che l'utente digiti alcuni dei
> caratteri presenti nella descrizione di una delle categorie
> merceologiche presenti nel percorso completo della specifica categoria
> che sta effettivamente cercando**

- **Categorie Statistiche:** in questo caso le possibili opzioni di
  scelta da visualizzare all'interno del menu a tendina o come possibili
  opzioni di auto-completamento del campo, corrisponderanno all'elenco
  delle categorie statistiche cui appartengono gli articoli pubblicati
  sul sito e che il cliente/agente è effettivamente in grado di gestire.

> **In queste condizioni il valore del campo passato allo sprix in fase
> di esecuzione sarà il codice della categoria statistica selezionata**.
>
> **ATTENZIONE!:** Nel caso di auto-completamento la ricerca di una
> specifica categoria merceologica viene effettuata sulla base della sua
> descrizione Mexal. **Per avviare la ricerca e visualizzare delle
> possibili opzioni, l'utente dovrà quindi digitare i caratteri iniziali
> della descrizione Mexal relativa alla categoria merceologica che sta
> cercando**

**Valore di Default:** consente di specificare un valore di default per
il parametro in esame. Per i parametri di tipo Stringa è possibile
utilizzare anche dei valori automatici.

In particolare è possibile settare il "Valore di default" di un
parametro di tipo Stringa come:

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

Per maggiori informazioni relativamente alle modalità di esecuzione
degli eseguibili sprix codificati da questa sezione del Wizard, si veda
anche la sezione *"Business to Business Area Riservata"* di questo
manuale.

I restanti pulsanti presenti nella barra degli strumenti della maschera
"**Gestione Parametri per lo Sprix 'Nome Sprix'** " consentono
rispettivamente di:

![Videate\\gestione_parametri_sprix_remoto.bmp](./assets/media/image229.png)

**Elimina Parametro Sprix** **(**
![Videate\\pulsante_elimina_parametro_sprix.bmp](./assets/media/image230.png) **)**: consente di eliminare il
parametro attualmente selezionato in elenco

**Giù e Su** **(**
![Videate\\pulsante_su_giu.bmp](./assets/media/image231.png) **)**: consentono definire l'esatta posizione in cui
dovrà comparire il parametro attualmente selezionato all'interno del
form che andrà poi compilato per la corretta esecuzione dello sprix in
oggetto.

