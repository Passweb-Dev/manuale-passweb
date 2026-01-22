# ALLINEAMENTO COMPONENTI INTERNI



L'icona "**Allineamento Componenti Interni**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\icona_allineamento_componenti_interni.bmp](./assets/media/image231.png) ) presente nel R.O.C. del componente e/o
nella barra degli strumenti dell' Albero dei Componenti consente di
impostare un allineamento automatico (verticale e/o orizzontale) **per
gli elementi di primo livello** interni al componente in esame.

**Per ovvie ragioni questo tipo di azione può essere eseguita solo ed
esclusivamente su "Componenti Contenitore", "Griglie" e "Colonne" che
hanno al loro interno altri componenti Passweb.**

**ATTENZIONE! questo tipo di allineamento (così come del resto tutti i
moderni framework responsivi) lavora sul modello Flexbox (proprietà
display dei vari elementi nella pagina impostata sul valore flex o
inline-flex) per cui per poter funzionare in maniera corretta richiede
il verificarsi di determinate condizioni che possono variare in
relazione al fatto di considerare un Contenitore piuttosto che una
Griglia o delle Colonne.**

Per le stesse ragioni (modello Flexbox e proprietà display impostata sul
valore flex o inline-flex) la compatibilità di allineamenti realizzati
mediante la funzionalità in oggetto **è garantita a partire da versioni
di Internet Explorer maggiori o uguali alla 11 oltre che ovviamente
sulle ultime versioni di Chrome, Firefox, Safari e Opera.**

Per maggiori informazioni relativamente all'utilizzo di Componenti
Contenitore, Griglie e Colonne si rimanda ai relativi capitoli di questo
manuale.

Nei successivi capitoli verranno analizzate le possibili opzioni di
allineamento automatico per quel che riguarda le Colonne di una Griglia
e i componenti interni ad un Componente Contenitore piuttosto che alle
Colonne di una Griglia.

##### ALLINEAMENTO AUTOMATICO DELLE COLONNE DI UNA GRIGLIA

Cliccando sull'icona "**Allineamento Componenti Interni**" (
![Videate\\icona_allineamento_componenti_interni.bmp](./assets/media/image232.png) ) presente sul R.O.C. di un Componente
di tipo Griglia verrà visualizzata nella parte bassa della pagina una
piccola maschera mediante la quale poter settare le varie opzioni di
allineamento automatico (orizzontale e verticale) per le colonne
presenti all'interno della griglia stessa.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento.bmp](./assets/media/image233.png)

Il menu a tendina posto nella parte alta di questa maschera permette di
impostare la proprietà "**display**" del componente griglia abilitando o
disabilitando, di fatto, l'allineamento automatico delle sue colonne.

Come evidenziato nel precedente capitolo infatti, l'allineamento
automatico delle colonne di una griglia potrà funzionare solo ed
esclusivamente nel caso in cui la proprietà display del contenitore di
tali colonne sia impostata sul valore flex o inline-flex.

E' possibile selezionare uno dei seguenti valori:

- **Visualizzazione Flex:** selezionando questa opzione:

  - la proprietà display del contenitore delle colonne della griglia
    verrà impostata sul valore **flex**

  - la griglia assumerà una larghezza pari al 100% del suo contenitore
    padre

  - ogni colonna assumerà, in relazione alla griglia, una larghezza
    definita dalle impostazioni di configurazione della colonna stessa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_7.bmp](./assets/media/image234.png)

> Tecnicamente in questa configurazione verrà assegnata la classe
> "**d-flex**" (corrispondente alla proprietà "display: flex")
> all'elemento Riga della Griglia che è, per l'appunto, l'elemento che
> contiene le varie colonne.

- **Visualizzazione Inline-Flex:** selezionando questa opzione:

  - la proprietà display del contenitore delle colonne della griglia
    verrà impostata sul valore **inline-flex**

  - la griglia assumerà una larghezza dettata dai contenuti delle varie
    colonne

  - ogni colonna assumerà, in relazione alla griglia, una larghezza
    definita dalle impostazioni di configurazione della colonna stessa

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_8.bmp](./assets/media/image235.png)

> Tecnicamente in questa configurazione verrà assegnata la classe
> "**d-inline-flex**" (corrispondente alla proprietà "display:
> inline-flex") all'elemento Riga della Griglia che è, per l'appunto,
> l'elemento che contiene le varie colonne.

- **Visualizzazione Custom:** selezionando questa opzione il contenitore
  delle colonne della griglia manterrà la sua configurazione iniziale,
  non gli verrà infatti assegnata alcuna classe particolare
  disabilitando, di fatto, le opzioni di allineamento automatico.

> In queste condizioni non sarà quindi possibile selezionare nessuna
> delle opzioni di allineamento presenti all'interno della maschera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_2.bmp](./assets/media/image236.png)

**ATTENZIONE! Condizione necessaria affinchè l'allineamento automatico
delle colonne di una griglia possa funzionare correttamente è quella di
aver impostato il menu a tendina presente nella parte alta della
maschera di allineamento sul valore "Visualizzazione Flex" oppure
"Visualizzazione Inline-Flex"**

Una volta soddisfatta tale condizione i check presenti all'interno delle
due sezioni, orizzontale e verticale, consentiranno di definire quello
che dovrà essere l'allineamento di default per le colonne della griglia.

**ATTENZIONE!** l'allineamento di default potrà poi essere modificato
agendo direttamente sulla singola colonna mediante il pulsante di
"**Allineamento Componente**". Per maggiori informazioni in merito si
veda il successivo capitolo di questo manuale.

In realtà c'è un altro aspetto da prendere in considerazione affinchè le
opzioni di allineamento automatico possano essere applicate
correttamente.

Nello specifico:

- **L'allineamento orizzontale avrà senso** e potrà quindi essere
  applicato correttamente solo nel caso in cui le colonne della griglia
  non occupino il 100% della griglia stessa

> In altri termini se avessimo, ad esempio, una griglia fatta da 3
> colonne ciascuna di larghezza pari ad 1/3 della griglia,
> l'allineamento orizzontale di tali colonne non avrebbe alcun senso.
>
> Indipendentemente dal fatto di impostare un allineamento a sinistra, a
> destra o centrato le tre colonne occuperebbero sempre l'intera
> larghezza della griglia rendendo di fatto inutile ogni tipo di
> allineamento orizzontale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_3.bmp](./assets/media/image237.png)

> Al contrario se nella stessa griglia avessimo solo due colonne
> ciascuna di larghezza pari ad un terzo della griglia allora gli
> effetti di un' allineamento orizzontale a destra, piuttosto che
> centrato o a sinistra sarebbero piuttosto evidenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_4.bmp](./assets/media/image238.png)

- Allo stesso modo **l'allineamento verticale delle colonne di una
  griglia avrà senso**, e potrà quindi essere applicato correttamente
  solo nel caso in cui l'altezza di tali colonne sia inferiore a quella
  del suo contenitore.

> In sostanza sarà dunque necessario accertarsi che l'elemento
> "**Riga**" della griglia (che è effettivamente il contenitore delle
> sue colonne) abbia un'altezza superiore a quella delle colonne stesse.
> In caso contrario qualunque sia l'opzione di allineamento verticale
> impostata l'effetto non sarebbe ovviamente evidente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_5.bmp](./assets/media/image239.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_6.bmp](./assets/media/image240.png)

Di seguito vengono indicate le possibili configurazioni di allineamento
orizzontale e verticale (per altro già piuttosto evidenti dalle piccole
figure presenti al di sotto delle relative opzioni nella maschera di
configurazione dell'allineamento).

**[POSSIBILI ALLINEAMENTI ORIZZONTALI]{.underline}**

**Allineamento automatico a sinistra:** Le colonne sono posizionate, una
a fianco all'altra a partire dal bordo sinistro della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_9.bmp](./assets/media/image241.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**justify-content-start**"

**Allineamento automatico a destra:** Le colonne sono posizionate, una a
fianco all'altra a partire dal bordo destro della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_10.bmp](./assets/media/image242.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**justify-content-end**"

**Allineamento automatico centrato:** Le colonne sono posizionate, una a
fianco all'altra a partire dal centro della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_11.bmp](./assets/media/image243.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**justify-content-center**"

**Allineamento automatico giustificato:** La prima colonna viene
posizionata sulla sinistra della griglia, l'ultima colonna sulla destra
e lo spazio residuo (differenza tra la larghezza del contenitore e la
somma delle larghezze delle colonne) viene distribuito tra le altre
colonne eventualmente presenti all'interno della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_12.bmp](./assets/media/image244.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**justify-content-between**"

**Allineamento automatico giustificato centrato:** l'eventuale spazio
residuo (differenza tra la larghezza del contenitore e la somma delle
larghezze delle colonne) viene diviso per il numero di margini (n. di
elementi x 2) e successivamente applicato ad ogni margine di ciascuna
colonna

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_13.bmp](./assets/media/image245.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**justify-content-around**"

**[POSSIBILI ALLINEAMENTI VERTICALI]{.underline}**

**Allineamento automatico in alto:** le colonne sono posizionate a
partire dal bordo alto della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_14.bmp](./assets/media/image246.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**align-items-start**"

**Allineamento automatico in basso:** le colonne sono posizionate a
partire dal bordo basso della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_15.bmp](./assets/media/image247.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**align-items-end**"

**Allineamento automatico centrato:** le colonne sono posizionate al
centro della griglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_16.bmp](./assets/media/image248.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**align-items-center**"

**Allineamento automatico baseline:** le colonne sono posizionate in
maniera tale da essere tutte allineate sulla stessa linea di base

![Videate\\opzioni_allineamento_16.bmp](./assets/media/image249.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**align-items-baseline**"

**Allineamento automatico stretch:** le colonne sono stirate in maniera
tale da occupare l'intera altezza della griglia

![Videate\\opzioni_allineamento_16.bmp](./assets/media/image248.png)

Tecnicamente, in queste condizioni verrà applicata all'elemento "Riga"
della griglia la classe "**align-items-stretch**"

##### ALLINEAMENTO DEI COMPONENTI INTERNI AD UNA COLONNA E/O AD UN CONTENITORE

Le opzioni di allineamento automatico degli elementi interni ad un
Componente Contenitore seguono esattamente le stesse logiche di gestione
di quelle che regolano l'allineamento automatico delle colonne interne
ad una griglia.

Anche in questo caso dunque la **condizione fondamentale da soddisfare
affinchè tali allineamenti possano essere applicati in maniera corretta
è che la proprietà display del Componente Contenitore sia impostata sul
valore flex o inline-flex**

In questo senso dunque cliccando sull'icona "**Allineamento Componenti
Interni**" (
![Videate\\icona_allineamento_componenti_interni.bmp](./assets/media/image232.png) ) presente sul R.O.C. di un Componente
Contenitore, verrà visualizzata, nella parte bassa della pagina, la
maschera di configurazione degli allineamenti automatici

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_19.bmp](./assets/media/image250.png)

maschera questa del tutto analoga a quella esaminata nel precedente
capitolo di questo manuale.

Il menu a tendina presente nella parte alta permette di impostare, anche
in questo caso, la proprietà "**display**" del componente contenitore
abilitando (Visualizzazione Flex / Visualizzazione Inline-Flex) o
disabilitando (Visualizzazione Custom), l'allineamento automatico dei
suoi componenti interni.

Per maggiori informazioni relativamente alle opzioni di allineamento si
rimanda al precedente capitolo di questo manuale.

Sulla base di quanto detto fino ad ora, nel momento in cui si dovesse
decidere di utilizzare per gli elementi interni a un Contenitore o alla
Colonna di una griglia un'opzione di allineamento automatico, si
dovrebbe per forza di cose assegnare al Contenitore stesso piuttosto che
alla Colonna una Visualizzazione Flex o Inline Flex.

Ora, a differenza di quanto avveniva per le colonne interne ad una
griglia, il fatto di impostare la visualizzazione Flex o Inline-flex per
un contenitore piuttosto che per una colonna avrà una ripercussione
diretta sull' effettiva larghezza e sul posizionamento di quelli che
saranno poi i componenti interni a questi stessi elementi.

**In queste condizioni infatti i componenti interni ad un Contenitore o
ad una Colonna assumeranno sempre una larghezza automatica (proprietà
width impostata sul valore auto) indipendentemente da come verrà
impostato per essi il parametro "Larghezza" presente nella maschera di
configurazione del componente stesso (sezione "Avanzate e Animazioni"),
predisponendosi dunque per poter soddisfare le opzioni di allineamento
automatico settate.**

Per la stessa ragione, in queste stesse condizioni (visualizzazione Flex
o Inline-flex dell'elemento padre), i componenti interni ad una colonna
o ad un contenitore non si posizioneranno mai su due o più righe
distinte **ma si disporranno sempre su di una stessa riga andando ad
occupare la larghezza del contenitore in maniera dinamica** sulla base
della loro larghezza, dello spazio disponibile all'interno del
contenitore e, ovviamente, delle opzioni di allineamento impostate.

