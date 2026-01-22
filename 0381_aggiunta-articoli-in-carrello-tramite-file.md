# AGGIUNTA ARTICOLI IN CARRELLO TRAMITE FILE



Oltre alla normale operatività che prevede di inserire articoli in
carrello in maniera manuale mediante l'apposito componente "Aggiunta al
Carrello", Passweb offre anche la possibilità di automatizzare e
velocizzare questo processo mediante l'upload di un file appositamente
realizzato e contente l'elenco di tutti gli articoli, con relative
quantità, che dovranno essere effettivamente aggiunti.

Per poter realizzare una cosa di questo tipo è necessario:

- Inserire in una qualsiasi pagina del sito, tipicamente all'interno
  della pagina Carrello, il componente Form e configurarlo impostando il
  parametro **Tipo Valore** su **Carrello tramite file**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_aggiunta_articoli_carrello_res.bmp](./assets/media/image170.png){width="5.122916666666667in"
height="3.129166666666667in"}

> In queste condizioni verranno visualizzati due ulteriori campi
> "**Separatore File**" e "**Campi Codice**"
>
> Il primo (**Separatore File**) consentirà di indicare, selezionando
> una delle opzioni presenti all'interno del relativo menu a tendina, il
> carattere separatore dei vari campi che verrà poi utilizzato nella
> realizzazione del file contente l'elenco di articoli da aggiungere
> automaticamente in carrello.
>
> Il secondo (**Campi Codice**) consentirà invece di specificare quali
> informazioni potranno effettivamente essere presenti, nel tracciato
> del file di importazione in corrispondenza della colonna "Codice"

- Inserire all'interno del Form un componente di tipo "**Campo File**"
  in maniera tale da realizzare il modulo per l'upload del file contente
  l'elenco di articoli da aggiungere in carrello

- Realizzare il file esterno contenente l'elenco di articoli che
  dovranno essere aggiunti, seguendo determinate regole.

> Nello specifico:

- Il file dovrà avere necessariamente estensione .csv o .txt

- Il formato del file ed il carattere separatore dei vari campi dovrà
  essere coerente con quanto impostato, in configurazione del form per
  il parametro "**Separatore File**"

- Nei campi di intestazione del file dovrà essere necessariamente
  presente un campo denominato **Codice.**

> In corrispondenza di questo campo potrà poi essere inserito, per ogni
> singolo record e dipendentemente da quanto settato in corrispondenza
> del parametro "Campi Codice", il codice gestionale dell'articolo da
> aggiungere in carrello, il suo Codice Alternativo (solo per Ecommerce
> Mexal) o uno dei suoi Codici Alias.
>
> Supponendo, ad esempio, di aver attivato per il parametro "Campi
> Codice" le sole opzioni Codice Articolo e Codice Alternativo Articolo,
> nel tracciato record del file di importazione, in corrispondenza della
> colonna "Codice", potrà essere inserito indifferentemente il Codice
> gestionale oppure il Codice Alternativo dell'articolo da aggiungere in
> carrello (articolo questo che dovrà, ovviamente essere correttamente
> gestito all'interno del sito)

- Nei campi di intestazione potrà essere inserito, in maniera opzionale,
  un campo denominato **Quantita** in corrispondenza del quale andrà poi
  dichiarato, per ogni record, l'esatta quantità con cui il
  corrispondente articolo dovrà essere aggiunto in carrello.

> **ATTENZIONE!** Il campo Quantita deve essere inserito così come
> indicato (con il carattere "a" non accentato)
>
> Nel caso in cui il file di importazione non contenga il campo
> Quantita, così come nel caso in cui tale campo sia presente ma, per
> certi articoli, non sia valorizzato, questi stessi articoli verranno
> aggiunti in carrello con quantità unitaria

- Nei campi di intestazione potrà essere inserito, in maniera opzionale,
  un campo denominato **Sconto** in corrispondenza del quale andrà poi
  dichiarato, per ogni record, l'esatto sconto che dovrà essere
  applicato all' articolo automaticamente aggiunto in carrello.

> **ATTENZIONE!** **il campo Sconto verrà preso in considerazione solo
> ed esclusivamente nel caso in cui ad effettuare l'upload del file sia
> un Agente opportunamente abilitato, mediante la relativa funzionalità
> Mexal, alla modifica degli Sconti**
>
> Nel caso in cui il valore indicato per il campo Sconto in
> corrispondenza di un dato articolo non sia corretto, verrà
> visualizzato un apposito messaggio di errore personalizzabile
> all'interno della sezione "Testi / Messaggi del Sito" selezionando il
> componente Form ed intervenendo in corrispondenza della voce "Errore
> Sconto non valido".
>
> **Infine, nel caso in cui lo sconto impostato all'interno del file per
> un dato articolo dovesse superare lo sconto massimo consentito per
> quello stesso articolo, questo verrà comunque inserito in carrello ma
> con lo sconto massimo gestibile.**

- Nei campi di intestazione potrà essere inserito, in maniera opzionale,
  un campo denominato **Prezzo** in corrispondenza del quale andrà poi
  dichiarato, per ogni record, il valore esatto del prezzo che dovrà
  essere applicato all' articolo automaticamente aggiunto in carrello.

> **ATTENZIONE!** **il campo Prezzo verrà preso in considerazione solo
> ed esclusivamente nel caso in cui ad effettuare l'upload del file sia
> un Agente opportunamente abilitato, mediante la relativa funzionalità
> Mexal, alla modifica dei Prezzi**
>
> Nel caso in cui il valore indicato per il campo Prezzo in
> corrispondenza di un dato articolo non sia corretto, verrà
> visualizzato un apposito messaggio di errore personalizzabile
> all'interno della sezione "Testi / Messaggi del Sito" selezionando il
> componente Form ed intervenendo in corrispondenza della voce "Errore
> Prezzo non valido".
>
> **Infine, nel caso in cui il prezzo impostato all'interno del file per
> un dato articolo dovesse essere inferiore al prezzo minimo impostato
> per quello stesso articolo, questo verrà comunque inserito in carrello
> ma con il prezzo minimo gestibile.**
>
> Anche in questo caso, come per la variazione manuale del prezzo, non
> sarà possibile modificare il prezzo di Articoli Campionario.

- Nel caso in cui si debbano aggiungere in carrello articoli a Taglie,
  nei campi di intestazione del file dovrà essere necessariamente
  presente un campo denominato **Taglia** in corrispondenza del quale
  andrà poi dichiarato, per ogni record, la descrizione della taglia con
  cui il relativo articolo dovrà essere aggiunto in carrello. **Nel caso
  in cui tale campo non sia presente eventuali articoli a taglie
  indicati nel file di importazione non verranno mai aggiunti in
  carrello**

> **ATTENZIONE!** **la descrizione della taglia indicata all'interno del
> campo in oggetto deve coincidere esattamente con quella impostata
> all'interno di Passweb per la lingua di visualizzazione del sito (che
> può essere diversa da quella impostata, per la stessa taglia,
> all'interno del gestionale)**
>
> Ciò significa dunque che, nel caso in cui l'import del file avvenga
> dal sito visualizzato ad esempio in lingua inglese, all'interno del
> file di importazione degli articoli la descrizione delle varie taglie
> dovrà essere esattamente quella impostata in Passweb per la lingua
> inglese.
>
> Infine nel caso in cui lo stesso articolo debba essere inserito in
> carrello in taglie diverse sarà necessario indicare nel file di
> importazione un record per ogni singola taglia.

- A differenza di quanto avviene con la procedura di aggiunta manuale,
  nel caso in cui all'interno del file di importazione siano stati
  indicati degli articoli figli di struttura, è necessario che tali
  articoli siano già stati esportati e siano quindi già presenti
  all'interno del sito. In caso contrario infatti la procedura di
  aggiunta automatica in carrello non troverà alcuna corrispondenza e
  gli articoli in esame non verranno quindi inseriti.

> **ATTENZIONE!** Gli articoli padri di struttura, ovviamente, non
> verranno mai inseriti in carrello ne mediante aggiunta manuale ne
> tanto meno mediante la procedura di aggiunta automatica da file

Una volta effettuato quanto indicato, in fase di ordine l'utente
potrebbe trovarsi, all'interno della pagina Carrello, il controllo da
utilizzare per poter effettuare l'upload del file contente l'elenco di
articoli da aggiungere.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_aggiunta_articoli_carrello3.bmp](./assets/media/image171.png){width="5.564583333333333in"
height="3.435416666666667in"}

Selezionando il file e cliccando sul pulsante di conferma, Passweb
aggiungerà automaticamente in carrello tutti gli articoli indicati
all'interno del file che hanno correttamente superato tutti i controlli
di validazione del caso.

Ciò significa dunque che nel momento in cui, ad esempio, all'interno del
file sia indicato un codice articolo attualmente non gestito sul sito,
al termine della procedura di importazione verrà visualizzato un
apposito messaggio di errore e, ovviamente, l'articolo in questione non
verrà aggiunto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_aggiunta_articoli_carrello4.bmp](./assets/media/image172.png){width="5.564583333333333in"
height="3.435416666666667in"}

Messaggi analoghi verranno visualizzati:

- in mancanza del campo Taglia

- nel caso in cui la descrizione indicata per una taglia non corrisponda
  con quella dichiarata in Passweb

- nel caso in cui l'estensione del file importato non sia una di quelle
  ammesse

- nel caso in cui la quantità indicata non sia numerica o sia negativa
  ecc...

**Va inoltre precisato che, a parte il codice articolo e l'eventuale
quantità indicata all'interno del file di importazione, una volta
aggiunti gli articoli in carrello tutto funzionerà poi come se questi
stessi articoli fossero stati aggiunti in maniera manuale**.

Ciò significa quindi che verranno considerati anche eventuali limiti
sulle quantità massime o minime acquistabili, che in relazione a ciò il
funzionamento del carrello sarà sempre coerente con quanto impostato per
il parametro "Aggiunta in Carrello" presente nella sezione "Gestione
Massimo e Minimo Fatturabile" della maschera "Configurazione Catalogo
Mexal / Ho.Re.Ca." del Wizard e che, soprattutto, verranno
automaticamente applicate sia le condizioni commerciali relative
all'utente che sta effettuando l'ordine sia eventuali promozioni
definite per gli articoli aggiunti in carrello.

