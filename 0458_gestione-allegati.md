# GESTIONE ALLEGATI



Nel momento in cui per il documento in esame dovessero essere gestiti
altri allegati oltre alla "Stampa PDF", nella parte bassa della maschera
di visualizzazione del dettaglio comparirà anche una sezione
"**Allegati**" contenente l'elenco di tutti i file attualmente allegati
al documento in esame.

![](./assets/media/image403.png)

Cliccando sul nome dell'allegato verrà avviato il download del relativo
file

**ATTENZIONE!** Nel caso in cui la risorsa da scaricare sia un file xml
generato dall'emissione di una fattura elettronica, in fase di download
verrà creato uno zip contenente l'xml della fattura stessa e un file
html mediante il quale poter visualizzare il dettaglio della fattura
elettronica utilizzando il file xsl di Passepartout. In queste
condizioni per visualizzare sul browser il dettaglio della fattura
elettronica sarà quindi necessario decomprimere l'archivio .zip ed
aprire il file con estensione .html presente al suo interno.

Inoltre, una volta attivata e configurata correttamente, sul componente
"Ordine Custom (Checkout)", la gestione degli allegati, all' interno di
questa sezione potrà comparire anche il pulsante "**Gestisci Allegati**"

![](./assets/media/image404.png)

Cliccando su questo pulsante sarà quindi possibile aggiungere nuovi
allegati, rimuovere eventuali file precedentemente allegati al documento
stesso e/o variarne la relativa nota, il tutto ovviamente sempre in
accordo con i parametri di configurazione impostati sul componente
"Ordine Custom (Checkout)".

**ATTENZIONE!** in fase di visualizzazione del dettaglio di un documento
il pulsante "Gestisci Allegati" verrà visualizzato solo ed
esclusivamente al verificarsi di almeno una delle condizioni di seguito
elencate:

- **E' consentito l'inserimento di nuovi allegati**. Il parametro
  "Inserimento Allegati ordini esistenti" deve essere selezionato e il
  numero di allegati già presenti sul documento deve essere inferiore al
  numero massimo di allegati gestibili.

- **E' ammessa la rimozione di eventuali allegati al documento**. Il
  parametro "Rimozione Allegati ordini esistenti" deve essere
  selezionato e almeno uno degli allegati presenti sul documento può
  effettivamente essere eliminato.

- **Il documento in esame ha degli allegati uplodati direttamente dagli
  utenti del sito** ed esiste quindi la possibilità di variarne la
  relativa nota.

Per quel che riguarda, nello specifico, la rimozione di eventuali
allegati è bene sottolineare che, per Siti E-commerce collegati a Mexal,
indipendentemente dal fatto di aver attivato o meno la possibilità di
rimuovere allegati, **eventuali file associati ad un ordine operando
direttamente all'interno del gestionale (e partendo quindi da
Docuvision) non potranno mai essere eliminati né tanto meno variati a
livello di titolo, descrizione e/o nota**

Allo stesso modo, e per ovvie ragioni, è bene sottolineare anche che la
gestione degli allegati riguarda solo ed esclusivamente documenti di
tipo OC/OX e PR/PX. **Su documenti di tipo Bolla, Fattura e/o Nota di
credito non sarà mai possibile, indipendentemente dalle opzioni di
configurazione del componente, rimuovere eventuali file allegati al
documento stesso né tanto meno aggiungerne di nuovi.**

