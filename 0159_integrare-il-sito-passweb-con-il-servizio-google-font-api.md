# INTEGRARE IL SITO PASSWEB CON IL SERVIZIO GOOGLE FONT API



Nel caso in cui non si dovesse disporre delle conoscenze tecniche
necessarie per operare direttamente a livello di codice CSS e/o nel caso
in cui si desideri utilizzare direttamente lo Style Editor di Passweb
per l'applicazione dei Google Font è possibile seguire la procedura di
seguito indicata.

- Per poter disporre dei Google Font direttamente all'interno dello
  Style Editor di Passweb è necessario, per prima cosa, integrare
  correttamente il proprio sito con il servizio Google Font Api, creando
  e registrando in questo senso un'apposita Api Key.

> Accedere quindi all'area developer di Google al seguente indirizzo
> <https://console.developers.google.com> e autenticarsi con il proprio
> Account Google.

![](./assets/media/image167.png)

> **ATTENZIONE!** L'Account Google è il prerequisito necessario per
> poter usufruire di tutti i servizi messi a disposizione da Google. Nel
> caso in cui non si disponga ancora di un Account è quindi
> indispensabile, per prima cosa, crearlo.
>
> Per maggiori informazioni in merito alla creazione di un Account
> Google si veda anche la sezione "*Google Analytics*" di questo manuale
> o l'apposita documentazione presente in rete.

- Accedere alla maschera di gestione dei progetti e creare un nuovo
  progetto cliccando sul pulsante raffigurante un piccolo +

![](./assets/media/image168.png)

- Assegnare un nome al progetto (es. Google Font) e cliccare sul
  pulsante **Crea**

![](./assets/media/image169.png)

- Una volta completata la creazione del progetto cliccare sul pulsante
  "**Abilita API e Servizi**" presente nella parte alta della pagina

![](./assets/media/image170.png)

- Dal pannello di gestione delle API selezionare la voce **Web Fonts
  Developer API** presente all'interno della sezione **Altro**

![](./assets/media/image171.png)

- Abilitare la relativa API cliccando per questo sul pulsante
  **ABILITA** presente nella parte alta della maschera

![](./assets/media/image172.png)

- Una volta abilitata la Api Key prima di poterla effettivamente
  utilizzare all'interno del proprio progetto è necessario creare delle
  apposite credenziali, come indicato da Google stesso

![](./assets/media/image173.png)

> Cliccare quindi sul pulsante **Crea Credenziali** per accedere alla
> sezione di gestione delle suddette credenziali

- Nella successiva maschera di gestione delle credenziali impostare la
  combo box "**Quale API stai utilizzando**" sul valore **Web Fonts
  Developer API** e cliccare sul pulsante "**Di quali credenziali hai
  bisogno?**"

![](./assets/media/image174.png)

- A questo punto all'interno della sezione **"Ottieni le tue
  credenziali"** verrà visualizzata l'API Key di cui abbiamo bisogno per
  completare l'integrazione del servizio con il nostro sito Passweb.

![](./assets/media/image175.png)

- Una volta ottenuta l'API Key, prima di completare il processo
  cliccando sul pulsante **Fatto**, copiarla ed incollarla all'interno
  del campo **Chiave Google API** presente nella sezione
  **Integrazioni** della pagina **Sito -- Preferenze** del proprio sito
  Passweb

![](./assets/media/image176.png)

> L' Api Key appena creata potrà comunque essere sempre visualizzata
> nella developer console di Google all'interno della sezione
> "**Credenziali**"

![](./assets/media/image177.png)

- Completata la creazione della Api Key e inserita questa stessa chiave
  sul proprio sito Passweb, per poter effettivamente disporre di uno o
  più Google Font direttamente nello Style Editor sarà ora necessario
  creare, **nel Layout associato alle pagine in cui si vogliono
  effettivamente utilizzare questi font**, apposite inclusioni di tipo
  Google Font.

> Portarsi quindi nella sezione "**Inclusioni nella Pagina**" della
> maschera di gestione del Layout e cliccare sul pulsante "**Nuova
> Inclusione**"
> ![Videate\\pulsante_nuova_inclusione_res.bmp](./assets/media/image178.png) in maniera tale da poter creare una
> nuova inclusione di tipo **Google Font**.

![](./assets/media/image179.png)

> In queste condizioni all'interno del campo **"Google Font"** verrà
> visualizzato l'elenco di tutti i web fonts messi a disposizione da
> Google
>
> **ATTENZIONE!** Nel caso in cui l' Api Key indicata all'interno del
> campo **Chiave Google API** presente nella sezione **Integrazioni**
> della pagina **Sito -- Preferenze** del Wizard, non sia corretta non
> sarà possibile selezionare, in questa fase, alcun tipo di font.
>
> Allo stesso modo nel caso in cui non sia stata inserita alcuna Api Key
> realizzando questo tipo di inclusione verrà visualizzato un apposito
> messaggio di errore con indicata la necessità di inserire tale Api Key
> prima di poter effettivamente selezionare il Google Font desiderato
>
> **ATTENZIONE! E' necessario creare un inclusione di tipo Google Fonts
> per ogni singolo font che si desidera utilizzare nelle pagine cui sarà
> associato il layout in esame**
>
> **Ovviamente nel caso in cui il/i Google Fonts debbano essere
> utilizzati in tutte le pagine del sito è consigliabile effettuare
> questo tipo di inclusioni nel layout di Variante**
>
> Una volta selezionato il font desiderato, cliccare sul pulsante
> **Salva** e successivamente sul pulsante **Applica Modifiche al
> Layout.**

- Arrivati a questo punto potremo quindi utilizzare tutti i Google Font
  per cui sono state create specifiche inclusioni a livello di layout,
  selezionandoli direttamente nello Style Editor di Passweb allo stesso
  modo in cui si seleziona ed utilizza un qualsiasi altro font standard.

> Supponendo, ad esempio, di voler ora utilizzare il Google Font appena
> importato come font per un ben preciso componente Paragrafo, sarà
> sufficiente attivare, nel Live Editing, la modalità di gestione dei
> componenti, selezionare il componente desiderato e nel **R.O.C.
> (Riquadro Opzioni Componente)** cliccare sul pulsante di Editing
> Grafico in maniera tale da aprire lo **Style Editor**

![](./assets/media/image180.png)

> **ATTENZIONE!** Per maggiori informazioni relativamente al R.O.C.,
> allo Style Editor e/o in generale alla gestione dei componenti si veda
> anche il capitolo "*Live Editing per Varianti Responsive --
> Componenti"* di questo manuale
>
> Cliccando quindi sul campo **Font** presente all'interno della sezione
> "**Font e Stile del Testo"** verrà visualizzato l'elenco dei font
> utilizzabili per l'elemento selezionato e tra questi troveremo ora
> anche i Google Font precedentemente inclusi nel layout

![](./assets/media/image181.png)

> Per utilizzare il font desiderato sarà quindi sufficiente selezionarlo
> dall'elenco e cliccare sul pulsante raffigurante un piccolo **+**
> (![](./assets/media/image182.png))

**ATTENZIONE!** Nel caso in cui il font selezionato debba essere
utilizzato come font generale di tutto il sito si consiglia di
abilitarlo a livello di contenitori strutturali sull'elemento **Corpo
Pagina**

