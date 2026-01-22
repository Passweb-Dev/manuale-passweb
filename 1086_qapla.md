# QAPLA'



La sezione "**Qaplà**", visualizzabile solo nel momento in cui sia stata
attivata in maniera corretta l'integrazione tra Passweb e la relativa
piattaforma terza, consente di impostare determinate opzioni di gestione
della spedizione (es. Consegna al piano, Consegna al sabato ecc...) che
verranno poi passate a Qaplà nel momento in cui l'utente dovesse
selezionare in fase di checkout la spesa accessoria in esame.

![](./assets/media/image425.png)

**ATTENZIONE!** la sezione Qaplà è visibile solo nel momento in cui
siano state inserite le relative chiavi di configurazione in
corrispondenza dei campi "**Qaplà API Key Privata**" e "**Qaplà API Key
Pubblica**" presenti nella sezione "**Logistica -- Qaplà**" alla pagina
"**Sito -- Preferenze**" del Wizard (tab "**Integrazioni**")

I parametri presenti all'interno di questa sezione sono di due tipi
diversi:

- Le "**Opzioni di spedizione**" sono legate allo specifico corriere e,
  attualmente, sono disponibili solo per i corrieri Bartolini (BRT) e
  GLS.

> **Lato** **Qaplà l'effettiva gestione di queste informazioni dipende
> quindi dal corriere che verrà poi utilizzato per gestire la
> corrispondente spedizione**.
>
> In sostanza dunque, nel momento in cui il cliente dovesse selezionare,
> in fase di checkout, una spesa accessoria configurata per inviare a
> Qaplà determinate opzioni di spedizione (es. la consegna al piano),
> Passweb invierà alla piattaforma terza, assieme ai dati dell'ordine,
> anche queste informazioni aggiuntive su come gestire la spedizione.
> Lato Qaplà tali informazioni diventeranno però visibili solo nel
> momento in cui l'utente dovesse decidere di gestire la spedizione con
> il corriere corretto.
>
> Supponendo dunque di configurare una spesa accessoria con l'opzione
> "Servizio al Sabato" questa informazione sarà effettivamente visibile
> su Qaplà solo nel momento in cui la relativa spedizione dovesse poi
> essere gestita con GLS.

![](./assets/media/image28.png)

> **Un'altra cosa di fondamentale importanza da tenere in considerazione
> è che le opzioni di spedizione sono definite in fase di configurazione
> della spesa accessoria e non possono quindi essere selezionate
> direttamente dall'utente sul front end del sito.**
>
> Nel momento in cui l'esigenza dovesse dunque essere quella di offrire
> all'utente, ad esempio, la possibilità di selezionare tra la "Consegna
> su appuntamento" o la "Consegna al piano" di Bartolini sarà necessario
> codificare due diverse spese accessorie, con descrizioni differenti,
> magari anche con due costi differenti e comunque, ciascuna, con la
> relativa opzione di spedizione Qaplà selezionata.
>
> Considerando poi che le spese accessorie possono essere tutte
> impostate come selezionabili dall'utente, operando in questo modo il
> cliente stesso in fase di checkout potrà decidere di selezionare la
> sola opzione di "Consegna su appuntamento", la sola opzione di
> "Consegna al sabato" oppure entrambe le opzioni indicate.

- **Tipologia di assicurazione:** consente di definire la metodologia di
  calcolo dell'importo da assicurare che dovrà poi essere passato a
  Qaplà nel momento in cui l'utente dovesse selezionare, in fase di
  checkout, il metodo di trasporto in esame.

> E' possibile selezionare una delle seguenti opzioni:

- **Disabilitato:** selezionando questa opzione non verrà trasmesso a
  Qaplà nessun importo da assicurare

- **Solo Merce**: in queste condizioni l'importo da assicurare passato a
  Qaplà coinciderà con il **Totale Merce Ivato**

- **Merce + Trasporto**: in queste condizioni l'importo da assicurare
  passato a Qaplà coinciderà con il Totale Merce Ivato + eventuali spese
  di trasporto (anch'esse ivate)

- **Totale ordine**: in queste condizioni l'importo da assicurare
  passato a Qaplà coinciderà con il Totale Ordine

> **ATTENZIONE!** lato Qaplà il valore dell'importo da assicurare verrà
> visualizzato nel dettaglio del documento a patto che la relativa
> spedizione sia gestita mediante uno specifico corriere (es. BRT, GLS
> ...)

![](./assets/media/image30.png)

- Le "**Custom Label**" sono invece campi che possono esseri utilizzati
  per passare a Qaplà delle informazioni testuali personalizzate e che,
  a differenza delle opzioni di spedizione, non sono legate su Qaplà, ad
  uno specifico corriere.

> Anche le etichette personalizzate vanno comunque definite in fase di
> configurazione della specifica spesa accessoria e non potranno quindi
> essere inserite direttamente dagli utenti sul front end del sito.
>
> Come detto però su Qaplà questi dati sono indipendenti dal corriere
> effettivamente utilizzato per gestire la spedizione e potranno quindi
> essere sempre visualizzati all'interno dei campi "Custom 1 / 2 / 3"
> aprendo il dettaglio dell'ordine inviato da Passweb

![](./assets/media/image29.png)

Un' ultima considerazione di fondamentale importanza da fare è che, lato
Passweb, le "Opzioni di spedizione per Qaplà" possono essere associate,
a seconda delle esigenze, a:

- Metodi di Trasporto

- Spese Accessorie

- Pagamenti

Nel momento in cui si dovesse dunque decidere, per una qualsiasi
ragione, di configurare queste opzioni di spedizione contemporaneamente
per due o più dei suddetti elementi, sarà necessario prestare
particolare attenzione, in fase di configurazione, a non creare delle
possibili situazioni di conflitto come potrebbe essere ad esempio, un
metodo di trasporto con associata l'opzioni di consegna al piano per
Bartolini e un pagamento con associata invece, sempre per Bartolini,
l'opzione di consegna al sabato.

In queste condizioni infatti verranno passate a Qaplà entrambe le
opzioni di spedizione solo nel momento in cui l'utente dovesse
effettivamente selezionare quello specifico metodo di trasporto e anche
quello specifico pagamento.

Allo stesso modo, in caso di conflitti, verrà fatto un merge delle
informazioni da passare a Qaplà, anche per quel che riguarda eventuali
valori settati per le Custom Label.

Supponendo dunque di aver impostato per un determinato metodo di
trasporto la "Custom Label 1" di Qaplà con la stringa "Trasporto X" e la
"Custom Label 2" di un pagamento con la stringa "Pagamento Y", nel
momento in cui l'utente dovesse selezionare in fase di checkout quello
specifico metodo di trasporto e quello specifico pagamento verrà passato
a Qaplà sia il valore della "Custom Label 1" (determinato dalla
selezione del metodo di trasporto) che quello della "Custom Label 2"
(determinato invece dalla selezione del pagamento)

![](./assets/media/image33.png)

Nel momento in cui invece, sia per il metodo di trasporto che per il
pagamento selezionato dall'utente in fase di checkout dovesse essere
stato impostato un valore per la stessa Custom Label, verranno passate a
Qaplà ed inserite nello stesso campo entrambe queste informazioni
separate da un ;

Supponendo dunque di aver impostato la "Custom Label 1" per il metodo di
trasporto selezionato in fase di checkout sul valore "opzione A" e la
stessa "Custom Label 1" per il pagamento selezionato in fase di checkout
sul valore "opzione B" ci ritroveremo poi su Qaplà una situazione del
tipo di quella rappresentata in figura

![](./assets/media/image34.png)

Infine, se conflitto dovesse verificarsi a livello di "Tipologia di
assicurazione" verrà utilizzato il seguente livello di priorità:

- Totale ordine

- Merce + trasporto

- Merce

- Disabilitata

Ciò significa dunque che nel momento in cui l'utente dovesse selezionare
in fase di checkout ad esempio, un metodo di trasporto configurato per
passare a Qaplà come importo da assicurare il Totale Merce + le spese di
trasporto e un pagamento configurato invece per passare a Qaplà come
importo da assicurare il Totale Ordine, seguendo l'ordine di priorità
sopra indicato l'importo da assicurare effettivamente passato a Qaplà
per quel determinato documento sarà proprio il Totale Ordine.

