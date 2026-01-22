# REGOLE DI CONSEGNA



Le **Regole di Consegna** sono quelle regole utili a definire
esattamente **la data prevista per la consegna della merce**

Tali regole dovranno quindi tener conto necessariamente, da una parte,
di quello che è **l'orario lavorativo del Vettore utilizzato per
consegnare la merce** e, dall'altra parte, anche **del tempo che il
Vettore stesso indicherà come necessario per portare a termine la
consegna**, tempo questo che, come precedentemente evidenziato, dovrà
essere inserito in corrispondenza del campo "**Ore Consegna**" presente
nella maschera di configurazione della Consegna in esame e/o,
eventualmente, in corrispondenza del campo "**Ore aggiuntive consegna**"
presente nella maschera di configurazione della specifica zona di
spedizione merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\regole_consegna.bmp](./assets/media/image398.png){width="5.571527777777778in"
height="3.428472222222222in"}

**ATTENZIONE!** Nel momento in cui per un determinato giorno non dovesse
essere impostato nessun'intervallo orario e/o nessuna specifica
esclusione, si assumerà allora che per quello stesso giorno l'orario
lavorativo del Vettore (e quindi l'intervallo di tempo utile per portare
a termine la consegna) sia esattamente di 24 ore

**ATTENZIONE!** Nel determinare la data di prevista consegna verranno
considerate non solo le ore di consegna (in relazione all'orario
lavorativo del vettore) ma, ovviamente, anche le ore di preparazione (in
relazione all'orario lavorativo dell'esercente)

Per definire queste regole è sufficiente selezionare la consegna
desiderata tra quelle presenti all'interno della maschera "Consegne" e
cliccare poi sul pulsante "**Regole Consegna**" presente nella
contestuale barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Regole**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_regole_2.bmp](./assets/media/image399.png){width="5.792361111111111in"
height="3.545138888888889in"}

contenente l'elenco di tutte le regole attualmente associate alla
consegna in esame.

Per creare una nuova regola sarà sufficiente cliccare sul pulsante
"**Aggiungi Regola**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_regola.bmp](./assets/media/image391.png){width="0.6104166666666667in"
height="0.18194444444444444in"} ) in maniera tale da accedere alla
maschera "**Nuova Regola Consegna**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_regole_3.bmp](./assets/media/image400.png){width="5.792361111111111in"
height="3.545138888888889in"}

all'interno della quale poter specificare un valore per i seguenti
parametri:

**Nome:** consente di assegnare un nome identificativo alla regola in
maniera tale da poterla poi identificare tra le altre presenti in elenco

**Tipologia:** consente di specificare la tipologia della regola in
esame. A seconda della tipologia scelta sarà poi possibile indicare in
maniera più precisa quelli che sono gli orari e i giorni in cui il
Vettore potrà effettuare le consegne (si ricorda infatti che tali
regole, tipicamente, dovranno essere definite sulla base degli orari di
lavoro del Vettore utilizzato per portare a termine la consegna)

E' possibile selezionare uno dei seguenti valori:

- **Eccezione Giorno Settimanale:** selezionando questa opzione sarà poi
  possibile indicare all'interno del successivo campo "**Giorno
  Settimanale**" [il giorno esatto della settimana]{.underline} (Lunedì,
  Martedì ....) in cui il Vettore non lavora e in cui non potrà quindi
  essere portata a termine la consegna.

- **Eccezione Giorno:** selezionando questa opzione sarà poi possibile
  utilizzare i successivi campi **Giorno**, **Mese** e **Anno** per
  indicare [la data]{.underline} in cui il Vettore non lavora, non potrà
  quindi essere portata a termine la consegna.

> **ATTENZIONE!** I campi Giorno, Mese e Anno sono campi numerici. E
> possibile indicare anche solamente uno o due di questi elementi.
>
> Supponendo dunque di valorizzare il solo campo "Giorno" con il numero
> 3, ciò starà a significare che il Vettore non potrà effettuare
> consegne il 3 di ogni mese
>
> Allo stesso modo valorizzando solo il campo "Mese" con il valore 4 ciò
> starà a significare che non potranno essere effettuate consegne da
> parte del Vettore per tutto il mese di Aprile di ogni anno
>
> Valorizzando invece il campo "Giorno" con il numero 3 e il campo
> "Mese" con il numero 4 ciò starà a significare che non potranno essere
> effettuate consegne da parte del Vettore il 3 Aprile di ogni anno.

- **Eccezione Periodo:** selezionando questa opzione sarà poi possibile
  indicare il periodo in cui il Vettore non lavora e non potrà quindi
  portare a termine la consegna

> In questo caso infatti oltre ai campi "Giorno", "Mese" e "Anno", che
> consentiranno di stabilire la data di partenza del periodo verranno
> visualizzati anche 3 ulteriori campi "**Giorno Termine**", "**Mese
> Termine**" e "**Anno Termine**" mediante i quali poter stabilire
> esattamente la data di fine del periodo durante il quale non verranno
> effettuate consegne a domicilio
>
> Supponendo, ad esempio che il Vettore non effettui consegne tutti gli
> anni dal 1 a 15 Agosto sarà sufficiente indicare nei campi "Giorno" e
> "Mese" i valori 1 e 8 e nei campi "Giorno Termine" e "Mese Termine" i
> valori 15 e 8

- **Intervallo Orario:** a differenza delle tipologie precedenti,
  selezionando questa opzione sarà possibile indicare esattamente **gli
  intervalli orari in cui il Vettore lavora e in cui potranno quindi
  essere effettuate le consegne**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\delivery_regole_4.bmp](./assets/media/image401.png){width="5.792361111111111in"
height="3.545138888888889in"}

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
>
> Il campo "**Quota limite intervallo orario**" consente invece di
> indicare il numero massimo di consegne che potranno essere effettuate
> nell'intervallo indicato.

**ATTENZIONE!** In base alla data di consegna indicata in fase di
checkout, i possibili intervalli orari selezionabili dall'utente
verranno proposti valutando tutte le regole definite per la consegna in
esame secondo le seguenti priorità:

- giorno -- mese -- anno

- giorno -- mese

- giorno -- anno

- mese -- anno

- mese - giorno della settimana

- mese

- giorno

- giorno della settimana

- nessuna impostazione

Ciò significa dunque che per prima cosa verranno proposti intervalli
orari definiti esattamente per lo specifico giorno, mese e anno
corrispondenti alla data di consegna selezionata dall'utente.

Se non dovessero esserci intervalli definiti esattamente per quello
specifico giorno, mese e anno, verranno proposti quelli eventualmente
definiti per il giorno e il mese corrispondenti alla data di consegna
selezionata dall'utente. Se poi non dovessero esserci intervalli
definiti specificatamente neppure per quel giorno e quel mese, si
valuteranno quelli eventualmente definiti per il giorno e l'anno
corrispondenti alla data di consegna ...

Altra cosa di fondamentale importanza da tenere sempre in considerazione
è che **nel momento in cui si dovesse decidere di impostare una "Quota
limite" per tutti gli intervalli orari gestiti sarà poi necessario
accertarsi di avere impostato anche la "Quota limite giornaliera" su di
un valore pari alla somma delle singole "Quote limite orarie"**

In caso contrario infatti potrebbero verificarsi situazioni in cui
l'utente selezioni una data che risulta disponibile per la consegna,
perché non rientra in nessuna eccezione e perché non è stata impostata
nessuna "Quota limite giornaliera", senza poter poi selezionare nessun
intervallo orario perché per ciascuno di essi è stata già raggiunta la
specifica Quota limite.

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

**[ESEMPIO]{.underline}**

Supponiamo di dover mettere in piedi un sistema di Regole di Consegna
che tenga conto, in relazione al Vettore utilizzato per la spedizione,
del seguente orario lavorativo

- dal lunedì al giovedì dalle 8.00 alle 18.00

- il venerdì dalle 8.00 alle 13.00

- il sabato e la domenica non effettua consegne

e che tenga conto anche del fatto che il Vettore stesso abbia indicato
in un giorno lavorativo il tempo necessario a portare a termine (sulla
zona di spedizione considerata) la consegna.

Per realizzare tale sistema sarà necessario, per prima cosa, considerare
che il giorno lavorativo indicato dal Vettore come necessario per
portare a termine la consegna sarà, in considerazione degli orari sopra
riportati, di **10 ore** (dalle 8 alle 18 e il venerdì lavora dalle 8
alle 13 ossia mezza giornata). In conseguenza di ciò il parametro "**Ore
preparazione**", presente nella maschera di configurazione della
Consegna, dovrà essere impostato sul valore 10. Successivamente andranno
poi codificate le seguenti regole:

- Una regola di tipo "Intervallo Orario" dalle 8.00 alle 18.00 senza
  indicare in maniera specifica giorni mesi o anni

- Una regola di tipo "Intervallo Orario" dalle 8.00 alle 13.00 indicando
  in maniera specifica il giorno "Venerdì" (campo "Giorno Settimanale")

- Una regola di tipo "Eccezione Giorno Settimanale" indicando come
  giorno in cui non si effettuano consegne il Sabato

- Una regola di tipo "Eccezione Giorno Settimanale" indicando come
  giorno in cui non si effettuano consegne la Domenica

In queste condizioni, supponendo di avere un tempo di preparazione pari
a 2 ore, e supponendo anche che il negozio resti chiuso (come
nell'esempio indicato nel capitolo precedente) il venerdì pomeriggio, il
sabato e la domenica, avremo che:

- Ordini acquisiti il lunedì mattina alle 10.00 (e pronti per essere
  spediti alle 12) avranno come data di prevista consegna il martedì.
  Delle 10 ore (il giorno lavorativo indicato dal Vettore) necessarie
  per la consegna infatti 6 verranno "consumate" il giorno stesso (dalle
  12 alle 18) e le 4 restanti il giorno successivo (martedì dalle 8 alle
  12). La data esatta di prevista consegna sarebbe quindi martedì alle
  12 orario questo in cui il Vettore assicura effettivamente le consegne

- Ordini acquisiti il lunedì pomeriggio alle 17 saranno considerati
  pronti per la spedizione il giorno seguente alle 9 (delle due ore
  richieste per la preparazione una verrà usata il lunedì e una la
  mattina seguente) e la data di prevista consegna sarà quindi il
  mercoledì. Delle 10 ore (il giorno lavorativo indicato dal Vettore)
  necessarie per la consegna infatti 9 verranno "consumate" il martedì
  (dalle 9 alle 18) e l'ora restante verrà invece utilizzata il
  mercoledì (dalle 8 alle 9). La data esatta di prevista consegna
  sarebbe quindi mercoledì alle 9 orario questo in cui il Vettore
  assicura effettivamente le consegne

- Ordini acquisiti il venerdì mattina alle 11 saranno considerati pronti
  per la spedizione il giorno stesso alle 13 e la data di prevista
  consegna sarà quindi il lunedì seguente. Considerando infatti che il
  venerdì pomeriggio, il sabato e la domenica il Vettore non effettua
  consegne, le 10 ore necessarie per la consegna verranno "consumate" il
  lunedì successivo (dalle 8 alle 18). La data esatta di prevista
  consegna sarebbe quindi lunedì alle 18 orario questo in cui il Vettore
  assicura ancora le consegne

- Ordini acquisiti il venerdì pomeriggio alle 15 saranno considerati
  pronti per la spedizione il successivo lunedì mattina alle 10 (le due
  ore richieste per la preparazione verranno usate entrambe il lunedì
  seguente dalle 8 alle 10) e la data di prevista consegna sarà quindi
  mercoledì. Delle 10 ore (il giorno lavorativo indicato dal Vettore)
  necessarie per la consegna infatti 8 verranno "consumate" il lunedì
  (dalle 10 alle 18) e le due ore restanti verranno invece utilizzata il
  martedì (dalle 8 alle 10). La data esatta di prevista consegna sarebbe
  quindi martedì alle 10 orario questo in cui il Vettore assicura
  effettivamente le consegne

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Gli ulteriori pulsanti presenti nella barra degli strumenti della
maschera "Regole" consentono rispettivamente di:

**Modifica Regola**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_regola.bmp](./assets/media/image394.png){width="0.5909722222222222in"
height="0.16875in"} ): consente di modificare la regola attualmente
selezionata

**Elimina Regola**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_regola.bmp](./assets/media/image395.png){width="0.5388888888888889in"
height="0.18194444444444444in"} ): consente di eliminare la regola
attualmente selezionata

**Esporta**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta.bmp](./assets/media/image367.png){width="0.33125in"
height="0.175in"} ): consente di esportare tutte le regole attualmente
presenti in elenco all'interno di un apposito file csv.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Esportazione Regole**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\esportazione_regole.bmp](./assets/media/image396.png){width="5.792361111111111in"
height="3.545138888888889in"}

all'interno della quale poter indicare il separatore da utilizzare nella
creazione del file csv. Il pulsante "**Salva**" consente di avviare la
procedura di esportazione

**Importa da File**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_importa_da_file.bmp](./assets/media/image388.png){width="0.6166666666666667in"
height="0.1951388888888889in"} ): consente di creare in maniera massiva,
mediante importazione di un apposito file csv, un' insieme di regole da
associare alla consegna in esame.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Importazione Regole**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importazione_regole.bmp](./assets/media/image397.png){width="5.792361111111111in"
height="3.545138888888889in"}

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

> *tipologia;nome;giornoweek;giornostart;mesestart;annostart;orastart;giornoend;meseend;annoend;oraend;quotamax*

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

  - ***quotamax:*** consente di indicare il numero massimo di consegne
    che potranno essere effettuate nel relativo intervallo

- Il file di importazione deve soddisfare le specifiche del formato
  RFC4180

**[ESEMPIO -- CARATTERE SEPARATORE ;]{.underline}**

tipologia;nome;giornoweek;giornostart;mesestart;annostart;orastart;giornoend;meseend;annoend;oraend;quotamax

0;Eccezione Sabato;6;;;;;;;;;

0;Eccezione Domenica;0;;;;;;;;;

3;Intervallo 9-10;;;;;09:00:00;;;;10:00:00;1

3;Intervallo 10-11;;;;;10:00:00;;;;11:00:00;1

3;Intervallo 11-12;;;;;11:00:00;;;;12:00:00;1

3;Intervallo 13-14;;;;;13:00:00;;;;14:00:00;2

3;Intervallo 14-15;;;;;14:00:00;;;;15:00:00;2

3;Intervallo 15-16;;;;;15:00:00;;;;16:00:00;2

3;Intervallo 16-17;;;;;16:00:00;;;;17:00:00;2

3;Intervallo 17-18;;;;;17:00:00;;;;18:00:00;2

3;Consegne Venerdì 9-10;5;;;;09:00:00;;;;10:00:00;1

3;Consegne Venerdì 10-11;5;;;;10:00:00;;;;11:00:00;1

3;Consegne Venerdì 11-12;5;;;;11:00:00;;;;12:00:00;1

