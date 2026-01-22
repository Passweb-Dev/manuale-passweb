# PARAMETRI DI CONFIGURAZIONE



Per ciascun Costo associato ad una determinata Spesa Accessoria è
possibile impostare i seguenti parametri di configurazione:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_costo.bmp](./assets/media/image430.png){width="5.779166666666667in"
height="3.5256944444444445in"}

**Descrizione:** etichetta identificativa del costo che si sta
codificando

**Valuta di Riferimento:** consente di selezionare, tra quelle gestite
all\'interno del sito, la specifica valuta in cui dovranno essere
considerati gli importi relativi al costo in oggetto.

**Scaglioni e Calcolo Percentuale**: permette di specificare l'unità di
misura sulla base della quale verranno definiti i vari scaglioni nel
caso di Costi di tipo Tabellare e la base di calcolo (**Totale Merce o
Imponibile**) da utilizzare per la determinazione dei valori in
percentuale.

Nello specifico poi, per quel che riguarda i valori di Totale Merce e
Imponibile utilizzati per determinare in quale scaglione si ricade, ed
eventualmente anche l'importo dello scaglione stesso occorre sempre
ricordare che:

- Totale Merce ed Imponibile verranno considerati comprensivi o meno di
  eventuali articoli spesa inserti in carrello (a seguito
  dell'applicazione di determinate promozioni o buoni sconto)
  dipendentemente dall'impostazione scelta per il parametro "**Gestione
  Totale Merce**" presente nella sezione "*Catalogo -- Configurazione
  Parametri Catalogo*" del Wizard

- Totale Merce ed Imponibile verranno considerati **sempre al netto di
  eventuali articoli di tipo "Gift Card" inseriti in ordine**. In
  conseguenza di ciò possiamo quindi affermare che eventuali Gift Card
  (sia Fisiche che Virtuali) presenti in ordine non avranno alcun
  impatto né sulla determinazione dello scaglione di applicazione del
  costo, né tanto meno su quello che potrebbe essere l'importo assegnato
  a quel determinato scaglione (nel caso ovviamente di calcolo in
  percentuale)

E' possibile selezionare uno dei seguenti valori:

- **Scaglioni in base al Prezzo e Calcolo Percentuale sul Totale
  Merce**: in questo caso gli scaglioni del costo verranno definiti in
  base al Totale Merce. Il passaggio quindi da uno scaglione ad un altro
  e conseguentemente l'applicazione di uno specifico importo per il
  costo in esame dipenderà dal Totale Merce (comprensivo di IVA).

> Allo stesso modo in queste condizioni, nel caso in cui dovessero
> essere indicati, per gli importi del costo, dei valori in percentuale,
> la percentuale indicata verrà calcolata sempre sul Totale Merce
> (comprensivo di IVA)

- **Scaglioni in base all'Imponibile e Calcolo Percentuale
  sull'Imponibile:** in questo caso gli scaglioni del costo verranno
  definiti in base all'Imponibile (Totale Merce NON comprensivo di IVA).
  Il passaggio dunque da uno scaglione all\'altro, e conseguentemente
  l\'applicazione di uno specifico importo per il costo in esame,
  dipenderà dal valore dell'Imponibile (Totale Merce NON comprensivo di
  IVA).

> In queste condizioni , nel caso in cui dovessero essere indicati, per
> gli importi del costo, dei valori in percentuale, la percentuale
> indicata verrà calcolata sempre sull'Imponibile (Totale merce NON
> comprensivo di IVA)

- **Scaglioni in base al numero di Articoli e Calcolo Percentuale sul
  Totale Merce:** in questo caso gli scaglioni del costo verranno
  definiti in base al numero di articoli presenti in ordine. Il
  passaggio dunque da uno scaglione all\'altro, e conseguentemente
  l\'applicazione di uno specifico importo per il costo in esame,
  dipenderà dal numero di articoli acquistati.

> **ATTENZIONE!** Nel calcolo del numero di articoli in ordine non
> verranno considerati articoli di tipo Gift Card
>
> In queste condizioni, ovviamente, nel momento in cui dovessero essere
> indicati, per gli importi del costo, dei valori in percentuale, la
> percentuale indicata verrà calcolata sempre sul Totale Merce
> (comprensivo di IVA)

- **Scaglioni in base al numero di Articoli e Calcolo Percentuale
  sull'Imponibile:** in questo caso gli scaglioni del costo verranno
  definiti in base al numero di articoli presenti in ordine. Il
  passaggio dunque da uno scaglione all\'altro, e conseguentemente
  l\'applicazione di uno specifico importo per il costo in esame,
  dipenderà dal numero di articoli acquistati.

> **ATTENZIONE!** Nel calcolo del numero di articoli in ordine non
> verranno considerati articoli di tipo Gift Card
>
> In queste condizioni, ovviamente, nel momento in cui dovessero essere
> indicati, per gli importi del costo, dei valori in percentuale,
> indicata verrà calcolata sempre sull'Imponibile (Totale merce NON
> comprensivo di IVA)

- **Scaglioni in base al campo Personalizzato e Calcolo Percentuale sul
  Totale Merce:** in questo caso gli scaglioni del costo accessorio che
  si sta codificando potranno essere definiti, **per siti Ecommerce
  collegati a Mexal:**

  - sulla base di quanto indicato all'interno dello specifico campo
    gestionale collegato alla funzionalità Mexal **"Spese di trasporto a
    Scaglioni"**

  - sulla base del Peso indicato all'interno del relativo campo presente
    nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

  - sulla base di quanto indicato all'interno di un Attributo Articolo
    Passweb appositamente realizzato

> Nel caso invece di **siti Ecommerce collegati ad uno dei gestionali
> Ho.Re.Ca.** gli scaglioni della spesa di trasporto potranno essere
> definiti:

- sulla base di quanto impostato per il campo **"Misuratore Trasporto a
  Scaglioni"** nell'Anagrafica Passweb degli articoli presenti in ordine
  (sezione **Informazioni Generali**)

- sulla base del Peso indicato all'interno del relativo campo presente
  nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

- sulla base di quanto indicato all'interno di un Attributo Articolo
  Passweb appositamente realizzato.

> In queste condizioni nel caso in cui dovessero essere indicati dei
> valori in percentuale, la percentuale indicata, per gli importi del
> costo, verrà calcolata sempre sul Totale Merce (comprensivo di IVA).

- **Scaglioni in base al campo Personalizzato e Calcolo Percentuale
  sull'Imponibile:** in questo caso gli scaglioni del costo accessorio
  che si sta codificando potranno essere definiti, **per siti Ecommerce
  collegati a Mexal:**

  - sulla base di quanto indicato all'interno dello specifico campo
    gestionale collegato alla funzionalità Mexal **"Spese di trasporto a
    Scaglioni"**

  - sulla base del Peso indicato all'interno del relativo campo presente
    nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

  - sulla base di quanto indicato all'interno di un Attributo Articolo
    Passweb appositamente realizzato

> Nel caso invece di **siti Ecommerce collegati ad uno dei gestionali
> Ho.Re.Ca.** gli scaglioni della spesa di trasporto potranno essere
> definiti:

- sulla base di quanto impostato per il campo **"Misuratore Trasporto a
  Scaglioni"** nell'Anagrafica Passweb degli articoli presenti in ordine
  (sezione **Informazioni Generali**)

- sulla base del Peso indicato all'interno del relativo campo presente
  nell'Anagrafica Passweb dell'Articolo (sezione **Spedizione**)

- sulla base di quanto indicato all'interno di un Attributo Articolo
  Passweb appositamente realizzato.

> In queste condizioni nel caso in cui dovessero essere indicati, per
> gli importi del costo, dei valori in percentuale, la percentuale
> indicata verrà calcolata sempre sull'Imponibile (Totale merce NON
> comprensivo di IVA).

**Tipo di campo:** visualizzato solo nel caso in cui il precedente
parametro "**Scaglioni e Calcolo percentuale**" sia stato impostato su
uno dei seguenti valori: **Scaglioni in base al campo Personalizzato e
Calcolo Percentuale sull'Imponibile** oppure **Scaglioni in base al
campo Personalizzato e Calcolo Percentuale sul Totale Merce**.

Consente di stabilire la tipologia del campo da utilizzare nel calcolo
dello scaglione in cui ricade il costo accessorio in oggetto.

E' possibile selezionare uno dei seguenti valori:

- **Campo Articolo:** in queste condizioni sarà possibile decidere di
  utilizzare come campo per il calcolo dello scaglione, selezionandolo
  dal menu a tendina presente in corrispondenza del successivo parametro
  (**Campo**), il Peso definito per l'articolo all'interno del
  corrispondente campo dell'Anagrafica Passweb (sezione
  "**Spedizione**"), oppure il campo gestionale collegato alla
  funzionalità Mexal **"Spese di trasporto a Scaglioni" (**opzione
  "**Misuratore**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\costo_accessorio_tipo_campo_1.bmp](./assets/media/image431.png){width="5.779166666666667in"
height="3.5256944444444445in"}

- **Attributo Articolo**: in queste condizioni sarà possibile decidere
  di utilizzare come campo per il calcolo dello scaglione,
  selezionandolo dal menu a tendina presente in corrispondenza del
  successivo parametro (**Attributo**), uno degli Attributi articolo
  Passweb appositamente creati per questo scopo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\costo_accessorio_tipo_campo_2.bmp](./assets/media/image432.png){width="5.779166666666667in"
height="3.5256944444444445in"}

**ATTENZIONE!** All'interno del menu a tendina verranno visualizzati
solo ed esclusivamente Attributi Articolo di tipo "**Testo**" o
"**Numero**"

**Filtro Articoli:** consente di definire uno specifico filtro da
applicare agli articoli inseriti in ordine. Impostando un filtro
articoli occorre poi considerare che:

- Il relativo costo verrà applicato solo ed esclusivamente nel caso in
  cui uno o più articoli presenti in ordine soddisfino il filtro
  impostato

- In caso di Costo Tabellare il valore indicato nel precedente campo
  "Scaglioni e Calcolo Percentuale" verrà determinato prendendo in
  considerazione solo ed esclusivamente gli articoli presenti in ordine
  che soddisfano il filtro impostato (si vedano anche a tal proposito
  gli esempi presenti nel successivo paragrafo *"Spese Accessorie --
  Casi d'uso"*).

In questo senso poi occorre sottolineare che, **relativamente agli
articoli di tipo Campionario**, la validazione del filtro impostato
verrà fatta prendendo in considerazione l'articolo Campionario in sé
piuttosto che i singoli Componenti dipendentemente da come è stato
impostato il parametro "**Gestione Articoli Box**" alla pagina
"**Configurazione Catalogo**" del Wizard.

In particolare nel caso in cui il parametro in questione dovesse essere
impostato sul valore:

- **Considera il Box** -- **opzione di default**: verrà preso in
  considerazione soltanto l'articolo Campionario.

> In questo caso dunque, la condizione che determina l'applicazione o
> meno del costo accessorio verrà validata prendendo in considerazione
> solo l'articolo Campionario in sé, indipendentemente dal fatto che i
> suoi componenti possano poi soddisfare o meno lo stesso filtro

- **Considera i componenti del Box**: verranno presi in considerazione
  soltanto i singoli componenti del Campionario

> In queste caso dunque, la condizione che determina l'applicazione o
> meno del costo accessorio verrà validata prendendo in considerazione i
> componenti del Campionario ma non l'articolo Campionario in sé che,
> quindi, potrebbe anche non soddisfare il filtro impostato.

**Limite Minimo di Costo (Ivato):** consente di impostare per il costo
in oggetto uno specifico limite minimo. Se impostato, nel caso in cui il
valore complessivo del costo risultasse poi inferiore al valore
indicato, verrà comunque considerato il limite minimo.

> **NOTA BENE:** i valori indicati all'interno di questo campo sono
> sempre considerati comprensivi di IVA

**Limite Massimo di Costo (Ivato):** consente di impostare per il costo
in oggetto uno specifico limite massimo. Se impostato, nel caso in cui
il valore complessivo del costo risultasse poi superiore al valore
indicato, verrà comunque considerato il limite massimo.

> **NOTA BENE:** i valori indicati all'interno di questo campo sono
> sempre considerati comprensivi di IVA

**Gestione Limite:** consente di indicare se i successivi valori
impostati all'interno dei campi "Limite Minimo / Massimo del totale
merce" dovranno essere considerati o meno privi di iva

**Limite Minimo del totale merce:** valore del totale merce al di sotto
del quale il costo accessorio in esame non dovrà essere considerato.

Nel caso in cui dunque il totale merce del documento dovesse essere
minore del valore indicato all'interno di questo campo, il
corrispondente costo accessorio non concorrerà alla determinazione del
valore complessivo della relativa spesa accessoria**.**

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**Limite Massimo del totale merce:** valore del totale merce al di sopra
del quale il costo accessorio in esame non dovrà essere considerato.

Nel caso in cui dunque il totale merce del documento dovesse essere
maggiore o uguale al valore indicato all'interno di questo campo, il
corrispondente costo accessorio non concorrerà alla determinazione del
valore complessivo della relativa spesa accessoria.

**ATTENZIONE!** l'importo indicato all'interno di questo campo verrà
considerato comprensivo o meno di iva a seconda di quanto impostato per
il precedente parametro "Gestione Limite"

**NOTA BENE:** nel caso in cui l'utente che effettua l'ordine abbia una
valuta diversa da quella specificata all'interno del campo "Valuta di
riferimento" gli importi dei limiti minimo e massimo specificati in fase
di configurazione della spesa di trasporto verranno convertiti nella
valuta in uso dal cliente.

**ATTENZIONE!** anche in questo caso il Totale Merce, sarà considerato
comprensivo o meno di eventuali articoli spesa inserti in carrello (a
seguito dell'applicazione di determinate promozioni o buoni sconto)
dipendentemente dall'impostazione scelta per il parametro "**Gestione
Totale Merce**" presente nella sezione "*Catalogo -- Configurazione
Parametri Catalogo*" del Wizard

I parametri esaminati fino a questo momento consentono,
fondamentalmente, di definire le principali caratteristiche del costo
che si sta configurando, **ma non indicano ancora la specifica modalità
di calcolo (fissa o tabellare) da applicare a questo costo ne tanto meno
consentono di indicare i relativi importi.**

**Allo stesso modo di quanto avviene per le spese di spedizione, anche
in questo caso infatti tali informazioni non vengono associate al costo
nel suo complesso ma bensì alla specifica zona di spedizione della
merce**.

**NOTA BENE:** l'importo dei costi associati ad una spesa accessoria, e
conseguentemente anche l'importo della spesa stessa, potrà variare in
base all'area geografica di spedizione della merce.

