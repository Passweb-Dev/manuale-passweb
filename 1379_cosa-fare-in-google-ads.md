# COSA FARE IN GOOGLE ADS



Per poter attivare il flusso di gestione delle conversioni offline
secondo quanto descritto nei precedenti capitoli di questo manuale sarà
necessario settare in maniera corretta anche il proprio account Google
Ads.

Nello specifico, da una parte dovremo attivare e settare correttamente
le "Conversioni Avanzate per i Leads" e, dall'altra parte, dovremo
invece configurare correttamente un upload schedulato dei dati prodotti
da Passweb relativamente a quegli ordini che sono stati pagati e
conclusi in maniera corretta senza però che l'utente sia tornato nella
pagina di Conferma Ordine.

Per quel che riguarda l'attivazione delle Conversioni Avanzate per i
Leads sarà necessario:

1.  Accedere all'account Google Ads, portarsi alla sezione "**Obiettivi
    -- Impostazioni**" ed espandere la voce "Conversioni avanzate per i
    lead" presente nella parte destra della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_5.bmp](./assets/media/image32.png)

2.  Selezionare il check "**Attiva le conversioni avanzate per i lead**"

![Videate\\conversioni_offline_5.bmp](./assets/media/image32.png)

3.  Come già fatto nel caso delle "Conversioni Avanzate per il web",
    anche in questo caso abilitando il parametro "Attiva le conversioni
    avanzate i lead" verrà visualizzato un ulteriore campo all'interno
    del quale dovremo andare ad indicare il metodo utilizzato per
    gestire e configurare i dati forniti dagli utenti (nel caso
    specifico la mail che verrà inviata da Passweb a Google Ads nel
    momento in cui l'utente abbandonerà il sito per essere ridiretto sul
    gateway di pagamento).

> In sostanza dovremo indicare esattamente, selezionandolo dal relativo
> menu a tendina, il metodo adottato nel nostro sistema di tracciamento
> per inviare a Google Ads i dati utente.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_7.bmp](./assets/media/image33.png)

> Come evidenziato in figura le opzioni possibili sono 2:

- Tag Google

- Google Tag Manager

> Passweb gestisce entrambe le opzioni indicate, nello specifico dovremo
> quindi selezionare:

- **Tag Google** se abbiamo scelto di inviare ad Ads la mail dell'utente
  che sta effettuando l'ordine direttamente dal sito Passweb

- **Google Tag Manager** se abbiamo scelto di inviare ad Ads la mail
  dell'utente che sta effettuando l'ordine mediante Google Tag manager

> **ATTENZIONE!** **E' fondamentale selezionare esattamente l'opzione
> corrispondente al metodo di tracciamento che abbiamo deciso di
> implementare all'interno del nostro sito Passweb**
>
> Nel momento in cui dovessimo infatti indicare, all'interno di questo
> campo, un valore non corrispondente a quello che poi andremo
> effettivamente ad utilizzare per inviare i dati utente a Google Ads,
> questi stessi dati non verranno mail elaborati.
>
> Tanto per intenderci se, all'interno di questo campo, dovessimo
> selezionare l'opzione Google Tag, ma lato Passweb dovessimo poi
> decidere di implementare l'invio dei dati utente a Google Ads mediante
> Google Tag Manager quello indicato all'interno di Google Ads non
> corrisponderà a quello che effettivamente facciamo all'interno del
> sito Passweb per cui i dati utente non potranno mai essere elaborati.

Per quel che riguarda invece il fatto di dover configurare correttamente
un upload schedulato dei dati prodotti da Passweb relativamente a quegli
ordini che sono stati pagati e conclusi in maniera corretta senza però
che l'utente sia tornato nella pagina di Conferma Ordine sarà
necessario:

1.  Accedere all'account Google Ads, portarsi alla sezione "**Obiettivi
    -- Caricamenti - Pianificazioni**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_8.bmp](./assets/media/image34.png)

> e, da qui cliccare sul pulsante raffigurante un piccolo **+** per
> creare una nuova pianificazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_9.bmp](./assets/media/image35.png)

2.  Nella maschera di creazione della nuova pianificazione dovremo
    cliccare sul menu a tendina "**Seleziona origine**" selezionando poi
    tra le opzioni proposte la voce "**HTTPS**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_10.bmp](./assets/media/image36.png)

3.  In questo modo avremo la possibilità di indicare a Google Ads un
    indirizzo web che Ads stesso controllerà periodicamente, con la
    frequenza che andremo poi ad indicare, e da cui preleverà i dati
    relativi a quegli ordini che si sono conclusi correttamente sul
    nostro sito ecommerce senza però il ritorno dell'utente sulla pagina
    di conferma, e senza quindi che Passweb abbia potuto inviare i dati
    di conversione

![Videate\\conversioni_offline_11.bmp](./assets/media/image37.png)

> In particolare all'interno del campo **URL di origine** dovremo
> indicare un url del tipo:
>
> **https://www.nomesito.it/wizard/orders/GetConversionFileADS**
>
> dove ovviamente la stringa "www.nomesito.it" dovrà essere sostituita
> con il dominio effettivo del nostro sito Passweb
>
> I campi "**Nome utente**" e "**Password**" possono invece essere
> lasciati vuoti, mentre in corrispondenza dei campi "**Frequenza**" e
> "**Ora**" dovremo indicare esattamente ogni quanto tempo (consigliata
> l'opzione "**Ogni 24 ore**") e a che ora Google Ads dovrà andare a
> prelevare dal' url indicato il file contenente i dati delle
> conversioni da importare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_12.bmp](./assets/media/image38.png)

> Cliccando sul pulsante "**Salva e visualizza l'anteprima**" presente
> nella parte bassa della maschera oltre a salvare la pianificazione
> indicata potremo anche verificare un anteprima di quello che sarà il
> risultato dell'importazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_13.bmp](./assets/media/image39.png)

> All'interno della sezione "Caricamenti" avremo invece la possibilità
> di visualizzare lo storico dei caricamenti effettuati con il relativo
> esito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_14.bmp](./assets/media/image40.png)

Ora per quel che riguarda il file contenente i dati delle conversioni da
uplodare in Google Ads, disponibile come detto all'indirizzo
*https://www.nomesito.it/wizard/orders/GetConversionFileADS***,** vanno
fatte alcune considerazioni di fondamentale importanza:

- Il file in questione verrà prodotto da Passweb nel momento stesso in
  cui verrà effettuata la chiamata all' url indicato, per cui il suo
  contenuto sarà sempre aggiornato in maniera automatica

- All'interno di questo file verranno inseriti automaticamente **i dati
  dei soli ordini** (no bolle e neppure fatture o preventivi) che:

  - risultano essere marcati come "**Non ancora esportati su Google
    Ads**" (colonna GADS nella maschera "Lista Ordini" marcata con una
    X)

![Videate\\ordine_non_esportato_su_ads.bmp](./assets/media/image29.png)

- si trovano in uno dei seguenti stati: **Memorizzato**, **Sospeso**,
  **Evaso**

<!-- -->

- Tutti gli ordini inseriti all'interno di questo file verranno poi
  marcati automaticamente come "**Già esportati su Google Ads**"
  (colonna GADS nella maschera "Lista Ordini" marcata con un check
  verde) in maniera tale da non essere poi inseriti nel file prodotto a
  seguito della successiva chiamata evitando così di importare più volte
  i dati di una stessa conversione

![Videate\\ordine_esportato_su_ads.bmp](./assets/media/image28.png)

> **ATTENZIONE!** per maggiori informazioni in merito a come viene
> gestito lo stato di esportazione di un ordine verso Google Ads si veda
> quanto indicato all'interno del capitolo "*Ordini -- Ordini --
> Gestione Ordini*" di questo manuale

- Il file contenente i dati delle conversioni da importare su Google Ads
  avrà una struttura del tipo di quella di seguito indicata

> *Parameters:TimeZone=+0100*
>
> *Email,Phone Number,Conversion Name,Conversion Time,Conversion
> Value,Conversion Currency,Ad User Data,Ad Personalization,Order
> ID,Google Click ID*
>
> *4320a7f0c1410f644da83b6601b44dbcb3f45922d1826a112b24a67126b52ca8,2b937f7cd69b540584db1a0529e555b60e37755e23c25e26a5285490ebb4ff16,Acquisto
> Online,2020-11-17T09:51:48,1000.00,EUR,Granted,Granted,5232,*
>
> ...
>
> dove la colonna:

- **Email**: contiene l'email hashata dell'utente che ha effettuato il
  relativo ordine

- **Phone Number**: contiene il numero di telefono hashato dell'utente
  che ha effettuato il relativo ordine

- **Conversion Name:** contiene il valore impostato in corrispondenza
  del campo "**Nome azione conversione**" presente alla pagina "Sito --
  Preferenze" del Wizard (tab "**Tracciamento Dati**" sezione "**Google
  Ads**")

> **ATTENZIONE!** è di fondamentale importanza che il nome inserito
> all'interno di questo campo coincida esattamente, anche a livello di
> spazi, lettere maiuscole e minuscole, con quello assegnato su Ads alla
> relativa azione di conversione

- **Conversion Value:** contiene il totale del relativo ordine

- **Conversion Currency**: contiene la valuta (in formato ISO) in uso al
  relativo ordine

- **Ad User Data** / **Ad Personalization**: contiene lo stato (Granted
  o Denied) dei relativi consensi marketing prestati dall'utente nel
  momento di creazione dell'ordine

- **Order ID**: contiene l'identificativo Passweb del relativo ordine

- **Google Click ID**: contiene l'eventuale valore del gclid nel momento
  in cui è stato creato l'ordine

> **ATTENZIONE!** la presenza o meno del gclid nel file di esportazione
> verso Google Ads dipende prima di tutto da come è stato settato il
> parametro "Inserisci GCLID export csv" alla pagina "Sito --
> Preferenze" del Wizard (tab "Tracciamento Dati" sezione "Google Ads")
> e poi, ovviamente, anche dal fatto che l'ordine in esame sia stato
> effettivamente generato a seguito di una visita generata da un primo
> click su di un annuncio Google Ads

Infine nel momento in cui, per qualsiasi ragione, dovesse andare storto
qualcosa nell'upload schedulato dei dati delle conversioni offline o
dovesse sorgere l'esigenza di effettuare degli import manuali su Ads dei
dati di conversione legati a determinati documenti, Passweb mette a
disposizione dell'utente la possibilità di effettuare in un qualsiasi
momento l'export dei dati richiesti all'interno di un file csv,
strutturato esattamente come quello prodotto in automatico, che potrà
essere scaricato in locale sul proprio pc e successivamente uplodato in
Ads mediante la relativa procedura.

Per quel che riguarda l'export di questi file csv sarà sufficiente agire
dalla maschera "**Esportazione Ordini**" del Wizard selezionando come
"**Tipologia di esportazione**" l'opzione "**Google Ads**" e impostando
il filtro di selezione dei documenti da inserire all'interno del file
(per maggiori informazioni in merito si veda quanto indicato all'interno
del capitolo "*Ordini -- Ordini -- Gestione Ordini -- Esportazione
Ordini*" di questo manuale).

Per quel che riguarda infine la procedura di import manuale su Ads di
questi file sarà sufficiente:

1.  Accedere all'account Google Ads, portarsi alla sezione "**Obiettivi
    -- Caricamenti** "

![Videate\\conversioni_offline_14.bmp](./assets/media/image40.png)

> e, da qui cliccare sul pulsante raffigurante un piccolo **+** per
> avviare un nuovo caricamento manuale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_15.bmp](./assets/media/image41.png)

2.  Cliccare quindi sul menu a tendina "**Seleziona origine**" e
    selezionare tra le opzioni proposte la voce "**Carica un file**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_16.bmp](./assets/media/image42.png)

3.  A questo punto sarà sufficiente cliccare sul pulsante "Seleziona un
    file dal tuo computer" e selezionare il file precedentemente
    esportato da Passweb e salvato in locale sul proprio pc.

> Sarà inoltre necessario flaggare anche il check mediante il quale
> confermiamo che i dati presenti all'interno del file che andremo ad
> importare sono stati raccolti secondo le norme previste da Google

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_17.bmp](./assets/media/image43.png)

4.  Infine, considerando quella che è la struttura del file prodotto da
    Passweb dovremo anche selezionare tra le due opzioni proposte quella
    relativa a "**Dati sottoposti ad hashing**"

![Videate\\conversioni_offline_18.bmp](./assets/media/image44.png)

5.  Il pulsante "**Applica**" presente nella parte bassa di questa
    maschera consentirà di avviare la procedura di import

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\conversioni_offline_19.bmp](./assets/media/image45.png)
