# INTEGRAZIONE PASSWEB -- MAGENTO / PRESTASHOP



Nel caso in cui Passweb dovesse essere utilizzato esclusivamente come
connettore tra uno dei gestionali Passepartout (Mexal / Ho.Re.Ca.) e
Magento, l'attivazione di determinate modalità di trasporto servirà solo
ed esclusivamente per consentire di mappare i corrieri in uso su Magento
/ Prestashop con vettori utilizzati all'interno del gestionale
Passepartout.

In queste condizioni dunque il punto fondamentale nell'attivazione, lato
Passweb, di un determinato vettore sarà quello di associare ad esso, il
codice conto o la ragione sociale del vettore codificato nelle relative
anagrafiche gestionali.

Nello specifico dunque per quel che riguarda i vettori di tipo:

- **Gestionale** (solo Ecommerce Mexal): il collegamento ad un specifico
  codice conto (e quindi al relativo vettore Mexal) è insito nella
  tipologia stessa di questo vettore.

> In questo caso quindi per fare in modo che il vettore in esame possa
> poi essere tra quelli effettivamente utilizzabili per mappare uno dei
> vettori in uso su Magento / Prestashop, sarà sufficiente attivarlo
> verificando anche che il campo "**Trasporto a mezzo**" presente nel
> suo form di configurazione sia correttamente impostato sul valore
> "**Vettore**"

![](./assets/media/image353.png)

- **Passweb:** il collegamento ad uno dei vettori codificati all'interno
  del gestionale è gestito, come evidenziato nei precedenti capitoli di
  questo manuale, dai parametri "**Codice Gestionale del Vettore**", nel
  caso di collegamento con Mexal, e "**Nome del Vettore**" nel caso
  invece di collegamento con uno dei gestionali Ho.Re.Ca.

> In questo caso per fare in modo che il vettore in esame possa poi
> essere tra quelli effettivamente utilizzabili per mappare uno dei
> vettori in uso su Magento / Prestashop sarà necessario creare il
> relativo trasporto impostando i parametri di configurazione
> obbligatori come di seguito indicato:

- **Stato del Metodo di Trasporto**: Abilitato

- **Descrizione**: descrizione assegnata al Vettore che si intende
  attivare

- **Valuta di riferimento**: può essere impostato su uno qualsiasi dei
  valori presenti in elenco

- **Scaglioni e Calcolo Percentuale**: può essere impostato su uno
  qualsiasi dei valori presenti in elenco

- **Gestione Limite**: può essere impostato su uno qualsiasi dei valori
  presenti in elenco

- **Tipo di costo**: può essere impostato su uno qualsiasi dei valori
  presenti in elenco

- **Trasporto a mezzo**: deve essere impostato su **Vettore**

- **Codice Gestionale del Vettore** (Mexal): indicare il codice mastro
  di un vettore, opportunamente codificato all'interno del gestionale
  (attraverso un'apposita anagrafica fornitore)

- **Nome del Vettore** (Ho.Re.Ca.): indicare la Ragione Sociale di un
  vettore, opportunamente codificato all'interno del gestionale
  (attraverso un'apposita anagrafica fornitore)

**ATTENZIONE!** In fase di mapping dei corrieri in uso su Magento /
Prestashop con i vettori presenti sul gestionale, all' interno del campo
"**Vettore Gestionale**" verranno visualizzati solo ed esclusivamente i
trasporti a cui è stato associato uno specifico "Codice Gestionale"
(Ecommerce Mexal) o uno specifico "Nome del Vettore" (Ecommerce Horeca)

Per maggiori informazioni relativamente a come poter effettuare questa
mappatura si veda anche quanto indicato all'interno del capitolo
"*Marketplace -- Altri Marketplace -- Magento / Prestashop --
Configurazione Ordini -- Vettori*" di questo manuale.

