# CONFIGURAZIONE



All'interno di questa sezione è possibile tra le altre cose:

- definire la modalità di accesso al proprio sito web

- impostare i crediti del sito

- abilitare lo Smooth Scrolling

- impostare la Favicon

- impostare i principali parametri di configurazione dell'Area Riservata
  (es. tema grafico, visualizzazione del menu, abilitazione /
  disabilitazione delle singole sezioni ecc...)

- impostare il tempo massimo di conservazione dei log

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze.bmp](./assets/media/image1.png){width="4.486805555555556in"
height="2.7402777777777776in"}

Nello specifico i parametri presenti all'interno della sezione
"**Visibilità Sito e Restrizioni**" consentono rispettivamente di:

- **Sito in lavorazione:** permette di decidere se porre o meno il sito
  nello stato di "Work in progress". E' possibile selezionare una delle
  seguenti opzioni:

  - **No:** in questo caso il sito sarà on line e correttamente
    visualizzabile in tutte le sue pagine

  - **Si:** in questo caso il sito verrà messo nello stato di "Work in
    progress" e visitando un suo qualsiasi url verrà sempre visualizzata
    una pagina di manutenzione con il contenuto inserito nel successivo
    campo "**Testo Sito in Lavorazione"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_workinprogress.bmp](./assets/media/image2.png){width="4.461111111111111in"
height="2.7729166666666667in"}

- **Logo dell'Area Riservata e Sito in Lavorazione:** consente di
  selezionare l'immagine che verrà visualizzata:

  - in testata all'interno dell'Area Riservata del sito nel caso di
    visualizzazione "light mode"

  - nella pagina "Sito in Lavorazione"

  - nella pagina di pagamento di SumUp

> Cliccando sul pulsante "**Seleziona la Risorsa**" verrà visualizzata
> la maschera di "**Gestione Risorse**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_gest_risorse.bmp](./assets/media/image3.png){width="4.590972222222222in"
height="2.876388888888889in"}

> attraverso la quale poter selezionare l'immagine da utilizzare come
> Logo.
>
> Nel caso in cui la risorsa non sia presente tra quelle in elenco, è
> possibile aggiungerla cliccando sul pulsate **"Pubblica un File"**

- **Logo Dark Area Riservata**: consente di selezionare l'immagine che
  verrà visualizzata, in testata, all'interno dell'Area Riservata del
  sito in visualizzazione "dark mode"

- **Designed by:** consente di impostare il nome dell'azienda che ha
  progettato e realizzato il sito.

> Valorizzando questo campo nella parte bassa di ogni pagina del sito
> compariranno i crediti "Designed by ..." seguito dal nome dell'azienda
> impostato all'interno del campo in esame.
>
> **ATTENZIONE! Oltre ai crediti "Designed by ..." opzionali e
> attivabili semplicemente inserendo un testo all'interno del campo in
> esame, nella parte bassa di ogni pagina compariranno sempre anche i
> crediti "Powered by Passepartout" (con link alla relativa sezione del
> sito Passepartout.net) relativi all'azienda produttrice del software
> utilizzato per realizzare e gestire il sito.**
>
> I crediti sono gestiti come ultimo elemento all'interno del
> contenitore strutturale "Riquadro sito". Per poterli quindi stilizzare
> in maniera tale da renderli uniformi con il resto del piede di pagina
> è sufficiente abilitare da Live Editing la modalità di gestione dei
> contenitori strutturali, selezionare dall'albero dei componenti il
> contenitore strutturale "Riquadro Sito", aprire il Live Editing ed
> agire sugli elementi "**Credits**" e "**Credits Link**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stile_crediti.bmp](./assets/media/image4.png){width="2.8569444444444443in"
height="2.2270833333333333in"}

- **Mostra popup sessione scaduta:** se attivato, consente di
  visualizzare, una volta scaduta la sessione sul front end del sito, un
  apposito messaggio per informare l'utente relativamente al fatto che
  potrebbe essere necessario effettuare nuovamente l'autenticazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\popup_sessione_frontend.bmp](./assets/media/image5.png){width="5.376388888888889in"
height="3.325in"}

> Il messaggio in questione può essere personalizzato alla pagina
> "**Sito -- Testi Messaggi del sito -- Testi Generici**" agendo
> sull'elemento "**Sessione Utente**"
>
> **ATTENZIONE!** il popup di "Sessione Scaduta" verrà visualizzato solo
> ed esclusivamente nel momento in cui si dovesse tentare, una volta
> scaduta la sessione utente, di interagire in qualche modo con la
> pagina del browser rimasta aperta. Tentando di cambiare pagina il
> messaggio in esame non verrà quindi visualizzato.

La sezione "**Smooth scrolling**" (scorrimento dolce della pagina web),
consente invece di abilitare, per il proprio sito web, l'omonimo effetto
javascript.

**ATTENZIONE!** L'effetto di Smooth Scrolling può essere attivato solo
ed esclusivamente su Varianti Responsive.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\smooth_scrolling.bmp](./assets/media/image6.png){width="4.486805555555556in"
height="2.7729166666666667in"}

Nel caso in cui l'esigenza dovesse essere quindi quella di attivare per
le pagine del proprio sito l'effetto di scorrimento dolce, sarà
sufficiente flaggare il campo "**Abilita lo Smooth Scrolling**" e
impostare poi un valore per i due parametri di seguito indicati:

- **ScrollTime:** consente di impostare il tempo di scrolling della
  pagina web, ossia l'intervallo di tempo entro cui verrà portata a
  termine la relativa animazione di scorrimento

- **Scroll Distance**: consente di indicare il numero di pixel di cui si
  sposterà la pagina web ad ogni scrollata. Utilizzando valori più
  piccoli lo scrolling della pagina avverrà in maniera più lenta,
  utilizzando invece valori più grandi lo scrolling avverrà più
  velocemente.

Si consiglia di utilizzare questo tipo di effetto grafico principalmente
nel caso in cui si utilizzi all'interno del proprio sito anche un
effetto di parallasse in maniera tale da evitare scatti allo scrolling
della pagina rendendo quindi più fluido ed evidente l'effetto stesso del
parallasse.

Per maggiori informazioni in merito all'effetto di parallasse si veda
anche la relativa sezione di questo manuale ("*Varianti Responsive --
Lista Componenti Comuni -- Componente Contenitore*")

**ATTENZIONE! Eventuali modifiche ai parametri presenti all'interno di
questa sezione verranno applicati al sito solo al termine della sessione
corrente.**

Per rendere quindi immediatamente visibili e attive sul proprio browser
tali modifiche sarà sufficiente eliminare tutti i cookie di sessione.

La sezione "**Favicon**" consente di impostare la Favicon del proprio
sito web.

- **Favicon:** consente di definire l'icona che verrà visualizzata nella
  barra degli indirizzi del Browser accanto al nome del sito web.

> Cliccando sul pulsante "**Seleziona la Risorsa**" verrà visualizzata
> la maschera di "Gestione Risorse" attraverso cui poter selezionare
> l'immagine da utilizzare come Favicon. Per maggiori informazioni sul
> caricamento di una risorsa in Passweb si rimanda al paragrafo
> "Gestione Risorse del Sito" di questo manuale.
>
> **NOTA BENE**: la risorsa da utilizzare come Favicon deve
> necessariamente essere un file di tipo icona (.ico) di dimensioni non
> superiori a 16 X 16 pixel.
>
> Nel caso in cui la risorsa non sia presente tra quelle in elenco, è
> possibile aggiungerla cliccando sul pulsate **"Pubblica un File"**
> (vedi anche pagina "Gestione Risorse del Sito" di questo manuale).

La sezione "**Area Riservata\"** consente di impostare i principali
parametri di configurazione dell'Area Riservata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\preferenze_area_riservata2.bmp](./assets/media/image7.png){width="4.5256944444444445in"
height="2.7729166666666667in"}

Per maggiori informazioni in merito a questa sezione si veda quanto
indicato nel successivo capitolo di questo manuale.

La sezione "**Sistema\"** consente infine di impostare il tempo di
conservazione di determinati log.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\preferenze_logIIS.bmp](./assets/media/image8.png){width="5.629861111111111in"
height="3.4479166666666665in"}

Nello specifico il parametro

- **Tempo di Conservazione dei Log del Web Server**: consente di
  definire quello che dovrà essere il tempo massimo di conservazione dei
  Log utilizzati per gestire le statistiche del sito e dei Log relativi
  alle pubblicazione sui vari Marketplace (sia a livello di singoli
  articoli che di intere liste di vendita)

- **Tempo di conservazione dei Log delle Mail:** consente di definire
  quello che dovrà essere il tempo massimo di conservazione dei Log
  delle Mail

**ATTENZIONE!** Variando le impostazioni relative al tempo di
conservazione dei log eventuali cancellazioni di file precedenti al
periodo impostato, avverranno in automatico durante la notte del giorno
di variazione.

