# COMPONENTE FORM -- PERSONALIZZAZIONE DEL TEMPLATE DELLE EMAIL



Come evidenziato nei precedenti capitoli di questo manuale, volendo, è
possibile configurare il Componente Form in maniera tale che al
salvataggio del form sul sito venga inviata, all'amministratore e/o
all'utente stesso, una mail di riepilogo contenente tutti i dati del
form.

In questo senso è bene sottolineare che il testo delle mail inviate da
questo componente è composto, essenzialmente, da due distinti elementi:

- Un "**Testo libero**"

- **Il dettaglio del form**, ossia i dati inseriti dall'utente sul front
  end del sito in fase di compilazione del form stesso

Per quel che riguarda il "Testo Libero", questo può essere
tranquillamente gestito all'interno del campo "**Testo Mail**"

![](./assets/media/image149.png)

campo questo presente tra i parametri di configurazione del Componente
Form, nel momento in cui si dovesse decidere di configurarlo impostando
il campo "Tipo Valore" sull'opzione "Mail"

Il campo "**Template Mail**" presente anch'esso nella maschera di
configurazione del Form, consente invece di definire e personalizzare il
Template utilizzato per la costruzione e la visualizzazione del
dettaglio del form

![](./assets/media/image150.png)

Nel momento in cui l'esigenza dovesse essere dunque, quella di
personalizzare, in relazione alle mail inviate da un Componente Form i
dati inseriti dall'utente sul front end del sito in fase di compilazione
del form stesso, sarà necessario agire sul codice HTML presente
all'interno del campo "**Template Mail**" evidenziato in figura.

Volendo è possibile aprire l'editor in modalità full screen utilizzando
il tasto funzione **F11**.

![](./assets/media/image151.png)

Una volta entrati in modalità full screen è poi possibile ritornare alla
visualizzazione standard utilizzando il tasto **ESC**.

Il pulsante "**Preview**" presente nella parte alta della maschera
consente invece di visualizzare un'anteprima del Template che si sta
realizzando, dove, ovviamente, al posto dei dati reali relativi ai campi
del form, verranno visualizzati appositi segnaposto.

In modalità Preview è possibile selezionare uno qualsiasi degli elementi
presenti all'interno del Template.

Cliccandoci sopra si passerà automaticamente alla versione
"**Sorgente**" del template con evidenziata la riga di codice relativa
all'elemento selezionato

La possibilità di intervenire direttamente sul codice HTML del template
offre, indubbiamente, ampie possibilità di personalizzazione.

**D'altra parte dovendo intervenire direttamente sul codice HTML questo
tipo di personalizzazione richiede chiaramente specifiche conoscenze
tecniche.**

In questo senso Passweb viene comunque in aiuto dell'utente in due modi
diversi.

Innanzi tutto il pulsante "**Default**" presente immediatamente al di
sotto dell'editor HTML consente di impostare una struttura di base per
il form utente, comprensiva di tutti gli elementi effettivamente
gestibili.

Inoltre nel momento in cui il template auto generato non dovesse
soddisfare le specifiche esigenze del caso, e ci fosse quindi la
necessità di integrarlo a livello di contenuti con altre informazioni
sarà possibile sfruttare uno degli appositi segnaposto messi a
disposizione da Passweb.

Una volta posizionato il cursore nel punto del template in cui dovrà
essere inserita la nuova informazione, sarà necessario cliccare sul
pulsante "**Seleziona un segnaposto ...**" in maniera tale da
visualizzare l'elenco di tutti i segnaposto disponibili.

Selezionando quindi il segnaposto desiderato tra quelli presenti in
elenco, Passweb provvederà poi ad inserire automaticamente nel template
tutto il codice necessario per gestire quello specifico tipo di
informazione

Gli elementi presenti all'interno della sezione "**Campi Form**"
consento di:

- **Etichetta:** consente di inserire nel Template del form la label dei
  vari campi

- **Valore:** consente di visualizzare nel Template del form il dato
  inserito dall'utente stesso, in fase di compilazione del form,
  all'interno dei vari campi

- **Ciclo -- Campi Form:** consente di inserire l'istruzione necessaria
  per creare un ciclo di iterazione su tutti i campi del form, in
  maniera tale quindi da non dover gestire, individualmente ogni singolo
  campo.

> Selezionando questo elemento nel Template verranno inserite le
> seguenti istruzioni
>
> **\$listValues:{**
>
> **}\$**
>
> Fatto questo andranno poi inseriti tra le due parentesi graffe i
> segnaposto relativi all'etichetta e/o al valore dei campi del form.
>
> In questo caso ovviamente tutti i campi del form verranno tratti e
> gestiti allo stesso modo

Nel caso in cui l'esigenza dovesse essere invece quella di formattare
individualmente i singoli campi del form, sarà possibile indirizzare
questi stessi campi **facendo riferimento a quanto per essi indicato in
corrispondenza del parametro "Id/Name"** presente nella loro maschera di
configurazione.

Ovviamente in queste condizioni non dovrà essere creato alcun ciclo e
ogni singolo campo del form andrà inserito e gestito manualmente
all'interno del Template

In questo senso per inserire nel Template del form la label e/o il
valore di uno specifico campo sarà necessario utilizzare i seguenti
segnaposto:

- **\$\<name\>\_key\$** - consente di inserire nel Template del form la
  label di uno specifico campo

- **\$\<name\>\_value\$** - consente di inserire nel Template del form
  il dato di uno specifico campo

dove \<name\> dovrà essere sostituito, ovviamente, con quanto indicato,
nella maschera di configurazione del relativo campo del form, in
corrispondenza del parametro "Id/Name"

![](./assets/media/image152.png)

Supponendo quindi di aver impostato, come in figura, per un determinato
campo del form, il suo parametro "Id/Name" sul valore "Nome_Utente", per
poter inserire label e dato di questo campo nel Template del form sarà
necessario utilizzare, rispettivamente, le seguenti variabili:
**\$Nome_Utente_key\$** (per la label del campo) e
**\$Nome_Utente_value\$** (per il valore del campo)

Una volta definito e personalizzato il Template da utilizzare per il
Dettaglio del Form, questo potrà poi essere inserito in una qualsiasi
posizione del corpo della relativa mail utilizzando il segnaposto
"**Dettaglio Form**", segnaposto questo attivabile cliccando sul
corrispondente pulsante presente immediatamente al di sotto del campo
"Testo Mail"

![](./assets/media/image153.png)

**ATTENZIONE!** Nel caso in cui si decida di non utilizzare nel testo di
una mail il segnaposto "Dettaglio Form" i dati del relativo form
verranno inseriti come ultimo elemento della corrispondente mail

