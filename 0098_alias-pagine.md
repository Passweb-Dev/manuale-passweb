# ALIAS PAGINE



All'interno di questa sezione è possibile definire e gestire gli Alias
di tutte le pagine ad eccezione di quelli relativi alle specifiche
Pagine Prodotto.

Nel caso in cui l'esigenza dovesse essere dunque quella di definire un
Alias per una pagina prodotto del tipo
**www.miosito.it/catalogo-articoli/prodotti/informatica/accessori/apple/magic-mouse,**
sarà necessario agire dalla sezione "Alias Articoli" impostando l'Alias
stesso in corrispondenza dell'articolo "Magic Mouse".

Per maggior informazioni in merito si veda anche il successivo capitolo
di questo manuale.

**ATTENZIONE! non è possibile definire da questa sezione del Wizard (né
manualmente né tanto meno mediante import di file csv) Alias di Pagina
che contengano parametri di query string.**

Nel momento in cui l'esigenza dovesse essere quindi quella di
reindirizzare url con parametri di query string su specifiche pagine del
proprio sito sarà necessario agire all'interno della sezione "*Gestione
Alias / Redirects*" creando apposite regole di reindirizzamento (per
maggiori informazioni in merito si veda anche il successivo capitolo
"Redirects" di questo manuale)

Accedendo a questa sezione del Wizard verrà quindi visualizzata la
maschera "**Gestione Alias Pagine**" suddivisa in due distinte sezioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_pagina_1.bmp](./assets/media/image472.png){width="5.759722222222222in"
height="3.3895833333333334in"}

- nella parte sinistra è visualizzato l'albero delle pagine del proprio
  sito

- nella parte destra vengono invece visualizzati gli Alias associati
  alla pagina attualmente selezionata all'interno dell'albero

**ATTENZIONE!!!: gli Alias di pagina sono gestiti a livello di Variante
Sito. Per poter quindi visualizzare e/o gestire gli Alias di una
specifica Variante è necessario per prima cosa caricare la Variante
stessa all'interno del Wizard**

Per maggiori informazioni sulla gestione delle Varianti Sito si veda la
sezione *"Live Editing -- Varianti Sito"* di questo manuale

I due pulsanti presenti nella barra degli strumenti contestuale
all'Albero delle Pagine consentono rispettivamente di:

- **Importa da file** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_da_file.bmp](./assets/media/image473.png){width="0.5583333333333333in"
  height="0.175in"} ): consente di importare in maniera massiva gli
  Alias di pagina partendo da un file .csv o .txt. Cliccando su questo
  pulsante verrà infatti aperta la maschera di importazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importa_alias.bmp](./assets/media/image474.png){width="5.759722222222222in"
height="3.3895833333333334in"}

> all'interno della quale poter indicare:

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  l'elenco dei vari Alias di Pagina che dovranno essere importati

- **Lingua:** consente di indicare la lingua del sito a cui dovranno
  fare riferimento gli Alias indicati all'interno del file di
  importazione

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

> Il parametro "**Elimina Alias non presenti nel file**" consente, se
> selezionato di eliminare, a seguito della procedura di importazione,
> eventuali Alias già codificati ma non indicati e quindi non presenti
> nel file di importazione.
>
> Affinchè la procedura di import possa funzionare in maniera corretta,
> consentendo a Passweb di codificare automaticamente gli Alias di
> pagina sulla base dei dati presenti all'interno del file, è necessario
> che il file di importazione sia stato creato rispettando determinate
> regole. Nello specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il file da importare non deve avere particolari intestazioni

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- E' necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180**.

> **ATTENZIONE!** In questo senso è quindi necessario che il valore dei
> campi contenenti interruzioni di riga, doppi apici e/o lo stesso
> carattere utilizzato anche come separatore **sia necessariamente
> racchiuso da virgolette**

- Supponendo di aver indicato il ; come carattere separatore, il formato
  del file di importazione dovrà essere di questo tipo:

> **\<permalink pagina\>;\<alias\>;\<redirect\>;\<default\>**
>
> dove
>
> **\<permalink pagina\> 🡪** indica **l' url relativo** **(privo di /
> iniziale)** assegnato in Passweb alla specifica pagina per cui si vuol
> creare un Alias
>
> **ATTENZIONE!** il permalink della pagina, viene utilizzato come
> chiave nella procedura di associazione automatica degli alias alle
> pagine del sito, per cui deve essere necessariamente indicato nella
> lingua corrente di visualizzazione dell'albero delle pagine (lingua
> questa che corrisponde a quella impostata come default all'interno
> dell'apposito campo "Lingua di default" presente nella sezione *"Sito
> -- Gestione lingue del Wizard"*)
>
> In altri termini per individuare il permalink corretto da inserire nel
> file di importazione è necessario prestare particolare attenzione al
> nome della specifica pagina attualmente visualizzato nell'albero delle
> pagine.
>
> **\<alias\> 🡪** indica l'alias che si intende associare al permalink e
> quindi alla pagina indicata nel campo precedente
>
> **\<redirect\> 🡪** necessario per indicare se l'alias in esame dovrà
> essere impostato o meno come Redirect. **Sono ammessi i soli valori S
> o N**
>
> **\<default\> 🡪** necessario per indicare se l'alias in esame dovrà
> essere impostato o meno come indirizzo di default per la relativa
> pagina. **Sono ammessi i soli valori S o N**
>
> **Esempio**:
>
> **articoli-in-offerta;offerte;S;N** 🡪 Consente di creare un alias per
> la pagina www.miosito.it/articoli-in-offerta. L'alias si chiamerà
> semplicemente "offerte", per cui a seguito della sua creazione la
> stessa pagina risponderà anche all' url www.miosito.it\\offerte.
> L'alias sarà inoltre impostato come Redirect e NON come indirizzo di
> default
>
> Nel caso in cui la lingua di visualizzazione corrente dell'albero
> delle pagine, e quindi la lingua di default del sito, fosse l'inglese
> e la pagina in oggetto assumesse ancora il nome assegnatole a default
> da Passweb, ossia "Articoli in Offerta-en", il record da inserire
> all'interno del file di importazione dovrà essere il seguente:
>
> **articoli-in-offerta-en;offerte;S;N**
>
> **ATTENZIONE!** Nel tracciato del file csv di importazione potrebbe
> anche essere aggiunto un ulteriore ultimo campo (**\<automatico\>**)
> utilizzato per definire se l'Alias in questione è stato creato
> automaticamente (valore S) o in maniera manuale (valore N).
>
> Tale campo, presente nel caso in cui si operi, ad esempio, partendo da
> un file csv esportato direttamente da Passweb, **non verrà comunque
> considerato in fase di importazione** **dati**.
>
> **Per tutti gli Alias presenti all'interno del file di importazione il
> campo "Automatico" verrà infatti impostato sempre a "N"**

- **Esporta** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image475.png){width="0.31805555555555554in"
  height="0.1625in"} ): consente di esportare l'elenco degli Alias di
  pagina attualmente codificati all'interno di un file .csv. Cliccando
  su questo pulsante verrà infatti visualizzata la maschera di
  esportazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esporta_alias.bmp](./assets/media/image476.png){width="5.759722222222222in"
height="3.3895833333333334in"}

> all'interno della quale poter indicare:

- **Lingua:** consente di indicare la lingua in relazione alla quale
  esportare gli Alias di pagina

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che dovrà essere utilizzato all'interno
  del file come separatore per i vari campi

> Il parametro "**Includi pagine senza Alias**" consente di decidere se
> dovranno o meno essere inseriti, all'interno del file esportato, anche
> i record relativi alle pagine del sito cui non è attualmente associato
> nessun Alias.
>
> L'ultimo campo di ogni record presente nel file di esportazione
> rappresenta il flag "Automatico" ed è valorizzato a:

- **S** nel caso in cui l'Alias corrispondente sia stato generato
  automaticamente dall'applicazione

- **N** nel caso in cui l'Alias corrispondente sia stato creato in
  maniera manuale

> I permalink presenti nel file di esportazione saranno sempre indicati
> nella lingua corrente di visualizzazione dell'albero delle pagine.
>
> **ATTENZIONE!** Nel momento in cui il sito dovesse avere diversi alias
> codificati e si dovessero apportare svariate modifiche a questi stessi
> Alias, il modo più veloci di procedere potrebbe essere quello di
> esportare gli Alias attualmente codificati, apportare le modifiche
> necessarie al file scaricato ed effettuare un nuovo import di questo
> stesso file selezionando, magari, anche l'opzione relativa
> all'eliminazione degli alias non indicati all'interno del file di
> importazione

Per creare manualmente un nuovo Alias sarà invece sufficiente
selezionare la pagina cui si vuole associare questo stesso Alias e,
successivamente, cliccare sul pulsante "**Nuovo**" presente nella barra
degli strumenti della parte destra della maschera.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_alias.bmp](./assets/media/image477.png){width="5.759722222222222in"
height="3.3895833333333334in"}

All'interno della maschera "**Nuovo Alias**" sarà quindi necessario
assegnare un valore ai seguenti parametri:

- **Alias:** consente di definire l'Alias da associare alla pagina
  attualmente selezionata all'interno dell'albero.

> **ATTENZIONE! Nel definire un nuovo Alias vanno indicati solo ed
> esclusivamente percorsi relativi.**
>
> Nel caso in cui dunque, l'intenzione fosse quella di associare alla
> pagina
>
> *www.nome_sito.passweb.it/archivi-cms/archivio-news*
>
> l'Alias
>
> *www.nome_sito.passweb.it/archivio-notizie/notizie-recenti*
>
> all'interno di questo campo andrebbe specificata semplicemente la
> stringa archivio-notizie/notizie-recenti
>
> **ATTENZIONE! in fase di conferma verrà effettuato un controllo di
> univocità in maniera tale da verificare che l'Alias che si sta
> tentando di inserire non corrisponda ad una pagina del sito
> effettivamente presente e/o che non sia già stato associato ad
> un\'altra pagina del sito.**
>
> Tale controllo terrà conto, ovviamente, di quello che è il formato che
> si è scelto di adottare il permalink delle pagine del proprio sito
> (per maggiori informazioni in merito si veda anche la sezione "*Sito
> -- Preferenze -- Seo Permalink*" di questo manuale)
>
> Nel momento in cui si dovesse verificare che l'alias inserito sia già
> stato utilizzato su di un\'altra pagina del sito e/o che corrisponda
> all' url di una pagina effettivamente on line non sarà possibile,
> ovviamente, effettuarne il salvataggio.
>
> **In fase di definizione di un Alias, inoltre, è possibile utilizzare
> come Wildcard, con il significato dunque di "qualsiasi carattere",
> anche il carattere speciale "%"**
>
> Supponendo quindi di codificare per la pagina "Contatti" del sito un
> Alias di questo tipo:
>
> ***azienda/%***

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_wildcard.bmp](./assets/media/image478.png){width="5.532638888888889in"
height="3.2534722222222223in"}

> il risultato che otterremo sarà esattamente quello di ridirigere
> automaticamente sulla pagina Contatti del sito tutti gli url il cui
> path relativo inizia con la stringa "azienda/".
>
> In queste condizioni dunque nel caso in cui il path relativo del url
> dovesse essere ad esempio:

- ***aziendalivorno***: l'alias non verrà considerato

- ***azienda/chi-siamo***: l'alias verrà correttamente individuato e
  l'utente verrà quindi indirizzato sulla pagina "contatti" del sito

- ***azienda/info/societa***: l'alias verrà correttamente individuato e
  l'utente verrà quindi indirizzato sulla pagina "contatti" del sito

> Il carattere Wildcard può essere utilizzato, ovviamente, in un
> qualsiasi punto dell'Alias per cui oltre all'esempio appena analizzato
> potremmo anche creare alias del tipo di quelli di seguito indicati

- ***%/test**:* in questo caso tutti gli url il cui path relativo
  terminerà con "/test" verranno automaticamente ridiretti sulla pagina
  di definizione dell'Alias

- ***test%/prova:*** in questo caso tutti gli url il cui path relativo
  inizierà con la stringa "test" e terminerà con la stringa "prova"
  verranno automaticamente ridiretti sulla pagina di definizione
  dell'Alias

- ***%test%prova%:*** in questo caso tutti gli url il cui path relativo
  conterrà in una qualsiasi posizione sia la stringa "test" che la
  stringa "prova" verranno automaticamente ridiretti sulla pagina di
  definizione dell'Alias

- *...*

> **ATTENZIONE! Il carattere Wildcard può essere utilizzato, con lo
> stesso significato ovviamente, non solo in fase di definizione manuale
> di un singolo Alias ma anche all'interno del file csv/txt utilizzato
> per l'import massivo degli Alias di Pagina**

- **Lingua:** consente di selezionare, tra quelle attualmente gestite,
  la specifica lingua per cui considerare valido l'Alias che si sta
  realizzando. Nel caso di siti multilingua è quindi possibile definire
  per ogni pagina uno specifico Alias per ogni lingua gestita.

- **Redirect:** se selezionato consente di utilizzare l'Alias che si sta
  realizzando come Redirect sulla corrispondente pagina del proprio
  sito.

> Un possibile caso d'uso in questo senso potrebbe essere dato dalle
> necessità di indicizzazione legate al trasferimento di un sito NON
> Passweb in ambiente Passweb.
>
> In questo senso infatti occorre considerare che, ovviamente, ogni sito
> NON Passweb ha un suo specifico formato degli indirizzi associati alle
> pagine web, indirizzi questi che potrebbero essere del tipo
> www.nomesito/nome_pagina1/nome_pagina2.html oppure del tipo
> www.nomesito/nome_pagina1/nome_pagina2_parametri_di_query.aspx o
> ancora del tipo
> www.nomesito/nome_pagina1/nome_pagina2_parametri_di_query.php ecc\...
>
> Considerando quindi un sito già esistente saranno chiaramente questi
> gli indirizzi indicizzati dai vari motori di ricerca e riportati come
> risultati ad esempio in una ricerca effettuata su Google.
>
> Nel momento in cui questo sito dovesse essere portato in ambiente
> Passweb le pagine del sito assumerebbero a default gli indirizzi
> assegnati da Passweb con lo standard utilizzato da Passweb stesso. In
> queste condizioni dunque le vecchie pagine precedentemente indicizzate
> e i relativi risultati visualizzati in Google non sarebbero più validi
> per cui gli utenti che dovessero tentare di visitare queste pagine
> partendo dai risultati di ricerca offerti da Google di fatto non
> riuscirebbero a visualizzare nulla (gli verrebbe ritornato un errore
> 404 di pagina non esistente, in conseguenza del fatto che
> effettivamente quella specifica pagina del tipo
> www.nomesito/nome_pagina1/nome_pagina2_parametri_di_query.aspx ora non
> esiste più).
>
> **La gestione degli Alias offerta da Passweb, con l'impostazione
> Redirect, consente di evitare questo tipo di problemi informando
> inoltre i vari motori di ricerca della modifica nell'indirizzo della
> pagina ricercata "costringendoli" inoltre ad aggiornare i loro
> risultati**.
>
> Sarebbe quindi sufficiente, dopo aver effettuato il porting di un sito
> NON Passweb, in ambiente Passweb, associare ad ogni pagina del sito un
> Alias corrispondente all'indirizzo che la relativa pagina aveva prima
> del passaggio, impostando inoltre questi stessi Alias come Redirect.
>
> Considerando quindi che in questo modo la pagina del sito Passweb, per
> quello che è il funzionamento degli Alias, potrà essere richiamata sia
> dal suo indirizzo di default (in standard Passweb) sia dai suoi Alias,
> anche nel caso in cui un utente dovesse trovare tra i risultati
> indicati da Google il vecchio indirizzo della pagina web, cliccando su
> esso verrebbe comunque visualizzata la corrispondente pagina del sito
> Passweb. Inoltre Google riuscirà anche a capire che la nuova pagina
> viene visualizzata a seguito di un redirect generato da un errore di
> tipo 301 (spostamento definitivo di URL ad un nuovo indirizzo),
> leggerà quindi il nuovo indirizzo e aggiornerà di conseguenza i suoi
> risultati di ricerca (indicizzando di fatto la nuova pagina Passweb).
>
> In queste condizioni va infine considerato che nella barra degli
> indirizzi del browser verrà comunque visualizzato non l'Alias
> associato alla pagina ma l'indirizzo di default assegnatole da Passweb
> secondo quello che è lo standard utilizzato da Passweb stesso.

**NOTA BENE**: selezionando per un Alias il parametro **Redirect** nella
barra degli indirizzi del browser verrà sempre visualizzato l'indirizzo
assegnato alla pagina stessa, a default, da Passweb secondo quello che è
lo standard di Passweb.

- **Indirizzo di default:** se selezionato consente di utilizzare
  l'Alias che si sta realizzando come Indirizzo di Default per la
  corrispondente pagina del proprio sito.

> In queste condizioni nel momento in cui l'utente dovesse digitare,
> nella barra degli indirizzi del browser, l'indirizzo assegnato a
> default da Passweb alla pagina in esame o un qualsiasi altro Alias di
> questa stessa pagina, verrà automaticamente ridiretto, **con codice
> 301**, sull'indirizzo impostato come default.
>
> Si potrebbe quindi pensare di utilizzare questo tipo di soluzione, ad
> esempio, per fornire un formato degli indirizzi web delle pagine del
> proprio sito contenente un maggior numero di informazioni
> relativamente alla specifica pagina visitata o comunque un formato più
> semplice, e magari più facile da ricordare, rispetto a quello che gli
> verrebbe assegnato direttamente da Passweb in base alla struttura
> dell'albero delle pagine attualmente utilizzato.

**NOTA BENE**: non è possibile selezionare contemporaneamente entrambi i
flag "Redirect" e "Indirizzo di default"

**ATTENZIONE!** Nel caso in cui l'Alias indicato sia già stato
utilizzato o assegnato da Passweb stesso ad un'altra pagina del sito, il
pulsante "Salva" sarà disabilitato e non sarà quindi possibile terminare
la codifica del nuovo Alias.

Per ciascuno degli Alias presenti in griglia è indicato:

- Se l'Alias in esame è o meno un Redirect (prima colonna)

- Se l'Alias in esame è o meno il Default (seconda colonna)

- Se l'Alias in esame è o meno un alias Automatico (terza colonna)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\alias_automatici_e_manuali.bmp](./assets/media/image479.png){width="5.759722222222222in"
height="3.50625in"}

> Gli Alias automatici possono poi essere gestiti, ricercati e
> modificati al pari di quelli creati in maniera manuale. Ovviamente nel
> caso in cui si dovessero apportare delle modifiche ad Alias
> automatici, al salvataggio, questi diverranno a tutti gli effetti
> Alias manuali per cui scomparirà il flag A di automatico e la riga
> corrispondente non sarà più evidenziata in blu.

- La lingua di riferimento dell'Alias (quarta colonna)

- Lo slug dell'Alias, ossia la parte relativa del vecchio url di pagina
  (ultima colonna)

I due pulsanti visualizzati nella barra degli strumenti della parte
destra della maschera nel momento in cui si dovesse selezionare uno
degli alias attualmente associati alla pagina selezionata consentiranno
infine di:

- **Modifica Alias** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image349.png){width="0.35694444444444445in"
  height="0.16875in"} ): consente di modificare l'Alias di pagina
  attualmente selezionato

- **Elimina Alias** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image347.png){width="0.31805555555555554in"
  height="0.16875in"} ): consente di eliminare definitivamente l'Alias
  di pagina attualmente selezionato

