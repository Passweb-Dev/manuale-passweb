# PUNTI VENDITA



La sezione **" Punti Vendita",** accessibile dalla voce di menu
principale "Ordini", consente di impostare e configurare i diversi punti
vendita gestiti all'interno del sito e che potranno poi essere
utilizzati, ad esempio, per realizzare delle spedizioni di tipo "Ritiro
in Sede".

All'interno di questa pagina verrà quindi visualizzata la maschera
**"Lista dei Punti Vendita"**

![](./assets/media/image354.png)

in cui sono elencati tutti i Punti Vendita attualmente attivabili ed
utilizzabili all'interno del sito.

La creazione di un nuovo Punto Vendita varia in relazione alla tipologia
di sito considerata.

**[ECOMMERCE MEXAL]{.underline}**

**Per i siti Ecommerce collegati a Mexal ogni Punto Vendita corrisponde
ad un ben preciso indirizzo di spedizione codificato sul gestionale
all'interno della relativa tabella "Anagrafica indirizzi di spedizione",
in maniera tale da non risultare associato ad uno specifico cliente
(campo "Cliente/Forn = Tutti").**

In queste condizioni dunque per poter utilizzare un nuovo Punto Vendita
è necessario:

1.  Codificare lato Mexal un apposito indirizzo di spedizione facendo
    attenzione a non associare questo stesso indirizzo ad uno specifico
    cliente.

![](./assets/media/image355.png)

**NOTA BENE**: indirizzi di spedizione associati a specifici clienti non
verranno considerati tra gli indirizzi dei punti vendita.

2.  Effettuare una sincronizzazione Sito -- Gestionale in maniera tale
    da poter visualizzare il nuovo Punto Vendita tra quelli presenti
    nella lista sopra evidenziata

3.  Configurare e abilitare il nuovo Punto Vendita, inserendo, in
    particolare, **quelle che sono le sue esatte coordinate
    geografiche**

> **ATTENZIONE!** Per poter abilitare un nuovo Punto Vendita è
> necessario impostare le esatte coordinate geografiche (latitudine e
> longitudine) in corrispondenza delle quali dovrà essere posizionato,
> sulla mappa, il marker del punto vendita

4.  Associare il nuovo Punto Vendita ad un determinato metodo di
    trasporto, operazione quest'ultima effettuabile direttamente in fase
    di configurazione dello specifico metodo di trasporto.

**[ECOMMERCE HO.RE.CA.]{.underline}**

**Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.
ogni Punto Vendita dovrà essere codificato e gestito interamente
all'interno del Wizard di Passweb.**

In queste condizioni dunque per poter utilizzare un nuovo Punto Vendita
è necessario:

1.  Accedere alla maschera "**Lista dei Punti Vendita**" precedentemente
    evidenziata

2.  Cliccare sul pulsante **Aggiungi Punto Vendita**
    (![](./assets/media/image356.png) ) presente nella barra degli
    strumenti e impostare i parametri di configurazione necessari per
    poter salvare il nuovo Punto Vendita.

3.  Associare il nuovo Punto Vendita ad un determinato metodo di
    trasporto, operazione quest'ultima effettuabile direttamente in fase
    di configurazione dello specifico metodo di trasporto.

Considerando quanto appena detto i campi presenti all'interno della
maschera "Configurazione del Punto Vendita" potranno essere o meno campi
a sola lettura, dipendentemente dalla tipologia di sito considerato.

**ATTENZIONE!** Per i siti **Ecommerce collegati a Mexal** i campi
**Ragione Sociale, Nazione, Provincia, Località, CAP, Indirizzo, Codice
nell'anagrafica Indirizzi di Spedizione, Telefono, Fax, Email** presenti
nel dettaglio di un Punto Vendita, visualizzano i valori per essi
impostati all'interno dell'Anagrafica indirizzi di spedizione di Mexal e
come tali non sono modificabili dal Wizard di Passweb.

Per poter apportare delle modifiche a questi campi è quindi necessario
agire direttamente all'interno del gestionale.

![](./assets/media/image357.png)

In ogni caso sia che si operi dal gestionale sia che si operi dal Wizard
di Passweb, in fase di configurazione di un punto vendita sarà
necessario impostare un valore per i seguenti parametri:

- **Abilitato:** consente di Abilitare/Disabilitare il punto vendita in
  esame

- **Ragione Sociale:** consente di indicare il nome del Punto Vendita
  presso cui l'utente dovrà poi recarsi a ritirare la merce

- **Nazione, Provincia, Località, CAP, Indirizzo:** consentono di
  indicare tutti gli estremi dell'indirizzo del punto vendita presso cui
  l'utente dovrà poi recarsi per ritirare la merce

- **Coordinate Google Map (obbligatorio):** consente di impostare le
  esatte coordinate geografiche (latitudine e longitudine) in
  corrispondenza delle quali dovrà essere posizionato, sulla mappa, il
  marker del punto vendita.

> L'utilizzo di tali coordinate è obbligatorio (anche nel caso di siti
> Ecommerce collegati a Mexal) in quanto le sole informazioni relative a
> Nazione, Provincia, Località, Indirizzo e CAP potrebbero rallentare
> notevolmente il caricamento della mappa laddove, ovviamente, si sia
> deciso di visualizzare i punti vendita all'interno di un'apposita
> Google Map (per maggiori informazioni in merito si veda anche la
> sezione *"Ordini -- Configurazione Metodi di Trasporto -- Trasporti di
> tipo Passweb"* di questo manuale)
>
> Per poter individuare le esatte coordinate geografiche da inserire
> all'interno di questo campo è sufficiente:

- inserire l'indirizzo del punto vendita in esame direttamente
  all'interno di Google Maps (https://www.google.it/maps)

![](./assets/media/image358.png)

- cliccare con il tasto destro del mouse sul marker posizionato da
  google all'interno della mappa e selezionare l'opzione "**Che cosa c'è
  qui?**"

![](./assets/media/image359.png)

- le coordinate in esame potranno quindi essere prelevate direttamente
  dal piccolo fumetto visualizzato ora nella parte bassa della google
  map

![](./assets/media/image360.png)

- **Telefono:** consente di indicare il telefono del punto vendita che
  si sta codificando

- **Fax:** consente di indicare il numero di fax del punto vendita che
  si sta codificando

- **Magazzino:** consente di associare al punto vendita che si sta
  codificando uno specifico magazzino.

> **ATTENZIONE!** L'associazione di un magazzino al punto vendita verrà
> considerata anche in fase di checkout (ma non in carrello)
>
> Nel momento in cui dovessero infatti essere verificate le seguenti
> condizioni:

- Il magazzino associato al punto vendita è anche uno di quelli indicati
  per il calcolo della disponibilità articolo (sezione 'Disponibilità'
  della maschera "Configurazione Catalogo")

- Parametro "Gestione Acquisto" (sezione "Disponibilità" della pagina
  "Configurazione Catalogo" del Wizard) impostato su "Acquista solo se
  disponibile"

> quando poi sul front end del sito l'utente andrà a selezionare la
> modalità di spedizione di tipo "Ritiro in negozio", indicando come
> punto di ritiro il punto vendita con il magazzino associato, verrà
> effettuato, su questo stesso magazzino per gli articoli in ordine, un
> controllo della disponibilità.
>
> Se il controllo dovesse dare esito positivo, il punto vendita verrà
> correttamente selezionato e si potrà procedere alla conferma
> dell'ordine.
>
> Nel caso in cui invece il controllo dovesse dare esito negativo verrà
> visualizzato un apposito messaggio indicante le mancate disponibilità
> e il punto vendita non potrà essere selezionato (il testo del
> messaggio può essere modificato alla sezione "Testi/Messaggi del Sito"
> agendo sul componente "Aggiunta al Carrello" e modificando il testo
> "Massima disponibilità negozio")
>
> **In queste condizioni, inoltre, in fase di memorizzazione del
> documento sul gestionale verrà utilizzato, come Magazzino dell'ordine,
> non quello definito in "Configurazione Ordini" ma bensì quello
> associato in maniera specifica al Punto Vendita selezionato**

- **Email:** consente di indicare l'indirizzo mail del punto vendita che
  si sta codificando

- **Valorizza Indirizzo del Negozio nel Piede del Documento del
  Gestionale:** se impostato a **SI** nel momento in cui effettuando un
  ordine sul sito il cliente dovesse scegliere come metodo di spedizione
  il "Ritiro in Negozio" nel piede del relativo documento gestionale
  verrà inserito, come indirizzo di spedizione, l'indirizzo del negozio
  selezionato dal cliente in fase di acquisto.

> Nel momento in cui il parametro in esame dovesse invece essere
> impostato sul valore **NO** nel piede del relativo documento
> gestionale non verrà inserito nessun indirizzo.

- **Descrizione**: consente di impostare un testo con eventuali immagini
  da utilizzare come descrizione del punto vendita, descrizione questa
  che potrà poi essere visualizzata all'interno del fumetto che si
  aprirà cliccando sul marker che individua la posizione del punto
  vendita all'interno della mappa

![](./assets/media/image361.png)

**NOTA BENE**: per attivare la visualizzazione della mappa di Google
all'interno del Componente Checkout Ordine è necessario spuntare il
check sul parametro "Visualizza Google Map dei Punti Vendita".

- **Pagina Negozio per sito:** consente di impostare, selezionandola del
  relativo albero, la pagina di dettaglio del punto vendita, pagina
  questa cui sarà ricondotto l'utente, nel momento in cui dovesse
  cliccare sul corrispondente link presente, all' interno del componente
  "Store Locator", in corrispondenza del punto vendita in esame.

![](./assets/media/image362.png)

> Per maggiori informazioni relativamente alla gestione del componente
> "Store Locator" si veda il relativo capitolo di questo manuale
> ("*Varianti Sito Responsive -- Lista Componenti Comuni -- Componente
> Store Locator*")

**ATTENZIONE! Indipendentemente dalla tipologia di sito considerata una
volta configurato e salvato correttamente un Punto Vendita, per poterlo
poi utilizzare all'interno del sito sarà necessario, ovviamente,
associarlo ad un metodo di trasporto** appositamente configurato per
creare una spedizione a carico del cliente che ha acquistato la merce
con ritiro della stessa presso uno dei punti vendita abilitati.

Nel momento in cui il cliente dovesse selezionare proprio questo tipo di
spedizione avrà poi la possibilità di scegliere, tra tutti i punti
vendita ad esso associati, quello in cui desidera ritirare la merce,
informazione questa che verrà ovviamente inserita anche nel piede del
corrispondente documento gestionale.

Per maggiori informazioni relativamente alla configurazione dei metodi
di trasporto si veda anche la sezione "*Ordini -- Configurazione Metodi
di trasporto* " di questo manuale.

Gli ulteriori pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

- **Coordinate Punti Vendita**
  (![](./assets/media/image363.png) ) -- visualizzato indipendentemente dal fatto di
  aver selezionato o meno uno specifico punto vendita tra quelli
  presenti in elenco.

> Consente di effettuare la conversione automatica degli indirizzi
> associati a tutti i Punti Vendita gestiti, in coordinate geografiche
> (latitudine e longitudine) operazione questa di fondamentale
> importanza per diverse ragioni, come ad esempio nel momento in cui si
> dovesse decidere di associare determinati punti vendita ai metodi di
> spedizione merce (per maggiori informazioni in merito, si veda anche
> quanto indicato nel precedente capitolo di questo manuale)
>
> **ATTENZIONE!** La conversione di indirizzi in coordinate geografiche
> avviene effettuando apposite chiamate alle API di Google Map. Tale
> servizio richiede quindi la corretta impostazione della chiave
> "**Google Maps API**" all'interno della relativa sezione alla pagina
> "Sito -- Preferenze" del Wizard

- **Abilita Punto Vendita**
  (![](./assets/media/image364.png) ): consente di abilitare il punto vendita in esame
  rendendolo quindi visibile e selezionabile in fase di configurazione
  dei vari metodi di trasporto.

> **ATTENZIONE!** Prima di poter abilitare un Punto Vendita è necessario
> averlo configurato correttamente valorizzando tutti i suoi campi
> obbligatori

- **Disabilita Punto Vendita**
  (![](./assets/media/image365.png) ): consente di disabilitare il punto vendita in
  esame eliminandolo, contestualmente, anche da eventuali metodi di
  trasporto cui era stato precedentemente associato

- **Modifica Punto Vendita**
  (![](./assets/media/image366.png) ): consente di accedere alla maschera
  di configurazione del punto vendita attualmente selezionato.

- **Esporta**
  (![](./assets/media/image367.png) ) / **Importa**
  (![](./assets/media/image368.png) ): consente di Esportare / Importare
  in maniera massiva mediante un apposito file .csv i dati dei punti
  vendita attualmente presenti in elenco.

> **ATTENZIONE!** l'import mediante file csv consente di modificare in
> maniera massiva i dati dei punti vendita attualmente presenti in
> elenco ma non consente di creare nuovi punti vendita
>
> Per maggiori informazioni relativamente a questo tipo di operazioni si
> veda anche quanto indicato nel successivo capitolo di questo manuale

