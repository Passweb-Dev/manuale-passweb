# ORDINI



All'interno della sezione "**Ordini**" è possibile decidere se l'Account
in esame dovrà interagire o meno con Amazon anche a livello di ordini ed
eventualmente in che modo.

![](./assets/media/image191.png)

Nello specifico il campo:

**Creare ordini in Passweb:** consente di decidere se l'Account in esame
dovrà o meno interagire con Amazon a livello di ordini. E' possibile
selezionare uno dei seguenti valori:

- **No:** selezionando questa opzione l'Account in esame potrà
  interagire con i Marketplace Amazon **solo ed esclusivamente a livello
  di esportazione articoli**.

> **ATTENZIONE!** In queste condizioni eventuali ordini acquisiti su
> Amazon a seguito dell'acquisto di articoli messi in vendita a partire
> da sito Passweb non potranno in alcun modo essere importati su
> Passweb, ne tanto meno, all'interno del gestionale.

- **Si:** selezionando questa opzione l'integrazione tra Passweb e
  Amazon sarà completa.

> Sarà quindi possibile non solo esportare articoli **ma anche importare
> all'interno del proprio sito Passweb e da qui all'interno del
> gestionali, eventuali nuovi ordini (e relativi clienti) acquisiti
> direttamente sul marketplace di Amazon**

**Data Ultima Sincronizzazione Ordini:** consente di visualizzare ed
eventualmente reimpostare secondo le proprie esigenze quella che verrà
poi considerata da Passweb come la data in cui è stata effettuata
l'ultima sincronizzazione ordini tra Passweb stesso ed il Marketplace.

Tale campo potrebbe quindi rivelarsi particolarmente utile nel momento
in cui, ad esempio, si dovesse rendere necessaria una sincronizzazione
manuale per forzare la lettura e l'eventuale importazione dal
marketplace di ordini effettuati in una data successiva a quella
impostata all'interno di questo campo.

**Magazzino degli articoli gestiti (MFN):** consente di indicare lo
specifico magazzino che dovrà essere utilizzato e quindi movimentato in
relazione ad ordini provenienti dal Marketplace e contenenti articoli
gestiti in modalità MFN

**Magazzino Ordini degli Articoli gestiti AFN:** consente di indicare lo
specifico magazzino che dovrà essere utilizzato e quindi movimentato in
relazione ad ordini provenienti dal Marketplace e contenenti articoli
gestiti in modalità AFN.

**Si ricorda inoltre che nel caso di ordini contenenti articoli gestiti
in modalità AFN, per ragioni di privacy, Amazon non fornisce a
piattaforme esterne dati inerenti ad esempio il nominativo o l'indirizzo
dell'utente che ha effettuato l'ordine sul Marketplace**. Tali ordini
potranno comunque essere acquisiti su Passweb ma, in conseguenza di
quanto appena detto, saranno ovviamente incompleti e, di base, prima di
poterli inserire nel gestionale sarà quindi necessario inserire
manualmente i dati mancanti.

Nel momento in cui si volesse comunque acquisire comunque in maniera
automatica anche questi ordini incompleti, ad esempio perché l'unica
esigenza in merito ad essi è quella di averli nel gestionale per poter
così aggiornare in maniera corretta i progressivi degli articoli, sarà
necessario attivare il relativo modulo presente su Passstore (Amazon
Gestione Ordini AFN)

Per maggior informazioni in merito si veda anche il successivo capitolo
"*Amazon -- Gestione Ordini -- Ordini AFN* di questo manuale)

Nel passaggio dalla modalità di gestione MFN a quella AFN Amazon azzera
le quantità degli articoli per cui il magazzino in oggetto verrà
utilizzato solo ed esclusivamente come magazzino di testata per gli
ordini provenienti dal Marketplace e contenenti articoli gestiti da
Amazon.

**Su tale magazzino non verrà effettuato nessun tipo di calcolo per le
regole di pubblicazione automatica degli articoli.**

**ATTENZIONE!** A default i due campi sopra indicati verranno
valorizzati con il magazzino impostato a livello generale come magazzino
degli ordini Passweb alla pagina "*Ordini -- Gestione Ordini --
Configurazione Ordini*" del Wizard

**Sezionale degli Ordini:** consente di indicare uno specifico
sezionale, tra quelli codificati all'interno del gestionale, in cui
verranno memorizzati gli ordini acquisiti direttamente dal relativo
marketplace Amazon

**Codici Mastro dei Clienti**: consente di indicare lo specifico codice
Mastro del gestionale in cui verranno poi memorizzati i clienti
acquisiti direttamente dal relativo marketplace Amazon

**Codice Cliente per Ordini Incompleti da Logistica Amazon**:
utilizzabile solo nel caso in cui si sia deciso di attivare il modulo
Passstore **Amazon Gestione Ordini AFN.** Consente di indicare il codice
conto di un cliente fittizio (che dovrà ovviamente esistere all'interno
del gestionale) cui verranno associati tutti gli ordini prelevati dal
marketplace che dovessero venire a trovarsi nello stato "**Incompleto da
Logistica Amazon**" in maniera tale da poterli così inserire comunque
nel gestionale in maniera completamente automatica aggiornando i
progressivi dei relativi articoli.

Per maggiori informazioni relativamente al modulo "Amazon Gestione
Ordini AFN" si veda anche quanto indicato nel relativo capitolo di
questo manuale ("*Marketplace -- Amazon -- Gestione Ordini -- Ordini
AFN*")

**Numero Causale Movimento di Magazzino Documento**: consente di
indicare il numero della Causale che dovrà essere utilizzata,
all'interno del gestionale, per indicare che l'ordine corrispondente è
stato originato sui marketplace Amazon

**ATTENZIONE!** Nel momento in cui per il campo in esame non dovesse
essere indicato uno specifico valore, come Numero della Causale del
Movimento di Magazzino verrà utilizzato quello impostato in
corrispondenza dello stesso parametro presente alla pagina "**Ordini --
Configurazione Ordini**" del Wizard

**Numero del centro di Costo/Ricavo**: consente di indicare il numero da
attribuire al campo "**Costi/ricavi",** presente nella testata del
relativo documento gestionale, nel caso in cui l'ordine provenga da un
marketplace Amazon

**ATTENZIONE!** Nel momento in cui per il campo in esame non dovesse
essere indicato uno specifico valore, come Numero del Centro di
Costo/Ricavo verrà utilizzato quello impostato in corrispondenza dello
stesso parametro presente alla pagina "**Ordini -- Configurazione
Ordini**" del Wizard

**Vettore del Documento:** consente di impostare il Vettore che dovrà
essere inserito a default nel piede del documento gestionale generato a
seguito di ordini, acquisiti direttamente da Amazon, con spese di
spedizione maggiori di 0.

**ATTENZIONE!** E' possibile selezionare solo ed esclusivamente Vettori
codificati all'interno del gestionale ed esportati all'interno del
proprio sito Passweb.

**Vettore del Documento per spedizioni gratis:** consente di impostare
il Vettore che dovrà essere inserito a default nel piede del documento
gestionale generato a seguito di ordini, acquisiti direttamente da
Amazon, con spese di spedizione nulle.

Anche in questo caso sarà possibile selezionare solo ed esclusivamente
Vettori codificati all'interno del gestionale ed esportati all'interno
del proprio sito Passweb

**Articolo Spesa per Spedizione Standard:** consente di impostare,
selezionandolo dal relativo menu a tendina, l'articolo Spesa da
utilizzare per gestire le spese di spedizione di articoli venduti
all'interno del Marketplace con "Spedizioni Standard"

**Articolo Spesa per Spedizione Express:** consente di impostare,
selezionandolo dal relativo menu a tendina, l'articolo Spesa da
utilizzare per gestire le spese di spedizione di articoli venduti
all'interno del Marketplace con "Spedizioni Express"

**ATTENZIONE! Il costo delle spese di spedizione può essere definito
solo ed esclusivamente all'interno del Back end di Amazon dalla relativa
sezione "Impostazioni di Spedizione".**

![Videate\\amazon_gruppo_costi_spedizione2.bmp](./assets/media/image192.png)

All'interno di questa sezione sarà infatti possibile impostare diversi
"Gruppi di costi di spedizione" definendo per ciascuno di essi specifici
costi sia per le spedizioni di tipo Standard che per quelle di tipo
Express.

Nel momento in cui un cliente dovesse acquistare sul marketplace un
determinato articolo selezionando per esso, ad esempio, una spedizione
"Standard", nel corpo del relativo documento gestionale verrà inserito
l'articolo spesa indicato all'interno del campo "**Articolo Spesa per
Spedizione Standard**" con un valore pari a quello definito, su Amazon,
per la spedizione di tipo standard all'interno del gruppo dei costi di
spedizione associato all'articolo in esame.

**ATTENZIONE!** Gli stessi parametri possono anche essere impostati a
livello di singola inserzione e, in questo caso, avranno priorità
rispetto a quelli definiti in generale livello di account

In conseguenza di ciò, nel momento in cui si dovesse decidere di
impostare**"** , ad esempio, per il parametro "**Articolo Spesa per
Spedizione Standard** l'articolo "Spesa A" a livello di account e
l'articolo "Spesa B" a livello invece di singola inserzione, nel momento
in cui dovesse poi entrare un ordine Amazon con un articolo appartenente
all'inserzione in esame, all'interno del relativo documento gestionale
le spese di spedizione saranno gestite con l'articolo "Spesa B"

La sezione "**Stati Ordine**" consente, infine, di definire gli stati
degli ordini Amazon che dovranno essere utilizzati come filtro di
importazione sul Gestionale.

![](./assets/media/image193.png)

Nel box di sinistra sono elencati gli stati degli ordini Amazon che
possono essere gestiti da Passweb in fase di importazione.

Per fare in modo che gli ordini che si trovano, su Amazon, in uno degli
stati indicati possano essere importati in Passweb (e quindi nel
gestionale Passepartout) sarà sufficiente selezionare lo stato in
questione tra quelli presenti in elenco e inserirlo nel box di destra
cliccando sul pulsante raffigurante una piccola freccia verde rivolta
verso destra.

**ATTENZIONE! In fase di sincronizzazione verranno prelevati da Amazon
ed inseriti, tramite Passweb, nel gestionale Passepartout, solo ed
esclusivamente quegli ordini che si trovano in uno degli stati indicati
all'interno del box di destra**

Indipendentemente dagli stati gestiti, nel momento in cui un determinato
documento dovesse essere importato in Passweb e conseguentemente nel
gestionale Passepartout, questo verrà ovviamente considerato come un
normale ordine.

In altri termini dunque se si dovesse decidere, ad esempio, di importare
anche ordini in stato "Shipped" (ossia ordini che per Amazon sono già
stati spediti) questi verranno poi inseriti nel gestionale Passepartout
allo stesso modo degli ordini in stato "Unshipped". **Non verranno
quindi create automaticamente bolle / fatture o altri tipi di documento
ne tanto meno questi ordini verranno posti automaticamente in uno stato
particolare.**

Nel corpo del documento verrà comunque inserita una nota con
l'indicazione dello stato in cui si trovava l'ordine Amazon nel momento
in cui quello stesso ordine è stato effettivamente importato

**ATTENZIONE!** **In ogni caso occorre sempre prestare particolare
attenzione alle operazioni e ad eventuali cambi di stato che verranno
poi effettuati lato gestionale sugli ordini importati. Al fine di
evitare problemi tali operazioni dovranno infatti essere sempre coerenti
con quello che è lo stato in cui si trovano gli stessi documenti
all'interno della piattaforma terza**

Tornando all'esempio precedente, se si dovesse decidere di importare
anche gli ordini già spediti questi, una volta inseriti nel gestionale,
potrebbero anche essere trasformati in bolla o fattura (se necessario)
ma prestando particolare attenzione a non scatenare poi, a seguito di
questa trasformazione, eventuali cambi di stato anche sull'ordine Amazon
che, a questo punto, potrebbero anche non essere corretti.

