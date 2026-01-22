# GOOGLE RECATPCHA



All'interno dei siti Passweb è possibile attivare, in pochi semplici
passaggi, il **Google Recaptcha** ossia il sistema antispam offerto da
Google e in grado di semplificare la vita agli utenti del sito grazie al
fatto che non li costringe più ad interpretare e riscrivere sequenze più
o meno leggibili di caratteri e/o numeri per poter dimostrare, in fase
di compilazione di un form, di non essere un bot e li mette quindi nelle
condizioni di poter procedere rapidamente alla conferma del form stesso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_1.bmp](./assets/media/image84.png){width="5.304861111111111in"
height="3.7402777777777776in"}

Attualmente esistono 2 versioni di Google Recaptcha la v2 e v3 (entrambe
attivabili all'interno del proprio sito Passweb).

- **Google Recaptcha v2:** può richiedere di selezionare l'opzione "Non
  sono un robot" per passare la validazione

- **Google Recaptcha v3**: con questa versione il recaptcha è totalmente
  invisibile. Rispetto alla controparte v2 non c'è una richiesta di
  validazione del tipo "fai check su tutti i cartelli presenti nelle
  immagini", viene infatti modificato il meccanismo che identifica un
  utente, o un bot, restituendo un punteggio indicante il livello di
  sospettosità di un'interazione ed eliminando di fatto la necessità
  della challenge. Questa versione del recaptcha aziona un'analisi
  adattiva del rischio in background per notificare il traffico sospetto
  e la sicurezza sta nel fatto che Google analizza anche il
  comportamento dell'utente dall'istante esatto in cui atterra
  all'interno della pagina

> 
>
> **ATTENZIONE!** **Per poter utilizzare correttamente la versione 3 di
> Google Recaptcha è necessario disporre di un sito sviluppato su di una
> Variante Responsiva**

Come detto in Passweb è possibile attivare entrambe le versioni del
Google Recaptcha agendo mediante i parametri di configurazione presenti
all'interno della sezione "**Google recaptcha**" alla pagina "*Sito --
Preferenze -- Integrazioni*" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_2.bmp](./assets/media/image85.png){width="5.811805555555556in"
height="3.532638888888889in"}

Nello specifico il campo:

- **Versione Google Recaptcha:** consente di impostare la versione di
  Google Recaptcha che si intende attivare all'interno del proprio sito
  (per le differenze tra la versione v2 e la versione v3 si consiglia di
  far sempre riferimento alla specifica documentazione presente in rete)

- **Soglia di validazione Google Recaptcha:** visibile solo nel caso in
  cui si sia scelto di implementare la versione v3 di Google Recaptcha.
  Come detto in questo caso l\'utente non dovrà selezionare nessun flag
  o passare nessun test per dimostrare di non essere un robot. La
  validazione avviene tramite un punteggio che viene assegnato da Google
  nel range 0 → 1 in cui 0 indica Robot al 100% e 1 indica Umano al
  100%.

> Il parametro in questione serve proprio a determinare quando
> considerare attendibile un utente in relazione alla valutazione
> fornita da Google all'utente stesso.
>
> Supponendo dunque di impostare la soglia di validazione a 0.5 il
> controllo verrà passato solo nel momento in cui la valutazione fornita
> da Google all'utente che sta navigando il sito sia superiore a 0.5
> (assumendo quindi un valore compreso tra 0.6 e 1)

Indipendentemente dal fatto di voler implementare la versione 2 o la
versione 3, per completare la configurazione sarà poi necessario
disporre di un'apposita coppia di valori, "**Chiave Sito**", "**Chiave
Segreta**" da inserire all'interno dei relativi campi ("**Chiave Google
Recaptcha**" e "**Chiave Secret Google Recaptcha**") presenti in questa
sezione del Wizard.

Per poter ottenere questa coppia di chiavi è necessario:

1.  Accedere alla Google Cloud Console
    <https://console.cloud.google.com/> utilizzando il proprio account
    Google e selezionare dal menu a sinistra la voce "**Security --
    reCAPTCHA**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_3.bmp](./assets/media/image86.png){width="5.33125in"
height="3.3895833333333334in"}

2.  Una volta effettuato l'accesso a questa sezione delle Google Cloud
    Console sarà poi necessario cliccare sul pulsante "**Create key**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_3a.bmp](./assets/media/image87.png){width="5.33125in"
height="3.3895833333333334in"}

> per avviare il processo di creazione di una nuova coppia di chiavi

3.  Nella successiva maschera di creazione delle chiavi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_4.bmp](./assets/media/image88.png){width="5.33125in"
height="3.3895833333333334in"}

> sarà quindi necessario:

- assegnare un nome identificativo alla coppia di chiavi che andremo a
  realizzare (campo "**Display name**")

- impostare il parametro "**Application type**" sull'opzione "**Web**"

- cliccare sul pulsante "**Add a domain**" e inserire nel successivo
  campo di input il dominio del proprio sito privo di www

4.  A questo punto, dipendentemente dal fatto di voler attivare il
    reCAPTCHA in versione v2 (quindi con la possibilità da parte
    dell'utente di dover interagire con la pagina web per provare di non
    essere un bot) o in versione v3 (quindi senza richiesta di
    interazione da parte dell'utente) sarà necessario cliccare o meno
    sul pulsante "Next step"

> In particolare nel momento in cui l'esigenza dovesse essere quella di
> attivare il reCAPTCHA in versione v2 sarà necessario cliccare sul
> pulsante "Next step" e abilitare poi, nella successiva maschera, il
> parametro "**Will you use challenges**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_4a.bmp](./assets/media/image89.png){width="5.33125in"
height="3.3833333333333333in"}

> impostando anche la difficoltà del challenge che dovrà essere
> applicata all'interno del sito.
>
> **ATTENZIONE!** questa impostazione richiede necessariamente che il
> parametro "**Versione Google Recaptcha**" presente alla pagina
> "**Preferenze Sito -- Integrazioni**" del Wizard (sezione "**Google
> Recaptcha**") sia impostato sull'opzione v2
>
> Nel caso in cui l'esigenza dovesse essere invece quella di attivare il
> reCAPTCHA in versione v3 il secondo step può tranquillamente essere
> saltato cliccando immediatamente sul pulsante "Create Key" presente
> nella parte bassa della pagina
>
> **ATTENZIONE!** in queste condizioni (utilizzo di Google reCAPTCHA in
> modalità trasparente all'utente) il parametro **Versione Google
> Recaptcha**" presente alla pagina "**Preferenze Sito --
> Integrazioni**" del Wizard (sezione "**Google Recaptcha**") dovrà
> essere necessariamente impostato sull'opzione v3
>
> **ATTENZIONE!** una volta creata la coppia di chiavi non sarà più
> possibile modificare l'opzione relativa all'uso o meno del challenge,
> per cui se dovesse esserci l'esigenza di passare da una gestione
> all'altra sarà per forza di cose necessario creare una nuova coppia di
> chiavi.

5.  Una volta decisa la tipologia di reCAPTCHA da utilizzare, e
    impostati di conseguenza i relativi parametri, cliccando sul
    pulsante "**Create key**" verranno create le chiavi e verremo
    automaticamente ridiretti alla sezione "**Integration**" del
    pannello di gestione del nostro reCAPTCHA

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_5.bmp](./assets/media/image90.png){width="5.33125in"
height="3.3895833333333334in"}

6.  A questo punto sarà sufficiente copiare la chiave indicata in
    corrispondenza del campo **ID** (nella parte alta della maschera)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_6.bmp](./assets/media/image91.png){width="5.33125in"
height="3.3895833333333334in"}

> ed incollarla all'interno del campo "**Chiave Google Recaptcha**"
> presente nella sezione "**Google recaptcha**" alla pagina "*Sito --
> Preferenze -- Integrazioni*" del Wizard
>
> Per ottenere la secret key sarà invece necessario utilizzare il
> pulsante "**Integrate with a third -party service or plugin**"
> evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_7.bmp](./assets/media/image92.png){width="5.33125in"
height="3.3895833333333334in"}

> In questo modo verrà infatti visualizzata la maschera "Legacy
> reCAPTCHA"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_8.bmp](./assets/media/image93.png){width="5.33125in"
height="3.3895833333333334in"}

> all'interno della quale potremo prelevare il valore della legacy
> secret key ed inserirlo, sul Wizard di Passweb, in corrispondenza del
> campo "**Chiave Segreta Google Recaptcha**"

Una volta terminata la procedura e attivato correttamente il servizio il
Google Recaptcha potrà essere inserito all'interno di tutti i form del
sito per i quali è possibile gestire il componente "**Captcha**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\recaptcha_9.bmp](./assets/media/image94.png){width="5.954861111111111in"
height="3.785416666666667in"}

**ATTENZIONE!** Nel caso in cui si decida di non attivare il servizio di
Google sarà comunque possibile inserire all'interno dei vari form del
proprio sito Passweb il componente Captcha classico che richiederà
all'utente di ripetere una determinata sequenza di caratteri prima di
poter effettivamente confermare il form.

Per maggiori informazioni relativamente alla gestione dei form in
Passweb e, nello specifico, al componente Captcha, si veda anche la
corrispondente sezione di questo manuale (es. "*Varianti Responsive --
Lista Componenti Comuni -- Componente Form -- Componenti per il Form
Campo Captcha*")

