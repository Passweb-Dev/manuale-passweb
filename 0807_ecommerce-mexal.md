# ECOMMERCE MEXAL



Nel caso di siti Ecommerce collegati a Mexal **l\'inserimento, la
variazione, la cancellazione e, in generale, la gestione degli
abbinamenti avviene direttamente all'interno del gestionale** operando
nell\'anagrafica dell\'articolo a cui si desidera associare gli Abbinati
stessi.

In anagrafica articolo è infatti presente il pulsante **"Altri Dati
Anagrafici (F5)"** che consente di accedere ad ulteriori dati anagrafici
relativi all'articolo considerato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mexal_abbinati_1.bmp](./assets/media/image448.png)

All'interno della maschera "**Altri Dati Anagrafici**" sono poi presenti
due ulteriori pulsanti, **Alias e Abbinati**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mexal_abbinati_2.bmp](./assets/media/image449.png)

Selezionato Abbinati, se nessun codice è presente comparirà il seguente
messaggio:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_abbinati_4.bmp](./assets/media/image450.png)

dove sono attivi i seguenti comandi:

- **OK \[Invio\]** = abbandona la finestra e torna sul codice
  alternativo dell\'anagrafica articoli.

- **Inserisci \[Ins\]** = entra nell\'anagrafica codici Abbinati per
  permetterne l\'inserimento.

Premuto **Inserisci \[Ins\]** viene aperta la seguente finestra:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_abbinati_5.bmp](./assets/media/image451.png)

dove vengono gestiti i seguenti campi:

- **Codice --** Codice articolo da abbinare all\'articolo attualmente in
  uso. Sono attivi i comandi di ricerca/immissione dell\'anagrafica
  articoli. E\' possibile utilizzare il carattere **\"?\"** con il
  significato di qualsiasi carattere nella posizione. Quindi si possono
  agganciare come articoli abbinati più codici senza doverli selezionare
  uno per volta. Immesso un codice con punti interrogativi compare la
  descrizione **\"articolo variabile\"**.

> Nella finestra di ricerca articoli, quando viene richiesto di
> visualizzare i codici abbinati, verranno elencati codici abbinati
> considerando che il carattere ? assume il significato di qualsiasi
> carattere nella posizione.

- **Categoria** -- Gli articoli Abbinati possono essere generici oppure
  possono essere suddivisi per categoria di abbinamento. Sono attivi i
  pulsanti **"\[F2\]** **Elenco**" per visualizzare tutte le categorie
  presenti e **"\[F4\] Anagrafica Categoria"** per crearne di nuove
  oppure per variare quelle esistenti. Premendo il pulsante \[F4\] verrà
  quindi visualizzata la finestra **\"Anagrafica categorie\"** nella
  quale specificare il **codice** (4 caratteri liberi) e la
  **descrizione** (32 caratteri liberi) della categoria di abbinamento.

> **NOTA BENE:** il testo inserito all'interno del campo "Descrizione"
> verrà utilizzato a default all'interno del sito web come etichetta
> identificativa della relativa categoria di abbinati. Tale valore potrà
> comunque essere personalizzato nel back -- end di Passweb dalla
> relativa maschera di gestione degli abbinati (sezione "Catalogo --
> Gestione Articoli -- Gestione Abbinati").

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_abbinati_7.bmp](./assets/media/image452.png)

> Il pulsante **"\[F10\] OK"** memorizza la categoria fino ad un massimo
> di 50, mentre **"\[ShF3\] Elimina"** la cancella.

**NOTA BENE:** per poter visualizzare correttamente un articolo abbinato
all'interno del sito web è obbligatorio associarlo ad una categoria
abbinati. **Gli articoli abbinati non associati ad alcuna categoria non
verranno visualizzati all'interno del componente "Articoli Abbinati"**
(vedi anche la sezione "Live Editing -- Lista Componenti Ecommerce --
Componente Articoli Abbinati" all'interno di questo manuale).

All'interno della maschera "Anagrafica Codici Abbinati" sono gestiti
inoltre i seguenti campi:

- **Articolo** -- Viene riportato il codice articolo in uso al quale
  saranno abbinati gli articoli specificati nel campo \"Codice\"
  precedentemente descritto.

- **Nota** -- (Nota 1 e Nota 2). Descrizioni non obbligatorie da 52
  caratteri per l\'inserimento di eventuali informazioni sul codice
  Abbinato.

- **Data Creazione** -- Gestita automaticamente, rappresenta la data
  della creazione dell\'anagrafica Abbinato.

- **Data Aggiornamento** -- Gestita automaticamente, rappresenta la data
  dell\'ultima conferma dell\'Abbinato.

Premendo **"Annulla \[Esc\]"** si abbandona la codifica (viene richiesto
conferma dell\'uscita); completata l\'immissione dei dati il comando
**"OK \[F10\]"** conferma l\'abbinamento.

Se i codici Abbinati sono suddivisi per categoria, saranno visualizzati
solo quelli della categoria di appartenenza che viene indicata nel
titolo della finestra.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_abbinati_8.bmp](./assets/media/image453.png)

Nel caso in cui per uno stesso articolo siano presenti più categorie di
abbinati, prima della finestra di selezione degli articoli abbinati
compare una selezione per categoria.

E' possibile, infine, visualizzare i vari abbinamenti anche dalla
maschera di Ricerca Articoli.

Una volta individuato l'articolo desiderato è attivo il pulsante
**"\[F8\] Abbinati"** che permette di visualizzare immediatamente senza
il bisogno di accedere all'anagrafica dell'articolo quelli che sono i
suoi abbinati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_abbinati_10.bmp](./assets/media/image454.png)

Selezionando Abbinati, se presenti dei codici abbinati agganciati
all\'articolo su cui è posizionata la barra di scorrimento, si apre la
finestra di selezione dei codici eventualmente suddivisi per categoria
di abbinamento.

**NOTA BENE:** per maggiori informazioni relativamente alla gestione in
Mexal degli Abbinati si rimanda all'apposito manuale.

La sezione **"Abbinati",** accessibile all'interno del Wizard dalla voce
di menu ***"Catalogo -- Gestione Articoli"**,* consente di visualizzare
le diverse categorie di abbinati codificate all'interno del gestionale
ed esportate sul sito, gli articoli ad esse associati con i relativi
abbinati e, se necessario, consente anche di personalizzare, in tutte le
lingue gestite le descrizioni di ciascuna di queste categorie.

All'interno di questa pagina verrà infatti visualizzata la maschera
**"Gestione Articoli Abbinati"**, suddivisa in due distinte sezioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_gestione_abbinati.bmp](./assets/media/image455.png)

- Nella parte sinistra della maschera sono elencate tutte le Categorie
  di Abbinati codificate in Mexal ed esportate all'interno del sito.

> Il pulsante **Modifica** (
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image43.png) ) presente nella corrispondente barra
> degli strumenti, consente di modificare e personalizzare la
> descrizione della Categoria Abbinati attualmente selezionata in
> elenco.
>
> Cliccando su questo pulsante verrà infatti visualizzata la maschera
> **Modifica Categoria**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_categoria.bmp](./assets/media/image456.png)

> all'interno della quale poter indicare, in ciascuna delle lingue
> gestite all'interno del sito, l'etichetta utilizzata per identificare,
> all'interno del componente "Abbinati", la categoria in esame.
>
> **NOTA BENE:** il campo "Descrizione" è valorizzato a default con la
> descrizione inserita in Mexal per la relativa Categoria di Abbinati.

- Nella parte destra della maschera vengono invece visualizzati tutti
  gli articoli associati alla Categoria Abbinati attualmente selezionata
  (nella parte sinistra della maschera)

> Nello specifico, in corrispondenza della colonna "**Articolo**" viene
> indicato il codice dell'articolo associato alla Categoria Abbinati
> selezionata in elenco, mentre in corrispondenza della colonna
> "**Codice**" viene indicato il codice dell'articolo ad esso abbinato.
>
> Il pannello di ricerca presente nella parte alta di questa sezione
> consente di ricercare un particolare articolo e/o abbinato indicandone
> nei rispettivi campi codice o descrizione.
>
> Il pulsante **Esporta** (
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image136.png) ) presente nella contestuale barra
> degli strumenti, consente invece di esportare l'elenco degli articoli
> associati a ciascuna delle Categorie Abbinati gestite, in un file csv
> in cui verranno inserite, rispettivamente, le seguenti informazioni:
>
> **codice_articolo; codice_abbinato; codice_categoria_abbinato**
>
> Cliccando su questo pulsante verrà visualizzata, all'interno della
> maschera "Gestione Articoli Abbinati" un' ulteriore sezione
> "**Esportazione Abbinati**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_abbinati.bmp](./assets/media/image457.png)

> all'interno della quale poter indicare, selezionandolo dall'apposito
> menu a tendina, il carattere che dovrà essere utilizzato all'interno
> del file di esportazione come separatore per i vari campi.

**ATTENZIONE!** Si ricorda che per siti Ecommerce collegati a Mexal la
gestione delle Categorie Abbinati (creazione ed eliminazione) e degli
abbinamenti tra i vari articoli è demandata interamente al gestionale

