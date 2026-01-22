# BRAINLEAD



**ATTENZIONE! Per usufruire dell'integrazione tra Passweb e Brainlead è
necessario attivare per prima cosa il relativo modulo su Passstore**

Brainlead ( <https://brainlead.it> ) è una piattaforma italiana di
**Data Tracking** e **Marketing Automation** che consente di monitorare
e segmentare i clienti del proprio sito ecommerce, di acquisire i lead
generati dalle campagne di marketing tracciandone il comportamento e
creando anche funnel di vendita completi ai quali poter collegare poi
diverse azioni di marketing automation.

La piattaforma si pone quindi a metà tra i software di web analytics
"puri", come possono essere Google Analytics o Matomo, e sistemi di mail
marketing come MailChimp o Active Campaign; traccia il comportamento
degli utenti all'interno del sito, li profila e utilizza le informazioni
raccolte per le attività di conversione alle vendite (carrelli
abbandonati, cross selling, up selling ...), attività queste che possono
essere eseguite su diversi canali: Email, SMS, Whatsapp ...

La sezione "**Brainlead -- Marketing automation software**" del tab
"**Tracciamento Dati**" consente quindi di impostare tutti i parametri
di configurazione necessari per attivare il tracciamento ed inviare i
relativi dati alla piattaforma in oggetto

![](./assets/media/image202.png)

**ATTENZIONE!** Brainlead è uno strumento che offre diverse possibilità
di configurazione e di gestione della marketing automation; può essere
integrato nativamente con i siti Passweb attraverso l'impostazione di
semplici parametri ma rimane comunque un software di terze parti
indipendente da Passweb che richiede, al fine di poter essere utilizzato
al meglio in tutte le sue funzionalità, specifiche conoscenze.

All'interno di questo manuale è presente un'apposita sezione
(*Brainlead*) per approfondire un po' le conoscenze e l'utilizzo di
questo strumento avendo comunque sempre ben chiaro che lo scopo del
presente manuale **non è** **quello di offrire una guida completa
all'utilizzo e alla configurazione di questa piattaforma.** Nel momento
in cui l'esigenza dovesse essere quella di approfondire ulteriormente
questo argomento si consiglia quindi di fare riferimento sempre alla
documentazione ufficiale e al relativo supporto tecnico.

Fatta questa doverosa considerazione passiamo ora ad analizzare nel
dettaglio i diversi parametri che consentono di attivare e configurare
il collegamento diretto tra il proprio sito Passweb e Brainlead.

- **Brainlead API Key:** consente di inserire la chiave API necessaria
  per l'integrazione tra le due piattaforme. La chiave in questione può
  essere prelevata direttamente dal back office di Brainlead all'interno
  della sezione "**Impostazioni -- Gestisci API**" (campo "**API Key**")

![](./assets/media/image203.png)

> **ATTENZIONE!** nel momento in cui la chiave api inserita all'interno
> del campo in questione non dovesse essere esattamente quella presente
> anche nel back office di Brainlead la comunicazione tra le due
> piattaforme non potrà avvenire in maniera corretta

- **window.\_bl_cid / window.\_bl\_ msid** **:** parametri necessari per
  gestire correttamente il tracciamento lato client delle pageview
  collegandolo anche agli eventi inviati a Brainlead lato server
  (creazione di carrelli e ordini).

> I parametri in questione possono essere prelevati direttamente dallo
> script di tracciamento presente nel back office di Brainlead
> all'interno della sezione "**Web Visits**" (campo "**Codice HTML**")

![](./assets/media/image204.png)

> **ATTENZIONE!** lo script di tracciamento Brainlead è già presente in
> Passweb in maniera nativa.
>
> Di base quindi, per attivare questo tipo di tracciamento è sufficiente
> valorizzare in maniera corretta i due parametri sopra evidenziati.
>
> Se necessario è comunque possibile personalizzare e gestire in maniera
> manuale lo script inserendolo all'interno del successivo campo
> "**Codice di tracciamento**"

- **Codice di tracciamento**: consente di impostare manualmente lo
  snippet di codice necessario per attivare il tracciamento lato client
  di Brainlead.

> **ATTENZIONE!** Nel caso in cui non ci sia la necessità di
> personalizzare il codice di monitoraggio è sufficiente valorizzare in
> maniera corretta i due parametri **window.\_bl_cid /
> window.\_bl_msid** precedentemente analizzati lasciano vuoto il campo
> "Codice di tracciamento"
>
> Nel momento in cui dovesse essere invece necessario apportare delle
> personalizzazioni al codice di tracciamento (ad esempio per poterlo
> utilizzare in maniera corretta assieme ad una piattaforma CMP non
> integrata nativamente in Passweb) sarà sufficiente copiare lo snippet
> di codice direttamente dal backend di Brainlead, incollarlo
> all'interno del campo in oggetto e apportare qui tutte le
> personalizzazioni richieste.
>
> In queste condizioni il valore dei due parametri **window.\_bl_cid /
> window.\_bl\_ msid** può essere inserito direttamente nello snippet di
> codice oppure all'interno dei relativi campi Passweb.
>
> In quest'ultimo caso sarà poi necessario modificare lo snippet di
> codice inserendo al posto del valore di questi due parametri i
> seguenti segnaposto

- **\$CID_BRAINLEAD\$ -** sostituito a runtime con quanto inserito
  all'interno del campo Passweb **window.\_bl_cid**

- **\$MSID_BRAINLEAD\$ -** sostituito a runtime con quanto inserito
  all'interno del campo Passweb **window.\_bl_msid**

> Inoltre, per poter consentire a Passweb, di collegare in maniera
> corretta il tracciamento lato client con quello lato server, sarà di
> fondamentale importanza inserire all'interno dello snippet di
> tracciamento, immediatamente al di sotto dei due parametri
> window.\_bl_cid / window.\_bl_msid, anche il segnaposto di seguito
> indicato

- **\$ID_SESSIONE_CARRELLO\$** - necessario per consentire a Passweb di
  collegare in maniera corretta gli eventi client a quelli server

> In definitiva dunque, posto di aver inserito il valore dei due
> parametri window.\_bl_cid / window.\_bl_msid all'interno dei relativi
> campi Passweb lo snippet da inserire all'interno del campo "Codice di
> tracciamento" dovrà essere del tipo di quello qui di seguito indicato
>
> *\< script type=\'text/javascript\' \>*
>
> ***var \_bl_cid = \$CID_BRAINLEAD\$;***
>
> ***var \_bl_msid = \$MSID_BRAINLEAD\$;***
>
> ***\$ID_SESSIONE_CARRELLO\$***
>
> *var \_bl_track = document.createElement(\'script\');*
>
> *\_bl_track.async = true;*
>
> *\_bl_track.type = \'text/javascript\';*
>
> *\_bl_track.src = \'https://analytics.brainlead.it/analytics.js\';*
>
> *var s = document.getElementsByTagName(\'script\');*
>
> *if (s.length) {*
>
> *s\[0\].parentNode.appendChild(\_bl_track);*
>
> *} else {*
>
> *var s_h = document.getElementsByTagName(\'head\');*
>
> *s_h.length && trackcmp_h\[0\].appendChild(\_bl_track);*
>
> *}*
>
> *\< /script \>*
>
> **ATTENZIONE!** verificare sempre che lo script sopra evidenziato sia
> effettivamente lo stesso presente anche all'interno del backoffice di
> Brainlead

**ATTENZIONE!** **anche se Brainlead offre specifiche funzioni di
marketing automation, rimane pur sempre un sistema di tracciamento e di
profilazione degli utenti**

In conseguenza di ciò nel momento in cui si dovesse decidere di attivare
e gestire questo tipo di tracciamento sarà necessario, da una parte
fornire, nelle Norme sulla gestione della privacy del proprio sito,
un'informativa adeguata circa l'utilizzo della piattaforma terza e,
dall'altra parte, verificare di aver gestito in maniera corretta la
richiesta di consenso preventivo come effettivamente richiesto dalla
normativa GDPR.

Per ulteriori informazioni relativamente all'integrazione Passweb --
Brainlead si veda anche quanto indicato nel relativo capitolo di questo
manuale

