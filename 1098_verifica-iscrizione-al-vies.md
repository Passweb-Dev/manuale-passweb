# VERIFICA ISCRIZIONE AL VIES



Il **VIES** (VAT Information Exchange System) è un sistema elettronico
sviluppato dalla Commissione Europea che consente di verificare la
validità dei numeri di partita IVA degli operatori economici registrati
nell'Unione Europea.

Il VIES è essenziale per facilitare il commercio intra-UE, consentendo
alle aziende di confermare se i loro partner commerciali sono soggetti
IVA registrati in un altro Stato membro.

Questo sistema è particolarmente utile per garantire che le operazioni
siano conformi alle regole fiscali e per beneficiare dell'esenzione IVA
nelle transazioni intra-UE. Una volta verificato infatti che la partita
IVA di un' azienda che acquista all'interno del nostro sito ecommerce
risulti correttamente iscritta al VIES, sarà poi possibile emettere
verso essa fatture senza IVA utilizzando per questo un apposito codice
esenzione che identifica appunto questo tipo di cessioni
intracomunitarie.

**ATTENZIONE!** Per maggiori informazioni in merito si consiglia di fare
sempre riferimento alle specifiche normative fiscali e al proprio
commercialista

Considerando che, al momento, non è possibile verificare direttamente
all'interno del gestionale se un'azienda (potenziale utente del sito
ecommerce) risulti essere o meno iscritta al VIES e che quindi il
gestionale non riesce a trasferire al sito questo tipo di informazione,
per determinare se un'azienda abilitata ad effettuare acquisti sul sito
sia o meno iscritta al VIES e se, quindi, si possa applicare per essa
una determinata esenzione IVA Passweb si comporterà come di seguito
indicato:

- Dopo che l'azienda in questione avrà effettuato l'autenticazione al
  sito, Passweb utilizzerà la Partita IVA ad essa associata per
  verificare, innanzitutto, che questa sia effettivamente una Partita
  IVA Europea.

- Nel caso in cui la Partita IVA associata all'azienda non dovesse
  essere una Partita IVA Europea l'azienda verrà ovviamente marcata come
  non iscritta al VIES

- Nel caso in cui la Partita IVA associata all'azienda dovesse invece
  essere una Partita IVA Europea, Passweb la utilizzerà per effettuare
  determinate chiamate ai servizi esposti dal VIES e per verificare
  quindi se quella stessa Partita IVA risulti o meno essere iscritta al
  sistema

- Considerando che il VIES mette a disposizione due diversi servizi, uno
  di tipo REST e l'altro di tipo SOAP, per verificare se una determinata
  Partita IVA risulti o meno iscritta al sistema Passweb effettuerà una
  prima richiesta, relativa alla Partita IVA in esame, verso il servizio
  di tipo REST. Se poi questa richiesta dovesse, per un qualsiasi
  motivo, non andare a buon fine ritornando un errore, Passweb
  effettuerà automaticamente la stessa richiesta verso l'altro tipo di
  servizio (quello SOAP)

- Nel momento in cui entrambe le richieste dovessero ritornare degli
  errori (ad esempio perché i relativi endpoint risultano essere
  momentaneamente non raggiungibili o fuori servizio) Passweb marcherà
  momentaneamente l'azienda come non iscritta al VIES, la gestirà come
  tale (in relazione alle Tasse di tipo IVA codificate e attive
  all'interno del sito) e, fintantoché l'azienda stessa continuerà a
  navigare sul sito continuerà anche, ad intervalli regolari, ad
  effettuare richieste ai servizi VIES per ottenere una risposta,
  positiva o negativa che sia, ma comunque una risposta valida

- Ottenuta una risposta valida Passweb si comporterà in maniera diversa
  a seconda del fatto che questa sia positiva oppure negativa e quindi a
  seconda del fatto che l'azienda risulti essere iscritta o non iscritta
  al VIES.

- In caso di risposta negativa Passweb marcherà l'azienda come non
  iscritta al VIES con tutto ciò che ne consegue in fase di applicazione
  delle relative Tasse di tipo IVA. In queste condizioni inoltre ogni
  volta che l'azienda dovesse autenticarsi sul sito Passweb continuerà
  ad effettuare chiamate al VIES per verificare se nel frattempo la sua
  situazione dovesse essere cambiata.

- In caso di risposta positiva invece Passweb marcherà l'azienda come
  iscritta al VIES con tutto ciò che ne consegue in fase di applicazione
  delle relative Tasse di tipo IVA. Inoltre, da questo momento in
  avanti, non effettuerà più nessun tipo di chiamata verso il VIES per
  verificare lo stato di iscrizione al sistema, stato questo che quindi,
  in Passweb, da questo momento in poi non potrà più essere modificato.

Per verificare lo stato di iscrizione al VIES degli utenti di tipo
Azienda attualmente gestiti all'interno del sito e sufficiente accedere
alla loro anagrafica Passweb.

All'interno della maschera "Dati Utente" del Wizard troveremo infatti i
due campi "**Iscrizione VIES**" e "**Dettaglio Risposta VIES**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\stato_iscrizione_vies.bmp](./assets/media/image457.png){width="5.83125in"
height="4.214583333333334in"}

che consentono rispettivamente:

- **Iscrizione VIES**: consente di visualizzare quello che per Passweb
  risulta essere lo stato di iscrizione al VIES per l'azienda in esame.

- **Dettaglio Risposta VIES**: consente di visualizzare quella che è
  stata l'ultima risposta ottenuta da Passweb a seguito delle richieste
  effettuate ai servizi esposti dal VIES per determinare se l'azienda in
  esame risulta essere o meno iscritta al sistema. Tale campo potrebbe
  risultare particolarmente utile nel momento le richieste effettuate da
  Passweb dovessero ritornare degli errori per visualizzare che tipo di
  errore si è verificato e perché quindi la richiesta effettuata non ha
  ottenuto una risposta valida.

**ATTENZIONE!** considerando che la verifica dello stato di iscrizione
al VIES è un processo gestito da Passweb in maniera completamente
automatica i due campi "Iscrizione VIES" e "Dettaglio Risposta VIES"
evidenziati in figura saranno campi in sola lettura.

Ovviamente la verifica di iscrizione al VIES per una determinata azienda
di per sé non è sufficiente per fare in modo che, quando quella stessa
azienda andrà poi ad acquistare sul sito gli venga applicata la corretta
esenzione e/o la corretta aliquota IVA.

Per ottenere questo risultato sono necessarie infatti altre due cose di
fondamentale importanza ossia:

- Aver creato e attivato, in fase di configurazione del sito, due Tasse
  di tipo IVA configurate in maniera corretta per poter gestire da una
  parte le Cessioni intracomunitarie e dall'altra parte le Esportazioni
  verso paese extra UE

<!-- -->

- L'indirizzo di spedizione merce selezionato dall'azienda in fase di
  ordine sul sito dovrà rientrare effettivamente in una delle due zone
  geografiche assegnate alle Tasse di cui al punto precedente

Per maggiori informazioni in merito a come configurare delle Tasse di
tipo IVA tali da poter gestire in maniera corretta le Cessioni
intracomunitarie e le Esportazioni verso paese extra UE si veda quanto
indicato nel successivo capitolo di questo manuale.

