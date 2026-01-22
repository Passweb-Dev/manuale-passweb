# CONSENT SOLUTION



Oltre alla "Privacy e Cookie Policy" e alla "Cookie Solution", volendo,
è possibile integrare all'interno del proprio sito Passweb anche il
servizio di "**Consent Solution**" offerto da Iubenda in maniera tale da
mantenere un registro dei consensi popolato in automatico con i dati
inseriti dagli utenti sui vari form presenti all'interno del proprio
sito.

**ATTENZIONE! L'integrazione della Consent Solution utilizza i metodi e
la libreria javascript messi a disposizione da Iubenda stesso. Richiede
quindi l'inserimento di un' apposito script nelle pagine del sito e,
soprattutto, richiede l'inserimento e la personalizzazione di una
specifica funzione javascript necessaria per inviare a Iubenda e
memorizzare nel relativo registro, i consensi forniti dagli utenti del
proprio sito.**

Nello specifico per integrare il servizio di "Consent Solution" messo a
disposizione da Iubenda sarà necessario:

1.  Attivare e configurare su Iubenda tutto il necessario per gestire il
    servizio di **Consent Solution**

> In particolare in fase di generazione e configurazione della Consent
> Solution si consiglia di selezionare il parametro "**Sincronizza i
> tuoi documenti legali Iubenda con la Consent Solution**" in maniera
> tale da mantenere aggiornati in maniera automatica i documenti legali
> prodotti da Iubenda con i relativi consensi forniti dagli utenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\consent_solution_2.bmp](./assets/media/image7.png){width="4.571527777777778in"
height="3.863888888888889in"}

> Per maggiori informazioni relativamente a come attivare e configurare
> su Iubenda la Consent Solution si consiglia di fare sempre riferimento
> alla documentazione presente sul relativo portale (
> <https://www.iubenda.com/it/help/6525-introduzione-consent-solution> )

2.  Una volta completata la configurazione della Consent Solution sarà
    necessario prelevare dal sito di Iubenda il codice di integrazione
    ed inserirlo poi nella sezione \< head \> di tutte le pagine del
    sito in cui sono presenti form deputati alla raccolta di consensi da
    inviare alla piattaforma terza (es. form di registrazione utenti,
    form del profilo utente, form generici di richiesta dati ...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\consent_solution_3.bmp](./assets/media/image8.png){width="4.571527777777778in"
height="3.863888888888889in"}

> Come nel caso della Cookie Solution anche questa volta il codice di
> integrazione potrà essere inserito nell' \< head \> delle relative
> pagine usando, ad esempio, la sezione "**Meta Tags**" del layout di
> sito, il campo "**Code Snippet -- Head**" presente alla sezione "*Sito
> -- Preferenze -- Integrazioni*" del Wizard oppure il campo "**Head**"
> presente tra i parametri di configurazione della singola pagina

3.  Arrivati a questo punto sarà necessario, infine, portarsi nella
    specifica pagina del sito in cui è presente il form deputato alla
    raccolta dei consensi (e in cui sono dunque inseriti appositi check
    di accettazione della privacy, dei termini e condizioni, della
    newsletter ecc...) e inserire **immediatamente dopo il componente
    Form di Passweb**, un componente HTML all'interno del quale
    implementare la funzione javascript necessaria per inviare e
    memorizzare nel registro dei consensi di Iubenda i dati inserti
    dagli utenti in fase di compilazione di quello stesso form.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\consent_solution_4.bmp](./assets/media/image9.png){width="4.571527777777778in"
height="4.629861111111111in"}

Relativamente all'implementazione della funzione javascript necessaria
per inviare i relativi consensi al registro di Iubenda occorre
sottolineare che:

- In Passweb alla conferma dei form relativi ai componenti "**Form**",
  "**Registrazione Utente**" e "**Profilo Utente**", in mancanza di
  errori, è possibile richiamare una funzione javascript di callback che
  dovrà avere un nome del tipo:

> **callback\<id_componente\>**
>
> Nello specifico dunque, se il form deputato alla raccolta dei consensi
> dovesse essere il form di registrazione utente, la funzione javascript
> con cui inviare i dati a Iubenda dovrebbe essere inserita all'interno
> di una variabile di questo tipo:
>
> var **callbackuserregistration_12984** = function()
>
> {
>
> Istruzioni di invio dati a Iubenda
>
> }
>
> dove, ovviamente, **userregistration_12984** sarà l'id del componente
> Passweb di "Registrazione Utente"
>
> Allo stesso modo, nel momento in cui il form deputato alla raccolta
> dei consensi dovesse essere il form del profilo utente, la funzione
> javascript con cui inviare i dati a Iubenda dovrebbe essere inserita
> all'interno di una variabile di questo tipo:
>
> var **callbackuserprofile_7751**= function()
>
> {
>
> Istruzioni di invio dati a Iubenda
>
> }
>
> Infine, nel momento in cui il form deputato alla raccolta dei consensi
> dovesse essere un form generico di raccolta informazioni, la funzione
> javascript con cui inviare i dati a Iubenda dovrebbe essere inserita
> all'interno di una variabile di questo tipo:
>
> var **callbackform_12984**= function()
>
> {
>
> Istruzioni di invio dati a Iubenda
>
> }

- **La funzione javascript dovrà essere implementata secondo le
  specifiche esigenze del caso e seguendo sempre quanto previsto dalla
  relativa documentazione Iubenda** accessibile al seguente indirizzo
  <https://www.iubenda.com/it/help/6530-consent-solution-documentazione-js>

Di seguito viene fornito un esempio di funzione javascript implementata
in relazione al componente "Registrazione Utente" di Passweb utilizzando
il submit del form come metodologia di invio dati

*\<script type=\"text/javascript\"\>*

*var callbackuserregistration_86212 = function () {*

*// Synchronous call, it\'s sent right when this function is executed*

*\_iub.cons_instructions.push(\[\"submit\", {*

*writeOnLocalStorage: false,*

*form: {*

*selector: document.getElementById(\'userregistration_86212-form\'),*

*map: { // optional: map consent attributes directly to the
corresponding*

*// input\'s \"name\" attribute, instead of using data-cons-x
attributes*

*subject: {*

*id: \"entityid\",*

*email: \"username\",*

*first_name: \"name\",*

*last_name: \"last_name\"*

*},*

*preferences: {*

*privacy: \"privacy\",*

*newsletter_interna: \"234\",*

*newsletter_esterna: \"237\"*

*}*

*}*

*},*

*consent: {*

*legal_notices: \[*

*{*

*identifier: \'privacy_policy\',*

*},*

*{*

*identifier: \'cookie_policy\',*

*},*

*{*

*identifier: \'term\',*

*}*

*\],*

*}*

*},{*

*success: function(response) {*

*console.log(response);*

*},*

*error: function(response) {*

*console.log(response);*

*}*

*}\])*

***sleep(1000);//1 secondo***

*}*

***function sleep(milliseconds) {***

***const date = Date.now();***

***let currentDate = null;***

***do {***

***currentDate = Date.now();***

***} while (currentDate - date \< milliseconds);***

***}***

*\</script\>*

**ATTENZIONE!** La parte evidenziata in grassetto e relativa alla
funzione "**sleep()**" dovrà essere inserita solo nel caso in cui il
form in questione dovesse redirigere ad una pagina diversa da quella in
cui si trova il form stesso

