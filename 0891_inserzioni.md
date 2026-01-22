# INSERZIONI



Una volta terminata correttamente la configurazione dell'Account, il
passo successivo sarà quello di creare le Inserzioni mediante cui poter
definire esattamente quali dovranno essere i dati articolo (Titolo,
Categoria Merceologia, Immagini ...) da trasferire sulla piattaforma
terza e quelle che dovranno essere le regole di pubblicazione da
applicare in fase di esportazione dati.

**ATTENZIONE! Il metodo scelto per la pubblicazione degli articoli (Api
o Pubblicazione via csv) non influenza in alcun modo la creazione e la
gestione delle Inserzioni.**

In altri termini dunque con l'Inserzione andremo a definire esattamente
quali informazioni dovranno essere passate alla piattaforma terza per
ogni singolo prodotto, in quale lingua e quali dovranno essere le regole
di pubblicazione / arresto automatico.

Il metodo di pubblicazione scelto definisce invece il modo in cui i dati
articolo, stabiliti all'interno delle Inserzioni, verranno
effettivamente passati alla piattaforma terza.

In particolare dunque nel momento in cui si dovesse decidere di
pubblicare gli articoli:

- **via Api**: i dati impostati nelle Inserzioni verranno trasferiti ed
  inseriti sulla piattaforma terza in maniera automatica sfruttando,
  appunto, le API messe a disposizione dalla piattaforma stessa

- **via CSV**: i dati impostati nelle Inserzioni verranno pubblicati
  all'interno di appositi file csv. Tali file potranno poi essere
  scaricati direttamente dal Wizard di Passweb e uplodati manualmente
  sulla piattaforma terza oppure, al termine della pubblicazione,
  potranno essere copiati automaticamente all'interno di un'area
  condivisa (Ftp, Google Drive ...) stabilita in fase di configurazione
  dell'Account.

La colonna "**Destinazione**" presente nella maschera di configurazione
delle singole Inserzioni (tab "**Specifiche**") consente di
visualizzare, per ogni specifica gestita, quella che è la sua
destinazione e quindi se questa stessa specifica verrà poi presa in
considerazione nella pubblicazione via API, nella pubblicazione via CSV
o in entrambi i casi

![](./assets/media/image493.png)

Per maggiori informazioni in merito a come poter creare o gestire
un'Inserzione si veda invece quanto indicato all'interno del capitolo
"*Altri Marketplace -- Gestione Inserzioni*".

Per maggiori informazioni relativamente ai due diversi possibili metodi
di pubblicazione articoli si veda invece quanto indicato nel capitolo di
"*Marketplace -- Altri Marketplace - Google Merchant -- Configurazione
Account -- Metodi di pubblicazione articoli*" di questo manuale

**ATTENZIONE!** in ogni caso nel momento in cui gli articoli da gestire
dovessero essere dell'ordine delle migliaia, è sempre preferibile
utilizzare una pubblicazione via csv inquanto i tempi pubblicazione via
API, in queste condizioni, potrebbero essere particolarmente elevati
(senza considerare eventuali limiti imposti dalla piattaforma terza in
merito al numero di chiamate API giornaliere effettivamente gestibili).

Di seguito vengono elencate le Specifiche Standard, obbligatorie e
opzionali, di cui tener conto in fase di creazione di una nuova
Inserzione.

##### SPECIFICHE OBBLIGATORE 

Di seguito vengono riportate le Specifiche obbligatorie necessarie per
poter creare in maniera corretta Inserzioni mediante le quali poter
pubblicare articoli all'interno del Google Merchant Center.

![](./assets/media/image494.png)

**ATTENZIONE!** Indipendentemente dal fatto che la specifica considerata
sia una di quelle obbligatorie o una di quelle addizionali la cosa
importante da tenere sempre in considerazione è che **nel momento in cui
tali specifiche vengano mappate con "Attributi Passweb" il valore che
esse andranno ad assumere articolo per articolo, all'interno di Passweb,
dovrà essere necessariamente uno dei valori effettivamente accettati e/o
presenti anche sulla piattaforma terza**.

In conseguenza di ciò se, per determinati articoli, il valore assunto
per una specifica mappata con un Attributo Passweb dovesse non
combaciare con uno dei valori ammessi per la specifica stessa lato
Google, la pubblicazione degli articoli coinvolti in un inserzione che
fa uso di quella stessa specifica potrebbe dare degli errori.

Oltre alle specifiche di seguito indicate, in fase di pubblicazione
verranno passate alla piattaforma terza, per ciascuno degli articoli
coinvolti nell'Inserzione anche le seguenti informazioni:

- **codice gestionale** dell'articolo mappato

- **immagine principale della scheda prodotto**

> Nel momento in cui l'esigenza dovesse essere quella di inviare alla
> piattaforma terza altre immagini, sarà necessario utilizzare la
> relativa specifica addizionale

###### TITOLO

Nome dell'articolo pubblicato sulla piattaforma terza

**Modalità ammesse:** Attributo Articolo / Attributo Passweb

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato unicamente sulla seguente
opzione:

- **Titolo**: in questo caso il nome dell'articolo da passare alla
  piattaforma terza sarà esattamente lo stesso di quello visualizzato in
  Passweb all'interno del componente "Titolo". In questo senso
  l'effettivo valore (descrizione presente nell'anagrafica gestionale,
  valore di un attributo o valore personalizzato) dipendono direttamente
  da come si è deciso di gestire il "Titolo" dell'articolo

###### DESCRZIONE

Descrizione estesa dell'articolo pubblicato sulla piattaforma terza

**Modalità ammesse:** Attributo Articolo / Attributo Passweb /
Personalizzato

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato su una delle seguenti
opzioni:

- **Titolo**: in questo caso il valore della descrizione estesa da
  passare alla piattaforma terza sarà esattamente lo stesso di quello
  visualizzato in Passweb all'interno del componente "Titolo". In questo
  senso l'effettivo valore (descrizione presente nell'anagrafica
  gestionale, valore di un attributo o valore personalizzato) dipendono
  direttamente da come si è deciso di gestire il "Titolo" dell'articolo

- **Descrizione:** in questo caso il valore della descrizione estesa da
  passare alla piattaforma terza sarà esattamente lo stesso di quello
  visualizzato in Passweb all'interno del componente "Descrizione" (e
  quindi la descrizione inserita per l'articolo in Docuvision o
  direttamente nell'apposito campo dell'Anagrafica Passweb)

- **Descrizione HTML / 2 / 3**: in questo caso il valore della
  descrizione estesa da passare alla piattaforma terza sarà esattamente
  lo stesso di quello presente all'interno dei campi "Descrizione HTML /
  2 / 3" presenti nella sezione "Descrizioni" dell'anagrafica Passweb
  del relativo articolo

- **Descrizione estesa**: in questo caso il valore della descrizione
  estesa da passare alla piattaforma terza sarà esattamente lo stesso di
  quello visualizzato in Passweb presente all'interno del campo
  "Descrizione Dettagliata" presente nella sezione "Descrizioni"
  dell'anagrafica Passweb del relativo articolo

###### MARCA

Marca del prodotto pubblicato sulla piattaforma terza

**Modalità ammesse:** Attributo Articolo / Attributo Passweb /
Personalizzato

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato su una delle seguenti
opzioni:

- **Natura:** in questo caso il valore della marca passato alla
  piattaforma terza sarà esattamente quello indicato, per il relativo
  articolo, all'interno della sua anagrafica gestionale in
  corrispondenza del campo "Natura"

- **Categoria Statistica:** in questo caso il valore della marca passato
  alla piattaforma terza sarà esattamente quello indicato, per il
  relativo articolo, all'interno della sua anagrafica gestionale in
  corrispondenza del campo relativo alla "Categoria Statistica"

<!-- -->

- **Nominativo Fornitore:** in questo caso il valore della marca passato
  alla piattaforma terza corrisponderà con la Ragione Sociale del
  fornitore principale (Fornitore 1) dell'articolo in questione

![](./assets/media/image495.png)

> **ATTENZIONE!** Nel caso di siti Ecommerce collegati ad uno dei
> gestionali Ho.Re.Ca. è necessario abilitare, in "**Replica Dati**" il
> canale relativo ai fornitori. In caso contrario infatti non verranno
> esportate sul sito le informazioni dei fornitori

![](./assets/media/image496.png)

Nel momento in cui la marca dovesse essere gestita all'interno di un
campo differente da quelli appena considerati e si voglia comune creare
un'Inserzione dinamica mediante cui poter pubblicare sulla piattaforma
terza articoli diversi appartenenti a marche diverse sarà necessario
mappare la specifica in esame sulla modalità "Attributo Passweb"
selezionando poi dal relativo menu a tendina l'Attributo Passweb
deputato a gestire questo tipo di informazione

###### GTIN

Global Trade Item Number è un codice (UPC, EAN, ISBN) utilizzato per
identificare univocamente il prodotto pubblicato sulla piattaforma terza

**Modalità ammesse:** Attributo Articolo / Attributo Passweb /
Personalizzato

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato su una delle seguenti
opzioni:

- **Codice:** in questo caso il codice passato alla piattaforma terza
  sarà esattamente il codice gestionale del relativo articolo

- **Codice Alternativo:** in questo caso il codice passato alla
  piattaforma terza coinciderà esattamente con il codice alternativo
  impostato per l'articolo stesso all'interno del gestionale

- **Codice Alias GTIN:** in questo caso il codice passato alla
  piattaforma terza coinciderà esattamente con il codice alias impostato
  per l'articolo stesso all'interno del gestionale e opportunamente
  marcato come codice GTIN.

> **ATTENZIONE!** a differenza del codice e del codice alternativo,
> all'interno del gestionale possono essere definiti anche più codici
> alias per lo stesso prodotto.
>
> In queste condizioni l'applicazione si comporterà poi in maniera
> diversa a seconda del fatto che il gestionale collegato al sito
> Ecommerce sia Mexal oppure uno dei gestionali Ho.Re.Ca.
>
> **[SITI ECOMMERCE COLLEGATI A MEXAL]{.underline}**
>
> In questo caso è possibile marcare uno degli N codici alias in uso
> all'interno del gestionale in maniera tale da identificarlo
> esattamente come quello che dovrà poi essere passato ad Google
> Merchant in fase di pubblicazione dell'articolo.
>
> Per far questo è sufficiente accedere alla maschera di creazione del
> codice Alias

![](./assets/media/image87.png)

> e compilare i vari campi come di seguito indicato:

- **Codice**: inserire il valore del codice GTIN che dovrà essere
  passato alla piattaforma terza in fase di pubblicazione del prodotto

- **Descrizione:** per marcare lo specifico Codice Alias, tra gli N
  presenti, come il codice GTIN da passare alla piattaforma terza in
  fase di pubblicazione, sarà necessario indicare all'interno di questo
  campo la stringa **GTIN**

- **Elemento TG -- solo per articoli a Taglia:** indicare,
  selezionandola dall'apposito menu a tendina, la specifica Taglia cui
  il codice in esame dovrà essere riferita

> Supponendo dunque di aver utilizzato all'interno del gestionale N
> codici alias per un determinato articolo e di aver marcato in maniera
> corretta solo uno di essi come codice GTIN (secondo quanto sopra
> indicato) il corrispondente campo dell'Inserzione andrà poi impostato
> sul valore "**Codice Alias GTIN**" come evidenziato in figura

![](./assets/media/image497.png)

> In queste condizioni in fase di pubblicazione verrà passato alla
> piattaforma terza il codice alias marcato sul gestionale in maniera
> specifica come codice GTIN.
>
> **[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI
> HO.RE.CA.]{.underline}**
>
> In questo caso sarà possibile mappare il campo GTIN con il codice
> alias di una determinata tipologia (es. Codice EAN13, Codice EAN8
> ecc...) selezionandola tra quelle in uso all'interno del gestionale.
>
> A differenza di Mexal in questo caso però, non è possibile marcare uno
> degli N codici alias o EAN in uso all'interno del gestionale come
> quello che identifica in maniera specifica il codice da passare alla
> piattaforma terza in fase di pubblicazione pertanto, nel momento in
> cui un determinato articolo dovesse avere più valori per la stessa
> tipologia di Alias verrà considerato, ai fini dell'inserzione, solo il
> primo valore utile.

###### MPN

Codice assegnato dal produttore all'articolo pubblicato sulla
piattaforma terza

**Modalità ammesse:** Attributo Articolo / Attributo Passweb

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato su una delle seguenti
opzioni:

- **Codice:** in questo caso il codice passato alla piattaforma terza
  sarà esattamente il codice gestionale del relativo articolo

- **Codice Alternativo:** in questo caso il codice passato alla
  piattaforma terza coinciderà esattamente con il codice alternativo
  impostato per l'articolo stesso all'interno del gestionale

###### CONDIZIONE

Condizione (es. nuovo, usato ....) dell'articolo pubblicato sulla
piattaforma terza

**Modalità ammesse:** Attributo Marketplace / Attributo Passweb

**ATTENZIONE!** Per non ottenere errori in fase di pubblicazione degli
articoli, tale specifica deve assumere per forza di cose uno dei valori
proposti direttamente dalla piattaforma terza.

Nel momento in cui tale specifica dovesse essere mappata sulla modalità
"**Attributo Marketplace**" portandosi poi nel campo valore verranno
immediatamente proposti tutti i possibili valori che la specifica in
esame può assumere.

In queste condizioni selezionando uno dei valori proposti, poi tutti gli
articoli pubblicati sulla piattaforma terza mediante l'inserzione in
esame, assumeranno come valore per la specifica "Condizione" quello
impostato all'interno di questo campo.

Nel caso in cui l'esigenza dovesse essere quella di gestire
un'Inserzione più dinamica facendo in modo di pubblicare mediante essa
articoli che presentino valori diversi per la specifica in esame, sarà
necessario mapparla sulla modalità "**Attributo Passweb**" selezionando
poi dal relativo menu a tendina l'attributo deputato a gestire questo
tipo di informazione.

L'attributo indicato dovrà quindi essere valorizzato articolo per
articolo prestando comunque particolare attenzione al fatto di inserire
sempre uno dei valori effettivamente accettati dalla piattaforma terza
(fare riferimento in questo senso all'elenco di opzioni visualizzate nel
momento in cui la specifica fosse mappata sulla modalità "Attributo
Marketplace")

##### SPECIFCHE ADDIZIONALI

Di seguito vengono riportate le principali Specifiche addizionali da
gestire nell'integrazione tra Passweb e Google Merchant Center

###### LINK_IMMAGINE_AGGIUNTIVO (ADDITIONAL_IMAGE_LINK)

Consente di indicare il numero di immagini aggiuntive da inviare alla
piattaforma terza oltre all'immagine principale della scheda prodotto.

**Modalità ammesse:** Attributo Passweb / Personalizzato

**ATTENZIONE!** La specifica **link_immagine_aggiuntivo
(additional_image_link)** è gestita come campo numerico

Nel caso in cui l'esigenza dovesse essere quella di inviare alla
piattaforma terza, per tutti per tutti gli articoli coinvolti
nell'Inserzione, lo stesso numero di immagini aggiuntive, sarà
necessario:

- mappare la specifica in oggetto sulla modalità "Personalizzato"

- inserire all'interno del campo Valore il numero di immagini aggiuntive
  da utilizzare

Nel caso in cui l'esigenza dovesse invece essere quella di passare per
diversi articoli coinvolti nell'inserzione un diverso numero di immagini
addizionali, sarà necessario:

- mappare la specifica in oggetto sulla modalità "Attributo Passweb"

- impostare il campo "Valore" sull'Attributo Passweb deputato a gestire
  per ogni singolo articolo questo tipo di informazione, prestando
  particolare attenzione al fatto che tale attributo sia di tipo
  numerico.

###### ID

Codice identificativo assegnato all'articolo direttamente dalla
piattaforma terza su cui l'articolo stesso è stato pubblicato

**Modalità ammesse:** Attributo Passweb / Personalizzato

Questa specifica è di fondamentale importanza, in quanto verrà
utilizzata come campo chiave nel momento in cui si vogliano agganciare,
in fase di pubblicazione articoli, dei prodotti già presenti sulla
piattaforma terza che, generalmente, non sono stati inseriti mediante
l'integrazione con Passweb

###### CATEGORIA

Categoria merceologica cui associare l'articolo all'interno della
piattaforma terza

**Modalità ammesse:** Attributo Marketplace / Attributo Articolo /
Attributo Passweb

**ATTENZIONE!** Nel caso di integrazione tra Passweb e Google
Merchant**, lo schema delle categorie merceologiche cui fare
riferimento** è quello messo a disposizione da Google stesso
(consultabile anche al seguente indirizzo
<https://support.google.com/merchants/answer/6324436?hl=it> )

In queste condizioni dunque codificando un' Inserzione al fine di
pubblicare articoli sul Merchant Center di Google sarà possibile
configurare la Specifica "**Categoria**" impostandola sulla modalità
"**Attributo Marketplace**"

![](./assets/media/image498.png)

Il campo "**Valore**" verrà gestito come un campo ad autocompletamento
per cui iniziando a digitare alcuni caratteri (relativamente a quella
che si possa pensare essere la categoria merceologica degli articoli
coinvolti nell'Inserzione) verranno automaticamente visualizzate le
categorie merceologiche predisposte da Google e coerenti con quanto
digitato dall'utente.

Sarà quindi sufficiente selezionare, tra quelle proposte, l'opzione
desiderata in maniera tale da inserire all'interno del campo
"**Valore**" il percorso completo della categoria merceologica cui
dovranno appartenere tutti gli articoli pubblicati mediante l'Inserzione
in esame.

**ATTENZIONE!** Lavorando in questo tutti gli articoli pubblicati
mediante l'Inserzione in esame verranno associati, ovviamente, alla
stessa categoria merceologica (quella indicata, appunto, all'interno del
campo Valore)

Nel caso in cui si voglia ottenere qualcosa di più dinamico, in maniera
tale da poter sfruttare una stessa Inserzione per pubblicare sulla
piattaforma terza articoli appartenenti a diverse categorie
merceologiche sarà necessario configurare la Specifica "**Categoria**"
impostandola, questa volta, sulla modalità "**Attributo Articolo**"

![](./assets/media/image499.png)

In queste condizioni il campo "**Valore**" verrà gestito come una combo
box e l'unica opzione di scelta disponibile sarà "**Google Categoria
Prodotto**"

Ciò significa che per ogni articolo pubblicato mediante l'Inserzione in
esame il valore relativo alla categoria merceologica di appartenenza
coinciderà esattamente con quanto impostato in corrispondenza del campo
"**Google Product Category**" presente all'interno della sezione
"**Marketplace**" nell' Anagrafica Passweb della effettiva categoria
merceologica di appartenenza dell'articolo.

![](./assets/media/image500.png)

Il campo **"Google Product Category"** è infatti un campo ad
autocompletamento e, come nel caso precedente per il campo Valore, anche
questa volta iniziando a digitare alcuni caratteri (relativamente a
quella che si possa pensare essere la categoria merceologica
corrispondente nella tassonomia di Google) verranno automaticamente
visualizzate le categorie merceologiche predisposte da Google e coerenti
con quanto digitato dall'utente.

Lavorando in questo modo potrebbe quindi essere possibile assegnare a
due articoli appartenenti su Passweb a due categorie merceologiche
completamente diverse (es. Smartphone e Televisori) due altrettanto
diverse categorie Google. Questi stessi articoli potrebbero quindi
essere pubblicati su Google Merchant utilizzando la stessa inserzione e
associandoli allo stesso tempo, sulla piattaforma terza, a due diverse
categorie merceologiche.

###### PESO_SPEDIZIONE

Consente di indicare il peso del articolo pubblicato sulla piattaforma
terza.

**Modalità ammesse:** Attributo Articolo / Attributo Passweb /
Personalizzato

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato unicamente sulla seguente
opzione:

- **Peso**: in questo caso il valore del peso passato alla piattaforma
  terza sarà esattamente quello indicato, per il relativo articolo,
  all'interno della sua Anagrafica Passweb in corrispondenza del campo
  "**Peso -- kg**" (tab "**Spedizione**" sezione "**Dimensioni
  Imballo**")

###### CUSTOM LABEL 0/1/2/3/4

Etichette personalizzate mediante cui poter associare agli articoli
pubblicati sulla piattaforma terza informazioni di diverso tipo

**Modalità ammesse:** Attributo Articolo / Attributo Passweb /
Personalizzato

Mappando la specifica in esame sulla modalità "**Attributo Articolo**"
il campo valore potrà poi essere impostato su una delle seguenti
opzioni:

- **Passweb Categoria Prodotto**: in questo caso il valore da passare
  alla piattaforma terza, e che verrà poi memorizzato nella
  corrispondente etichetta personalizzata, coinciderà esattamente con il
  nome della categoria merceologica principale cui risulterà essere
  associato su Passweb (e quindi anche sul gestionale Passepartout) il
  relativo articolo

- **Articolo in offerta**: in questo caso il valore da passare alla
  piattaforma terza, e che verrà poi memorizzato nella corrispondente
  etichetta personalizzata, varierà in relazione al fatto che l'articolo
  coinvolto nell'inserzione abbia o meno un sconto. Nello specifico:

  - Nel caso in cui l'articolo coinvolto nell'inserzione dovesse avere
    uno sconto la custom label verrà valorizzata con l'etichetta
    "OFFERTA"

  - Nel caso in cui l'articolo coinvolto nell'inserzione non dovesse
    avere sconti di alcun tipo non verrà passato alla piattaforma terza
    alcun valore e, di conseguenza, la corrispondente custom label
    risulterà vuota

###### SPECIFCHE PER ARTICOLI VARIANTI

- colore (color)

- motivo (pattern)

- materiale (material)

- taglia (size)

- sesso (gender)

- età (age_group)

Per maggiori informazioni relativamente a come gestire inserzioni con
articoli che presentano un massimo di due elementi varianti (es. Taglie
e Colori) si veda anche quanto indicato all'interno del capitolo
"*Marketplace -- Altri Marketplace -- Articoli a Taglie / Colori"* di
questo manuale.

##### SPECIFICHE CUSTOM

Come già evidenziato nei precedenti capitoli di questo manuale
all'interno di Inserzioni per la pubblicazione di prodotti su Google
Merchant, è possibile utilizzare, oltre alle Specifiche Standard
(obbligatorie e addizionali) anche delle Specifiche Custom

Tali specifiche dovranno prima essere codificate all'interno della
corrispondente sezione del Wizard (*Catalogo -- Altri Marketplace --
Specifiche*)

![](./assets/media/image501.png)

Una volta codificate sarà poi possibile gestirle, per ogni singola
Inserzione, esattamente allo stesso modo in cui si gestiscono le
specifiche standard precedentemente analizzate.

Per maggiori informazioni in merito a come poter codificare delle nuove
specifiche custom per Google Merchant si veda anche quanto indicato
all'interno del capitolo "*Marketplace -- Altri Marketplace -- Gestione
Specifiche -- Specifiche Custom Google / Facebook per pubblicazioni via
API / CSV"* di questo manuale.

**ATTENZIONE!** ogni Specifica Custom potrà essere utilizzata solo in
relazione al Marketplace e al tipo di pubblicazione per cui è stata
definita.

**GESTIONE QUANTITA'**

Come evidenziato nei precedenti capitoli di questo manuale la quantità
con cui un determinato articolo verrà pubblicato sulla piattaforma terza
dipende esattamente dalle impostazioni settate all'interno della sezione
"**Quantità**" presente nella maschera di configurazione della specifica
Inserzione (tab "Prezzo, quantità e formato") utilizzata per pubblicare
i prodotti.

![](./assets/media/image502.png)

Per maggiori informazioni in merito ai parametri di configurazione
presenti all'interno di questa sezione si rimanda a quanto indicato
all'interno del capitolo "*Altri Marketplace -- Gestione Inserzioni --
Creazione di una nuova inserzione -- Prezzo Quantità Formato --
Quantità*" di questo manuale

**ATTENZIONE!** Nel valutare quella che per Passweb è la quantità
effettiva di un certo articolo su di un determinato magazzino occorre
sempre tener conto:

- di quanto impostato alla pagina "**Catalogo -- Configurazione
  Parametri Catalogo**" all'interno della sezione "Disponibilità", sia
  in termini di **formula utilizzata** per il calcolo della
  disponibilità che in termini di **Scorta Minima**

- del fatto che la quantità disponibile su Passweb e, conseguentemente,
  la quantità con cui un determinato articolo potrebbe poi essere
  pubblicato sulla piattaforma terza, **potrebbe essere determinata
  anche dall'attivazione, per l' articolo stesso, della sua unità di
  misura secondaria** e dal relativo fattore di conversione impostato
  direttamente sul gestionale.

> Per maggiori informazioni in merito alla gestione dell'unità di misura
> secondaria si veda anche quanto indicato nel relativo capitolo di
> questo manuale (*Configurazione -- Mexal Configurazione Gestionale --
> Attivazione Passweb -- Funzionalità Mexal Articoli -- Gestione unità
> di misura principale / secondaria*)

##### GESTIONE PREZZI

**ATTENZIONE! Considerando che l'integrazione con Google prevede che
l'acquisto venga effettuato sempre all'interno del sito Ecommerce, il
prezzo pubblicato su Google Merchant dovrà essere esattamente lo stesso
di quello utilizzato sul sito.**

Nel momento in cui i due prezzi, quello utilizzato per l'inserzione
pubblicitaria e quello effettivamente applicato sul sito non siano
esattamente gli stessi, i relativi annunci (soprattutto nel caso di
Google) potrebbero anche essere sospesi o non validati dalla piattaforma
terza.

In questo tipo di integrazioni è quindi consigliabile:

- Utilizzare per l'inserzione lo stesso listino impostato come listino
  di default per il sito

- Lasciare invariato il campo "**Modifica del prezzo**"

- Applicare l'eventuale sconto che verrebbe visualizzato sul sito anche
  ad utenti non autenticati

Fatta questa osservazione di fondamentale importanza è bene sottolineare
anche che, nel caso di integrazione con **Google Merchant:**

- il prezzo di listino dei prodotti pubblicati sulla piattaforma sarà
  inserito all'interno del campo "**prezzo**" della corrispondente
  anagrafica articolo

![](./assets/media/image503.png)

- nel caso di articoli gestiti a confezione sul Merchant Center di
  Google verrà pubblicato all'interno del campo "prezzo" il prezzo della
  confezione e all'interno del campo "**multipack**" il numero di pezzi
  che compongono la confezione.

![](./assets/media/image504.png)

- nel caso in cui dovesse essere applicata anche una particolare
  categoria sconto (campo "Sconto Cliente" dell'Inserzione) il prezzo
  finale di vendita sulla piattaforma terza, risultato dello sconto
  applicato al prezzo di listino, verrà invece inserito all'interno del
  campo "**prezzo scontato**" della corrispondente anagrafica articolo

![](./assets/media/image505.png)

