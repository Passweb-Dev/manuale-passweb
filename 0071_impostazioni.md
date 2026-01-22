# IMPOSTAZIONI



All'interno di questa sezione è possibile impostare i parametri di
configurazione necessari per attivare l'integrazione tra il proprio sito
Passweb e Chat GPT sbloccando così le diverse funzioni di intelligenza
artificiale generativa disponibili in diversi punti dell'applicativo.

![](./assets/media/image371.png)

Nello specifico il parametro:

- **Api Key:** consente di impostare l'API Key indispensabile per poter
  consentire la comunicazione tra il sito Passweb e i modelli di
  intelligenza artificiale messi a disposizione da Open AI

> **ATTENZIONE!** Per maggiori informazioni relativamente a come poter
> ottenere questa chiave di configurazione si faccia riferimento a
> quanto indicato all'interno del precedente capitolo di questo manuale
> ("*Come Ottenere l'API Key di OpenAI*")

- **Totale Token Utilizzati:** campo in sola visualizzazione. Mostra il
  numero di token attualmente utilizzati dal modulo Passweb AI
  consentendo quindi all'utente di farsi un'idea di quelli che saranno
  poi i costi sostenuti in relazione all'utilizzo delle API di OpenAI

> **ATTENZIONE!** Si ricorda che i costi sostenuti per la generazione
> dei contenuti mediante AI non dipendono da Passepartout ma dal listino
> della piattaforma terza e, soprattutto, dal quantitativo di dati
> (token) scambiati
>
> Per maggiori dettagli relativamente a questi costi, su come poter
> caricare del credito e su come impostare, eventualmente, dei limiti di
> utilizzo si consiglia di fare sempre riferimento a quanto indicato
> all'interno della dashboard del proprio account OpenAI

I successivi parametri **Temperatura, Maximum Tokens, Top P, Frequency
Penalty** e **Presence Penalty** consentono invece di controllare il
comportamento dei modelli di AI utilizzati rendendoli più o meno
creativi, più o meno coincisi e più o meno coerenti.

**[TEMPERATURA]{.underline}**

- **Funzionalità**: consente di regolare la casualità delle risposte
  fornite dal modello

- **Valori accettati**: da 0 a 1. Temperature più basse (es. 0.2)
  rendono le risposte più prevedibili, mentre temperature più alte (es.
  0.8 o 1) le rendono più creative.

- **Valore di default**: può variare in relazione allo specifico modello
  di AI utilizzato ma generalmente si attesta sempre sul valore 1

**[MAXIMUM TOKENS]{.underline}**

- **Funzionalità**: consente di stabilire il numero massimo di token
  (parole e frammenti di parola) che il modello potrà utilizzare per
  generare una risposta.

- **Valori accettati**: possono variare in relazione allo specifico
  modello di AI utilizzato. GPT-4, ad esempio, può gestire fino a circa
  8.000 token (o più con le versioni avanzate), mentre GPT-3.5 ha un
  limite inferiore. Ovviamente limiti più alti consentono di ottenere
  risposte più lunghe ma, di contro, comportano poi anche dei costi
  maggiori

- **Valore di default**: di default, il modello scelto genera una
  risposta completa (entro i limiti del modello stesso) se non viene
  impostato un numero massimo di token da utilizzare.

**[TOP P]{.underline}**

- **Funzionalità**: È un parametro di "campionamento del nucleo" che
  controlla il range di probabilità delle parole da cui il modello può
  scegliere.

- **Valori accettati**; da 0 a 1. Con top_p = 0.9, il modello sceglie
  dalle parole con una probabilità cumulativa del 90%, filtrando le meno
  probabili. Impostando ad esempio, un valore tra 0.8 e 0.95, si possono
  ottenere risposte meno rigide rispetto all'uso della sola temperatura.

> **ATTENZIONE!** solitamente i parametri Top P e Temperatura sono
> alternativi per cui impostarli entrambi è sconsigliato e potrebbe
> portare a risposte confuse.

- **Valore di Default**: 1. In questo modo il modello considera tutte le
  possibili parole senza filtrare in base alla probabilità cumulativa

**[FREQUENCY PENALTY]{.underline}**

- **Funzionalità**: consente di penalizzare il modello in relazione
  all'utilizzo di parole già presenti nella risposta

- **Valori accettati**: da -2 a 2. Un valore più alto (es. 1) scoraggia
  la ripetizione di parole, mentre un valore negativo può incoraggiare
  la ripetizione. Impostando un valore positivo è possibile ottenere
  risposte concise e varie (utile per evitare frasi ripetitive).

- **Valore di Default:** nullo. Non viene applicata nessun tipo di
  penalità sulla frequenza delle parole, quindi il modello non evita
  attivamente le ripetizioni.

**[PRESENCE PENALTY]{.underline}**

- **Funzionalità**: consente di penalizza il modello per l'apparizione
  di parole nuove nella risposta.

- **Valori accettati**: da -2 a 2. Valori più alti aumentano la
  probabilità che il modello esplori nuovi argomenti o concetti.
  Impostando un valore positivo è possibile ottenere risposte più varie
  o creative (ideale per generare risposte meno ripetitive e più
  originali).

- **Valore di Default:** nullo. Non viene applicata nessun tipo di
  penalità in relazione alla presenza di nuovi concetti nella risposta,
  permettendo quindi al modello di rispondere liberamente senza vincoli
  su nuove idee

**ATTENZIONE!** i parametri indicati non sono obbligatori e andrebbero
valorizzarti in maniera consapevole. **Per un utilizzo "comune" il
consiglio è quello di lasciare vuoti i relativi campi in maniera tale da
utilizzare automaticamente i valori di default**

