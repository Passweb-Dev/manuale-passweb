# GESTIONE DI UN SISTEMA DI RACCOLTA PUNTI



Una volta definite e configurate le regole sarà necessario attivare il
relativo sistema di raccolta punti cliccando sul corrispondente pulsante
(**Attiva**) presente nella barra degli strumenti della maschera
"**Raccolta Punti**" oppure flaggando il parametro di configurazione
generale "**Attivo**" precedentemente esaminato

Da questo momento in avanti, registrandosi al sito piuttosto che
portando a termine determinati ordini, gli utenti potranno accumulare
punti secondo quanto stabilito nella configurazione e nelle regole del
sistema di raccolta attualmente attivo sul sito.

I punti accumulabili per ogni articolo acquistato potranno essere
visionati direttamente in catalogo piuttosto che nella scheda del
relativo prodotto (per maggiori informazioni in merito si veda anche
quanto indicato alla sezione "*Componenti Ecommerce -- Componenti
interni ai componenti Ecommerce -- Componente Punti*" di questo manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_punti_fe.bmp](./assets/media/image395.png){width="5.454861111111111in"
height="3.279166666666667in"}

**ATTENZIONE! Il componente "Punti" visualizza sempre e soltanto il
numero di punti che si andrebbero ad accumulare nel momento in cui
l'utente dovesse decidere di acquistare quel determinato articolo in
quantità = 1**

Ogni utente avrà la possibilità di visualizzare il proprio saldo punti,
con il dettaglio delle transazioni che hanno prodotto i relativi
accumuli / sottrazioni alla pagina "**Punti Premio**" del sito (per
maggiori informazioni in merito si veda anche quanto indicato alla
sezione "*Componenti Ecommerce -- Componente Punti Premio"* di questo
manuale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\punti_premio.bmp](./assets/media/image396.png){width="5.363888888888889in"
height="3.3506944444444446in"}

In questo senso la voce:

- **Punti Guadagnati**: indica il numero di punti che, allo stato
  attuale, possono effettivamente essere utilizzati in fase di ordine

- **Punti Provvisori**: indica il numero di punti accumulati ma che non
  possono ancora essere effettivamente utilizzati (perché provenienti,
  ad esempio, da un ordine in stato di "Pagamento non confermato" per il
  quale non c'è quindi ancora la certezza del pagamento)

- **Punti Spesi**: indica il numero dei punti già utilizzati nel corso
  di precedenti ordini

- **Punti Scaduti**: indica il numero di punti, che alla data attuale,
  risultano scaduti e quindi non più utilizzabili

Inoltre in merito a quelli che sono i punti effettivamente utilizzabili
o meno in fase di ordine occorre sempre ricordare che:

- I punti accumulati potranno eventualmente essere utilizzati solo ed
  esclusivamente per ordini successivi a quelli che hanno prodotto il
  relativo accumulo

- Verranno considerati come "**Guadagnati**" e saranno quindi
  effettivamente utilizzabili solo ed esclusivamente i punti generati da
  ordini per cui si ha la certezza dell'avvenuto pagamento. Ciò
  significa che potranno quindi essere utilizzati solo ed esclusivamente
  i punti accumulati a seguito di ordini che sono stati trasformati in
  bolla o fattura

- Come conseguenza di quanto indicato al punto precedente è chiaro che:

  - I punti relativi ad ordini **in stato diverso da "Trasformato" o
    "Annullato"** verranno sempre e comunque considerati come punti
    "Provvisori"

  - Nel momento in cui si dovesse decidere di attivare una Raccolta
    punti sarà poi necessario esportare all'interno del sito le bolle /
    fatture generate da ordini Web. In caso contrario infatti il sito
    non potrà mai avere la certezza dell'avvenuto pagamento e, in
    conseguenza di ciò, la voce "Punti Guadagnati" potrebbe risultare a
    0 o comunque non indicare il numero di punti che l'utente potrebbe
    effettivamente utilizzare a seguito di ordini effettivamente pagati.

- I punti spesi per ordini che risultano essere nello stato di
  "**Pagamento non confermato / Da Verificare**" verranno eventualmente
  riaccreditati solo dopo che l'ordine sarà stato correttamente
  annullato da gestionale, da Wizard o da Sito (nel caso in cui sia
  stata attivata la possibilità di modificare gli ordini in sospeso)

Infine, anche l'amministratore del sito avrà la possibilità, operando
ovviamente dal back-end, di:

- controllare il saldo punti di ogni utente

- effettuare determinate operazioni di accredito o reset punti

- modificare la data di scadenza dei punti già acquisiti dai clienti

In questo senso i pulsanti "**Scadenza Punti**", "**Reset Punti**" e
"**Punti Utenti**" presenti nella barra degli strumenti della maschera
"Raccolta Punti" consentono rispettivamente di:

**Scadenza Punti** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_scadenza_punti.bmp](./assets/media/image365.png){width="0.5652777777777778in"
height="0.175in"} )**:** consente, all'amministratore del sito, di
modificare la scadenza dei punti già acquisiti dai singoli clienti.
Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Impostazione Data Scadenza Punti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\impostazione_data_scadenza_punti.bmp](./assets/media/image397.png){width="5.759722222222222in"
height="3.4090277777777778in"}

all'interno della quale poter indicare un valore per i seguenti
parametri:

- **Data Scadenza**: consente di impostare una specifica data di
  scadenza per i punti acquisiti dai vari clienti in relazione al
  relativo sistema di raccolta.

> **ATTENZIONE!** indicando una certa data l'effettiva scadenza sarà
> impostata alla mezzanotte del giorno successivo a quello specificato
>
> Nel momento in cui invece **il campo dovesse essere lasciato vuoto**,
> cliccando poi sul pulsante "**Applica**" la data di scadenza dei vari
> punti verrà impostata a NULL e, di fatto, **questi stessi punti non
> avranno più nessuna scadenza.**

- **Applica anche ai punti senza scadenza:** consente, se selezionato,
  di applicare l'eventuale data di scadenza impostata in corrispondenza
  del precedente parametro, anche ai punti che non hanno nessuna
  scadenza

**Reset Punti** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_reset_punti.bmp](./assets/media/image364.png){width="0.44166666666666665in"
height="0.175in"} ): consente all'amministratore del sito di azzerare e
quindi cancellare tutti i punti legati al sistema di raccolta
attualmente selezionato.

**ATTENZIONE!** Il Reset Punti è un'operazione irreversibile. Eseguito a
livello di "sistema di raccolta" avrà effetto sui punti accumulati da
ogni singolo utente del sito.

Al termine di questa procedura quindi, i punti raccolti fino a quel
momento dai vari utenti (in relazione ovviamente a quella specifica
Raccolta) verranno eliminati in maniera permanente. Volendo è comunque
possibile effettuare un'operazione analoga di reset mirata però sul
singolo utente.

**Punti Utente** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_punti_utenti.bmp](./assets/media/image398.png){width="0.5131944444444444in"
height="0.18819444444444444in"} ): consente all'amministratore del sito
di gestire i punti attualmente accumulati, in relazione al sistema di
raccolta in esame, da ogni singolo utente del sito.

Cliccando su questo pulsante si avrà infatti accesso alla maschera
"**Lista Punti Utente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_punti_utente.bmp](./assets/media/image399.png){width="5.792361111111111in"
height="3.5256944444444445in"}

dove sarà possibile visualizzare immediatamente, per ogni utente, il
relativo "Saldo Punti" (colonna "**Saldo**").

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image29.png){width="0.10416666666666667in"
height="0.12986111111111112in"} ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image30.png){width="0.12361111111111112in"
height="0.14930555555555555in"} )

L'icona raffigurante una piccola i, posta in corrispondenza di ogni riga
utente con saldo punti diverso da 0, consente di visualizzare un
dettaglio sulla ripartizione dei punti accumulati in base alla loro
scadenza

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_punti_utente_2.bmp](./assets/media/image400.png){width="5.792361111111111in"
height="3.5256944444444445in"}

I pulsanti presenti nella barra degli strumenti della maschera "Lista
Punti Utente" consentono invece di:

- **Transazioni** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_transazioni.bmp](./assets/media/image320.png){width="0.4284722222222222in"
  height="0.175in"} )**:** consente di visualizzare il dettaglio delle
  transazioni che hanno portato, per l'utente attualmente selezionato,
  al relativo Saldo Punti.

> Cliccando su questo pulsante verrà infatti visualizzata la maschera
> "**Transazioni Punti**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\transazioni_punti.bmp](./assets/media/image401.png){width="5.759722222222222in"
height="3.4090277777777778in"}

> all'interno della quale potremo trovare l'elenco di tutte le
> operazioni che hanno portato ad ottenere il relativo saldo.
>
> **ATTENZIONE!** le transazioni corrispondenti ad ordini in stato di
> "**Pagamento non confermato**" e che hanno prodotto quindi dei
> "**Punti Provvisori**" sono evidenziate in giallo
>
> Nello specifico, le operazioni in elenco possono essere di tre tipi
> diversi:

- **Accumulo punti**: evento che si verifica nel momento in cui, per
  l'utente in esame, vengono accreditati dei punti a seguito di un
  operazione effettuata sul sito (registrazione, conclusione di un
  ordine ...)

- **Sottrazione punti**: evento che si verifica nel momento in cui
  l'utente in esame deciderà di utilizzare il proprio saldo punti per
  effettuare acquisti all'interno del sito

- **Variazione amministrativa**: evento che si verifica nel momento in
  cui l'amministratore del sito dovesse decidere di variare da Wizard il
  saldo punti dell'utente in esame

> **ATTENZIONE**! Le transazioni tracciate e visualizzate all'interno di
> questa sezione del Wizard sono visibili, al relativo utente, anche sul
> front end del sito all'interno della pagina "Punti Premio".
>
> I testi descrittivi delle diverse tipologie di transazione possono
> essere personalizzati all'interno della sezione "Testi/Messaggi Sito"
> agendo sul componente "Punti Premio".
>
> I pulsanti presenti nella barra degli strumenti della maschera
> "**Transazioni Punti**" consentono invece di:

- **Elimina** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image95.png){width="0.3506944444444444in"
  height="0.18819444444444444in"} ): consente di eliminare la
  transazione attualmente selezionata in elenco

- **Modifica** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image116.png){width="0.4027777777777778in"
  height="0.18819444444444444in"} ): consente di modificare la
  transazione attualmente selezionata in elenco

> **ATTENZIONE!** per ovvie ragioni le operazioni di eliminazione e
> modifica potranno essere effettuate solo ed esclusivamente in
> relazione a transazioni corrispondenti a variazioni amministrative
> effettuate direttamente dall'amministratore sul Wizard del sito.
> Transazioni corrispondenti invece ad operazioni effettuate
> direttamente dall'utente sul front end del sito (e che hanno portato
> ad un accumulo o ad una sottrazione di punti) non potranno mai essere
> modificate da questa sezione del Wizard.

- **Aggiungi** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi.bmp](./assets/media/image362.png){width="0.43472222222222223in"
  height="0.21458333333333332in"} )**:** consente all'amministratore del
  sito di aggiungere una nuova transazione andando quindi ad incidere
  direttamente sul saldo punti del relativo cliente. Cliccando su questo
  pulsante verrà infatti visualizzata la maschera "Transazione"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\transazione.bmp](./assets/media/image402.png){width="5.759722222222222in"
height="3.4090277777777778in"}

> all'interno della quale poter indicare il numero di punti coinvolti
> nella transazione in esame (campo "**Punti**"), un eventuale data di
> scadenza per questi stessi punti (campo "**Data di Scadenza**") e un
> eventuale nota esplicativa della transazione che si sta registrando
> (campo "**Nota**").
>
> **ATTENZIONE!** il valore inserito all'interno del campo "Punti" può
> essere positivo o negativo.
>
> Nel primo caso (valore positivo) i punti indicati verranno aggiunti al
> Saldo Punti dell'utente, nel secondo caso (valore negativo) i punti
> indicati verranno invece sottratti dal Saldo attuale

- **Reset** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_reset.bmp](./assets/media/image403.png){width="0.2659722222222222in"
  height="0.175in"} ): consente di eliminare l'elenco delle transazioni
  che avevano portato al relativo Saldo Punti, resettando e quindi
  cancellando in maniera definitiva tutti i punti accumulati dall'utente
  in esame

- **Importa da file** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_da_file.bmp](./assets/media/image319.png){width="0.6236111111111111in"
  height="0.1951388888888889in"} ): consente di modificare in maniera
  massiva il saldo punti di più utenti contemporaneamente.

- **Esporta** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_testo.bmp](./assets/media/image329.png){width="0.3506944444444444in"
  height="0.18194444444444444in"} )**:** consente di esportare
  all'interno di un apposito file csv / txt il residuo punti di ciascun
  utente del sito.

**ATTENZIONE!** per maggiori informazioni relativamente alle operazioni
di importazione / esportazione massiva dei punti utente si veda anche il
successivo capitolo di questo manuale

