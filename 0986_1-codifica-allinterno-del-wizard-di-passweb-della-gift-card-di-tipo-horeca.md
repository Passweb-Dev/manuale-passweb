# 1 -- CODIFICA ALL'INTERNO DEL WIZARD DI PASSWEB DELLA GIFT CARD DI TIPO HO.RE.CA.



In questa fase sarà necessario portarsi all'interno della sezione
"**Utenti -- Gift Card**" del Wizard e cliccare sul pulsante "**Aggiungi
Gift Card**" presente nella barra degli strumenti della maschera
"**Lista delle Gift Card**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_1.bmp](./assets/media/image335.png)

In questo modo verrà infatti visualizzata la maschera "**Nuova Gift
Card**" all'interno della quale poter impostare tutti i parametri di
configurazione della Gift Card che si intende effettivamente codificare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_2.bmp](./assets/media/image336.png)

**ATTENZIONE!** I parametri presenti all'interno di questa sezione
variano in relaziona alla specifica tipologia di Gift Card considerata

Dopo aver impostato il parametro "**Tipologia**" sul valore HoReCa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_3.bmp](./assets/media/image337.png)

sarà quindi necessario configurare correttamente anche i seguenti campi:

- **Nome:** consente di impostare il nome identificativo della Gift Card
  in esame, in maniera tale da poterla poi distinguere tra tutte le
  altre presenti in elenco

- **Serie:** serie del Buono Sconto che verrà creato su Beauty
  contestualmente all'inserimento di un ordine da web contenente almeno
  un articolo di tipo "Ricarica Promozione" e / o un Trattamento gestito
  come Gift Card.

> La Serie indicata all'interno di questo campo è di fondamentale
> importanza inquanto assieme al Codice del Buono Sconto che verrà poi
> creato su Beauty andrà, tipicamente, a comporre il codice della Gift
> Card che gli utenti dovranno poi utilizzare sul sito o direttamente
> nel punto vendita per poter usufruire del relativo sconto.
>
> Il campo "Serie" è alfanumerico e accetta un numero massimo di 30
> caratteri.
>
> **ATTENZIONE! Si consiglia di utilizzare un numero di caratteri uguale
> a quello impostato per il campo Serie in fase di configurazione del
> codice a barre su Beauty**
>
> In caso contrario, nel momento in cui dovesse essere impostata una
> Serie con un numero di caratteri maggiore di quello definito su
> Beauty, in fase di creazione del codice a barre la Serie impostata su
> Passweb verrebbe troncata.

- **Durata (giorni):** consente di impostare il numero di giorni di
  validità del Buono Sconto creato all'interno di Beauty a seguito
  dell'inserimento di un ordine contente almeno una "Ricarica
  Promozione" e/o un Trattamento gestito come una Gift Card.

> Il numero di giorni impostato all'interno di questo campo determinerà
> dunque il valore inserito all'interno del campo "**Scadenza**"
> presente nella maschera di configurazione del relativo Buono Sconto di
> Beauty

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_4.bmp](./assets/media/image338.png)

> Supponendo di aver impostato il campo in oggetto sul valore 30 il
> Buono Sconto creato su Beauty a seguito di un ordine web effettuato in
> data 24 Settembre 2023 avrà quindi una scadenza impostata
> automaticamente sul 24 Ottobre 2023

Per completare la creazione della Gift Card HoReCa sarà poi necessario
configurare correttamente anche la **mail di Attivazione** (tab "**Dati
Email**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_5.bmp](./assets/media/image339.png)

e il Template da utilizzare per la creazione di questa stessa mail (tab
"**Template**")

In particolare **in fase di configurazione del Template della mail di
Attivazione sarà di fondamentale importanza verificare di aver inserito
correttamente il segnaposto relativo al "Codice Gift Card".**

In caso contrario infatti l'acquirente non avrà a disposizione il codice
da utilizzare sul sito e/o in negozio per poter effettivamente
utilizzare la Gift Card acquistata.

![Videate\\gift_card_horeca_6.bmp](./assets/media/image340.png)

Oltre al segnaposto relativo al Codice della Gift Card è sempre buona
norma inserire all'interno del Template della mail di attivazione anche
il segnaposto "**Trattamento**" e/o "**Link Trattamento**".

Il primo verrà infatti sostituito, in fase di generazione della mail,
con il titolo del trattamento acquistato. Il secondo consentirà invece
di inserire all'interno della mail di attivazione un link diretto alla
pagina del sito relativa allo specifico trattamento in relazione al
quale è stato generato il codice sconto presente all'interno della
stessa mail.

**ATTENZIONE!** Per le Gift Card di tipo HoReCa. non è gestita la mail
di Scadenza, per cui eventuali notifiche sulla scadenza di un Buono
Sconto, scadenza questa, per altro, modificabile direttamente
all'interno del gestionale, dovranno essere inviate dal gestionale
stesso.

Per maggiori informazioni relativamente alla Mail di Attivazione e alla
costruzione del Template di questa stessa mail si rimanda a quanto
indicato all'interno dei precedenti capitoli di questo manuale ("*Gift
Card -- Dati Email*" e "*Gift Card -- Template*")

**ATTENZIONE!** Si ricorda anche che **è possibile creare una sola Gift
Card di tipo Ho.Re.Ca**. Nel momento in cui si dovesse tentare di creare
una seconda Gift Card di questo tipo verrà quindi visualizzato un
messaggio di errore del tipo di quello evidenziato nell'immagine di
seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gift_card_horeca_7.bmp](./assets/media/image341.png)

