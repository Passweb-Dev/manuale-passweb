# COMPONENTI E-COMMERCE -- TASSE



Il Componente Ecommerce **"Tasse"**

![](./assets/media/image443.png)

può essere inserito all'interno di componenti Ecommerce di primo livello
come il "Catalogo Ecommerce", la "Scheda Prodotto", le "Offerte /
Novità", "Carrello Custom" ecc... e consente di visualizzare, per
ciascun articolo, l'importo di eventuali tasse addizionali cui
l'articolo stesso è sottoposto.

![](./assets/media/image444.png)

**ATTENZIONE!** Il componente Tasse consente di visualizzare solo ed
esclusivamente gli importi di eventuali Tasse Addizionali configurate
quindi con il parametro "**Tipologia di Tassa = Tassa Extra**".

Per maggior informazioni relativamente alle diverse tipologie di tasse
gestite da Passweb si veda anche quanto indicato all'interno del
relativo capitolo di questo manuale ("*Ordini -- Tasse*")

L'importo visualizzato in corrispondenza dei vari articoli per ogni
singola tassa gestita dipende, inoltre, da come è stata configurata la
tassa stessa (dal fatto di aver impostato un tipo di costo ivato o non
ivato, dal fatto che ad effettuare l'ordine sia un'Azienda piuttosto che
un Privato, dal tipo di documento che si è scelto di generare per i
Privati piuttosto che per le Aziende, dal fatto di aver associato o meno
la Tassa a determinati gruppi di utenti ecc...)

In ogni caso **la logica di calcolo che, per una determinata tassa
extra, consente di ricavare l'importo cui dovrà essere soggetto un
determinato articolo va gestita esternamente Passweb.** L' importo
ottenuto andrà quindi inserito articolo per articolo all'interno
dell'attributo dichiarato in fase di configurazione della tassa e tale
importo verrà poi utilizzato da Passweb per determinare il prezzo
complessivo del relativo articolo.

Per maggiori informazioni in merito a come poter codificare e gestire
eventuali tasse addizionali (CONAI, RAEE, ECOTASSA ecc...) si faccia
riferimento a quanto indicato all'interno del corrispondente capitolo di
questo manuale ("*Ordini -- Tasse*")

Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image445.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di definire un nome per il Componente che si sta
  editando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Label: :** consente di impostare una label che verrà poi
  visualizzata all'interno del sito in corrispondenza del componente in
  oggetto

- **Visualizzazione Tasse:** per ogni singola tassa cui l'articolo è
  sottoposto verrà visualizzata la descrizione in lingua della relativa
  tassa (corrispondente a quanto indicato in fase di configurazione
  della tassa stessa all'interno del campo "Descrizione") e il
  corrispondente importo

> Il parametro "Visualizzazione Tasse" consente quindi di definire come
> dovranno essere visualizzati graficamente questi elementi selezionando
> una tra le seguenti opzioni: **In linea, Incolonnato**, **Tabellare**
>
> **ATTENZIONE!** Come per il componente Prezzo, anche in questo caso
> l'importo visualizzato per eventuali tasse addizionali sarà o meno
> comprensivo di IVA a seconda di chi sta effettuando l'ordine e
> soprattutto a seconda di come è stato impostato il parametro "Prezzo"
> presente all'interno della maschera "*Configurazione Catalogo*" del
> Wizard

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

