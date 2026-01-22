# CAUSALI DOCUMENTO



La sezione **"Causali Documento"**, disponibile solo per Ecommerce
Mexal, consente di gestire e personalizzare tutte le causali documento
definite all'interno del gestionale ed esportate anche all'interno del
proprio sito Ecommerce.

Una volta effettuato l'accesso a questa sezione del Wizard verrà quindi
visualizzata la maschera "**Lista Causali Documento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_causali_documento.bmp](./assets/media/image715.png){width="5.545138888888889in"
height="3.1881944444444446in"}

contenente l'elenco delle causali definite, in Mexal, all'interno della
tabella "**Causali movimenti magazzino**" (*Magazzino -- Tabelle
Generali*)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_tabella_causali_documento.bmp](./assets/media/image716.png){width="5.616666666666666in"
height="3.3048611111111112in"}

I pulsanti presenti nella contestuale barra degli strumenti consentono,
rispettivamente di:

**Attiva / Disattiva Causale**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_causale.bmp](./assets/media/image717.png){width="0.5652777777777778in"
height="0.18819444444444444in"} /
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_disattiva_causale.bmp](./assets/media/image718.png){width="0.6819444444444445in"
height="0.18819444444444444in"} ): consente di attivare / disattivare la
causale documento selezionata in elenco (le causali documento attivate
sono evidenziate in grassetto).

**ATTENZIONE!** Le causali abilitate potranno essere visualizzate e
selezionate sul front end del sito, in fase di checkout, all'interno
della sezione relativa ai "**Parametri Documento**"

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image675.png){width="0.3958333333333333in"
height="0.18819444444444444in"} ): consente di personalizzare la causale
documento attualmente selezionata. Cliccando su questo pulsante verrà
infatti visualizzata la maschera "**Modifica Causale Documento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\modifica_causale_documento.bmp](./assets/media/image719.png){width="5.545138888888889in"
height="3.1881944444444446in"}

all'interno della quale poter specificare un valore per i seguenti
parametri:

- **Numero** -- **campo in sola visualizzazione**: consente di
  visualizzare l'identificativo della causale all'interno della relativa
  tabella Mexal

- **Stato della Causale Documento**: consente di attivare / disattivare
  la causale documento in esame

- **Gestisci**: consente di decidere se la causale in esame, una volta
  attivata, dovrà poi essere mostrata sul front end del sito, in fase di
  checkout, solo in relazione ai documenti di tipo ordine, solo in
  relazione ai documenti di tipo preventivo o in entrambi i casi
  (opzione "Sempre")

- **Descrizione**: consente di personalizzare, in tutte le lingue
  attualmente gestite all'interno del sito, la descrizione della causale
  in esame.

> In questo senso è bene sottolineare anche il fatto che la descrizione
> delle causali documento, in quella che è la lingua impostata come
> "**Lingua installazione**" nei parametri di configurazione del sito
> (pagina "*Configurazione Gestionale*" del Wizard ), è controllata dal
> parametro "**Tabella Causali Documento**" presente in corrispondenza
> della sezione "**Aggiornamento descrizioni in italiano dal
> Gestionale**" alla pagina "**Parametri di Sincronizzazione**" del
> Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sincronizzazione_descrizione_tabella_causali.bmp](./assets/media/image720.png){width="5.545138888888889in"
height="3.8048611111111112in"}

> In sostanza dunque, nel caso in cui il parametro evidenziato in figura
> dovesse essere selezionato, in fase di sincronizzazione le descrizioni
> delle causali documento nella lingua di installazione (tipicamente la
> lingua italiana) verranno sovrascritte con quanto presente nei
> corrispondenti campi della tabella Mexal.
>
> Nel momento in cui l'esigenza dovesse essere invece quella di non
> modificare eventuali personalizzazioni apportate alle descrizioni
> delle causali documento nella lingua di installazione, **sarà
> necessario verificare di non aver attivato il parametro evidenziato in
> figura**
>
> In ogni caso il parametro in questione ha effetto solo ed
> esclusivamente per le descrizioni di causali documento già esportate e
> gestite all'interno del sito. In conseguenza di ciò tutte le nuove
> causali documento verranno importate, alla prima sincronizzazione
> utile, con la stessa descrizione per esse impostata all'interno del
> gestionale
>
> **ATTENZONE!** le descrizioni delle causali documento in lingue
> diverse dalla lingua di installazione potranno essere personalizzate
> solo ed esclusivamente all'interno del Wizard di Passweb e non
> verranno, in nessun caso, sovrascritte a seguito di sincronizzazioni
> sito -- gestionale.

**Importa** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa.bmp](./assets/media/image368.png){width="0.3506944444444444in"
height="0.175in"} ): consente di personalizzare e configurare in maniera
massiva, mediante l'importazione di un apposito file csv / txt, tutte le
causali documento attualmente gestite all'interno del sito

Cliccando su questo pulsante verrà infatti aperta la maschera di
importazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_causali_documento.bmp](./assets/media/image721.png){width="5.545138888888889in"
height="3.8048611111111112in"}

all'interno della quale poter indicare:

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  i dati delle causali documento da configurare

- **Lingua:** consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati delle causali documento presenti all'interno
  del file di importazione

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta,
consentendo a Passweb di andare poi a configurare le causali documento
secondo quanto indicato all'interno del file, è necessario che il file
di importazione sia stato creato rispettando determinate regole. Nello
specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180**.

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, doppi apici e/o lo stesso
> carattere utilizzato anche come separatore **sia necessariamente
> racchiuso da virgolette**

- Il file di importazione potrà contenere i seguenti campi:

  - **numero** (campo obbligatorio): numero identificativo della causale
    documento (corrispondente all'identificativo della causale stessa
    all'interno della relativa tabella mexal)

  - **isAbilitata:** campo booleano che consente di indicare se la
    relativa causale documento dovrà o meno essere abilitata. I valori
    accettati sono "**SI**" e "**NO**"

  - **gestione:** campo che consente di indicare se la relativa causale
    dovrà essere utilizzata in relazione ai soli ordini, ai soli
    preventivi o per entrambe le tipologie di documenti. I valori
    accettati sono:

    - **0:** corrispondente all'opzione "**Sempre**". La causale
      documento sarà quindi utilizzabile sia per gli ordini che per i
      preventivi

    - **1:** corrispondente all'opzione "**Escludi** **Preventivi**". La
      causale documento sarà quindi utilizzabile solo per i documenti di
      tipo Ordine

    - **2:** corrispondente all'opzione "**Escludi** **Ordini**". La
      causale documento sarà quindi utilizzabile solo per i documenti di
      tipo Preventivo

  - **descrizione:** consente di indicare, nella lingua del file di
    importazione, la descrizione da utilizzare per la relativa causale
    documento

> Supponendo dunque di aver impostato come carattere di separazione il ;
> un possibile esempio di file di importazione potrebbe essere il
> seguente:
>
> *numero;isAbilitata;gestione;descrizione*
>
> *2;SI;0;Acquisti Speciali*
>
> *1;SI;0;Acquisti Web*
>
> *3;SI;0;Acquisto con condizioni Categoria A*
>
> *4;SI;0;Preventivi web*
>
> *5;NO;0;Condizioni Extra*

**Esporta** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image311.png){width="0.31805555555555554in"
height="0.1625in"} ): consente di esportare le configurazioni delle
casuali documento all'interno di un file .csv.

Cliccando su questo pulsante verrà infatti visualizzata la maschera di
esportazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_causali_documento.bmp](./assets/media/image722.png){width="5.545138888888889in"
height="3.201388888888889in"}

All'interno della quale poter indicare:

- **Lingua:** consente di indicare la lingua in relazione alla quale
  esportare le configurazione delle causali documento in elenco

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che dovrà essere utilizzato all'interno
  del file come separatore per i vari campi

Dal punto di vista del loro utilizzo, come già evidenziato all'interno
di questo capitolo, tutte le causali documento attivate potranno poi
essere selezionate sul front end del sito, direttamente in fase di
checkout dipendentemente dalla tipologia di documento considerata e,
soprattutto, dipendentemente dal fatto di aver attivato o meno la
visualizzazione della sezione relativa ai "Parametri Documento"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_causale_documento.bmp](./assets/media/image723.png){width="5.545138888888889in"
height="3.792361111111111in"}

Nello specifico dunque la sezione "Casuale Documento" evidenziata in
figura potrà essere effettivamente visualizzata all'interno del checkout
solo nel momento in cui si sia deciso di impostare il campo
"**Visualizza Parametri Documento**" su una delle opzioni "**Agente**" o
"**Agente e Cliente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_causale_documento_2.bmp](./assets/media/image724.png){width="5.00625in"
height="3.3180555555555555in"}

Il testo dell'etichetta "Causale Movimento" può essere personalizzato
alla pagina "Testi Messaggi Sito" del Wizard agendo per il componente
"Checkout" in corrispondenza dell'elemento "Causale Documento"

Per quel che riguarda invece le causali presenti all'interno del menu a
tendina la descrizione visualizzata corrisponde, ovviamente, a quella
impostata in fase di configurazione della causale stessa e la presenza o
meno di una delle causali attive all'interno di questo menu a tendina
può dipendere anche dalla tipologia di documento attualmente
considerata.

Infine è bene sottolineare anche che, tra tutte le opzioni disponibili,
all'interno del menu a tendina verranno visualizzate a default
(ovviamente se correttamente attivate) le causali impostate alla pagina
"Configurazione Ordini" del Wizard in corrispondenza dei parametri
"**Numero Causale Movimento di Magazzino Documento**" e "**Numero
Causale Movimento di Magazzino Preventivo**" (la prima nel caso in cui
il documento generato sia un ordine, la seconda nel momento in cui il
documento generato dovesse invece essere un preventivo)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\selezione_causale_documento_default.bmp](./assets/media/image725.png){width="5.545138888888889in"
height="4.545138888888889in"}

**In ogni caso, nel momento in cui si dovesse decidere di gestire la
selezione lato front end delle causali, in fase di salvataggio
all'interno del gestionale il relativo documento mexal verrà generato
esattamente con la causale selezionata dall'utente in fase di
checkout.**

