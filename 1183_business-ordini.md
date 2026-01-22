# BUSINESS -- ORDINI



Per poter accedere a questa particolare sezione dell'Area Riservata è
necessario, innanzitutto, aver abilitato l'App Business operando per
questo all'interno dell'apposita sezione del Wizard accessibile dal menu
"*Sito -- Preferenze*".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_business_attivazione.bmp](./assets/media/image163.png)

Una volta attivata l'App, all'interno di questa sezione dell' area
riservata l'utente attualmente loggato avrà poi la possibilità di
visualizzare l'elenco e lo stato di tutti i suoi documenti.

**ATTENZIONE**!: **Nel momento in cui l'utente attualmente loggato
dovesse essere un Agente Mexal, all'interno di questa sezione verranno
visualizzati i documenti di tutti i clienti che l'Agente stesso è in
grado di gestire**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_agente_ordini.bmp](./assets/media/image205.png)

Per ciascuno dei documenti presenti in elenco viene indicato:

- **Sigla** del documento

- **Cliente** Intestatario

- **Totale** Documento

- **Stato** Documento

- **Agente** (se presente)

- **Data** Documento

Inoltre nel caso in cui uno specifico documento sia stato originato
dalla trasformazione o dalla fusione di altri documenti, nella relativa
riga della tabella Ordini comparirà anche un'icona raffigurante una
piccola i (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_icona_proprieta.bmp](./assets/media/image206.png) ), attraverso cui poter visualizzare
l'elenco dei documenti che lo hanno originato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ricerca_documenti_origine.bmp](./assets/media/image207.png)

I dati presenti in tabella sono ordinati, a default, per data
decrescente (quindi dal documento più recente a quello meno recente). L'
icona raffigurante due piccole frecce (
![Videate\\icona_ordinamento_griglia.bmp](./assets/media/image77.png) ) posta in testata a fianco del nome
delle varie colonne, consente invece di modificare l'ordinamento dei
dati, in maniera crescente e/o decrescente, sulla base dei valori
presenti all'interno della relativa colonna.

Il pulsante "**Colonne**" (
![Videate\\pulsante_colonne_ar.bmp](./assets/media/image170.png) ), presente, in corrispondenza
dell'ultima colonna della griglia, consente di decidere quali
informazioni dovranno essere visualizzate direttamente in tabella.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Colonne**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_colonne_ordini_ar.bmp](./assets/media/image208.png)

mediante la quale poter decidere quale campo attivare / disattivare e
conseguentemente quale informazione mostrare / nascondere.

Il pulsante "**Colonne**" (
![Videate\\pulsante_colonne_ar.bmp](./assets/media/image170.png) ) è presente anche in visualizzazione
mobile ma, in questo caso, il suo comportamento sarà leggermente diverso
rispetto a quello che si ha in visualizzazione desktop

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_griglia_ordini_mobile.bmp](./assets/media/image209.png)

In questo caso infatti le colonne visibili in tabella saranno sempre e
soltanto due (per ovvie ragioni di spazio) di cui la prima, quella
relativa alla sigla del documento conterrà anche l'informazione relativa
allo stato e sarà sempre visibile, la seconda potrà invece essere
impostata dall'utente scegliendola tra quelle disponibili all'interno
del pop up di selezione delle colonne.

Inoltre, sempre in visualizzazione mobile, nel momento in cui si dovesse
decidere di non visualizzare una seconda colonna, all'interno della
colonna Sigla verrà automaticamente visualizzato, oltre alla sigla e
allo stato del documento, anche il nome del cliente intestatario del
documento stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_griglia_ordini_mobile_sc.bmp](./assets/media/image210.png)

**ATTENZIONE!** l'impostazione delle colonne da visualizzare è un dato
specifico per singolo utente. Ogni utente abilitato ad accedere in area
riservata potrà quindi decidere quali colonne visualizzare
immediatamente in griglia e quali no

Il pannello di **"Ricerca"**, presente nella parte alta della pagina
consente invece di ricercare uno specifico documento, tra quelli in
elenco, per:

- **Sigla**

- Periodo temporale (campi **Da Data a** **Data**)

- **Nome** dell'intestatario (campo **Cliente**)

- **Stato Documento**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_ricerca_ordini.bmp](./assets/media/image211.png)

**ATTENZIONE!** Nel caso in cui si voglia effettuare una ricerca dei
documenti emessi in una specifica data è sufficiente indicare questa
stessa data all'interno del campo "Da Data"

Relativamente alle ricerche effettuate per sigla documento, i risultati
potranno essere relativi a documenti che hanno per sigla o per origine
il valore ricercato o parte di esso.

Nel caso in cui, ad esempio sia stato evaso l'ordine OC1/686 con la
bolla BC1/22 nell'elenco dei documenti comparirà, come mostrato nella
figura sopra riportata, la bolla BC1/22 con a fianco un'icona che
consentirà di visualizzare i documenti di origine di questa stessa
bolla. In queste condizioni dunque effettuando una ricerca per sigla
documento, e .nello specifico, indicando come sigla documento
indifferentemente OC1/686 o BC1/22 verrà comunque visualizzato come
risultato della ricerca lo stesso documento (BC1/22).

**L\'unico vincolo relativo a questo tipo di ricerca (ricerca per
origine) è rappresentato dal fatto che il valore indicato come filtro
deve necessariamente contenere almeno la tipologia di documento**.

In pratica dunque, se, come filtro di ricerca viene indicato
semplicemente "686", la ricerca si limiterà a trovare tutte le possibili
corrispondenze di documenti che hanno il valore "686" nella loro sigla,
senza effettuare ricerche sui documenti di origine. In queste condizioni
dunque nell'esempio sopra riportato la ricerca per Sigla Documento = 686
non produrrebbe alcun risultato

Nel caso in cui invece come filtro di ricerca venga indicato "OC1/686"
allora la ricerca verrà effettuata sia documenti effettivamente presenti
in elenco sia sui loro documenti di origine e, nell'esempio sopra
riportato il risultato di questa ricerca sarebbe correttamente il
documento BC1/22 (restituito grazie alla presenza del relativo documento
di origine OC1/6868)

Ovviamente è anche possibile visualizzare il dettaglio di ogni singolo
documento presente in elenco.

Per far questo, in "modalità desktop" sarà sufficiente cliccare sulla
riga del documento desiderato per aprire automaticamente la relativa
maschera di dettaglio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_dettaglio_documento.bmp](./assets/media/image212.png)

In visualizzazione mobile, sarà invece necessario selezionare il
documento desiderato tra quelli presenti in elenco e cliccare sul
pulsante "**Visualizza Dettaglio**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_elenco_ordini_mobile.bmp](./assets/media/image213.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_dettaglio_ordine_mobile.bmp](./assets/media/image214.png)

Relativamente alla pagina di dettaglio è bene sottolineare che, una
parte del layout di questa pagina è cablato e non si può quindi
modificare in alcun modo, mentre un'altra parte può essere
tranquillamente personalizzata operando direttamente dal backend di
Passweb.

Nello specifico la parte **non modificabile** è quella relativa ai tab
"**Dettaglio Ordine**" e "**Docuvision**", **ai pulsanti "Elenco Ordini"
e "Stampa" e agli identificativi del documento**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_dettaglio_ordine_non_modificabile.bmp](./assets/media/image215.png)

Tutto il resto della pagina, ossia il vero e proprio dettaglio del
documento, può essere personalizzato secondo le specifiche esigenze del
caso, agendo direttamente nel backend di Passweb dal campo
"**Dettaglio**" presente alla pagina "**Ordini -- Configurazione
Ordini**" (tab "**Documento**") o dall'analogo campo relativo ai Resi

![Videate\\ordine_dettaglio_ar.bmp](./assets/media/image216.png)

Per maggiori informazioni in merito alla creazione del Template
utilizzato per la visualizzazione del dettaglio dei documenti in Area
Riservata si veda anche quanto indicato nei relativi capitoli di questo
manuale ("*Ordini -- Ordini -- Configurazione Ordini -- Documento*")

Una volta visualizzato il dettaglio di un documento sarà possibile
stamparlo -- pulsante **Stampa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_pulsante_stampa_dettaglio.bmp](./assets/media/image217.png)) -- o accedere al documentale
Passepartout per prelevare, in tempo reale, tutte le risorse associate,
all'interno del gestionale, al documento in esame.

Per quel che riguarda la Stampa, il layout utilizzato può essere
personalizzato secondo le proprie esigenze operando, anche in questo
caso, dal backend di Passweb e, nello specifico, agendo all'interno del
campo "**Dettaglio Stampa**" presente anch'esso alla pagina "**Ordini --
Configurazione Ordini**" (tab "**Documento**") del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_dettaglio_stampa.bmp](./assets/media/image218.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ordine_dettaglio_stampa_esempio.bmp](./assets/media/image219.png)

Per maggiori informazioni in merito alla creazione del Template
utilizzato per la Stampa dei si veda anche quanto indicato nel relativo
capitolo di questo manuale ("*Ordini -- Ordini -- Configurazione Ordini
-- Documento*")

**ATTENZIONE!** Si ricorda che il layout di Stampa è lo stesso
utilizzato anche nel front end del sito

Per quel che riguarda invece l'accesso al documentale Passepartout sarà
sufficiente cliccare sul pulsante "**Docuvision**" (
![Videate\\pulsante_docuvision_ordine.bmp](./assets/media/image220.png) ) presente in testata. In questo modo
verrà infatti aperta una connessione in tempo reale con Mexal e verrà
prelevato l'elenco di tutte le risorse associate, all'interno del
gestionale, al documento in esame

![Videate\\ar_docuvision_ordini.bmp](./assets/media/image199.png)

**ATTENZIONE:** la chiamata a Mexal per visualizzare l'elenco delle
risorse associate al documento in esame, verrà effettuata
automaticamente soltanto la prima volta che si effettua l'accesso al tab
"Docuvision"

In questo modo sarà quindi possibile passare tranquillamente dal tab
"Dettaglio Ordine" al "tab "Docuvision" senza dover ogni volta attendere
il termine della comunicazione sito -- gestionale.

Il pannello di ricerca presente nella sezione di sinistra consente di
effettuare ricerche mirate tra gli allegati del documento per Data e/o
per Titolo

**ATTENZIONE!** **il pannello di ricerca sarà visibile solo nel caso in
cui siano state correttamente attivate, per il proprio sito Ecommerce,
le Web Api Mexal.** In caso contrario (Web Api non attive) non sarà
quindi possibile effettuare alcun tipo di ricerca tra gli allegati del
documento.

Per maggiori informazioni relativamente all'attivazione delle Web Api
Mexal si veda anche quanto indicato nel capitolo "*Configurazione --
Mexal Configurazione Gestionale -- WebApi Mexal*" di questo manuale

Infine per scaricare e visualizzare il dettaglio di una delle risorse
associate al documento sarà sufficiente cliccare sul pulsante di
download
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_pulsante_scarica_documento.bmp](./assets/media/image221.png)) relativo a quella specifica risorsa.

Nel caso in cui la risorsa da scaricare dovesse essere un file xml
generato dall'emissione di una fattura elettronica, in fase di download
verrà creato uno zip contenente l'xml della fattura stessa e un file
html mediante il quale poter visualizzare il dettaglio della fattura
elettronica utilizzando il file xsl di Passepartout.

In queste condizioni per visualizzare sul browser il dettaglio della
fattura elettronica sarà quindi necessario decomprimere l'archivio .zip
ed aprire il file con estensione .html presente al suo interno.

**ATTENZIONE!** **in questa sezione dell'area riservata verranno
prelevati dal gestionale solo ed esclusivamente le risorse associate in
Docuvision alla classe dei "Movimenti di Magazzino"**

**ATTENZIONE!** dipendentemente dalle dimensioni del file da scaricare,
e considerando anche che lo stesso file verrà prelevato in tempo reale
dal gestionale, il download potrebbe impiegare un po' di tempo.

In conseguenza di ciò, una volta avviato il download, verrà visualizzata
un'animazione di loading in maniera tale, da una parte, da indicare
all'utente che l'operazione sta procedendo e, dall'altra parte, da
impedirgli di effettuare ulteriori click su eventuali altri documenti da
scaricare prima che l'operazione in essere sia terminata correttamente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_loading_docuvison_ordini.bmp](./assets/media/image222.png)

