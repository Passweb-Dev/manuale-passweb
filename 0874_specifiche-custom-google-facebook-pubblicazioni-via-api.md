# SPECIFICHE CUSTOM -- GOOGLE / FACEBOOK -- PUBBLICAZIONI VIA API



Nel momento in cui l'esigenza dovesse essere quella di gestire delle
Specifiche Custom da utilizzare in fase di pubblicazione articoli su
Google Merchant e/o Facebook Business Manager, la prima cosa da tenere
in considerazione è che, in queste condizioni, l'esigenza potrebbe
essere quella di gestire situazioni in cui il dato da inviare a Google
e/o Facebook potrebbe anche non avere un valore semplice e diretto come
avveniva con Prestashop o Magento, e potrebbe invece essere gestito con
una struttura più articolata come potrebbe essere, ad esempio, quella di
un oggetto, di un array, di un array di oggetti ...

In questo caso dunque, in fase di codifica della specifica, non sarà più
sufficiente assegnarle un nome ma occorrerà ricreare esattamente la
stessa struttura dati richiesta dalla piattaforma terza e questo sia nel
caso di pubblicazione via API che nel caso di pubblicazione via CSV,
dove anche l'intestazione della colonna destinata a contenere questi
dati, dovrà avere una sintassi ben precisa.

**Un'altra differenza rispetto a quanto indicato nel precedente capitolo
di questo manuale, è dunque che nel caso di Google e Facebook le
Specifiche Custom potranno tranquillamente essere utilizzate sia con
pubblicazioni via CSV che con pubblicazioni via API.**

Detto ciò, per codificare una nuova specifica di questo tipo è
necessario accedere alla sezione "**Gestione Specifiche**" del Wizard
(menu "*Catalogo -- Altri Marketplace*") e cliccare poi sul pulsante
**Aggiungi Specifica** (
![](./assets/media/image324.png) ) presente nella contestuale barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Dati
Specifica**"

![](./assets/media/image327.png)

all'interno della quale poter impostare tutti i parametri di
configurazione della specifica custom che si intende creare.

Sarà possibile indicare un valore per i seguenti campi .

**Nome**: consente di assegnare un nome descrittivo alla specifica che
si sta codificando in maniera tale da poterla poi identificare
univocamente tra tutte le specifiche custom effettivamente presenti in
elenco (il nome assegnato all'interno di questo campo sarà poi quello
mostrato in griglia in corrispondenza della colonna "Descrizione")

**Marketplace**: consente di indicare, selezionandolo da un apposito
menu a tendina, il Marketplace in relazione al quale potrà poi essere
utilizzata la specifica custom che si sta codificando.

In questo caso, ovviamente**, andrà selezionata l'opzione Google
Merchant o Facebook Business Manager**

**ATTENZIONE!** una volta assegnato un Marketplace ad una Specifica
questo non potrà più essere modificato. Nel caso in cui fosse necessario
apportare una modifica a questo parametro sarà quindi necessario
eliminare la specifica e crearne una nuova

**Pubblicazione:** consente di indicare il metodo di pubblicazione in
relazione al quale sarà poi possibile utilizzare la specifica in esame.

E' possibile selezionare uno dei seguenti valori:

- API

- CSV

- API e CSV

**ATTENZIONE!** le Specifiche Custom per Google e/o Facebook potranno
essere utilizzate sia con pubblicazioni via CSV che con pubblicazioni
via API

Ora, come già indicato, in queste condizioni per completare la codifica
della specifica custom potrebbe non essere sufficiente assegnarle un
nome (quello cioè che, nel caso di Prestashop o Magento, era gestito con
il campo "Tag") e questo perché il dato da inviare a Google e/o Facebook
potrebbe anche avere una struttura più complessa rispetto al semplice
"nome:valore" (che rimane comunque, anche in questo caso, una
possibilità).

Potremmo trovarci a dover inviare a Google e/o Facebook dati che,
secondo quanto richiesto da questi stessi marketplace, dovranno essere
gestiti con degli array, con degli oggetti, con degli array di oggetti
... e in questi casi, per non avere poi errori in fase di pubblicazione,
dovremo poter ricreare esattamente la struttura dati richiesta dal
Marketplace su cui andremo a pubblicare.

La sezione "**Struttura Specifica Custom**" evidenziata in figura, e
visualizzata solo nel momento in cui sia stata selezionata, per il
parametro "**Marketplace**", l'opzione Google Merchant o Facebook
Business Manager

![](./assets/media/image328.png)

consente proprio di fare questo, ossia ricreare esattamente la struttura
del dato da inviare così come richiesto dallo specifico Marketplace e
questo sia nel caso di "dato semplice" (del tipo "nome:valore") sia nel
caso di dato strutturato (es. array, oggetto, array di aggetti ecc...).

Il campo "**Preview Json**" consente di visualizzare in tempo reale la
struttura dati che si sta realizzando.

I pulsanti presenti all'interno di questa sezione consentono invece di:

**Aggiungi nodo** (
![](./assets/media/image329.png) ): consente di aggiungere un nuovo nodo
di tipo radice alla struttura dati che si sta realizzando.

I campi visualizzati dopo aver cliccato su questo pulsante consentono di
indicare, rispettivamente:

- il nome della specifica da codificare -- campo "**Elemento chiave**"

- la struttura dati con cui la specifica dovrà essere gestita (se è una
  proprietà semplice oppure se dovrà essere gestita come un oggetto,
  come un array ...) -- campo "**Tipo**"

In particolare per quel che riguarda **le diverse tipologie di strutture
dati che potranno essere abilitate per gestire una specifica custom,** è
possibile selezionare una delle seguenti opzioni:

- **Valore Semplice**: da selezionare nel caso in cui la specifica da
  inviare al marketplace dovesse essere gestita con un "dato semplice"

![](./assets/media/image330.png)

> e quindi con una struttura del tipo
>
> ***"nome specifica" : "valore"***
>
> In queste condizioni quando poi si andrà ad utilizzare la specifica in
> esame all'interno di determinate Inserzioni, occorrerà prestare
> attenziona al fatto che il campo con cui la specifica stessa verrà
> mappata sia effettivamente un campo che accetta solamente valori
> semplici (tipicamente delle stringhe)

- **Array di stringhe / Array di numeri**: da selezionare nel caso in
  cui la specifica da inviare al marketplace dovesse essere gestita come
  un Array di stringhe / Array di numeri

![](./assets/media/image331.png)

> e quindi con una struttura del tipo
>
> ***"nome specifica":\['valore1','valore2', ...'valoreN'\]*** oppure
> ***"nome specifica":\[numero1,numero2, ...numeroN\]***
>
> In queste condizioni quando poi si andrà ad utilizzare la specifica in
> esame all'interno di determinate Inserzioni, occorrerà prestare
> attenziona al fatto che il campo con cui la specifica stessa verrà
> mappata sia effettivamente un campo a valori multipli

- **Oggetto**: da selezionare nel caso in cui la specifica da inviare al
  marketplace dovesse essere gestita come un oggetto

![](./assets/media/image332.png)

> e quindi con una struttura del tipo
>
> ***"nome specifica" {***
>
> ***"nome proprietà\": tipo proprietà,***
>
> ***\"nome proprietà\": tipo proprietà,***
>
> ***\"nome proprietà\": tipo proprietà***
>
> ***...***
>
> ***}***
>
> in cui la specifica in esame potrà avere più proprietà ognuna delle
> quali dovrà essere indicata con una sintassi del tipo
> ***"chiave":"valore"***
>
> In questo caso infatti, una volta impostato il campo "**Tipo**"
> sull'opzione "**Oggetto**" verrà visualizzato il pulsante "**Aggiungi
> proprietà**" (
> ![](./assets/media/image333.png) mediante il quale poter aggiungere le
> singole proprietà all'oggetto in esame

![](./assets/media/image334.png)

> Nel momento in cui l'esigenza dovesse essere quella di creare la
> struttura dati di un oggetto "semplice" ogni proprietà dovrà,
> ovviamente, essere impostata sulla tipologia "Valore Semplice".
>
> Volendo è comunque possibile creare anche strutture dati più complesse
> come ad esempio, un oggetto di array o un oggetto di oggetti

- **Array di oggetti**: da selezionare nel caso in cui la specifica da
  inviare al marketplace dovesse essere gestita come un array di oggetti

![](./assets/media/image335.png)

> e quindi con una struttura del tipo
>
> ***"nome specifica":\[***
>
> ***{***
>
> ***"nome proprietà\": tipo proprietà,***
>
> ***\" nome proprietà\": tipo proprietà,***
>
> ***\" nome proprietà\": tipo proprietà***
>
> ***...***
>
> ***},***
>
> ***{***
>
> ***"nome proprietà\": tipo proprietà,***
>
> ***\" nome proprietà\": tipo proprietà,***
>
> ***\" nome proprietà\": tipo proprietà***
>
> ***...***
>
> ***},***
>
> ***....***
>
> ***\]***
>
> In questo caso, una volta impostato il campo "**Tipo**" sull'opzione
> "**Array di oggetti**" verrà visualizzato il pulsante "**Aggiungi
> elemento**" (
> ![](./assets/media/image336.png) ) grazie al quale poter aggiungere, in
> maniera manuale, i singoli oggetti all'array

![](./assets/media/image337.png)

> I due pulsante "**Aggiungi proprietà**" (
> ![](./assets/media/image333.png) ) e "**Rimuovi proprietà**" (
> ![](./assets/media/image338.png) ) consentiranno invece di aggiungere le
> singole proprietà ad ogni oggetto

![](./assets/media/image339.png)

**Pulisci Struttura** (
![](./assets/media/image340.png) ): consente di azzerare la struttura
dati che si sta realizzando

**Esporta JSON** (
![](./assets/media/image341.png) ): consente di esportare la struttura
dati in esame all'interno di un file JSON

**Importa JSON da file** (
![](./assets/media/image342.png) ): consente di creare automaticamente
una struttura dati più o meno complessa importandola direttamente da un
apposito file JSON.

Volendo dunque si potrebbe anche realizzare la struttura dati
esternamente a Passweb, creando il suo schema all'interno un file JSON
che una volta importato, consentirà a Passweb di creare automaticamente
tutti i campi necessari per gestire quella stessa struttura dati.

**ATTENZIONE! ovviamente per poter conoscere e replicare la struttura
dati richiesta per la gestione di una determinata specifica è di
fondamentale importanza consultare la documentazione del corrispondente
Marketplace.**

Anche in questo caso una volta completata la codifica, la specifica in
questione verrà poi resa disponibile, assieme a quelle "standard",
nell'elenco delle specifiche effettivamente gestibili per ogni
Inserzione, ma solo per il Marketplace e il metodo pubblicazione
indicati in fase di configurazione.

In particolare, nel caso di specifiche "semplici", come nel caso di
Prestashop e Magento, verrà indicato solo il nome della specifica custom
precedentemente realizzata

![](./assets/media/image326.png)

Nel caso invece di specifiche "composte" realizzate cioè con strutture
dati più complesse (es. array di oggetti) troveremo anche l'indicazione
di tutto il percorso della struttura fino alla foglia che dovrà poi
essere mappata con un Attributo / Campo Articolo e, nel caso in cui la
foglia faccia parte di un array, verrà indicato anche un numerino che
identifica la posizione (indice) dell'array a cui corrisponde quello
stesso elemento.

![](./assets/media/image343.png)

**Ovviamente, in fase di mapping della specifica custom, sarà di
fondamentale importanza assicurarsi del fatto che il Campo / Attributo
Articolo da cui verrà poi prelevato il dato sia della stessa tipologia
della specifica in esame.**

In altri termine nel momento in cui la specifica in esame dovesse essere
stata definita, ad esempio, con una struttura dati del tipo.

*"nome specifica": "valore specifica"* -- dove "valore specifica" è una
stringa

per evitare errori in fase di pubblicazione articoli, anche il Campo /
Attributo articolo con cui verrà mappata dovrà essere effettivamente un
campo di tipo stringa

**ATTENZIONE!** Per maggiori informazioni relativamente a come poter
inserire una determinata specifica in un Inserzione e su come mapparla,
si veda quanto indicato nel capitolo "*Gestione Inserzioni"* di questo
manuale

Anche in questo caso, infine, nel momento in cui si dovesse utilizzare
un metodo di pubblicazione via csv e si dovesse decidere di aggiungere /
eliminare delle specifiche custom dalle varie Inserzioni sarà necessario
accertarsi anche di aver correttamente svuotato il repository utilizzato
per la pubblicazione dei file in maniera tale da evitare incoerenza nei
dati presenti al loro interno e conseguenti problemi in fase di
importazione dati sulla piattaforma terza

##### ESEMPIO -- PUBBLICAZIONE VIA API

Per comprendere in maniera più chiara la differenza tra "dato semplice"
e "dato strutturato" e per capire anche come utilizzare al meglio la
sezione "**Struttura Specifica Custom**" analizzata nel precedente
capitolo di questo manuale, possiamo fare riferimento, ad esempio, a
quelle che sono le specifiche gestite da Google Merchant relativamente
alla pubblicazione via API, specifiche queste documentate al seguente
indirizzo

<https://developers.google.com/shopping-content/reference/rest/v2.1/products>

Osservando l'elenco delle specifiche presenti all'interno della sezione
"**JSON representation**", possiamo trovare specifiche gestite con un
"dato semplice" (del tipo "nome:valore"), come ad esempio '**material**'

![](./assets/media/image344.png)

ma anche specifiche gestite con un "dato strutturato" (nel caso
specifico, un array di oggetti) come ad esempio '**certification**'

![](./assets/media/image345.png)

Nel momento in cui l'esigenza dovesse essere quella di gestire la
specifica 'material' dovremo quindi creare una Specifica Custom del tipo
di quella rappresentata in figura

![](./assets/media/image346.png)

formata da un solo nodo radice di tipo "Valore Semplice"

Nel momento in cui l'esigenza dovesse essere invece quella di gestire la
specifica 'certification', la struttura dati da ricreare sarà quella di
un array di oggetti che, considerando anche la definizione dell'oggetto
'ProductCertification'
(<https://developers.google.com/shopping-content/reference/rest/v2.1/products#ProductCertification>),
dovrà quindi essere del tipo

*\"certifications\": \[*

*{*

*"certificationAuthority\": string,*

*\"certificationName\": string,*

*\"certificationCode\": string,*

*\"certificationValue\": string*

*},*

*{*

*"certificationAuthority\": string,*

*\"certificationName\": string,*

*\"certificationCode\": string,*

*\"certificationValue\": string*

*},*

*...*

*\]*

dove, ovviamente, all'interno dell'array

*\"certifications\": \[ \]*

dovranno essere inseriti tanti oggetti

*{*

*"certificationAuthority\": string,*

*\"certificationName\": string,*

*\"certificationCode\": string,*

*\"certificationValue\": string*

*}*

quante sono le certificazioni da inviare a Google Merchant.

In questo caso dovremo quindi creare una Specifica Custom del tipo di
quella evidenziata in figura

![](./assets/media/image347.png)

formata da un nodo radice di tipo "Array" e N nodi di secondo livello di
tipo "Oggetto" con all'interno un elemento di tipo "Valore Semplice" per
ogni proprietà richiesta (come da documentazione) per l'oggetto
"ProductCertification"

