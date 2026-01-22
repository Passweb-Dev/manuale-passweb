# TRACCIAMENTO LATO SERVER



Oltre al tracciamento "tradizionale", che come ormai chiaro viene
effettuato lato client con l'utilizzo dei cookie, Matomo mette a
disposizione degli utenti anche la possibilità di implementare un
tracciamento lato server in maniera sostanzialmente analoga a quello che
avviene con il Measurement Protocol di Google Analytics.

L'integrazione Passweb -- Matomo offre la possibilità di sfruttare anche
questo tipo di tracciamento in relazione però alla sola acquisizione di
nuovi ordini

**ATTENZIONE! Al momento l'unico evento che può essere tracciato lato
server nell'integrazione Passweb -- Matomo è l'acquisizione di un nuovo
ordine**

Per attivare questo tipo di tracciamento è necessario accedere alla
pagina "**Sito -- Preferenze -- Tracciamento Dati**" del Wizard del
proprio sito Passweb e selezionare il parametro "**Abilita Tracciamento
Server**" presente all'interno della sezione "**Matomo -- Server**"

![](./assets/media/image31.png)

Selezionando questo parametro verranno poi visualizzati altri campi che
dovranno essere appositamente compilati per poter attivare in maniera
corretta il tracciamento lato server degli ordini effettuati all'interno
del sito.

Nello specifico dunque il parametro:

- **Dominio Matomo Server -- obbligatorio:** all'interno di questo campo
  è necessario indicare il dominio (privo del protocollo utilizzato e
  quindi senza http o https) assegnato alla propria installazione Matomo
  (in questo senso è consigliabile utilizzare un sottodominio del
  dominio principale in uso al sito Passweb)

- **Id Sito -- obbligatorio:** all'interno di questo campo è necessario
  indicare l'Id assegnato da Matomo al sito che si intende monitorare.
  Tale identificativo viene assegnato direttamente in fase di
  configurazione del sito stesso su Matomo e può essere visualizzato
  portandosi all'interno della pagina "**Siti Web -- Amministrazione**"
  (parametro **ID** evidenziato in figura)

![](./assets/media/image32.png)

> **ATTENZIONE!** "Id Sito" e "Dominio Matomo Server" sono parametri
> obbligatori. Nel momento in cui uno di essi dovesse essere impostato
> in maniera non corretta non sarà possibile attivare il tracciamento
> lato server

- **Utilizza User Id:** consente di inviare a Matomo, anche in relazione
  al tracciamento lato server, lo User Id aumentando quindi
  l'accuratezza dei dati tracciati. Attivando questo parametro infatti
  anche le transazioni tracciate lato server potranno essere legate ad
  uno specifico utente e verranno quindi inserite, su Matomo,
  all'interno della scheda anagrafica dell'utente stesso. In questo
  senso, ovviamente, è richiesto il tracciamento dello User Id anche
  lato Client

> **ATTENZIONE!** Si ricorda che per il GDPR lo User Id viene trattato a
> tutti gli effetti come un'informazione di identificazione personale
> (PII) e questo anche nel momento in cui dovesse essere utilizzata,
> come User Id, una generica stringa alfanumerica e/o si dovesse
> ricorrere alle funzioni di anonimizzazione messe a disposizione da
> Matomo.
>
> In conseguenza di ciò nel momento in cui si dovesse decidere di
> attivare e gestire anche questo tipo di tracciamento sarà necessario,
> da una parte, fornire nelle Norme sulla gestione della privacy del
> proprio sito un'informativa adeguata circa l'utilizzo degli
> identificatori utilizzati e, dall'altra parte, verificare di aver
> gestito in maniera corretta la richiesta di consenso preventivo come
> effettivamente richiesto dal GDPR

Una volta impostati correttamente i parametri sopra indicati verrà
quindi abilitato, **in merito alla sola acquisizione di nuovi ordini,**
il tracciamento di Matomo anche lato server. Ciò significa che sarà
direttamente il server su cui risiede il sito Passweb ad inviare a
Matomo i dati relativi all'acquisizione del nuovo ordine.

In queste condizioni, dunque, nel caso in cui l'utente, una volta chiuso
un ordine, non dovesse approdare sulla relativa pagina di conferma (ad
esempio perché ha scelto di effettuare un pagamento online e, una volta
completata la transazione, decide poi di non ritornare sul sito del
venditore) Passweb potrebbe comunque inviare a Matomo tutti i dati
necessari al tracciamento dell'ordine stesso, operando direttamente a
livello server.

**Affinchè ciò possa avvenire in maniera corretta è però indispensabile
che il pagamento utilizzato implementi la modalità Server to Server.**
Sarà infatti la risposta ricevuta dal gateway di pagamento a determinare
o meno l'invio a Matomo dei dati relativi all'ordine acquisito.

Nello specifico, una volta ricevuta risposta positiva dal gateway di
pagamento, Passweb avrà la certezza che l'ordine in questione è stato
correttamente pagato e quindi, oltre ad inserire il documento
all'interno del gestionale, provvederà anche ad inviare a Matomo tutti i
dati necessari al tracciamento dell'ordine

Se, al contrario, dal gateway di pagamento non dovesse arrivare nessuna
risposta o dovesse comunque arrivare una risposta negativa, Passweb non
avrà la certezza che l'ordine sia stato correttamente pagato; lascerà
quindi il documento in stato di "Pagamento non confermato" e non invierà
a Matomo nessun dato.

**ATTENZIONE! Ovviamente la corretta acquisizione di un ordine verrà
tracciata una sola volta**

Ciò significa dunque che nel momento in cui un utente dovesse
selezionare un pagamento online con modalità Server to Server chiudendo
il giro correttamente tornando quindi, una volta concluso il pagamento,
sul sito del venditore, si verificherebbero entrambe le condizioni
necessarie per inviare a Matomo i dati dell'ordine.

Da una parte verrebbe infatti eseguito l'evento javascript necessario
per inviare i dati dell'ordine a livello client; allo stesso modo
dall'altra parte una volta ricevuta risposta positiva dal gateway di
pagamento si verificherebbero le condizioni necessarie per inviare a
Matomo i dati dello stesso ordine anche a livello server.

In queste condizioni dunque il primo dei due eventi a verificarsi
(tipicamente quello javascript) determinerà l'invio dei relativi dati a
Matomo mentre il secondo verrà scartato evitando così di tracciare lo
stesso ordine due volte.

**ATTENZIONE!** Nel momento in cui il tracciamento lato server non
dovesse essere abilitato l'acquisizione di un nuovo ordine potrà essere
correttamente tracciata solo nel momento in cui l'utente dovesse
effettivamente approdare nella pagina di "Conferma Ordine", pagina
questa che, come noto, avrà un indirizzo del tipo

www.url_sito.it/store/cart/checkout/success?id=xxxx

Nel momento in cui l'utente non dovesse, per una qualsiasi ragione,
approdare su questa pagina (ad esempio perché ha scelto di effettuare un
pagamento online e, una volta completata la transazione, decide poi di
non ritornare sul sito del venditore) l'evento javascript necessario per
comunicare a Matomo i dati dell'ordine non potrà ovviamente essere
eseguito e, conseguentemente, non sarà possibile tracciare il relativo
acquisto.

