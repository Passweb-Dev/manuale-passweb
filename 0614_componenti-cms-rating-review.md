# COMPONENTI CMS -- RATING REVIEW



Il Componente **"Rating Review"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\cms_componente_rating_res.bmp](./assets/media/image60.png){width="2.545138888888889in"
height="2.765972222222222in"}

può essere inserito solo ed esclusivamente all'interno di quei
componenti di primo livello che, come l'Archivio News, vengono
utilizzati per visualizzare le news pubblicate all'interno del sito.

Il Rating Review consente infatti di visualizzare per ogni singola
notizia presente nel corrispondente componente di primo livello, il
valore medio (in un range che va da 1 a 5 stelle), delle valutazioni
assegnate dagli utenti del sito alla notizia stessa.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_esempio_cms.bmp](./assets/media/image61.png){width="4.66875in"
height="3.4805555555555556in"}

**Ovviamente, affinché il componente possa funzionare in maniera
corretta, è necessario gestire all'interno del sito anche i relativi
componenti CMS "Commenti Associati" e "Rating News".**

In caso contrario gli utenti non avrebbero infatti la possibilità di
commentare e/o di votare le singole notizie per cui il componente Rating
Review mostrerebbe sempre 5 stelle vuote.

> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> dei componenti "Commenti Associati" e "Rating News" si vedano anche le
> corrispondenti sezioni di questo manuale.

Dipendentemente dalla configurazione del componente, esso potrà
visualizzare soltanto la media dei voti assegnati alla notizia oppure
anche il totale delle recensioni effettuate dagli utenti per quella
stessa notizia.

In quest'ultimo caso il totale delle recensioni sarà un link che porterà
direttamente alla specifica sezione della pagina "Dettaglio News" in cui
è stato inserito il componente "Commenti Associati" e in cui verrà
dunque visualizzato il dettaglio di tutte le recensioni.

Inoltre è anche possibile abilitare, al passaggio del mouse sulle 5
stelle, la visualizzazione di un pop up contenente un istogramma con il
dettaglio dei voti assegnati alla relativa notizia. In questo modo sarà
quindi possibile sapere esattamente quante recensioni hanno assegnato
alla notizia 5 stelle, quante 4, quante 3 ecc...

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_istogramma_cms.bmp](./assets/media/image62.png){width="4.66875in"
height="3.4805555555555556in"}

All'interno del tooltip, come mostrato nella figura sopra riportata,
verrà infine visualizzato il valore esatto della media dei voti
assegnati alla specifica notizia.

Rilasciando il Componente nella posizione desiderata all'interno della
pagina, verrà visualizzata **la sua maschera di gestione e
configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\rating_review_cms_configurazione_res.bmp](./assets/media/image63.png){width="4.623611111111111in"
height="3.084722222222222in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile settare i
principali parametri di configurazione del componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di definire un nome per il Componente che si sta
editando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

**Percorso immagine Stella Off/On/Half:** consente di impostare le
immagini da utilizzare per la visualizzazione del rating della notizia.
A default per l'immagine Off viene utilizzata una stella vuota (colore
grigio), per l'immagine On una stella piena (colore giallo) e per
l'immagine Half una stella piena a metà

**Visualizzazione Totale recensioni:** consente di abilitare o meno la
visualizzazione all'interno del componente anche del totale delle
recensioni effettuate sulla notizia. E' possibile selezionare uno dei
seguenti valori:

- **Non visualizzare totale recensioni:** in questo caso all'interno del
  componente verranno visualizzate solo le 5 stelle (o le eventuali
  immagini personalizzate) che indicheranno il valore medio dei voti
  ricevuti dalla notizia.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_no_recensioni_cms.bmp](./assets/media/image64.png){width="4.6819444444444445in"
height="3.4805555555555556in"}

- **Numero totale recensioni senza testo:** in questo caso verrà
  visualizzato all'interno del componente, oltre alle 5 stelle (o alle
  eventuali immagini personalizzate) anche il numero totale delle
  recensioni ottenute dalla specifica notizia.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_tot_recensioni_cms.bmp](./assets/media/image65.png){width="4.6819444444444445in"
height="3.4805555555555556in"}

- **Numero totale recensioni con testo:** in questo caso verrà
  visualizzato all'interno del componente, oltre alle 5 stelle (o alle
  eventuali immagini personalizzate) anche il numero totale delle
  recensioni ottenute dalla notizia con a fianco una specifica label

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_testo_recensioni_cms.bmp](./assets/media/image66.png){width="4.6819444444444445in"
height="3.5131944444444443in"}

**NOTA BENE**: negli ultimi due casi il testo con il totale delle
recensioni sarà un link che porterà direttamente alla specifica sezione
della pagina di "Dettaglio News" in cui è stato inserito il componente
"Commenti Associati" e in cui verrà dunque visualizzato il dettaglio di
tutte le recensioni.

**Visualizza Istogramma recensioni:** consente di impostare la modalità
di visualizzazione dell'istogramma contenete il dettaglio dei voti
assegnati alla relativa news. E' possibile selezionare uno dei seguenti
valori

- **Visualizza Popup istogramma recensioni:** se selezionato consente di
  visualizzare, al passaggio del mouse sulle 5 stelle, un pop up
  contenente un istogramma con il dettaglio dei voti assegnati alla
  relativa news. In questo modo sarà quindi possibile sapere esattamente
  quante recensioni hanno assegnato alla notizia 5 stelle, quante 4,
  quante 3 ecc...

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\rating_review_istogramma_cms.bmp](./assets/media/image62.png){width="4.6819444444444445in"
height="3.49375in"}

> All'interno del tooltip, come mostrato nella figura sopra riportata,
> verrà visualizzato il valore esatto della media dei voti assegnati
> alla news.
>
> **All'interno del Wizard il Popup con l'istogramma dei voti a default
> non è visualizzato.**
>
> E' comunque possibile richiamarlo per poterlo poi editare graficamente
> con lo style editor di Passweb, visualizzando quello che sarà il
> risultato ottenuto all'interno del sito. Per fare questo è sufficiente
> cliccare sul piccolo segno + posto a fianco del componente

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\grafica_istogramma_cms.bmp](./assets/media/image67.png){width="4.6819444444444445in"
height="3.4027777777777777in"}

> Il pulsante raffigurante un piccolo segno -- consente invece di
> chiudere il Popup dell'istogramma e di tornare quindi nelle condizioni
> iniziali.

- **Visualizza tramite tabella:** consente di visualizzare l'istogramma
  con il dettaglio dei voti assegnati alla news direttamente all'interno
  della pagina web mediante un'apposita tabella

**Posizionamento rating e totale recensioni:** consente di posizionare
gli elementi principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- I controlli per il rating del prodotto

- Il totale delle recensioni

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

