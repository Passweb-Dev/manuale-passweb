# GA4 -- USER PROVIDED DATA E CONVERSIONI AVANZATE



Come indicato nei precedenti capitoli di questo manuale l'integrazione
diretta Passweb -- GA4 consente, se necessario, di attivare anche il
tracciamento dei dati utente di prima parte (i cosiddetti **User
Provided Data**) dati questi che potrebbero rivelarsi particolarmente
utili per:

- Gestire i dati demografici e di interesse senza dover per forza di
  cose ricorrere ai cookie di terze parti

- Gestire le conversioni avanzate su GA4 con il fine di esportarle poi
  all'interno di Google Ads (richiede il collegamento dei due account
  Analytics ed Ads)

- Creare in GA4 audience di pubblico esportabili anche in Google Ads
  (richiede il collegamento dei due account Analytics ed Ads)

**Al netto di tutto questo occorre sempre tenere bene in considerazione
che l'attivazione di questa funzionalità all'interno di Google
Analytics** **andrà di fatto a modificare completamente il modo in cui
GA stesso identificherà e riconoscerà i vari utenti** e, per forza di
cose, avrà quindi un impatto diretto anche sui report generati (che
potrebbero quindi essere sostanzialmente diversi prima e dopo
l'attivazione della funzionalità in questione) e sul sistema di
attribuzione delle diverse conversioni, il tutto sempre in relazione
anche a come è stato settato il **report identity** della proprietà di
GA4 interessata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_attivazione_upd_4.bmp](./assets/media/image22.png){width="5.363194444444445in"
height="3.4583333333333335in"}

Inoltre è bene considerare anche che:

- nel momento in cui è stata scritta questa guida la funzionalità
  "User-provided data collection" in Google Analytics è, come indicato
  anche da Google stesso, ancora una **funzionalità in beta** che
  andrebbe quindi attivata in maniera più che consapevole essendo bene a
  conoscenza anche di tutti possibili problemi che potrebbe causare

- la gestione degli user provided data all'interno di GA4 potrebbe
  "interrompere" il tracciamento degli User Id perché di fatto cambia il
  modo in cui GA4 identifica gli utenti (non più in base allo user-id ma
  in base agli user-provided data che gli vengono forniti o che GA
  stesso recupera in maniera automatica dal sito). In queste condizioni
  inoltre lo user-id eventualmente inviato dal sito non sarebbe più
  disponibile neppure all'interno di Big Query

- **dal punto di vista delle conversioni avanzate, laddove possibile, è
  sempre consigliabile inviare i dati di conversione direttamente a
  Google Ads piuttosto che importarli da GA4**

In sostanza, nel momento in cui è stata scritta questa guida e
supponendo di poter inviare i dati delle conversioni avanzate
direttamente a Google Ads senza passare prima da Analytics (cosa questa
effettivamente possibile in Passweb), l'unico vero vantaggio che si
potrebbe avere nell'attivazione della raccolta degli user provided data
direttamente in GA4 potrebbe essere effettivamente quello di creare in
GA audience di pubblico esportabili ed utilizzabili poi anche in Google
Ads

Ora considerando che il modo di gestire i dati in Google Analytics non
dipende assolutamente da Passweb e che l'attivazione degli User Provided
Data nel tracciamento diretto Passweb -- Analytics comporta unicamente
l'invio diretto da Passweb ad Analytics di determinati dati utente,
secondo le modalità richieste da Analytics stesso, **il consiglio è
sempre quello di documentarsi bene in rete su quello che comporta
effettivamente l'attivazione di questa funzionalità in GA4, su come
potrebbero cambiare i propri report dati e di attribuzione e, alla fine,
di** **attivare questa funzionalità solo se strettamente necessario**

**ATTENZIONE!** per maggiori informazioni sulla gestione degli
user-provided data e delle conversioni avanzate in GA4 si consiglia di
fare sempre riferimento alla specifica documentazione disponibile in
rete e rilasciata da Google stesso

(es.
<https://support.google.com/analytics/answer/14077171?hl=en&ref_topic=14272008&sjid=6691544721313496912-EU#zippy=>
)

Fatte queste doverose e importanti considerazioni, nel momento in cui
l'utente decida comunque di attivare la raccolta degli user provided
data e la gestione delle conversioni avanzate anche in GA4 dovrà
accedere alla sezione "**Admin**" del proprio account di Google
Analytics, cliccare sulla voce "**Data collection**" presente
all'interno della sezione "**Data** **collection and modification**"

![Videate\\ga4_attivazione_upd.bmp](./assets/media/image23.png){width="5.363194444444445in"
height="3.4583333333333335in"}

e cliccare poi sul pulsante "**Turn on**" presente all'interno della
sezione "**User-provided data collection**"

![Videate\\ga4_attivazione_upd_2.bmp](./assets/media/image24.png){width="5.363194444444445in"
height="3.4583333333333335in"}

**ATTENZIONE!** una volta attivata la funzionalità "User-provided data
collection", verrà automaticamente abilitata anche la raccolta
automatica di questo tipo di informazioni (parametro "**Collect
automatically-detected user-provided data**" selezionato a default)
lasciando quindi a Google il compito di ricavarsi automaticamente dalle
pagine del sito i dati di cui ha bisogno, senza però sapere come questi
dati vengono effettivamente ricavati.

Sarà quindi di fondamentale importanza, una volta attivata la
funzionalità in oggetto, ricordarsi anche di disattivare la raccolta
automatica dei dati andando a deselezionare il parametro "**Collect
automatically-detected user-provided data**"

![Videate\\ga4_attivazione_upd_3.bmp](./assets/media/image25.png){width="5.363194444444445in"
height="3.4583333333333335in"}

anche e soprattutto in considerazione del fatto che sarà poi Passweb a
passare ad Analytics gli user-provided data e non avrebbe quindi alcun
senso lasciare ad Analytics la possibilità di ricavarsi questi stessi
dati in maniera del tutto automatica utilizzando degli algoritmi non
noti e che potrebbero anche portarlo a collezionare questi stessi dati
in maniera errata.

Una volta attivata la funzionalità all'interno del proprio account
Analytics, lato Passweb sarà sufficiente abilitare il parametro
"**Raccolta Dati Utente GA**" presente all'interno della sezione Google
Analytics alla pagina "Sito -- Preferenze" del Wizard (tab
"**Tracciamento Dati**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_attivazione_upd_5.bmp](./assets/media/image26.png){width="5.726388888888889in"
height="3.34375in"}

**ATTENZIONE! per poter gestire in GA4 le conversioni avanzate, non è
sufficiente attivare il parametro "Raccolta Dati Utente GA" ma è
necessario anche attivare la relativa funzionalità all'interno di Google
Analytics stesso**

Dal punto di vista tecnico l'attivazione di questo parametro comporta
l'inserimento, in tutte le pagine web, della seguente istruzione

*gtag(\'set\', \'user_data\', {*

*\"**sha256_email_address\":* *valore hashato della mail utente*

*\"**sha256_phone_number\":* *valore hashato del telefono utente,*

*\"address\": {*

> *\"**sha256_first_name\":* *valore hashato del nome utente,*
>
> *\"**sha256_last_name\":* *valore hashato del cognome / ragione
> sociale utente,*
>
> *\"street\":* *indirizzo utente (via),*
>
> *\"city\":* *indirizzo utente (città),*
>
> *\"postal_code\":* *indirizzo utente (CAP),*
>
> *\"country\":* *indirizzo utente (Nazione)*
>
> *}*

*});*

subito dopo la "*gtag('config' ...*" in maniera tale che i dati utente,
se presenti, possano poi essere passati ad Analytics assieme a tutti i
diversi eventi già gestiti dal sistema di tracciamento.

Inoltre:

- l'istruzione "*gtag(\'set\', \'user_data\' ..."* sarà presente solo
  nel momento in cui a visitare la pagina dovesse essere un utente
  autenticato

- nel momento in cui un utente dovesse effettuare un ordine da "Ospite"
  la "*gtag(\'set\', \'user_data\' ..."* verrà eseguita alla conferma
  dell'ultimo step (quindi eventualmente prima di abbandonare il sito
  per essere ridiretti sul gateway di pagamento) oltre che, ovviamente,
  nella pagina di conferma ordine. In conseguenza di ciò, per ordini
  effettuati da utenti "Guest" i dati utente potranno essere inviati
  unicamente in relazione all'evento di purchase

- i parametri mail, telefono, ... saranno hashati come richiesto da
  google e verranno effettivamente inseriti nell'istruzione solo se il
  loro valore non dovesse essere nullo (nel caso in cui, ad esempio, per
  un dato utente non dovessimo avere disponibile il telefono il
  parametro *sha256_phone_number* non sarà inserito nel comando evitando
  quindi di passare a Google un dato nullo)

- relativamente agli eventi di "*sign_up*" l'istruzione "*gtag(\'set\',
  \'user_data\' ..."* verrà eseguita contestualmente all'evento stesso
  e, ovviamente, con i dati inseriti dall'utente in fase di
  registrazione. Nello specifico, in questo caso come dato utente
  collegato all'evento di *sign_up* verrà inviato solamente l'indirizzo
  mail

- relativamente agli eventi di "*generate_lead*" l'istruzione
  "*gtag(\'set\', \'user_data\' ..."* verrà eseguita contestualmente
  all'evento stesso e, anche in questo caso come dato utente collegato
  all'evento verrà inviato solamente l'indirizzo mail di chi ha
  compilato il form (quindi del lead).

> In questo senso sarà quindi di fondamentale importanza inserire
> all'interno del form un campo di tipo Email obbligatorio che l'utente
> dovrà valorizzare con il proprio indirizzo mail e, in fase di
> configurazione, impostare il parametro **Id/Name** del campo in
> oggetto sul valore "**email**"

- i dati utente verranno inseriti anche in eventuali chiamate server
  effettuate mediante Measurement Protocol (MP) verso Analytics nel
  momento in cui si dovesse decidere di abilitare anche questo tipo di
  tracciamento (parametro "**Google Analytics -- Abilita tracciamento
  server**")

