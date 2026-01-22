# INFORMATIVA ESTESA O COOKIE POLICY



Tenendo conto di quanto indicato nel precedente capitolo di questo
manuale, il primo passo da fare per soddisfare la normativa vigente in
materia di cookie, sarà quello di individuare l'elenco completo dei
cookie utilizzati dal proprio sito.

Per fare questo è possibile ricorrere ad uno dei tanti servizi presenti
on line oppure utilizzare in autonomia gli strumenti di sviluppo del
proprio browser (come indicato, ad esempio, in [[questa
guida]{.underline}](https://www.iubenda.com/it/help/290-quali-cookie-usi))

Una volta ottenuto tale elenco è necessario poi fare dei distinguo. La
cookie law prevede infatti di distinguere fra i seguenti tipi di cookie:

- **cookie tecnici**: sono quelli necessari per il normale funzionamento
  del sito;

- **cookie di profilazione**: servono ad acquisire informazioni
  personali sui visitatori (gusti e interessi ...)

- **cookie di terze parti**: sono cookie installati da servizi esterni
  (es. Google Analytics, video YouTube, Social Network ...)

> **ATTENZIONE:** Tutti i tag script, iframe e img utilizzati
> all'interno del proprio sito e che fanno riferimento ad altri siti
> potrebbero installare dei cookie

In tutto questo dunque è importante conoscere esattamente quelli che
sono i cookie che possono essere installati direttamente da Passweb e
quelli che invece sono i cookie installati da un servizio di terze
parti.

Nello specifico, per quel che riguarda Passweb occorre considerare che:

- Ogni sito Passweb installa, sul browser dei visitatori, il seguente
  **cookie tecnico**: **ASP.NET_SessionId** con una durata pari alla
  sessione di navigazione

> **ATTENZIONE!** Questo cookie viene utilizzato nei siti sviluppati con
> Microsoft.Net. Quando un utente inizia a navigare, viene creato un ID
> di sessione univoco, che tiene traccia di tutte le informazioni
> relative a quella specifica sessione. Queste informazioni vengono
> memorizzate nel server Web e vengono identificate tramite un GUID. Il
> GUID è essenziale per fare in modo che un qualsiasi sito ASP.NET possa
> funzionare in maniera corretta

- L'inserimento nella pagina web di determinati componenti Passweb,
  nello specifico **quelli che prevedono l'utilizzo della Google Map o
  dei Video (YouTube, Vimeo ecc...)**, potrebbe comportare
  l'installazione, sul browser dei visitatori, di determinati cookie di
  profilazione.

> Per quel che riguarda la **Google Map** ad esempio è bene evidenziare
> che ogni mappa installa sul browser dei visitatori un cookie
> denominato **NID** e classificato, generalmente, come cookie di
> profilazione. Tale cookie viene infatti utilizzato per memorizzare le
> preferenze utente e altre informazioni, come ad esempio la lingua
> preferita, il numero di risultati di ricerca preferiti ecc....
>
> Allo stesso modo un **video di YouTube** potrebbe installare nel
> browser dei visitatori, tra gli altri, un cookie denominato **PREF**
> anch'esso classificato come cookie di profilazione e utilizzato
> essenzialmente per memorizzare informazioni quali la configurazione di
> pagina preferita, le preferenze di riproduzione dell\'utente...
>
> Per quel che riguarda, nello specifico, i video di YouTube o di Vimeo
> è bene sottolineare però che queste piattaforme offrono comunque la
> possibilità di incorporare video all'interno di una pagina web senza
> che questi rilascino cookie di profilazione e senza quindi che questi
> stessi video vengano eventualmente bloccati e non mostrati agli utenti
> che dovessero aver rifiutato l'utilizzo di cookie.
>
> In particolare per ottenere ciò, nel caso di YouTube sarà necessario
> selezionare, in fase di individuazione del codice di condivisione, il
> parametro "**Abilita modalità di privacy avanzata**" evidenziato in
> figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\cookie_youtube.bmp](./assets/media/image1.png)

> In questo modo infatti il video incorporato all'interno della pagina
> avrà come sorgente un dominio diverso da YouTube (nello specifico
> **www.youtube-nocookie.com**) non rilascerà alcun cookie di
> profilazione e quindi non sarà sottoposto a nessun tipo di blocco
> preventivo.
>
> Nel caso di **Vimeo** per ottenere lo stesso risultato sarà necessario
> invece inserire nell' url di condivisione il parametro di query string
> **dnt=1** come indicato anche nella relativa documentazione
> (https://developer.vimeo.com/api/oembed/videos) ottenendo così come
> sorgente dell'iframe un url del tipo
> "https://vimeo.com/xxxxxx**?dnt=1**"

- L'utilizzo del **Google recaptcha mediante i relativi componenti
  Passweb** comporta l'installazione, sul browser dei visitatori, di un
  cookie denominato **\_GRECAPTCHA** classificato come cookie di
  profilazione e utilizzato per memorizzare informazioni come: i cookie
  inseriti da Google negli ultimi 6 mesi, quanti clic del mouse sono
  stati fatti su quella schermata, le informazioni CSS per quella
  pagina, la data esatta ...

- L'attivazione dell'integrazione tra Passweb e Google Analytics
  potrebbe comportare l'installazione, sul browser dei visitatori, di
  determinati cookie di profilazione.

> Detto che, secondo quanto indicato dal Garante, il cookie di Google
> Analytics, **se anonimizzato**, può essere considerato un cookie
> tecnico e quindi non essere soggetto al blocco preventivo, l'effettivo
> utilizzo o meno di cookie di profilazione, in questo caso, dipende
> ovviamente non da Passweb ma da come è stato configurato Analytics e
> quindi da quale tipo di informazioni si è deciso di tracciare

**ATTENZIONE!** **In ogni caso per maggiori informazioni relativamente
agli specifici cookie rilasciati a seguito dell'utilizzo dei suddetti
componenti Passweb, si consiglia di fare riferimento sempre al servizio
terzo** (Google, YouTube, Vimeo ecc...) oppure di inserire, ove
concesso, nella propria informativa estesa il link diretto del relativo
servizio (es. <https://policies.google.com/technologies/cookies> )

A questo punto, dopo aver individuato e classificato tutte le tipologie
di cookie utilizzate dal proprio sito, la cookie law impone, come detto,
l'obbligo di redigere una informativa estesa (cookie policy) e di
linkarla a tutte le pagine del sito.

**ATTENZIONE! l'informativa estesa o "cookie policy", da non confondere
con la "privacy policy" va redatto se si utilizzano cookie di qualsiasi
tipo.**

Tale informativa dovrebbe contenere:

- Specifiche informazioni su cosa siano i cookie;

- Categoria del cookie utilizzato (tecnici, terze parti, profilazione);

- Finalità del cookie utilizzato;

- Scadenza del cookie;

- I cookie di terze parti con i link ai singoli servizi;

- Il responsabile dei trattamenti dei dati con indicazione di contatto;

- Indicazioni sulla gestione dei cookie dal proprio browser.

Nel momento in cui non si dovesse essere in grado di individuare /
classificare tutti i cookie utilizzati dal sito, in relazione anche a
quelli che possono essere i servizi terzi attivati, o di redigere in
maniera corretta un' "Informativa estesa" è possibile appoggiarsi ad
appositi servizi online che facilitano notevolmente questo tipo di
operazioni.

Un' esempio, in questo senso, è quello di Iubenda
(<https://www.iubenda.com> ), un servizio questo che, tra l'altro, si
può integrare anche con il proprio sito Passweb per gestire il blocco
preventivo dei cookie rilasciati dai componenti nativi precedentemente
indicati (per maggiori informazioni in merito, si veda anche quanto
indicato nel successivo capitolo di questo manuale)

