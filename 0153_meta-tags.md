# META TAGS



All'interno di questa sezione è possibile gestire i Meta Tag (non
presenti nativamente in Passweb) da inserire all'interno delle varie
pagine cui verrà associato il layout in esame.

![Videate\\layout_caratteristiche_1_res.bmp](./assets/media/image155.png)

I **Meta Tag** sono metadati presenti nel linguaggio HTML e utilizzati
per fornire informazioni sulle pagine agli utenti o ai motori di
ricerca.

I meta tag non forniscono al browser alcun dato di formattazione della
pagina, per cui il loro influsso sul layout grafico finale è
praticamente nullo; sono perciò totalmente invisibili all\'utente (se
non attraverso la visualizzazione del codice sorgente in HTML della
pagina oppure tramite le finestre di proprietà dei browser) e possono
essere utilizzati per svariati scopi.

Per aggiungere un nuovo Meta Tag al layout è sufficiente inserirlo
all'interno dell'apposita area di testo (**Meta Tag nella Pagina**) e
cliccare poi sul pulsante **"Applica Modifiche al Layout"**.

**ATTENZIONE! E' necessario inserire, all'interno di quest'area, il
corretto markup del Meta Tag e non solo il valore dei suoi attributi.**

Come precedentemente evidenziato i meta tag indicati all'interno di
questa sezione verranno poi inseriti su tutte le pagine cui verrà
applicato il layout in esame. Volendo è poi possibile inserire anche
altri meta tag sulle singole pagine (indipendenti da quelli gestiti a
livello di layout) agendo per questo dalle proprietà della pagina stessa
(per maggiori informazioni in merito si veda anche la sezione "*Live
Editing per Varianti Responsive -- Gestione Pagine*" di questo manuale.

Il pulsante **"Aggiungi segnaposto"** consente infine di inserire, nella
definizione del meta tag, dei segnaposto che verranno poi valorizzati in
maniera dinamica a seconda della specifica pagina in cui il meta tag
verrà applicato.

Sono gestiti i seguenti segnaposto:

- **Url sito:** il segnaposto verrà sostituito a runtime con il domino
  del sito (es. www.miosito.it)

- **Url pagina:** il segnaposto verrà sostituito a runtime con l' url
  della relativa pagina web, esclusi eventuali parametri di query string
  (es. www.miosito.it\\catalogo-articoli)

- **Url pagina completo della stringa di Query:** il segnaposto verrà
  sostituito a runtime con l' url competo della relativa pagina web (es.
  www.miosito/cms/blog/dettaglio-post?a=phasellus-fringilla)

- **Titolo Pagina:** il segnaposto verrà sostituito a runtime con lo
  stesso valore utilizzato per il meta tag \< title \>

Per inserire un nuovo segnaposto è sufficiente posizionare il cursore
nella posizione in cui questo dovrà essere effettivamente inserito,
cliccare sul pulsante "**Aggiungi segnaposto**" e selezionare dal
relativo menu contestuale la tipologia di segnaposto da inserire.

Grazie a questi segnaposto è quindi possibile definire a livello di
layout, dei meta tag con attributi che verranno poi valorizzati in
maniera diversa e completamente automatica per ogni singola pagina del
sito cui verrà applicato il layout in esame, senza dover dunque andare a
specificare in maniera manuale questo stesso meta tag nelle proprietà di
ogni singola pagina.

Un possibile caso d'uso, in questo senso, potrebbe essere quello
relativo alla gestione, **per pagine generiche**, del meta tag
"**canonical**" utilizzato per gestire problemi di penalizzazione, da
parte dei motori di ricerca, legati a contenuti duplicati presenti
all'interno del sito. Questo tag ha infatti un markup del tipo di quello
qui di seguito indicato:

**\<link rel=\"canonical\" href=\"http://www.miosito.com\" /\>**

dove l'attributo href dovrà essere valorizzato con l' url da
considerare, per la specifica pagina, come indirizzo predefinito (e
dunque l'unico da indicizzare).

Ora, anziché inserire questo meta tag in ogni singola pagina, indicando
manualmente il valore dell'attributo href, potrebbe essere possibile
inserirlo a livello di layout valorizzando l'attributo href con il
segnaposto **"Url Pagina".**

In questo modo sarà poi Passweb, in maniera completamente automatica, a
valorizzare correttamente per ogni singola pagina l'attributo href con
l'esatto url.

**ATTENZIONE! Nel caso in cui sia stato indicato un layout sia a livello
di Variante che a livello di singola Pagina i Meta Tag definiti sul
layout di Pagina andranno a sommarsi a quelli eventualmente definiti a
livello di Variante**

In particolare, nel codice HTML della pagina web verranno inseriti prima
i Meta Tag definiti sul layout associato alla Variante Sito, e poi
quelli definiti sul layout associato alla specifica pagina web.

