# SEO -- SOCIAL TAG



La sezione "**Social Tag**", presente all'interno del menu **"Preferenze
--SEO"** consente di abilitare la gestione dei social media tag per la
condivisione, all'interno dei vari social network, dei contenuti
pubblicati sul proprio sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\seo_social_tag.bmp](./assets/media/image50.png)

**Gestione dei Social Media Tag:** consente di abilitare o meno **la
gestione del protocollo** **Opengraph** facilitando così la condivisione
dei contenuti del proprio sito web all'interno dei vari social network.

In sostanza tentando di condividere su un social network i contenuti di
una pagina del proprio sito, potrebbe capitare che all'interno del
social venga condivisa un'immagine e/o una descrizione casuale, presente
sì nella pagina che l'utente ha deciso di condividere ma non esattamente
quella che volevamo fosse effettivamente inviata al social.

Questo tipo di problema è dovuto al fatto che nel codice sorgente della
pagina web mancano appositi riferimenti mediante i quali poter
specificare esattamente quali contenuti della pagina dovranno essere
inviati ai vari social in fase di condivisione.

Il protocollo Opengraph (http://ogp.me/) introdotto da Facebook nel
2010, ed oggi utilizzato anche da tutti i maggiori social network
(Twitter, Linkedin. Google +, Pinterest ....), risolve questo tipo di
problema specificando come dovranno essere inseriti questi riferimenti e
definendo quindi un insieme di regole mediante le quali poter
specificare esattamente quali contenuti della pagina web dovranno essere
inviati al social in fase di condivisone.

In realtà questa è solo una piccola parte delle funzioni del protocollo
Opengraph, più in generale questo protocollo, che rispecchia la
specifica RDF (Resource Description Framework) in quanto sfrutta i
meta-tag in pagina, permette a ciascuna pagina presente in Internet di
essere rappresentata sotto forma di un oggetto, caratterizzato da alcune
proprietà chiave, e di poter essere inclusa in quello che viene chiamato
"grafo sociale" ovvero una sorta di mappatura di tutte le pagine
Internet e di quello che esse rappresentano e contengono.

Selezionando il parametro **"Gestione dei Social Media Tag"** Passweb
andrà dunque ad inserire automaticamente, nella sezione \< head \> di
tutte le pagine del sito appositi Meta Tag all'interno dei quali
verranno specificate le informazioni che dovranno poi essere inviate al
social nel momento in cui un visitatore del sito dovesse decidere di
condividere quella specifica pagina.

Più nel dettaglio, verranno inseriti i seguenti Meta Tag:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opengraph_tag1.bmp](./assets/media/image51.png)

- **meta property=\"og:title\" content=\"titolo dell'oggetto da
  condividere\"**

> Consente di specificare il titolo dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto indicato per il tag Title della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Title si veda anche la sezione *"Sito -- Preferenze -- SEO Nome
> del sito e configurazione Tag Title"* di questo manuale
>
> Nel caso in cui non dovesse essere indicato nessun Title di pagina il
> Meta Tag in oggetto non verrà inserito.

- **meta property=\"og:type\" content=\"tipologia\"**

> Consente di specificare il tipo dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb in base alla
> specifica pagina e, ovviamente, ai valori ammessi dallo specifico
> social. Nel caso ad esempio di una pagina generica il valore di questo
> tag sarà impostato su content="website" mentre nel caso di una pagina
> Prodotto potrebbe essere invece impostato sul valore
> content="product.item"

- **meta property=\"og:url\" content="indirizzo della pagina web"**

> Consente di specificare l' url dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide
> ovviamente con l'indirizzo completo della pagina web condivisa

- **meta property=\"og:image\" content=\"indirizzo dell'immagine\"**

> Consente di specificare l' url di un immagine che rappresenta
> l'oggetto, nel nostro caso la pagina web, che verrà condiviso sul
> social.
>
> In questo caso occorre poi considerare che per le **Pagine Prodotto**
> il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, sarà esattamente l' url dell'immagine principale presente
> nella scheda prodotto del relativo articolo.
>
> Per pagine in cui è stata inserito il componente "**Dettaglio CMS**"
> il contenuto di questo tag sarà invece l' url dell' Immagine Articolo
> (se presente) o quello dell' Immagine Sommario (se presente).
>
> Infine, per Pagine Generiche (e prive del componente "Dettaglio News")
> il tag in oggetto non viene inserito automaticamente da Passweb per
> cui non esiste, per questo tipo di pagine, un'immagine di default da
> inviare al social in fase di condivisione. In queste condizioni sarà
> quindi necessario inserire manualmente il tag in oggetto nella
> specifica pagina indicando espressamente l' url dell'immagine che la
> rappresenta e che dovrà quindi essere inviata al social in fase di
> condivisione.
>
> Per maggiori informazioni relativamente a come impostare manualmente
> Meta Tag per una specifica pagina si veda anche la sezione **"***Live
> Editing -- Pagine -- Pagine Generiche***"** di questo manuale.
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere presente, in una
> Pagina Prodotto l'immagine prodotto e/o in una Pagina "Dettaglio News"
> l'immagine articolo o sommario, il tag in oggetto non verrà inserito
> (così come avviene per le pagine generiche se non indicato
> espressamente). In queste condizioni dunque l'immagine inviata al
> social in fase di condivisione verrà prelevata dal social stesso in
> maniera del tutto casuale.

- **meta property=\"og:description\" content=\"Descrizione\"**

> Consente di specificare la descrizione dell'oggetto, nel nostro caso
> della pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto impostato per il Meta Tag Description della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Description si veda anche quanto precedentemente indicato
> all'interno di questo stesso capitolo

- **meta property=\"og:site_name\" content=\"nome del sito\"**

> Consente di specificare il nome del sito web che incapsula l'oggetto
> condiviso.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> il "Nome Sito".
>
> Per maggiori informazioni relativamente a come impostare il nome del
> proprio sito web si veda anche la sezione *"Sito -- Preferenze -- SEO
> Nome del sito e configurazione Tag Title"* di questo manuale

- **meta property=\"fb:app_id\" content=\"id dell'app facebook\"**

> Facebook, per una miglior condivisone dei contenuti all'interno della
> piattaforma, consiglia anche di creare un apposita APP e indicare l'id
> di questa stessa APP in fase di condivisione di un contenuto.
>
> Il Meta Tag in oggetto viene quindi inserito da Passweb nel momento in
> cui si dovesse decidere di seguire questo consiglio e sarà ovviamente
> valorizzato con l'ID della propria APP.
>
> In questo senso è possibile utilizzare la stessa APP creata per
> consentire agli utenti del sito di effettuare la registrazione e
> l'accesso al sito stesso mediante il proprio profilo Facebook. Per
> maggiori informazioni relativamente a come creare questa APP e su dove
> indicare, all'interno di Passweb, il relativo ID si veda anche la
> sezione "*Sito -- Preferenze -- Social Media - Facebook*" di questo
> manuale.

I Meta Tag esaminati fino a questo momento sono, in generale, più che
sufficienti per condividere immagini e testi all'interno di tutti i
maggiori social network (non solamente in facebook).

E' bene sottolineare però che alcuni social, come ad esempio Twitter o
Google+, pur sfruttando sempre il protocollo Opengraph implementano
anche dei tag "proprietari" e, ovviamente, consigliano per una miglior
condivisione sulla loro piattaforma di utilizzare proprio questi tag.

In questo senso quindi Passweb si preoccuperà di inserire
automaticamente, per Twitter e Google+ rispettivamente, anche i seguenti
meta tag:

[TWITTER]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opengraph_tag2.bmp](./assets/media/image52.png)

- **meta name=\"twitter:card\" content=\"tipologia\"**

> Consente di specificare il tipo dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb in base alla
> specifica pagina e, ovviamente, ai valori ammessi dallo specifico
> social. Nel caso ad esempio di una pagina generica il valore di questo
> tag sarà impostato su content="summary" mentre nel caso di una pagina
> Prodotto potrebbe essere invece impostato sul valore content="product"

- **meta name=\"twitter:title\" content=\" Titolo della pagina\"**

> Consente di specificare il titolo dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto indicato per il tag Title della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Title si veda anche la sezione *"Sito -- Preferenze -- SEO Nome
> del sito e configurazione Tag Title"* di questo manuale
>
> Nel caso in cui non dovesse essere indicato nessun Title di pagina il
> Meta Tag in oggetto non verrà inserito

- **meta name=\"twitter:description\" content=\" Descrizione\"**

> Consente di specificare la descrizione dell'oggetto, nel nostro caso
> della pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto impostato per il Meta Tag Description della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Description si veda anche quanto precedentemente indicato
> all'interno di questo stesso capitolo

- **meta name=\"twitter:image\" content=\"indirizzo dell'immagine\"**

> Consente di specificare l' url di un immagine che rappresenta
> l'oggetto, nel nostro caso la pagina web, che verrà condiviso sul
> social.
>
> In questo caso occorre poi considerare che per le **Pagine Prodotto**
> il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, sarà esattamente l' url dell'immagine principale presente
> nella scheda prodotto del relativo articolo.
>
> Per pagine in cui è stata inserito il componente "**Dettaglio CMS**"
> il contenuto di questo tag sarà invece l' url dell' Immagine Articolo
> (se presente) o quello dell' Immagine Sommario (se presente).
>
> Infine, per Pagine Generiche (e prive del componente "Dettaglio News")
> il tag in oggetto non viene inserito automaticamente da Passweb per
> cui non esiste, per questo tipo di pagine, un'immagine di default da
> inviare al social in fase di condivisione. In queste condizioni sarà
> quindi necessario inserire manualmente il tag in oggetto nella
> specifica pagina indicando espressamente l' url dell'immagine che la
> rappresenta e che dovrà quindi essere inviata al social in fase di
> condivisione.
>
> Per maggiori informazioni relativamente a come impostare manualmente
> Meta Tag per una specifica pagina si veda anche la sezione **"***Live
> Editing -- Pagine -- Pagine Generiche***"** di questo manuale.
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere presente, in una
> Pagina Prodotto l'immagine prodotto e/o in una Pagina "Dettaglio News"
> l'immagine articolo o sommario, il tag in oggetto non verrà inserito
> (così come avviene per le pagine generiche se non indicato
> espressamente). In queste condizioni dunque l'immagine inviata al
> social in fase di condivisione verrà prelevata dal social stesso in
> maniera del tutto casuale.

- **meta name=\"twitter:site\" content=\"Account di Twitter \"**

> Twitter, per una miglior condivisone dei contenuti all'interno della
> piattaforma, consiglia anche di indicare il proprio Account Twitter.
>
> Il Meta Tag in oggetto viene quindi inserito da Passweb nel momento in
> cui si dovesse decidere di seguire questo consiglio e sarà valorizzato
> con l'Account indicato nel campo "**Account Twitter**" presente alla
> pagina "**Sito -- Preferenze -- Social Media**" del Wizard (sezione
> Twitter).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_twitter.bmp](./assets/media/image53.png)

[GOOGLE +]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\opengraph_tag3.bmp](./assets/media/image54.png)

- **meta itemprop=\"name\" content=\" Titolo della pagina \"**

> Consente di specificare il titolo dell'oggetto, nel nostro caso della
> pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto indicato per il tag Title della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Title si veda anche la sezione *"Sito -- Preferenze -- SEO Nome
> del sito e configurazione Tag Title"* di questo manuale
>
> Nel caso in cui non dovesse essere indicato nessun Title di pagina il
> Meta Tag in oggetto non verrà inserito

- **meta itemprop=\"description\" content=\"Descrizione\"**

> Consente di specificare la descrizione dell'oggetto, nel nostro caso
> della pagina web, che verrà condiviso sul social.
>
> Il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, viene impostato automaticamente da Passweb e coincide con
> quanto impostato per il Meta Tag Description della relativa pagina.
>
> Per maggiori informazioni relativamente a come impostare in Passweb il
> tag Description si veda anche quanto precedentemente indicato
> all'interno di questo stesso capitolo

- **meta itemprop=\"image\" content=\"indirizzo dell'immagine\"**

> Consente di specificare l' url di un immagine che rappresenta
> l'oggetto, nel nostro caso la pagina web, che verrà condiviso sul
> social.
>
> In questo caso occorre poi considerare che per le **Pagine Prodotto**
> il contenuto di questo tag, e quindi il valore effettivamente
> condiviso, sarà esattamente l' url dell'immagine principale presente
> nella scheda prodotto del relativo articolo.
>
> Per pagine in cui è stata inserito il componente "**Dettaglio CMS**"
> il contenuto di questo tag sarà invece l' url dell' Immagine Articolo
> (se presente) o quello dell' Immagine Sommario (se presente).
>
> Infine, per Pagine Generiche (e prive del componente "Dettaglio News")
> il tag in oggetto non viene inserito automaticamente da Passweb per
> cui non esiste, per questo tipo di pagine, un'immagine di default da
> inviare al social in fase di condivisione. In queste condizioni sarà
> quindi necessario inserire manualmente il tag in oggetto nella
> specifica pagina indicando espressamente l' url dell'immagine che la
> rappresenta e che dovrà quindi essere inviata al social in fase di
> condivisione.
>
> Per maggiori informazioni relativamente a come impostare manualmente
> Meta Tag per una specifica pagina si veda anche la sezione **"***Live
> Editing -- Pagine -- Pagine Generiche***"** di questo manuale.
>
> **ATTENZIONE!** Nel momento in cui non dovesse essere presente, in una
> Pagina Prodotto l'immagine prodotto e/o in una Pagina "Dettaglio News"
> l'immagine articolo o sommario, il tag in oggetto non verrà inserito
> (così come avviene per le pagine generiche se non indicato
> espressamente). In queste condizioni dunque l'immagine inviata al
> social in fase di condivisione verrà prelevata dal social stesso in
> maniera del tutto casuale.

