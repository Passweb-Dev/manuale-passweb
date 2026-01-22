# FASE 1 -- REGISTRAZIONE E ATTIVAZIONE DELL'ACCOUNT GTM



La prima cosa da fare è, ovviamente, quella di iscriversi al servizio,
creare il proprio Account GTM e configurare le sue impostazioni
iniziali.

Portandosi quindi nella pagina di accesso al servizio (
<https://marketingplatform.google.com/about/tag-manager/> ), sarà
necessario cliccare sul pulsante **Accedi a Tag Manager** e inserire,
dove richiesto, le credenziali del proprio **Account Google**

![](./assets/media/image7.png)

**ATTENZIONE! Come indicato nei precedenti capitoli di questo manuale il
fatto di possedere un proprio Account Google è il prerequisito
indispensabile per poter accedere ai servizi offerti da GTM e creare
quindi il proprio Account.**

Per maggiori informazioni relativamente a come creare un Account Google
si veda anche la sezione "*Google Analytics*" di questo manuale o la
specifica documentazione presente in rete.

Una volta effettuato l'accesso con il nostro Account Google, ci verranno
richieste alcune informazioni di base necessarie per poter consentire a
GTM di creare correttamente il nuovo Account.

Nello specifico dovremo quindi inserire, innanzitutto, il nome del nuovo
Account (campo **Nome Account**), dovremo impostare il paese in cui
andremo ad operare (campo "**Paese**") e, infine, dovremo decidere se
condividere o meno, in forma anonima, le informazioni con Google

![](./assets/media/image8.png)

Nel secondo step sarà invece necessario assegnare un nome al Tag
Contenitore (campo **"Nome Contenitore"**) e indicare, soprattutto, la
tipologia di piattaforma su cui il Tag andrà inserito, selezionando, nel
nostro caso, l'opzione "**Web**"

![](./assets/media/image9.png)

**ATTENZIONE!** Ogni Account di GTM deve avere almeno un Contenitore. Si
consiglia di assegnare all'Account il nome della propria azienda e ad
ogni Contenitore il nome dello specifico sito in cui il Contenitore
stesso verrà poi utilizzato

Una volta impostate le informazioni richieste, cliccando sul pulsante
**Crea** verranno visualizzate le condizioni e i termini del servizio di
GTM e, una volta accettate, verrà finalmente creato il nuovo Account GTM
e verranno immediatamente visualizzati anche gli snippet di codice da
inserire nei relativi campi di configurazione del proprio sito Passweb.

Nello specifico il primo snippet di codice (da inserire "quanto più in
alto possibile nella sezione \< head \> della pagina") dovrà essere
copiato e incollato all'interno campo "**Monitoraggio Google Tag Manager
-- HEAD**" presente alla pagina "**Sito -- Preferenze**" del Wizard (tab
"**Tracciamento Dati**", sezione "**Google Tag Manager**")

Il secondo snippet (da inserire "immediatamente dopo il tag \< body \>
") dovrà invece essere copiato e incollato all'interno del campo
"**Monitoraggio Google Tag Manager -- BODY**" presente anch'esso alla
pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento Dati**",
sezione "**Google Tag Manager**")

Una volta creato l'Account sarà comunque possibile visualizzare il
codice di installazione in un qualsiasi altro momento. Per far questo è
infatti sufficiente accedere alla sezione di **Amministrazione** di GTM

![](./assets/media/image10.png)

e cliccare sulla voce "**Installa Google Tag Manager**" presente in
corrispondenza della colonna "**Contenitore**"

![](./assets/media/image11.png)

**ATTENZIONE!** Per maggiori informazioni in merito all'interfaccia web
di Google Tag Manager e, nel caso specifico, alla sua sezione di
Amministrazione, si consiglia di fare riferimento alla specifica
documentazione presente in rete.

**ATTENZIONE!** Nelle condizioni attuali il Tag Contenitore risulterà
essere correttamente installato sul sito Passweb. **Questo stesso Tag
Contenitore, però, non è stato ancora pubblicato** come indicato anche
nell'interfaccia web di GTM

![](./assets/media/image12.png)

Per maggiori informazioni relativamente a come e quando pubblicare
effettivamente un Tag Contenitore si vedano anche i successivi capitoli
di questo manuale

