# CREAZIONE DELL'INSERZIONE



Per poter pubblicare sui Marketplace Amazon articoli con un massimo di
due elementi varianti (es. taglie e colori) **è necessario utilizzare
apposite inserzioni** definendo in maniera corretta tutte le specifiche
necessarie per poter consentire all'inserzione stessa di gestire questa
ben precisa tipologia di articoli.

In particolare dunque una volta indicate la Categoria Articoli e la
Tipologia di Prodotto gestita per l'inserzione, sarà necessario
individuare dal successivo elenco le seguenti specifiche (specifiche
queste che dovranno essere obbligatoriamente aggiunte all'interno
dell'inserzione):

- **Parentage:** consente di abilitare l'inserzione che si sta
  realizzando per la gestione di articoli a Taglie

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie2.bmp](./assets/media/image279.png)

> **ATTENZIONE! In assenza di tale specifica l'inserzione potrà essere
> utilizzata per pubblicare solo ed esclusivamente articoli di magazzino
> "tradizionali"**
>
> La specifica **Parentage** può assumere solo ed esclusivamente il
> valore **child** che sarà quindi l'unica opzione possibile in fase di
> valorizzazione della specifica stessa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie1.bmp](./assets/media/image280.png)

- **Variation Theme:** consente di indicare quali sono gli elementi di
  variazione degli articoli (es. taglia, colore, taglia e colore, colore
  e taglia ecc...)

> **ATTENZIONE! E' possibile gestire fino ad un massimo di due diversi
> elementi di variazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie3.bmp](./assets/media/image281.png)

> Tale specifica **deve essere mappata con un "Attributo Amazon"** e
> dovrà quindi assumere necessariamente uno dei valori proposti nel
> relativo menu a tendina, valori questi forniti direttamente da Amazon
> e variabili in relazione alla particolare Categoria di articoli
> utilizzata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie4.bmp](./assets/media/image282.png)

Una volta definiti, mediante la specifica "Variation Theme", gli
elementi di variazione, sarà poi necessario inserire anche le
corrispondenti specifiche della sezione "**Variation Data**" in maniera
tale da avere poi a disposizione i campi necessari per valorizzare,
articolo per articolo, i suddetti elementi.

Supponendo dunque di aver impostato la specifica "Variation Theme" sul
valore **SizeColor**, indicando di fatto che i due elementi di
variazione degli articoli sono rispettivamente la Taglia e il Colore,
sarà poi necessario cercare e inserire all'interno dell'inserzione anche
le specifiche Size e Color della sezione "Variation Data"

- **Size (Nome categoria \> Variation Data \> Size )**

- **Color (Nome categoria \> Variation Data \> Color )**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie6.bmp](./assets/media/image283.png)

indicando inoltre da dove dovranno essere prelevati i valori sia per
l'una che per l'altra specifica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie5.bmp](./assets/media/image284.png)

In questo senso le opzioni possibili saranno, per i siti Ecommerce
collegati a Mexal, "**Tabella Taglie**" e "**Ultimo campo Struttura**".

Per i siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca. le
opzioni possibili saranno invece "**Ultimo campo Struttura**" e
"**Penultimo campo struttura**"

Facendo riferimento, ad esempio, alla configurazione indicata in figura
il colore (**Color**) degli articoli pubblicati sul marketplace
coinciderà con i valori, indicati lato gestionale, nell'ultimo livello
della struttura utilizzata mentre le taglie (**Size**) verranno
prelevate direttamente dai valori indicati nella tabella taglie di
Mexal.

Infine, per poter completare correttamente l'inserzione, sarà necessario
inserire, se non già presenti tra le specifiche attuali e sempre
relativamente agli elementi di variazione indicati, le corrispondenti
specifiche di tipo "**Map**"

Facendo riferimento, ancora una volta, alla configurazione indicata in
figura sarà quindi necessario gestire anche le due specifiche

- **Size Map**

- **Color Map**

Tali specifiche sono necessarie per poter strutturare correttamente il
file xml che verrà poi inviato ad Amazon in fase di pubblicazione
articoli e verranno valorizzate automaticamente da Passweb.

In fase di configurazione dell'inserzione queste ultime due specifiche
possono quindi essere mappate tranquillamente su valori
"**Personalizzati**" di qualsiasi tipo, in quanto, come detto, la loro
effettiva valorizzazione verrà poi effettuata direttamente da Passweb in
fase di pubblicazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\amazon_taglie8.bmp](./assets/media/image285.png)

**ATTENZIONE! Le inserzioni configurate con le specifiche indicate
all'interno di questo capitolo, e abilitate quindi per poter gestire
articoli a taglie / colori, potranno essere utilizzate solo ed
esclusivamente per la pubblicazione di questa particolare tipologia di
articoli**

Allo stesso modo inserzioni "tradizionali", utilizzate cioè per
pubblicare normali articoli di magazzino, non potranno mai essere
utilizzate per pubblicare articoli a taglie / colori

