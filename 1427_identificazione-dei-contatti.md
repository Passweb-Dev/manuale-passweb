# IDENTIFICAZIONE DEI CONTATTI



Come evidenziato nei precedenti capitoli di questo manuale il punto
fondamentale di tutto il processo di monitoraggio è quello di riuscire a
identificare in maniera corretta gli utenti che stanno navigando sul
sito in modo tale che ActiveCampaign possa poi associare al relativo
Contatto i dati di tracciamento e visualizzarli quindi nella sezione
"**Attività recenti**" della sua anagrafica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\timeline_activecampaign.bmp](./assets/media/image21.png){width="4.714583333333334in"
height="2.9743055555555555in"}

**ATTENZIONE!** i dati di tracciamento inviati ad ActiveCampaign
potranno essere visualizzati solo nel momento in cui sarà anche
possibile associarli ad uno specifico contatto

In questo senso, come indicato nella documentazione ufficiale (
<https://help.activecampaign.com/hc/it/articles/221542267-Una-panoramica-del-Monitoraggio-del-sito>
) ActiveCampaign ha tre modi diversi per riuscire ad identificare in
maniera corretta un determinato contatto, vale a dire:

- **Quando il contatto fa click su di un collegamento presente in una
  campagna**.

> In questo caso il link su cui il contatto andrà a cliccare dovrà
> portare ad una pagina del sito in cui è stato inserito il codice di
> monitoraggio e che, ovviamente, fa parte delle pagine inserite in
> whitelist e che possono quindi essere effettivamente tracciate (il
> consiglio è quindi quello di mettere in whitelist sempre l'intero
> sito, come indicato nel precedente capitolo di questo manuale)
>
> **ATTENZIONE!** questo tipo di identificazione del contatto non
> funziona nelle mail personalizzate 1 a 1

- **Quando il contatto si registra utilizzando un modulo di iscrizione
  nativo di ActiveCampaign**

> In questo caso il form di iscrizione di ActiveCampaign deve
> reindirizzare l'utente che si è iscritto, ad una pagina del sito in
> cui è stato inserito il codice di monitoraggio e che, ovviamente, fa
> parte delle pagine inserite in whitelist e che possono quindi essere
> effettivamente tracciate. La thankyou page predefinita dei moduli di
> ActiveCampaign non genererà un cookie di tracciamento e non sarà
> quindi possibile identificare il contatto.
>
> Inoltre occorre anche ricordare che:

- se il modulo utilizzato ha il double opt-in attivato le
  visualizzazioni di pagina non verranno monitorate fino a quando
  l'utente non avrà completato il processo di opt-in

- **moduli di iscrizione di terze parti non possono generare il cookie
  di tracciamento e non possono quindi portare all'identificazione del
  contatto**

> In considerazione di quanto appena detto dunque se l'utente dovesse
> registrarsi alla Newsletter:

- da un form generico di Passweb

- dal modulo Passweb di Registrazione utente

- dal modulo Passweb di Profilo utente

> non verrà generato nessun cookie di tracciamento, il contatto non
> verrà identificato e, nella sua Anagrafica ActiveCampaign, non
> verranno riportati dati relativi alle pagine visitate.
>
> In queste condizioni il consiglio è quindi quello di implementare
> l'identificazione del contatto mediante indirizzo Email.
>
> Altra cosa fondamentale da mettere in evidenza è che
> **l'identificazione di un contatto mediante la compilazione di un
> modulo nativo di ActiveCampaign è retroattiva** per cui le visite al
> sito effettuate da quello stesso utente e precedentemente anonime,
> perché il contatto non era ancora stato identificato, nel momento in
> cui verrà identificato verranno associate alla sua anagrafica e
> saranno quindi visibili nella sezione "Attività recenti"

- **Quando viene inserita la mail dell'utente che naviga il sito
  direttamente nel codice di tracciamento**

> Una volta che l'utente che naviga il sito è stato identificato, quindi
> dopo che ha effettuato la login, è possibile inserire il suo indirizzo
> email nel codice di monitoraggio ed inviarlo quindi ad ActiveCampaign
> assieme agli altri dati.
>
> In questo modo l'indirizzo email farà ovviamente da chiave e se sulla
> piattaforma è già presente un contatto con quella stessa mail i dati
> di tracciamento verranno associati alla sua anagrafica
>
> **ATTENZIONE! l'identificazione del contatto mediante invio di
> indirizzo mail da codice di tracciamento non è retroattiva**
>
> A differenza del caso precedente dunque, in queste condizioni verranno
> visualizzati, nella sezione "Attività recenti" dell'anagrafica del
> contatto ActiveCampaign, solo i dati delle pagine visitate dopo
> l'identificazione del contatto (quindi dopo che l'utente ha effettuato
> il login)

In considerazione di quanto detto nel momento in cui si volesse
implementare sul proprio sito Passweb il sistema di tracciamento di
ActiveCampaign il consiglio è quello di utilizzare, come modulo di
iscrizione alla Newsletter a se stante, uno dei moduli nativi di
ActiveCampaign.

Considerando però che l'iscrizione potrebbe avvenire anche direttamente
in fase di registrazione al sito, quindi da uno dei componenti Passweb,
per non perdere dati di tracciamento si dovrebbe implementare anche
l'invio della mail utente mediante lo snippet di codice.

In questo senso, seguendo quanto indicato dalla documentazione
ufficiale, una possibilità potrebbe essere quella di modificare lo
snippet di tracciamento standard, aggiungendo il codice evidenziato in
grassetto immediatamente prima dell'istruzione vgo('process') come di
seguito indicato:

*\<script\>
(function(e,t,o,n,p,r,i){e.visitorGlobalObjectAlias=n;e\[e.visitorGlobalObjectAlias\]=e\[e.visitorGlobalObjectAlias\]\|\|function(){(e\[e.visitorGlobalObjectAlias\].q=e\[e.visitorGlobalObjectAlias\].q\|\|\[\]).push(arguments)};e\[e.visitorGlobalObjectAlias\].l=(new
Date).getTime();r=t.createElement(\"script\");r.src=o;r.async=true;i=t.getElementsByTagName(\"script\")\[0\];i.parentNode.insertBefore(r,i)})(window,document,\"https://diffuser-cdn.app-us1.com/diffuser/diffuser.js\",\"vgo\");*

*vgo(\'setAccount\', \'XXXXXXXX\');*

*vgo(\'setTrackByDefault\', true);*

***var userEmail = \"{{userEmail}}\";***

***if(userEmail != "") {***

***vgo(\'setEmail\', userEmail);***

***}***

*vgo(\'process\');*

*\</script\>*

In particolare infatti la porzione di codice

***var userEmail = \"{{userEmail}}\";***

***if(userEmail != "") {***

***vgo(\'setEmail\', userEmail);***

***}***

verifica per prima cosa che il segnaposto ***{{userEmail}}*** sia
valorizzato e, considerando che tale segnaposto viene sostituito a
runtime con la mail dell'utente attualmente loggato, questa condizione
potrà essere soddisfatta solo dopo che l'utente ha effettuato il login
(posto ovviamente che abbia una mail associata alla sua anagrafica).

Una volta verificata la condizione verrà poi eseguita l'istruzione
**vgo('setEmail', userEmail);** che, come indicato nella documentazione
ufficiale di ActiveCampaign andrà a settare la mail dell'utente che sta
navigando il sito prima di inviarla (con la successiva istruzione
vgo('process') ) ad ActiveCampaign assieme a tutti gli altri dati di
tracciamento

In questo modo se la mail inviata ad ActiveCampaign dovesse
corrispondere a quella di un contatto già presente sulla piattaforma le
pagine vistate dopo il login verranno correttamente registrate
nell'anagrafica di questo stesso contatto

Per maggiori informazioni sulle procedure di identificazione dei
contatti si consiglia di fare sempre riferimento alla relativa
documentazione di prodotto presente sul sito ufficiale di ActiveCampaign
(<https://help.activecampaign.com/hc/it/articles/221542267-Una-panoramica-del-Monitoraggio-del-sito>)

