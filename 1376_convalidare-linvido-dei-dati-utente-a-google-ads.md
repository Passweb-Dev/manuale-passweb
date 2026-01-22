# CONVALIDARE L'INVIDO DEI DATI UTENTE A GOOGLE ADS



Per verificare che le conversioni avanzate per il web di Google Ads
funzionino in maniera corretta e che quindi non ci siano problemi nel
nostro sistema di tracciamento è possibile procedere in diversi modi:

- Seguendo la procedura indicata all'interno del capitolo "*Google Tag
  Manager -- User Provided Data e Conversioni Avanzate -- Tag di
  tracciamento di GA4 / ADS con User Provided Data -- Convalidare
  l'invio dei dati utente a GA4 / Google Ads*" di questo manuale

- Utilizzando gli strumenti per sviluppatori di Chrome (nel caso in
  tracciamento diretto Sito Passweb -- Google Ads)

- Utilizzando Tag Assistant partendo direttamente da Google Ads

Per quel che riguarda il primo dei tre metodi indicati si rimanda al
relativo capitolo del manuale.

Per quel che riguarda invece la procedura di validazione mediante gli
strumenti per sviluppatori di Chrome, anche in questo caso il modo di
procedere è sostanzialmente analogo a quello descritto all'interno del
capitolo relativo alle conversioni avanzate di Google Analytics e, di
base, si tratta sempre di analizzare il dettaglio delle chiamate inviate
dal sito direttamente a Google Ads ricercando poi la variabile em
deputata alla gestione dei dati utente.

Nello specifico sarà dunque necessario:

- Portarsi alla pagina del sito in cui dovrebbe registrarsi la
  conversione.

> In questo senso **si ricorda che** **Passweb gestisce il tracciamento
> diretto Sito -- Google Ads solo ed esclusivamente in merito a
> conversioni legate ad eventi di Purchase.**
>
> In considerazione di ciò sarà quindi necessario portarsi alla pagina
> di checkout e inserire tutti i dati necessari per poter poi confermare
> l'ordine.
>
> Prima della conferma definitiva aprire gli strumenti per sviluppatori
> di Chrome (tasto funzione F12) e accedere alla sezione **Network** (o
> Rete dipendentemente da quella che è la lingua di utilizzo del
> browser) dove potremo esaminare il dettaglio di tutte le chiamate
> effettuate dal browser

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_1.bmp](./assets/media/image9.png){width="5.346527777777778in"
height="3.5in"}

- Una volta effettuato l'accesso a questa sezione degli Strumenti per
  Sviluppatori dovremo cliccare sul piccolo segnale di divieto posto in
  alto a sinistra nella barra degli strumenti in maniera tale da
  eliminare lo storico di eventuali precedenti chiamate e dovremo anche
  verificare di aver selezionato l'opzione All presente sempre nella
  barra degli strumenti di questa sezione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_2.bmp](./assets/media/image10.png){width="5.346527777777778in"
height="3.5in"}

- A questo punto posto, ovviamente, di aver prestato tutti i consensi
  necessari per consentire di attivare il sistema di tracciamento,
  dovremo completare la conversione finalizzando l'acquisto. Verremo
  quindi ricondotti alla pagina di conferma dell'ordine e vedremo
  popolarsi la scheda Network degli Strumenti per sviluppatori di Chrome
  con tutte le varie chiamate effettuate dal browser

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_3.bmp](./assets/media/image11.png){width="5.353472222222222in"
height="3.5069444444444446in"}

- Tra tutte queste chiamate dovremo ora isolare quelle effettuate verso
  Google Ads e per far questo sarà sufficiente inserire nel pannello di
  ricerca presente nella barra degli strumenti di questa sezione la
  stringa "**googleadservices.com/pagead/conversion**" oppure la stringa
  "**google.com/pagead/1p-conversion**" (la stringa da ricercare che
  individua la chiamata fatta dal browser verso Google Ads può cambiare
  a seconda del browser utilizzato)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_4.bmp](./assets/media/image12.png){width="5.346527777777778in"
height="3.5in"}

- Una volta isolate la chiamate effettuate dal browser verso Google Ads
  dovremo esaminarne il dettaglio semplicemente cliccandoci sopra e
  portandoci poi nella scheda "**Payload**" cliccando sull'apposito
  pulsante presente nella parte destra della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_5.bmp](./assets/media/image13.png){width="5.346527777777778in"
height="3.5in"}

- Arrivati a questo punto per verificare che i dati utente siano stati
  inviati correttamente a Google Ads assieme alla relativa conversione,
  dovremo semplicemente cercare, tra quelli presenti all'interno della
  scheda Payload evidenziata in figura, il **parametro em che è per
  l'appunto quello deputato alla gestione dei dati utente.**

> La presenza e il valore di questo parametro ci dirà dunque se,
> nell'ambito della chiamata esaminata, i dati utente necessari per la
> conversione avanzata sono stati inviati o meno a Google Analytics e,
> in caso positivo, se tale invio ha presentato o meno degli errori

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_6.bmp](./assets/media/image14.png){width="5.346527777777778in"
height="3.5in"}

> Nello specifico:

- **Se il parametro em manca** completamente, significa che i dati
  utente, necessari per la gestione delle conversioni avanzate, non sono
  stati inviati.

- **Se è presente il parametro em**, ma è simile a "**tv.1\~em.**",
  significa che il parametro delle conversioni avanzate viene inviato,
  ma è vuoto e quindi, anche in questo caso, che i dati utente non sono
  stati inviati

- **Se è presente il parametro em**, ma è simile a "**tv.1\~em.e1**",
  significa che il parametro delle conversioni avanzate è stato inviato
  correttamente, ma si è verificato un problema nei dati inviati.

- **Se il parametro em è presente** ed è simile a **"tv.1\~em." seguito
  da una lunga stringa di caratteri** (come nel caso evidenziato in
  figura), significa che il tag delle conversioni avanzate sta rilevando
  ed eseguendo correttamente l\'hashing dell\'oggetto
  enhanced_conversion_data, che i dati utente sono stati trasferiti
  correttamente a Google Ads e che quindi la conversione avanzata
  dovrebbe essere registrata senza problemi

Per quel che riguarda, infine l'ultimo possibile metodo di convalida
che, come detto, comporta l'utilizzo di Tag Assistant si dovrà partire
direttamente dal proprio account Ads.

Qui una volta attivate le conversioni avanzate (secondo quanto descritto
nel precedente capitoli di questo manuale) e inserito un obiettivo di
conversione, se questo dovesse poi presentare dei problemi verranno
visualizzati appositi messaggi in corrispondenza delle colonne "Stato" e
"Azioni"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_7.bmp](./assets/media/image15.png){width="5.406944444444444in"
height="3.520138888888889in"}

In queste condizioni, sarà quindi necessario:

- Cliccare sul pulsante "**Risolvi i problemi**" presente in
  corrispondenza dell'obiettivo per cui dovremo tracciare la conversione
  avanzata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_8.bmp](./assets/media/image16.png){width="5.406944444444444in"
height="3.520138888888889in"}

- Nella successiva maschera, che ci spiegherà la procedura da seguire
  per validare la conversione, cliccare sul pulsante "**Continua**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_9.bmp](./assets/media/image17.png){width="5.406944444444444in"
height="3.520138888888889in"}

- Verrà quindi aperta la maschera di connessione a Tag Assistant

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_10.bmp](./assets/media/image18.png){width="5.406944444444444in"
height="3.520138888888889in"}

> Digitare quindi, se non presente, l'url del nostro sito e cliccare sul
> pulsante "**Connetti**"

- Su di un nuovo tab del browser verrà aperto il nostro sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_12.bmp](./assets/media/image19.png){width="5.406944444444444in"
height="3.520138888888889in"}

> mentre nel tab attuale avremo la possibilità di vedere ed esaminare
> nel dettaglio tutti i tag e gli hit inviati dal browser ai sistemi di
> tracciamento collegati tra cui anche Google Ads

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_11.bmp](./assets/media/image20.png){width="5.406944444444444in"
height="3.520138888888889in"}

- Spostandoci nel tab di visualizzazione del sito dovremo a questo punto
  completare un ordine in maniera tale da attivare la conversione che
  dovrebbe poi essere registrata da Ads

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_13.bmp](./assets/media/image21.png){width="5.406944444444444in"
height="3.520138888888889in"}

- Una volta completata la conversione, se tutto ha funzionato
  correttamente, vedremo cambiare il messaggio presente all'interno del
  piccolo pop up di Tag Assistant

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_14.bmp](./assets/media/image22.png){width="5.406944444444444in"
height="3.520138888888889in"}

> messaggio questo che, ora, ci informerà che è tutto a posto e che la
> conversione effettuata sul sito sta inviando correttamente i dati

- Ad ulteriore verifica potremmo anche aprire il tab del browser con i
  vari tag di tracciamento, selezionare il Tag di conversione e nella
  maschera di dettaglio (come già indicato nei corrispondenti capitoli
  relativi a Google Analytics o Google Tag manager) cercare il solito
  parametro em

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_15.bmp](./assets/media/image23.png){width="5.406944444444444in"
height="3.520138888888889in"}

- Fatte tutte le verifiche del caso potremo chiudere Tag Assistant
  cliccando sul pulsante "Fine" presente nel suo piccolo pop up
  iniettato nel tab del nostro sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_16.bmp](./assets/media/image24.png){width="5.406944444444444in"
height="3.520138888888889in"}

> e nella successiva maschera sul pulsante "Chiudi Tag Assistant"

![Videate\\gads_convalida_ec_16.bmp](./assets/media/image24.png){width="5.406944444444444in"
height="3.520138888888889in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_17.bmp](./assets/media/image25.png){width="5.406944444444444in"
height="3.520138888888889in"}

- A questo punto dovremo soltanto attendere che il sito inizi ad inviare
  dei dati reali ad Ads (tipicamente sono richieste almeno 72 ore) dopo
  di che se tutto ha funzionato correttamente anche l'obiettivo
  configurato all'interno di Ads dovrebbe mostrare in corrispondenza
  della colonna "Stato" l'etichetta "**Attivo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gads_convalida_ec_18.bmp](./assets/media/image26.png){width="5.406944444444444in"
height="3.520138888888889in"}

