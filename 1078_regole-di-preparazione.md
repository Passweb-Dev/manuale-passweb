# REGOLE DI PREPARAZIONE



Le **Regole di Preparazione** sono quelle regole utili a definire
esattamente **quando la merce sarà pronta per essere spedita**

Tali regole dovranno quindi tener conto del tempo necessario
all'azienda, una volta ricevuto l'ordine, per preparare i relativi
pacchi di spedizione, tempo questo che dovrà essere inserito, come
precedentemente evidenziato, in corrispondenza del campo "**Ore
Preparazione**" presente nella maschera di configurazione della consegna
in esame

![](./assets/media/image389.png)

Sulla base di quanto detto è semplice comprende anche che **le Regole di
Preparazione dovranno essere definite sulla base di quelli che sono gli
orari di lavoro dell'esercente** o, meglio ancora, sulla base di quelli
che sono gli orari di lavoro del reparto deputato alla preparazione dei
pacchi.

**ATTENZIONE!** Nel momento in cui per un determinato giorno non dovesse
essere impostato nessun'intervallo orario e/o nessuna specifica
esclusione, si assumerà allora che per quello stesso giorno l'orario
lavorativo del negozio (e quindi l'intervallo di tempo utile alla
preparazione del pacco) sia esattamente di 24 ore

Per definire queste regole è sufficiente selezionare la consegna
desiderata tra quelle presenti all'interno della maschera "Consegne" e
cliccare poi sul pulsante "**Regole Preparazione**" presente nella
contestuale barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Regole**"

![](./assets/media/image390.png)

contenente l'elenco di tutte le regole di preparazione attualmente
associate alla consegna in esame.

Per creare una nuova regola sarà sufficiente cliccare sul pulsante
"**Aggiungi Regola**"
(![](./assets/media/image391.png) ) in maniera tale da accedere alla
maschera "**Nuova Regola Preparazione**"

![](./assets/media/image392.png)

all'interno della quale poter specificare un valore per i seguenti
parametri:

**Nome:** consente di assegnare un nome identificativo alla regola in
maniera tale da poterla poi identificare tra le altre presenti in elenco

**Tipologia:** consente di specificare la tipologia della regola in
esame. A seconda della tipologia scelta sarà poi possibile indicare in
maniera più precisa quelli che sono gli orari e i giorni di lavoro
dell'esercente (si ricorda infatti che tali regole, tipicamente,
dovranno essere definite sulla base degli orari di lavoro
dell'esercente)

E' possibile selezionare uno dei seguenti valori:

- **Eccezione Giorno Settimanale:** selezionando questa opzione sarà poi
  possibile indicare all'interno del successivo campo "**Giorno
  Settimanale**" [il giorno esatto della settimana]{.underline} (Lunedì,
  Martedì ....) in cui il negozio sarà chiuso, giorno questo in cui non
  sarà ovviamente possibile preparare eventuali nuovi ordini per la
  spedizione.

- **Eccezione Giorno:** selezionando questa opzione sarà poi possibile
  utilizzare i successivi campi **Giorno**, **Mese** e **Anno** per
  indicare [la data di chiusura]{.underline} del negozio, data questa in
  cui non sarà ovviamente possibile preparare eventuali nuovi ordini per
  la spedizione.

> **ATTENZIONE!** I campi Giorno, Mese e Anno sono campi numerici. E
> possibile indicare anche solamente uno o due di questi elementi.
>
> Supponendo dunque di valorizzare il solo campo "Giorno" con il numero
> 3, ciò starà a significare che il 3 di tutti i mesi e di tutti gli
> anni non sarà possibile preparare per la spedizione eventuali nuovi
> ordini
>
> Allo stesso modo valorizzando solo il campo "Mese" con il valore 4 ciò
> starà a significare che per tutto il mese di Aprile di ogni anno non
> sarà possibile preparare per la spedizione eventuali nuovi ordini.
>
> Valorizzando invece il campo "Giorno" con il numero 3 e il campo
> "Mese" con il numero 4 ciò starà a significare che non sarà possibile
> preparare per la spedizione eventuali nuovi ordini il 3 Aprile di ogni
> anno.

- **Eccezione Periodo:** selezionando questa opzione sarà poi possibile
  indicare [il periodo in cui eventuali nuovi ordini non potranno essere
  preparati per la spedizione]{.underline}

> In questo caso infatti oltre ai campi "Giorno", "Mese" e "Anno", che
> consentiranno di stabilire la data di partenza del periodo verranno
> visualizzati anche 3 ulteriori campi "**Giorno Termine**", "**Mese
> Termine**" e "**Anno Termine**" mediante i quali poter stabilire
> esattamente la data di fine periodo
>
> Supponendo, ad esempio di essere in ferie tutti gli anni dal 1 a 15
> novembre sarà sufficiente indicare nei campi "Giorno" e "Mese" i
> valori 1 e 11 e nei campi "Giorno Termine" e "Mese Termine" i valori
> 15 e 11

- **Intervallo Orario:** a differenza delle tipologie precedenti,
  selezionando questa opzione sarà possibile indicare esattamente **gli
  intervalli orari in cui il negozio risulta aperto** e in cui sarà
  quindi possibile preparare eventuali nuovi ordini per la spedizione

![](./assets/media/image393.png)

> Gli intervalli orari (campi "**Ora Inizio**" e "**Ora Fine**") possono
> essere definiti in relazione ad uno specifico giorno della settimana
> (campo "**Giorno Settimanale**") piuttosto che in relazione allo
> specifico giorno di un certo mese e/o di un certo anno (campi
> "**Giorno**", "**Mese**" e "**Anno**")
>
> **ATTENZIONE!** Nel momento in cui i campi "Giorno Settimanale",
> "Giorno", "Mese", "Anno" dovessero essere lasciati vuoti gli
> intervalli indicati saranno da ritenersi sempre validi (a meno
> ovviamente di altre eccezioni indicate mediante specifiche regole)

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

**[ESEMPIO]{.underline}**

Supponiamo di dover mettere in piedi un sistema di Regole di
Preparazione che tenga conto del seguente orario lavorativo
dell'esercente

- dal lunedì al giovedì dalle 8.00 alle 13.00 e dalle 14.00 e alle 19.00

- il venerdì dalle 8.00 e le 13.00

- il sabato e la domenica chiuso

e che tenga in considerazione anche un tempo di preparazione dei pacchi
pari a 2 ore.

Per realizzare tale sistema, sarà necessario per prima cosa impostare il
parametro "**Ore Preparazione**", presente nella maschera di
configurazione della Consegna, sul valore 2. Successivamente andranno
poi codificate le seguenti regole:

- Una regola di tipo "Intervallo Orario" per ciascuna delle fasce orarie
  comprese tra le 8.00 e le 13.00 e tra le 14.00 e le 19.00 senza
  indicare in maniera specifica giorni mesi o anni

- Una regola di tipo "Intervallo Orario" per tra le 8.00 e le 13.00
  indicando in maniera specifica il giorno "Venerdì" (campo "Giorno
  Settimanale")

- Una regola di tipo "Eccezione Giorno Settimanale" indicando come
  giorno il Sabato

- Una regola di tipo "Eccezione Giorno Settimanale" indicando come
  giorno la Domenica

In queste condizioni dunque:

- Ordini acquisiti il lunedì mattina alle 10.00 saranno considerati
  pronti per la spedizione il giorno stesso alle 12

- Ordini acquisiti il lunedì mattina alle 12 saranno considerati pronti
  per la spedizione il giorno stesso alle 15. Una delle due ore
  necessarie alla preparazione verrà infatti "consumata" dalle 12 alle
  13 e l'altra dalle 14 alle 15 del giorno stesso (non verrà considerata
  l'ora dalle 13 alle 14 in cui il negozio risulta chiuso e in cui sarà
  quindi impossibile lavorare alla preparazione del pacco)

- Ordini acquisiti il venerdì mattina alle 12 saranno considerati pronti
  per la spedizione il successivo lunedì mattina alle 9. Una delle due
  ore necessarie alla preparazione verrà infatti "consumata" dalle 12
  alle 13 del giorno stesso e l'altra dalle 8 alle 9 del lunedì
  successivo (non abbiamo infatti orari lavorativi validi per poter
  completare la preparazione del pacco né il venerdì dopo le 13 né tanto
  meno il sabato o la domenica)

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Gli ulteriori pulsanti presenti nella barra degli strumenti della
maschera "Regole" consentono rispettivamente di:

**Modifica Regola**
(![](./assets/media/image394.png) ): consente di modificare la regola attualmente
selezionata

**Elimina Regola**
(![](./assets/media/image395.png) ): consente di eliminare la regola
attualmente selezionata

**Esporta**
(![](./assets/media/image367.png) ): consente di esportare tutte le regole attualmente
presenti in elenco all'interno di un apposito file csv.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Esportazione Regole**"

![](./assets/media/image396.png)

all'interno della quale poter indicare il separatore da utilizzare nella
creazione del file csv. Il pulsante "**Salva**" consente di avviare la
procedura di esportazione

**Importa da File**
(![](./assets/media/image388.png) ): consente di creare in maniera massiva,
mediante importazione di un apposito file csv, un' insieme di regole da
associare alla consegna in esame.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Importazione Regole**"

![](./assets/media/image397.png)

all'interno della quale poter configurare l'importazione dei dati in
oggetto. In particolare il campo

- **File (csv-txt)**: consente di indicare il file txt o csv contenente
  i dati relativi alle regole da creare

- **Separatore:** consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta,
consentendo a Passweb di creare le varie regole di consegna, è
necessario che il file stesso soddisfi determinate condizioni. Nello
specifico:

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- L'intestazione, ossia la prima riga del file, deve contenere i campi
  di seguito indicati:

> *tipologia;nome;giornoweek;giornostart;mesestart;annostart;orastart;giornoend;meseend;annoend;oraend*

- Per ciascun record presente nel file di importazione, i vari campi
  dovranno essere compilati tenendo in considerazione quanto di seguito
  indicato:

  - ***tipologia:*** consente di indica la tipologia di regola che dovrà
    essere creata. Sono ammessi i seguenti valori

    - **0 🡪 Eccezione Giorno Settimanale**

    - **1 🡪 Eccezione Giorno**

    - **2 🡪 Eccezione Periodo**

    - **3 🡪 Intervallo Orario**

  - ***nome:*** consente di indicare il nome descrittivo da associare
    alla regola che dovrà essere creata.

  - ***giornoweek**:* consente di indicare il giorno della settimana
    coinvolto nella regola.. Sono ammessi i seguenti valori:

    - **0 🡪 Domenica**

    - **1 🡪 Lunedì**

    - **2 🡪 Martedì**

    - **3 🡪 Mercoledì**

    - **4 🡪 Giovedì**

    - **5 🡪 Venerdì**

    - **6 🡪 Sabato**

    - 

  - ***giornostart:*** consente di indicare lo specifico giorno
    coinvolto nella regola (o quello di inizio periodo). Sono ammessi
    valori numerici da 1 a 31

  - ***mesestart**:* consente di indicare lo specifico mese coinvolto
    nella regola (o quello di inizio periodo). Sono ammessi valori
    numerici da 1 a 12

  - ***annostart**:* consente di indicare lo specifico anno coinvolto
    nella regola (o quello di inizio periodo). I valori ammessi vanno
    dall\'anno in corso fino ai 50 anni seguenti

  - ***orastart**:* consente di indicare l'orario di inizio intervallo
    (in formato h24). Sono ammessi orari del tipo HH:mm dove HH sono
    numeri da 00 a 23 e mm sono numeri da 00 a 59

  - ***giornoend**:* consente di indicare il giorno in cui termina il
    periodo coinvolto nella regola. Sono ammessi valori numerici da 1 a
    31

  - ***meseend**:* consente di indicare il mese in cui termina il
    periodo coinvolto nella regola. Sono ammessi valori numerici da 1 a
    12

  - ***annoend:*** consente di indicare l'anno in cui termina il periodo
    coinvolto nella regola. I valori ammessi vanno dall\'anno in corso
    fino ai 50 anni seguenti

  - ***oraend**:* consente di indicare l'orario di fine intervallo (in
    formato h24). Sono ammessi orari del tipo HH:mm dove HH sono numeri
    da 00 a 23 e mm sono numeri da 00 a 59

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180

**[ESEMPIO -- CARATTERE SEPARATORE ;]{.underline}**

tipologia;nome;giornoweek;giornostart;mesestart;annostart;orastart;giornoend;meseend;annoend;oraend

0;Eccezione Sabato;6;;;;;;;;

0;Eccezione Domenica;0;;;;;;;;

3;Intervallo 9-10;;;;;09:00:00;;;;10:00:00

3;Intervallo 10-11;;;;;10:00:00;;;;11:00:00

3;Intervallo 11-12;;;;;11:00:00;;;;12:00:00

3;Intervallo 13-14;;;;;13:00:00;;;;14:00:00

3;Intervallo 14-15;;;;;14:00:00;;;;15:00:00

3;Intervallo 15-16;;;;;15:00:00;;;;16:00:00

3;Intervallo 16-17;;;;;16:00:00;;;;17:00:00

3;Intervallo 17-18;;;;;17:00:00;;;;18:00:00

3;Consegne Venerdì 9-10;5;;;;09:00:00;;;;10:00:00

3;Consegne Venerdì 10-11;5;;;;10:00:00;;;;11:00:00

3;Consegne Venerdì 11-12;5;;;;11:00:00;;;;12:00:00

