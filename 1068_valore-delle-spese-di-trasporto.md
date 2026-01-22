# VALORE DELLE SPESE DI TRASPORTO



Considerando che la gestione dei Trasporti di tipo Mexal, come
evidenziato nei precedenti capitoli di questo manuale è, di fatto,
demandata interamente al gestionale, anche il valore delle spese di
spedizione applicate sul sito nel momento in cui il cliente dovesse
scegliere come metodo di spedizione quello corrispondente al suo Vettore
Abituale, dovrà, ovviamente, essere impostato direttamente all'interno
di Mexal operando, in questo senso, dalla maschera "**Vettore / Dati di
trasporto**" accessibile, nell'anagrafica di ogni singolo cliente, dal
menu *Condizioni e automatismi -- Condizioni documenti di magazzino --
Vettore / Dati di trasporto*

![](./assets/media/image343.png)

Tra i vari parametri presenti all'interno di questa maschera troviamo
infatti anche **Tipo spese spedizione**, **Valore** e **Fino a** che
consentono rispettivamente di:

- **Tipo spese spedizione**: consente di impostare il metodo di calcolo
  delle spese di spedizione scegliendo sostanzialmente se dovranno
  essere spese fisse o in percentuale sul valore merce

- **Valore**: consente di impostare il valore da addebitare per il
  trasporto. Nel caso di spese fisse il valore immesso in questo campo
  sarà esattamente l'importo delle spese di spedizione; nel caso invece
  di calcolo in percentuale il valore immesso in questo campo
  identificherà la percentuale da calcolare sul valore totale della
  merce

- **Fino a**: consente di impostare un valore di soglia fino al quale
  dovranno essere applicate le spese indicate. Nel momento in cui il
  valore del totale merce dovesse superare la soglia indicata le spese
  di trasporto verranno azzerate.

**NOTA BENE:** per maggiori informazioni relativamente alle modalità di
gestione del vettore abituale all'interno del gestionale si consiglia di
fare riferimento alla relativa documentazione di prodotto.

In particolare per quel che riguarda l'azzeramento delle spese di
spedizione oltre una certa soglia del totale merce, occorre fare alcune
considerazioni di fondamentale importanza.

Come visto infatti, **tale soglia è impostata direttamente
sull'anagrafica del singolo cliente (non sul documento) e, soprattutto,
è vincolante all'interno del gestionale per cui, una volta impostata,
non è possibile in alcun modo bypassare il suo comportamento**

Questo significa dunque che nel momento in cui, all'interno del sito,
dovesse essere applicata una logica diversa per il calcolo delle spese
di spese di spedizione, quando poi l'ordine verrà inserito e lavorato
all'interno del gestionale, se il suo totale merce dovesse superare la
soglia impostata per il cliente, **le spese di spedizione verranno
comunque azzerate indipendentemente da quello che era il valore
originariamente calcolato per esse sul sito (e con buona probabilità
anche già pagato dal cliente)**

Per evitare problemi di questo tipo nel momento in cui si dovesse
decidere di impostare, sul gestionale, la soglia di azzeramento delle
spese di spedizione e, sul sito, di proporre ai clienti Mexal anche il
loro trasporto abituale sarà necessario:

- impostare il parametro "**Gestione del Trasporto Abituale**" presente
  alla pagina "**Configurazione parametri dell'ordine**" del Wizard sul
  valore "**Abilitato Esclusivo**" in maniera tale che il trasporto
  abituale sia, di fatto, l'unica opzione selezionabile per questi
  clienti in fase di ordine all'interno del sito

oppure

- gestire le spese di trasporto non abituali mediante l'inserimento nel
  corpo del documento di un articolo di tipo spesa. In questo modo
  infatti le spese di trasporto presenti nel piede del documento Mexal
  saranno sempre a 0 e eventuali variazioni della soglia di azzeramento
  impostata sull'anagrafica del cliente non comporteranno variazioni nei
  totali dei relativi documenti

Infine, un'altra conseguenza del fatto che la soglia di azzeramento
delle spese di spedizione non è impostata sul documento ma
sull'anagrafica dell'utente, è che nel momento in cui si dovesse per
qualche ragione modificare il suo valore, verranno automaticamente
ricalcolati anche tutti i valori delle spese di spedizione presenti su
**ordini e/o bolle** intestate a quello specifico cliente.

**In definitiva dunque una variazione della soglia di azzeramento delle
spese di trasporto potrebbe portare i totali dei documenti presenti sul
gestionale ad essere diversi da quelli presenti sul sito e comunque
diversi da quelli originariamente presentati al cliente che ha concluso
l'ordine**

**ATTENZIONE!** a differenza di ordine e bolle, **per le fatture il
valore della soglia viene salvato sul documento,** per cui un'eventuale
variazione della soglia impostata sul cliente non determinerà la
modifica dei totali delle fatture a lui intestate

Anche in questo caso, la cosa migliore da fare per evitare problemi su
eventuali ricalcoli dei totali del documento potrebbe essere quella
gestire le spese di spedizione in arrivo dal sito mediante appositi
articoli spesa inseriti nel corpo del documento.

