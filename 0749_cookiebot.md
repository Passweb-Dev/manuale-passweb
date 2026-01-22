# COOKIEBOT



Nel momento in cui l'esigenza dovesse essere quella di attivare e
gestire il blocco preventivo dei cookie appoggiandosi alla piattaforma
di Cookiebot (<https://www.cookiebot.com>) sarà necessario:

1.  Configurare su Cookiebot tutto il necessario per consentire al
    servizio di scansionare il proprio sito web in modo tale da rilevare
    i cookie attualmente in uso, classificarli e generare così le
    corrispondenti informative.

> Per maggiori informazioni relativamente a come configurare Cookiebot
> si rimanda alla documentazione presente sul relativo portale
> (<https://www.cookiebot.com/it/help/>)
>
> **ATTENZIONE!** In relazione a questa configurazione è fondamentale
> accertarsi di aver impostato la "**Modalità di blocco dei cookie**"
> (sezione "**I tuoi script**") sull'opzione "**Manuale**"

![](./assets/media/image10.png)

> **Impostando infatti l'opzione in esame sul valore "Automatico"
> potrebbe poi essere compromessa l'intera funzionalità del sito**

2.  Una volta completata la configurazione sulla piattaforma di
    Cookiebot, sarà necessario prelevare il codice di integrazione
    (sezione "**I tuoi script**")

![](./assets/media/image11.png)

> ed inserirlo all'interno del campo "**Code Snippet Cookie**" presente
> alla pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento
> Dati**" sezione "**Blocco Preventivo**")

![](./assets/media/image6.png)

> Il secondo script invece è relativo alla "**Cookie Declaration**" e,
> volendo, potrebbe anche essere inserito solo in una specifica pagina
> del sito (es. la pagina relativa alla Privacy o quella specifica della
> Cookie Policy)

![](./assets/media/image12.png)

3.  Impostare il parametro "**Blocco Preventivo dei Cookie**" presente
    anch'esso alla pagina "**Sito -- Preferenze**" del Wizard (tab
    "**Tracciamento Dati**" sezione "**Blocco Preventivo**") sul valore
    "**CookieBot**" o "**CookieBot + Consent Mode**" (dipendentemente
    dal fatto di voler gestire o meno, in relazione al tracciamento di
    Google Analytics, anche la Consent Mode)

> L'impostazione di questo parametro garantisce che il blocco preventivo
> dei cookie effettuato da CookieBot funzioni correttamente in relazione
> a:

- Componenti nativi di Passweb che fanno uso di **Google Map** (es.
  Google Map, Store locator ecc...)

- Componente nativo di Passweb per la gestione dei **Video** (YouTube,
  Vimeo)

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
> Cookiebot si preoccuperà di disattivare tali componenti impedendo
> quindi il rilascio dei relativi cookie fintanto che l'utente non
> decida di accettarne l'utilizzo.
>
> Una volta accettato l'utilizzo dei cookie questi componenti verranno
> sbloccati e tutto tornerà a funzionare correttamente.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente all'opzione
> "**Cookiebot + Consent Mode**" si rimanda a quanto indicato
> all'interno del capitolo "*Google Analytics -- Google Analytics 4 --
> Universal Analytics e GA4 Principali differenze -- Privacy e Raccolta
> dei dati -- Consent Mode*" di questo manuale

4.  Nel momento in cui si dovesse decidere di implementare all'interno
    del proprio sito l'integrazione con un qualunque altro servizio di
    terze parti che dovesse far uso di cookie non strettamente tecnici
    (es. Hotjar, Pulsanti social, live chat ...), l'amministratore del
    sito dovrà preoccuparsi di attivare, anche in merito a questi stessi
    servizi, il blocco preventivo dei cookie secondo quanto specificato
    nel blocco manuale previsto da Cookiebot

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
> essenzialmente di apportare a tali script alcune semplici modifiche
> (<https://www.cookiebot.com/it/installazione-manuale/>) in maniera
> tale che Cookiebot possa prevenirne l'esecuzione nei casi in cui non è
> stato ancora prestato il relativo consenso
>
> Nello specifico sarà necessario:

- **Applicare a questi script l'attributo "data-cookieconsent" e
  impostare il suo valore su una o più delle categorie di cookie
  "preferences", "statistics" e "marketing" in base ai tipi di cookie
  effettivamente impostati dal relativo script.**

> Nel caso in cui un dato script dovesse rilasciare ad esempio sia
> cookie di marketing che cookie statistici l'attributo
> "data-cookieconsent" dovrà essere impostato sui valori "marketing" e
> "statistics" separati da , (data-cookieconsent =
> "statistics,marketing"

- **Cambiare l'attributo type di questi script da text/javascript a
  text/plain**

> Supponendo quindi che lo script originale sia del tipo di quello di
> seguito indicato e che rilasci solo cookie di marketing
>
> \<script **type = "text/javascript"** src= "file_javascript.js"\>
>
> ....
>
> \</script\>
>
> per poterne prevenire l'esecuzione nei casi in cui non sia stato
> ancora prestato il relativo consenso, questo stesso script dovrà
> essere modificato in questo modo
>
> \<script **type = "text/plain"** **data-cookieconsent="marketing"**
> src=\"file_javascript.js\"\>
>
> ....
>
> \</script\>

5.  Un'operazione di tagging manuale del tutto analoga a quella
    descritta al punto 4 dovrà essere utilizzata anche in relazione a
    specifici tag \< iframe \> per i quali è stato verificato l'utilizzo
    di cookie non tecnici
    (<https://support.cookiebot.com/hc/en-us/articles/360003790854-Iframe-cookie-consent-with-YouTube-example>)

> In questo senso infatti occorre ricordare che in determinati casi
> anche l'utilizzo di un semplice \< iframe \> potrebbe portare al
> rilascio di cookie di profilazione o di terze parti che dovranno
> quindi essere sottoposti a blocco preventivo.
>
> **In queste condizioni per evitare il rilascio di cookie prima che
> l'utente abbia espresso il proprio consenso sarà necessario:**

- **Assegnare il link sorgente dell'iframe non nel tag src ma bensì
  all'interno di un attributo data-src**

- **Assegnare all'iframe** **l'attributo "data-cookieconsent" e
  impostare il suo valore su una o più delle categorie di cookie
  "preferences", "statistics" e "marketing" in base ai tipi di cookie
  effettivamente impostati dal relativo iframe.**

> Supponendo dunque che l'iframe originale per il quale abbiamo
> verificato l'utilizzo di cookie marketing sia del tipo
>
> \< iframe src = "http://www.dominiosito.com" frameborder=\"0\"
> allowfullscreen \> \< /iframe \>
>
> per poter applicare il blocco preventivo dei cookie dovrà essere
> modificato in questo modo
>
> \< iframe **data-src = "http://www.dominiosito.com" data-cookieconsent
> = "marketing"** frameborder=\"0\" allowfullscreen \>
>
> \< /iframe \>

6.  Fanno eccezione rispetto a quanto indicato al punto 5, i video di
    YouTube e di Vimeo inseriti all'interno della pagina web mediante
    componenti CMS, Paragrafo o HTML e quindi mediante l'utilizzo
    esplicito di un tag \< iframe \>

> In questo senso infatti occorre sottolineare che, attivando il blocco
> preventivo di Cookiebot, Passweb effettuerà, in automatico, un
> controllo su tutti gli iframe presenti all'interno del sito che
> risultino avere la sorgente (attributo src) impostata sui seguenti
> domini:

- **www.youtube.com**

- **www.vimeo.com** con il parametro di querystring **dnt** assente o
  impostato sul valore **0** oppure sul valore **false**

> e, sempre in maniera automatica provvederà a sostituire il markup HTML
> di questi iframe con quello richiesto specificatamente da Cookiebot
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
implementare con Cookiebot il blocco di script o di elementi che
potrebbero installare cookie si consiglia di fare riferimento sempre
alla relativa documentazione presente sul portale di Cookiebot**

