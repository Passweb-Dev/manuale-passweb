# ORDINI -- GESTIONE ALLEGATI



Nel caso in cui l'esigenza dovesse essere quella di fornire agli utenti
la possibilità di allegare determinati documenti agli ordini effettuati
all'interno del sito, sarà necessario, per prima cosa, impostare il
parametro "**Gestione Allegati**" presente nella maschera di
configurazione del componente **Ordine (Checkout)** sul valore **SI**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\allegati_ordine_1_res.bmp](./assets/media/image322.png)

In queste condizioni verranno infatti visualizzati altri parametri
mediante i quali poter definire esattamente come dovranno essere
gestiti, in fase di ordine, eventuali allegati.

Nello specifico il parametro:

- **Dimensione Massima Allegato**: consente di indicare la dimensione
  massima (in byte) che potrà avere ogni singolo file allegato
  all'ordine.

> **ATTENZIONE!** Nel caso in cui il campo in esame dovesse essere
> lasciato vuoto non verrà effettuato nessun controllo sulla dimensione
> degli allegati. Per evitare problemi relativi ad eventuali mail che
> dovranno poi contenere tali allegati è quindi consigliabile impostare
> sempre una dimensioni massima.

- **Estensioni Consentite Allegato:** consente di indicare le estensioni
  che andranno poi a definire i tipi di file che potranno essere
  effettivamente allegati all'ordine. Nel caso in cui si voglia dare
  agli utenti la possibilità di allegare file di diverso tipo (es.
  documenti Word, file Excel, file Pdf ...) le singole estensioni
  dovranno essere separate da virgola.

> Come per le dimensioni massime, anche in questo caso, è sempre
> consigliabile indicare esattamente i tipi di file che potranno essere
> allegati agli ordini
>
> **ATTENZIONE!** Indipendentemente da quanto impostato all'interno del
> campo in esame non sarà mai possibile allegare agli ordini file con le
> seguenti estensioni: **.exe, .vb, .aspx, .asp, .jsp**

- **Numero minimo di Allegati:** consente di impostare il numero minimo
  di file che dovranno essere allegati ad ogni singolo ordine.

> Se il campo in oggetto dovesse essere lasciato vuoto non verrà
> effettuato nessun tipo di controllo. In queste condizioni sarà quindi
> possibile concludere l'ordine senza dover per forza di cose allegare
> determinati documenti.
>
> Al contrario, nel momento in cui il parametro in esame dovesse essere
> impostato su di un valore maggior di zero, **per portare a termine
> l'ordine sarà obbligatorio** allegare ad esso un numero di file
> maggiore o uguale al numero indicato all'interno di questo campo.

- **Numero massimo di Allegati:** consente di impostare il numero
  massimo di file che potranno essere allegati ad ogni singolo ordine.

> Anche in questo caso se il campo in oggetto dovesse essere lasciato
> vuoto non verrà effettuato nessun tipo di controllo e gli utenti
> potranno quindi allegare ad ogni singolo ordine tutti i documenti che
> vorranno (coerentemente sempre con eventuali altre limitazioni
> impostate mediante i parametri precedentemente esaminati).

- **Inserimento Allegati ordini esistenti:** consente di specificare se
  gli utenti dovranno avere o meno la possibilità di allegare file anche
  a documenti già presenti all'interno del sito.

> Nel caso in cui il parametro in esame non dovesse essere selezionato,
> sarà quindi possibile gestire degli allegati solo ed esclusivamente su
> nuovi ordini.

- **Rimozione Allegati ordini esistenti:** consente di specificare se
  gli utenti dovranno avere o meno la possibilità di eliminare eventuali
  allegati relativi ad ordini già registrati.

> **ATTENZIONE!** affinché un utente del sito possa effettivamente
> eliminare un file allegato all'ordine da Wizard (e quindi
> dall'amministratore del sito) non è sufficiente selezionare il
> parametro in esame ma è necessario accertarsi anche che sul singolo
> file allegato sia stato selezionato il check "**Consenti rimozione
> utente**"
>
> Per maggiori informazioni relativamente a come poter gestire eventuali
> allegati all'ordine direttamente dal Wizard di Passweb, si veda anche
> la corrispondente sezione ("*Ordini -- Gestione Ordini -- Allegati
> Ordine*") di questo manuale

Una volta attivata e configurata la gestione degli allegati, in fase di
ordine comparirà, all'interno del componente Checkout, una nuova sezione
all'interno della quale poter gestire l'upload dei file.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\allegati_ordine_2_res.bmp](./assets/media/image323.png)

Il pulsante "**Seleziona file da allegare**" consente di selezionare il
file da uplodare e allegare al documento.

Nel caso in cui il numero di allegati dovesse essere uguale al numero
massimo impostato in fase di configurazione del componente il pulsante
"Seleziona file da allegare" verrà automaticamente nascosto. In queste
condizioni per poter allegare un nuovo file sarà quindi necessario per
prima cosa eliminare uno degli allegati già presenti (pulsante
"**Rimuovi allegato**").

In fase di upload, nel momento in cui non dovessero essere soddisfatte
alcune delle condizioni impostate (es. tipi di file gestiti, dimensione
massima dei file da allegare ecc...) verrà visualizzato un apposito
messaggio di errore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\allegati_ordine_3_res.bmp](./assets/media/image324.png)

Per ciascuno dei file allegati al documento verrà indicata la data di
upload ed il nome del file; il campo "**Nota**" consentirà infine di
assegnare a ciascun allegato una specifica nota.

Nel caso in cui l'esigenza dovesse essere quella di offrire agli utenti
del sito la possibilità di allegare documenti anche ad ordini
preesistenti (oltre che ovviamente in fase di creazione di un nuovo
ordine) sarà necessario verificare, per prima cosa, di aver
correttamente selezionato in fase di configurazione, il parametro
"**Inserimento Allegati ordini esistenti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\allegati_ordine_4_res.bmp](./assets/media/image325.png)

In queste condizioni infatti, andando a visualizzare il dettaglio di un
ordine già registrato comparirà, in coda ad eventuali allegati già
presenti sull'ordine, anche il pulsante "**Gestisci Allegati**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\allegati_ordine_5_res.bmp](./assets/media/image326.png)

Cliccando su questo pulsante sarà quindi possibile aggiungere nuovi
allegati, rimuovere eventuali file precedentemente allegati al documento
stesso e/o variarne la relativa nota, il tutto ovviamente sempre in
accordo con i parametri di configurazione precedentemente impostati.

**ATTENZIONE!** in fase di visualizzazione del dettaglio di un documento
il pulsante "Gestisci Allegati" verrà visualizzato solo ed
esclusivamente al verificarsi di almeno una delle condizioni di seguito
elencate:

- **E' consentito l'inserimento di nuovi allegati**. Il parametro
  "Inserimento Allegati ordini esistenti" deve essere selezionato e il
  numero di allegati già presenti sul documento deve essere inferiore al
  numero massimo di allegati gestibili.

- **E' ammessa la rimozione di eventuali allegati al documento**. Il
  parametro "Rimozione Allegati ordini esistenti" deve essere
  selezionato e almeno uno degli allegati presenti sul documento può
  effettivamente essere eliminato.

- **Il documento in esame ha degli allegati uplodati direttamente dagli
  utenti del sito** ed esiste quindi la possibilità di variarne la
  relativa nota.

Per quel che riguarda **eventuali file allegati ad un ordine operando
direttamente all'interno del gestionale (e partendo quindi da
Docuvision)** -- Siti E-commerce collegati a Mexal -- è bene
sottolineare che tali file non potranno mai, ovviamente, essere
eliminati dagli utenti del sito e, allo stesso modo anche
l'amministratore del sito operando direttamente dal Wizard di Passweb
non avrà la possibilità ne di eliminarli ne tanto meno di variarli a
livello di titolo, descrizione e/o nota. Gli allegati Docuvision, in
sostanza possono essere gestiti solo ed esclusivamente operando
all'interno del gestionale.

Allo stesso modo, e per ovvie ragioni, è bene sottolineare anche che la
gestione degli allegati da front end (e quindi da parte degli utenti del
sito) riguarda solo ed esclusivamente documenti di tipo OC/OX e PR/PX.
**Su documenti di tipo Bolla o Fattura non sarà mai possibile, operando
da front end, rimuovere eventuali file allegati al documento stesso né
tanto meno aggiungerne di nuovi.**

Anche l'amministratore del sito ha la possibilità, come precedentemente
evidenziato, di aggiungere eventuali allegati ad uno specifico documento
potendo scegliere di effettuare questo tipo di operazione in due modi
diversi:

- Operando direttamente all'interno del gestionale, andando quindi ad
  inserire eventuali allegati direttamente in Docuvision (solo Ecommerce
  Mexal)

- Operando direttamente all'interno del Wizard del proprio sito Passweb

In questo senso verranno quindi applicate determinate regole di
gestione.

Nello specifico:

- Eventuali file allegati ad un documento operando direttamente
  all'interno del gestionale (Docuvision) potranno essere gestiti solo
  ed esclusivamente all'interno del gestionale stesso. Ne
  l'amministratore del sito ne tanto meno gli utenti del sito stesso
  avranno mai la possibilità, quindi, di variare e/o eliminare questo
  tipo di allegati operando direttamente da Passweb.

- Eventuali file allegati ad un documento direttamente dagli utenti del
  sito, partendo quindi dal Front End del sito stesso, non potranno
  essere modificati all'interno del Wizard. L'amministratore del sito
  potrà, eventualmente, eliminare tali file ma non potrà modificarli in
  alcun modo.

<!-- -->

- Eventuali file allegati ad un documento da parte dell'amministratore
  del sito operando direttamente dal Wizard di Passweb potranno sempre
  essere modificati e/o eliminati dall'amministratore stesso. Gli utenti
  del sito avranno invece la possibilità di eliminare tali file solo al
  verificarsi delle seguenti condizioni:

  - è stato correttamente selezionato il campo "**Rimozione Allegati
    ordini esistenti**" (parametri di configurazione del componente
    Ordine)

  - in fase di upload, l'amministratore del sito ha selezionato per essi
    il parametro "**Consenti rimozione utente**"

<!-- -->

- **Eventuali file allegati ad un documento partendo da Passweb (Back
  end o Front end non fa differenza) non verranno mai inseriti
  all'interno del gestionale, resteranno legati allo specifico
  documento,** e potranno quindi essere gestiti, secondo le regole
  precedentemente elencate, solo ed esclusivamente all'interno di
  Passweb.

> **ATTENZIONE! In conseguenza di ciò, a seguito della trasformazione di
> un documento da una tipologia ad un'altra (es. passaggio da ordine a
> bolla / fattura), eventuali allegati presenti sul documento di
> partenza andranno persi**
>
> Nel caso in cui l'esigenza dovesse essere quella di mantenere uno
> storico dei documenti allegati da Passweb (Back end o Front end non fa
> differenza) ad un ordine, è quindi consigliabile salvarsi localmente
> tali allegati (inserendoli magari all'interno di Docuvision) prima
> della trasformazione dell'ordine in bolla / fattura.

Per maggiori informazioni relativamente a come poter allegare file ad un
ordine operando direttamente dal Wizard del proprio sito Passweb e/o su
come configurare l'ambiente in modo tale da far si che eventuali
allegati ad un ordine vengano inseriti anche nelle mail connesse ai vari
stati del documento stesso si faccia riferimento a quanto indicato
all'interno delle sezioni "*Ordini -- Configurazione Ordini -- Dati
Email*" e "*Ordini -- Gestione Ordini -- Allegati Ordine*" di questo
manuale.

