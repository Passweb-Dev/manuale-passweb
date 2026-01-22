# PARAMETRI GENERALI



La sezione "**Generale**" presente alla pagina "**Gestione DDos**" del
Wizard, consente di attivare / disattivare la funzione di blocco
automatico delle richieste indesiderate e di impostare i parametri che
andranno a definire le condizioni necessarie per far scattare un
determinato blocco.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_1.bmp](./assets/media/image276.png){width="5.571527777777778in"
height="3.422222222222222in"}

Nello specifico dunque il parametro:

**Abilita Prevenzione Attacchi DDos**: consente di attivare /
disattivare la funzione di blocco automatico delle richieste
indesiderate secondo i parametri successivamente impostati.

**ATTENZIONE!** nel caso in cui il parametro "Abilita Prevenzione
Attacchi DDos" dovesse essere disattivato, eventuali configurazioni di
blocco determinate dai restanti parametri presenti all'interno di questa
pagina non avranno alcun effetto. **Per poter applicare un qualsiasi
blocco è quindi indispensabile, per prima cosa, attivare il parametro in
questione**

**Numero Massimo di Richieste -- valore consigliato 31 --** Consente di
impostare il numero massimo di richieste che potranno arrivare sul sito,
nell'intervallo di tempo indicato (parametro "Intervallo Richieste"),
prima che scatti la regola di blocco.

**ATTENZIONE!** nel conteggio verranno prese in esame solo ed
esclusivamente richieste in GET a pagine del sito. Non verranno quindi
conteggiate né richieste di eventuali risorse statiche (immagini, file
css, file js ...) che la vista di una pagina potrebbe scatenare, né
tantomeno eventuali richieste POST collegate a funzioni specifiche
dell'applicativo (es. paginazione di determinati componenti,
visualizzazione di diverse sezioni di un tab ...)

**Intervallo Richieste -- valore consigliato 30000 --** Consente di
impostare l'intervallo di tempo (in millisecondi) entro cui dovrà
arrivare il numero massimo di richieste impostate mediante il precedente
parametro ("Numero massimo richieste"), per poter far scattare le regole
di blocco.

**Intervallo Divieto -- valore consigliato 900000 --** Consente di
impostare la durata (in millisecondi) di eventuali ban temporanei
applicati a seguito dell'attivazione di una condizione di blocco.

**ATTENZIONE!** eventuali blocchi temporanei di richieste provenienti da
determinati indirizzi IP e/o da determinati user agent verranno
automaticamente eliminati una volta trascorso l'intervallo di tempo
indicato all'interno di questo campo

**Abilita blocco permanente**: consente, se attivato, di abilitare un
blocco permanente per le richieste in arrivo da indirizzi IP e/o user
agent che hanno già fatto scattare, in precedenza, un certo numero
consecutivo di ban temporanei

Nello specifico, il blocco permanente verrà applicato secondo il
seguente schema:

- nel caso in cui dovesse arrivare da uno stesso indirizzo ip e/o da
  indirizzi ip appartenenti ad una stessa subnet mask e /o da uno stesso
  user agent, nell'intervallo di tempo indicato (parametro "Intervallo
  richieste"), un numero di richieste superiore a quello stabilito (
  parametro "Numero massimo richieste" ) verrà applicato automaticamente
  un primo **ban temporaneo** a seguito del quale tali richieste
  verranno automaticamente rifiutate dall'applicativo (con codice di
  errore 403).

> Il ban temporaneo sarà attivo per un intervallo di tempo pari a quello
> specificato all'interno del parametro "Intervallo Divieto".
>
> **ATTENZIONE!** Se, in queste condizioni (ban temporaneo attivo), ci
> si dovesse collegare al sito da uno degli ip bloccati e/o utilizzando
> uno degli user agent bloccati, la risposta che si otterrà sarà
> esattamente quella evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_2.bmp](./assets/media/image277.png){width="5.707638888888889in"
height="1.0715277777777779in"}

> Gli indirizzi IP e/o gli user agent bloccati a seguito
> dell'applicazione di un ban temporaneo potranno essere visualizzati
> alla pagina "**Real Time Monitor**" del Wizard (menu "*Configurazione
> -- DDos -- Real Time Monitor*")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_3.bmp](./assets/media/image278.png){width="5.707638888888889in"
height="3.4479166666666665in"}

- Trascorso l'intervallo di tempo indicato all'interno del parametro
  "Intervallo Richieste" il ban temporaneo verrà automaticamente rimosso
  e gli indirizzi IP / user agent precedentemente bloccati potranno
  tornare ad accedere normalmente al sito

> **ATTENZIONE!** per far scadere un ban temporaneo è necessario che non
> arrivino più richieste dagli ip / user agent bloccati per un periodo
> di tempo pari a quello impostato
>
> Supponendo dunque di aver impostato un blocco temporaneo di due minuti
> se, trascorso un solo minuto dall'attivazione del blocco, dovesse
> arrivare un ulteriore richiesta dall'indirizzo ip / user agent
> bloccato, questa farebbe ripartire il conteggio da zero per cui
> dovranno poi trascorrere due ulteriori minuti, sempre senza ricevere
> altre richieste dagli ip / user agent bloccati, prima che il blocco
> possa automaticamente essere eliminato.

- Nel caso in cui un determinato indirizzo ip / user agent dovesse
  essere sottoposto ad un ban temporaneo per due volte consecutivamente
  (nell'arco di 24 ore), il terzo eventuale ban sarà un **Long ban** ed
  avrà **una durata preimpostata e non modificabile di 24 ore**.

> **ATTENZIONE!** come per il ban temporaneo anche il Log ban terminerà
> automaticamente solo se per un periodo di 24 ore non arriveranno più
> richieste dall'indirizzo ip / user agent bloccato. Eventuali richieste
> in arrivo da ip / user agent bloccati faranno automaticamente
> ripartire il conteggio.

- Trascorse le 24 ore di blocco dovuto al Long ban gli indirizzi ip /
  user agent precedentemente bloccati potranno tornare a visitare
  normalmente il sito e, nel momento in cui dovessero farlo in maniera
  non corretta (superando nuovamente i limiti impostati per il blocco
  automatico) verranno nuovamente sottoposti prima a due ban temporanei
  e, successivamente, ad un secondo Long ban di altre 24 ore

- Infine, se a seguito del secondo Log ban e del relativo sblocco lo
  stesso indirizzo ip / user agent dovesse tornare ancora a dar fastidio
  al sito visitandolo in maniera non corretta, il successivo blocco sarà
  automaticamente un **ban permanente.**

> Verrà quindi inviata un'apposita mail all'amministratore del sito per
> informarlo del blocco applicato e l'indirizzo ip / user agent bloccato
> verrà automaticamente inserito tra l'elenco degli ip / user agent
> bannati presente alla pagina "**Lista deli IP/UA Bannati**" del Wizard

![Videate\\lista_ip_bannati.bmp](./assets/media/image279.png){width="5.941666666666666in"
height="3.5972222222222223in"}

> **ATTENZIONE!** eventuali ban permanenti potranno essere rimossi solo
> ed esclusivamente in maniera manuale andando ad eliminare l'indirizzo
> ip / user agent interessato dalla "**Lista degli IP/UA Bannati**"
> evidenziata in figura

**Ovviamente i parametri presenti all'interno di questa sezione che
determinano l'applicazione o meno di una regola di blocco, vanno settati
con molta attenzione perché, se non tarati in maniera corretta,
potrebbero anche portare al blocco di richieste "lecite" impedendo di
fatto la visualizzazione del sito anche ad utenti "umani".**

Il punto fondamentale, in questo senso, è cercare di capire se una
determinata frequenza di visite (numero di richieste e quindi di pagine
visitate in un determinato intervallo di tempo) può essere associata
effettivamente a utenti umani (che navigano il sito in maniera
"normale") o comunque a visite di bot "leciti", come possono essere i
bot di Google o di Bing (che navigano il sito al fine di indicizzarne le
pagine con una certa logica atta a non creare problemi al sito stesso),
oppure se la frequenza delle visite è tale da poterla associare a bot
malevoli (i cosiddetti "Bad Bot") o a diversi tool che in maniera e con
finalità più o meno lecite cercano di accedere alle pagine del nostro
sito.

Purtroppo non esistono valori predefiniti che possano assicurarci con
certezza che una determinata visita provenga da un utente "umano"
piuttosto che da un bot o da altri strumenti simili (anche perché le
possibilità di mascherare e modificare le richieste in arrivo al sito
facendole sembrare umane, sono tante e neppure difficili da applicare).

Sicuramente però se dovessimo ricevere, ad esempio, un centinaio di
visite a pagine diverse da uno stesso indirizzo ip nel giro di una
decina di secondi potremmo facilmente assumere che quelle visite non
siano umane e che quindi l'unica finalità che hanno è quella di causare
più o meno volutamente problemi al sito.

Detto ciò i valori proposti a default da Passweb in corrispondenza dei
campi presenti all'interno della sezione "Generale" possono sicuramente
essere un ottimo punto di partenza.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ddos_9.bmp](./assets/media/image280.png){width="5.792361111111111in"
height="3.571527777777778in"}

Nel caso in cui si dovesse decidere di utilizzare tali valori, eventuali
regole di blocco verranno applicate nel momento in cui dovessero
arrivare al sito **almeno 31 richieste** in un **intervallo di tempo
pari a 30 secondi**, il che in sostanza significa che per applicare un
blocco il sito dovrà ricevere dalla stesso ip o da ip appartenenti ad
una stessa subnet mask o da uno degli user agent selezionati, negli
ultimi 30 secondi più di una visita al secondo (comportamento questo che
con ottima approssimazione possiamo ipotizzare non umano).

In queste condizioni inoltre il ban temporaneo applicato da Passweb sarà
di

**ATTENZIONE**! in ogni caso, i valori proposti a default da Passweb
possono essere modificati secondo le specifiche esigenze del caso in un
qualsiasi momento.

