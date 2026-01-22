# DEFINIZIONE DELLO SCHEMA DI COLONNE



La gestione e la configurazione del Componente "Contenitore Colonna" è
leggermente diversa da quella di un qualsiasi altro Componente Passweb.

In effetti una volta inserito il Componente all'interno di una griglia,
verrà aperta in automatico la maschera "**Aggiungi Colonne**" che non
rappresenta esattamente la maschera di configurazione di una singola
colonna.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\aggiungi_colonne.bmp](./assets/media/image106.png)

**Attraverso questa maschera è infatti possibile definire esattamente lo
schema base di colonne da inserire in blocco all'interno della Griglia**

Ora, per poter comprendere ed utilizzare correttamente questa
particolare maschera di configurazione occorre mettere in evidenza
alcuni concetti di fondamentale importanza:

- Ogni riga, all'interno di una griglia è suddivisa esattamente in 12
  distinte sezioni

- La larghezza delle colonne inserite all'interno della griglia non è
  determinata in pixel o in percentuale ma in base a quante delle
  sezioni in cui risulta essere suddivisa la riga, dovranno essere
  occupate dalla colonna in esame.

> **ATTENZIONE! Per mantenere inalterato il comportamento responsivo
> della griglia occorre fare attenzione a non assegnare mai a nessuna
> colonna una specifica larghezza che sia in pixel o in percentuale o in
> qualsiasi altra unità di misura**

- Per definire il dimensionamento di una colonna viene adottata una
  convenzione basata su due numeri separati da uno slash (es. 2/12). In
  tale convenzione il secondo valore indica il numero di sezioni in cui
  è suddivisa complessivamente ogni riga di una griglia; il primo valore
  indica invece quante di queste sezioni dovranno essere occupate dalla
  colonna in esame.

> Supponendo dunque di assegnare ad una colonna un dimensionamento pari
> a 2/12 si intenderà considerare la riga suddivisa in 12 distinte
> sezioni due delle quali saranno occupate dalla colonna in esame. Le
> restanti 10 sezioni potranno essere occupate, ad esempio da altre due
> colonne entrambe dimensionate a 5/12. In queste condizioni la somma
> dei dimensionamenti delle tre colonne sarebbe infatti pari a 12/12
> (2/12 +5/12 + 5/12) che coincide effettivamente con la larghezza
> complessiva dell'intera riga.
>
> Allo stesso modo se volessimo suddividere una riga in due parti di
> ugual dimensione, dovremmo utilizzare due distinte colonne ciascuna
> dimensionata a 6/12

- Seguendo la convenzione di cui al punto precedente nel dimensionare
  una colonna sarà necessario considerare sempre che:

  - Il secondo valore dovrà essere necessariamente uguale 12

  - Il primo valore dovrà essere sempre minore o uguale a 12.

  - Nel momento in cui dovessimo inserire all'interno della griglia due
    o più colonne tutte posizionate sulla stessa riga la somma dei primi
    valori, indicati nel dimensionamento di ogni singola colonna, dovrà
    essere minore o uguale 12. Nel caso in cui si dovessero, infatti,
    inserire all'interno di una griglia tre colonne dimensionate ad
    esempio a 3/12 + 3/12 + 7/12 il risultato che otterremmo sarebbe
    quello di posizionare le prime due colonne su di una stessa riga
    lasciando alla terza uno spazio residuo di 6 sezioni. In conseguenza
    di ciò la terza colonna che dovrebbe occupare 7 di queste sezioni
    non potrà essere inserita sulla stessa riga delle prime due e verrà
    quindi posizionata su di una nuova riga.

Sulla base di quanto appena detto dovrebbe ora essere abbastanza chiaro
anche il funzionamento della maschera "**Aggiungi Colonne**"
precedentemente evidenziata.

Nello specifico infatti i campi presenti all'interno della sezione
"**Seleziona un layout**" individuano alcuni possibili schemi di colonne
preconfigurate da poter inserire in blocco all'interno della nostra
Griglia.

Supponendo dunque di voler inserire all'interno della griglia tre
colonne distinte di ugual dimensioni, sarà sufficiente cliccare sul
pulsante corrispondente allo schema "4/12 + 4/12 + 4/12" in maniera tale
da inserire questo stesso schema nel successivo campo "**Layout
Selezionato**".

Nulla vieta poi di andare a personalizzare, secondo le proprie
specifiche esigenze, e sempre seguendo le convenzioni indicate in
precedenza, lo schema di colonne da utilizzare.

Se la nostra esigenza fosse ad esempio quella di inserire all'interno
della griglia due distinte colonne una dimensionata a 4/12 e l'altra a
8/12 sarà sufficiente inserire manualmente il corrispondente schema
(4/12 + 8/12 ) all'interno del campo "Layout Selezionato".

**ATTENZIONE! Cliccando sul pulsante Salva presente nella parte alta
della maschera verrà inserito all'interno della griglia lo schema di
colonne attualmente indicato all'interno del campo "Layout
Selezionato"**

Una volta inserito all'interno della griglia un certo schema di colonne,
il passo successivo, tipicamente, è quello che prevede di andare a
configurare tali colonne definendo esattamente il dimensionamento che
ognuna di esse dovrà avere in corrispondenza delle diverse risoluzioni
del dispositivo di visualizzazione del sito.

