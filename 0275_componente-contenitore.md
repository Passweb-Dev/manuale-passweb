# COMPONENTE CONTENITORE



Il Componente **"Contenitore"** permette all'utente di raggruppare al
suo interno diversi elementi definendo quindi una sorta di
'**raggruppamento'** dimensionabile e posizionabile all'interno della
pagina web a proprio piacimento.

> **NOTA BENE:** un Componente Contenitore altro non è se non un insieme
> di tanti componenti diversi

**A livello di markup HTML questo raggruppamento di contenuti può essere
gestito mediante un tag \< div \> tradizionale, oppure mediante uno dei
nuovi tag semantici propri del HTML5 (es. \< header \> , \< footer \>,
\< nav \> ecc...)**

Grazie a questo particolare componente è quindi possibile
spostare/copiare/replicare un insieme di elementi (definiti da altri
Componenti Passweb) senza dover ripetere l'operazione più e più volte.

Si potrebbe ad esempio utilizzare un Contenitore per realizzare la
colonna di un sito inserendo al suo interno tutti gli elementi che
dovranno effettivamente essere presenti in questa stessa colonna.
Successivamente anziché replicare ogni singolo Componente presente
all'interno del Contenitore in ogni singola pagina del sito si potrà
replicare una volta soltanto l'intero Componente Contenitore.

All'interno di Passweb è inoltre possibile arrivare a realizzare
strutture annidate di contenitori a N livelli, inserendo Componenti
Contenitore all'interno di altri Componenti Contenitore.

Questo tipo di componente può quindi essere utilizzato anche per
suddividere un Componente Contenitore più esterno in diverse sezioni
logiche, semplicemente inserendo tanti componenti Contenitore innestati
al suo interno.

In Passweb esistono poi diversi componenti che possono, a tutti gli
effetti, essere considerati come **Componenti di tipo Contenitore**.
Possono essere considerati esempi in questo senso il Componente Form, il
Componente Contenuti su Tabs, su Accordion o su Slider oltre a molti dei
"Componenti E-commerce" (Catalogo E-commerce, Offerte ecc ...) e
"Interazione Utente" che verranno esaminati nel dettaglio più avanti
all'interno di questo manuale.

> **NOTA BENE:** i componenti che possono essere inseriti all'interno di
> un Componente Contenitore o, in generale, all'interno di un componente
> di tipo contenitore, possono dipendere da eventuali componenti di tipo
> contenitore più esterni oltre che dalla specifica pagina del sito in
> cui tali componenti vengono inseriti

La logica di gestione dei contenuti, per ciascuno di questi componenti
di tipo contenitore, comunque, è esattamente la stessa di quella che
andremo ora ad analizzare per il Componente Contenitore vero e proprio.

