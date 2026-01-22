# ACQUISTI CON CONSEGNA A DOMICILIO



Dopo aver codificato le diverse tipologie di consegna a domicilio
indicando per ciascuna di esse le relative regole di preparazione e di
consegna e, soprattutto, dopo averle associate alle modalità di
spedizione gestite all'interno del sito, tutta la parte di front end
sarà gestita in maniera automatica all'interno del componente "Checkout
Custom"

In questo senso dunque nel momento in cui, in fase di checkout, l'utente
dovesse selezionare una modalità di spedizione per cui è prevista la
consegna a domicilio, gli verrà automaticamente visualizzato un primo
campo (obbligatorio) all'interno del quale potrà indicare esattamente il
giorno in cui desidera ricevere la merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_1.bmp](./assets/media/image380.png){width="5.038888888888889in"
height="3.545138888888889in"}

I giorni effettivamente selezionabili all'interno del calendario
dipenderanno:

- Da quanto impostato, in fase di configurazione della relativa
  consegna, per il campo "**Numero massimo di giorni**"

- Da eventuali regole di eccezione in cui sono stati specificati giorni
  per i quali non si effettuano consegne a domicilio

- Dal fatto che per un dato giorno sia già stata raggiunta o meno
  l'eventuale quota massima di consegne previste per la giornata
  (parametro "**Quota limite giornaliera**")

Dopo aver selezionato uno dei giorni disponibili a calendario verrà
visualizzato un ulteriore campo all'interno del quale l'utente potrà
selezionare, tra quelli disponibili, l'intervallo orario in cui
desidererebbe ricevere la merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_2.bmp](./assets/media/image402.png){width="5.038888888888889in"
height="3.545138888888889in"}

Gli intervalli orari selezionabili in questa fase dipenderanno:

- Da quanto impostato per le regole di tipo "**Intervallo Orario**"
  definite per la consegna in esame

<!-- -->

- Dal fatto che per un determinato intervallo sia già stata raggiunta o
  meno l'eventuale quota massima di consegne previste per quello stesso
  intervallo (parametro "**Quota limite intervallo orario**")

<!-- -->

- Dall'ora in cui viene effettuato l'ordine e da quanto impostato, in
  fase di configurazione della consegna, per i parametri "**Ore
  Preparazione**" e "**Ore Consegna**"

> Nel caso in cui, ad esempio, la data di consegna sia riferita al
> giorno corrente, eventuali intervalli orari precedenti l\'ora attuale
> saranno comunque mostrati all'interno della select ma non potranno
> essere selezionati.
>
> **ATTENZIONE!** Nel caso in cui non fosse possibile selezionare
> nessuno degli intervalli orari previsti verrà mostrato un messaggio
> per notificare al cliente di selezionare un altro giorno tra quelli
> disponibili a calendario.
>
> Il testo del messaggio in questione è modificabile dalla sezione
> "Testi/Messaggi del Sito" agendo sulla voce "Consegna - Intervallo
> orario non disponibile" del componente "Checkout Custom".

**ATTENZIONE!** La possibilità da parte dell'utente di selezionare il
giorno e l'intervallo orario in cui desidera ricevere la merce così come
il fatto di visualizzare soltanto data e orario di prevista consegna
senza poter variare in alcun modo queste informazioni dipende dalle
impostazioni settate per il parametro "**Gestione Calendario**" presente
nella maschera di configurazione della consegna in esame (per maggiori
informazioni in merito si veda anche quanto indicato all'interno del
precedente capitolo "*Consegne*" di questo manuale)

Una volta confermato l'ordine, la data e l'intervallo orario selezionati
(o semplicemente mostrati al) dal cliente verranno visualizzati:

- nel riepilogo del documento all'interno del box relativo alla
  spedizione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_3.bmp](./assets/media/image403.png){width="5.038888888888889in"
height="3.545138888888889in"}

- nel dettaglio di Ordini/Bolle/Fatture in Area Riservata, nelle Stampe
  e nelle varie Email inviate in automatico dall'applicazione in
  relazione ai diversi stati ordine, a patto però di aver inserito gli
  appositi segnaposto "**Data Consegna**" e "**Ora Consegna**"
  all'interno del campo "Dettaglio" nella sezione "Documento" della
  maschera di "Configurazione Ordini"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_4.bmp](./assets/media/image404.png){width="5.792361111111111in"
height="3.545138888888889in"}

> Per maggiori informazioni in merito al campo "Dettaglio" si veda anche
> quanto indicato nel successivo capitolo "Ordini -- Configurazione
> Ordini -- Documento" di questo manuale

Infine, per quel che riguarda il documento inserito all'interno del
gestionale, le informazioni relative alla data e all'ora di consegna
verranno inserite come nota di corpo del relativo documento con
indicato: **#Consegna \<data\> \<intervallo orario\>#**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_5.bmp](./assets/media/image405.png){width="5.220833333333333in"
height="2.6166666666666667in"}

Inoltre i campi Data e Ora di inizio trasporto presenti nel piede del
documento gestionale verranno valorizzati automaticamente con la data
indicata per la consegna e, se presente, con l\'orario iniziale
dell\'intervallo selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_acquisto_6.bmp](./assets/media/image406.png){width="4.104166666666667in"
height="1.8569444444444445in"}

Per organizzare al meglio le consegne sarà quindi possibile:

- ordinare i documenti presenti all'interno del gestionale per data di
  inizio trasporto

- tenere sotto controllo la pagina "Lista Ordini" del Wizard filtrandola
  magari per "data di consegna"

**ATTENZIONE!** Eventuali variazioni fatte, lato gestionale, alla data e
all\'ora di inizio trasporto non verranno riportate sul sito.

In questo senso quindi, farà fede sempre e soltanto quanto indicato dal
cliente in fase di checkout.

