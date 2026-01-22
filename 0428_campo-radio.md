# CAMPO RADIO



Inserendo il componente "**Campo Radio**" all'interno del form di
Registrazione presente nel modulo di One Step Checkout, verrà aperta la
sua maschera di gestione e configurazione.

Per maggiori informazioni in merito alla gestione e alla configurazione
di un componente "Campo Radio" si veda anche il relativo capitolo di
questo manuale ("*Varianti Sito Responsive -- Lista Componenti
Interazione Utente -- Componenti Interni ai Componenti Interazione
Utente -- Campo Radio Registrazione e Profilo*")

In questo caso però oltre alle normali opzioni di configurazione
impostando il parametro "**Tipo Valore**" su "**Scelta**" e "**Tipo di
dato di Destinazione**" su "**Campo Cliente**" in corrispondenza del
successivo parametro "**Campo di Destinazione**" troveremo anche
l'opzione "**Scelta Indirizzo**"

![](./assets/media/image312.png)

**Scelta Indirizzo:** selezionando questa opzione il componente Radio
Button potrà essere utilizzato per consentire all'utente di decidere,
direttamente in fase di checkout se utilizzare o meno gli stessi dati
per l'indirizzo di fatturazione e per quello di spedizione

In questo caso all'interno del form di Registrazione dovranno dunque
essere inseriti, necessariamente, i seguenti campi:

- **Indirizzo, Località, Provincia, Nazione e CAP**, mappati come noto
  con i relativi campi dell'Anagrafica Utente gestionale e utilizzati
  per definire l'**Indirizzo di Fatturazione**

- **Indirizzo n.2 (o n.3 / n.4), Località n.2 (o n.3 / n.4), Provincia
  n.2 (o n.3 / n.4), Nazione n.2 (o n.3 / n.4), CAP n.2 (o n.3 / n.4)**
  e **Nominativo n.2 (o n.3 / n.4)**, mappati come noto con i relativi
  campi dell' Anagrafica Indirizzi di spedizione, e utilizzati dunque
  per definire uno specifico **Indirizzo di Spedizione Merce**

Nelle condizioni in esame, all'interno del form di informazioni utente
verrà quindi inserito un Radio Button con le due opzioni "Spedire a
questo indirizzo" e "Spedire ad un indirizzo diverso" che consentono
rispettivamente di:

- **Spedire a questo indirizzo:** consente, se selezionato, di
  utilizzare gli stessi dati sia per l'indirizzo di spedizione che per
  quello di fatturazione.

![](./assets/media/image313.png)

> **ATTENZIONE!** In queste condizioni i campi utilizzati per definire
> l'eventuale indirizzo di spedizione merce (Indirizzo n.2 (o n.3 /
> n.4), Località n.2 (o n.3 / n.4) ...) verranno nascosti

- **Spedire ad un indirizzo diverso:** consente, se selezionato, di
  utilizzare un indirizzo di spedizione diverso da quello di
  fatturazione. In queste condizioni verranno infatti automaticamente
  visualizzati i campi Indirizzo n.2 (o n.3 / n.4), Località n.2 (o n.3
  / n.4), Provincia n.2 (o n.3 / n.4), Nazione n.2 (o n.3 / n.4), CAP
  n.2 (o n.3 / n.4) e Nominativo n.2 (o n.3 / n.4), che, come detto
  dovranno per forza di cose essere gestiti all'interno del form, e che
  l'utente potrà ora utilizzare per indicare un indirizzo di spedizione
  merce diverso da quello di fatturazione

![](./assets/media/image314.png)

**ATTEZNIONE!** Nel caso in cui l'esigenza dovesse quindi essere quella
di permettere all'utente di decidere, direttamente in fase di checkout,
se utilizzare o meno per la fatturazione e la spedizione lo stesso
indirizzo sarà possibile utilizzare indifferentemente, all'interno del
form di Registrazione, il componente "**Campo Checkbox**" o il
componente "**Campo Radio**" configurati secondo quanto indicato in
questi capitoli

**Nel caso in cui il sito debba gestire anche delle Liste Regalo,
diventa invece obbligatorio gestire la selezione dell'indirizzo di
spedizione mediante il componente "Campo Radio".**

In queste condizioni infatti nel momento in cui l'ordine in esame
dovesse essere inerente ad una certa Lista Regalo, oltre alle due
opzioni sopra indiate comparirà anche una terza opzione "**Indirizzo del
gestore della Lista Regalo**" selezionata a default

![](./assets/media/image315.png)

che consente di utilizzare come indirizzo di spedizione merce quello
impostato direttamente dal gestore della Lista in fase di creazione
della Lista stessa.

Anche in queste condizioni l'utente che acquista per la lista regalo
avrà comunque la possibilità di variare l'impostazione di default
indicando un suo specifico indirizzo di spedizione nel caso, ad esempio,
in cui desideri farsi consegnare a casa la merce per poi recapitarla
direttamente al gestore della lista.

**ATTENZIONE!** Nel caso in cui il sito gestisca delle Liste Regalo è
indispensabile gestire, per il modulo di One Step Checkout, la selezione
dell'indirizzo di spedizione mediante il componente "Campo Radio". Il
componente "Campo Checkbox" non consente infatti di utilizzare come
indirizzo di spedizione quello impostato dal gestore della Lista

**ATTENZIONE!** nel caso in cui siano attive determinate funzionalità
(gestione iva oss, promozioni basate su determinate zone di spedizione
...) il cambiamento dell'indirizzo di spedizione potrebbe anche
comportare dei cambiamento nei totali del documento

I testi della label "Spedire a questo indirizzo", "Spedire ad un
indirizzo diverso" e "Indirizzo del gestore della Lista Regalo" sono
personalizzabili all'interno della sezione "Testi / Messaggi del Sito"
agendo in corrispondenza dei relativi parametri del componente "Checkout
Custom"

