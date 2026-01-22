# GESTIONE ALIAS



La sezione "**Gestione Alias**" consente di:

- definire ed associare ad ogni singola pagina del sito, e per ogni
  lingua gestita, uno o più Alias differenti, offrendo anche all'utente
  la possibilità di decidere se tali Alias dovranno essere considerati
  come "indirizzi di default" per la relativa pagina (ed essere quindi
  visualizzati nella barra degli indirizzi del browser), oppure come
  "redirect" in maniera tale da poter gestire eventuali errori 301. --
  **Alias Pagine / Articoli**

- creare apposite regole di reindirizzamento mediante le quali poter
  mappare url generici (compresi anche di eventuali parametri di query
  string) su indirizzi specifici del proprio sito web -- **Redirects**

Ora, prima di passare ad esaminare nel dettaglio le varie sottosezioni
di questo menu del Wizard, è bene chiarire che cosa sia un Alias di
pagina e quando possa o debba essere effettivamente utilizzato.

In Passweb ad ogni pagina corrisponde a default un ben preciso url
definito dalla posizione occupata dalla pagina stessa all'interno
dell'albero delle pagine. Supponendo ad esempio di avere a che fare, per
il sito **www.nome_sito.passweb.it**, con un albero del tipo di quello
indicato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\albero_pagine_alias.bmp](./assets/media/image471.png){width="5.902777777777778in"
height="3.3180555555555555in"}

alla pagina "Dettaglio" corrisponderà l' url
**www.nome_sito.passweb.it/blog/archivio-notizie/dettaglio**

**Un Alias di pagina altro non è se non un indirizzo personalizzato, e
differente dunque da quello assegnato a default da Passweb, attraverso
cui poter mappare e richiamare la pagina in esame.**

Facendo sempre riferimento al caso sopra indicato si potrebbe pensare,
ad esempio, di associare alla pagina web in esame un Alias del tipo:
**archivio-notizie/notizie-recenti**

In questo modo la pagina "Archivio News" risponderà correttamente sia
all'indirizzo assegnatole a default da Passweb
(**www.nome_sito.passweb.it/archivi-cms/archivio-news)** sia all'Alias
definito per la pagina stessa
(**www.nome_sito.passweb.it/archivio-notizie/notizie-recenti).**

Nella barra degli indirizzi del Browser potrà poi essere visualizzato
l'indirizzo assegnatole a default da Passweb oppure il suo Alias
dipendentemente dal fatto di aver configurato l'Alias stesso come un
**Redirect** oppure come **Indirizzo di default** per la pagina in
esame.

La possibilità di configurare questi Alias come dei Redirect, in
particolare, consente all'utente di gestire eventuali errori 301
(spostamento definitivo di URL ad un nuovo indirizzo) che si possono
originare quando si effettua il porting di un sito NON Passweb (con una
sua struttura di url) in ambiente Passweb, quando una pagina web già
indicizzata (e presente quindi nei risultati di ricerca di Google) viene
spostata in un\'altra posizione dell'albero delle pagine, quando gli
viene cambiato nome o comunque quando vengono effettuate operazioni che
determinano in qualche modo una modifica del suo effettivo url.

**ATTENZIONE! La gestione degli errori 301 e, conseguentemente, la
corretta codifica di Alias di pagina impostati come Redirect, è di
fondamentale importanza per indicare agli spider dei vari motori di
ricerca quale sia la versione attualmente corretta del url di una pagina
web, permettendo poi al motore di visualizzare l' url corretto nei suoi
risultati di ricerca.**

**ATTENZIONE! All'interno di Passweb è possibile abilitare anche una
gestione automatica degli Alias in maniera tale da non doversi
preoccupare, ad esempio, di creare manualmente un Alias dopo aver
modificato il nome di una pagina o di un articolo lasciando questo
compito all'applicativo e minimizzando così sia gli errori di creazione
che gli errori di tipo 404.**

Per maggiori informazioni su come abilitare e gestire la generazione
automatica degli Alias si veda anche la sezione "*Sito -- Preferenze --
SEO Alias*" di questo manuale

