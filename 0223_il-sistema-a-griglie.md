# IL SISTEMA A GRIGLIE



Il **Grid System** o **Sistema a Griglia** altro non è se non un sistema
di suddivisione degli spazi di una pagina web particolarmente utile per
cerare design proporzionati, efficaci e semplici da gestire.

**In parole povere si tratta di suddividere la pagina web in un certo
numero di righe e ogni riga in un certo numero di colonne immaginarie di
dimensione fissa, separate l'una dall'altra da un certo spazio
(generalmente detto gutter) prestabilito.**

In questo modo quando dovremo decidere la dimensione (in larghezza) di
un certo elemento potremo ragionare non più in termini di pixel ma in
termini appunto di "colonne".

Un blocco di contenuti inserito all'interno di una riga non avrà più una
larghezza di 100px, ma occuperà ad esempio 1 delle N colonne in cui
avevamo pensato di suddividere la riga in esame. L'unità di misura
diventa quindi "la colonna" e l'effettiva larghezza di un blocco di
contenuti dipenderà da quante colonne occupa e da quante sono le N
colonne in cui avevamo pensato di suddividere la riga.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gr_8.png](./assets/media/image52.png){width="3.7534722222222223in"
height="2.1868055555555554in"}

Nell'esempio illustrato in figura si è pensato di suddividere:

- la prima e la quarta riga in una sola colonna.

> In queste condizioni se dovessimo decidere di posizionare all'interno
> di queste righe un blocco di contenuti e di fargli occupare una
> colonna, la sua effettiva larghezza sarà ovviamente pari al 100% e
> andrà quindi ad occupare interamente la riga in esame

- la seconda riga in due colonne.

> In queste condizioni se dovessimo decidere di posizionare all'interno
> di questa riga un blocco di contenuti e di fargli occupare una sola
> colonna, la sua effettiva larghezza sarà pari alla metà (50%) della
> riga (il contenuto verrà posizionato quindi all'interno del primo dei
> due blocchi presenti in figura). Se poi volessimo, anche in questo
> caso, fare in modo che il nostro blocco di contenuti occupi, in
> larghezza, l'intera riga dovremo allora specificare che la sua
> occupazione non è più di una ma bensì di due colonne

- la terza riga in tre colonne.

> In questo caso per fare in modo che il nostro contenuto occupi, in
> larghezza, l'intera riga, dovremo assegnargli una dimensione di 3
> colonne. Assegnandogli invece una dimensione di 2 colonne, lo spazio
> ad esso riservato sarà pari a quello individuato dai primi due blocchi
> presenti in figura.

Strutturare un layout a griglia significa quindi dare priorità ad
elementi come l'ordine, la razionalità e la proporzione tra i vari
elementi. **Fondamentale, in questo senso, risulta la fase di
progettazione che precede l'effettiva implementazione del sito**.

Ad un livello basilare e molto semplificato, sarà sufficiente approntare
un bozzetto del layout che stabilisca misure e proporzioni di quelli che
sono i due componenti fondamentali di una griglia: **le colonne e lo
spazio interno**, ovvero quello che separa una colonna dall'altra (il
gutter).

Tipicamente, in un layout a griglia le colonne potranno assumere una
larghezza variabile (pur rispondendo a precise regole di
proporzionalità), mentre lo spazio interno sarà fisso.

Sempre semplificando, sono tre le operazioni di base da compiere nella
fase di progettazione:

- definire la larghezza complessiva del layout

- impostare lo spazio che separa le colonne

- stabilire il numero di colonne che ci servono

Ora, se nel definire questi elementi si dovessero utilizzare delle
dimensioni in pixel, quello che otterremmo sarebbe pur sempre un sistema
a griglia in cui però la griglia stessa avrà delle dimensioni fisse.

Nell'ottica di realizzare un sito responsivo dovremmo invece poter
disporre di una griglia fluida in grado di adattarsi alle diverse
dimensioni dell'area di visualizzazione del documento (viewport). Per
far questo dovremo quindi, ancora una volta, da una parte utilizzare
dimensioni percentuali e dall'altra ricorre all'utilizzo delle media
query in maniera tale da poter variare il numero di colonne occupate da
un certo blocco di contenuti in relazione alle effettive dimensioni
della pagina web.

In altri termini dunque mentre su schermi di grandi dimensioni due
distinti blocchi di contenuti potrebbero, ad esempio, occupare ciascuno
2 delle 4 colonne in cui avevamo pensato di suddividere una riga,
disponendosi quindi uno a fianco dell'altro, su schermi di piccole
dimensioni questi stessi blocchi di contenuti dovranno occupare ciascuno
4 colonne in maniera tale da assumere una larghezza pari al 100%,
linearizzare il layout e disporsi uno sotto l'altro.

