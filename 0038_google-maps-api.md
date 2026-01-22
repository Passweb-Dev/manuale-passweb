# GOOGLE MAPS API



Passweb dispone di una serie di componenti mediante i quali poter
integrare all'interno del proprio sito una o più Google Map con scopi
differenti

**ATTENZIONE! Come indicato da Google, dal 16 Luglio 2018 è entrato in
vigore un nuovo piano tariffario basato sul consumo per Maps, Routes e
Places.**

In sostanza, mentre prima di tale data era necessario semplicemente
possedere un account Google e generare ed associare una chiave API per
poter visualizzare correttamente le mappe sul sito, dal 16 Luglio 2018 è
imperativo associare una carta di credito all'account Google utilizzato
per la generazione delle API key stesse (pena problematiche nella
visualizzazione della mappa), in modo che, a seconda della fruizione
delle mappe sul sito, Google possa poi fatturare quanto necessario.

Questo non significa, in ogni caso, che sia necessario pagare per poter
fruire delle mappe, è infatti la stessa Google a specificare che:

"quando attiverai la fatturazione, riceverai \$ 200 al mese di utilizzo
gratuito per Maps, Routes o Places. In base ai milioni di utenti che
utilizzano ogni giorno le nostre API, grazie a questo credito la maggior
parte di loro potrà continuare a usare gratuitamente Google Maps
Platform".

Per maggiori informazioni relativamente alle politiche Google in merito
all'utilizzo della mappe è possibile consultare il seguente link:

<https://cloud.google.com/maps-platform/user-guide/?hl=it>

Posto quindi di aver ottemperato a tutte le richieste effettuate da
Google in merito all'utilizzo delle mappe, all'interno della sezione
"**Google -- Google Maps API**" del Wizard sarà poi possibile impostare
le chiavi necessarie per utilizzare all'interno del proprio sito le
varie funzionalità messe a disposizione dalle Mappe di Google

![](./assets/media/image67.png)

Nello specifico il campo:

- **Chiave Google Maps API**: consente di inserire la chiave che verrà
  poi utilizzata per visualizzare e gestire correttamente all'interno
  del sito tutti i componenti che fanno uso della Google Map (Google
  Map, Store Locator, Checkout ecc...)

> **ATTENZIONE!** In fase di creazione della chiave è bene sempre
> applicare tutte le restrizioni di sicurezza richieste da Google in
> maniera tale da essere sicuri che questa stessa chiave non venga poi
> utilizzata in maniera indesiderata anche in altri contesti.
>
> In questo senso secondo quanto richiesto da Google la chiave in esame
> dovrebbe implementare delle restrizioni **a livello di referrer**

![](./assets/media/image68.png)

- **Chiave Google Maps Distance API**: consente di inserire la chiave
  che verrà poi utilizzata per calcolare, in fase di checkout, la
  distanza tra l'indirizzo di spedizione dell'utente e i vari punti
  vendita associati al metodo di trasporto selezionato in modo tale da
  visualizzare solamente quelli che rientrano nel raggio di km indicato
  in fase di configurazione della specifica zona (per maggiori
  informazioni in merito si veda anche quanto indicato all'interno del
  capitolo "*Ordini -- Metodi di trasporto -- Trasporti di tipo Passweb
  -- Zone di spedizione*" di questo manuale).

> **ATTENZIONE!** In fase di creazione della chiave è bene sempre
> applicare tutte le restrizioni di sicurezza richieste da Google in
> maniera tale da essere sicuri che questa stessa chiave non venga poi
> utilizzata in maniera indesiderata anche in altri contesti.
>
> In questo senso secondo quanto richiesto da Google la chiave in esame
> dovrebbe implementare delle restrizioni **a livello Indirizzo IP** (in
> questo caso sarà quindi necessario richiedere a Passepartout
> l'indirizzo IP della macchina su cui risiede il sito o, in alternativa
> ricavarlo in autonomia effettuando un semplice ping al dominio del
> sito)

![](./assets/media/image69.png)

Nel successivo capitolo di questo manuale ("*Chiavi Google Maps*"),
viene descritta la procedura da seguire per ottenere le due chiavi da
inserire nei campi appena esaminati (si consiglia comunque di fare
sempre riferimento alla specifica documentazione Google)

##### CHIAVI GOOGLE MAPS

Per ottenere le chiavi da inserire all'interno dei campi "**Chiave
Google Maps API**" e "**Chiave Google Maps Distance API**" esaminati nel
precedente capitolo di questo manuale è necessario:

1.  Accedere all'indirizzo <https://console.developers.google.com>
    utilizzando il proprio account Google

![](./assets/media/image70.png)

2.  Una volta effettuato l'accesso alla Google Developers Console aprire
    il menu a tendina posizionato nella parte alta della pagina e creare
    poi un nuovo progetto cliccando sulla relativa voce

![](./assets/media/image71.png)

3.  Una volta avviata la creazione di un nuovo progetto sarà necessario
    assegnargli un nome e cliccare poi sul pulsante **Crea**

![](./assets/media/image72.png)

4.  Una volta completata la creazione del progetto sarà poi necessario
    accedere alla sezione "**Libreria**" cliccando per questo sulla
    relativa voce di menu presente sulla sinistra della pagina

![](./assets/media/image73.png)

5.  Selezionare quindi, tra quelle presenti in Libreria, le api relative
    al servizio "**Maps Javascript API**"

![](./assets/media/image74.png)

> e successivamente cliccare sul pulsante "**Abilita**"

![](./assets/media/image75.png)

6.  Seguendo lo stesso procedimento abilitare anche le API di seguito
    indicate:

    - **Geocoding API** (necessaria per la chiave da inserire
      all'interno )

    - **Places API**

    - **Directions API**

    - **Geolocation API**

> **ATTENZIONE!** è necessaria l'attivazione di tutte le api indicate
> per garantire il corretto funzionamento sul sito dei componenti che
> fanno uso della Google Map

7.  Allo stesso modo nel momento in cui l'esigenza dovesse essere quella
    di ottenere la chiave da inserire all'interno del campo Passweb
    "**Chiave Google Maps Distance API**" è necessario attivare anche le
    seguenti API:

    - **Distance Matrix API**

> **ATTENZIONE!** per fare in modo che possa essere correttamente
> calcolata la distanza tra l'indirizzo di spedizione dell'utente e i
> vari punti vendita associati al metodo di trasporto selezionato, è
> necessario accertarsi che per la chiave inserita all'interno del campo
> Passweb "**Chiave Google Maps Distance API**" sia stata correttamente
> attivata l'API sopra evidenziata

8.  Una volta abilitate le API di cui ai due punti precedenti, aprire il
    menu di navigazione cliccando sul relativo pulsante presente nella
    parte alta della pagina e selezionare la voce "**API e servizi -
    Credenziali**"

![](./assets/media/image76.png)

9.  Cliccare quindi sulla voce "**Crea Credenziali**" e successivamente
    sulla voce "**Chiave API**" evidenziata in figura

![](./assets/media/image77.png)

10. Completata la creazione verrà visualizzata una maschera contenente
    la chiave da inserire all'interno del proprio sito Passweb

![](./assets/media/image78.png)

> Copiare quindi il contenuto del campo "**La tua chiave API**" ed
> inserirlo, a seconda del tipo chiave che si è deciso di generare,
> all'interno del campo "**Chiave Google Maps API**" o "**Chiave Google
> Maps Distance API**" presente alla pagina "*Sito -- Preferenze --
> Integrazioni*" del Wizard, sezione relativa a Google.

![](./assets/media/image67.png)

11. Completare la configurazione della chiave API aggiungendo tutte le
    limitazioni del caso. Portarsi quindi, sulla Google developer
    console, all'interno della sezione "**Credenziali**", individuare la
    chiave API precedentemente generata e cliccare quindi sull'icona
    raffigurante una piccola matita presente in corrispondenza di questa
    stessa chiave

![](./assets/media/image79.png)

12. Nella maschera di dettaglio della chiave, assegnare un nome alla
    chiave stessa all'interno del campo "**Nome**" e soprattutto
    configurare le limitazioni come di seguito indicato

> **[CHIAVE PER IL CAMPO GOOGLE MAPS API]{.underline}**
>
> All'interno della sezione "**Restrizione delle applicazioni**"
> selezionare l'opzione "**Referrer http (siti web)**", cliccare sul
> pulsante "**Aggiungi un elemento**" e successivamente inserire
> all'interno del campo "Nuovo elemento" il dominio del proprio sito web

![](./assets/media/image80.png)

> Cliccare quindi sul pulsante "**Fine**"
>
> All'interno della sezione "**Restrizioni delle API**" selezionare
> invece l'opzione "**Limita chiave**" e cliccare sul campo "**Select
> APIs**"

![](./assets/media/image81.png)

> In questo modo dovrebbero comparire tutte le API attualmente attive
> per il progetto su cui stiamo lavorando (e tra queste quindi anche
> quelle precedentemente abilitate).
>
> Selezionare quindi le 5 API abilitate ai punti 5 e 6 e,
> successivamente cliccare sul pulsante "**Salva**" presente nella parte
> bassa della pagina
>
> **[CHIAVE PER IL CAMPO GOOGLE MAPS DISTANCE API]{.underline}**
>
> All'interno della sezione "**Restrizione delle applicazioni**"
> selezionare l'opzione "**Indirizzi IP**", cliccare sul pulsante
> "**Aggiungi un elemento**" e successivamente inserire all'interno del
> campo "Nuovo elemento" l'indirizzo IP del server su cui è hostato il
> proprio sito web.
>
> Per ottenere questo indirizzo IP è necessario chiedere direttamente a
> Passepartout oppure ricavare questa informazione con un semplice ping
> al dominio del proprio sito

![](./assets/media/image69.png)

> Cliccare quindi sul pulsante "**Fine**"
>
> All'interno della sezione "**Restrizioni delle API**" selezionare
> invece l'opzione "**Limita chiave**" e cliccare sul campo "**Select
> APIs**"

![](./assets/media/image82.png)

> In questo modo dovrebbero comparire tutte le API attualmente attive
> per il progetto su cui stiamo lavorando (e tra queste quindi anche la
> Distance Matrix API).
>
> Selezionare quindi le API abilitate ai punti 5 e 6 e, successivamente
> cliccare sul pulsante "**Salva**" presente nella parte bassa della
> pagina

**ATTENZIONE! Si ricorda ancora una volta che poter visualizzare
correttamente le mappe sul sito, a partire dal 16 Luglio 2018 è
imperativo associare una carta di credito all'account Google utilizzato
per la generazione delle API key**

