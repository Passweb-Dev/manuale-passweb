# REGOLE



La sezione **"Regole"** accessibile dalla voce di menu ***"Utenti --
Utenti Sito"*** consente di definire due diverse tipologie di regole
applicabili agli utenti del sito.

- **Regole di valorizzazione degli Attributi Utente**: consentono di
  valorizzare massivamente, per gli utenti del sito che soddisfano i
  criteri di selezione impostati nella regola in esame, determinati
  Attributi Utente

> **Questo tipo di regola potrà essere applicata sia agli utenti di tipo
> "Cliente" che a quelli di tipo "Contatto"**

- **Regole di valorizzazione delle Condizioni Commerciali Utente**:
  consentono di valorizzare massivamente le condizioni commerciali degli
  utenti del sito che soddisfano i criteri di selezione impostati nella
  regola in esame

> **Questo tipo di regola potrà essere applicata solo ed esclusivamente
> agli utenti di tipo "Contatto"**

Per ogni nuova regola è quindi possibile definire:

- Uno o più filtri di selezione degli utenti attualmente gestiti sul
  sito

- Gli attributi utente / Le condizioni commerciali (dipendentemente
  dalla tipologia di regola creata) che dovranno essere coinvolti
  nell'applicazione di tale regola

- Il valore che ciascuno di questi elementi dovrà assumere per tutti gli
  utenti che andranno poi a soddisfare il filtro associato alla regola
  stessa.

I pulsanti presenti nella barra degli strumenti della maschera "**Regole
di valorizzazione**"

![](./assets/media/image78.png)

consentono rispettivamente di:

**Modifica Regola** (
![](./assets/media/image79.png) ): consente di modificare la regola attualmente
selezionata in elenco

**Elimina Regola** (
![](./assets/media/image80.png) ): consente di eliminare la regola
attualmente selezionata in elenco

**Nuova Regola** (
![](./assets/media/image81.png) ): consente di creare una nuova regola di
valorizzazione degli Attributi Utente

**Nuova Regola Condizioni** (
![](./assets/media/image82.png) ): consente di creare una nuova regola di
valorizzazione delle Condizioni Commerciali Utente

**Applica Regola** (
![](./assets/media/image83.png) ): consente di applicare manualmente la regola
attualmente selezionata in elenco

Per maggiori informazioni relativamente alle modalità di creazione delle
due diverse tipologie di Regole Utente si vedano i successivi capitoli
di questo manuale

##### REGOLE DI VALORIZZAZIONE DEGLI ATTRIBUTI UTENTE

Come evidenziato nei precedenti capitoli di questo manuale, le Regole di
valorizzazione degli Attributi Utente permettono di valorizzare
massivamente, per tutti gli utenti del sito che soddisfano i criteri di
selezione impostati nella regola in esame, gli Attributi Utente definiti
all'interno della regola stessa

Per creare una nuova Regola Utente di questo tipo sarà necessario per
prima cosa cliccare sul pulsante **Nuova Regola** (
![](./assets/media/image81.png) ) presente nella barra degli strumenti della maschera
"**Regole di valorizzazione**"

In questo modo verrà infatti visualizzata la maschera di creazione della
nuova regola

![](./assets/media/image84.png)

mediante la quale poter definire i filtri di selezione utente, gli
attributi coinvolti nella regola e i valori che questi attributi
dovranno assumere alla sua applicazione.

A questo punto sarà quindi necessario:

1.  **Decidere su quali attributi utente dovrà andare ad agire la regola
    che si sta realizzando**.

> Per fare questo sarà necessario per prima cosa selezionare gli
> attributi utente desiderati, dall'elenco presente nel box di sinistra
> della sezione "**Campi**" ed inserirli nel box di destra cliccando sul
> pulsante raffigurante una piccola freccia rivolta verso destra.
>
> Una volta definiti i campi su cui dovrà agire la regola sarà poi
> necessario cliccare sul pulsante "**Aggiorna**" in modo tale da
> inserire i campi selezionati all'interno del form sottostante.

![](./assets/media/image85.png)

2.  **Definire il criterio di selezione degli utenti del sito in
    relazione ai quali dovrà essere applicata la regola che si sta
    realizzando.**

> Dopo aver assegnato un nome identificativo alla regola (campo
> "**Nome**") sarà quindi necessario selezionare il campo o i campi su
> cui impostare il criterio di selezione degli utenti. Cliccando sul
> pulsante "**Aggiungi un nuovo filtro**" verranno visualizzati,
> all'interno di un corrispondente menu a tendina, tutti i campi che
> potranno essere utilizzati nel filtro di selezione.

![](./assets/media/image86.png)

> Per maggiori informazioni relativamente alla creazione di un filtro
> utente si veda anche la sezione *"Utenti -- Gruppi Utenti Sito --
> Filtri Utente e Filtri Articolo -- Filtri Utente"* di questo manuale
>
> **ATTENZIONE! Questo tipo di Regola Utente potrà essere applicata sia
> agli Utenti del sito di tipo "Cliente" che a quelli di tipo
> "Contatto"**

3.  **Impostare per ciascuno degli attributi selezionati al punto 1 il
    valore che questi stessi attributi dovranno assumere per gli Utenti
    che andranno poi a soddisfare il criterio di selezione impostato al
    punto2.**

> Per fare questo sarà sufficiente inserire il valore desiderato in
> corrispondenza del relativo campo presente all'interno della sezione
> "**Regola**"

![](./assets/media/image87.png)

4.  **Definire il criterio di esecuzione della regola.**

> **ATTENZIONE! Questo tipo di Regola Utente potrà essere eseguita sia
> manualmente che automaticamente**
>
> In questo senso il campo **Esecuzione Automatica** consente, se
> selezionato, di attivare l'applicazione automatica della regola.
> L'automatismo scatterà:

- ad ogni sincronizzazione (soltanto per i nuovi clienti e/o per quelli
  variati rispetto l'ultima sincronizzazione)

- ad ogni nuova registrazione utente

- ogni volta che un utente registrato apporterà delle modifiche al
  proprio profilo.

> Nel caso in cui il parametro in oggetto non venga selezionato, la
> regola dovrà invece essere necessariamente applicata in maniera
> manuale cliccando sul corrispondente pulsante (**Applica Regola**)

![](./assets/media/image88.png)

Il pulsante "**Salva**", presente nella parte bassa della maschera,
consente di salvare la regola appena creata e tornare così alla maschera
"Regole di valorizzazione" precedentemente esaminata, dove le regole con
applicazione automatica verranno evidenziate in grassetto.

**NOTA BENE:** la definizione di una regola non comporta la sua
applicazione. Per poter applicare una regola sarà necessario cliccare
sull'apposito pulsante "Applica Regola" oppure attendere la sua
applicazione automatica

##### REGOLE DI VALORIZZAZIONE DELLE CONDIZIONI COMMERCIALI UTENTE

Come evidenziato nei precedenti capitoli di questo manuale, le Regole di
valorizzazione delle Condizioni Commerciali permettono di valorizzare
massivamente, per tutti gli utenti del sito che soddisfano i criteri di
selezione impostati nella regola in esame, le Condizioni Commerciali
definite all'interno della regola stessa

**ATTENZIONE! Per ovvie ragioni questa tipologia di Regola potrà essere
applicata** **solo ed esclusivamente per utenti** **di tipo Contatto,
Contatto Non Attivo e Contatto Non Verificato.**

Per gli Utenti di tipo Cliente infatti le condizioni commerciali
dovranno essere definite e gestite direttamente all'interno del
gestionale.

Per creare una nuova Regola Utente di questo tipo sarà necessario per
prima cosa cliccare sul pulsante **Nuova Regola Condizioni**
(![](./assets/media/image82.png)) presente nella barra degli strumenti della maschera
"**Regole di valorizzazione**"

In questo modo verrà infatti visualizzata la maschera di creazione della
nuova regola

![](./assets/media/image89.png)

mediante la quale poter definire i filtri di selezione utente, i campi
delle condizioni commerciali coinvolti nella regola e i valori che
questi stessi campi dovranno assumere alla sua applicazione.

A questo punto sarà quindi necessario:

1.  **Decidere su quali campi delle condizioni commerciali dovrà andare
    ad agire la regola che si sta realizzando**.

> Per fare questo sarà necessario per prima cosa selezionare i campi
> desiderati, dall'elenco presente nel box di sinistra della sezione
> "**Campi**" ed inserirli nel box di destra cliccando sul pulsante
> raffigurante una piccola freccia rivolta verso destra (1).
>
> Una volta definiti i campi su cui dovrà agire la regola sarà poi
> necessario cliccare sul pulsante "**Aggiorna**" in modo tale da
> inserire i campi selezionati all'interno del form sottostante (2).

![](./assets/media/image90.png)

2.  **Definire il criterio di selezione degli utenti del sito in
    relazione ai quali dovrà essere applicata la regola che si sta
    realizzando.**

> Dopo aver assegnato un nome identificativo alla regola (campo
> "**Nome**") sarà quindi necessario selezionare il campo o i campi su
> cui impostare il criterio di selezione degli utenti. Cliccando sul
> pulsante "**Aggiungi un nuovo filtro**" verranno visualizzati,
> all'interno di un corrispondente menu a tendina, tutti i campi che
> potranno essere utilizzati nel filtro di selezione.

![](./assets/media/image91.png)

> Per maggiori informazioni relativamente alla creazione di un filtro
> utente si veda anche la sezione *"Utenti -- Gruppi Utenti Sito --
> Filtri Utente e Filtri Articolo -- Filtri Utente"* di questo manuale
>
> **ATTENZIONE! Questo tipo di Regola Utente potrà essere applicata dolo
> ad Utenti di tipo Contatto, Contatto Non Attivo e Contatto Non
> Verificato.**

3.  **Impostare per ciascuno dei campi selezionati al punto 1 il valore
    che questi stessi campi dovranno assumere per gli Utenti che
    andranno poi a soddisfare il criterio di selezione impostato al
    punto2.**

> Per fare questo sarà sufficiente inserire il valore desiderato in
> corrispondenza del relativo campo presente all'interno della sezione
> "**Regola**"

![](./assets/media/image92.png)

**ATTENZIONE! Le regole di valorizzazione delle condizioni commerciali
potranno essere applicate solo ed esclusivamente in maniera manuale**

Una volta definita una regola di questo tipo, per poterla poi applicare
sarà quindi necessario tornare alla maschera "Regole di valorizzazione",
selezionarla tra quelle presenti in elenco e cliccare sul pulsante
**Applica Regola** presente nella contestuale barra degli strumenti

![](./assets/media/image93.png)

