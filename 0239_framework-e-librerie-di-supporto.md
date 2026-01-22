# FRAMEWORK E LIBRERIE DI SUPPORTO



Se, da una parte, tutti i concetti esaminati fino a questo momento
(media query, break-point, griglie fluide ecc...) possono
tranquillamente essere implementati "manualmente" in una Variante
Standard di Passweb e senza dover per forza di cose ricorrere a
strumenti esterni, dall'altra parte è comunque vero che un concetto
fondamentale, non solo del responsive design, ma di tutta l'informatica
è quello di **riutilizzare il più possibile quanto di buono è già stato
fatto.**

In questo senso, in ambito responsivo, non mancano di certo le
opportunità. Innanzitutto però è importante distinguere due casi e cioè
se la necessità è quella di adattare un'qualcosa di già esistente
rendendolo responsive oppure se il sito è nuovo o va comunque rifatto da
zero.

Nel primo caso l'introduzione di un framework potrebbe essere una
soluzione troppo invasiva e il discorso diventerebbe quindi più
complicato. In queste condizioni la soluzione migliore sarebbe
indubbiamente quella di sporcarsi le mani andando a modificare ed
ottimizzare il codice CSS esistente anche se, come inizialmente
evidenziato, riuscire a rendere responsivo un sito pensato, progettato e
implementato non con questa finalità diventa un'impresa veramente ardua.

Nel secondo caso invece non c'è che l'imbarazzo della scelta, esistono
orami tantissimi framework responsivi completi, ben fatti ed efficaci,
che implementano già tutte regole viste e molto di più.

In questo senso va detto che le **Varianti Responsive di Passweb**
implementano in maniera nativa il framework **Bootstrap** **4
(<https://getbootstrap.com/> )** ereditandone dunque le principali
caratteristiche strutturali come, ad esempio, quelle di seguito
indicate:

- Compatibilità con le ultime versioni di **Chrome, Firefox, Safari,
  Internet Explorer 10 -- 11 e Microsoft Edge**

- Box-sizing impostato sul valore Border-box

> Di base tutti i componenti delle Varianti Responsive di Passweb hanno
> il valore della proprietà CSS box-sizing impostata sul valore
> border-box.
>
> In queste condizioni dunque **padding e bordi di ogni elemento vengono
> inclusi nel calcolo della larghezza impostata per l'elemento stesso
> dalla proprietà width**
>
> In ogni caso è perfettamente possibile modificare il valore di questa
> proprietà agendo mediante lo Style Editor di Passweb.
>
> Per maggiori informazioni in merito si veda anche il capitolo "*Style
> Editor per Varianti Responsive*" di questo manuale.

- Breakpoint responsivi impostati sui seguenti valori della larghezza
  minima del dispositivo di visualizzazione:

  - **576 px 🡪 Small Devices (es. Smartphone in modalità Landscape)**

  - **768 px 🡪 Medium Devices (es. Tablet in modalità Portrait)**

  - **992 px 🡪 Large Devices (es. Tablet in modalità Landscape)**

  - **1200 px 🡪 Extra Large Devices (es. Desktop con risoluzioni
    superiori o uguali ai 1200px)**

- Modello di visualizzazione Flexbox

> ...

Ovviamente poi, il fatto di implementare nativamente il framework
Bootstrap consente agli utenti più esperti di utilizzare i vari campi
presenti nelle maschere di configurazione dei componenti (es. "Classi
Addizionali" e "Attributi Addizionali") piuttosto che gli strumenti di
editing avanzato offerti da Passweb (Componenti HTML, Layout, CSS,
Javascript) per sfruttare appieno tutte le funzionalità di questo
framework, comprese anche quelle non presenti nativamente su alcuni
componenti.

Una volta compresi i concetti fondamentali che stanno alla base di un
design responsivo e, a livello generale, come questi vengono
implementati nelle Varianti Responsive di Passweb, possiamo ora scendere
maggiormente nei dettagli andando ad esaminare le opzioni di
configurazione e le possibilità offerte da ogni singolo componente
presente nella libreria delle Varianti Responsive di Passweb.

