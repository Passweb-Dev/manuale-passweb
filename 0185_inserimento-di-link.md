# INSERIMENTO DI LINK



Per creare un collegamento ipertestuale nel testo è sufficiente
selezionare il testo desiderato e premere sul pulsante
"**Inserisci/Modifica Collegamento"** presente nella barra degli
strumenti (). Verrà in questo modo aperta la maschera **"Collegamento"**
qui di seguito riporta

![](./assets/media/image288.png)

attraverso la quale poter specificare tutte le caratteristiche del
collegamento ipertestuale che si intende realizzare.

In particolare il parametro:

- **Tipo di Collegamento:** consente di selezionare, dal relativo menù a
  tendina, il tipo di collegamento che si vuole realizzare (per maggiori
  informazioni relativamente alle diverse tipologie di link gestibili da
  questa sezione dell'Editor, si vedano i successivi capitoli di questo
  manuale).

I Tab "**Destinazione** " e "**Avanzate**" presenti nell'interfaccia di
configurazione dei link consentono di definire ulteriori proprietà e
caratteristiche del collegamento che si intende realizzare.

Nello specifico la scheda "**Destinazione**" consente di stabilire dove
e come dovrà essere aperto il collegamento che si sta realizzando.

![](./assets/media/image289.png)

In particolare per il parametro "Target" i valori:

- **Riquadro/Topmost Window/Parent Window:** consentono di gestire la
  destinazione del collegamento nel caso in cui siano presenti
  all'interno della stessa pagina uno o più framset

- **New Window:** consente di aprire la destinazione del collegamento in
  una nuova scheda del browser

- **Same Window:** consente di aprire la destinazione del collegamento
  nella stessa scheda del browser in cui si trova il link che si sta
  realizzando

- **Finestra popup:** consente di aprire la destinazione del
  collegamento in un apposito popup. Selezionando questo valore
  l'interfaccia di configurazione del link si modificherà offrendo
  all'utente tutti i parametri necessari per configurare, secondo quelle
  che sono le sue specifiche esigenze, la finestra di popup che verrà
  generata.

Sarà quindi possibile impostare le dimensioni della finestra di popup,
le coordinate in corrispondenza delle quali fare aprire il popup, se la
finestra del popup dovrà essere ridimensionabile o meno ecc...

All'interno della scheda "**Avanzate**" sarà invece possibile
specificare, per il link in esame proprietà quali l'id, il title,
eventuali classi css aggiuntive ecc...

##### LINK ESTERNO (URL)

Impostando il parametro **"Tipo Collegamento**" sul valore **URL** è
possibile creare un link ad una qualsiasi pagina di un qualsiasi altro
sito internet oppure ad una risorsa interna al sito stesso (es. un
documento o un file compresso), risorsa questa che potrà poi essere
downlodata dagli utenti del sito cliccando sul collegamento in esame.

![](./assets/media/image290.png)

Nel primo caso (collegamento ad una qualsiasi pagina di un qualsiasi
altro sito internet) i campi **Protocollo** e **URL** consentono di
specificare rispettivamente il protocollo (http, https, ftp ecc ...) da
utilizzare nel collegamento ipertestuale che si sta realizzando e
l'indirizzo di destinazione del collegamento stesso(es. www.google.it)

Nel secondo caso, per poter realizzare il collegamento ad una risorsa
del sito e permettere quindi ai vari visitatori di poter effettuare poi
il download di questa stessa risorsa, sarà necessario, per prima cosa,
cliccare sul pulsante "**Cerca sul server**".

In questo modo verrà infatti aperta la maschera di "**Gestione
Risorse**" del sito attraverso cui poter selezionare la risorsa da
associare al link che si sta realizzando.

Una volta selezionata la risorsa desiderata, il campo "Protocollo" verrà
automaticamente valorizzato con "altro" mentre il campo "URL" verrà
anch'esso valorizzato in maniera completamente automatica con l'esatto
percorso della risorsa precedentemente selezionata.

**ATTENZIONE**! Nel caso in cui la risorsa da scaricare sia di
dimensioni considerevoli (svariati MB) si consiglia di selezionare il
check "**Download file in Streaming**" in modo tale da velocizzare il
processo di download evitando così di sovraccaricare il proprio sito.

Lato front end, nel momento in cui un utente dovesse cliccare sul link
appena creato, verrebbe avviato immediatamente il download della risorsa
associa al link stesso.

##### LINK INTERNO ALLA PAGINA (ANCORA) 

Impostando il parametro **"Tipo Collegamento**" sul valore "**Ancora nel
testo**" è possibile creare un link ad uno specifico elemento
(**ancora**) presente all'interno della pagina stessa.

Per poter realizzare questo tipo di collegamento è quindi necessario,
per prima cosa, creare all'interno della pagina apposite ancore da poter
poi utilizzare come destinazione del collegamento.

Per far questo è sufficiente posizionare il cursore, all'interno di un
componente Paragrafo, nella posizione in cui si vuole realizzare
l'ancora e cliccare poi sul pulsante "**Inserisci / Modifica Ancora**" (
) presente nella barra degli strumenti. Verrà in questo modo
visualizzata la maschera "**Proprietà ancora**"

![](./assets/media/image291.png)

attraverso cui poter assegnare un nome all'ancora che si sta
realizzando.

Il nome delle varie ancore create all'interno della pagina verrà poi
visualizzato nel relativo combo box del pannellino "Scegli ancora", in
maniera tale da permettere di selezionare uno specifico punto
all'interno della pagina, da utilizzare come destinazione per il "**Link
interno alla Pagina**" che si intende realizzare.

##### LINK AD UNA PAGINA DEL SITO

Impostando il parametro **"Tipo Collegamento**" sul valore "**Link ad
una Pagina del sito**" è possibile creare un collegamento dinamico ad
una pagina interna al sito.

![](./assets/media/image292.png)

L'albero delle pagine presente all'interno del riquadro "**Link ad una
pagina del sito**" permette di selezionare la specifica pagina di
destinazione per il collegamento che si sta realizzando.

Il check "**Apri come finestra modale**" consente, se selezionato di
aprire la pagina di destinazione all'interno di un'apposita finestra
modale (Pop Up).

Per maggiori informazioni in merito alla gestione delle pagine di tipo
Pop Up si veda anche il capitolo "*Live Editing -- Pagine -- Pagine
Popup Creazione e Gestione*" di questo manuale.

##### LINK ALL'AREA RISERVATA

Impostando il parametro **"Tipo Collegamento**" sul valore "**Link
all'Area Riservata**" è possibile creare collegamenti diretti alle varie
sezioni dell'Area Riservata.

In particolare selezionando questa opzione la destinazione del
collegamento verrà gestita a livello di codice HTML, come evidenziato
nella figura di seguito riportata, con il segnaposto **AR** racchiuso
tra doppie parentesi graffe.

![](./assets/media/image293.png)

In queste condizioni il link creato funzionerà in maniera diversa a
seconda del fatto che l'utente abbia o meno già effettuato
l'autenticazione al sito.

Nel primo caso (utente già autenticato) il link porterà direttamente
alla "Bacheca"

Nel secondo caso (utente non ancora autenticato) il link porterà invece
alla pagina di accesso in Area Riservata e l'utente dovrà, per poter
accedere, inserire le proprie credenziali.

Nel caso in cui l'esigenza dovesse essere invece quella di creare dei
collegamenti diretti a specifiche sezioni dell'Area Riservata, sarà
necessario intervenire manualmente andando a modificare il segnaposto
AR, inserito da Passweb, aggiungendo ad esso anche l'indicazione della
specifica sezione dell'Area Riservata cui il collegamento in esame dovrà
ricondurre.

**ATTENZIONE! I segnaposto indicati dovranno essere racchiusi sempre tra
doppie parentesi graffe**

Le sezioni linkabili sono le seguenti:

- **Bacheca**: per raggiungere tale sezione sarà necessario inserire
  come valore dell'attributo href, per il link in esame, il seguente
  segnaposto **AR:Bacheca**

- **Messaggi/Ricevuti**: per raggiungere tale sezione sarà quindi
  necessario utilizzare la stringa **AR:Messaggi/Ricevuti**

- **Documenti**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:Documenti**

- **Agenda**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:Agenda**

- **B2B/Clienti**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:B2B/Clienti**

- **B2B/Ordini**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:B2B/Ordini**

- **B2B/Cliente**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:B2B/Cliente**

- **Sprix**: per raggiungere tale sezione sarà quindi necessario
  utilizzare la stringa **AR:Sprix**

Ovviamente le relative sezioni potranno essere raggiunte in maniera
diretta solo nel caso in cui l'utente abbia già effettuato
l'autenticazione al sito. In caso contrario, indipendentemente dalla
particolare sezione linkata l'utente verrà comunque ricondotto alla
pagina di accesso in Area Riservata e, per poter accedere, dovrà prima
inserire le proprie credenziali

##### LINK A PRODOTTO

Impostando il parametro **"Tipo Collegamento**" sul valore "**Link a
Prodotto**" è possibile creare un collegamento ad una specifica pagina
Prodotto.

![](./assets/media/image294.png)

Il prodotto da utilizzare come destinazione del collegamento potrà
essere selezionato tra quelli presenti all'interno del riquadro "**Link
ad un prodotto**".

##### LINK A ARTICOLO CMS

Impostando il parametro **"Tipo Collegamento**" sul valore "**Link a
Articolo CMS**" è possibile creare un collegamento ad uno specifico
articolo/post del proprio sito web, realizzato utilizzando i componenti
CMS messi a disposizione da Passweb.

![](./assets/media/image295.png)

Lo specifico articolo da utilizzare come destinazione del collegamento
potrà essere selezionato tra quelli presenti all'interno del box
"**Articolo**".

L'albero delle pagine presente invece all'interno del box "**Pagina di
Lettura Articolo**" consente di specificare la pagina del sito in cui
dovrà essere visualizzato l'articolo selezionato.

**NOTA BENE:** la pagina di lettura dell'articolo dovrà necessariamente
contenere il componente CMS **"Dettaglio News"** correttamente
configurato. Per maggiori informazioni relativamente ai componenti CMS
si veda la corrispondente sezione di questo manuale.

##### E-MAIL

Impostando il parametro **"Tipo Collegamento**" sul valore "**E-mail**"
è possibile creare un collegamento ad una specifica casella di posta.

![](./assets/media/image296.png)

Cliccando sul di un link di questo tipo verrà aperto in maniera
completamente automatica il client di posta predefinito dell'utente e
verrà predisposto un nuovo messaggio che avrà: come destinatario
l'indirizzo specificato nel campo "**Indirizzo Mail**" della maschera
sopra evidenziata, come oggetto il testo indicato nel campo
"**Oggetto**" e come contenuto il testo inserito all'interno del campo
"**Corpo del Messaggio**".

