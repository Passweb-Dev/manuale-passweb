# IMPORTAZIONE / ESPORTAZIONE MASSIVA DEI PUNTI UTENTE



Come accennato nel precedente capitolo di questo manuale,
l'amministratore del sito, volendo, ha la possibilità di effettuare
operazioni di accredito / sottrazione dei punti accumulati dai vari
utenti operando direttamente dal Back end di Passweb.

Questo tipo di operazioni possono essere eseguite in maniera puntuale
andando a lavorare sul saldo punti del singolo utente, oppure in maniera
massiva mediante importazione di apposti file csv.

In quest'ultimo caso (importazione massiva) sarà necessario accedere
alla maschera "**Lista Punti Utente**" precedentemente analizzata e
cliccare sul pulsante "**Importa da File**" presente nella contestuale
barra degli strumenti

In questo modo verrà infatti visualizzata la maschera "**Importazione
Punti**"

![](./assets/media/image404.png)

dalla quale poter importare un file csv / txt con l'indicazione dei
punti da caricare / sottrarre al saldo attuale dei vari utenti.

Affinchè la procedura di import possa funzionare in maniera corretta
dovranno essere rispettate delle regole ben precise.

Nello specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180.

- L'intestazione, ossia la prima riga del file, dovrà contenere i
  seguenti campi (indicati esattamente come di seguito riportato):

  - utente

  - punti

  - dataScadenza

  - nota

- Coerentemente con l'intestazione del file, per ogni singolo record
  dovranno essere indicate in corrispondenza della relativa colonna le
  seguenti informazioni:

  - **utente**: identificativo dell'utente in relazione al quale si
    desidera applicare la variazione al Saldo Punti

> **ATTENZIONE!** Per consentire all'amministratore del sito di
> assegnare dei punti anche ad utenti che non sono ancora clienti, in
> corrispondenza del campo in questione **dovrà essere utilizzato
> l'identificativo Passweb e NON il codice cliente gestionale.**
>
> E' possibile ottenere l'identificativo Passweb dei vari utenti
> mediante una semplice operazione di "Esportazione Utenti" inserendo
> tra i dati di esportazione il campo "ID"
>
> **ATTENZIONE!** Nel momento in cui si dovesse decidere di non inserire
> il campo utente nel tracciato record del file di importazione, i punti
> indicati verranno assegnati indistintamente a tutti gli utenti del
> sito.
>
> Se invece si dovesse decidere di inserire il campo utente nel
> tracciato record ma poi questo non dovesse essere valorizzato in
> maniera corretta, in fase di importazione dei dati verrà restituito un
> apposito messaggio di errore.

- **punti**: numero di punti da assegnare al relativo utente. Sono
  accettati sia valori positivi che negativi. Nel primo caso i punti
  indicati andranno a sommarsi al saldo attuale del cliente, nel secondo
  caso i punti indicati verranno invece sottratti dal saldo attuale

- **dataScadenza**: data di scadenza dei relativi punti (valore
  opzionale).

> Nel momento in cui il campo in esame non dovesse essere valorizzato i
> punti indicati non avranno scadenza.
>
> Se invece si dovesse decidere di assegnare ai relativi punti una
> specifica data di scadenza, questa dovrà essere indicata nel formato
> dd/mm/yyyy

- **nota**: campo testuale (valore opzionale)

In considerazione di quanto detto e supponendo di voler utilizzare come
carattere separatore dei vari campi il carattere ; un possibile esempio
di file di importazione potrebbe essere quello qui di seguito riportato:

utente;punti;dataScadenza;nota

496;20;12/09/2021;accredito amministrativo

302;-15;;allineamento amministrativo saldo punti utente

Il pulsante **Esporta** (
![](./assets/media/image329.png) ), presente anch'esso nella barra degli
strumenti della maschera "Lista Punti Utente" consente invece di
esportare all'interno di un apposito file csv / txt il residuo punti di
ciascun utente del sito.

Cliccando sul questo pulsante verrà infatti visualizzata la maschera
"**Esportazione Punti**"

![](./assets/media/image405.png)

all'interno della quale poter indicare il carattere separatore da
utilizzare nel file di esportazione.

**Nel file di esportazione saranno presenti sempre e soltanto i seguenti
campi:**

- **utente --** identificativo Passweb dell'utente del sito

- **nominativo --** nome e cognome / Ragione Sociale dell'utente

- **punti --** valore residuo al momento dell'esportazione dei punti del
  relativo utente

Infine, oltre alle operazioni di importazione ed esportazione manuale
dei punti utente (gestite mediante i pulsanti appena analizzati), è
possibile anche automatizzare questo tipo di operazioni utilizzando in
questo senso uno degli appositi Webservices messi a disposizione da
Passweb (per maggior informazioni in merito si veda anche quanto
indicato nella sezione "*Developer*" di questo manuale)
