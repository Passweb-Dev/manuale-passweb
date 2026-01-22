# CODIFICA AUTOMATICA DI NUOVE ANAGRFICHE ARTICOLO



Come evidenziato nei precedenti capitoli di questo manuale, volendo è
possibile fare in modo che eventuali articoli presenti nel documento
Prestashop, ma non ancora codificati nelle anagrafiche del gestionale,
vengano creati in maniera automatica contestualmente all'inserimento del
nuovo ordine.

**ATTENZIONE!** Per ovvie ragioni gli articoli codificati
automaticamente a seguito dell'acquisizione di ordini Prestashop saranno
tutti articoli semplici (su Mexal saranno ad esempio articoli di tipo
A). **NON verranno quindi codificati in maniera automatica articoli a
taglie, a peso netto, né tanto meno campionari o articoli strutturati**

Nel momento in cui l'esigenza dovesse essere quella di gestire queste
particolari tipologie di articolo, compatibilmente sempre con le
possibilità offerte dall'integrazione Passweb -- Mexal, sarà necessario
partire dal gestionale codificando quindi manualmente gli articoli
interessati per poi esportarli sulla piattaforma terza.

Per abilitare questa funzionalità è necessario agire sul parametro
"**Creare Nuovi Articoli nel Gestionale**" presente nella sezione
"**Ordini**" della maschera di configurazione "**Dati Account**",
impostandolo sul valore **SI** (per maggiori informazioni in merito alla
gestione di questo parametro si veda anche quanto indicato all'interno
del capitolo "*Altri Marketplace -- Prestashop -- Configurazione
Ordini*" di questo manuale)

![](./assets/media/image705.png)

In queste condizioni dunque nel momento in cui sull'ordine acquisto da
Prestashop dovesse essere presente un articolo non ancora codificato sul
gestionale, questo verrà creato in maniera completamente automatica
seguendo le regole di seguito indicate:

- Il **codice articolo sul gestionale** corrisponderà a quanto inserito
  su Prestashop in corrispondenza del campo "**Riferimento**"

![](./assets/media/image706.png)

> **ATTENZIONE!** per non ottenere errori in fase di codifica del nuovo
> articolo è di fondamentale importanza verificare che il numero di
> caratteri utilizzati per gestire il "Riferimento" in Prestashop, sia
> coerente con il numero di caratteri impostato per gestire i codici
> articolo sul gestionale
>
> Nel caso in cui, infatti, il codice utilizzato su Prestashop dovesse
> essere costituito da un numero di caratteri maggiore di quello
> utilizzato per gestire i codici articolo sul gestionale, l'articolo
> non potrà essere codificato e, in fase di inserimento del nuovo
> ordine, otterremo un errore.

- Nel **caso di prodotti Prestashop con combinazioni**, il codice del
  nuovo articolo inserito sul gestionale verrà costruito in maniera
  diversa dipendentemente dal fatto di aver impostato o meno un
  "Riferimento" anche per la specifica combinazione.

> In particolare nel caso in cui le combinazioni dovessero essere
> create, in Prestashop, senza indicare un riferimento allora il codice
> dell'articolo Mexal verrà creato utilizzando il "**Riferimento**"
> Prestashop dell'articolo "padre" a cui verrà però aggiunto anche il
> carattere "underscore" seguito dall'id della specifica combinazione.
> Supponendo dunque che il "Riferimento" Prestashop dell'articolo
> "padre" sia
>
> **demo_6**
>
> e che l'id assegnato da Prestashop alla specifica combinazione
> inserita in ordine sia 25 il codice gestionale del nuovo articolo sarà
> esattamente
>
> **demo_6_25**
>
> Nel momento in cui dovesse, invece, essere assegnato alla singola
> combinazione Prestashop uno specifico "Riferimento", il codice
> dell'articolo creato in Mexal corrisponderà esattamente con quanto
> indicato all'interno di questo stesso campo:

![](./assets/media/image707.png)

- La **descrizione dell'articolo sul gestionale** corrisponderà al
  **Nome Prodotto** impostato su Prestashop.

![](./assets/media/image708.png)

> Anche in questo caso è di fondamentale importanza tenere sempre in
> considerazione il numero massimo di caratteri effettivamente
> disponibili, lato gestionale, per la descrizione del prodotto
>
> **ATTENZIONE!** Nel caso in cui il Nome Prodotto impostato su
> Prestashop sia formato da un numero di caratteri maggiore rispetto a
> quelli disponibili, sul gestionale, per la descrizione del prodotto,
> tale descrizione verrà troncata

- Nel caso di **prodotti Prestashop con combinazioni** la descrizione
  dell'articolo sul gestionale corrisponderà al **Nome Prodotto**
  impostato su Prestashop seguito dal valore della specifica
  combinazione (in accordo sempre con il numero massimo di caratteri in
  uso all'interno del gestionale per la descrizione articolo)

- **L'unità di misura** dell'articolo verrà automaticamente impostata
  sul valore **pz**

- **L'aliquota IVA** assegnata all'articolo **sarà esattamente quella
  presente sull'ordine Prestashop** in relazione all'articolo stesso

- **Il prezzo** assegnato all'articolo sarà quello presente sul
  corrispondente documento Prestashop e verrà associato al listino
  definito, in Passweb, come listino di default.

> La base di calcolo nella determinazione del prezzo degli articoli
> sarà, come detto, il prezzo ritornato da Prestashop poi, nel caso in
> cui il listino impostato in Passweb come default dovesse essere:

- **Non Ivato**: il valore del prezzo coinciderà esattamente con il
  valore ritornato da Prestashop

- **Ivato**: il valore del prezzo coinciderà con il valore ritornato da
  Prestashop maggiorato dell'IVA calcolata secondo l'aliquota in uso per
  l'articolo stesso

<!-- -->

- L'articolo non verrà associato automaticamente a nessuna categoria
  merceologica ne ad alcun listino

Altra cosa di fondamentale importanza da mettere in evidenza è che
**contestualmente alla codifica di questi nuovi articoli verrà generato,
in maniera automatica, anche un documento di tipo CL (Carico
Lavorazione) in maniera tale da allineare, a livello di Esistenza, i
progressivi gestionali dell'articolo con le quantità per esso
disponibili (al momento dell'ordine) sulla piattaforma terza.**

**ATTENZIONE!** la codifica automatica degli articoli non abilita
l'articolo stesso per essere poi esportato e gestito, mediante regole di
sincronizzazione, sulla piattaforma esterna.

Prima dunque di poter fare rientrare gli articoli codificati
automaticamente nel giro dell'esportazione sulla piattaforma terza,
potendoli quindi controllare direttamente dal gestionale mediante regole
di sincronizzazione sarà necessario:

- Assegnare l'articolo ad una delle categorie merceologiche gestite
  sulla Lista di Vendita utilizzata per pubblicare i prodotti

- Impostare per l'articolo in esame il campo "Trasferisci sul sito" a S

- Verificare che prezzi e progressivi dell'articolo siano effettivamente
  quelli desiderati

**ATTENZIONE!** Nel caso in cui si dovessero far rientrare articoli
codificati automaticamente nel giro della pubblicazione su Prestashop
partendo dal gestionale, **senza aver prima verificato che i progressivi
e i prezzi impostati siano effettivamente quelli desiderati** si
correrebbe il rischio di sovrascrivere i dati presenti su Prestashop con
valori non corretti.

