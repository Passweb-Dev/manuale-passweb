# ATTRIBUTI PASSWEB



Come precedentemente evidenziato gli **Attributi Passweb** altro non
sono se non **Attributi Articolo definiti direttamente in Passweb,** la
cui creazione e gestione è quindi demandata interamente a Passweb
stesso.

Tali attributi potranno quindi essere gestiti tanto su siti Ecommerce
collegati a Mexal, quanto su siti Ecommerce collegati ad un qualsiasi
gestionale Ho.Re.Ca.

**ATTENZIONE!** **Ogni attributo di questo tipo dovrà essere definito e
valorizzato direttamente all'interno del Wizard del proprio sito
e-commerce.**

Per creare un nuovo Attributo Articolo di tipo Passweb è necessario, per
prima cosa, portarsi all'interno della pagina **"Attributi per il
Catalogo"** accessibile dalla voce di menu ***"Catalogo -- Attributi
Articoli -- Attributi"*** del Wizard e cliccare, successivamente, sul
pulsante **"Nuovo"**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo.bmp](./assets/media/image88.png) ) presente nella barra degli strumenti.
In questo modo verrà visualizzata la maschera **"Attributi"** attraverso
cui poter definire le caratteristiche dell'Attributo che si sta
realizzando.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\creazione_attributo_passweb.bmp](./assets/media/image89.png)

Nel caso in esame sarà poi necessario indicare un valore per i seguenti
parametri:

**Nome Attributo:** consente di definire il nome dell'Attributo Articolo
che si sta realizzando.

**Riportabile sul documento:** permette di indicare se l'Attributo
Passweb che si sta realizzando dovrà essere considerato o meno come un
Attributo Riportabile in maniera tale da poterlo eventualmente
utilizzare anche all'interno dei vari documenti presenti sul sito.

In particolare nel caso in caso in cui il parametro in questione sia
stato:

- **Deselezionato**: il corrispondente Attributo Articolo potrà essere
  utilizzato all'interno del sito, ad esempio nelle varie celle del
  catalogo piuttosto che nella Scheda Prodotto, mediante il componente
  "Dati Articolo" ma non potrà in alcun modo essere utilizzato e
  visualizzato nel dettaglio dei documenti in corrispondenza delle
  relative righe articolo.

- **Selezionato:** il corrispondente Attributo Articolo oltre a poter
  essere visualizzato sul sito mediante il componente "Dati Articolo",
  come nel caso precedente, alla conferma dell'ordine verrà anche
  copiato nella relativa riga del documento e, **se valorizzato**, sarà
  quindi visualizzabile in corrispondenza di questa stessa riga nel
  dettaglio del Documento stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_articoli_rip_documento.bmp](./assets/media/image90.png)

> **ATTENZIONE! Trattandosi di un Attributo di tipo Passweb, ovviamente,
> quest'informazione non potrà mai essere trasferita sul gestionale e
> potrà quindi essere visualizzata solo ed esclusivamente all'interno
> del sito**

Inoltre, come già per gli Attributi Riportabili Mexal, anche in questo
caso per poter visualizzare l'Attributo nel dettaglio del documento sul
front end del sito, sarà necessario utilizzare il componente "Checkout
Custom" ed inserire al suo interno un componente "Dati Articolo" mappato
con l'Attributo in questione.

Per la stessa ragione, nel momento in cui fosse necessario modificare il
valore di un Attributo di questo tipo per uno specifico documento
occorrerà operare, per forza di cose, direttamente da Passweb.

Nello specifico, sarà necessario portarsi per prima cosa all'interno
della sezione *"Ordini -- Gestione Ordini"* del Wizard e cliccare sul
pulsante "**Attiva Modifica Attributi**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_modifiche_attributo.bmp](./assets/media/image105.png) ) in maniera tale da attivare la
visualizzazione del dettaglio di un documento con la possibilità di
modificare eventuali Attributi Passweb collegati al documento stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_attributi_lista_ordini.bmp](./assets/media/image106.png)

Una volta attivata la modalità "Modifica Attributi" sarà poi necessario
selezionare tra quelli presenti in elenco lo specifico documento in cui
effettuare l'operazione e cliccare sul pulsante "**Visualizza Ordine**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_visualizza_ordine.bmp](./assets/media/image107.png) )

In questo modo si avrà quindi accesso in modifica al dettaglio del
Documento selezionato.

Nello specifico sarà possibile modificare solo ed esclusivamente il
valore di tutti gli Attributi Passweb, siano essi di Testata (Attributi
dell'Ordine) o di Riga (Attributi Articolo Riportabili) presenti
all'interno del documento stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_attributi_lista_ordini_3.bmp](./assets/media/image108.png)

Anche in questo caso **eventuali variazioni apportate ai valori di
questi Attributi nel dettaglio di uno specifico ordine saranno valide
solo ed esclusivamente per quello stesso specifico documento.**

**Sorgente Dati (solo per siti Ecommerce collegati a Mexal):** consente
di specificare la tipologia di Attributo che si intende realizzare.
**Nel caso in esame questo campo dovrà essere impostato, ovviamente, sul
valore "Passweb"** (come evidenziato nella figura di seguito riportata)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_attributo_passweb.bmp](./assets/media/image109.png)

**ATTENZIONE!** **Per siti Ecommerce collegati ad un gestionale
Ho.Re.Ca. essendo la tipologia Passweb l'unica tipologia di Attributo
Articolo gestita, il campo "Sorgente Dati" non sarà ovviamente
disponibile.**

Una volta impostata la tipologia dell'attributo occorrerà poi settare
tutta una serie di altri parametri caratteristici della tipologia
stessa.

Nello specifico sarà quindi necessario impostare un valore anche per i
seguenti campi

**Etichetta del campo:** consente di specificare, in tutte le lingue
gestite all'interno del sito, l'etichetta identificativa dell'attributo
che si sta realizzando. Tale etichetta verrà poi visualizzata, in
corrispondenza dell'attributo stesso all'interno del componente **"Set
Attributi"**

**Tipo di Campo:** consente di specificare **il tipo di controllo di
input** **che verrà poi utilizzato, all'interno dell'anagrafica Passweb
dell'articolo**, per valorizzare il corrispondente attributo. E'
possibile selezionare, dal relativo menu a tendina, uno dei seguenti
valori:

- **Testo:** il corrispondente attributo potrà poi essere valorizzato
  utilizzando un normale campo di input

- **Numero**: anche in questo caso il corrispondente attributo potrà
  essere valorizzato utilizzando un normale campo di input.

> **ATTENZIONE!** Ovviamente a differenza degli attributi di tipo testo
> in questo caso il campo di input accetterà solo ed esclusivamente
> valori decimali.

- **Testo HTML:** il corrispondente attributo potrà poi essere
  valorizzato utilizzando un editor HTML esteso mediante il quale poter
  associare al testo una specifica formattazione, poter inserire
  tabelle, immagini ecc ...

- **Data:** il corrispondente attributo dovrà essere, ovviamente, una
  "Data" e potrà essere valorizzato selezionando la relativa data da un
  apposito calendario

- **Immagine:** il corrispondente attributo dovrà essere un' "Immagine"
  e potrà essere valorizzato, nelle varie anagrafiche Passweb,
  selezionando attraverso un apposito controllo, una qualsiasi delle
  immagini attualmente presenti in "Gestione Risorse". In alternativa
  sarà sempre possibile decidere di caricare una nuova immagine in fase
  di valorizzazione dell'attributo stesso.

- **Drop Down:** il corrispondente attributo potrà essere valorizzato
  selezionando uno dei valori presenti all'interno di un apposito menu a
  tendina.

> In queste condizioni non sarà quindi possibile inserire un valore
> diverso da quelli proposti.
>
> In ogni caso l'elenco dei valori che verranno proposti nel momento in
> cui si andrà a valorizzare, articolo per articolo, questo attributo,
> può essere definito direttamente in fase di creazione e/o di modifica
> dell'attributo stesso.
>
> Al salvataggio dell'Attributo verrà infatti visualizzata la sezione
> **"Gestione Opzioni"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributo_nuova_opzione.bmp](./assets/media/image110.png)

> all'interno della quale poter definire l'elenco dei valori che
> l'attributo in questione potrà assumere.
>
> Per inserire un nuovo valore è sufficiente cliccare sul pulsante
> raffigurante un piccolo +
> (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image99.png) ) presente nella barra degli
> strumenti.
>
> In questo modo verrà infatti visualizzata la maschera "**Nuova
> Opzione**", all'interno della quale poter inserire (parametro
> "**Etichetta del campo**") il valore desiderato per ognuna delle
> lingue gestite all'interno del sito.
>
> Il check "**Selezionato**" consente invece di stabilire se il valore
> attualmente considerato dovrà rappresentare o meno il valore di
> default per l'attributo in esame. Considerando che il controllo di
> tipo Drop Down permetterà, in fase di valorizzazione dell'attributo,
> di selezionare uno solo dei valori disponibili, uno soltanto dei
> valori inseriti in griglia potrà essere considerato come valore di
> default del controllo (evidenziato in grassetto).

- **Selezione Multipla:** il corrispondente attributo potrà essere
  valorizzato selezionando **uno o più valori** tra quelli presenti
  all'interno di un'apposita lista.

> Anche in questo caso al salvataggio dell'Attributo verrà visualizzata
> la sezione **"Gestione Opzioni"** all'interno della quale poter
> definire l'elenco dei valori che l'attributo in questione potrà poi
> assumere.
>
> Considerando che, a differenza del caso precedente, il controllo di
> tipo "Selezione Multipla" permetterà, in fase di valorizzazione
> dell'attributo, di selezionare per esso uno o più valori tra quelli
> presenti in elenco, in questo caso sarà possibile definire due o più
> valori che dovranno poi essere considerati come valori di default l'
> attributo stesso (e inseriti quindi, a default, nel box di destra).

**NOTA BENE:** nel caso di controllo "Selezione Multipla", a livello di
valore dell'attributo, i valori selezionati verranno poi tradotti in
un'unica stringa contenente le etichette degli elementi indicati
separate da una virgola.

**NOTA BENE**: tenendo conto dell'osservazione precedente, è quindi
possibile **realizzare anche un Attributo Articolo Mexal in grado di
accogliere per uno stesso articolo due o più valori.** Per far questo è
sufficiente inserire all'interno del corrispondente campo Mexal,
opportunamente separati da una virgola, tutti i valori che l'attributo
in questione può assumere per lo specifico articolo

**Valore di default:** consente di specificare un valore di default che
potrà essere associato al relativo attributo lanciando la relativa
procedura presente all'interno della sezione "Utilità" (per maggiori
informazioni in merito si vedano i successivi capitoli di questo
manuale) .

**ATTENZIONE!** Per i controlli di tipo Drop Down e Selezione Multipla
la definizione del valore di default avverrà all'interno della sezione
"Gestione Opzioni" secondo quanto precedentemente indicato.

**Campo Univoco (solo per controlli di tipo "Testo" e "Data"):**
selezionando questo parametro, verrà associata al corrispondente
attributo, la proprietà di univocità. Questo significa dunque che in
fase di valorizzazione dell'attributo stesso verrà effettuato un
controllo di univocità in base al quale non sarà possibile specificare
per articoli differenti lo stesso valore.

**Campo Obbligatorio:** selezionando questo parametro, verrà associata
al corrispondente attributo, la proprietà di obbligatorietà. Questo
significa dunque che in fase compilazione dell'anagrafica
articolo/servizio Passweb, il corrispondente attributo dovrà essere
obbligatoriamente valorizzato.

**NOTA BENE**:al salvataggio di un'anagrafica articolo/servizio Passweb,
verranno effettuati i controlli di univocità e di obbligatorietà sugli
attributi presenti all'interno di questa stessa anagrafica. Verranno
quindi visualizzati eventuali messaggi di errore in relazione ad
attributi obbligatori non valorizzati e/o ad attributi univoci che
riportano lo stesso valore per articoli differenti.

**Gestisci nelle combinazioni:** consente di decidere se l'attributo in
esame dovrà o meno essere considerato nella definizione delle
combinazioni create per il set di attributi cui l'attributo stesso
risulterà essere associato

Per maggiori informazioni relativamente ai Set di attributi e alle
Combinazioni di attributi ad essi associate set si veda anche il
relativo capitolo di questo manuale "*Catalogo -- Gestione Attributi
Articolo -- Set di Attributi*"

Per quel che riguarda invece la possibilità di visualizzare o meno
l'Attributo in esame all'interno del componenti "Set Attributi" e
"Filtro Set Attributi" si veda il successivo capitolo di questo manuale.

##### GESTIONE VISUALIZZAZIONE

La sezione **"Gestione Visualizzazione"** consente di specificare se
l'attributo in esame dovrà essere visualizzato o meno all'interno del
componente "Set Attributi" / "Filtro Set Attributi" e che tipo di
ordinamento dovrà essere utilizzato per i valori da esso assunti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_attributi_gestione_visualizzazione.bmp](./assets/media/image111.png)

In questo senso dunque il parametro:

**Ordinamento Ricerca:** consente di indicare che tipo di ordinamento
(Alfabetico, Alfanumerico, Numerico) dovrà essere utilizzato per i
valori assunti dall'attributo in esame nel momento in cui questo stesso
attributo dovesse essere utilizzato come campo di filtro all'interno di
un pannello di ricerca articoli e dovesse essere visualizzato mediante
controlli di tipo "**Filtro Lista**", "**Filtro Indice**", "**Filtro
Checkbox**", "**Filtro Autocompletamento**"

Nel caso in cui il campo in esame dovesse essere lasciato vuoto, per i
valori assunti dal relativo attributo verrà utilizzato:

- un ordinamento di tipo Numerico per attributi Passweb di tipo "Numero"
  e per attributi Mexal collegati a campi numerici

- un ordinamento alfabetico in tutti gli altri casi

**ATTENZIONE!** Per ovvie ragioni un ordinamento di tipo numerico è
comunque ammesso solo su attributi numerici

In sostanza dunque, il campo "**Ordinamento Ricerca**" può rivelarsi
particolarmente utile, principalmente, in relazione ad attributi di tipo
testuale, offrendo all'utente la possibilità di scegliere tra
ordinamento alfabetico o alfanumerico e di ordinare quindi correttamente
valori del tipo "5 cm", "10 cm" ...

**Visualizza nel componente "Set Attributi"**: consente, se selezionato,
di rendere visibile il corrispondente attributo all'interno del
componente **"Set Attributi"**, componente questo che potrà essere
inserito all'interno della scheda prodotto dei vari articoli e che
consentirà di visualizzare in un colpo solo tutti gli attributi articolo
per i quali è stato selezionato il parametro in oggetto.

**Visualizza nel componente "Filtro Set Attributi"**: consente, se
impostato a **SI**, di visualizzare il corrispondente attributo
all'interno del pannello di ricerca articoli (componente "Filtro/Ricerca
Catalogo"), nel caso in cui sia stato inserito in questo stesso pannello
il componente **"Filtro Set Attributi"**.

**Tipo Campo di Ricerca (solo nel caso in cui il parametro "Visualizza
nel componente Filtro Set Attributi" sia stato impostato a SI)**:
consente di specificare il tipo di controllo che verrà utilizzato (lato
front-end) all'interno del componente "Filtro Set Attributi" per gestire
l'attributo in esame. E' possibile selezionare uno dei seguenti valori:

- **Testo:** all'interno del componente "Filtro Set Attributi" verrà
  visualizzato un semplice campo di input, nel quale l'utente dovrà
  digitare, per l'attributo in esame, il valore in base al quale
  effettuare una ricerca.

> In queste condizioni verranno inoltre visualizzati due ulteriori
> parametri "Segnaposto" e "Valore di Default" mediante i quali poter
> specificare rispettivamente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_filtro_set_testo.bmp](./assets/media/image95.png)

- **Segnaposto:** permette di definire un testo che verrà utilizzato
  **come segnaposto** all'interno del campo di input utilizzato per
  gestire, nel componente "Filtro Set Attributi", l'Attributo in esame

> **ATTENZIONE!** Al click dell'utente sul campo in esame il testo
> indicato scomparirà consentendo quindi all'utente di inserire il
> valore desiderato. Quanto indicato all'interno di questo campo non
> verrà quindi considerato alla conferma del form.

- **Valore di Default:** consente di indicare un testo che verrà
  utilizzato (e visualizzato) **come valore di default** per il campo di
  input utilizzato per gestire, nel componente "Filtro Set Attributi",
  l'Attributo in esame.

> **ATTENZIONE!** A differenza di quanto indicato per il precedente
> parametro "Segnaposto", il testo inserito all'interno del campo
> "Valore di default" **non scomparirà** in automatico al click
> dell'utente sul campo di input ma, al contrario, verrà considerato
> come se fosse un vero e proprio valore indicato dall\'utente stesso in
> fase di compilazione.
>
> Il valore indicato dall'utente all'interno di questi campi verrà
> effettivamente considerato nell'applicazione del filtro solo dopo aver
> cliccato sul relativo pulsante di ricerca.

- **Lista:** all'interno del componente "Filtro Set Attributi" verrà
  visualizzato un menu a tendina contenente l'elenco di tutti i
  possibili valori per l'attributo in esame, valori questi che l'utente
  del sito potrà utilizzare per effettuare le sue ricerche.

> In queste condizioni verranno inoltre visualizzati due ulteriori
> parametri "Valore di Default" e "Step" mediante i quali poter
> specificare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_filtro_set_lista.bmp](./assets/media/image96.png)

- **Valore di Default:** consente di indicare un testo che verrà
  utilizzato (e visualizzato) **come valore di default** per la select
  box utilizzata per gestire, nel componente "Filtro Set Attributi",
  l'Attributo in esame.

- **Step:** consente di indicare l'intervallo di definizione dei vari
  scaglioni che rappresenteranno poi le diverse possibili opzioni di
  scelta presenti all'interno del menu a tendina utilizzato per gestire,
  nel componente "Filtro Set Attributi", l'Attributo in esame.

> Supponendo dunque di impostare questo campo sul valore 100,
> all'interno del menu a tendina verranno visualizzate le seguenti
> opzioni: 0-100, 100-200, 200-300 ... L'utente potrà quindi ricercare
> tutti gli articoli per i quali l'attributo collegato al campo di
> ricerca in questione ha un valore compreso in uno dei range indicati
>
> Il valore del primo e dell'ultimo scaglione verranno determinati
> automaticamente sulla base de valori impostati sui vari articoli per
> l'attributo in esame.
>
> **ATTENZIONE!** Nel caso in cui lo step impostato dovesse essere tale
> da produrre un numero di scaglioni superiore a 100, all'interno del
> componente "Filtro Set Attributi" verrà visualizzato un apposito
> messaggio di errore e non verrà di fatto impostato nessun tipo di
> scaglione.
>
> **ATTENZIONE!** Per ovvie ragioni il campo Step potrà essere
> utilizzato solo ed esclusivamente su Attributi di tipo numerico. In
> caso contrario infatti, al salvataggio dell'Attributo, verrà ritornato
> un apposito messaggio di errore.

- **Slider:** all'interno del componente "Filtro Set Attributi" verrà
  visualizzato un controllo di tipo Slider mediante il quale poter
  consentire all'utente che naviga il sito di effettuare delle ricerche
  sulla base di attributi di tipo numerico.

> Le ricerche potranno essere effettuate impostando uno specifico valore
> minimo e/o massimo all'interno degli appositi campi di input, oppure
> impostando il range di ricerca mediante il trascinamento dei due
> piccoli pulsanti posti ai lati della barra visualizzata immediatamente
> al di sopra degli stessi campi di input.
>
> **ATTENZIONE!** Per ovvie ragioni il controllo di tipo Slider potrà
> essere utilizzato solo ed esclusivamente su Attributi di tipo
> numerico. In caso contrario infatti, al salvataggio dell'Attributo,
> verrà ritornato un apposito messaggio di errore.
>
> Per maggiori informazioni su questa particolare tipologia di controllo
> si veda anche la sezione "*Varianti Sito Responsive / Standard e
> Mobile -- Lista Componenti Ecommerce -- Componenti Interni ai
> Componenti Ecommerce -- Filtro Slider*" di questo manuale

- **Indice con/senza contatore di elementi:** all'interno del componente
  "Filtro Set Attributi" verrà visualizzato un elenco di tutti i
  possibili valori assunti dall'attributo in esame per i vari articoli
  gestiti all'interno del sito (eventualmente anche delle immagini).
  Ogni singola voce di questo elenco, se cliccata, consentirà di
  filtrare gli articoli in catalogo per l'attributo in esame e sulla
  base del valore selezionato. A fianco di ogni singola voce potrà
  inoltre comparire o meno (a seconda del fatto che l'indice sia con o
  senza contatore di elementi) l'esatto numero degli articoli in
  catalogo per i quali l'attributo in esame assume quello specifico
  valore.

- **Autocompletamento:** all'interno del componente "Filtro Set
  Attributi" verrà inserito un campo di input ad autocompletamento in
  cui poter visualizzare una lista di possibili opzioni da selezionare
  sulla base del testo mano a mano digitato dall'utente

> In queste condizioni verranno inoltre visualizzati tre ulteriori
> parametri "Segnaposto", "Valore di Default" e "Numero minimo di
> caratteri da digitare" mediante i quali poter specificare
> rispettivamente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributi_filtro_set_autocompletamento.bmp](./assets/media/image97.png)

- **Segnaposto:** permette di definire un testo che verrà utilizzato
  **come segnaposto** all'interno del campo ad autocompletamento
  utilizzato per gestire, nel componente "Filtro Set Attributi",
  l'Attributo in esame

> **ATTENZIONE!** Al click dell'utente sul campo in esame il testo
> indicato scomparirà consentendo quindi all'utente di inserire il
> valore desiderato. Quanto indicato all'interno di questo campo non
> verrà quindi considerato alla conferma del form.

- **Valore di Default:** consente di indicare un testo che verrà
  utilizzato (e visualizzato) **come valore di default** per il campo ad
  autocompletamento utilizzato per gestire, nel componente "Filtro Set
  Attributi", l'Attributo in esame

> **ATTENZIONE!** A differenza di quanto indicato per il precedente
> parametro "Segnaposto", il testo inserito all'interno del campo
> "Valore di default" non scomparirà in automatico al click dell'utente
> sul campo di input ma, al contrario, verrà considerato come se fosse
> un vero e proprio valore indicato dall\'utente stesso in fase di
> compilazione.
>
> In queste condizioni, per poter visualizzare l'elenco delle possibili
> opzioni di scelta sarà quindi indispensabile apportare una qualche
> variazione ad eventuali "Valori di Default" gestiti per il campo in
> esame.

- **Numero minimo di caratteri da digitare:** permette di specificare,
  selezionandolo da un apposito menu a tendina, l'esatto numero di
  caratteri che dovranno necessariamente essere digitati dall'utente
  prima di poter visualizzare l'elenco delle possibili opzioni di scelta

- **Numero massimo di opzioni da mostrare:** permette di specificare il
  numero massimo di opzioni che dovranno essere visualizzate nell'elenco
  delle possibili opzioni di scelta ottenute come risultato
  dell'autocompletamento

<!-- -->

- **Checkbox** **con/senza contatore di elementi:** all'interno del
  componente "Filtro Set Attributi" verrà visualizzato un elenco di
  tutti i possibili valori assunti dall'attributo in esame per i vari
  articoli gestiti all'interno del sito (eventualmente anche delle
  immagini) con a fianco un apposito check di selezione. La selezione di
  una delle voci presenti in elenco consentirà di filtrare gli articoli
  in catalogo per l'attributo in esame e sulla base del valore
  selezionato. A fianco di ogni singola voce potrà inoltre comparire o
  meno (a seconda del fatto che il check box sia con o senza contatore
  di elementi) l'esatto numero degli articoli in catalogo per i quali
  l'attributo in esame assume quello specifico valore.

- **Toggle Switch con/senza contatore di elementi:** all'interno del
  componente "Filtro Set Attributi" verrà visualizzato un elenco di
  tutti i possibili valori assunti dall'attributo in esame per i vari
  articoli gestiti all'interno del sito (eventualmente anche delle
  immagini) con a fianco un apposito controllo "on/off" di tipo Toggle
  Switch. L' impostazione del controllo su "on" consentirà di filtrare
  gli articoli in catalogo per l'attributo in esame e sulla base del
  valore selezionato. A fianco di ogni singola voce potrà inoltre
  comparire o meno (a seconda del fatto di aver selezionato l'opzione
  con o senza contatore di elementi) l'esatto numero degli articoli in
  catalogo per i quali l'attributo in esame assume quello specifico
  valore.

**NOTA BENE**: per maggiori informazioni relativamente alla gestione dei
componenti "Set Attributi" e "Filtro Set Attributi" si rimanda alla
relativa sezione di questo manuale.

##### GESTIONE OPZIONI

Una volta impostati tutti i parametri di configurazione dell'attributo
il pulsante "**Salva**", presente nella parte bassa della maschera,
oltre ad effettuare il salvataggio dei dati impostati, creando di fatto
il nuovo attributo articolo, permetterà di visualizzare anche
un'ulteriore sezione di configurazione, la sezione "**Gestione
Opzioni**" all'interno della quale poter indicare tutti i valori che
l'attributo in esame potrà assumere per ogni singolo articolo gestito
all'interno del sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opzioni_attributo_mexal.bmp](./assets/media/image112.png)

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in corrispondenza del campo "Valore" consente di filtrare i
dati in griglia sulla base del valore delle singole opzioni.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![Videate\\icona_elimina_filtro.bmp](./assets/media/image86.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

**Nel caso in esame per Attributi Passweb di tipo "Drop Down" e
"Selezione Multipla" i valori inseriti all'interno di questa sezione
verranno poi riproposti, come precedentemente evidenziato, in fase di
valorizzazione dell'attributo stesso.**

Per inserire un nuovo valore è sufficiente cliccare sul pulsante
raffigurante un piccolo +
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image99.png) ) presente nella barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Nuova
Opzione**", all'interno della quale poter inserire (parametro
"**Etichetta del campo**") il valore desiderato per ognuna delle lingue
gestite all'interno del sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributo_nuova_opzione.bmp](./assets/media/image100.png)

Gli altri due pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Esporta** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_esporta.bmp](./assets/media/image101.png) ): consente di esportare un file .csv
contenente tutti i valori attualmente presenti in elenco. Cliccando su
questo pulsante verrà visualizzata la maschera "**Esporta Valori**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributo_esporta_valori.bmp](./assets/media/image102.png)

all'interno della quale poter indicare lo specifico carattere separatore
che dovrà essere utilizzato nella generazione del file di esportazione.

Il pulsante "Conferma" consente invece di avviare la procedura di
creazione ed esportazione del file

**Importa** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_importa.bmp](./assets/media/image103.png) ) : consente di codificare in maniera
massiva i diversi possibili valori per l'attributo in oggetto
importandoli da un file .csv o .txt. Cliccando su questo pulsante verrà
visualizzata la maschera "**Importa Valori**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\attributo_importa_valori.bmp](./assets/media/image104.png)

all'interno della quale poter selezionare il file da importare (campo
"**File (csv-txt)**").

Il campo "**Lingua di riferimento**" consente di definire,
selezionandola tra quelle attualmente gestite, la lingua i cui valori
dovranno essere utilizzati come chiave per determinare se i contenuti
del file di importazione dovranno andare in aggiunta o in modifica ad
eventuali valori già presenti in elenco.

**ATTENZIONE!** Il file di importazione deve sempre contenere la lingua
impostata come lingua di riferimento

Supponendo dunque di indicare come lingua di riferimento la lingua
Italiana, per ogni valore dell'attributo inserito nel file di
importazione in corrispondenza della lingua italiana, verrà valutato se
questo stesso valore è o meno presente tra i valori già inseriti in
elenco.

In caso positivo verranno aggiornati, per lo stesso elemento i valori
corrispondenti nelle altre lingue gestite. In caso negativo verrà invece
inserito un nuovo elemento in elenco

Il campo **Separatore**: consente di indicare, selezionandolo,
dall'apposito menu a tendina, il carattere che è stato utilizzato
all'interno del file di importazione come separatore per i vari campi

Il check "**Elimina valori non presenti nel file**" consente invece, se
selezionato, di eliminare eventuali valori precedentemente inseriti e
non presenti nel file di importazione.

**ATTENZIONE! l'eliminazione di uno dei valori presenti in elenco
determina l'eliminazione di eventuali combinazioni di attributi in cui
questo stesso valore era stato utilizzato**

Affinchè la procedura di importazione possa terminare correttamente è
necessario che il file di importazione soddisfi le seguenti specifiche:

- L'intestazione, ossia la prima riga del file, deve contenere
  l'indicazione delle lingue gestite all'interno del sito, esattamente
  come queste stesse lingue sono indicate nella sezione "Sito --
  Gestione Lingue" del Wizard.

- Ogni riga del file deve contenere un possibile valore dell'attributo
  in ciascuna delle lingue indicate nella riga di intestazione.

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.

> In questo senso è quindi necessario che il valore dei campi contenenti
> interruzioni di riga, doppi apici e/o lo stesso carattere utilizzato
> anche come separatore sia necessariamente racchiuso da virgolette

Come per gli Attributi Mexal, anche in questo caso tali valori
diventeranno di fondamentale importanza nel momento in cui si dovesse
decidere di utilizzare l'attributo in esame all'interno di una serie di
filtri di ricerca in cascata vincolati sulla base di specifiche
combinazioni di attributi definite direttamente all'interno del Wizard
di Passweb.

I valori che un attributo potrà assumere in fase di creazione di una
particolare combinazione saranno infatti proprio quelli presenti
all'interno di questa stessa sezione.

In conseguenza di ciò è indispensabile, nel momento in cui si dovesse
decidere di utilizzare filtri di ricerca in cascata vincolati sulla base
di specifiche combinazioni di attributi, che **i valori inserirti
all'interno di questa sezione corrispondano esattamente con tutti i
diversi valori assunti da questo stesso attributo per gli articoli
gestiti all'interno del sito**

Per maggiori informazioni in merito alla gestione dei filtri di ricerca
vincolati in base a specifiche combinazioni di attributi si veda anche
il capitolo *"Live Editing -- Lista Componenti Ecommerce -- Componente
Ricerca--Ricerca Ecommerce -- Filtri di ricerca vincolati"* di questo
manuale.

