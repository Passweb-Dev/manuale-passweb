# ONETRUST



Nel momento in cui l'esigenza dovesse essere quella di attivare e
gestire il blocco preventivo dei cookie appoggiandosi alla piattaforma
di Iubenda (<https://www.onetrust.it/> )sarà necessario:

1.  Configurare dal proprio account OneTrust tutto il necessario per
    generare correttamente sia l'Informativa estesa (catalogando tutti i
    cookie in uso sul sito) che il Banner necessario per gestire l'
    Informativa breve

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\onetrust1.bmp](./assets/media/image13.png){width="5.590972222222222in"
height="3.33125in"}

> Per maggiori informazioni relativamente a come configurare su OneTrust
> l'Informativa estesa e la Cookie Solution si rimanda alla relativa
> documentazione di prodotto.

2.  Una volta completata la configurazione e la generazione
    dell'Informativa estesa e del Banner necessario per gestire l'
    Informativa breve sarà necessario prelevare il codice di
    integrazione fornito dalla piattaforma terza

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\onetrust2.bmp](./assets/media/image14.png){width="5.590972222222222in"
height="3.33125in"}

> ed inserirlo all'interno del campo "**Code Snippet Cookie**" presente
> alla pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento
> Dati**" sezione "**Blocco Preventivo**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\code_snippet_cookie.bmp](./assets/media/image6.png){width="5.740277777777778in"
height="3.623611111111111in"}

> Una volta inserito correttamente lo script di integrazione, nel
> momento in cui un utente dovesse effettuare per la prima volta
> l'accesso al sito verrà visualizzato l'apposito banner di consenso e
> di gestione dei cookie

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\onetrust4.bmp](./assets/media/image15.png){width="5.590972222222222in"
height="3.2402777777777776in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\onetrust5.bmp](./assets/media/image16.png){width="5.590972222222222in"
height="3.2402777777777776in"}

> e non verranno rilasciati cookie di profilazione o di terze parti fino
> a che l'utente non abbia fornito esplicitamente il proprio consenso
> cliccando sull'apposito pulsante di accettazione

3.  Impostare il parametro "**Blocco Preventivo dei Cookie**" presente
    anch'esso alla pagina "**Sito -- Preferenze**" del Wizard (tab
    "**Tracciamento Dati**" sezione "**Blocco Preventivo**") sul valore
    "**OneTrust**"

> L'impostazione di questo parametro garantisce che il blocco preventivo
> dei cookie effettuato da OneTrust funzioni correttamente in relazione
> a:

- Componenti nativi di Passweb che fanno uso di **Google Map** (es.
  Google Map, Store locator ecc...)

- Componente nativo di Passweb per la gestione dei **Video** (YouTube,
  Vimeo )

- **Video di YouTube o di Vimeo** inseriti nella pagina web mediante
  componenti Paragrafo, HTML o CMS e quindi mediante l'utilizzo
  esplicito di un tag \< iframe \> con src impostata sui domini
  [www.youtube.com](http://www.youtube.com) oppure su
  [www.vimeo.com](http://www.vimeo.com)

> **ATTENZIONE!** per maggiori informazioni in merito al blocco
> automatico di video YouTube o Vimeo non gestiti con il componente
> "Video" di Passweb si veda anche quanto indicato al punto 6

- Utilizzo di **Google Recaptcha** (mediante l'apposita funzione e i
  relativi componenti Passweb)

- Attivazione del tracciamento di **Google Analytics** (implementato
  mediante le funzionalità native di Passweb)

- Attivazione del tracciamento **Facebook** (implementato mediante le
  funzionalità native di Passweb)

- Attivazione del tracciamento **Brainlead** (implementato mediante le
  funzionalità native di Passweb)

> In queste condizioni dunque nel momento in cui un visitatore dovesse
> accedere ad una pagina del sito in cui è presente, ad esempio, un
> componente Google Map o un Video YouTube, il blocco preventivo di
> OneTrust si preoccuperà di disattivare tali componenti impedendo
> quindi il rilascio dei relativi cookie fintanto che l'utente non
> decida di accettarne l'utilizzo cliccando sull'apposito pulsante
> presente all'interno del banner dell' Informativa Breve.
>
> Una volta accettato l'utilizzo dei cookie questi componenti verranno
> sbloccati e tutto tornerà a funzionare correttamente.

4.  Nel momento in cui si dovesse decidere di implementare all'interno
    del proprio sito l'integrazione con un qualunque altro servizio di
    terze parti che dovesse far uso di cookie non strettamente tecnici
    (es. Hotjar, Pulsanti social, live chat ...), l'amministratore del
    sito dovrà preoccuparsi di attivare, anche in merito a questi stessi
    servizi, il blocco preventivo dei cookie di OneTrust utilizzando
    l'apposita procedura di tagging manuale

> **ATTENZIONE!** eventuali servizi di terze parti installati sul sito
> che dovessero rilasciare cookie non tecnici dovranno essere bloccati
> mediante operazioni di tagging manuale.
>
> **Non dovrà quindi mai essere attivata l'opzione di blocco automatico
> offerto dalla piattaforma terza, cosa questa che potrebbe
> compromettere il corretto funzionamento del sito.**
>
> **ATTENZIONE! Passweb non può sapere a priori quali servizi di terze
> parti l'utente ha deciso di attivare. In conseguenza di ciò sarà
> compito dell'amministratore del sito verificare se il servizio in
> questione utilizzi effettivamente dei cookie non tecnici, quali siano
> ed eventualmente gestirne il blocco preventivo.**
>
> In questo senso le operazioni da effettuare per attivare il blocco
> preventivo di script che potrebbero installare cookie, prevedono
> essenzialmente di apportare a tali script alcune semplici modifiche in
> maniera tale che One Trust possa prevenirne l'esecuzione nei casi in
> cui non è stato ancora prestato il relativo consenso
>
> Nello specifico sarà necessario:

- **Applicare a questi script una specifica classe (es.
  optanon-category-C0003)**

- **Cambiare l'attributo type di questi script da text/javascript a
  text/plain** (o eventualmente aggiungere l'attributo type =
  "text/plain" se questo non dovesse essere presente)

> Supponendo quindi che lo script originale sia del tipo di quello di
> seguito indicato
>
> \<script **type = "text/javascript"** src= "file_javascript.js"\>
>
> ....
>
> \</script\>
>
> per poterne prevenire l'esecuzione nei casi in cui non è stato ancora
> prestato il consenso, questo stesso script dovrà essere modificato in
> questo modo
>
> \<script **type = "text/plain"** **class = "optanon-category-C0003"**
> src=\"file_javascript.js\"\>
>
> ....
>
> \</script\>

5.  La stessa operazione di tagging manuale descritta al punto 4 dovrà
    essere utilizzata anche in relazione a specifici tag \< iframe \>
    per i quali è stato verificato l'utilizzo di cookie non tecnici.

> In questo senso infatti occorre ricordare che in determinati casi
> anche l'utilizzo di un semplice \< iframe \> potrebbe portare al
> rilascio di cookie di profilazione o di terze parti che dovranno
> quindi essere sottoposti a blocco preventivo.
>
> **In queste condizioni per evitare il rilascio di cookie prima che
> l'utente abbia espresso il proprio consenso sarà necessario:**

- **Cambiare l'attributo src dell'iframe in data-src**

- **Assegnare all'iframe una specifica classe (es.
  optanon-category-C0003)**

> Supponendo dunque che l'iframe originale per il quale abbiamo
> verificato l'utilizzo di cookie di profilazione sia del tipo
>
> \< iframe src = "http://www.dominiosito.com" \> \< /iframe \>
>
> per poter applicare il blocco preventivo dei cookie dovrà essere
> modificato in questo modo
>
> \< iframe **class = "optanon-category-C0003"** **data-src =
> "http://www.dominiosito.com"** \> \< /iframe \>

6.  Fanno eccezione rispetto a quanto indicato al punto 5, i video di
    YouTube e di Vimeo inseriti all'interno della pagina web mediante
    componenti CMS, Paragrafo o HTML e quindi mediante l'utilizzo
    esplicito di un tag \< iframe \>

> In questo senso infatti occorre sottolineare che, attivando il blocco
> preventivo di One Trust, Passweb effettuerà, in automatico, un
> controllo su tutti gli iframe presenti all'interno del sito che
> risultino avere la sorgente (attributo src) impostata sui seguenti
> domini:

- **www.youtube.com**

- **www.vimeo.com** con il parametro di querystring **dnt** assente o
  impostato sul valore **0** oppure sul valore **false**

> e, sempre in maniera automatica provvederà a sostituire il markup HTML
> di questi iframe con quello richiesto specificatamente da One Trust
> per bloccare questo tipo di risorse.
>
> In questo senso è bene sottolineare anche che tanto YouTube quanto
> Vimeo offrono comunque la possibilità di incorporare video all'interno
> di una pagina web senza che questi rilascino cookie di profilazione e
> senza quindi che questi stessi video vengano eventualmente bloccati e
> non mostrati agli utenti che dovessero aver rifiutato l'utilizzo di
> cookie di profilazione (per maggiori informazioni in merito si veda
> anche quanto indicato all'interno del precedente capitolo
> "*Informativa Estesa o Cookie Policy*" di questo manuale).
>
> Nel momento in cui dunque il codice per embeddare i video di YouTube
> e/o di Vimeo all'interno della pagina web dovesse essere generato in
> maniera tale da non far rilasciare a questi video cookie di
> profilazione, il markup del corrispondente iframe non verrebbe
> modificato e i video stessi verrebbero sempre visualizzati
> indipendentemente dalle scelte fatte dagli utenti in materia di
> gestione dei cookie

**ATTENZIONE!** **Per maggiori informazioni relativamente a come poter
implementare con OneTrust il blocco di script o di elementi che
potrebbero installare cookie si consiglia di fare riferimento sempre
alla relativa guida presente sul portale di OneTrust
(<https://my.onetrust.com/s/article/UUID-c5122557-2070-65cb-2612-f2752c0cc4aa>
,
<https://my.onetrust.com/s/article/UUID-3dc06342-ff6b-3578-5024-6d7c05d03283>
)**
