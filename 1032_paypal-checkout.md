# PAYPAL CHECKOUT



PayPal Checkout è una nuova soluzione di pagamento di PayPal che
utilizza il collegamento con le API REST messe a disposizione dalla
piattaforma e implementa nativamente anche il servizio Server2Server
mediante l'utilizzo di appositi webhooks.

**ATTENZIONE!** **Per poter attivare questa modalità di pagamento sarà
necessario disporre di un proprio account sull'ambiente developer di
PayPal ( <https://developer.paypal.com> ), creare un APP da cui poter
prelevare i parametri di configurazione richiesti dall'integrazione e
attivare appositi webhooks**. Per maggiori informazioni in merito a
questi passaggi si rimanda a quanto indicato nel successivo capitolo di
questo manuale ("*PayPal Checkout -- Creazione APP*")

Una volta creato tutto quanto richiesto in ambiente developer di PayPal,
sarà poi necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione PAYPAL
    CHECKOUT

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **"Lista dei Metodi di Pagamento"**
    precedentemente esaminata.

3.  Attivare questa nuova modalità di pagamento secondo quanto descritto
    nel capitolo *"Configurazione Modalità di Pagamento"* di questo
    manuale.

4.  Impostare in maniera corretta i parametri specifici per questa
    particolare modalità di pagamento.

In particolare per poter eseguire quest'ultimo passaggio sarà necessario
selezionare il pagamento in oggetto (PayPal API) all'interno della
maschera **"Lista dei Metodi di Pagamento"** e cliccare sul pulsante
"**Modifica Pagamento**", presente nella barra degli strumenti.

Verrà quindi visualizzata la maschera di configurazione e
personalizzazione del pagamento, all'interno della quale sarà necessario
impostare, oltre ai parametri classici di configurazione del pagamento,
anche quelli specifici del gateway attualmente considerato e presenti
all'interno della sezione " **Parametri Gateway**

![](./assets/media/image165.png)

Nello specifico all'interno di questa sezione il campo:

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Client ID / Secret ID:** chiavi di configurazione necessarie per
  poter integrare correttamente il proprio sito con il gateway di
  pagamento di PayPal.

> **ATTENZIONE!** I valori da inserire all'interno dei campi Client ID e
> Secret ID dovranno essere prelevati dall'APP appositamente creata
> nell'ambiente developer di PayPal. Per maggiori informazioni in merito
> si veda anche il successivo capitolo di questo manuale

- **Contabilizzazione:** consente di specificare se la contabilizzazione
  delle transazioni effettuate dovrà avvenire in maniera immediata
  (**Vendita**) o differita (**Autorizzazione**). Una contabilizzazione
  immediata, ad esempio, permetterà all'esercente di rendere
  automaticamente contabili tutte le transazione autorizzate, senza un
  suo specifico intervento dall' applicazione di Back Office. Una
  contabilizzazione differita richiederà invece che le operazioni
  autorizzate siano esplicitamente rese contabili dall'esercente
  attraverso la relativa applicazione di Back Office.

- **Banner:** consente di inserire il codice HTML necessario per
  visualizzare, sul front end del sito, il banner relativo all'opzione
  di pagamento rateale offerta da PayPal, banner questo che potrà essere
  visualizzato direttamente nella singola pagina prodotto (mediante
  l'utilizzo del Componente Ecommerce "Simulatore del Pagamento")

![](./assets/media/image166.png)

> oppure in fase di checkout in corrispondenza della relativa modalità
> di pagamento

![](./assets/media/image167.png)

> **ATTENZIONE! la rateizzazione del pagamento è gestita interamente da
> PayPal**
>
> Per ottenere il codice in esame è necessario agire direttamente sul
> sito di PayPal partendo, ad esempio, dal seguente link
> <https://www.paypal.com/ppcredit/messaging/customize>

![](./assets/media/image168.png)

> Una volta impostati i parametri di configurazione desiderati
> (posizionamento, logo, colori ...) sarà sufficiente cliccare sul
> pulsante "**Ottieni il codice**" per essere ricondotti alla pagina da
> cui poter poi prelevare il codice che dovrà essere effettivamente
> copiato e incollato nei parametri di configurazione del pagamento
> Passweb.

![](./assets/media/image169.png)

> In particolare, come evidenziato nella figura sopra riportata,
> all'interno di questa pagina verranno forniti due diversi snippet di
> codice:

- Il codice indicato in corrispondenza del **Passaggio 1** è relativo
  all'inclusione della libreria javascript utilizzata da PayPal per la
  gestione del banner. Tale codice è gestito in automatico da Passweb e
  **NON dovrà** quindi essere inserito da nessuna parte.

- Il codice indicato in corrispondenza del **Passaggio 2 è invece quello
  relativo al banner informativo e sarà dunque questo a dover essere
  inserito in corrispondenza del relativo parametro** presente nella
  maschera di configurazione del pagamento Passweb.

> In questa fase, inoltre, è di fondamentale importanza sostituire la
> stringa **ENTER_VALUE_HERE,** presente nel codice generato da PayPal,
> con il segnaposto Passweb **{0}**
>
> Supponendo dunque che lo snippet generato da PayPal sia il seguente:
>
> \<div data-pp-message data-pp-style-layout=\"text\"
> data-pp-style-logo-type=\"inline\" data-pp-style-text-color=\"black\"
> data-pp-amount=\"**ENTER_VALUE_HERE**\"\>\</div\>
>
> il codice da inserire in Passweb dovrà essere esattamente quello di
> seguito indicato
>
> \<div data-pp-message data-pp-style-layout=\"text\"
> data-pp-style-logo-type=\"inline\" data-pp-style-text-color=\"black\"
> data-pp-amount=\"**{0}**\"\>\</div\>
>
> **ATTENZIONE!** Nel momento in cui la stringa ENTRE_VALUE_HERE non
> dovesse essere sostituita dal segnaposto Passweb {0} il banner
> visualizzato sul sito non mostrerà l'importo corretto delle diverse
> rate

- **Sovrascrivi indirizzo**: consente, se selezionato, di sovrascrivere
  (limitatamente alla transazione in esame) l'indirizzo eventualmente
  presente su PayPal con l'indirizzo di spedizione indicato dall'utente
  in fase di ordine

Una volta impostati correttamente i parametri di configurazione e
verificato anche di aver attivato, sempre in ambiente developer di
PayPal, i webhooks richiesti, se l'utente dovesse, alla conferma
dell'ordine, selezionare la modalità di pagamento in esame, l'ordine
sarà memorizzato nel database di Passweb, e l'utente verrà reindirizzato
sul sito del gateway di pagamento dove potrà scegliere se pagare con
carta di credito (pulsante "**Paga con una carta**") oppure utilizzando
il proprio account PayPal (pulsante "**Accedi**" dopo aver inserito le
credenziali del proprio account)

![](./assets/media/image160.png)

**A questo punto però l'ordine non è ancora stato preso in carico da
PayPal e, conseguentemente, non è ancora avvenuto alcun pagamento**.
L'utente potrà ancora decidere, quindi, di annullare tutto (pulsante
"Annulla" nella parte bassa della pagina) oppure di portare a termine
l'acquisto e completare la transazione.

Nel primo caso, annullamento della transazione, l'utente verrà
reindirizzato al sito ecommerce dove si troverà l'ordine ancora da
confermare. Volendo potrà dunque decidere di ripartire dalla situazione
attuale, modificando se necessario l'ordine in essere con l'aggiunta o
l'eliminazione di determinati articoli, selezionando altre tipologie di
trasporto e /o altri pagamenti ecc... per poi passare nuovamente a
concludere l'ordine.

In queste condizioni dunque non essendo concluso, l'ordine non verrà
ovviamente memorizzato nel database di Passweb né tanto meno verrà
inserito in Mexal

Nel secondo caso, una volta scelta la modalità di pagamento (Carta o
Account PayPal ) verrà presentata all'utente una pagina web con il
riassunto dei dati relativi alla transazione in essere.

![](./assets/media/image161.png)

Cliccando sul pulsante "**Paga Adesso**" verrà completata la relativa
transazione e l'utente verrà automaticamente ricondotto al sito
Ecommerce. L'ordine verrà considerato valido ed inserito quindi
all'interno del gestionale

**NOTA BENE**: eventuali notifiche di avvenuta transazione, così come
gli accrediti e addebiti sui relativi c/c sono gestiti totalmente dal
gateway di pagamento.

**NOTA BENE**: verranno inseriti all'interno del gestionale unicamente
gli ordini in relazione ai quali è stata ricevuta, dal gateway di
pagamento, una risposta positiva.

**ATTENZIONE!** **PayPal Checkout supporta la modalità Server to
Server**. In tale modalità l'applicazione di PayPal grazie ai webhooks
appositamente attivati, invierà una notifica al sito per gestire l'esito
della transazione anche nel caso in cui l'acquirente non dovesse fare
ritorno sul sito dell'esercente (ad esempio perché a transazione
conclusa chiude semplicemente il browser).

In ogni caso nel momento in cui siano stati effettuati ordini a seguito
dei quali la piattaforma di finanziamento non ha restituito alcuna
risposta tali ordini resteranno unicamente all'interno del database di
Passweb nello stato di **"Pagamento Non Confermato"**.

Per maggiori informazioni relativamente a come poter gestire eventuali
ordini in stato di **"Pagamento Non Confermato"** si veda anche quanto
indicato all'interno del capitolo "*Ordini -- Ordini -- Stati
dell'Ordine*" di questo manuale.

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di utilizzare la specifica
manualistica.

**NOTA BENE**: per eventuali malfunzionamenti o problemi relativi ad
addebiti o accrediti sui c/c o alle applicazioni di Back Office di
proprietà del Gateway di paramento occorre rivolgersi alla relativa
assistenza.

